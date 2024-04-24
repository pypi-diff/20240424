# Comparing `tmp/bgpy_pkg-7.0.8.tar.gz` & `tmp/bgpy_pkg-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgpy_pkg-7.0.8.tar", last modified: Thu Apr 18 08:34:42 2024, max compression
+gzip compressed data, was "bgpy_pkg-7.0.9.tar", last modified: Thu Apr 18 09:10:30 2024, max compression
```

## Comparing `bgpy_pkg-7.0.8.tar` & `bgpy_pkg-7.0.9.tar`

### file list

```diff
@@ -1,198 +1,199 @@
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.135031 bgpy_pkg-7.0.8/
--rwxrwxr-x   0 anon      (1000) anon      (1000)     1460 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.8/LICENSE.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       76 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.8/MANIFEST.in
--rw-r--r--   0 anon      (1000) anon      (1000)     4622 2024-04-18 08:34:42.135031 bgpy_pkg-7.0.8/PKG-INFO
--rw-rw-r--   0 anon      (1000) anon      (1000)     1342 2024-01-31 07:10:08.000000 bgpy_pkg-7.0.8/README.md
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.115030 bgpy_pkg-7.0.8/bgpy/
--rw-rw-r--   0 anon      (1000) anon      (1000)      275 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      874 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/__main__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.115030 bgpy_pkg-7.0.8/bgpy/as_graphs/
--rw-rw-r--   0 anon      (1000) anon      (1000)      513 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/as_graphs/base/
--rw-rw-r--   0 anon      (1000) anon      (1000)      396 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/
--rw-rw-r--   0 anon      (1000) anon      (1000)       83 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     9806 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/as_graph.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     6062 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/base_as.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2444 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/customer_cone_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3185 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/graph_building_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1228 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/propagation_rank_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1821 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3769 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph_constructor.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1562 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph_info.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/as_graphs/base/links/
--rw-rw-r--   0 anon      (1000) anon      (1000)      168 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/links/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1149 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/links/customer_provider_link.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      911 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/links/link.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      687 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/base/links/peer_link.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/as_graphs/caida_as_graph/
--rw-rw-r--   0 anon      (1000) anon      (1000)      260 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/caida_as_graph/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      239 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/caida_as_graph/caida_as_graph.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3848 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/caida_as_graph/caida_as_graph_collector.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     4649 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/as_graphs/caida_as_graph/caida_as_graph_constructor.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2811 2024-04-15 22:21:08.000000 bgpy_pkg-7.0.8/bgpy/enums.py
--rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.8/bgpy/py.typed
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/simulation_engine/
--rw-rw-r--   0 anon      (1000) anon      (1000)     2311 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/
--rw-rw-r--   0 anon      (1000) anon      (1000)      302 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1717 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/ann_container.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      370 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/local_rib.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      975 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/recv_queue.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2421 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/ribs_in.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1047 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/ribs_out.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2894 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/send_queue.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     5311 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/announcement.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/
--rw-rw-r--   0 anon      (1000) anon      (1000)      590 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/aspa/
--rw-rw-r--   0 anon      (1000) anon      (1000)       98 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/aspa/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     5142 2024-04-18 08:26:10.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/aspa/aspa.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      226 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/aspa/aspa_full.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/
--rw-rw-r--   0 anon      (1000) anon      (1000)       81 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.119030 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/
--rw-rw-r--   0 anon      (1000) anon      (1000)       40 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3417 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/bgp.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2768 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/gao_rexford.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3348 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/process_incoming_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3446 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/propagate_funcs.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp_full/
--rw-rw-r--   0 anon      (1000) anon      (1000)       53 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp_full/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2918 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp_full/bgp_full.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    10946 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp_full/process_incoming_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1796 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgpsec/
--rw-rw-r--   0 anon      (1000) anon      (1000)      110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgpsec/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     4350 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgpsec/bgpsec.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      224 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgpsec/bgpsec_full.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/only_to_customers/
--rw-rw-r--   0 anon      (1000) anon      (1000)      168 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/only_to_customers/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1532 2024-03-28 08:04:49.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      294 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/only_to_customers/only_to_customers_full.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/pathend/
--rw-rw-r--   0 anon      (1000) anon      (1000)      116 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/pathend/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1129 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/pathend/pathend.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      244 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/pathend/pathend_full.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2926 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/policy.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/rov/
--rw-rw-r--   0 anon      (1000) anon      (1000)      195 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/rov/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/rov/peer_rov.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      219 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/rov/peer_rov_full.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      885 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/rov/rov.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      220 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/rov/rov_full.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_engine/simulation_engines/
--rw-rw-r--   0 anon      (1000) anon      (1000)      161 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/simulation_engines/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     3582 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/simulation_engines/base_simulation_engine.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     7142 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_engine/simulation_engines/simulation_engine.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_framework/
--rw-rw-r--   0 anon      (1000) anon      (1000)     1115 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_framework/as_graph_analyzers/
--rw-rw-r--   0 anon      (1000) anon      (1000)      157 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/as_graph_analyzers/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     6521 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/as_graph_analyzers/as_graph_analyzer.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      748 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/as_graph_analyzers/base_as_graph_analyzer.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     9418 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/graph_factory.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_framework/metric_tracker/
--rw-rw-r--   0 anon      (1000) anon      (1000)      149 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/metric_tracker/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      461 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/metric_tracker/data_key.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     4556 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/metric_tracker/metric.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      367 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/metric_tracker/metric_key.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     9936 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/metric_tracker/metric_tracker.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.123031 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/
--rw-rw-r--   0 anon      (1000) anon      (1000)      899 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.127030 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/
--rw-rw-r--   0 anon      (1000) anon      (1000)      693 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     6968 2024-03-28 08:32:38.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/accidental_route_leak.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1418 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_prefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1636 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1945 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_prefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2044 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/prefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2058 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/subprefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2381 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/superprefix_prefix_hijack.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1766 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/valid_prefix.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    16728 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/preprocess_anns_funcs.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      462 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/roa_info.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    23095 2024-04-04 07:57:43.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/scenario.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     6663 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/scenario_config.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    15693 2024-04-08 14:47:25.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/simulation.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1576 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/simulation_framework/utils.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.127030 bgpy_pkg-7.0.8/bgpy/tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)      228 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2412 2024-03-13 03:26:50.000000 bgpy_pkg-7.0.8/bgpy/tests/conftest.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.127030 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)      175 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.127030 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/
--rw-rw-r--   0 anon      (1000) anon      (1000)      180 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.131030 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/
--rw-rw-r--   0 anon      (1000) anon      (1000)     1735 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1529 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/as_graph_info_000.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      734 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_000.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      759 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_001.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_002.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      765 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_003.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      788 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_004.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      790 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_005.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      806 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_006.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      808 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_007.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      813 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_008.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      834 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_009.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      862 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_010.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      824 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_011.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      935 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_012.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      960 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_013.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1126 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_014.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1114 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_015.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1112 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_016.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1147 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_017.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_018.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1137 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_019.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1144 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_020.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      972 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_021.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      979 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1136 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1154 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1167 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1305 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1349 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_028.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.131030 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/
--rw-rw-r--   0 anon      (1000) anon      (1000)      368 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2206 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2792 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1211 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_003.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1950 2024-04-18 06:19:14.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      780 2024-04-18 07:44:17.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/test_engine.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.131030 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/utils/
--rw-rw-r--   0 anon      (1000) anon      (1000)      285 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/utils/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1757 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/utils/diagram_aggregator.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      566 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/utils/engine_test_config.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     9473 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/engine_tests/utils/engine_tester.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.131030 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.131030 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/system_tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)       76 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/system_tests/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      896 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/system_tests/test_sim_inputs.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.131030 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/unit_tests/
--rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/unit_tests/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      478 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/unit_tests/conftest.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    15144 2024-03-13 03:26:50.000000 bgpy_pkg-7.0.8/bgpy/tests/framework_tests/unit_tests/test_scenario.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.131030 bgpy_pkg-7.0.8/bgpy/utils/
--rw-rw-r--   0 anon      (1000) anon      (1000)      279 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/utils/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)    11631 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/bgpy/utils/diagram.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     1038 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/utils/engine_run_config.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     8230 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/utils/engine_runner.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.131030 bgpy_pkg-7.0.8/bgpy/utils/simulator_codec/
--rw-rw-r--   0 anon      (1000) anon      (1000)       74 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/utils/simulator_codec/__init__.py
--rw-rw-r--   0 anon      (1000) anon      (1000)     2834 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/utils/simulator_codec/simulator_codec.py
--rw-rw-r--   0 anon      (1000) anon      (1000)      322 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.8/bgpy/utils/simulator_codec/simulator_loader.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 08:34:42.135031 bgpy_pkg-7.0.8/bgpy_pkg.egg-info/
--rw-r--r--   0 anon      (1000) anon      (1000)     4622 2024-04-18 08:34:42.000000 bgpy_pkg-7.0.8/bgpy_pkg.egg-info/PKG-INFO
--rw-rw-r--   0 anon      (1000) anon      (1000)     8453 2024-04-18 08:34:42.000000 bgpy_pkg-7.0.8/bgpy_pkg.egg-info/SOURCES.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)        1 2024-04-18 08:34:42.000000 bgpy_pkg-7.0.8/bgpy_pkg.egg-info/dependency_links.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       44 2024-04-18 08:34:42.000000 bgpy_pkg-7.0.8/bgpy_pkg.egg-info/entry_points.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)      370 2024-04-18 08:34:42.000000 bgpy_pkg-7.0.8/bgpy_pkg.egg-info/requires.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)        5 2024-04-18 08:34:42.000000 bgpy_pkg-7.0.8/bgpy_pkg.egg-info/top_level.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)     3465 2024-04-18 08:28:07.000000 bgpy_pkg-7.0.8/pyproject.toml
--rwxrwxr-x   0 anon      (1000) anon      (1000)       69 2024-04-18 08:34:42.135031 bgpy_pkg-7.0.8/setup.cfg
--rw-rw-r--   0 anon      (1000) anon      (1000)     1157 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.8/tox.ini
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.414698 bgpy_pkg-7.0.9/
+-rwxrwxr-x   0 anon      (1000) anon      (1000)     1460 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.9/LICENSE.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)       76 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.9/MANIFEST.in
+-rw-r--r--   0 anon      (1000) anon      (1000)     4622 2024-04-18 09:10:30.414698 bgpy_pkg-7.0.9/PKG-INFO
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1342 2024-01-31 07:10:08.000000 bgpy_pkg-7.0.9/README.md
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.394698 bgpy_pkg-7.0.9/bgpy/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      275 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      874 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/__main__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.394698 bgpy_pkg-7.0.9/bgpy/as_graphs/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      513 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.394698 bgpy_pkg-7.0.9/bgpy/as_graphs/base/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      396 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       83 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     9806 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/as_graph.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     6062 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/base_as.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2444 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/customer_cone_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3185 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/graph_building_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1228 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/propagation_rank_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1821 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3769 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_constructor.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1562 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_info.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      168 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1149 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/customer_provider_link.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      911 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/link.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      687 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/peer_link.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      260 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      239 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3848 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph_collector.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     4649 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph_constructor.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2811 2024-04-15 22:21:08.000000 bgpy_pkg-7.0.9/bgpy/enums.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-01-30 07:34:53.000000 bgpy_pkg-7.0.9/bgpy/py.typed
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2311 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      302 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1717 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ann_container.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      370 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/local_rib.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      975 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/recv_queue.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2421 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ribs_in.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1047 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ribs_out.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2894 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/send_queue.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     5311 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/announcement.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      590 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       98 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     5142 2024-04-18 08:26:10.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/aspa.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      226 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/aspa_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       81 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       40 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3417 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/bgp.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2768 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/gao_rexford.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3348 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/process_incoming_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3446 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/propagate_funcs.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.398698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       53 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2918 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/bgp_full.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    10946 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/process_incoming_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1796 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     4350 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/bgpsec.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      224 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/bgpsec_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      168 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1532 2024-03-28 08:04:49.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      294 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/only_to_customers_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      116 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1129 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/pathend.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      244 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/pathend_full.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2926 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/policy.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      195 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/peer_rov.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      219 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/peer_rov_full.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      885 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/rov.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      220 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/rov_full.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      161 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3582 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/base_simulation_engine.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     7142 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/simulation_engine.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_framework/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1115 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      157 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     6521 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/as_graph_analyzer.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      748 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/base_as_graph_analyzer.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     9418 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/graph_factory.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      149 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      461 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/data_key.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     4556 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      367 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric_key.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     9936 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric_tracker.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.402698 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      899 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      693 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     6968 2024-03-28 08:32:38.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/accidental_route_leak.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1418 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_prefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1636 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1945 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_prefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2044 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/prefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2058 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/subprefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2381 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/superprefix_prefix_hijack.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1766 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/valid_prefix.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    16728 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/preprocess_anns_funcs.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      462 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/roa_info.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    23095 2024-04-04 07:57:43.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/scenario.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     6663 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/scenario_config.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    15693 2024-04-08 14:47:25.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/simulation.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1576 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/simulation_framework/utils.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      228 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2412 2024-03-13 03:26:50.000000 bgpy_pkg-7.0.9/bgpy/tests/conftest.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      175 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      180 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.406698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1855 2024-04-18 08:52:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1529 2024-04-18 08:48:15.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/as_graph_info_000.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      734 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_000.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      759 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_001.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_002.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      765 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_003.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      788 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_004.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      790 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_005.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      806 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_006.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      808 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_007.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      813 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_008.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      834 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_009.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      862 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_010.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      824 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_011.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      935 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_012.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      960 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_013.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1126 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_014.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1114 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_015.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1112 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_016.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1147 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_017.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1110 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_018.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1137 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_019.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1144 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_020.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      972 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_021.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      979 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1136 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1154 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1167 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1305 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1349 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_028.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1514 2024-04-18 08:54:44.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_029.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      368 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2206 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2338 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2792 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1211 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_003.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1950 2024-04-18 06:19:14.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      780 2024-04-18 07:44:17.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/test_engine.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      285 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1757 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/diagram_aggregator.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      566 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/engine_test_config.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     9473 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/engine_tester.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/system_tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       76 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/system_tests/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      896 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/system_tests/test_sim_inputs.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/
+-rw-rw-r--   0 anon      (1000) anon      (1000)        0 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      478 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/conftest.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    15144 2024-03-13 03:26:50.000000 bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/test_scenario.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/utils/
+-rw-rw-r--   0 anon      (1000) anon      (1000)      279 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)    11631 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/bgpy/utils/diagram.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1038 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/engine_run_config.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     8230 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/engine_runner.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/
+-rw-rw-r--   0 anon      (1000) anon      (1000)       74 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/__init__.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2834 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/simulator_codec.py
+-rw-rw-r--   0 anon      (1000) anon      (1000)      322 2024-02-23 22:41:12.000000 bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/simulator_loader.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2024-04-18 09:10:30.410698 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/
+-rw-r--r--   0 anon      (1000) anon      (1000)     4622 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/PKG-INFO
+-rw-rw-r--   0 anon      (1000) anon      (1000)     8523 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/SOURCES.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)        1 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/dependency_links.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)       44 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/entry_points.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)      370 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/requires.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)        5 2024-04-18 09:10:30.000000 bgpy_pkg-7.0.9/bgpy_pkg.egg-info/top_level.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)     3465 2024-04-18 09:10:06.000000 bgpy_pkg-7.0.9/pyproject.toml
+-rwxrwxr-x   0 anon      (1000) anon      (1000)       69 2024-04-18 09:10:30.414698 bgpy_pkg-7.0.9/setup.cfg
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1157 2024-02-24 05:53:40.000000 bgpy_pkg-7.0.9/tox.ini
```

### Comparing `bgpy_pkg-7.0.8/LICENSE.txt` & `bgpy_pkg-7.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/PKG-INFO` & `bgpy_pkg-7.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgpy_pkg
-Version: 7.0.8
+Version: 7.0.9
 Summary: Simulates BGP and ROV in an extensible manner
 Author-email: Justin Furuness <jfuruness@gmail.com>, Cameron Morris <cameron.morris@uconn.edu>, Reynaldo Morillo <reynaldo.morillo@uconn.edu>, Arvind Kasiliya <arvind.kasiliya@uconn.edu>
 Maintainer-email: Justin Furuness <jfuruness@gmail.com>
 License: Copyright 2020 Justin Furuness
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `bgpy_pkg-7.0.8/README.md` & `bgpy_pkg-7.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/__main__.py` & `bgpy_pkg-7.0.9/bgpy/__main__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/__init__.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/as_graph.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/as_graph.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/base_as.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/base_as.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/customer_cone_funcs.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/customer_cone_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/graph_building_funcs.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/graph_building_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph/propagation_rank_funcs.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph/propagation_rank_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph_collector.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_collector.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph_constructor.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_constructor.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/as_graph_info.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/as_graph_info.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/links/customer_provider_link.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/customer_provider_link.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/links/link.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/link.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/base/links/peer_link.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/base/links/peer_link.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/caida_as_graph/caida_as_graph_collector.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph_collector.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/as_graphs/caida_as_graph/caida_as_graph_constructor.py` & `bgpy_pkg-7.0.9/bgpy/as_graphs/caida_as_graph/caida_as_graph_constructor.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/enums.py` & `bgpy_pkg-7.0.9/bgpy/enums.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/__init__.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/ann_container.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ann_container.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/recv_queue.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/recv_queue.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/ribs_in.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ribs_in.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/ribs_out.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/ribs_out.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/ann_containers/send_queue.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/ann_containers/send_queue.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/announcement.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/announcement.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/__init__.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/aspa/aspa.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/aspa/aspa.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/bgp.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/bgp.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/gao_rexford.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/gao_rexford.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/process_incoming_funcs.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/process_incoming_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp/propagate_funcs.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp/propagate_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp_full/bgp_full.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/bgp_full.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp_full/process_incoming_funcs.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/process_incoming_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgp/bgp_full/propagate_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/bgpsec/bgpsec.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/bgpsec/bgpsec.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/only_to_customers/only_to_customers.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/pathend/pathend.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/pathend/pathend.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/policy.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/policy.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/rov/peer_rov.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/peer_rov.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/policies/rov/rov.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/policies/rov/rov.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/simulation_engines/base_simulation_engine.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/base_simulation_engine.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_engine/simulation_engines/simulation_engine.py` & `bgpy_pkg-7.0.9/bgpy/simulation_engine/simulation_engines/simulation_engine.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/__init__.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/as_graph_analyzers/as_graph_analyzer.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/as_graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/as_graph_analyzers/base_as_graph_analyzer.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/as_graph_analyzers/base_as_graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/graph_factory.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/graph_factory.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/metric_tracker/metric.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/metric_tracker/metric_tracker.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/metric_tracker/metric_tracker.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/__init__.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/__init__.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/accidental_route_leak.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/accidental_route_leak.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_prefix_hijack.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_prefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_hijack.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_prefix_hijack.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/non_routed_superprefix_prefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/prefix_hijack.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/prefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/subprefix_hijack.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/subprefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/superprefix_prefix_hijack.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/superprefix_prefix_hijack.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/custom_scenarios/valid_prefix.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/custom_scenarios/valid_prefix.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/preprocess_anns_funcs.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/preprocess_anns_funcs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/scenario.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/scenario.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/scenarios/scenario_config.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/scenarios/scenario_config.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/simulation.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/simulation.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/simulation_framework/utils.py` & `bgpy_pkg-7.0.9/bgpy/simulation_framework/utils.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/conftest.py` & `bgpy_pkg-7.0.9/bgpy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/__init__.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from .ex_config_021 import ex_config_021
 from .ex_config_022 import ex_config_022
 from .ex_config_023 import ex_config_023
 from .ex_config_024 import ex_config_024
 from .ex_config_025 import ex_config_025
 from .ex_config_026 import ex_config_026
 from .ex_config_027 import ex_config_027
+from .ex_config_028 import ex_config_028
+from .ex_config_029 import ex_config_029
 
 
 example_configs = [
     ex_config_000,
     ex_config_001,
     ex_config_002,
     ex_config_003,
@@ -53,10 +55,12 @@
     ex_config_021,
     ex_config_022,
     ex_config_023,
     ex_config_024,
     ex_config_025,
     ex_config_026,
     ex_config_027,
+    ex_config_028,
+    ex_config_029,
 ]
 
 __all__ = ["example_configs"]
```

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/as_graph_info_000.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/as_graph_info_000.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_000.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_000.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_001.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_001.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_002.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_002.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_003.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_003.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_004.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_004.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_005.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_005.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_006.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_006.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_007.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_007.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_008.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_008.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_009.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_009.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_010.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_010.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_011.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_011.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_012.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_012.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_013.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_013.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_014.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_014.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_015.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_015.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_016.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_016.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_017.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_017.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_018.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_018.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_019.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_019.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_020.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_020.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_021.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_021.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_028.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_028.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_003.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_003.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/test_engine.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/utils/diagram_aggregator.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/diagram_aggregator.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/utils/engine_test_config.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/engine_test_config.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/engine_tests/utils/engine_tester.py` & `bgpy_pkg-7.0.9/bgpy/tests/engine_tests/utils/engine_tester.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/framework_tests/system_tests/test_sim_inputs.py` & `bgpy_pkg-7.0.9/bgpy/tests/framework_tests/system_tests/test_sim_inputs.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/tests/framework_tests/unit_tests/test_scenario.py` & `bgpy_pkg-7.0.9/bgpy/tests/framework_tests/unit_tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/utils/diagram.py` & `bgpy_pkg-7.0.9/bgpy/utils/diagram.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/utils/engine_run_config.py` & `bgpy_pkg-7.0.9/bgpy/utils/engine_run_config.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/utils/engine_runner.py` & `bgpy_pkg-7.0.9/bgpy/utils/engine_runner.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy/utils/simulator_codec/simulator_codec.py` & `bgpy_pkg-7.0.9/bgpy/utils/simulator_codec/simulator_codec.py`

 * *Files identical despite different names*

### Comparing `bgpy_pkg-7.0.8/bgpy_pkg.egg-info/PKG-INFO` & `bgpy_pkg-7.0.9/bgpy_pkg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgpy_pkg
-Version: 7.0.8
+Version: 7.0.9
 Summary: Simulates BGP and ROV in an extensible manner
 Author-email: Justin Furuness <jfuruness@gmail.com>, Cameron Morris <cameron.morris@uconn.edu>, Reynaldo Morillo <reynaldo.morillo@uconn.edu>, Arvind Kasiliya <arvind.kasiliya@uconn.edu>
 Maintainer-email: Justin Furuness <jfuruness@gmail.com>
 License: Copyright 2020 Justin Furuness
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `bgpy_pkg-7.0.8/bgpy_pkg.egg-info/SOURCES.txt` & `bgpy_pkg-7.0.9/bgpy_pkg.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_022.py
 bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_023.py
 bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_024.py
 bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_025.py
 bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_026.py
 bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_027.py
 bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_028.py
+bgpy/tests/engine_tests/engine_test_configs/examples/ex_config_029.py
 bgpy/tests/engine_tests/engine_test_configs/internals/__init__.py
 bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_000.py
 bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_001.py
 bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_002.py
 bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_003.py
 bgpy/tests/engine_tests/engine_test_configs/internals/internal_config_004.py
 bgpy/tests/engine_tests/utils/__init__.py
```

### Comparing `bgpy_pkg-7.0.8/pyproject.toml` & `bgpy_pkg-7.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bgpy_pkg"
-version = "7.0.8"
+version = "7.0.9"
 requires-python = ">=3.10"
 description = "Simulates BGP and ROV in an extensible manner"
 readme = "README.md"
 authors = [
     {name = "Justin Furuness", email = "jfuruness@gmail.com"},
     {name = "Cameron Morris", email = "cameron.morris@uconn.edu"},
     {name = "Reynaldo Morillo", email = "reynaldo.morillo@uconn.edu"},
```

### Comparing `bgpy_pkg-7.0.8/tox.ini` & `bgpy_pkg-7.0.9/tox.ini`

 * *Files identical despite different names*

