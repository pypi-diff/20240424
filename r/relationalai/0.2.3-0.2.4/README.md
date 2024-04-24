# Comparing `tmp/relationalai-0.2.3.tar.gz` & `tmp/relationalai-0.2.4.tar.gz`

## Comparing `relationalai-0.2.3.tar` & `relationalai-0.2.4.tar`

### file list

```diff
@@ -1,429 +1,441 @@
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 relationalai-0.2.3/README.md
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 relationalai-0.2.3/.github/actions/end-to-end/action.yml
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 relationalai-0.2.3/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.2.3/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/README.md
--rw-r--r--   0        0        0    17337 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/README.md
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/extend.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_degree.md
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_degree.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_indegree.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/num_edges.md
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/num_nodes.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/README.md
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/add.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/call__.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/extend.md
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/set.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/to.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/Edge.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/Node.md
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/README.md
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/concat.md
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/contains.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/ends_with.md
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/join.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/length.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/lowercase.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/replace.md
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/python/std/strings/uppercase.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/cdc.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/custom_snowflake_connection.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/fraud.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/requirements.txt
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/simple_recursion.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/README.md
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/articles_graph.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/articles_graph_with_nlp.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/pyproject.toml
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/utils.py
--rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/articles_graph/daily_articles/04_04_2024.json
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/rel/foo.rel
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.3/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/index.html
--rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/package.json
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/App.styl
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/Selection.tsx
--rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/util.ts
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/assets/favicon.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/EventList.styl
--rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/EventList.tsx
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/EventViewer.styl
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/EventViewer.tsx
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Accordion.stories.tsx
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Accordion.styl
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Accordion.tsx
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Button.styl
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Button.tsx
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Code.styl
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Code.tsx
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.stories.tsx
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.styl
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.tsx
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Field.stories.tsx
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Field.styl
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Field.tsx
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Icon.styl
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Icon.tsx
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.stories.tsx
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.styl
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.styl
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.3/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/emit.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/compiler.py
--rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/debugging.py
--rw-r--r--   0        0        0    44804 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/dsl.py
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27821 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/rel2.py
--rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    10327 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    34436 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    14639 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/std/strings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    52000 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.3/src/relationalai/tools/notes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/README.md
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/conftest.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/strings.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/union.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/basics.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/centrality.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/community.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/degree.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/end2end/test_cases/graphs/similarity.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.3/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.3/.gitignore
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.3/docs/pypi/README.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 relationalai-0.2.4/README.md
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 relationalai-0.2.4/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 relationalai-0.2.4/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 relationalai-0.2.4/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/README.md
+-rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/README.md
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/extend.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/adamic_adar.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_degree.md
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_indegree.md
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/common_neighbor.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_outdegree.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_degree.md
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_indegree.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_outdegree.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/num_edges.md
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/num_nodes.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/preferential_attachment.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/weighted_degree_centrality.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/README.md
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/add.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/call__.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/extend.md
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/from_.md
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/set.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/to.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/Edge.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/Node.md
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/README.md
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/concat.md
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/contains.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/ends_with.md
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/join.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/length.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/lowercase.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/replace.md
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/python/std/strings/uppercase.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/faq/README.md
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/faq/engines.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/cdc.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/custom_snowflake_connection.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/fraud.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/requirements.txt
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/README.md
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/articles_graph.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/articles_graph_with_nlp.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/pyproject.toml
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/utils.py
+-rw-r--r--   0        0        0  1274296 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/articles_graph/daily_articles/04_04_2024.json
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.4/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/index.html
+-rw-r--r--   0        0        0   463836 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/package.json
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/App.styl
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/Selection.tsx
+-rw-r--r--   0        0        0    10577 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/util.ts
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/assets/favicon.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/EventList.styl
+-rw-r--r--   0        0        0     6781 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/EventList.tsx
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/EventViewer.styl
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/EventViewer.tsx
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.stories.tsx
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.styl
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.tsx
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Button.styl
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Button.tsx
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Code.styl
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Code.tsx
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.stories.tsx
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.styl
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.tsx
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Field.stories.tsx
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Field.styl
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Field.tsx
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Icon.styl
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Icon.tsx
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.stories.tsx
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.styl
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.styl
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.4/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/emit.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/compiler.py
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    44988 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27821 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    13261 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    36413 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7349 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    15314 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/std/strings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    52409 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/tools/notes
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 relationalai-0.2.4/src/relationalai/util/snowflake_logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/README.md
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__basics/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query1.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query2.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query3.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__centrality/query4.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query2.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query3.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__community/query4.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query0.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query10.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query11.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query2.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query3.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query4.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query6.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query7.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query8.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__degree/query9.txt
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query0.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query1.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__link_prediction/query2.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query0.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/graphs__similarity/query1.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query0.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query1.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query2.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query3.txt
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query4.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query5.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/strings/query6.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/union/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/strings.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/union.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/basics.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/centrality.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/community.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/degree.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/link_prediction.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/end2end/test_cases/graphs/similarity.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.4/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 relationalai-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.4/docs/pypi/README.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.4/PKG-INFO
```

### Comparing `relationalai-0.2.3/README.md` & `relationalai-0.2.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -168,8 +168,22 @@
 
 If you need to build a wheel for the package, you can do so with the following command:
 
 ```bash
 python -m build
 ```
 
-The resulting wheel and tarball will be in the `dist` directory.
+The resulting wheel and tarball will be in the `dist` directory.
+
+## Contributing to the Frequently Asked Questions (FAQ)
+
+- **Step 1**: Find or create a new markdown file in the `docs/faq/` directory.
+  Files are organized by topic.
+  For example, `docs/faq/engines.md` contains all the FAQ entries related to engines.
+- **Step 2**: Add a new heading to the file with the question.
+  For example, `## How are concurrent workloads handled by an engine?`.
+  Then answer the question in one or two paragraphs.
+- **Step 3**: Add a link to the new FAQ entry in the `docs/faq/README.md` file.
+- **Step 4**: Submit a pull request with your changes.
+- **Step 5**: Someone from the Experience team will review your PR and ask any clarifying questions.
+  We may reformat and rephrase things by pushing changes directly to the PR,
+  and we may ask you to double-check our edits for technical accuracy.
```

### Comparing `relationalai-0.2.3/.github/workflows/end-to-end.yml` & `relationalai-0.2.4/.github/workflows/end-to-end.yml`

 * *Files 21% similar despite different names*

```diff
@@ -30,16 +30,22 @@
     secrets:
       password:
         description: The password to run the tests against
         required: true
       dd_api_key:
         description: The Datadog API key
         required: true
-      
-     
+
+concurrency:
+  group:
+    ${{ github.workflow }}-${{ (github.ref_name == 'main' || github.event_name == 'workflow_dispatch')
+    && github.run_id
+    || github.ref }}
+  cancel-in-progress: true 
+
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         include:
@@ -61,14 +67,15 @@
         sf_account: ndsoebe-rai_integration_aws_uswest_1_consumer
         sf_warehouse: int_env_wh
         sf_rai_app_name: rai_int_app
         sf_compute_pool: int_env_benchmark_compute_xs
         sf_username: team-prod-experience@relational.ai
         sf_password: ${{ secrets.SF_TEST_ACCOUNT_PASSWORD }}
         datadog_api_key: ${{ secrets.DD_API_KEY }}
+        sf_reporting_password: ${{ secrets.SF_REPORTING_PASSWORD }}
     
     - name: Upload Coverage Artifact
       uses: actions/upload-artifact@v2
       with:
         name: coverage-artifact-${{ matrix.python-version }}
         path: coverage/lcov.info
```

### Comparing `relationalai-0.2.3/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/getting_started.md` & `relationalai-0.2.4/docs/getting_started.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,34 @@
 >
 > You may also encounter issues with workflows using the original CLI
 > if you install `relationalai` in your global environment.
 > Always using a project-specific virtual environment is highly recommended.
 > See [Virtual Environments and Packages](https://docs.python.org/3/tutorial/venv.html)
 > for a primer on Python virtual environments.
 
+### Updating Versions
+
 To update your install when new features are released,
 activate your project's virtual environment and run the following:
 
 ```sh
 python -m pip install --upgrade relationalai
 ```
 
 You will need to restart your Python interpreter to use the updated package.
 
+You can check what version you're on by running:
+
+```sh
+rai version
+```
+
+When a new version for a package is available, it will display alongside the installed version. For example, this shows that you currently have version 0.2.1, but 0.2.3 is available for download.
+![screenshot_2024-04-23_at_8 23 33___am_480](https://github.com/RelationalAI/relationalai-python/assets/313870/688dcc6f-8084-421a-a6f3-52a133984766)
+
 ## Create a Model
 
 A **model** consists of rules describing the properties of and relationships between entities from your data.
 Models live in your data cloud and are queried using RelationalAI's declarative query builder.
 
 Here's an example of a model of friendships between people:
```

### Comparing `relationalai-0.2.3/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.4/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/_old/metamodel.md` & `relationalai-0.2.4/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/_old/python_dsl.md` & `relationalai-0.2.4/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/_old/quickstart.md` & `relationalai-0.2.4/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/cli/README.md` & `relationalai-0.2.4/docs/api_reference/cli/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/configuration/README.md` & `relationalai-0.2.4/docs/api_reference/configuration/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Expression.md` & `relationalai-0.2.4/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Property.md` & `relationalai-0.2.4/docs/api_reference/python/Property.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,13 +54,13 @@
 with model.query() as select:
     title = Book.title
     author = Book.author
     title == "Foundation"  # This raises an exception.
     response = select(author) # This also raises an exception.
 ```
 
-`Property` objects may be passed as arguments to [`std.graphs.Edges.extend()`](./std/graphs/Edges/extend.md)
+`Property` objects may be passed as arguments to [`std.graphs.Edge.extend()`](./std/graphs/Edge/README.md)
 in order to add the relationships defined by a property as edges to a [`Graph`](./std/graphs/Graph/README.md).
 
 ## See Also
 
 [`Producer`](./Producer/README.md) and [`InstanceProperty`](./InstanceProperty/README.md).
```

### Comparing `relationalai-0.2.3/docs/api_reference/python/README.md` & `relationalai-0.2.4/docs/api_reference/python/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,27 +81,31 @@
 - [`aggregates.rank_asc()`](./std/aggregates/rank_asc.md)
 - [`aggregates.rank_desc()`](./std/aggregates/rank_desc.md)
 - [`aggregates.sum()`](./std/aggregates/sum.md)
 
 ### [`relationalai.std.graphs`](./std/graphs/README.md)
 
 - [`graphs.Compute`](./std/graphs/Compute/README.md)
+  - [`graphs.Compute.adamic_adar()`](./std/graphs/Compute/adamic_adar.md)
   - [`graphs.Compute.betweenness_centrality()`](./std/graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./std/graphs/Compute/cosine_similarity.md)
+  - [`graphs.Compute.common_neighbor()`](./std/graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.degree()`](./std/graphs/Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./std/graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.eigenvector_centrality()`](./std/graphs/Compute/eigenvector_centrality.md)
   - [`graphs.Compute.num_edges()`](./std/graphs//Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./std/graphs/Compute/indegree.md)
   - [`graphs.Compute.label_propagation()`](./std/graphs/Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./std/graphs/Compute/louvain.md)
   - [`graphs.Compute.num_nodes()`](./std//graphs//Compute/num_nodes.md)
   - [`graphs.Compute.outdegree()`](./std/graphs/Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./std/graphs/Compute/pagerank.md)
+  - [`graphs.Compute.preferential_attachment()`](./std/graphs/Compute/preferential_attachment.md)
   - [`graphs.Compute.weakly_connected_component()`](./std/graphs/Compute/weakly_connected_component.md)
+  - [`graphs.Compute.weighted_degree_centrality()`](./std/graphs/Compute/weighted_degree_centrality.md)
 - [`graphs.Edge`](./std/graphs/Edge/README.md)
   - [`graphs.Edge.add()`](./std/graphs/Edge/add.md)
   - [`graphs.Edge.extend()`](./std/graphs/Edge/extend.md)
 - [`graphs.EdgeInstance`](./std/graphs/EdgeInstance/README.md)
   - [`graphs.EdgeInstance.from_`](./std/graphs/EdgeInstance/from_.md)
   - [`graphs.EdgeInstance.to`](./std/graphs/EdgeInstance/to.md)
   - [`graphs.EdgeInstance.set()`](./std/graphs/EdgeInstance/set.md)
```

### Comparing `relationalai-0.2.3/docs/api_reference/python/Context/README.md` & `relationalai-0.2.4/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Context/enter__.md` & `relationalai-0.2.4/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Context/exit__.md` & `relationalai-0.2.4/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Context/iter__.md` & `relationalai-0.2.4/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Context/model.md` & `relationalai-0.2.4/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Context/results.md` & `relationalai-0.2.4/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.2.4/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.2.4/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.2.4/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.2.4/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Instance/README.md` & `relationalai-0.2.4/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Instance/persist.md` & `relationalai-0.2.4/docs/api_reference/python/Instance/persist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Instance/set.md` & `relationalai-0.2.4/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Instance/unpersist.md` & `relationalai-0.2.4/docs/api_reference/python/Instance/unpersist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.2.4/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.2.4/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/README.md` & `relationalai-0.2.4/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/Type.md` & `relationalai-0.2.4/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/found.md` & `relationalai-0.2.4/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/not_found.md` & `relationalai-0.2.4/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.2.4/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/query.md` & `relationalai-0.2.4/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/read.md` & `relationalai-0.2.4/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/rule.md` & `relationalai-0.2.4/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/scope.md` & `relationalai-0.2.4/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Model/union.md` & `relationalai-0.2.4/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/README.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/add__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/le__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.2.4/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Type/README.md` & `relationalai-0.2.4/docs/api_reference/python/Type/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Type/add.md` & `relationalai-0.2.4/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Type/call__.md` & `relationalai-0.2.4/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Type/extend.md` & `relationalai-0.2.4/docs/api_reference/python/Type/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/Type/or__.md` & `relationalai-0.2.4/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/clients/README.md` & `relationalai-0.2.4/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.2.4/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/README.md` & `relationalai-0.2.4/docs/api_reference/python/std/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 - [`aggregates.rank_asc()`](./aggregates/rank_asc.md)
 - [`aggregates.rank_desc()`](./aggregates/rank_desc.md)
 - [`aggregates.sum()`](./aggregates/sum.md)
 
 ## [`relationalai.std.graphs`](./graphs/README.md)
 
 - [`graphs.Compute`](./graphs/Compute/README.md)
+  - [`graphs.Compute.adamic_adar()`](./graphs/Compute/adamic_adar.md)
   - [`graphs.Compute.avg_degree()`](./graphs/Compute/avg_degree.md)
   - [`graphs.Compute.avg_indegree()`](./graphs/Compute/avg_indegree.md)
   - [`graphs.Compute.avg_outdegree()`](./graphs/Compute/avg_outdegree.md)
   - [`graphs.Compute.betweenness_centrality()`](./graphs/Compute/betweeness_centrality.md)
   - [`graphs.Compute.cosine_similarity()`](./graphs/Compute/cosine_similarity.md)
+  - [`graphs.Compute.common_neighbor()`](./graphs/Compute/common_neighbor.md)
   - [`graphs.Compute.degree()`](./graphs/Compute/degree.md)
   - [`graphs.Compute.degree_centrality()`](./graphs/Compute/degree_centrality.md)
   - [`graphs.Compute.eigenvector_centrality()`](./graphs/Compute/eigenvector_centrality.md)
   - [`graphs.Compute.num_edges()`](./graphs/Compute/num_edges.md)
   - [`graphs.Compute.indegree()`](./graphs/Compute/indegree.md)
   - [`graphs.Compute.label_propagation()`](./graphs/Compute/label_propagation.md)
   - [`graphs.Compute.louvain()`](./graphs/Compute/louvain.md)
@@ -35,15 +37,17 @@
   - [`graphs.Compute.max_outdegree()`](./graphs/Compute/max_outdegree.md)
   - [`graphs.Compute.min_degree()`](./graphs/Compute/min_degree.md)
   - [`graphs.Compute.min_indegree()`](./graphs/Compute/min_indegree.md)
   - [`graphs.Compute.min_outdegree()`](./graphs/Compute/min_outdegree.md)
   - [`graphs.Compute.num_nodes()`](./graphs/Compute/num_nodes.md)
   - [`graphs.Compute.outdegree()`](./graphs/Compute/outdegree.md)
   - [`graphs.Compute.pagerank()`](./graphs/Compute/pagerank.md)
+  - [`graphs.Compute.preferential_attachment()`](./graphs/Compute/preferential_attachment.md)
   - [`graphs.Compute.weakly_connected_component()`](./graphs/Compute/weakly_connected_component.md)
+  - [`graphs.Compute.weighted_degree_centrality()`](./graphs/Compute/weighted_degree_centrality.md)
 - [`graphs.Edge`](./graphs/Edge/README.md)
   - [`graphs.Edge.__call__()`](./graphs/Edge/call__.md)
   - [`graphs.Edge.add()`](./graphs/Edge/add.md)
   - [`graphs.Edge.extend()`](./graphs/Edge/extend.md)
 - [`graphs.EdgeInstance`](./graphs/EdgeInstance/README.md)
   - [`graphs.EdgeInstance.from_`](./graphs/EdgeInstance/from_.md)
   - [`graphs.EdgeInstance.to`](./graphs/EdgeInstance/to.md)
```

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/Vars.md` & `relationalai-0.2.4/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/alias.md` & `relationalai-0.2.4/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.2.4/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.2.4/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.2.4/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.2.4/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.2.4/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.2.4/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.2.4/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.2.4/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 ## Parameters
 
 | Name | Type | Description |
 | :--- | :--- | :------ |
 | `graph` | [`Graph`](../Graph/README.md) | The graph on which the `Compute` namespace is instantiated. |
 
 ## Methods
-
+- [`Compute.adamic_adar()`](./adamic_adar.md)
 - [`Compute.avg_degree()`](./avg_degree.md)
 - [`Compute.avg_indegree()`](./avg_indegree.md)
 - [`Compute.avg_outdegree()`](./avg_outdegree.md)
 - [`Compute.betweeness_centrality()`](./betweeness_centrality.md)
+- [`Compute.common_neighbor()`](./common_neighbor.md)
 - [`Compute.cosine_similarity()`](./cosine_similarity.md)
 - [`Compute.degree()`](./degree.md)
 - [`Compute.degree_centrality()`](./degree_centrality.md)
 - [`Compute.eigenvector_centrality()`](./eigenvector_centrality.md)
 - [`Compute.num_edges()`](./num_edges.md)
 - [`Compute.indegree()`](./indegree.md)
 - [`Compute.label_propagation()`](./label_propagation.md)
@@ -34,15 +35,17 @@
 - [`Compute.max_outdegree()`](./max_outdegree.md)
 - [`Compute.min_degree()`](./min_degree.md)
 - [`Compute.min_indegree()`](./min_indegree.md)
 - [`Compute.min_outdegree()`](./min_outdegree.md)
 - [`Compute.num_nodes()`](./num_nodes.md)
 - [`Compute.outdegree()`](./outdegree.md)
 - [`Compute.pagerank()`](./pagerank.md)
+- [`Compute.preferential_attachment()`](./preferential_attachment.md)
 - [`Compute.weakly_connected_component()`](./weakly_connected_component.md)
+- [`Compute.weighted_degree_centrality()`](./weighted_degree_centrality.md)
 
 ## Example
 
 ```python
 import relationalai as rai
 from relationalai.std.graphs import Graph
```

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_degree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_indegree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/avg_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     alice.set(follows=carol)
     bob.set(follows=alice)
     carol.set(follows=alice).set(follows=bob)
 
 # Create a graph and add all Person objects to the set of nodes
 # and the Person.follows property to the set of edges.
 graph = Graph(model)
-graph.nodes.extend(Person)
-graph.edges.extend(Person.follows)
+graph.Node.extend(Person)
+graph.Edge.extend(Person.follows)
 
 # Compute the degree centrality of each person in the graph.
 with model.query() as select:
     person = Person()
     centrality = graph.compute.degree_centrality(person)
     response = select(person.name, centrality)
```

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_degree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_indegree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/max_outdegree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/max_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_degree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_indegree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/min_outdegree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/min_outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/num_edges.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/num_edges.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/num_nodes.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/num_nodes.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/README.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     alice.set(follows=bob)
 
 # Create a directed graph.
 graph = Graph(model)
 
 # Add edges to the graph based on the `follows` property.
 # Note that nodes are automatically added to the graph when edges are added.
-graph.Edges.extend(Person.follows)
+graph.Edge.extend(Person.follows)
 
 # You may add specific edges to a graph using the `Edge.add()` method inside of a rule.
 with model.rule():
     p = Person(name="Alice")
     graph.Edge.add(from_=p, to=p.follows)
 
 # To query edges, call the `Edge` object and select the desired properties.
```

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/add.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/add.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,8 +50,8 @@
         to=transaction.receiver,
         weight=transaction.amount
     )
 ```
 
 ## See Also
 
-[`Edges.extend()`](./extend.md) and [`Graph.edges`](../Graph/edges.md).
+[`Edge.extend()`](./extend.md) and [`Graph.Edge`](../Graph/Edge.md).
```

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/call__.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Edge/extend.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Edge/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/README.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/from_.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/from_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/set.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/EdgeInstance/to.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/EdgeInstance/to.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/Edge.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/Edge.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/Node.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/Node.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/id.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/id.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/model.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png` & `relationalai-0.2.4/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/strings/concat.md` & `relationalai-0.2.4/docs/api_reference/python/std/strings/concat.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/strings/contains.md` & `relationalai-0.2.4/docs/api_reference/python/std/strings/contains.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/strings/ends_with.md` & `relationalai-0.2.4/docs/api_reference/python/std/strings/ends_with.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/strings/join.md` & `relationalai-0.2.4/docs/api_reference/python/std/strings/join.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/strings/length.md` & `relationalai-0.2.4/docs/api_reference/python/std/strings/length.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/strings/lowercase.md` & `relationalai-0.2.4/docs/api_reference/python/std/strings/lowercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/strings/replace.md` & `relationalai-0.2.4/docs/api_reference/python/std/strings/replace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/docs/api_reference/python/std/strings/uppercase.md` & `relationalai-0.2.4/docs/api_reference/python/std/strings/uppercase.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/README.md` & `relationalai-0.2.4/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/cdc.py` & `relationalai-0.2.4/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/custom_snowflake_connection.py` & `relationalai-0.2.4/examples/custom_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/emit_playground.py` & `relationalai-0.2.4/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/found.py` & `relationalai-0.2.4/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/fraud.ipynb` & `relationalai-0.2.4/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/fraud.py` & `relationalai-0.2.4/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/graph_algos.py` & `relationalai-0.2.4/examples/graph_algos.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #--------------------------------------------------
 
 with model.rule():
     joe = Person.add(name="Joe")
     jane = Person.add(name="Jane")
     bob = Person.add(name="Bob")
     dylan = Person.add(Criminal, name="Dylan")
+    dave = Person.add(name="Dave")
 
     joe.set(knows=jane)
     jane.set(knows=bob)
     bob.set(knows=joe)
     bob.set(knows=dylan)
     dylan.set(knows=joe)
```

### Comparing `relationalai-0.2.3/examples/nested.py` & `relationalai-0.2.4/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/or_types.py` & `relationalai-0.2.4/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/remote_load_csv.py` & `relationalai-0.2.4/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/simple_recursion.py` & `relationalai-0.2.4/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/simple_streamlit.py` & `relationalai-0.2.4/examples/simple_streamlit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/solver.py` & `relationalai-0.2.4/examples/solver.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/weighted_graph_algos.py` & `relationalai-0.2.4/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/articles_graph/README.md` & `relationalai-0.2.4/examples/articles_graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/articles_graph/articles_graph.py` & `relationalai-0.2.4/examples/articles_graph/articles_graph.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/articles_graph/articles_graph_with_nlp.py` & `relationalai-0.2.4/examples/articles_graph/articles_graph_with_nlp.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/articles_graph/utils.py` & `relationalai-0.2.4/examples/articles_graph/utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/articles_graph/daily_articles/04_04_2024.json` & `relationalai-0.2.4/examples/articles_graph/daily_articles/04_04_2024.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/data/people.csv` & `relationalai-0.2.4/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/data/transactions.csv` & `relationalai-0.2.4/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/ev_penetration/ev_penetration.py` & `relationalai-0.2.4/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.2.4/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/ev_penetration/state_stats.csv` & `relationalai-0.2.4/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/imdb/README.md` & `relationalai-0.2.4/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/imdb/imdb.csv` & `relationalai-0.2.4/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/imdb/imdb.py` & `relationalai-0.2.4/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/rel/solver.rel` & `relationalai-0.2.4/examples/rel/solver.rel`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.2.4/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.2.4/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.2.4/examples/social-money-network/snowflake_pagerank.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/package-lock.json` & `relationalai-0.2.4/frontend/debugger/package-lock.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/package.json` & `relationalai-0.2.4/frontend/debugger/package.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/tsconfig.json` & `relationalai-0.2.4/frontend/debugger/tsconfig.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/vite.config.ts` & `relationalai-0.2.4/frontend/debugger/vite.config.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/.storybook/main.ts` & `relationalai-0.2.4/frontend/debugger/.storybook/main.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/App.styl` & `relationalai-0.2.4/frontend/debugger/src/App.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/App.tsx` & `relationalai-0.2.4/frontend/debugger/src/App.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/Selection.tsx` & `relationalai-0.2.4/frontend/debugger/src/Selection.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/debugger_client.ts` & `relationalai-0.2.4/frontend/debugger/src/debugger_client.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/logo.svg` & `relationalai-0.2.4/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/util.styl` & `relationalai-0.2.4/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/util.ts` & `relationalai-0.2.4/frontend/debugger/src/util.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/assets/favicon.png` & `relationalai-0.2.4/frontend/debugger/src/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/EventList.styl` & `relationalai-0.2.4/frontend/debugger/src/components/EventList.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/EventList.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/EventList.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/EventViewer.styl` & `relationalai-0.2.4/frontend/debugger/src/components/EventViewer.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/EventViewer.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/EventViewer.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.2.4/frontend/debugger/src/components/Sidebar.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Accordion.stories.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Accordion.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Accordion.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Button.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Button.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Code.styl` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Code.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Code.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Code.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.stories.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.styl` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Collapsible.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Collapsible.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Field.stories.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Field.styl` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Field.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Field.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Icon.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Icon.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.stories.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.styl` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Modal.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Modal.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.stories.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.styl` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/components/ui/Tooltip.tsx` & `relationalai-0.2.4/frontend/debugger/src/components/ui/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.2.4/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.2.4/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.2.4/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.2.4/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.2.4/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/fixtures/union.json` & `relationalai-0.2.4/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.2.4/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/README.md` & `relationalai-0.2.4/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/emit.py` & `relationalai-0.2.4/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/exec.py` & `relationalai-0.2.4/src/gentest/exec.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/fixtures.py` & `relationalai-0.2.4/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/patch.py` & `relationalai-0.2.4/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/util.py` & `relationalai-0.2.4/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/cli/__main__.py` & `relationalai-0.2.4/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/cli/collect_failures.py` & `relationalai-0.2.4/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/cli/collect_tests.py` & `relationalai-0.2.4/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/cli/repro.py` & `relationalai-0.2.4/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/cli/watch.py` & `relationalai-0.2.4/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/gen/action.py` & `relationalai-0.2.4/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/gen/context.py` & `relationalai-0.2.4/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/gen/document.py` & `relationalai-0.2.4/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/gen/group_limited.py` & `relationalai-0.2.4/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/gen/ir.py` & `relationalai-0.2.4/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/gen/scope.py` & `relationalai-0.2.4/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/gen/task.py` & `relationalai-0.2.4/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/gen/test.py` & `relationalai-0.2.4/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/harness/database.py` & `relationalai-0.2.4/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/validate/diff.py` & `relationalai-0.2.4/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/validate/errors.py` & `relationalai-0.2.4/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/validate/mapping.py` & `relationalai-0.2.4/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/gentest/validate/roundtrip.py` & `relationalai-0.2.4/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/__init__.py` & `relationalai-0.2.4/src/relationalai/__init__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/compiler.py` & `relationalai-0.2.4/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/debugging.py` & `relationalai-0.2.4/src/relationalai/debugging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import ast
 import contextlib
 from dataclasses import dataclass
+import datetime
 import inspect
 import json
 from textwrap import dedent
 import os
 from typing import Dict
 import logging
-import time as _time
+import uuid
 
 from pandas import DataFrame
 from .metamodel import Action, Task
 
 DEBUG = True
 
 #--------------------------------------------------
@@ -73,41 +74,86 @@
 # if DEBUG:
 #     logger.addHandler(TestHandler())
 
 #--------------------------------------------------
 # Debug Spans
 #--------------------------------------------------
 
+# The deepest span in the tree
+TIP_SPAN = None
+
 def span_start(type: str, **kwargs):
     if not DEBUG:
         return
 
-    d = {**kwargs, "event": "span_start", "start_time": _time.perf_counter()}
-    d["span"] = [type]
-    logger.debug(d)
-    return d
+    global TIP_SPAN
+
+    span = Span(type, TIP_SPAN, kwargs)
+    TIP_SPAN = span
+
+    event = {
+        "event": "span_start",
+        "span": [type],
+        "id": str(span.id),
+        "parent_id": str(span.parent.id) if span.parent else None,
+        "start_timestamp": datetime.datetime.utcnow(),
+        **kwargs,
+    }
+    logger.debug(event)
+    return span
 
 def span_end(span):
     if not DEBUG:
         return
-
-    end_time = _time.perf_counter()
-    logger.debug({**span, "event": "span_end", "end_time": end_time, "elapsed": end_time - span["start_time"]})
+    
+    global TIP_SPAN
+    TIP_SPAN = span.parent
+    span.mark_finished()
+    
+    logger.debug({
+        "event": "span_end",
+        "id": str(span.id),
+        "parent_id": str(span.parent.id) if span.parent else None,
+        "span": [span.type],
+        "start_timestamp": span.start_timestamp,
+        "end_timestamp": span.end_timestamp,
+        "elapsed": span.end_timestamp - span.start_timestamp,
+        **span.attrs,
+    })
+
+class Span:
+    def __init__(self, type: str, parent, attrs: Dict):
+        self.id = uuid.uuid4()
+        self.parent = parent
+        self.type = type
+        self.attrs = attrs
+        # Would use `datetime.datetime.now(datetime.UTC)`, but it only works in 3.11.
+        self.start_timestamp = datetime.datetime.utcnow()
+    
+    def mark_finished(self):
+        self.end_timestamp = datetime.datetime.utcnow()
+    
+    def __setitem__(self, key, value):
+        self.attrs[key] = value
 
 @contextlib.contextmanager
 def span(type: str, **kwargs):
     cur = span_start(type, **kwargs)
     try:
         yield cur
     except Exception as err:
         error(err)
         raise
     finally:
         span_end(cur)
 
+def set_span_attr(attr, value):
+    global TIP_SPAN
+    TIP_SPAN.attrs[attr] = value
+
 #--------------------------------------------------
 # Debug Events
 #--------------------------------------------------
 
 EMPTY = {}
 
 def event(event:str, **kwargs):
```

### Comparing `relationalai-0.2.3/src/relationalai/dsl.py` & `relationalai-0.2.4/src/relationalai/dsl.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,15 +676,17 @@
     def _use_var(self):
         if not self._var:
             self._var = Var(Builtins.Unknown)
             prop = build.property_named("result", self._expr.types)
             self._expr.append(prop, self._var)
 
     def _make_sub(self, name: str, existing=None):
-        return None
+        if existing is not None and existing._instance._context is self._graph._stack.active():
+            return existing
+        return getattr(Instance(self._graph, ActionType.Get, [self], {}), name)
 
 #--------------------------------------------------
 # RelationNS
 #--------------------------------------------------
 
 unsafe_symbol_pattern = re.compile(r"[^a-zA-Z0-9_]", re.UNICODE)
 def safe_symbol(name: str):
```

### Comparing `relationalai-0.2.3/src/relationalai/errors.py` & `relationalai-0.2.4/src/relationalai/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import ast
+from collections import defaultdict
 import io
 import textwrap
+from typing import Any, List, Tuple
 from .metamodel import Action, Task
 from . import debugging
 from rich.console import Console
 
 #--------------------------------------------------
 # Print helpers
 #--------------------------------------------------
@@ -19,25 +21,25 @@
     body = textwrap.dedent(body)
     for line in body.splitlines():
         if not line.startswith("  "):
             console.print(line)
         else:
             console.print(line, soft_wrap=True)
 
-def mark_source(source, start_line:int, end_line:int, indent=8, highlight="yellow"):
+def mark_source(source, start_line:int, end_line:int, indent=8, highlight="yellow", highlight_lines = []):
     final_lines = []
     all_lines = source.source.splitlines()
     max_line = source.line + len(all_lines)
     line_number_len = len(str(max_line))
     for ix, line in enumerate(source.source.splitlines()):
         cur = line
         cur_indent = indent if ix > 0 else 0
         line_number = source.line + ix
         color = "dim white"
-        if line_number >= start_line and line_number <= end_line:
+        if (line_number >= start_line and line_number <= end_line) or line_number in highlight_lines:
             color = highlight + " bold"
         cur = f"{' '*cur_indent}[{color}]  {line_number :>{line_number_len}} |  {cur}[/{color}]"
         final_lines.append(cur)
     return "\n".join(final_lines)
 
 def print_source_error(source, name:str, content:str):
     fixed_content_length = len(name) + len(source.file) + len(str(source.line)) + 2  # 2 for the spaces around the dash
@@ -109,14 +111,52 @@
             if hasattr(node, 'type_comment'):
                 expr_node.type_comment = node.type_comment
 
             return expr_node
         return node
 
 #--------------------------------------------------
+# Finders
+#--------------------------------------------------
+
+class PropertyFinder(ast.NodeVisitor):
+    def __init__(self, start_line, properties):
+        self.errors = []
+        self.start_line = start_line
+        self.properties = properties
+        self.found_properties_lines = []  # To store lines where properties are found
+        self.dynamic_properties = []  # To store dynamic properties
+
+    def to_line_numbers(self, node):
+        return (node.lineno, node.end_lineno)
+
+    def visit_Attribute(self, node):
+        if node.attr in self.properties:
+            line_numbers = self.to_line_numbers(node)
+            if line_numbers[0] >= self.start_line:
+                self.found_properties_lines.append(node.lineno)
+        self.generic_visit(node)
+
+    def visit_Call(self, node):
+        # Check if this is a call to 'getattr'
+        if (isinstance(node.func, ast.Name) and node.func.id == 'getattr' and
+                len(node.args) >= 2):
+            if isinstance(node.args[1], ast.Str):
+                property_name = node.args[1].s
+                if property_name in self.properties:
+                    line_numbers = self.to_line_numbers(node)
+                    if line_numbers[0] >= self.start_line:
+                        self.found_properties_lines.append(node.lineno)
+            else:
+                line_numbers = self.to_line_numbers(node)
+                if line_numbers[0] >= self.start_line:
+                    self.dynamic_properties.append(node.lineno)
+        self.generic_visit(node)
+
+#--------------------------------------------------
 # Exceptions
 #--------------------------------------------------
 
 class RAIException(Exception):
     def __init__(self, message:str):
         self.message = message
 
@@ -279,14 +319,42 @@
 
         {marked}
         """
         print_source_error(source, "Reserved property name", content)
         exit()
 
     #--------------------------------------------------
+    # Rel errors
+    #--------------------------------------------------
+
+    @staticmethod
+    def rel_undefineds(undefineds:List[Tuple[str, Any]]):
+        # group by source
+        source_map = defaultdict(list)
+        for (name, source) in undefineds:
+            source_map[source.source].append((source, name))
+
+        for names in source_map.values():
+            source = names[0][0]
+            props = ", ".join([f"[yellow]{name}[/yellow]" for (_, name) in names])
+            prop_line = f"property {props} has" if len(names) == 1 else f"properties {props} have"
+            found = PropertyFinder(source.line, [name for (_, name) in names])
+            if source.block:
+                found.visit(source.block)
+            found_lines = found.found_properties_lines or found.dynamic_properties
+            marked = mark_source(source, -1, -1, indent=12, highlight_lines=found_lines)
+            content = f"""
+            The {prop_line} never been set or added to and so will always cause the rule or query to fail.
+
+            {marked}
+            """
+            print_source_error(source, "Uninitialized property", content)
+        raise RAIException("Uninitialized property") from None
+
+    #--------------------------------------------------
     # Snowflake errors
     #--------------------------------------------------
 
     @staticmethod
     def snowflake_app_missing(app_name):
         content = f"""
         The [yellow]{app_name}[/yellow] app doesn't appear to be installed in this snowflake account.
```

### Comparing `relationalai-0.2.3/src/relationalai/metagen.py` & `relationalai-0.2.4/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/metamodel.py` & `relationalai-0.2.4/src/relationalai/metamodel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/rel.py` & `relationalai-0.2.4/src/relationalai/rel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/rel2.py` & `relationalai-0.2.4/src/relationalai/rel2.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/rel_emitter.py` & `relationalai-0.2.4/src/relationalai/rel_emitter.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/rel_utils.py` & `relationalai-0.2.4/src/relationalai/rel_utils.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/analysis/mechanistic.py` & `relationalai-0.2.4/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/analysis/whynot.py` & `relationalai-0.2.4/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/clients/azure.py` & `relationalai-0.2.4/src/relationalai/clients/azure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json
 import textwrap
+import time
 from typing import Any, Tuple, List
 import base64
 from urllib.error import HTTPError
 
 from pandas import DataFrame
 import pandas as pd
 
+from relationalai import debugging
+
 from ..errors import Errors, RAIException
 from ..rel_utils import assert_no_problems
 from ..loaders.loader import emit_delete_import, import_file, list_available_resources
 from .config import Config
 from .types import ImportSource, ImportSourceFile
 from .client import Client, ResourceProvider
 from .. import dsl, rel, metamodel as m
@@ -54,15 +57,16 @@
     def list_engines(self):
         return api.list_engines(self._api_ctx())
 
     def get_engine(self, name:str):
         return api.get_engine(self._api_ctx(), name)
 
     def create_engine(self, name:str, size:str, pool:str=""):
-        return api.create_engine_wait(self._api_ctx(), name, size)
+        with debugging.span("create_engine", name=name, size=size):
+            return api.create_engine_wait(self._api_ctx(), name, size)
 
     def delete_engine(self, name:str):
         return api.delete_engine(self._api_ctx(), name)
 
     def suspend_engine(self, name:str):
         return api.suspend_engine(self._api_ctx(), name)
 
@@ -70,24 +74,28 @@
         return api.resume_engine_wait(self._api_ctx(), name)
 
     #--------------------------------------------------
     # Graphs
     #--------------------------------------------------
 
     def list_graphs(self) -> List[Any]:
-        return api.list_databases(self._api_ctx())
+        with debugging.span("list_models"):
+            return api.list_databases(self._api_ctx())
 
     def get_graph(self, name:str):
-        return api.get_database(self._api_ctx(), name)
+        with debugging.span("get_model", name=name):
+            return api.get_database(self._api_ctx(), name)
 
     def create_graph(self, name: str):
-        return api.create_database(self._api_ctx(), name)
+        with debugging.span("create_model", name=name):
+            return api.create_database(self._api_ctx(), name)
 
     def delete_graph(self, name:str):
-        return api.delete_database(self._api_ctx(), name)
+        with debugging.span("delete_model", name=name):
+            return api.delete_database(self._api_ctx(), name)
 
     #--------------------------------------------------
     # Models
     #--------------------------------------------------
 
     def list_models(self, database: str, engine: str):
         return api.list_databases(self._api_ctx())
@@ -95,16 +103,16 @@
     def create_models(self, database: str, engine: str, models:List[Tuple[str, str]]) -> List[Any]:
         lines = []
         for (name, code) in models:
             name = name.replace("\"", "\\\"")
             assert "\"\"\"\"\"\"\"" not in code, "Code literals must use fewer than 7 quotes."
 
             lines.append(textwrap.dedent(f"""
-            def delete[:rel, :catalog, :model, "{name}"] = rel[:catalog, :model, "{name}"]
-            def insert[:rel, :catalog, :model, "{name}"] = raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
+            def delete[:rel, :catalog, :model, "{name}"]: rel[:catalog, :model, "{name}"]
+            def insert[:rel, :catalog, :model, "{name}"]: raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
             """))
         rel_code = "\n\n".join(lines)
         results = self.exec_raw(database, engine, rel_code, readonly=False)
         if results.problems:
             return results.problems
         return []
 
@@ -144,15 +152,47 @@
 
     #--------------------------------------------------
     # Exec
     #--------------------------------------------------
 
     def exec_raw(self, database:str, engine:str, raw_code:str, readonly=True, raw_results=True, inputs: dict = {}):
         try:
-            return api.exec(self._api_ctx(), database, engine, raw_code, readonly=readonly, inputs=inputs)
+            with debugging.span("transaction") as txn_span:
+                ctx = self._api_ctx()
+                with debugging.span("create"):
+                    txn = api.exec_async(ctx, database, engine, raw_code, readonly=readonly, inputs=inputs)
+                txn_id = txn.transaction["id"]
+                txn_span["txn_id"] = txn_id
+
+                # TODO: dedup with SDK
+                rsp = api.TransactionAsyncResponse()
+                txn = api.get_transaction(ctx, txn_id)
+                start_time = time.time()
+
+                def check_done():
+                    with debugging.span("check_status"):
+                        state = api.get_transaction(ctx, txn_id)["state"]
+                        return api.is_txn_term_state(state)
+
+                with debugging.span("wait", txn_id=txn_id):
+                    api.poll_with_specified_overhead(
+                        check_done,
+                        overhead_rate=0.2,
+                        start_time=start_time,
+                    )
+
+                # TODO: parallelize
+                with debugging.span("fetch"):
+                    rsp.transaction = api.get_transaction(ctx, txn_id)
+                    rsp.metadata = api.get_transaction_metadata(ctx, txn_id)
+                    rsp.problems = api.get_transaction_problems(ctx, txn_id)
+                    with debugging.span("fetch_results"):
+                        rsp.results = api.get_transaction_results(ctx, txn_id)
+
+                return rsp
         except HTTPError as err:
             res = json.loads(err.read().decode())
             # RAI API uses a JSON payload in the body to explain why the request failed
             # This annotates the error with that to make the exception actually useful.
             if "engine not found" in res.get('message', ''):
                 print("") # the SDK appears to print some stuff before the error message
                 Errors.engine_not_found(self.config.get("engine", "Unknown"), res.get('message'))
```

### Comparing `relationalai-0.2.3/src/relationalai/clients/client.py` & `relationalai-0.2.4/src/relationalai/clients/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import atexit
+import re
 from collections import defaultdict
 from typing import Dict, List, Any, Tuple
 
 from abc import ABC, abstractmethod
 from pandas import DataFrame
 import time
 
@@ -15,46 +16,58 @@
 # InstallBatch
 #--------------------------------------------------
 
 class InstallBatch:
     def __init__(self):
         self.dirty = set()
         self.content:Dict[str, Dict[str, List[str]]] = defaultdict(lambda: defaultdict(list))
+        self.task_map = defaultdict(dict)
 
     def _cell(self):
         return debugging.jupyter.cell() or ""
 
     def _check_dirty_cells(self, name:str):
         for cell in debugging.jupyter.dirty_cells:
             self.content[name][cell].clear()
         debugging.jupyter.dirty_cells.clear()
 
-    def append(self, name:str, code:str):
+    def append(self, name:str, code:str, task:m.Task|None=None):
         self._check_dirty_cells(name)
         self.dirty.add(name)
-        self.content[name][self._cell()].append(code)
+        self.content[name][self._cell()].append((code, task))
 
-    def set(self, name:str, code:str):
+    def set(self, name:str, code:str, task:m.Task|None=None):
         self.dirty.add(name)
-        self.content[name][self._cell()] = [code]
+        self.content[name][self._cell()] = [(code, task)]
 
     def flush(self):
         items = []
         for name in self.dirty:
             all_cells = []
+            cur_line = 0
+            task_map = self.task_map[name]
             for _, content in self.content[name].items():
-                for code in content:
+                for (code, task) in content:
                     all_cells.append(code)
+                    end = code.count("\n") + cur_line + 2
+                    task_map[task] = (cur_line, end)
+                    cur_line = end
             items.append((name, "\n\n".join(all_cells)))
         self.dirty.clear()
         return items
 
     def is_dirty(self):
         return len(self.dirty) > 0
 
+    def line_to_task(self, name:str, line:int):
+        for task, (start, end) in self.task_map[name].items():
+            if start <= line <= end:
+                return task
+        return None
+
 #--------------------------------------------------
 # Resources
 #--------------------------------------------------
 
 class ResourceProvider(ABC):
     def __init__(self, profile: str | None = None, config:Config|None=None):
         super().__init__()
@@ -103,15 +116,15 @@
 
     @abstractmethod
     def resume_engine(self, name: str):
         pass
 
     def get_default_engine_name(self) -> str:
         return self.config.get("engine")
-    
+
     def get_app_name(self):
         return self.config.get("rai_app_name", "relationalai")
 
     #--------------------------------------------------
     # Transactions
     #--------------------------------------------------
 
@@ -230,26 +243,43 @@
             if not existing:
                 self.resources.create_graph(self._database)
                 debugging.time("create_database", time.perf_counter() - start)
 
     def get_engine_name(self, name:str|None=None) -> str:
         return str(name or self.resources.config.get("engine"))
 
-    def report_errors(self, errors:List[Any], abort_on_error=True):
+    def report_errors(self, errors:List[Any], abort_on_error=True, task=None):
         maybe_abort = False
+        undefineds = []
         if len(errors):
             for problem in errors:
                 if problem.get("is_error") or problem.get("is_exception"):
                     maybe_abort = True
-                    if "message" in problem:
-                        print(problem["message"])
-                    if "report" in problem:
-                        print(problem["report"])
+                    message = problem.get("message", "")
+                    report = problem.get("report", "")
+                    path = problem.get("path", "")
+                    if problem.get("error_code") == "UNDEFINED_IDENTIFIER":
+                        match = re.search(r'`(.+?)` is undefined', message)
+                        line = report.split("|")[0]
+                        if line:
+                            line = int(line) - 1
+                        source_task = self._install_batch.line_to_task(path, line) or task
+                        source = debugging.get_source(source_task)
+                        if not source:
+                            source = debugging.SourceInfo()
+                        undefineds.append((match.group(1), source))
+                    else:
+                        if message:
+                            print(message)
+                        if report:
+                            print(report)
         if abort_on_error and maybe_abort:
-            from relationalai.errors import RelQueryError
+            from relationalai.errors import RelQueryError, Errors
+            if undefineds:
+                Errors.rel_undefineds(undefineds)
             raise RelQueryError(errors)
 
     def load_raw_file(self, path:str):
         content = open(path).read()
         code = self.compiler.compile(dsl.build.raw_task(content))
         self._install_batch.set(path, code)
 
@@ -278,15 +308,15 @@
             dataframe, errors = self.resources.format_results(results, task)
             end_span["results"] = dataframe
             end_span["errors"] = errors
             if raw_results:
                 debugging.time("query", time.perf_counter() - start, DataFrame())
                 self.report_errors(errors, abort_on_error=False)
                 return results
-            self.report_errors(errors)
+            self.report_errors(errors, task=task)
             debugging.time("query", time.perf_counter() - start, dataframe)
             return dataframe
 
     def _install_batch_flush(self):
         if not self.dry_run:
             with debugging.span("install_batch", model=self._database):
                 start = time.perf_counter()
@@ -294,15 +324,15 @@
                 errors = self.resources.create_models(self._database, self.get_engine_name(), code)
                 self.report_errors(errors)
                 debugging.time("install_batch", time.perf_counter() - start, code="\n".join([c[1] for c in code]))
 
     def install(self, name, task:m.Task):
         with debugging.span("rule", model=self._database, task=task, name=name):
             code = self.compiler.compile(task)
-            self._install_batch.append("pyrel_batch_0", code)
+            self._install_batch.append("pyrel_batch_0", code, task=task)
 
     def export_udf(self, name, inputs:List[Tuple[str, m.Var, Any]], outputs, task:m.Task, engine=""):
         cols = task.return_cols()
         if len(outputs) != len(cols):
             raise Exception(f"Expected {len(outputs)} outputs, got {len(cols)}")
         emitted_inputs = [(name, self.compiler.emitter.emit(var), type) for (name, var, type) in inputs]
         outputs = list(zip(cols, outputs))
```

### Comparing `relationalai-0.2.3/src/relationalai/clients/config.py` & `relationalai-0.2.4/src/relationalai/clients/config.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/clients/snowflake.py` & `relationalai-0.2.4/src/relationalai/clients/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,16 @@
         return [{"name":name, "size":size, "state":state}
                 for (name, size, state) in results.fetchall()][0]
 
     def create_engine(self, name:str, size:str, pool:str = ""):
         if not pool:
             raise ValueError("Pool is required")
         try:
-            self._exec(f"call {APP_NAME}.api.create_engine('{name}', '{pool}', '{size}');")
+            with debugging.span("create_engine", name=name, size=size, pool=pool):
+                self._exec(f"call {APP_NAME}.api.create_engine('{name}', '{pool}', '{size}');")
         except Exception as e:
             raise Exception(f"Failed to create engine {name} using pool {pool} and size {size}") from e
 
     def delete_engine(self, name:str):
         self._exec(f"call {APP_NAME}.api.delete_engine('{name}');")
 
     def suspend_engine(self, name:str):
@@ -180,34 +181,38 @@
         raise Exception("Not implemented")
 
     #--------------------------------------------------
     # Graphs
     #--------------------------------------------------
 
     def list_graphs(self) -> List[AvailableModel]:
-        results = self._exec(f"select NAME from {APP_NAME}.api.databases WHERE state <> 'DELETED'")
-        if not results:
-            return []
-        return [{"name": name} for (name,) in results.fetchall()]
+        with debugging.span("list_models"):
+            results = self._exec(f"select NAME from {APP_NAME}.api.databases WHERE state <> 'DELETED'")
+            if not results:
+                return []
+            return [{"name": name} for (name,) in results.fetchall()]
 
     def get_graph(self, name:str):
-        results = self._exec(f"""
-            select ID, NAME, CREATED_ON, DELETED_ON, STATE
-            from {APP_NAME}.api.databases
-            where name='{name}' AND state <> 'DELETED'
-        """)
-        if not results:
-            return None
-        return results.fetchone()
+        with debugging.span("get_model", name=name):
+            results = self._exec(f"""
+                select ID, NAME, CREATED_ON, DELETED_ON, STATE
+                from {APP_NAME}.api.databases
+                where name='{name}' AND state <> 'DELETED'
+            """)
+            if not results:
+                return None
+            return results.fetchone()
 
     def create_graph(self, name: str):
-        self._exec(f"call {APP_NAME}.api.create_database('{name}');")
+        with debugging.span("create_model", name=name):
+            self._exec(f"call {APP_NAME}.api.create_database('{name}');")
 
     def delete_graph(self, name:str):
-        self._exec(f"call {APP_NAME}.api.delete_database('{name}');")
+        with debugging.span("delete_model", name=name):
+            self._exec(f"call {APP_NAME}.api.delete_database('{name}');")
 
     #--------------------------------------------------
     # Models
     #--------------------------------------------------
 
     def list_models(self, database: str, engine: str):
         pass
@@ -215,24 +220,24 @@
     def create_models(self, database: str, engine: str, models:List[Tuple[str, str]]) -> List[Any]:
         lines = []
         for (name, code) in models:
             name = name.replace("\"", "\\\"")
             assert "\"\"\"\"\"\"\"" not in code, "Code literals must use fewer than 7 quotes."
 
             lines.append(textwrap.dedent(f"""
-            def delete[:rel, :catalog, :model, "{name}"] = rel[:catalog, :model, "{name}"]
-            def insert[:rel, :catalog, :model, "{name}"] = raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
+            def delete[:rel, :catalog, :model, "{name}"]: rel[:catalog, :model, "{name}"]
+            def insert[:rel, :catalog, :model, "{name}"]: raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
             """))
         rel_code = "\n\n".join(lines)
         self.exec_raw(database, engine, rel_code, readonly=False)
         # TODO: handle SPCS errors once they're figured out
         return []
 
     def delete_model(self, database:str, engine:str, name:str):
-        self.exec_raw(database, engine, f"def delete[:rel, :catalog, :model, \"{name}\"] = rel[:catalog, :model, \"{name}\"]", readonly=False)
+        self.exec_raw(database, engine, f"def delete[:rel, :catalog, :model, \"{name}\"]: rel[:catalog, :model, \"{name}\"]", readonly=False)
 
     #--------------------------------------------------
     # Exports
     #--------------------------------------------------
 
     def list_exports(self, database: str, engine: str):
         return []
@@ -260,25 +265,38 @@
                 HANDLER = 'handle'
                 AS
                 $$
                 import json
                 from snowflake.snowpark import DataFrame
                 from snowflake.snowpark.functions import col
                 from snowflake.snowpark.types import StringType, IntegerType, StructField, StructType, FloatType, MapType, ArrayType, BooleanType, BinaryType
-
                 def handle(session{py_inputs}):
                     rel_code = f"{safe_rel}"
                     results = session.sql(f"select {APP_NAME}.api.exec('{database}','{engine}','{{rel_code}}', true);")
                     table_results = []
                     for row in results.collect():
                         parsed = json.loads(row[0])
                         table_results.extend(parsed["data"])
 
-                    schema = StructType([{py_outs}])
-                    return session.create_dataframe(table_results, schema=schema)
+                    try:
+                        schema = StructType([{py_outs}])
+                        return session.create_dataframe(table_results, schema=schema)
+                    except Exception as err:
+                        from collections import defaultdict
+                        import textwrap
+                        problems = defaultdict(dict)
+                        for row in table_results:
+                            if row[0] == "catalog" and row[1] == "diagnostic":
+                                if row[2] in ["code", "message", "report"]:
+                                    problems[row[3]][row[2]] = row[4]
+
+                        if (len(problems)):
+                            raise Exception("Failed to run exported query '{func_name}({", ".join([name for (name, *_) in inputs])})':\\n" + textwrap.indent("\\n".join([problem["code"] + " " + problem["message"] + "\\n" + problem["report"] for problem in problems.values()]), "\t")) from None
+                        else:
+                            raise err
                 $$;""")
         start = time.perf_counter()
         self._exec(sql_code)
         debugging.time("export", time.perf_counter() - start, DataFrame(), code=sql_code)
         return
 
     def delete_export(self, model: str, engine: str, export: str):
@@ -392,40 +410,44 @@
 
     #--------------------------------------------------
     # Exec Async
     #--------------------------------------------------
 
     def _check_exec_async_status(self, txn_id: str):
         """Check whether the given transaction has completed."""
-        response = self._exec(f"CALL {APP_NAME}.api.get_transaction('{txn_id}');")
-        assert response, f"No results from get_transaction('{txn_id}')"
+        with debugging.span("check_status"):
+            response = self._exec(f"CALL {APP_NAME}.api.get_transaction('{txn_id}');")
+            assert response, f"No results from get_transaction('{txn_id}')"
         status: str = next(iter(response))[2]
 
         if status == "ABORTED":
             raise Exception(f"Transaction aborted while waiting for results '{txn_id}'")
 
         return status == "COMPLETED"
 
     def _list_exec_async_artifacts(self, txn_id: str) -> Dict[str, str]:
         """Grab the list of artifacts produced in the transaction and the URLs to retrieve their contents."""
-        response = self._exec(f"CALL {APP_NAME}.api.list_transaction_outputs('{txn_id}');")
-        assert response, f"No results from list_transaction_outputs('{txn_id}')"
-        return {name: url for name, url in response}
+        with debugging.span("list_results"):
+            response = self._exec(f"CALL {APP_NAME}.api.list_transaction_outputs('{txn_id}');")
+            assert response, f"No results from list_transaction_outputs('{txn_id}')"
+            return {name: url for name, url in response}
 
     def _fetch_exec_async_artifacts(self, artifact_urls: Dict[str, str]) -> Dict[str, Any]:
         """Grab the contents of the given artifacts from SF."""
         contents = {}
-        with requests.Session() as session:
-            for name, url in artifact_urls.items():
-                response = session.get(url)
-                response.raise_for_status() # throw if something goes wrong.
-                if name.endswith(".json"):
-                    contents[name] = response.json()
-                else:
-                    contents[name] = response.content
+        with debugging.span("fetch_results"):
+            with requests.Session() as session:
+                for name, url in artifact_urls.items():
+                    with debugging.span("fetch_result", name=name):
+                        response = session.get(url)
+                    response.raise_for_status() # throw if something goes wrong.
+                    if name.endswith(".json"):
+                        contents[name] = response.json()
+                    else:
+                        contents[name] = response.content
 
         return contents
 
     def _parse_exec_async_results(self, arrow_files: List[Tuple[str, bytes]]):
         """Mimics the logic in _parse_arrow_results of railib/api.py#L303 without requiring a wrapping multipart form."""
         results = []
 
@@ -435,59 +457,63 @@
                 batches = [batch for batch in reader]
                 table = pa.Table.from_batches(batches=batches, schema=schema)
                 results.append({"relationId": file_name, "table": table})
 
         return results
 
     def _exec_async_raw(self, database:str, engine:str, raw_code:str, readonly=True, inputs={}):
-        if inputs:
-            raise Exception("Inputs aren't currently supported using exec_async in SPCS.")
-
-        response = self._exec(f"CALL {APP_NAME}.api.exec_async('{database}','{engine}','{raw_code}', {readonly});")
-        if not response:
-            raise Exception("No results from exec_async")
-
-        # Grab the txn_id from the response
-        txn_id, status = next(iter(response))
-        debugging.event("transaction", txn_id=txn_id)
-        # Wait for completion or failure
-        if status != "COMPLETED":
-            self._pending_transactions.append(txn_id)
-            poll_with_specified_overhead(lambda: self._check_exec_async_status(txn_id), 0.2)
-
-        self._pending_transactions.remove(txn_id)
-
-        # List the result artifacts (and the URLs to retrieve them)
-        artifact_urls = self._list_exec_async_artifacts(txn_id)
-        # Actually retrieve them
-        artifacts = self._fetch_exec_async_artifacts(artifact_urls)
-
-        meta = _parse_metadata_proto(artifacts["metadata.proto"])
-        meta_json = artifacts["metadata.json"]
-
-        # We use the metadata to map arrow files to the relations they contain data for.
-        # In Azure, this is provided sideband via response headers.
-        arrow_files_to_relations = {}
-        for ix, relation in enumerate(cast(Any, meta).relations):
-
-            arrow_file = relation.file_name
-            relation_id = meta_json[ix]["relationId"]
-            arrow_files_to_relations[arrow_file] = relation_id
-
-        # Hydrate the arrow files into tables
-        results = self._parse_exec_async_results([(arrow_files_to_relations[name], content) for name, content in artifacts.items() if name.endswith(".arrow")])
-
-        rsp = TransactionAsyncResponse()
-        # @FIXME: Hardcoding the `state` feels somewhat unsafe, but we can't have gotten here in the code otherwise.
-        # @FIXME: Missing `response_format_version`, which isn't obviously present anywhere in the results.
-        rsp.transaction = {"id": txn_id, "state": "COMPLETED", "response_format_version": None}
-        rsp.metadata = meta
-        rsp.problems = artifacts["problems.json"]
-        rsp.results = results
-        return rsp
+        with debugging.span("transaction") as txn_span:
+            if inputs:
+                raise Exception("Inputs aren't currently supported using exec_async in SPCS.")
+
+            with debugging.span("create"):
+                response = self._exec(f"CALL {APP_NAME}.api.exec_async('{database}','{engine}','{raw_code}', {readonly});")
+                if not response:
+                    raise Exception("No results from exec_async")
+
+            # Grab the txn_id from the response
+            txn_id, status = next(iter(response))
+            txn_span["txn_id"] = txn_id
+            # Wait for completion or failure
+            if status != "COMPLETED":
+                self._pending_transactions.append(txn_id)
+                with debugging.span("wait", txn_id=txn_id):
+                    poll_with_specified_overhead(lambda: self._check_exec_async_status(txn_id), 0.2)
+
+            self._pending_transactions.remove(txn_id)
+
+            with debugging.span("fetch"):
+                # List the result artifacts (and the URLs to retrieve them)
+                artifact_urls = self._list_exec_async_artifacts(txn_id)
+                # Actually retrieve them
+                artifacts = self._fetch_exec_async_artifacts(artifact_urls)
+
+                meta = _parse_metadata_proto(artifacts["metadata.proto"])
+                meta_json = artifacts["metadata.json"]
+
+                # We use the metadata to map arrow files to the relations they contain data for.
+                # In Azure, this is provided sideband via response headers.
+                arrow_files_to_relations = {}
+                for ix, relation in enumerate(cast(Any, meta).relations):
+
+                    arrow_file = relation.file_name
+                    relation_id = meta_json[ix]["relationId"]
+                    arrow_files_to_relations[arrow_file] = relation_id
+
+                # Hydrate the arrow files into tables
+                results = self._parse_exec_async_results([(arrow_files_to_relations[name], content) for name, content in artifacts.items() if name.endswith(".arrow")])
+
+                rsp = TransactionAsyncResponse()
+                # @FIXME: Hardcoding the `state` feels somewhat unsafe, but we can't have gotten here in the code otherwise.
+                # @FIXME: Missing `response_format_version`, which isn't obviously present anywhere in the results.
+                rsp.transaction = {"id": txn_id, "state": "COMPLETED", "response_format_version": None}
+                rsp.metadata = meta
+                rsp.problems = artifacts["problems.json"]
+                rsp.results = results
+                return rsp
 
     # Copied directly from azure.py
     def _has_errors(self, results):
         if len(results.problems):
             for problem in results.problems:
                 if problem['is_error'] or problem['is_exception']:
                     return True
@@ -721,18 +747,19 @@
     def _fetch_info(self):
         self._table_info = self._model._client.resources.schema_info(self._parent._name, self._name, self._imported)
 
     def _add(self, name, is_imported=False):
         name = name.lower()
         if name in self._tables:
             return self._tables[name]
-        self._tables[name] = SnowflakeTable(self, name)
         if is_imported:
             self._imported.add(name)
-        return self._tables[name]
+        else:
+            self._tables[name] = SnowflakeTable(self, name)
+        return self._tables.get(name)
 
     def __getattribute__(self, __name: str) -> 'SnowflakeTable':
         if __name.startswith("_"):
             return super().__getattribute__(__name)
         table = self._add(__name)
         table._lazy_init()
         return table
```

### Comparing `relationalai-0.2.3/src/relationalai/clients/test.py` & `relationalai-0.2.4/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/clients/types.py` & `relationalai-0.2.4/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/loaders/csv.py` & `relationalai-0.2.4/src/relationalai/loaders/csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,14 @@
         "type": (relation, self.type),
         "name": (relation, source.name)
         })}
         def insert[:__resource, :schema]: ("{relation}", config[:schema])
         def insert[:{relation}]: load_csv[config]
         """
         q = "\n".join(line.strip() for line in q.splitlines())
-        print(q)
         res = provider.exec_raw(model, provider.get_default_engine_name(), q, readonly=False, inputs=inputs)
         assert_no_problems(res)
 
     SAMPLE_LINES_COUNT = 100
 
     @classmethod
     def guess_syntax(cls, path: str) -> Syntax:
```

### Comparing `relationalai-0.2.3/src/relationalai/loaders/loader.py` & `relationalai-0.2.4/src/relationalai/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/loaders/types.py` & `relationalai-0.2.4/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/std/aggregates.py` & `relationalai-0.2.4/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/std/graphs.py` & `relationalai-0.2.4/src/relationalai/std/graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,21 +87,35 @@
 
     def avg_outdegree(self):
         return self._lib.average_outdegree(self._graph)
 
     # --------------------------------------------------
     # Basics
     # --------------------------------------------------
+
     def num_nodes(self):
         return self._lib.num_nodes(self._graph)
 
     def num_edges(self):
         return self._lib.num_edges(self._graph)
 
     # --------------------------------------------------
+    # Link Prediction
+    # --------------------------------------------------
+
+    def adamic_adar(self, node1, node2):
+        return self._lib.adamic_adar(self._graph, node1, node2)
+
+    def preferential_attachment(self, node1, node2):
+        return self._lib.preferential_attachment(self._graph, node1, node2)
+
+    def common_neighbor(self, node1, node2):
+        return self._lib.common_neighbor(self._graph, node1, node2)
+
+    # --------------------------------------------------
     # Similarity
     # --------------------------------------------------
 
     def cosine_similarity(self, node1, node2):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
         return self._lib.cosine_similarity(self._graph, node1, node2)
@@ -133,14 +147,17 @@
         return self._lib.degree_centrality(self._graph, node)
 
     def eigenvector_centrality(self, node):
         if not self._graph.undirected:
             invalid_param("graph", "must be undirected")
         return self._lib.eigenvector_centrality(self._graph, node)
 
+    def weighted_degree_centrality(self, node):
+        return self._lib.weighted_degree_centrality(self._graph, node)
+
     # --------------------------------------------------
     # Community Detection
     # --------------------------------------------------
 
     def weakly_connected_component(self, node):
         return self._lib.weakly_connected_component(self._graph, node)
 
@@ -247,14 +264,15 @@
             create_graph = f"{graph_type}[{self.Edge._type._name}]"
 
         self.model.install_raw(f"""
         declare {self.Node._type.name}
         declare {self.Edge._type._name}
         {f"declare {self.Edge._prop('weight')._name}" if weighted else ""}
         def {self._graph_ref()} {{{create_graph}}}
+        def {self._graph_ref()}[:node]: {{{self.Node._type.name}}}
         @inline
         def {self._lib_ref()} {{rel[:graphlib, {self._graph_ref()}]}}
         """)
 
         # Add a rule that makes all nodes used in edges are also added to
         # the nodes relation
         with model.rule():
```

### Comparing `relationalai-0.2.3/src/relationalai/std/strings.py` & `relationalai-0.2.4/src/relationalai/std/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/tools/cli.py` & `relationalai-0.2.4/src/relationalai/tools/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,21 @@
         rich.print("[yellow bold]No configuration file found.")
         rich.print("To create one, run: [green bold]rai init[/green bold]")
         divider()
         sys.exit(1)
     return cfg
 
 #--------------------------------------------------
+# Validators
+#--------------------------------------------------
+
+ENGINE_NAME_REGEX = re.compile(r'^[a-zA-Z]\w{2,}$')
+ENGINE_NAME_ERROR = "Min 3 chars, start with letter, only letters, numbers, underscores allowed."
+
+#--------------------------------------------------
 # Custom help printer
 #--------------------------------------------------
 
 class RichGroup(click.Group):
     def format_help(self, ctx: Context, formatter: HelpFormatter) -> None:
         global PROFILE
         # @NOTE: I couldn't find a sane way to access the --profile option from here, so insane it is.
@@ -437,15 +444,15 @@
             raise Exception(f"Error fetching engines: {e}")
 
     engine_names = ["Create a new engine"] + [engine.get("name") for engine in engines]
     rich.print("")
     default = get_default(cfg.get("engine", None), engine_names)
     engine = controls.fuzzy("Select an engine:", choices=engine_names, default=default, mandatory=False)
     if engine == "Create a new engine":
-        engine = controls.text("Engine name:")
+        engine = controls.text("Engine name:", validator=ENGINE_NAME_REGEX.match, invalid_message=ENGINE_NAME_ERROR)
         engine_size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
         engine_pool = ""
         if cfg.get("platform") == "snowflake":
             provider = cast(snowflake.Resources, provider)
             rich.print("")
             with Spinner(f"Fetching compute pools for engine size '{engine_size}'", f"Fetched compute pools for engine size '{engine_size}'"):
                 try:
@@ -750,15 +757,15 @@
 
 @cli.command(name="engines:create", help="Create a new engine")
 @click.option("--name", help="Name of the engine")
 @click.option("--size", type=click.Choice(ENGINE_SIZES, case_sensitive=False), help="Size of the engine")
 def engines_create(name, size):
     divider(flush=True)
     ensure_config()
-    name = controls.prompt("Engine name?", name, newline=True)
+    name = controls.prompt("Engine name?", name, validator=ENGINE_NAME_REGEX.match, invalid_message=ENGINE_NAME_ERROR, newline=True)
     if not size:
         size = controls.fuzzy("Engine size:", choices=ENGINE_SIZES)
         rich.print("")
     provider = get_resource_provider()
 
     if provider.config.get("platform") == "snowflake":
         provider = cast(snowflake.Resources, provider)
```

### Comparing `relationalai-0.2.3/src/relationalai/tools/cli_controls.py` & `relationalai-0.2.4/src/relationalai/tools/cli_controls.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,19 +74,24 @@
         {"key": "c-d"}
     ],
     "skip": [
         {"key": "c-s"}
     ]
 })
 
-def prompt(message:str, value:str|None, newline=False) -> str:
+def prompt(message:str, value:str|None, newline=False, validator:callable = None, invalid_message:str|None = None) -> str:
     if value:
         return value
     try:
-        result:str = inquirer.text(message, keybindings=default_bindings).execute()
+        result:str = inquirer.text(
+            message,
+            validate=validator,
+            invalid_message=invalid_message,
+            keybindings=default_bindings
+        ).execute()
     except KeyboardInterrupt:
         abort()
         raise Exception("Unreachable")
     if newline:
         rich.print("")
     return result
 
@@ -131,17 +136,23 @@
 
 def confirm(message:str, default:bool = False) -> bool:
     try:
         return inquirer.confirm(message, default=default, keybindings=default_bindings).execute()
     except KeyboardInterrupt:
         return abort()
 
-def text(message:str, default:str|None = None) -> str:
+def text(message:str, default:str|None = None, validator:callable = None, invalid_message:str|None = None) -> str:
     try:
-        return inquirer.text(message, default=default or "", keybindings=default_bindings).execute()
+        return inquirer.text(
+            message,
+            default=default or "",
+            keybindings=default_bindings,
+            validate=validator,
+            invalid_message=invalid_message
+        ).execute()
     except KeyboardInterrupt:
         return abort()
 
 def password(message:str, default:str|None = None) -> str:
     try:
         return inquirer.secret(message, default=default or "", keybindings=default_bindings).execute()
     except KeyboardInterrupt:
```

### Comparing `relationalai-0.2.3/src/relationalai/tools/debugger.py` & `relationalai-0.2.4/src/relationalai/tools/debugger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/tools/debugger_server.py` & `relationalai-0.2.4/src/relationalai/tools/debugger_server.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/src/relationalai/tools/dev.py` & `relationalai-0.2.4/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/conftest.py` & `relationalai-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/README.md` & `relationalai-0.2.4/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_graph_visualize.py` & `relationalai-0.2.4/tests/end2end/test_graph_visualize.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.2.4/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/bool.py` & `relationalai-0.2.4/tests/end2end/test_cases/bool.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/bottom.py` & `relationalai-0.2.4/tests/end2end/test_cases/bottom.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/export.py` & `relationalai-0.2.4/tests/end2end/test_cases/export.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.2.4/tests/end2end/test_cases/multi_valued.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/not_found.py` & `relationalai-0.2.4/tests/end2end/test_cases/not_found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/persist.py` & `relationalai-0.2.4/tests/end2end/test_cases/persist.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/smoke.py` & `relationalai-0.2.4/tests/end2end/test_cases/smoke.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/strings.py` & `relationalai-0.2.4/tests/end2end/test_cases/strings.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/top.py` & `relationalai-0.2.4/tests/end2end/test_cases/top.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/union.py` & `relationalai-0.2.4/tests/end2end/test_cases/union.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.2.4/tests/end2end/test_cases/weighted_graphs.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/graphs/basics.py` & `relationalai-0.2.4/tests/end2end/test_cases/graphs/basics.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/graphs/centrality.py` & `relationalai-0.2.4/tests/end2end/test_cases/graphs/community.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import relationalai as rai
 from relationalai import std
 
 # Query snapshots are output in same order as this list.
 ALGOS = [
-    "pagerank",
-    "eigenvector_centrality",
-    "degree_centrality",
-    "betweenness_centrality",
+    "louvain",
+    "weakly_connected_component",
+    "triangle_community",  # Expects empty dataframe b/c graph has no triangles.
+    "infomap",
+    "label_propagation",
 ]
 
 model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Object = model.Type("Object")
 Relationship = model.Type("Relationship")
 
 with model.rule():
     obj1 = Object.add(id=1)
     obj2 = Object.add(id=2)
+    obj3 = Object.add(id=3)
     Relationship.add(from_=obj1, to=obj2)
 
-# eigenvector_centrality only supports undirected graphs.
 graph = std.graphs.Graph(model, undirected=True)
+graph.Node.extend(Object)
 
 with model.rule():
     r = Relationship()
     graph.Edge.add(r.from_, r.to)
 
 for algo_name in ALGOS:
     with model.query() as select:
```

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/graphs/community.py` & `relationalai-0.2.4/tests/end2end/test_cases/graphs/similarity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import relationalai as rai
 from relationalai import std
 
 # Query snapshots are output in same order as this list.
 ALGOS = [
-    "louvain",
-    "weakly_connected_component",
-    "triangle_community",  # Expects empty dataframe b/c graph has no triangles.
-    "infomap",
-    "label_propagation",
+    "jaccard_similarity",
+    "cosine_similarity",
 ]
 
 model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Object = model.Type("Object")
 Relationship = model.Type("Relationship")
 
 with model.rule():
     obj1 = Object.add(id=1)
     obj2 = Object.add(id=2)
     Relationship.add(from_=obj1, to=obj2)
 
+# cosine_similarity only supports undirected graphs.
 graph = std.graphs.Graph(model, undirected=True)
 
 with model.rule():
     r = Relationship()
     graph.Edge.add(r.from_, r.to)
 
 for algo_name in ALGOS:
     with model.query() as select:
-        o = Object()
-        algo = getattr(graph.compute, algo_name)(o)
-        select(o, algo)
+        o1 = Object()
+        o2 = Object()
+        algo = getattr(graph.compute, algo_name)(o1, o2)
+        select(o1, o2, algo)
```

### Comparing `relationalai-0.2.3/tests/end2end/test_cases/graphs/degree.py` & `relationalai-0.2.4/tests/end2end/test_cases/graphs/degree.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/init-cli/azure_basic.py` & `relationalai-0.2.4/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/init-cli/common.py` & `relationalai-0.2.4/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/roundtrip/test_document.py` & `relationalai-0.2.4/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/tests/roundtrip/test_task.py` & `relationalai-0.2.4/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.3/pyproject.toml` & `relationalai-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.2.3'
+version = '0.2.4'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `relationalai-0.2.3/PKG-INFO` & `relationalai-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.3
+Version: 0.2.4
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: gravis
```

