# Comparing `tmp/tensorflow-gnn-1.0.2rc1.tar.gz` & `tmp/tensorflow-gnn-1.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-gnn-1.0.2rc1.tar", last modified: Tue Feb  6 16:40:08 2024, max compression
+gzip compressed data, was "tensorflow-gnn-1.0.3rc0.tar", last modified: Wed Apr 24 07:02:17 2024, max compression
```

## Comparing `tensorflow-gnn-1.0.2rc1.tar` & `tensorflow-gnn-1.0.3rc0.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.869631 tensorflow-gnn-1.0.2rc1/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      304 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/AUTHORS
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2616 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11357 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/LICENSE
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      177 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/MANIFEST.in
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5317 2024-02-06 16:40:08.869631 tensorflow-gnn-1.0.2rc1/PKG-INFO
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4001 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/README.md
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2030 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/WORKSPACE
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.793623 tensorflow-gnn-1.0.2rc1/package/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      507 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/package/BUILD
--rwxr-x---   0 arnoegw  (83441) primarygroup (89939)     1651 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/package/move_generated_files.sh
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      953 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/package/tfdep.bzl
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)       38 2024-02-06 16:40:08.869631 tensorflow-gnn-1.0.2rc1/setup.cfg
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7227 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/setup.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.793623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2067 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10320 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/__init__.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.793623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/api_def/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7865 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/api_def/api_symbols_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.797623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3829 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/networkx_io.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3732 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/networkx_io_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.797623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/ogb/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/ogb/__init__.py
--rwxr-x---   0 arnoegw  (83441) primarygroup (89939)    17657 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3645 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/ogb/ogb_lib.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3291 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/triples.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1692 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/triples_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.797623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/data/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1129 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/data/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/data/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    42057 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/data/unigraph.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    33369 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/data/unigraph_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.797623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      476 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1475 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/__init__.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.801624 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/datasets/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      893 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/datasets/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11569 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/datasets/pyg_adapter.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11829 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/datasets/pyg_adapter_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.805624 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      427 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2760 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/__init__.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.813625 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6376 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7552 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/accessors.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9061 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/accessors_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    22084 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19970 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    24838 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/executor_lib.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     8659 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    12166 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/sampler.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4272 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/sampler_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5447 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/subgraph_pipeline_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7193 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    41223 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10920 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    13738 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/utils_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    68431 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/core.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    60037 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/core_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7585 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/custom_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    30090 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/eval_dag.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6353 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/eval_dag_sampling_layers_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    31067 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/eval_dag_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7924 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/ext_ops.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4740 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14347 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/ext_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6255 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9353 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/interfaces.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19588 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/link_samplers.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.813625 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/proto/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      684 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/proto/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1545 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/proto/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5972 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/proto/eval_dag.proto
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    21425 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    23256 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.825626 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    15002 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    25122 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/adjacency.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    18552 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/adjacency_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    39304 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/batching_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    33306 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/batching_utils_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11626 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/broadcast_ops.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14505 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/broadcast_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1289 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/dict_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1348 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/dict_utils_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5899 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_constants.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    57680 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_piece.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    46241 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_piece_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    77580 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6605 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_encode.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7299 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_encode_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    20531 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_io.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    31460 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_io_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    51047 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_ops.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    75964 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2815 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_pprint.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1560 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_pprint_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14184 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_random.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11873 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_random_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    88793 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2635 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_test_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6883 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/normalization_ops.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10698 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/normalization_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    27233 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/padding_ops.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26973 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/padding_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    34763 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/pool_ops.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    22600 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/pool_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7818 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/preprocessing_common.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9440 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/preprocessing_common_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    29090 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/readout.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    25988 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/readout_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    13883 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/schema_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10938 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/schema_utils_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    17518 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/schema_validation.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    17314 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/schema_validation_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5192 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tag_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4878 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tag_utils_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    21394 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tensor_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16448 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tensor_utils_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5692 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tf_internal.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.825626 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3140 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1497 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10534 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/builders.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16006 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/builders_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2889 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/initializers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2005 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/initializers_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    18257 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/keras_tensors.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    33097 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/keras_tensors_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.833627 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7507 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2104 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19666 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/convolution_base.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    15602 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/convolution_base_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6913 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/convolutions.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5456 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/convolutions_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    38608 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/graph_ops.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    55270 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/graph_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26086 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/graph_update.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9853 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/graph_update_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3044 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/item_dropout.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2994 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/item_dropout_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19451 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/map_features.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    25707 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/map_features_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11780 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/next_state.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9905 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/next_state_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2617 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/padding_ops.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6463 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/padding_ops_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2283 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/parse_example.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7217 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/parse_example_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.785622 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.837628 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3405 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2214 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7190 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/distribute_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11905 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/layers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16271 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/layers_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6593 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/losses.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6301 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/losses_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11642 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/metrics.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6024 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/metrics_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14139 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/tasks.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    17706 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/tasks_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3125 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5574 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/utils_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.837628 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2495 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1750 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2687 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/config_dict.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3051 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/config_dict_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2867 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/hparams_vizier.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1585 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    28719 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/layers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    30259 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/layers_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.837628 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1119 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1394 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14406 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/gcn_conv.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    31405 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/gcn_conv_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.841628 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1056 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1588 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    34172 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/layers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26560 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/layers_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.841628 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2355 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1557 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2354 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/config_dict.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3483 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/config_dict_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2678 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/hparams_vizier.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1498 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/hparams_vizier_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    21050 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/layers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    34740 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/layers_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.845628 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2595 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1722 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3092 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/config_dict.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4297 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/config_dict_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3615 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/hparams_vizier.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2318 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19205 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/layers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16973 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/layers_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.845628 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2523 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1863 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2793 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/config_dict.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3134 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/config_dict_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2906 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1599 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    38107 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/layers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    56176 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/layers_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.849629 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2471 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1735 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2558 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/config_dict.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2990 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2157 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1296 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5427 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/layers.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7986 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/layers_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.849629 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1086 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2139 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1023 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/examples.proto
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11712 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/graph_schema.proto
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2412 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/graph_schema.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.849629 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3056 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5715 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     8329 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/distribute_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.789623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.789623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.853629 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1582 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    17688 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/train.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2697 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3346 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.853629 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/input/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      921 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/input/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19956 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/input/datasets.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9151 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/input/datasets_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9985 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/interfaces.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26695 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/orchestration.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16235 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/orchestration_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.857630 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2474 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26104 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/classification.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16616 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/classification_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     8772 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/link_prediction.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6643 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/link_prediction_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    39843 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/regression.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26015 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/regression_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.857630 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/trainers/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      499 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/trainers/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    12935 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/trainers/keras_fit.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.857630 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4816 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14492 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/attribution.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10632 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/attribution_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2497 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/label_fns.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1324 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/model_dir.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11775 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/model_export.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    13130 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/model_export_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4324 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/padding.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2576 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/parsing.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5001 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/parsing_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2073 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/saved_model_gen_testdata.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1940 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/saved_model_load_testdata.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1873 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/strategies.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.861630 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      462 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      478 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7766 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/sampling_spec.proto
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    18498 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/sampling_spec_builder.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10322 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/sampling_spec_builder_test.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.861630 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1467 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19030 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/graph_sampler.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    22343 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/graph_sampler_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    22798 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/sampling_lib.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    32231 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/sampling_lib_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4931 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/sampling_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5293 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/sampling_utils_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2123 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/subgraph.proto
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    13473 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/subgraph.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16541 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/subgraph_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3099 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tensorflow_gnn.bzl
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.865630 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      552 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3368 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/generate_training_data.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1375 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/generate_training_data_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3926 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/print_training_data.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2080 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/print_training_data_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2700 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/sampled_stats.proto
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7984 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/sampled_stats.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1975 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/sampled_stats_test.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1742 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/validate_graph_schema.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.865630 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      571 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/BUILD
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        1 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/__init__.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4673 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/api_utils.py
--rwxr-x---   0 arnoegw  (83441) primarygroup (89939)     2149 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/test_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5696 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/tf_test_utils.py
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2272 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn/version.py
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.793623 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5317 2024-02-06 16:40:08.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/PKG-INFO
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)    12148 2024-02-06 16:40:08.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/SOURCES.txt
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        1 2024-02-06 16:40:08.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/dependency_links.txt
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      465 2024-02-06 16:40:08.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/entry_points.txt
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        1 2024-02-06 16:40:08.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/namespace_packages.txt
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)        1 2024-02-06 16:40:08.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/not-zip-safe
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      253 2024-02-06 16:40:08.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/requires.txt
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)       22 2024-02-06 16:40:08.000000 tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/top_level.txt
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.869631 tensorflow-gnn-1.0.2rc1/testdata/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      238 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/testdata/BUILD
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.869631 tensorflow-gnn-1.0.2rc1/testdata/heterogeneous/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      420 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/testdata/heterogeneous/BUILD
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.869631 tensorflow-gnn-1.0.2rc1/testdata/homogeneous/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      294 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/testdata/homogeneous/BUILD
-drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-02-06 16:40:08.869631 tensorflow-gnn-1.0.2rc1/testdata/node_vs_edge/
--rw-r-----   0 arnoegw  (83441) primarygroup (89939)      366 2024-02-06 16:33:35.000000 tensorflow-gnn-1.0.2rc1/testdata/node_vs_edge/BUILD
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.609701 tensorflow-gnn-1.0.3rc0/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      304 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/AUTHORS
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2616 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11357 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/LICENSE
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      177 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/MANIFEST.in
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5494 2024-04-24 07:02:17.609701 tensorflow-gnn-1.0.3rc0/PKG-INFO
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4178 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/README.md
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2030 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/WORKSPACE
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.525692 tensorflow-gnn-1.0.3rc0/package/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      507 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/package/BUILD
+-rwxr-x---   0 arnoegw  (83441) primarygroup (89939)     1651 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/package/move_generated_files.sh
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      953 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/package/tfdep.bzl
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)       38 2024-04-24 07:02:17.609701 tensorflow-gnn-1.0.3rc0/setup.cfg
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7217 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/setup.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.525692 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2067 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10561 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/__init__.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.525692 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/api_def/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7865 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/api_def/api_symbols_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.529692 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3829 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/networkx_io.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3732 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/networkx_io_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.529692 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/ogb/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/ogb/__init__.py
+-rwxr-x---   0 arnoegw  (83441) primarygroup (89939)    17657 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3645 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/ogb/ogb_lib.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3291 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/triples.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1692 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/triples_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.529692 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/data/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1129 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/data/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/data/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    42057 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/data/unigraph.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    33369 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/data/unigraph_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.529692 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      476 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1475 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/__init__.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.529692 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/datasets/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      893 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/datasets/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11569 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/datasets/pyg_adapter.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11829 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/datasets/pyg_adapter_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.533693 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      427 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2760 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/__init__.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.537693 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6376 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7552 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/accessors.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9061 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/accessors_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    22084 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19970 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    24838 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     8659 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    12166 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/sampler.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4272 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/sampler_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5447 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/subgraph_pipeline_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7193 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    41223 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10920 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    13738 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/utils_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    68431 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/core.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    60037 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/core_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7585 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/custom_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    30090 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/eval_dag.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6353 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/eval_dag_sampling_layers_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    31067 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/eval_dag_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7924 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/ext_ops.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4740 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14347 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/ext_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6255 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9353 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/interfaces.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19588 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/link_samplers.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.537693 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/proto/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      684 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/proto/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1545 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/proto/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5972 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/proto/eval_dag.proto
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    21425 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    23256 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.549694 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    15002 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    25122 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/adjacency.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    18552 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/adjacency_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    39304 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/batching_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    33306 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/batching_utils_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11626 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/broadcast_ops.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14505 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/broadcast_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1289 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/dict_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1348 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/dict_utils_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5899 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_constants.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    57680 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_piece.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    46241 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_piece_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    77580 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6605 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_encode.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7299 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_encode_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    20531 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_io.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    31460 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_io_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    51047 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_ops.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    75964 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2815 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_pprint.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1560 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_pprint_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14184 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_random.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11873 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_random_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    88793 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2635 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_test_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6883 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/normalization_ops.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10698 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/normalization_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    27233 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/padding_ops.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26973 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/padding_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    34763 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/pool_ops.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    22600 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/pool_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7818 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/preprocessing_common.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9440 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/preprocessing_common_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    29090 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/readout.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    25988 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/readout_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    13883 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/schema_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10938 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/schema_utils_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    17518 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/schema_validation.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    17314 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/schema_validation_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5192 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tag_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4878 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tag_utils_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    21394 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tensor_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16448 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tensor_utils_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5692 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tf_internal.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.553695 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3140 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1497 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10534 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/builders.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16006 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/builders_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2889 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/initializers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2005 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/initializers_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    18257 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/keras_tensors.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    33097 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/keras_tensors_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.557695 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7507 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2104 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19666 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/convolution_base.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    15602 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/convolution_base_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6913 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/convolutions.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5456 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/convolutions_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    38608 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/graph_ops.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    55270 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/graph_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26086 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/graph_update.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9853 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/graph_update_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3044 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/item_dropout.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2994 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/item_dropout_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19451 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/map_features.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    25707 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/map_features_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11780 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/next_state.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9905 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/next_state_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2617 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/padding_ops.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6463 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/padding_ops_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2283 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/parse_example.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7217 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/parse_example_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.517691 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.561696 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3405 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2214 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7190 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/distribute_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11905 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/layers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16271 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/layers_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6593 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/losses.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6301 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/losses_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11642 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/metrics.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6024 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/metrics_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14139 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/tasks.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    17706 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/tasks_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3125 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5574 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/utils_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.565696 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2495 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1750 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2687 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/config_dict.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3051 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/config_dict_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2867 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/hparams_vizier.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1585 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    28719 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/layers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    30259 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/layers_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.565696 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1119 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1394 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14406 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/gcn_conv.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    31405 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/gcn_conv_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.565696 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1056 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1588 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    34172 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/layers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26560 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/layers_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.569697 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2355 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1557 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2354 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/config_dict.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3483 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/config_dict_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2678 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/hparams_vizier.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1498 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/hparams_vizier_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    21050 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/layers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    34740 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/layers_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.573697 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2595 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1722 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3092 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/config_dict.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4297 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/config_dict_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3615 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/hparams_vizier.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2318 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19205 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/layers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16973 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/layers_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.577697 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2523 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1863 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2793 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/config_dict.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3134 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/config_dict_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2906 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1599 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    38107 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/layers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    56176 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/layers_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.577697 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2471 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1735 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2558 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2990 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2157 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1296 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5427 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/layers.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7986 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/layers_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.581698 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1086 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2139 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1023 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/examples.proto
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11712 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/graph_schema.proto
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2412 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/graph_schema.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.581698 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3056 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5715 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     8329 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/distribute_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.521691 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.521691 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.585698 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1582 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    17688 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/train.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2697 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3346 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.585698 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/input/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      921 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/input/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19956 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/input/datasets.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9151 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/input/datasets_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     9985 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/interfaces.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26695 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/orchestration.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16235 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/orchestration_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.589699 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2474 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26104 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/classification.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16616 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/classification_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     8772 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/link_prediction.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     6643 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/link_prediction_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    39843 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/regression.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    26015 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/regression_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.589699 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/trainers/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      499 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/trainers/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    12935 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/trainers/keras_fit.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.593699 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4816 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    14492 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/attribution.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10632 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/attribution_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2497 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/label_fns.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1324 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/model_dir.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    11775 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/model_export.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    13130 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/model_export_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4324 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/padding.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2576 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/parsing.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5001 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/parsing_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2073 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/saved_model_gen_testdata.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1940 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/saved_model_load_testdata.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1873 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/strategies.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.597699 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      462 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      478 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7766 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/sampling_spec.proto
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    18498 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/sampling_spec_builder.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    10322 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/sampling_spec_builder_test.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.601700 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1467 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    19030 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/graph_sampler.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    22343 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/graph_sampler_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    22798 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/sampling_lib.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    32231 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/sampling_lib_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4931 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/sampling_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5293 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/sampling_utils_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2123 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/subgraph.proto
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    13473 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/subgraph.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    16541 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/subgraph_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3099 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tensorflow_gnn.bzl
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.605700 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      552 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3368 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/generate_training_data.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1375 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/generate_training_data_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     3926 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/print_training_data.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2080 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/print_training_data_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2700 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/sampled_stats.proto
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     7984 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/sampled_stats.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1975 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/sampled_stats_test.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     1742 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/validate_graph_schema.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.605700 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      571 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/BUILD
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        1 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/__init__.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     4673 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/api_utils.py
+-rwxr-x---   0 arnoegw  (83441) primarygroup (89939)     2149 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/test_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5696 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/tf_test_utils.py
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     2272 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn/version.py
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.525692 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)     5494 2024-04-24 07:02:17.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/PKG-INFO
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)    12148 2024-04-24 07:02:17.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/SOURCES.txt
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        1 2024-04-24 07:02:17.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/dependency_links.txt
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      465 2024-04-24 07:02:17.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/entry_points.txt
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        1 2024-04-24 07:02:17.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/namespace_packages.txt
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)        1 2024-04-24 07:02:17.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/not-zip-safe
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      243 2024-04-24 07:02:17.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/requires.txt
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)       22 2024-04-24 07:02:17.000000 tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/top_level.txt
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.605700 tensorflow-gnn-1.0.3rc0/testdata/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      238 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/testdata/BUILD
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.605700 tensorflow-gnn-1.0.3rc0/testdata/heterogeneous/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      420 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/testdata/heterogeneous/BUILD
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.605700 tensorflow-gnn-1.0.3rc0/testdata/homogeneous/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      294 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/testdata/homogeneous/BUILD
+drwxr-x---   0 arnoegw  (83441) primarygroup (89939)        0 2024-04-24 07:02:17.609701 tensorflow-gnn-1.0.3rc0/testdata/node_vs_edge/
+-rw-r-----   0 arnoegw  (83441) primarygroup (89939)      366 2024-04-24 06:44:23.000000 tensorflow-gnn-1.0.3rc0/testdata/node_vs_edge/BUILD
```

### Comparing `tensorflow-gnn-1.0.2rc1/BUILD` & `tensorflow-gnn-1.0.3rc0/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/LICENSE` & `tensorflow-gnn-1.0.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/PKG-INFO` & `tensorflow-gnn-1.0.3rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-gnn
-Version: 1.0.2rc1
+Version: 1.0.3rc0
 Summary: A library for building scalable graph neural networks in TensorFlow.
 Home-page: https://github.com/tensorflow/gnn
 Download-URL: https://github.com/tensorflow/gnn.git
 Author: Google LLC
 Author-email: tensorflow-gnn@googlegroups.com
 License: Apache 2.0
 Keywords: tensorflow gnn graph
@@ -79,26 +79,29 @@
 [API docs](tensorflow_gnn/docs/api_docs/README.md).
 
 ## Installation Instructions
 
 The latest stable release of TensorFlow GNN is available from
 
 ```
-pip install tensorflow_gnn
+pip install tensorflow-gnn
 ```
 
 For installation from source, see our [Developer
 Guide](tensorflow_gnn/docs/guide/developer.md).
 
 Key platform requirements:
 
-  * TensorFlow 2.12, 2.13, 2.14 or 2.15, and any GPU drivers it needs
+  * TensorFlow 2.12 or higher, and any GPU drivers it needs
     [[instructions](https://www.tensorflow.org/install)].
   * Keras v2, as traditionally included with TensorFlow 2.x.
-    (TF-GNN does not work with the new multi-backend Keras v3.)
+    TF-GNN does not work with the new multi-backend Keras v3.<br/>
+    **Users of TF2.16+ must also `pip install tf-keras` and set
+    TF_USE_LEGACY_KERAS=1**,
+    see our [Keras version](tensorflow_gnn/docs/guide/keras_version.md) guide for details.
   * Apache Beam for distributed graph sampling.
 
 TF-GNN is developed and tested on Linux. Running on other platforms supported
 by TensorFlow may be possible.
 
 ## Citation
```

### Comparing `tensorflow-gnn-1.0.2rc1/README.md` & `tensorflow-gnn-1.0.3rc0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,26 +48,29 @@
 [API docs](tensorflow_gnn/docs/api_docs/README.md).
 
 ## Installation Instructions
 
 The latest stable release of TensorFlow GNN is available from
 
 ```
-pip install tensorflow_gnn
+pip install tensorflow-gnn
 ```
 
 For installation from source, see our [Developer
 Guide](tensorflow_gnn/docs/guide/developer.md).
 
 Key platform requirements:
 
-  * TensorFlow 2.12, 2.13, 2.14 or 2.15, and any GPU drivers it needs
+  * TensorFlow 2.12 or higher, and any GPU drivers it needs
     [[instructions](https://www.tensorflow.org/install)].
   * Keras v2, as traditionally included with TensorFlow 2.x.
-    (TF-GNN does not work with the new multi-backend Keras v3.)
+    TF-GNN does not work with the new multi-backend Keras v3.<br/>
+    **Users of TF2.16+ must also `pip install tf-keras` and set
+    TF_USE_LEGACY_KERAS=1**,
+    see our [Keras version](tensorflow_gnn/docs/guide/keras_version.md) guide for details.
   * Apache Beam for distributed graph sampling.
 
 TF-GNN is developed and tested on Linux. Running on other platforms supported
 by TensorFlow may be possible.
 
 ## Citation
```

### Comparing `tensorflow-gnn-1.0.2rc1/WORKSPACE` & `tensorflow-gnn-1.0.3rc0/WORKSPACE`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/package/move_generated_files.sh` & `tensorflow-gnn-1.0.3rc0/package/move_generated_files.sh`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/package/tfdep.bzl` & `tensorflow-gnn-1.0.3rc0/package/tfdep.bzl`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/setup.py` & `tensorflow-gnn-1.0.3rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,16 +169,16 @@
     namespace_packages=[],
     install_requires=[
         'google-vizier>=0.0.13',
         'ml-collections',
         'networkx',
         'pyarrow',
         # pylint:disable=g-line-too-long
-        'tensorflow>=2.12.0,<2.16.0; platform_machine != "arm64" or platform_system != "Darwin"',
-        'tensorflow-macos>=2.12.0,<2.16.0; platform_machine == "arm64" and platform_system == "Darwin"',
+        'tensorflow>=2.12.0,<3; platform_machine != "arm64" or platform_system != "Darwin"',
+        'tensorflow-macos>=2.12.0,<3; platform_machine == "arm64" and platform_system == "Darwin"',
         # pylint:enable=g-line-too-long
         'apache-beam',
     ],
     python_requires='>=3.8,<4',
     packages=find_namespace_packages(
         exclude=['examples*', 'package*', 'testdata*'],
     ),
```

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,20 @@
   # Condition formulated per b/306638603#comment33.
   keras_version_fn = getattr(tf.keras, "version", None)
   if keras_version_fn:  # Not present in tf.keras for v2 / before TF 2.16.
     keras_version = keras_version_fn()
     if keras_version.startswith("3."):
       raise ImportError(
           "Package tensorflow_gnn requires tf.keras to be Keras version 2 "
-          f"but got version {keras_version}. Install tensorflow<=2.15 to fix.")
+          f"but got version {keras_version}. "
+          "For open-source TensorFlow 2.16 and above, "
+          "set the environment variable TF_USE_LEGACY_KERAS=1 to fix. "
+          "For more information, see "
+          "https://github.com/tensorflow/gnn/blob/main/tensorflow_gnn/docs/guide/keras_version.md"
+      )
 _check_keras_version()
 del _check_keras_version
 # pylint: enable=g-statement-before-imports
 
 # pylint: disable=line-too-long
 
 from tensorflow_gnn import experimental  # Exposed as submodule. pylint: disable=unused-import
```

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/api_def/api_symbols_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/api_def/api_symbols_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/networkx_io.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/networkx_io.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/networkx_io_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/networkx_io_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/ogb/ogb_lib.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/ogb/ogb_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/triples.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/triples.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/converters/triples_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/converters/triples_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/data/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/data/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/data/unigraph.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/data/unigraph.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/data/unigraph_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/data/unigraph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/datasets/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/datasets/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/datasets/pyg_adapter.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/datasets/pyg_adapter.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/datasets/pyg_adapter_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/datasets/pyg_adapter_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/accessors.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/accessors.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/accessors_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/accessors_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/executor_lib.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/sampler.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/sampler.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/sampler_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/sampler_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/subgraph_pipeline_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/subgraph_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/beam/utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/beam/utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/core.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/core.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/core_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/core_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/custom_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/custom_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/eval_dag.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/eval_dag.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/eval_dag_sampling_layers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/eval_dag_sampling_layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/eval_dag_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/eval_dag_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/ext_ops.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/ext_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/ext_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/ext_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/interfaces.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/link_samplers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/link_samplers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/proto/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/proto/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/proto/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/proto/eval_dag.proto` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/proto/eval_dag.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/adjacency.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/adjacency.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/adjacency_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/adjacency_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/batching_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/batching_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/batching_utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/batching_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/broadcast_ops.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/broadcast_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/broadcast_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/broadcast_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/dict_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/dict_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/dict_utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/dict_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_constants.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_constants.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_piece.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_piece.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_piece_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_piece_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_encode.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_encode.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_encode_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_encode_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_io.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_io.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_io_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_io_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_ops.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_pprint.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_pprint.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_pprint_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_pprint_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_random.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_random.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_random_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_random_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/graph_tensor_test_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/graph_tensor_test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/normalization_ops.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/normalization_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/normalization_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/normalization_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/padding_ops.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/padding_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/padding_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/padding_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/pool_ops.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/pool_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/pool_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/pool_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/preprocessing_common.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/preprocessing_common.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/preprocessing_common_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/preprocessing_common_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/readout.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/readout.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/readout_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/readout_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/schema_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/schema_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/schema_utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/schema_validation.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/schema_validation.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/schema_validation_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/schema_validation_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tag_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tag_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tag_utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tag_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tensor_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tensor_utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tensor_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/graph/tf_internal.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/graph/tf_internal.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/builders.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/builders.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/builders_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/builders_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/initializers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/initializers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/initializers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/initializers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/keras_tensors.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/keras_tensors.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/keras_tensors_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/keras_tensors_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/convolution_base.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/convolution_base.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/convolution_base_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/convolution_base_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/convolutions.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/convolutions.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/convolutions_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/convolutions_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/graph_ops.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/graph_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/graph_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/graph_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/graph_update.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/graph_update.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/graph_update_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/graph_update_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/item_dropout.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/item_dropout.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/item_dropout_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/item_dropout_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/map_features.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/map_features.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/map_features_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/map_features_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/next_state.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/next_state.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/next_state_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/next_state_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/padding_ops.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/padding_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/padding_ops_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/padding_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/parse_example.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/parse_example.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/keras/layers/parse_example_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/keras/layers/parse_example_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/distribute_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/distribute_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/layers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/layers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/losses.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/losses.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/losses_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/losses_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/metrics.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/metrics.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/metrics_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/tasks.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/tasks.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/tasks_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/tasks_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/contrastive_losses/utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/contrastive_losses/utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/config_dict.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/config_dict_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/hparams_vizier.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/layers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gat_v2/layers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gat_v2/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/gcn_conv.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/gcn/gcn_conv_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/gcn/gcn_conv_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/layers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/graph_sage/layers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/graph_sage/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/config_dict.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/config_dict_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/hparams_vizier.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/hparams_vizier_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/layers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/hgt/layers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/hgt/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/config_dict.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/config_dict_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/hparams_vizier.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/layers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/mt_albis/layers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/mt_albis/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/config_dict.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/config_dict_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/layers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/multi_head_attention/layers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/multi_head_attention/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/config_dict.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/layers.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/models/vanilla_mpnn/layers_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/models/vanilla_mpnn/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/examples.proto` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/examples.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/graph_schema.proto` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/graph_schema.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/proto/graph_schema.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/proto/graph_schema.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/__init__.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/distribute_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/distribute_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/train.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/train.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/input/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/input/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/input/datasets.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/input/datasets.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/input/datasets_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/input/datasets_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/interfaces.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/orchestration.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/orchestration.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/orchestration_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/orchestration_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/classification.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/classification_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/classification_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/link_prediction.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/link_prediction.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/link_prediction_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/link_prediction_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/regression.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/regression.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/tasks/regression_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/tasks/regression_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/trainers/keras_fit.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/trainers/keras_fit.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/attribution.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/attribution.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/attribution_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/attribution_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/label_fns.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/label_fns.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/model_dir.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/model_dir.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/model_export.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/model_export.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/model_export_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/model_export_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/padding.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/padding.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/parsing.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/parsing_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/parsing_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/saved_model_gen_testdata.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/saved_model_gen_testdata.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/saved_model_load_testdata.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/saved_model_load_testdata.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/runner/utils/strategies.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/runner/utils/strategies.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/sampling_spec.proto` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/sampling_spec.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/sampling_spec_builder.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/sampling_spec_builder.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/sampling_spec_builder_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/sampling_spec_builder_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/graph_sampler.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/graph_sampler.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/graph_sampler_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/graph_sampler_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/sampling_lib.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/sampling_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/sampling_lib_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/sampling_lib_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/sampling_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/sampling_utils_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/sampling_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/subgraph.proto` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/subgraph.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/subgraph.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/subgraph.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/sampler/unsupported/subgraph_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/sampler/unsupported/subgraph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tensorflow_gnn.bzl` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tensorflow_gnn.bzl`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/generate_training_data.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/generate_training_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/generate_training_data_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/generate_training_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/print_training_data.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/print_training_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/print_training_data_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/print_training_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/sampled_stats.proto` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/sampled_stats.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/sampled_stats.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/sampled_stats.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/sampled_stats_test.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/sampled_stats_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/tools/validate_graph_schema.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/tools/validate_graph_schema.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/BUILD` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/api_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/test_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/utils/tf_test_utils.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/utils/tf_test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn/version.py` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 #
 # Patch releases X.Y.Z, Z > 0, incl. their release candidates, can be done for
 # patches on branch rX.Y as needed.
 #
 # IMPORANT: Right after branching rX.Y, bump the main branch to X.(Y+1).0.dev1.
 # (Submit a change to the Source of Truth, get it out on the main branch asap.)
 
-__version__ = "1.0.2rc1"
+__version__ = "1.0.3rc0"
```

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/PKG-INFO` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-gnn
-Version: 1.0.2rc1
+Version: 1.0.3rc0
 Summary: A library for building scalable graph neural networks in TensorFlow.
 Home-page: https://github.com/tensorflow/gnn
 Download-URL: https://github.com/tensorflow/gnn.git
 Author: Google LLC
 Author-email: tensorflow-gnn@googlegroups.com
 License: Apache 2.0
 Keywords: tensorflow gnn graph
@@ -79,26 +79,29 @@
 [API docs](tensorflow_gnn/docs/api_docs/README.md).
 
 ## Installation Instructions
 
 The latest stable release of TensorFlow GNN is available from
 
 ```
-pip install tensorflow_gnn
+pip install tensorflow-gnn
 ```
 
 For installation from source, see our [Developer
 Guide](tensorflow_gnn/docs/guide/developer.md).
 
 Key platform requirements:
 
-  * TensorFlow 2.12, 2.13, 2.14 or 2.15, and any GPU drivers it needs
+  * TensorFlow 2.12 or higher, and any GPU drivers it needs
     [[instructions](https://www.tensorflow.org/install)].
   * Keras v2, as traditionally included with TensorFlow 2.x.
-    (TF-GNN does not work with the new multi-backend Keras v3.)
+    TF-GNN does not work with the new multi-backend Keras v3.<br/>
+    **Users of TF2.16+ must also `pip install tf-keras` and set
+    TF_USE_LEGACY_KERAS=1**,
+    see our [Keras version](tensorflow_gnn/docs/guide/keras_version.md) guide for details.
   * Apache Beam for distributed graph sampling.
 
 TF-GNN is developed and tested on Linux. Running on other platforms supported
 by TensorFlow may be possible.
 
 ## Citation
```

### Comparing `tensorflow-gnn-1.0.2rc1/tensorflow_gnn.egg-info/SOURCES.txt` & `tensorflow-gnn-1.0.3rc0/tensorflow_gnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

