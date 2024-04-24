# Comparing `tmp/modgeosys_graph_algorithms-0.3.0.tar.gz` & `tmp/modgeosys_graph_algorithms-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.3.0.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.3.1.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.3.0.tar` & `modgeosys_graph_algorithms-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3165 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.3.0/README.md
--rw-r--r--   0        0        0      489 2024-04-06 23:16:09.686541 modgeosys_graph_algorithms-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.3.0/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     3088 2024-04-06 18:54:45.417423 modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     5816 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     1944 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     7683 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0    23944 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     3198 2024-04-06 22:43:36.508467 modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3364 2024-04-24 20:00:01.568472 modgeosys_graph_algorithms-0.3.1/README.md
+-rw-r--r--   0        0        0      489 2024-04-24 20:52:25.797353 modgeosys_graph_algorithms-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.3.1/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     3238 2024-04-24 19:56:19.647912 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     7716 2024-04-24 20:40:43.795506 modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     3311 2024-04-24 20:47:47.452657 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     8139 2024-04-24 20:46:32.640456 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0    23944 2024-04-06 21:44:36.374237 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     3198 2024-04-06 22:43:36.508467 modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.3.1/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.3.0/README.md` & `modgeosys_graph_algorithms-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,30 +24,32 @@
 from pprint import pprint
 
 from modgeosys.graph.types import Graph
 from modgeosys.graph.distance import manhattan_distance, euclidean_distance
 from modgeosys.graph.a_star import a_star
 
 # Define a toy graph.
-toy_graph = Graph.from_edge_definitions(((2, ((0.0, 0.0), (0.0, 2.0))),
-                                         (1, ((0.0, 0.0), (1.0, 0.0))),
-                                         (1, ((1.0, 0.0), (2.0, 1.0))),
-                                         (3, ((0.0, 2.0), (2.0, 3.0))),
-                                         (1, ((2.0, 1.0), (2.0, 3.0)))))
+toy_graph = Graph.from_edge_definitions(edge_definitions=((2, ((0.0, 0.0), (0.0, 2.0))),
+                                                          (1, ((0.0, 0.0), (1.0, 0.0))),
+                                                          (1, ((1.0, 0.0), (2.0, 1.0))),
+                                                          (3, ((0.0, 2.0), (2.0, 3.0))),
+                                                          (1, ((2.0, 1.0), (2.0, 3.0)))),
+                                        heuristic_distance_function=manhattan_distance)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
     larger_graph = pickle.load(pickled_sample_larger_graph_file)
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
 print(f'Toy A* Path:')
 pprint(toy_a_star_path)
 print()
-larger_a_star_path = a_star(graph=larger_graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+larger_a_star_path = a_star(graph=larger_graph, start_node_index=0, goal_node_index=4,
+                            heuristic_distance=manhattan_distance)
 print(f'Large A* Path:')
 pprint(larger_a_star_path)
 ```
 
 ### Prim's algorithm
 
 ```python
@@ -61,15 +63,15 @@
                                          (1, ((0.0, 0.0), (1.0, 0.0))),
                                          (1, ((1.0, 0.0), (2.0, 1.0))),
                                          (3, ((0.0, 2.0), (2.0, 3.0))),
                                          (1, ((2.0, 1.0), (2.0, 3.0)))))
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
-    larger_graph = pickle.load(pickled_sample_larger_graph_file)
+  larger_graph = pickle.load(pickled_sample_larger_graph_file)
 
 # Call the Prim function.
 toy_minimum_spanning_tree = prim(graph=toy_graph, start_node_index=0)
 print('Toy Prim Minimum Spanning Tree:')
 print(toy_minimum_spanning_tree)
 print()
 larger_minimum_spanning_tree = prim(graph=larger_graph, start_node_index=0)
```

### Comparing `modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/a_star.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,20 +33,23 @@
     def __copy__(self):
         return Hop(edge=self.edge, g=self.g, h=self.h)
 
     def __deepcopy__(self, memo: Mapping | None = None):
         return Hop(edge=self.edge, g=self.g, h=self.h)
 
 
-def a_star(graph: Graph, start_node_index: int, goal_node_index: int, heuristic_distance: HeuristicDistanceCallable) -> list[Hop]:
+def a_star(graph: Graph, start_node_index: int, goal_node_index: int) -> list[Hop]:
     """Implement the A* algorithm for finding the shortest path between two nodes in a graph."""
 
     # Grab the nodes and adjacency map from the graph.
     nodes         = graph.nodes
     adjacency_map = graph.adjacency_map()
+    heuristic_distance = graph.heuristic_distance_function
+    if not heuristic_distance:
+        raise AttributeError('The graph must have a heuristic_distance property to use the A* algorithm.')
 
     # Initialize the edge hop lists.
     unhopped   = list(graph.edges)
     hops       = []
 
     # Current node begins with the starting node.
     current_node_index = start_node_index
```

### Comparing `modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.0/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.3.1/src/modgeosys/graph/prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_a_star.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,49 +22,58 @@
 def test_hop_equality():
     hop1 = Hop(Edge(weight=10.0, node_indices=frozenset((1, 2))), g=5.0, h=5.0)
     hop2 = Hop(Edge(weight=10.0, node_indices=frozenset((1, 2))), g=5.0, h=5.0)
     assert hop1 == hop2
 
 
 def test_a_star_finds_shortest_path_manhattan_graph1(valid_graph1):
-    result = a_star(graph=valid_graph1, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+    result = a_star(graph=valid_graph1, start_node_index=0, goal_node_index=4)
 
     assert len(result) == 2
     assert result == [Hop(Edge(weight=2.0, node_indices=frozenset({0, 1})), cached_f=5.0, g=2.0, h=3.0),
                       Hop(Edge(weight=3.0, node_indices=frozenset({1, 4})), cached_f=5.0, g=5.0, h=0.0)]
 
 
 def test_a_star_find_shortest_path_manhattan_graph_from_edge_definitions(valid_graph_from_edge_definitions):
-    result = a_star(graph=valid_graph_from_edge_definitions, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+    result = a_star(graph=valid_graph_from_edge_definitions, start_node_index=0, goal_node_index=4)
 
     assert len(result) == 2
     assert result == [Hop(Edge(weight=2.0, node_indices=frozenset({0, 1})), cached_f=5.0, g=2.0, h=3.0),
                       Hop(Edge(weight=3.0, node_indices=frozenset({1, 4})), cached_f=5.0, g=5.0, h=0.0)]
 
 
 def test_a_star_finds_shortest_path_manhattan_graph2(valid_graph2):
-    result = a_star(graph=valid_graph2, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+    result = a_star(graph=valid_graph2, start_node_index=0, goal_node_index=4)
 
     assert len(result) == 3
     assert result == [Hop(Edge(weight=1.0, node_indices=frozenset({0, 2})), cached_f=5.0, g=1.0, h=4.0),
                       Hop(Edge(weight=1.0, node_indices=frozenset({2, 3})), cached_f=4.0, g=2.0, h=2.0),
                       Hop(Edge(weight=1.0, node_indices=frozenset({3, 4})), cached_f=3.0, g=3.0, h=0.0)]
 
 
+def test_a_star_finds_shortest_path_manhattan_graph3(valid_graph3):
+    result = a_star(graph=valid_graph3, start_node_index=0, goal_node_index=4)
+
+    # assert len(result) == 3
+    assert result == [Hop(edge=Edge(weight=1.0, node_indices=frozenset({0, 2}), properties={'cost_per_unit': 1}), cached_f=5.0, g=1.0, h=4.0),
+                      Hop(edge=Edge(weight=2.0, node_indices=frozenset({2, 3}), properties={'cost_per_unit': 1}), cached_f=5.0, g=3.0, h=2.0),
+                      Hop(edge=Edge(weight=2.0, node_indices=frozenset({3, 4}), properties={'cost_per_unit': 1}), cached_f=5.0, g=5.0, h=0.0)]
+
+
 def test_a_star_with_no_path_manhattan(valid_nodes):
     with pytest.raises(NoNavigablePathError):
-        a_star(graph=Graph(valid_nodes, ()), start_node_index=0, goal_node_index=3, heuristic_distance=manhattan_distance)
+        a_star(graph=Graph(nodes=valid_nodes, edges=(), heuristic_distance_function=manhattan_distance), start_node_index=0, goal_node_index=3)
 
 
 def test_a_star_with_single_node_path_manhattan():
-    assert len(a_star(graph=Graph([(0.0, 0.0)], ()), start_node_index=0, goal_node_index=0, heuristic_distance=manhattan_distance)) == 0.0
+    assert len(a_star(graph=Graph(nodes=[(0.0, 0.0)], edges=(), heuristic_distance_function=manhattan_distance), start_node_index=0, goal_node_index=0)) == 0.0
 
 
 def test_a_star_finds_shortest_path_manhattan_larger_graph(valid_graph_larger):
-    result = a_star(graph=valid_graph_larger, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+    result = a_star(graph=valid_graph_larger, start_node_index=0, goal_node_index=4)
 
     assert len(result) == 12
     assert result == [Hop(edge=Edge(weight=122.70985671734266, node_indices=frozenset({0, 15})), cached_f=1177.683043473936, g=122.70985671734266, h=1054.9731867565933),
                       Hop(edge=Edge(weight=122.70985671734266, node_indices=frozenset({0, 15})), cached_f=1181.2230308807814, g=245.41971343468532, h=935.8033174460961),
                       Hop(edge=Edge(weight=327.68612780977446, node_indices=frozenset({0, 3})), cached_f=1836.5952865003298, g=573.1058412444597, h=1263.4894452558701),
                       Hop(edge=Edge(weight=450.3598302610208, node_indices=frozenset({3, 15})), cached_f=2078.438858262074, g=1023.4656715054805, h=1054.9731867565933),
                       Hop(edge=Edge(weight=327.68612780977446, node_indices=frozenset({12, 15})), cached_f=2733.811113881623, g=1351.151799315255, h=1382.6593145663683),
@@ -79,15 +88,15 @@
 def test_a_star_finds_shortest_path_with_string_edge_weights(valid_graph_larger_with_string_edge_weights):
     assert type(valid_graph_larger_with_string_edge_weights.edges[0].weight) == str
 
     # This is the only way to test edge construction with string weights in edges pickled before the automatic weight conversion was implemented.
     for edge in valid_graph_larger_with_string_edge_weights.edges:
         edge.__post_init__()
 
-    result = a_star(graph=valid_graph_larger_with_string_edge_weights, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+    result = a_star(graph=valid_graph_larger_with_string_edge_weights, start_node_index=0, goal_node_index=4)
 
     assert len(result) == 12
     assert result == [Hop(edge=Edge(weight=122.70985671734266, node_indices=frozenset({0, 15})), cached_f=1177.683043473936, g=122.70985671734266, h=1054.9731867565933),
                       Hop(edge=Edge(weight=122.70985671734266, node_indices=frozenset({0, 15})), cached_f=1181.2230308807814, g=245.41971343468532, h=935.8033174460961),
                       Hop(edge=Edge(weight=327.68612780977446, node_indices=frozenset({0, 3})), cached_f=1836.5952865003298, g=573.1058412444597, h=1263.4894452558701),
                       Hop(edge=Edge(weight=450.3598302610208, node_indices=frozenset({3, 15})), cached_f=2078.438858262074, g=1023.4656715054805, h=1054.9731867565933),
                       Hop(edge=Edge(weight=327.68612780977446, node_indices=frozenset({12, 15})), cached_f=2733.811113881623, g=1351.151799315255, h=1382.6593145663683),
```

### Comparing `modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.0/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.3.1/tests/modgeosys/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.0/PKG-INFO` & `modgeosys_graph_algorithms-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modgeosys-graph-algorithms
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Kevin Weller
 Author-email: klweller@icloud.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: heapdict (>=1.0.1,<2.0.0)
@@ -37,30 +37,32 @@
 from pprint import pprint
 
 from modgeosys.graph.types import Graph
 from modgeosys.graph.distance import manhattan_distance, euclidean_distance
 from modgeosys.graph.a_star import a_star
 
 # Define a toy graph.
-toy_graph = Graph.from_edge_definitions(((2, ((0.0, 0.0), (0.0, 2.0))),
-                                         (1, ((0.0, 0.0), (1.0, 0.0))),
-                                         (1, ((1.0, 0.0), (2.0, 1.0))),
-                                         (3, ((0.0, 2.0), (2.0, 3.0))),
-                                         (1, ((2.0, 1.0), (2.0, 3.0)))))
+toy_graph = Graph.from_edge_definitions(edge_definitions=((2, ((0.0, 0.0), (0.0, 2.0))),
+                                                          (1, ((0.0, 0.0), (1.0, 0.0))),
+                                                          (1, ((1.0, 0.0), (2.0, 1.0))),
+                                                          (3, ((0.0, 2.0), (2.0, 3.0))),
+                                                          (1, ((2.0, 1.0), (2.0, 3.0)))),
+                                        heuristic_distance_function=manhattan_distance)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
     larger_graph = pickle.load(pickled_sample_larger_graph_file)
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
 print(f'Toy A* Path:')
 pprint(toy_a_star_path)
 print()
-larger_a_star_path = a_star(graph=larger_graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+larger_a_star_path = a_star(graph=larger_graph, start_node_index=0, goal_node_index=4,
+                            heuristic_distance=manhattan_distance)
 print(f'Large A* Path:')
 pprint(larger_a_star_path)
 ```
 
 ### Prim's algorithm
 
 ```python
@@ -74,15 +76,15 @@
                                          (1, ((0.0, 0.0), (1.0, 0.0))),
                                          (1, ((1.0, 0.0), (2.0, 1.0))),
                                          (3, ((0.0, 2.0), (2.0, 3.0))),
                                          (1, ((2.0, 1.0), (2.0, 3.0)))))
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
-    larger_graph = pickle.load(pickled_sample_larger_graph_file)
+  larger_graph = pickle.load(pickled_sample_larger_graph_file)
 
 # Call the Prim function.
 toy_minimum_spanning_tree = prim(graph=toy_graph, start_node_index=0)
 print('Toy Prim Minimum Spanning Tree:')
 print(toy_minimum_spanning_tree)
 print()
 larger_minimum_spanning_tree = prim(graph=larger_graph, start_node_index=0)
```

