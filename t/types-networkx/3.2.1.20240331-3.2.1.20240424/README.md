# Comparing `tmp/types-networkx-3.2.1.20240331.tar.gz` & `tmp/types-networkx-3.2.1.20240424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-networkx-3.2.1.20240331.tar", last modified: Sun Mar 31 02:18:41 2024, max compression
+gzip compressed data, was "types-networkx-3.2.1.20240424.tar", last modified: Wed Apr 24 02:17:48 2024, max compression
```

## Comparing `types-networkx-3.2.1.20240331.tar` & `types-networkx-3.2.1.20240424.tar`

### file list

```diff
@@ -1,313 +1,313 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.643383 types-networkx-3.2.1.20240331/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-31 02:18:41.643383 types-networkx-3.2.1.20240331/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.603383 types-networkx-3.2.1.20240331/networkx-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/networkx-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.611383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.611383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/clique.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/clustering_coefficient.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/connectivity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/distance_measures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/dominating_set.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/kcomponents.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/matching.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/maxcut.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/ramsey.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/steinertree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/traveling_salesman.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/treewidth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/vertex_cover.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.615383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/connectivity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/correlation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/mixing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/neighbor_degree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/pairs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/asteroidal.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.615383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/centrality.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/covering.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/edgelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/generators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/matching.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/matrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/projection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/redundancy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/spectral.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/boundary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bridges.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.619383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/betweenness.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/betweenness_subset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/closeness.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/current_flow_betweenness.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/current_flow_betweenness_subset.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/current_flow_closeness.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/degree_alg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/dispersion.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/eigenvector.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/flow_matrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/group.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/harmonic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/katz.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/laplacian.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/load.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/percolation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/reaching.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/second_order.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/subgraph_alg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/trophic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/voterank_alg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/chains.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/chordal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/clique.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/cluster.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.619383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/coloring/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/coloring/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/coloring/equitable_coloring.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/coloring/greedy_coloring.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/communicability_alg.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.619383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/asyn_fluid.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/centrality.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/community_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/kclique.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/kernighan_lin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/label_propagation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/louvain.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/lukes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/modularity_max.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/quality.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.623383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/attracting.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/biconnected.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/connected.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/semiconnected.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/strongly_connected.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/weakly_connected.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.623383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/connectivity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/cuts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/disjoint_paths.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/edge_augmentation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/edge_kcomponents.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/kcomponents.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/kcutsets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/stoerwagner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/covering.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/cuts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/cycles.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/d_separation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/dag.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/distance_measures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/distance_regular.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/dominance.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/dominating.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/efficiency_measures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/euler.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.623383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/boykovkolmogorov.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/capacityscaling.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/dinitz_alg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/edmondskarp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/gomory_hu.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/maxflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/mincost.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/networksimplex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/preflowpush.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/shortestaugmentingpath.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/graph_hashing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/graphical.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/hierarchy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/hybrid.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isolate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.627383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/ismags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/isomorph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/isomorphvf2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/matchhelpers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/temporalisomorphvf2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/tree_isomorphism.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/vf2pp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/vf2userfunc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.627383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/link_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/link_analysis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/link_analysis/hits_alg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/link_analysis/pagerank_alg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/link_prediction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/lowest_common_ancestors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/matching.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.627383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/minors/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/minors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/minors/contraction.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/mis.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/moral.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/node_classification.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/non_randomness.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.627383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/operators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/operators/all.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/operators/binary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/operators/product.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/operators/unary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/planar_drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/planarity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/polynomials.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/reciprocity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/regular.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/richclub.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.627383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/astar.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/dense.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/generic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/unweighted.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/weighted.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/similarity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/simple_paths.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/smallworld.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/smetric.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/sparsifiers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/structuralholes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/summarization.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/swap.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/threshold.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tournament.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.627383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/beamsearch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/breadth_first_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/depth_first_search.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/edgebfs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/edgedfs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.631383 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/branchings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/coding.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/decomposition.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/mst.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/operations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/recognition.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/triads.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/vitality.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/voronoi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/algorithms/wiener.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.631383 types-networkx-3.2.1.20240331/networkx-stubs/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/coreviews.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/digraph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/function.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/graph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/graphviews.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/multidigraph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/multigraph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/classes/reportviews.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/convert.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/convert_matrix.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.631383 types-networkx-3.2.1.20240331/networkx-stubs/drawing/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/drawing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/drawing/layout.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/drawing/nx_agraph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/drawing/nx_latex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/drawing/nx_pydot.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/drawing/nx_pylab.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.635383 types-networkx-3.2.1.20240331/networkx-stubs/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/atlas.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/classic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/cographs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/community.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/degree_seq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/directed.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/duplication.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/ego.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/expanders.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/geometric.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/harary_graph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/internet_as_graphs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/intersection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/interval_graph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/joint_degree_seq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/lattice.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/line.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/mycielski.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/nonisomorphic_trees.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/random_clustered.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/random_graphs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/small.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/social.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/spectral_graph_forge.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/stochastic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/sudoku.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/trees.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/generators/triads.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/lazy_imports.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.639382 types-networkx-3.2.1.20240331/networkx-stubs/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/linalg/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/linalg/algebraicconnectivity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/linalg/attrmatrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/linalg/bethehessianmatrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/linalg/graphmatrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/linalg/laplacianmatrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/linalg/modularitymatrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/linalg/spectrum.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/networkx-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.639382 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/adjlist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/edgelist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/gexf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/gml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/graph6.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/graphml.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.639382 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/json_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/json_graph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/json_graph/adjacency.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/json_graph/cytoscape.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/json_graph/node_link.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/json_graph/tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/leda.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/multiline_adjlist.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/p2g.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/pajek.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/sparse6.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/readwrite/text.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/relabel.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.639382 types-networkx-3.2.1.20240331/networkx-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/backends.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/heaps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/mapped_queue.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/random_sequence.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/rcm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-31 02:17:27.000000 types-networkx-3.2.1.20240331/networkx-stubs/utils/union_find.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 02:18:41.643383 types-networkx-3.2.1.20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:41.643383 types-networkx-3.2.1.20240331/types_networkx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/types_networkx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/types_networkx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/types_networkx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/types_networkx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-31 02:18:41.000000 types-networkx-3.2.1.20240331/types_networkx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.098295 types-networkx-3.2.1.20240424/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-24 02:17:47.000000 types-networkx-3.2.1.20240424/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 02:17:47.000000 types-networkx-3.2.1.20240424/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-24 02:17:48.098295 types-networkx-3.2.1.20240424/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.062295 types-networkx-3.2.1.20240424/networkx-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-24 02:17:47.000000 types-networkx-3.2.1.20240424/networkx-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.070295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.070295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/clique.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/clustering_coefficient.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/connectivity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/distance_measures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/dominating_set.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/kcomponents.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/matching.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/maxcut.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/ramsey.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/steinertree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/traveling_salesman.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/treewidth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/vertex_cover.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.070295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/connectivity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/correlation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/mixing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/neighbor_degree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/pairs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/asteroidal.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.074295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/centrality.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/covering.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/edgelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/generators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/matching.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/matrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/projection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/redundancy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/spectral.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/boundary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bridges.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.078295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/betweenness.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/betweenness_subset.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/closeness.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/current_flow_betweenness.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/current_flow_betweenness_subset.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/current_flow_closeness.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/degree_alg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/dispersion.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/eigenvector.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/flow_matrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/group.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/harmonic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/katz.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/laplacian.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/load.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/percolation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/reaching.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/second_order.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/subgraph_alg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/trophic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/voterank_alg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/chains.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/chordal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/clique.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/cluster.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.078295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/coloring/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/coloring/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/coloring/equitable_coloring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/coloring/greedy_coloring.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/communicability_alg.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.078295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/asyn_fluid.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/centrality.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/community_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/kclique.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/kernighan_lin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/label_propagation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/louvain.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/lukes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/modularity_max.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/quality.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.078295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/attracting.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/biconnected.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/connected.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/semiconnected.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/strongly_connected.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/weakly_connected.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.082295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/connectivity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/cuts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/disjoint_paths.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/edge_augmentation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/edge_kcomponents.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/kcomponents.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/kcutsets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/stoerwagner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/covering.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/cuts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/cycles.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/d_separation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/dag.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/distance_measures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/distance_regular.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/dominance.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/dominating.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/efficiency_measures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/euler.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.082295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/boykovkolmogorov.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/capacityscaling.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/dinitz_alg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/edmondskarp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/gomory_hu.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/maxflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/mincost.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/networksimplex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/preflowpush.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/shortestaugmentingpath.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/graph_hashing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/graphical.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/hierarchy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/hybrid.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isolate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.082295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/ismags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/isomorph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/isomorphvf2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/matchhelpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/temporalisomorphvf2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/tree_isomorphism.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/vf2pp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/vf2userfunc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.086295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/link_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/link_analysis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/link_analysis/hits_alg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/link_analysis/pagerank_alg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/link_prediction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/lowest_common_ancestors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/matching.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.086295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/minors/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/minors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/minors/contraction.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/mis.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/moral.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/node_classification.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/non_randomness.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.086295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/operators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/operators/all.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/operators/binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/operators/product.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/operators/unary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/planar_drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/planarity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/polynomials.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/reciprocity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/regular.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/richclub.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.086295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/astar.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/dense.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/generic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/unweighted.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/weighted.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/similarity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/simple_paths.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/smallworld.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/smetric.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/sparsifiers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/structuralholes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/summarization.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/swap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/threshold.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tournament.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.086295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/beamsearch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/breadth_first_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/depth_first_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/edgebfs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/edgedfs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.086295 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/branchings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/coding.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/decomposition.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/mst.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/operations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/recognition.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/triads.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/vitality.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/voronoi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/algorithms/wiener.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.090295 types-networkx-3.2.1.20240424/networkx-stubs/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/coreviews.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/digraph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/function.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/graphviews.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/multidigraph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/multigraph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/classes/reportviews.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/convert.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/convert_matrix.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.090295 types-networkx-3.2.1.20240424/networkx-stubs/drawing/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/drawing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/drawing/layout.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/drawing/nx_agraph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/drawing/nx_latex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/drawing/nx_pydot.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/drawing/nx_pylab.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.094295 types-networkx-3.2.1.20240424/networkx-stubs/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/atlas.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/classic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/cographs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/community.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/degree_seq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/directed.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/duplication.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/ego.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/expanders.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/geometric.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/harary_graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/internet_as_graphs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/intersection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/interval_graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/joint_degree_seq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/lattice.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/line.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/mycielski.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/nonisomorphic_trees.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/random_clustered.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/random_graphs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/small.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/social.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/spectral_graph_forge.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/stochastic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/sudoku.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/trees.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/generators/triads.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/lazy_imports.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.094295 types-networkx-3.2.1.20240424/networkx-stubs/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/linalg/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/linalg/algebraicconnectivity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/linalg/attrmatrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/linalg/bethehessianmatrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/linalg/graphmatrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/linalg/laplacianmatrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/linalg/modularitymatrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/linalg/spectrum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 02:17:47.000000 types-networkx-3.2.1.20240424/networkx-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.098295 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/adjlist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/edgelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/gexf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/gml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/graph6.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/graphml.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.098295 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/json_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/json_graph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/json_graph/adjacency.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/json_graph/cytoscape.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/json_graph/node_link.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/json_graph/tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/leda.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/multiline_adjlist.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/p2g.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/pajek.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/sparse6.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/readwrite/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/relabel.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.098295 types-networkx-3.2.1.20240424/networkx-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/backends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/heaps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/mapped_queue.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/random_sequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/rcm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 02:17:28.000000 types-networkx-3.2.1.20240424/networkx-stubs/utils/union_find.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:17:48.098295 types-networkx-3.2.1.20240424/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-24 02:17:47.000000 types-networkx-3.2.1.20240424/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:48.098295 types-networkx-3.2.1.20240424/types_networkx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-24 02:17:48.000000 types-networkx-3.2.1.20240424/types_networkx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-24 02:17:48.000000 types-networkx-3.2.1.20240424/types_networkx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:17:48.000000 types-networkx-3.2.1.20240424/types_networkx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 02:17:48.000000 types-networkx-3.2.1.20240424/types_networkx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 02:17:48.000000 types-networkx-3.2.1.20240424/types_networkx.egg-info/top_level.txt
```

### Comparing `types-networkx-3.2.1.20240331/CHANGELOG.md` & `types-networkx-3.2.1.20240424/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.2.1.20240424 (2024-04-24)
+
+Annotate a few NetworkX algorithm types (#11811)
+
 ## 3.2.1.20240331 (2024-03-31)
 
 Remove bare Incomplete annotations in third-party stubs (#11671)
 
 ## 3.2.1.20240313 (2024-03-13)
 
 networkx: add another overload to OutEdgeView.__call__(). (#11578)
```

### Comparing `types-networkx-3.2.1.20240331/PKG-INFO` & `types-networkx-3.2.1.20240424/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-networkx
-Version: 3.2.1.20240331
+Version: 3.2.1.20240424
 Summary: Typing stubs for networkx
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/networkx.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/__init__.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/__init__.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/__init__.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/approximation/traveling_salesman.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/approximation/traveling_salesman.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/correlation.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/correlation.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/assortativity/mixing.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/assortativity/mixing.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/__init__.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/edgelist.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/edgelist.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bipartite/generators.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bipartite/generators.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/boundary.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/boundary.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/bridges.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/bridges.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/__init__.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/current_flow_betweenness.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/current_flow_betweenness.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/flow_matrix.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/flow_matrix.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/centrality/group.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/centrality/group.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/chordal.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/chordal.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/clique.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/clique.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/cluster.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/coloring/greedy_coloring.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/coloring/greedy_coloring.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/community/__init__.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/community/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/components/strongly_connected.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/components/strongly_connected.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/connectivity.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/connectivity.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/cuts.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/cuts.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/disjoint_paths.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/disjoint_paths.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/edge_augmentation.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/edge_augmentation.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/connectivity/edge_kcomponents.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/connectivity/edge_kcomponents.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/core.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/core.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/cuts.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/cuts.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/cycles.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/cycles.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/dag.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/dag.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/distance_measures.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/distance_measures.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/euler.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/euler.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/maxflow.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/maxflow.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/networksimplex.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/networksimplex.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/flow/utils.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/flow/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/ismags.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/ismags.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/isomorph.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/isomorph.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/isomorphvf2.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/isomorphvf2.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/matchhelpers.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/matchhelpers.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/temporalisomorphvf2.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/temporalisomorphvf2.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/vf2pp.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/vf2pp.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/isomorphism/vf2userfunc.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/isomorphism/vf2userfunc.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/link_analysis/pagerank_alg.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/link_analysis/pagerank_alg.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/link_prediction.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/link_prediction.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/minors/contraction.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/minors/contraction.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/operators/binary.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/operators/binary.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/planarity.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/planarity.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/generic.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/generic.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/unweighted.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/unweighted.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/shortest_paths/weighted.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/shortest_paths/weighted.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/similarity.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/similarity.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/simple_paths.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/simple_paths.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/smallworld.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/smallworld.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/breadth_first_search.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/breadth_first_search.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/traversal/depth_first_search.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/traversal/depth_first_search.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/branchings.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/branchings.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/algorithms/tree/mst.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/algorithms/tree/mst.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/classes/coreviews.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/classes/coreviews.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/classes/digraph.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/classes/digraph.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/classes/function.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/classes/function.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/classes/graph.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/classes/graph.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/classes/graphviews.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/classes/graphviews.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/classes/multidigraph.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/classes/multidigraph.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/classes/multigraph.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/classes/multigraph.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/classes/reportviews.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/classes/reportviews.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/convert.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/convert.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def to_networkx_graph(
     data: _Data[_Node], create_using: Graph[_Node] | Callable[[], Graph[_Node]] | None = None, multigraph_input: bool = False
 ) -> Graph[_Node]: ...
 @_dispatch
 def to_dict_of_lists(G: Graph[_Node], nodelist: None | Iterable[_Node] = None) -> dict[_Node, list[_Node]]: ...
 @_dispatch
-def from_dict_of_lists(d: dict[_Node, Iterable[_Node]], create_using: Incomplete | None = None): ...
-def to_dict_of_dicts(G, nodelist=None, edge_data=None) -> dict[Incomplete, Incomplete]: ...
+def from_dict_of_lists(d: dict[_Node, Iterable[_Node]], create_using: Incomplete | None = None) -> Graph[_Node]: ...
+def to_dict_of_dicts(G: Graph[_Node], nodelist=None, edge_data=None) -> dict[Incomplete, Incomplete]: ...
 @_dispatch
-def from_dict_of_dicts(d, create_using=None, multigraph_input=False): ...
+def from_dict_of_dicts(d, create_using=None, multigraph_input=False) -> Graph[Incomplete]: ...
 @_dispatch
-def to_edgelist(G, nodelist=None): ...
+def to_edgelist(G: Graph[_Node], nodelist=None): ...
 @_dispatch
-def from_edgelist(edgelist, create_using=None): ...
+def from_edgelist(edgelist, create_using=None) -> Graph[Incomplete]: ...
```

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/convert_matrix.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/convert_matrix.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/drawing/layout.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/drawing/layout.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/drawing/nx_agraph.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/drawing/nx_agraph.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/drawing/nx_latex.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/drawing/nx_latex.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/drawing/nx_pylab.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/drawing/nx_pylab.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/exception.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/exception.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/__init__.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/classic.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/classic.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/community.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/community.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/degree_seq.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/degree_seq.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/directed.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/directed.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/geometric.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/geometric.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/internet_as_graphs.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/internet_as_graphs.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/lattice.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/lattice.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/random_clustered.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/random_clustered.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/random_graphs.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/random_graphs.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/generators/small.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/generators/small.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/linalg/__init__.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/linalg/algebraicconnectivity.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/linalg/algebraicconnectivity.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/linalg/attrmatrix.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/linalg/attrmatrix.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/linalg/laplacianmatrix.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/linalg/laplacianmatrix.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/readwrite/adjlist.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/readwrite/adjlist.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/readwrite/edgelist.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/readwrite/edgelist.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/readwrite/gexf.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/readwrite/gexf.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/readwrite/gml.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/readwrite/gml.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/readwrite/graphml.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/readwrite/graphml.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/readwrite/multiline_adjlist.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/readwrite/multiline_adjlist.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/readwrite/text.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/readwrite/text.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/relabel.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/relabel.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/utils/backends.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/utils/backends.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/utils/decorators.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/utils/decorators.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/utils/heaps.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/utils/heaps.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/utils/mapped_queue.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/utils/mapped_queue.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/utils/misc.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/utils/misc.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/networkx-stubs/utils/random_sequence.pyi` & `types-networkx-3.2.1.20240424/networkx-stubs/utils/random_sequence.pyi`

 * *Files identical despite different names*

### Comparing `types-networkx-3.2.1.20240331/setup.py` & `types-networkx-3.2.1.20240424/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.2.1.20240331",
+      version="3.2.1.20240424",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/networkx.md",
```

### Comparing `types-networkx-3.2.1.20240331/types_networkx.egg-info/PKG-INFO` & `types-networkx-3.2.1.20240424/types_networkx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-networkx
-Version: 3.2.1.20240331
+Version: 3.2.1.20240424
 Summary: Typing stubs for networkx
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/networkx.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -32,10 +32,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-networkx-3.2.1.20240331/types_networkx.egg-info/SOURCES.txt` & `types-networkx-3.2.1.20240424/types_networkx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

