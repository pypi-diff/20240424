# Comparing `tmp/job_shop_lib-0.1.3.tar.gz` & `tmp/job_shop_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "job_shop_lib-0.1.3.tar", max compression
+gzip compressed data, was "job_shop_lib-0.2.0.tar", max compression
```

## Comparing `job_shop_lib-0.1.3.tar` & `job_shop_lib-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1069 2024-02-06 16:50:21.344036 job_shop_lib-0.1.3/LICENSE
--rw-r--r--   0        0        0    11815 2024-04-17 21:41:52.158608 job_shop_lib-0.1.3/README.md
--rw-r--r--   0        0        0      581 2024-04-17 18:49:25.563004 job_shop_lib-0.1.3/job_shop_lib/__init__.py
--rw-r--r--   0        0        0     1368 2024-04-17 18:49:22.658989 job_shop_lib-0.1.3/job_shop_lib/base_solver.py
--rw-r--r--   0        0        0     3354 2024-04-17 18:29:10.381234 job_shop_lib-0.1.3/job_shop_lib/benchmarking/__init__.py
--rw-r--r--   0        0        0   464841 2024-03-01 17:52:19.596032 job_shop_lib-0.1.3/job_shop_lib/benchmarking/benchmark_instances.json
--rw-r--r--   0        0        0     5625 2024-04-13 15:45:21.680914 job_shop_lib-0.1.3/job_shop_lib/benchmarking/load_benchmark.py
--rw-r--r--   0        0        0       97 2024-04-13 17:42:22.701917 job_shop_lib-0.1.3/job_shop_lib/cp_sat/__init__.py
--rw-r--r--   0        0        0     8130 2024-04-17 18:26:23.704578 job_shop_lib-0.1.3/job_shop_lib/cp_sat/ortools_solver.py
--rw-r--r--   0        0        0     1432 2024-04-17 18:51:16.107562 job_shop_lib-0.1.3/job_shop_lib/dispatching/__init__.py
--rw-r--r--   0        0        0    10135 2024-04-17 18:40:15.600273 job_shop_lib-0.1.3/job_shop_lib/dispatching/dispatcher.py
--rw-r--r--   0        0        0     4392 2024-04-17 18:50:15.491255 job_shop_lib-0.1.3/job_shop_lib/dispatching/dispatching_rule_solver.py
--rw-r--r--   0        0        0     5557 2024-04-17 14:11:05.549956 job_shop_lib-0.1.3/job_shop_lib/dispatching/dispatching_rules.py
--rw-r--r--   0        0        0     7267 2024-04-17 18:36:42.623252 job_shop_lib-0.1.3/job_shop_lib/dispatching/factories.py
--rw-r--r--   0        0        0     4378 2024-04-17 14:09:16.084490 job_shop_lib-0.1.3/job_shop_lib/dispatching/pruning_functions.py
--rw-r--r--   0        0        0      899 2024-04-16 16:26:15.416010 job_shop_lib-0.1.3/job_shop_lib/exceptions.py
--rw-r--r--   0        0        0      154 2024-04-17 18:37:08.259373 job_shop_lib-0.1.3/job_shop_lib/generators/__init__.py
--rw-r--r--   0        0        0     7533 2024-04-17 18:37:26.163458 job_shop_lib-0.1.3/job_shop_lib/generators/basic_generator.py
--rw-r--r--   0        0        0     1454 2024-04-17 18:38:06.339650 job_shop_lib-0.1.3/job_shop_lib/graphs/__init__.py
--rw-r--r--   0        0        0     7128 2024-04-02 19:34:54.999808 job_shop_lib-0.1.3/job_shop_lib/graphs/build_agent_task_graph.py
--rw-r--r--   0        0        0     2877 2024-04-17 18:51:04.799505 job_shop_lib-0.1.3/job_shop_lib/graphs/build_disjunctive_graph.py
--rw-r--r--   0        0        0      374 2024-03-27 15:56:38.467324 job_shop_lib-0.1.3/job_shop_lib/graphs/constants.py
--rw-r--r--   0        0        0     5972 2024-04-02 19:26:46.141395 job_shop_lib-0.1.3/job_shop_lib/graphs/job_shop_graph.py
--rw-r--r--   0        0        0     4880 2024-03-28 10:18:53.973376 job_shop_lib-0.1.3/job_shop_lib/graphs/node.py
--rw-r--r--   0        0        0    12801 2024-04-03 10:47:39.697352 job_shop_lib-0.1.3/job_shop_lib/job_shop_instance.py
--rw-r--r--   0        0        0     3862 2024-04-06 19:26:36.742129 job_shop_lib-0.1.3/job_shop_lib/operation.py
--rw-r--r--   0        0        0     6509 2024-04-11 17:06:21.882095 job_shop_lib-0.1.3/job_shop_lib/schedule.py
--rw-r--r--   0        0        0     3127 2024-04-11 17:12:11.243224 job_shop_lib-0.1.3/job_shop_lib/scheduled_operation.py
--rw-r--r--   0        0        0      693 2024-04-17 18:46:13.614040 job_shop_lib-0.1.3/job_shop_lib/visualization/__init__.py
--rw-r--r--   0        0        0     8284 2024-04-03 10:47:25.781302 job_shop_lib-0.1.3/job_shop_lib/visualization/agent_task_graph.py
--rw-r--r--   0        0        0     6382 2024-04-17 18:51:20.995586 job_shop_lib-0.1.3/job_shop_lib/visualization/create_gif.py
--rw-r--r--   0        0        0     5803 2024-04-17 18:49:29.543024 job_shop_lib-0.1.3/job_shop_lib/visualization/disjunctive_graph.py
--rw-r--r--   0        0        0     4415 2024-04-17 18:52:22.519817 job_shop_lib-0.1.3/job_shop_lib/visualization/gantt_chart.py
--rw-r--r--   0        0        0     1352 2024-04-17 21:54:32.534998 job_shop_lib-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    12622 1970-01-01 00:00:00.000000 job_shop_lib-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-02-06 16:50:21.344036 job_shop_lib-0.2.0/LICENSE
+-rw-r--r--   0        0        0    11817 2024-04-24 20:06:27.816437 job_shop_lib-0.2.0/README.md
+-rw-r--r--   0        0        0      581 2024-04-17 18:49:25.563004 job_shop_lib-0.2.0/job_shop_lib/__init__.py
+-rw-r--r--   0        0        0     1368 2024-04-17 18:49:22.658989 job_shop_lib-0.2.0/job_shop_lib/base_solver.py
+-rw-r--r--   0        0        0     3354 2024-04-17 18:29:10.381234 job_shop_lib-0.2.0/job_shop_lib/benchmarking/__init__.py
+-rw-r--r--   0        0        0   464841 2024-03-01 17:52:19.596032 job_shop_lib-0.2.0/job_shop_lib/benchmarking/benchmark_instances.json
+-rw-r--r--   0        0        0     5625 2024-04-13 15:45:21.680914 job_shop_lib-0.2.0/job_shop_lib/benchmarking/load_benchmark.py
+-rw-r--r--   0        0        0       97 2024-04-13 17:42:22.701917 job_shop_lib-0.2.0/job_shop_lib/cp_sat/__init__.py
+-rw-r--r--   0        0        0     8130 2024-04-17 18:26:23.704578 job_shop_lib-0.2.0/job_shop_lib/cp_sat/ortools_solver.py
+-rw-r--r--   0        0        0     1432 2024-04-17 18:51:16.107562 job_shop_lib-0.2.0/job_shop_lib/dispatching/__init__.py
+-rw-r--r--   0        0        0    10135 2024-04-17 18:40:15.600273 job_shop_lib-0.2.0/job_shop_lib/dispatching/dispatcher.py
+-rw-r--r--   0        0        0     4392 2024-04-17 18:50:15.491255 job_shop_lib-0.2.0/job_shop_lib/dispatching/dispatching_rule_solver.py
+-rw-r--r--   0        0        0     5557 2024-04-17 14:11:05.549956 job_shop_lib-0.2.0/job_shop_lib/dispatching/dispatching_rules.py
+-rw-r--r--   0        0        0     7267 2024-04-17 18:36:42.623252 job_shop_lib-0.2.0/job_shop_lib/dispatching/factories.py
+-rw-r--r--   0        0        0     4378 2024-04-17 14:09:16.084490 job_shop_lib-0.2.0/job_shop_lib/dispatching/pruning_functions.py
+-rw-r--r--   0        0        0      899 2024-04-16 16:26:15.416010 job_shop_lib-0.2.0/job_shop_lib/exceptions.py
+-rw-r--r--   0        0        0      154 2024-04-17 18:37:08.259373 job_shop_lib-0.2.0/job_shop_lib/generators/__init__.py
+-rw-r--r--   0        0        0     7533 2024-04-17 18:37:26.163458 job_shop_lib-0.2.0/job_shop_lib/generators/basic_generator.py
+-rw-r--r--   0        0        0     5290 2024-04-24 20:22:00.457532 job_shop_lib-0.2.0/job_shop_lib/generators/transformations.py
+-rw-r--r--   0        0        0     1454 2024-04-17 18:38:06.339650 job_shop_lib-0.2.0/job_shop_lib/graphs/__init__.py
+-rw-r--r--   0        0        0     7128 2024-04-02 19:34:54.999808 job_shop_lib-0.2.0/job_shop_lib/graphs/build_agent_task_graph.py
+-rw-r--r--   0        0        0     2877 2024-04-17 18:51:04.799505 job_shop_lib-0.2.0/job_shop_lib/graphs/build_disjunctive_graph.py
+-rw-r--r--   0        0        0      374 2024-03-27 15:56:38.467324 job_shop_lib-0.2.0/job_shop_lib/graphs/constants.py
+-rw-r--r--   0        0        0     5972 2024-04-02 19:26:46.141395 job_shop_lib-0.2.0/job_shop_lib/graphs/job_shop_graph.py
+-rw-r--r--   0        0        0     4880 2024-03-28 10:18:53.973376 job_shop_lib-0.2.0/job_shop_lib/graphs/node.py
+-rw-r--r--   0        0        0    12801 2024-04-03 10:47:39.697352 job_shop_lib-0.2.0/job_shop_lib/job_shop_instance.py
+-rw-r--r--   0        0        0     3862 2024-04-06 19:26:36.742129 job_shop_lib-0.2.0/job_shop_lib/operation.py
+-rw-r--r--   0        0        0     6509 2024-04-11 17:06:21.882095 job_shop_lib-0.2.0/job_shop_lib/schedule.py
+-rw-r--r--   0        0        0     3127 2024-04-11 17:12:11.243224 job_shop_lib-0.2.0/job_shop_lib/scheduled_operation.py
+-rw-r--r--   0        0        0      693 2024-04-17 18:46:13.614040 job_shop_lib-0.2.0/job_shop_lib/visualization/__init__.py
+-rw-r--r--   0        0        0     8284 2024-04-03 10:47:25.781302 job_shop_lib-0.2.0/job_shop_lib/visualization/agent_task_graph.py
+-rw-r--r--   0        0        0     6382 2024-04-17 18:51:20.995586 job_shop_lib-0.2.0/job_shop_lib/visualization/create_gif.py
+-rw-r--r--   0        0        0     5803 2024-04-17 18:49:29.543024 job_shop_lib-0.2.0/job_shop_lib/visualization/disjunctive_graph.py
+-rw-r--r--   0        0        0     4415 2024-04-17 18:52:22.519817 job_shop_lib-0.2.0/job_shop_lib/visualization/gantt_chart.py
+-rw-r--r--   0        0        0     1352 2024-04-24 20:24:10.345796 job_shop_lib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12624 1970-01-01 00:00:00.000000 job_shop_lib-0.2.0/PKG-INFO
```

### Comparing `job_shop_lib-0.1.3/LICENSE` & `job_shop_lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/README.md` & `job_shop_lib-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 [![Tests](https://github.com/Pabloo22/job_shop_lib/actions/workflows/tests.yaml/badge.svg)](https://github.com/Pabloo22/job_shop_lib/actions/workflows/tests.yaml)
 ![Python versions](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 </div>
 
-
-
 An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP) with a special focus on graph representations.
 
 It provides intuitive data structures to represent instances and solutions, as well as solvers and visualization tools.
 
 See the [this](https://colab.research.google.com/drive/1XV_Rvq1F2ns6DFG8uNj66q_rcowwTZ4H?usp=sharing) Google Colab notebook for a quick start guide! 
 
 ## Installation
@@ -148,15 +146,15 @@
     RANDOM = "random"
 ```
 
 We can visualize the solution with a `DispatchingRuleSolver` as a gif:
 
 ```python
 from job_shop_lib.visualization import create_gif, get_plot_function
-from job_shop_lib.solvers import DispatchingRuleSolver, DispatchingRule
+from job_shop_lib.dispatching import DispatchingRuleSolver, DispatchingRule
 
 plt.style.use("ggplot")
 
 mwkr_solver = DispatchingRuleSolver("most_work_remaining")
 plot_function = get_plot_function(title="Solution with Most Work Remaining Rule")
 create_gif(
     gif_path="ft06_optimized.gif",
```

### Comparing `job_shop_lib-0.1.3/job_shop_lib/__init__.py` & `job_shop_lib-0.2.0/job_shop_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/base_solver.py` & `job_shop_lib-0.2.0/job_shop_lib/base_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/benchmarking/__init__.py` & `job_shop_lib-0.2.0/job_shop_lib/benchmarking/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/benchmarking/benchmark_instances.json` & `job_shop_lib-0.2.0/job_shop_lib/benchmarking/benchmark_instances.json`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/benchmarking/load_benchmark.py` & `job_shop_lib-0.2.0/job_shop_lib/benchmarking/load_benchmark.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/cp_sat/ortools_solver.py` & `job_shop_lib-0.2.0/job_shop_lib/cp_sat/ortools_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/dispatching/__init__.py` & `job_shop_lib-0.2.0/job_shop_lib/dispatching/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/dispatching/dispatcher.py` & `job_shop_lib-0.2.0/job_shop_lib/dispatching/dispatcher.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/dispatching/dispatching_rule_solver.py` & `job_shop_lib-0.2.0/job_shop_lib/dispatching/dispatching_rule_solver.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/dispatching/dispatching_rules.py` & `job_shop_lib-0.2.0/job_shop_lib/dispatching/dispatching_rules.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/dispatching/factories.py` & `job_shop_lib-0.2.0/job_shop_lib/dispatching/factories.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/dispatching/pruning_functions.py` & `job_shop_lib-0.2.0/job_shop_lib/dispatching/pruning_functions.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/exceptions.py` & `job_shop_lib-0.2.0/job_shop_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/generators/basic_generator.py` & `job_shop_lib-0.2.0/job_shop_lib/generators/basic_generator.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/graphs/__init__.py` & `job_shop_lib-0.2.0/job_shop_lib/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/graphs/build_agent_task_graph.py` & `job_shop_lib-0.2.0/job_shop_lib/graphs/build_agent_task_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/graphs/build_disjunctive_graph.py` & `job_shop_lib-0.2.0/job_shop_lib/graphs/build_disjunctive_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/graphs/job_shop_graph.py` & `job_shop_lib-0.2.0/job_shop_lib/graphs/job_shop_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/graphs/node.py` & `job_shop_lib-0.2.0/job_shop_lib/graphs/node.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/job_shop_instance.py` & `job_shop_lib-0.2.0/job_shop_lib/job_shop_instance.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/operation.py` & `job_shop_lib-0.2.0/job_shop_lib/operation.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/schedule.py` & `job_shop_lib-0.2.0/job_shop_lib/schedule.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/scheduled_operation.py` & `job_shop_lib-0.2.0/job_shop_lib/scheduled_operation.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/visualization/__init__.py` & `job_shop_lib-0.2.0/job_shop_lib/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/visualization/agent_task_graph.py` & `job_shop_lib-0.2.0/job_shop_lib/visualization/agent_task_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/visualization/create_gif.py` & `job_shop_lib-0.2.0/job_shop_lib/visualization/create_gif.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/visualization/disjunctive_graph.py` & `job_shop_lib-0.2.0/job_shop_lib/visualization/disjunctive_graph.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/job_shop_lib/visualization/gantt_chart.py` & `job_shop_lib-0.2.0/job_shop_lib/visualization/gantt_chart.py`

 * *Files identical despite different names*

### Comparing `job_shop_lib-0.1.3/pyproject.toml` & `job_shop_lib-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "job-shop-lib"
-version = "0.1.3"
+version = "0.2.0"
 description = "An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP)"
 authors = ["Pabloo22 <pablete.arino@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "job_shop_lib"}]
 include = ["benchmarks/benchmark_instances.json"]
```

### Comparing `job_shop_lib-0.1.3/PKG-INFO` & `job_shop_lib-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: job-shop-lib
-Version: 0.1.3
+Version: 0.2.0
 Summary: An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP)
 License: MIT
 Author: Pabloo22
 Author-email: pablete.arino@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,16 +29,14 @@
 [![Tests](https://github.com/Pabloo22/job_shop_lib/actions/workflows/tests.yaml/badge.svg)](https://github.com/Pabloo22/job_shop_lib/actions/workflows/tests.yaml)
 ![Python versions](https://img.shields.io/badge/python-3.10%20%7C%203.11%20%7C%203.12-blue)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 </div>
 
-
-
 An easy-to-use and modular Python library for the Job Shop Scheduling Problem (JSSP) with a special focus on graph representations.
 
 It provides intuitive data structures to represent instances and solutions, as well as solvers and visualization tools.
 
 See the [this](https://colab.research.google.com/drive/1XV_Rvq1F2ns6DFG8uNj66q_rcowwTZ4H?usp=sharing) Google Colab notebook for a quick start guide! 
 
 ## Installation
@@ -170,15 +168,15 @@
     RANDOM = "random"
 ```
 
 We can visualize the solution with a `DispatchingRuleSolver` as a gif:
 
 ```python
 from job_shop_lib.visualization import create_gif, get_plot_function
-from job_shop_lib.solvers import DispatchingRuleSolver, DispatchingRule
+from job_shop_lib.dispatching import DispatchingRuleSolver, DispatchingRule
 
 plt.style.use("ggplot")
 
 mwkr_solver = DispatchingRuleSolver("most_work_remaining")
 plot_function = get_plot_function(title="Solution with Most Work Remaining Rule")
 create_gif(
     gif_path="ft06_optimized.gif",
```

