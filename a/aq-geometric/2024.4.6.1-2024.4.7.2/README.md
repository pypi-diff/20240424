# Comparing `tmp/aq_geometric-2024.4.6.1.tar.gz` & `tmp/aq_geometric-2024.4.7.2.tar.gz`

## Comparing `aq_geometric-2024.4.6.1.tar` & `aq_geometric-2024.4.7.2.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/requirements.txt
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/file/__init__.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/file/local.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/filter/__init__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/filter/node_features.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/__init__.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/compute_graph.py
--rw-r--r--   0        0        0    17069 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/graphs_builder.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/edges/__init__.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/edges/compute_edges.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/__init__.py
--rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/compute_node_features.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/compute_nodes.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/reindex/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/reindex/features.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/remote/__init__.py
--rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/remote/psql.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/datasets/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/datasets/in_memory/__init__.py
--rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py
--rw-r--r--   0        0        0    26545 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/__init__.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/base_model.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/test_base_model.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/edge_conv/__init__.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/edge_conv/edge_conv.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/edge_conv/test_edge_conv.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/gcn/__init__.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/gcn/gcn.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/gcn/test_gcn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/__init__.py
--rw-r--r--   0        0        0    16043 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/transforms/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/evaluation.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/forecasts.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/station_filters.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/test_evaluation.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/test_forecasts.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/test_station_filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/config/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/config/test_remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/data/__init__.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/data/test_aq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/datasets/__init__.py
--rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/datasets/test_aq.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/LICENSE.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/README.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/pyproject.toml
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/requirements.txt
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/file/__init__.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/file/local.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/filter/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/filter/node_features.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/__init__.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/compute_graph.py
+-rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/graphs_builder.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/edges/__init__.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/edges/compute_edges.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/__init__.py
+-rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/compute_node_features.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/compute_nodes.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/reindex/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/reindex/features.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/remote/__init__.py
+-rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/remote/psql.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/datasets/in_memory/__init__.py
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/datasets/in_memory/aq_geometric_dataset.py
+-rw-r--r--   0        0        0    26545 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/datasets/on_disk/aq_geometric_dataset.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/__init__.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/base_model.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/test_base_model.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/__init__.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/edge_conv.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/test_edge_conv.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/gcn/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/gcn/gcn.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/gcn/test_gcn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/__init__.py
+-rw-r--r--   0        0        0    16080 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/evaluation.py
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/forecasts.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/station_filters.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/test_evaluation.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/test_forecasts.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/test_station_filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/data/__init__.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/data/test_aq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/datasets/test_aq.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/LICENSE.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/README.md
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/PKG-INFO
```

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/file/local.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/file/local.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/filter/node_features.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/filter/node_features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/graph/compute_graph.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/graph/compute_graph.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/graph/graphs_builder.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/graph/graphs_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         self._ready = True
         self._gen = self._generate(self.num_graphs)
 
     def _compute_nodes(self):
         # determine the leaf h3 resolution if none is provided
         if self.leaf_h3_resolution is None:
             self.leaf_h3_resolution = determine_leaf_h3_resolution(
-                stations_info_df=self._stations_info_df,
+                df=self._stations_info_df,
                 min_h3_resolution=self.min_h3_resolution,
                 verbose=self.verbose,
             )
         # compute the nodes
         nodes = get_nodes_from_df(
             stations_info_df=self._stations_info_df,
             stations_info_filters=[],  # already applied
```

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/graph/edges/compute_edges.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/graph/edges/compute_edges.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/compute_node_features.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/compute_node_features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/compute_nodes.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/compute_nodes.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/reindex/features.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/reindex/features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/data/remote/psql.py` & `aq_geometric-2024.4.7.2/aq_geometric/data/remote/psql.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py` & `aq_geometric-2024.4.7.2/aq_geometric/datasets/in_memory/aq_geometric_dataset.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py` & `aq_geometric-2024.4.7.2/aq_geometric/datasets/on_disk/aq_geometric_dataset.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/models/test_base_model.py` & `aq_geometric-2024.4.7.2/aq_geometric/models/test_base_model.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/models/edge_conv/edge_conv.py` & `aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/models/edge_conv/test_edge_conv.py` & `aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/test_edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/models/gcn/gcn.py` & `aq_geometric-2024.4.7.2/aq_geometric/models/gcn/gcn.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/models/gcn/test_gcn.py` & `aq_geometric-2024.4.7.2/aq_geometric/models/gcn/test_gcn.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py` & `aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,45 +70,40 @@
         name: str = "AqHierarchicalEdgeConvModel",
         guid: str = str(uuid.uuid4()),
         stations: Union[List, None] = None,
         features: List[str] = ["OZONE", "PM2.5", "NO2"],
         targets: List[str] = ["OZONE", "PM2.5", "NO2"],
         num_samples_in_node_feature: int = 48,
         num_samples_in_node_target: int = 12,
-        num_features_in_node_feature: int = 3,
-        num_features_in_node_target: int = 3,
         finest_resolution: int = 6,
         coarsest_resolution: int = -1,
         cheb_k: int = 2,
         verbose: bool = False,
     ):
-        super().__init__(name=name, guid=guid, stations=stations)
-        self.features = features
-        self.targets = targets
-        self.verbose = verbose
-        self.num_samples_in_node_feature = num_samples_in_node_feature
-        self.num_samples_in_node_target = num_samples_in_node_target
-        self.num_features_in_node_feature = num_features_in_node_feature
-        self.num_features_in_node_target = num_features_in_node_target
+        super().__init__(name=name, guid=guid, stations=stations, features=features, targets=targets, num_samples_in_node_feature=num_samples_in_node_feature, num_samples_in_node_target=num_samples_in_node_target)
+        self.num_features_in_node_feature = len(features)
+        self.num_features_in_node_target = len(targets)
         self.finest_resolution = finest_resolution
         self.coarsest_resolution = coarsest_resolution
         self.cheb_k = cheb_k
         self.num_resolutions_between_finest_and_coarsest = finest_resolution - coarsest_resolution
         self.edges_low_to_high_resolution = edges_low_to_high_resolution
         self.edges_high_to_low_resolution = edges_high_to_low_resolution
-        self.hidden_channels = num_samples_in_node_feature * num_features_in_node_feature
+        self.verbose = verbose
+       
+        self.hidden_channels = self.num_samples_in_node_feature * self.num_features_in_node_feature
         self.in_norm = torch.nn.LayerNorm(self.hidden_channels)  # layer norm
         self.in_mlp = Seq(Linear(self.hidden_channels, self.hidden_channels),
                           ReLU(),
                           Linear(self.hidden_channels, self.hidden_channels))
         self.max_pool = torch.nn.MaxPool1d(self.hidden_channels)  # max pool
         self.learned_pool = Linear(
             self.hidden_channels + 3, self.hidden_channels
         )  # learned pool for the 4 pooled or convolved features
-        self.out_channels = num_samples_in_node_target * num_features_in_node_target
+        self.out_channels = self.num_samples_in_node_target * self.num_features_in_node_target
         self.out_mlp = Seq(Linear(self.hidden_channels, self.out_channels))
         self.edge_conv = HierarchicalEdgeConv(self.hidden_channels)
         self.node_target_conv = ChebGraphConv(self.hidden_channels,
                                               self.hidden_channels,
                                               K=self.cheb_k)
         self.node_target_mlp = Seq(
             Linear(self.hidden_channels, self.hidden_channels), ReLU(),
@@ -212,23 +207,23 @@
         self.coarsest_resolution = model_data.get("coarsest_resolution")
         self.cheb_k = model_data.get("cheb_k")
 
         self.load_state_dict(model_data["state_dict"])
 
         # set the kwargs
         for key, value in model_data.items():
-            if key not in ["name", "guid", "stations", "state_dict"]:
+            if key not in ["name", "guid", "stations", "edges_high_to_low_resolution", "edges_low_to_high_resolution", "features", "targets", "num_samples_in_node_feature", "num_samples_in_node_target", "num_features_in_node_feature", "num_features_in_node_target", "state_dict"]:
                 setattr(self, key, value)
 
     def __repr__(self):
         """Use the torch default representation, add new attrs."""
         representation = super().__repr__()
         # add new lines with the name, guid, and stations
-        representation += f"\nSamples in Node Features: {self.num_samples_in_node_feature}"
-        representation += f"\nSamples in Node Targets: {self.num_samples_in_node_target}"
+        representation += f"\nFinest h3 resolution: {self.finest_resolution}"
+        representation += f"\Coarsest h3 resolution: {self.coarsest_resolution}"
 
         return representation
 
 
 def process_aq_geometric_dataset_edges_by_h3_resolution(
     graph: "torch_geometric.data.data.Data",
     graph_includes_root_node: bool = True,
```

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py` & `aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/utils/evaluation.py` & `aq_geometric-2024.4.7.2/aq_geometric/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/utils/forecasts.py` & `aq_geometric-2024.4.7.2/aq_geometric/utils/forecasts.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         # read from the graph used to generate forecasts
         assert len(graph.h3_index) == len(graph.aqsid)
         df = pd.DataFrame(np.stack((graph.h3_index.T, graph.aqsid.T), axis=1), columns=["h3_index", "aqsid"])
 
         # obtain the timestamps
         timestamps = forecast_df.columns.to_list()
         data = forecast_df.values
-        max_timestamp_in_samples = g.feature_end_time
+        max_timestamp_in_samples = graph.feature_end_time
         predicted_at_timestamp = pd.Timestamp.now()
 
         # prepare the data
         for i, timestamp in enumerate(timestamps):
             df["value"] = data[:, i]
             df["timestamp"] = timestamp
             df["predicted_at_timestamp"] = predicted_at_timestamp
```

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/utils/station_filters.py` & `aq_geometric-2024.4.7.2/aq_geometric/utils/station_filters.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/utils/test_evaluation.py` & `aq_geometric-2024.4.7.2/aq_geometric/utils/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/utils/test_forecasts.py` & `aq_geometric-2024.4.7.2/aq_geometric/utils/test_forecasts.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/aq_geometric/utils/test_station_filters.py` & `aq_geometric-2024.4.7.2/aq_geometric/utils/test_station_filters.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/tests/data/test_aq.py` & `aq_geometric-2024.4.7.2/tests/data/test_aq.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/tests/datasets/test_aq.py` & `aq_geometric-2024.4.7.2/tests/datasets/test_aq.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/.gitignore` & `aq_geometric-2024.4.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/LICENSE.md` & `aq_geometric-2024.4.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.6.1/pyproject.toml` & `aq_geometric-2024.4.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="aq-geometric"
-version="2024.04.06.1"
+version="2024.04.07.2"
 authors=[
     {name="Chris Jellen", email="cdjellen@gmail.com"},
 ]
 description="Geometric deep learning on air quality data."
 readme="README.md"
 requires-python=">=3.9"
 keywords=[
```

### Comparing `aq_geometric-2024.4.6.1/PKG-INFO` & `aq_geometric-2024.4.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aq-geometric
-Version: 2024.4.6.1
+Version: 2024.4.7.2
 Summary: Geometric deep learning on air quality data.
 Project-URL: homepage, https://github.com/cdjellen/aq
 Project-URL: documentation, https://github.com/cdjellen/aq
 Author-email: Chris Jellen <cdjellen@gmail.com>
 License-File: LICENSE.md
 Keywords: deep-learning,earth-systems,geometric-deep-learning,pytorch
 Classifier: License :: OSI Approved :: MIT License
```

