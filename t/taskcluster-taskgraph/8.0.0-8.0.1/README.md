# Comparing `tmp/taskcluster-taskgraph-8.0.0.tar.gz` & `tmp/taskcluster-taskgraph-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-8.0.0.tar", last modified: Tue Apr  9 15:51:35 2024, max compression
+gzip compressed data, was "taskcluster-taskgraph-8.0.1.tar", last modified: Wed Apr 24 18:32:32 2024, max compression
```

## Comparing `taskcluster-taskgraph-8.0.0.tar` & `taskcluster-taskgraph-8.0.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.706315 taskcluster-taskgraph-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-09 15:51:35.706315 taskcluster-taskgraph-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.686315 taskcluster-taskgraph-8.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:51:35.706315 taskcluster-taskgraph-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.682315 taskcluster-taskgraph-8.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.686315 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12943 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/filter_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/loader/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/loader/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    29064 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/morph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18982 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/
--rwxr-xr-x   0 runner    (1001) docker     (127)    29990 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/hgrc
--rw-r--r--   0 runner    (1001) docker     (127)    30813 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45753 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/run-task
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/target_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.694315 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/from_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.694315 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/
--rw-r--r--   0 runner    (1001) docker     (127)    17731 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    52586 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/task_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.698315 taskcluster-taskgraph-8.0.0/src/taskgraph/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/set_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/treeherder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/workertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.706315 taskcluster-taskgraph-8.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_actions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_morph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_optimize_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_scripts_fetch_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_scripts_run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_target_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_taskgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transform_chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transform_docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transform_task_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_from_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_run_run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_run_toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_readonlydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_taskcluster.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_treeherder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_workertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.512606 taskcluster-taskgraph-8.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-24 18:32:32.512606 taskcluster-taskgraph-8.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.492606 taskcluster-taskgraph-8.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:32:32.512606 taskcluster-taskgraph-8.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.488606 taskcluster-taskgraph-8.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.492606 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/loader/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/loader/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29072 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/morph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18982 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29990 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 runner    (1001) docker     (127)    30813 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45753 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/run-task
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/target_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.500606 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/from_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.500606 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/
+-rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52586 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/task_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.504606 taskcluster-taskgraph-8.0.1/src/taskgraph/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/set_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.512606 taskcluster-taskgraph-8.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_actions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_morph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_optimize_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_scripts_fetch_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_scripts_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_target_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_taskgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transform_chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transform_docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transform_task_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_from_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_run_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_run_toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_readonlydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_taskcluster.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_treeherder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_workertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_yaml.py
```

### Comparing `taskcluster-taskgraph-8.0.0/LICENSE` & `taskcluster-taskgraph-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/PKG-INFO` & `taskcluster-taskgraph-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 8.0.0
+Version: 8.0.1
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `taskcluster-taskgraph-8.0.0/README.rst` & `taskcluster-taskgraph-8.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/pyproject.toml` & `taskcluster-taskgraph-8.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/requirements/base.txt` & `taskcluster-taskgraph-8.0.1/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/requirements/dev.txt` & `taskcluster-taskgraph-8.0.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/requirements/test.txt` & `taskcluster-taskgraph-8.0.1/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/setup.py` & `taskcluster-taskgraph-8.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 8.0.0
+Version: 8.0.1
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 src/taskgraph/util/verify.py
 src/taskgraph/util/workertypes.py
 src/taskgraph/util/yaml.py
 test/test_actions_rebuild_cached_tasks.py
 test/test_actions_registry.py
 test/test_create.py
 test/test_decision.py
+test/test_docker.py
 test/test_generator.py
 test/test_graph.py
 test/test_main.py
 test/test_morph.py
 test/test_optimize.py
 test/test_optimize_strategies.py
 test/test_parameters.py
@@ -116,15 +117,14 @@
 test/test_transforms_run_toolchain.py
 test/test_transforms_task.py
 test/test_util_archive.py
 test/test_util_attributes.py
 test/test_util_cached_tasks.py
 test/test_util_dependencies.py
 test/test_util_docker.py
-test/test_util_memoize.py
 test/test_util_parameterization.py
 test/test_util_path.py
 test/test_util_python_path.py
 test/test_util_readonlydict.py
 test/test_util_schema.py
 test/test_util_taskcluster.py
 test/test_util_templates.py
```

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/__init__.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "8.0.0"
+__version__ = "8.0.1"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/config.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/create.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/decision.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/decision.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,17 @@
         candidate_base_rev=options.get("base_rev"),
         head_rev=options.get("head_rev"),
         env_prefix=_get_env_prefix(graph_config),
     )
 
     # Define default filter list, as most configurations shouldn't need
     # custom filters.
-    parameters["files_changed"] = repo.get_changed_files("AM")
+    parameters["files_changed"] = repo.get_changed_files(
+        rev=parameters["head_rev"], base_rev=parameters["base_rev"]
+    )
     parameters["filters"] = [
         "target_tasks_method",
     ]
     parameters["optimize_strategies"] = None
     parameters["optimize_target_tasks"] = True
     parameters["existing_tasks"] = {}
     parameters["do_not_optimize"] = []
```

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/docker.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/docker.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,30 @@
     import zstandard as zstd
 except ImportError as e:
     zstd = e
 
 from taskgraph.util import docker
 from taskgraph.util.taskcluster import get_artifact_url, get_session
 
+DEPLOY_WARNING = """
+*****************************************************************
+WARNING: Image is not suitable for deploying/pushing.
+
+To automatically tag the image the following files are required:
+- {image_dir}/REGISTRY
+- {image_dir}/VERSION
+
+The REGISTRY file contains the Docker registry hosting the image.
+A default REGISTRY file may also be defined in the parent docker
+directory.
+
+The VERSION file contains the version of the image.
+*****************************************************************
+"""
+
 
 def get_image_digest(image_name):
     from taskgraph.generator import load_tasks_for_kind
     from taskgraph.parameters import Parameters
 
     params = Parameters(
         level=os.environ.get("MOZ_SCM_LEVEL", "3"),
@@ -101,27 +117,26 @@
     if not os.path.isdir(image_dir):
         raise Exception("image directory does not exist: %s" % image_dir)
 
     tag = tag or docker.docker_image(name, by_tag=True)
 
     buf = BytesIO()
     docker.stream_context_tar(".", image_dir, buf, "", args)
-    subprocess.run(
-        ["docker", "image", "build", "--no-cache", "-t", tag, "-"], input=buf.getvalue()
-    )
+    cmdargs = ["docker", "image", "build", "--no-cache", "-"]
+    if tag:
+        cmdargs.insert(-1, f"-t={tag}")
+    subprocess.run(cmdargs, input=buf.getvalue())
 
-    print(f"Successfully built {name} and tagged with {tag}")
+    msg = f"Successfully built {name}"
+    if tag:
+        msg += f" and tagged with {tag}"
+    print(msg)
 
-    if tag.endswith(":latest"):
-        print("*" * 50)
-        print("WARNING: no VERSION file found in image directory.")
-        print("Image is not suitable for deploying/pushing.")
-        print("Create an image suitable for deploying/pushing by creating")
-        print("a VERSION file in the image directory.")
-        print("*" * 50)
+    if not tag or tag.endswith(":latest"):
+        print(DEPLOY_WARNING.format(image_dir=os.path.relpath(image_dir), image=name))
 
 
 def load_image(url, imageName=None, imageTag=None):
     """
     Load docker image from URL as imageName:tag, if no imageName or tag is given
     it will use whatever is inside the zstd compressed tarball.
```

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/generator.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/graph.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/main.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     if exclude_keys:
         for label, task in taskgraph.tasks.items():
             task = task.to_json()
             for key in exclude_keys:
                 obj = task
                 attrs = key.split(".")
-                while attrs[0] in obj:
+                while obj and attrs[0] in obj:
                     if len(attrs) == 1:
                         del obj[attrs[0]]
                         break
                     obj = obj[attrs[0]]
                     attrs = attrs[1:]
             taskgraph.tasks[label] = Task.from_json(task)
```

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/morph.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/parameters.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/task.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/chunking.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/chunking.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/__init__.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,16 @@
 def add_resource_monitor(config, tasks):
     for task in tasks:
         if task.get("attributes", {}).get("resource-monitor"):
             worker_implementation, worker_os = worker_type_implementation(
                 config.graph_config, task["worker-type"]
             )
             # Normalise worker os so that linux-bitbar and similar use linux tools.
-            worker_os = worker_os.split("-")[0]
+            if worker_os:
+                worker_os = worker_os.split("-")[0]
             if "win7" in task["worker-type"]:
                 arch = "32"
             else:
                 arch = "64"
             task.setdefault("fetches", {})
             task["fetches"].setdefault("toolchain", [])
             task["fetches"]["toolchain"].append(f"{worker_os}{arch}-resource-monitor")
```

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/common.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/index_search.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/run_task.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/toolchain.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/task_context.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/docker.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,42 +3,53 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 import hashlib
 import io
 import os
 import re
+from typing import Optional
 
 from taskgraph.util.archive import create_tar_gz_from_files
 from taskgraph.util.memoize import memoize
 
 IMAGE_DIR = os.path.join(".", "taskcluster", "docker")
 
 from .yaml import load_yaml
 
 
-def docker_image(name, by_tag=False):
+def docker_image(name: str, by_tag: bool = False) -> Optional[str]:
     """
     Resolve in-tree prebuilt docker image to ``<registry>/<repository>@sha256:<digest>``,
     or ``<registry>/<repository>:<tag>`` if `by_tag` is `True`.
+
+    Args:
+        name (str): The image to build.
+        by_tag (bool): If True, will apply a tag based on VERSION file.
+            Otherwise will apply a hash based on HASH file.
+    Returns:
+        Optional[str]: Image if it can be resolved, otherwise None.
     """
     try:
         with open(os.path.join(IMAGE_DIR, name, "REGISTRY")) as f:
             registry = f.read().strip()
     except OSError:
-        with open(os.path.join(IMAGE_DIR, "REGISTRY")) as f:
-            registry = f.read().strip()
+        try:
+            with open(os.path.join(IMAGE_DIR, "REGISTRY")) as f:
+                registry = f.read().strip()
+        except OSError:
+            return None
 
     if not by_tag:
         hashfile = os.path.join(IMAGE_DIR, name, "HASH")
         try:
             with open(hashfile) as f:
                 return f"{registry}/{name}@{f.read().strip()}"
         except OSError:
-            raise Exception(f"Failed to read HASH file {hashfile}")
+            return None
 
     try:
         with open(os.path.join(IMAGE_DIR, name, "VERSION")) as f:
             tag = f.read().strip()
     except OSError:
         tag = "latest"
     return f"{registry}/{name}:{tag}"
```

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/path.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/set_name.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/set_name.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/time.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-8.0.1/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-8.0.1/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_actions_registry.py` & `taskcluster-taskgraph-8.0.1/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_create.py` & `taskcluster-taskgraph-8.0.1/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_decision.py` & `taskcluster-taskgraph-8.0.1/test/test_decision.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,75 +42,86 @@
             self.assertEqual(load_yaml(decision.ARTIFACTS_DIR, "artifact.yml"), data)
         finally:
             if os.path.exists(tmpdir):
                 shutil.rmtree(tmpdir)
             decision.ARTIFACTS_DIR = Path("artifacts")
 
 
+@unittest.mock.patch.object(
+    GitRepository,
+    "get_changed_files",
+)
 class TestGetDecisionParameters(unittest.TestCase):
     def setUp(self):
         self.options = {
             "base_repository": "https://hg.mozilla.org/mozilla-unified",
             "head_repository": "https://hg.mozilla.org/mozilla-central",
-            "head_rev": "abcd",
+            "head_rev": "bbbb",
             "head_ref": "default",
             "head_tag": "v0.0.1",
             "project": "mozilla-central",
             "pushlog_id": "143",
             "pushdate": 1503691511,
             "repository_type": "hg",
             "optimize_strategies": None,
             "owner": "nobody@mozilla.com",
             "tasks_for": "hg-push",
             "level": "3",
         }
         self.old_determine_more_accurate_base_rev = (
             decision._determine_more_accurate_base_rev
         )
-        decision._determine_more_accurate_base_rev = lambda *_, **__: "abcd"
+        decision._determine_more_accurate_base_rev = lambda *_, **__: "aaaa"
         self.old_determine_more_accurate_base_ref = (
             decision._determine_more_accurate_base_ref
         )
-        decision._determine_more_accurate_base_ref = lambda *_, **__: "abcd"
+        decision._determine_more_accurate_base_ref = lambda *_, **__: "aaaa"
 
     def tearDown(self):
         decision._determine_more_accurate_base_rev = (
             self.old_determine_more_accurate_base_rev
         )
         decision._determine_more_accurate_base_ref = (
             self.old_determine_more_accurate_base_ref
         )
 
-    def test_simple_options(self):
+    def test_simple_options(self, mock_files_changed):
+        mock_files_changed.return_value = ["foo.txt"]
         params = decision.get_decision_parameters(FAKE_GRAPH_CONFIG, self.options)
+        mock_files_changed.assert_called_once_with(rev="bbbb", base_rev="aaaa")
         self.assertEqual(params["build_date"], 1503691511)
         self.assertEqual(params["head_tag"], "v0.0.1")
         self.assertEqual(params["pushlog_id"], "143")
         self.assertEqual(params["moz_build_date"], "20170825200511")
+        self.assertEqual(params["files_changed"], ["foo.txt"])
 
-    def test_no_email_owner(self):
+    def test_no_email_owner(self, mock_files_changed):
+        mock_files_changed.return_value = ["foo.txt"]
         self.options["owner"] = "ffxbld"
         params = decision.get_decision_parameters(FAKE_GRAPH_CONFIG, self.options)
         self.assertEqual(params["owner"], "ffxbld@noreply.mozilla.org")
 
     @unittest.mock.patch.object(
         GitRepository,
         "get_commit_message",
         unittest.mock.MagicMock(return_value="Add Foo"),
     )
     @unittest.mock.patch.object(
         HgRepository,
         "get_commit_message",
         unittest.mock.MagicMock(return_value="Add Foo"),
     )
-    def test_regular_commit_message_yields_default_target_tasks_method(self):
+    def test_regular_commit_message_yields_default_target_tasks_method(
+        self, mock_files_changed
+    ):
         """
         Ensures `target_tasks_method` is `default` when the commit message does not contain
         `DONTBUILD`.
         """
+        mock_files_changed.return_value = ["foo.txt"]
         self.options["tasks_for"] = "github-push"
         params = decision.get_decision_parameters(FAKE_GRAPH_CONFIG, self.options)
         self.assertEqual(params["target_tasks_method"], "default")
 
         self.options["tasks_for"] = "hg-push"
         params = decision.get_decision_parameters(FAKE_GRAPH_CONFIG, self.options)
         self.assertEqual(params["target_tasks_method"], "default")
@@ -121,18 +132,21 @@
         unittest.mock.MagicMock(return_value="DONTBUILD"),
     )
     @unittest.mock.patch.object(
         HgRepository,
         "get_commit_message",
         unittest.mock.MagicMock(return_value="DONTBUILD"),
     )
-    def test_dontbuild_commit_message_yields_default_target_tasks_method(self):
+    def test_dontbuild_commit_message_yields_default_target_tasks_method(
+        self, mock_files_changed
+    ):
         """
         Ensures `target_tasks_method` is `nothing` when the commit message contains `DONTBUILD`.
         """
+        mock_files_changed.return_value = ["foo.txt"]
         self.options["tasks_for"] = "github-release"
         params = decision.get_decision_parameters(FAKE_GRAPH_CONFIG, self.options)
         self.assertNotEqual(params["target_tasks_method"], "nothing")
 
         self.options["tasks_for"] = "github-push"
         params = decision.get_decision_parameters(FAKE_GRAPH_CONFIG, self.options)
         self.assertEqual(params["target_tasks_method"], "nothing")
```

### Comparing `taskcluster-taskgraph-8.0.0/test/test_generator.py` & `taskcluster-taskgraph-8.0.1/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_graph.py` & `taskcluster-taskgraph-8.0.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_main.py` & `taskcluster-taskgraph-8.0.1/test/test_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 },
                 "b": {
                     "attributes": {"kind": "task", "thing": True},
                     "dependencies": {},
                     "description": "",
                     "kind": "task",
                     "label": "b",
-                    "optimization": None,
+                    "optimization": {"skip-unless-changed": True},
                     "soft_dependencies": [],
                     "if_dependencies": [],
                     "task": {
                         "foo": {"baz": 1},
                     },
                 },
             },
@@ -160,28 +160,29 @@
             {
                 "b": {
                     "attributes": {"kind": "task", "thing": True},
                     "dependencies": {},
                     "description": "",
                     "kind": "task",
                     "label": "b",
-                    "optimization": None,
+                    "optimization": {"skip-unless-changed": True},
                     "soft_dependencies": [],
                     "if_dependencies": [],
                     "task": {
                         "foo": {"baz": 1},
                     },
                 },
             },
             id="regex-b-only",
         ),
         pytest.param(
             None,
             [
                 "attributes.thing",
+                "optimization.skip-unless-changed",
                 "task.foo.baz",
             ],
             {
                 "a": {
                     "attributes": {"kind": "task"},
                     "dependencies": {"dep": "b"},
                     "description": "",
@@ -196,15 +197,15 @@
                 },
                 "b": {
                     "attributes": {"kind": "task"},
                     "dependencies": {},
                     "description": "",
                     "kind": "task",
                     "label": "b",
-                    "optimization": None,
+                    "optimization": {},
                     "soft_dependencies": [],
                     "if_dependencies": [],
                     "task": {
                         "foo": {},
                     },
                 },
             },
@@ -212,15 +213,19 @@
         ),
     ),
 )
 def test_get_filtered_taskgraph(regex, exclude, expected):
     tasks = {
         "a": Task(kind="task", label="a", attributes={}, task={"foo": {"bar": 1}}),
         "b": Task(
-            kind="task", label="b", attributes={"thing": True}, task={"foo": {"baz": 1}}
+            kind="task",
+            label="b",
+            attributes={"thing": True},
+            optimization={"skip-unless-changed": True},
+            task={"foo": {"baz": 1}},
         ),
     }
 
     graph = TaskGraph(tasks, Graph(set(tasks), {("a", "b", "dep")}))
     filtered = get_filtered_taskgraph(graph, regex, exclude)
     assert filtered.to_json() == expected
```

### Comparing `taskcluster-taskgraph-8.0.0/test/test_morph.py` & `taskcluster-taskgraph-8.0.1/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_optimize.py` & `taskcluster-taskgraph-8.0.1/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_optimize_strategies.py` & `taskcluster-taskgraph-8.0.1/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_parameters.py` & `taskcluster-taskgraph-8.0.1/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-8.0.1/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_scripts_run_task.py` & `taskcluster-taskgraph-8.0.1/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_target_tasks.py` & `taskcluster-taskgraph-8.0.1/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_taskgraph.py` & `taskcluster-taskgraph-8.0.1/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transform_chunking.py` & `taskcluster-taskgraph-8.0.1/test/test_transform_chunking.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transform_docker_image.py` & `taskcluster-taskgraph-8.0.1/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transform_task_context.py` & `taskcluster-taskgraph-8.0.1/test/test_transform_task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_base.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_cached_tasks.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_fetch.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_notify.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_run.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_run.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_run_run_task.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_run_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_run_toolchain.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_run_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_transforms_task.py` & `taskcluster-taskgraph-8.0.1/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_archive.py` & `taskcluster-taskgraph-8.0.1/test/test_util_archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_attributes.py` & `taskcluster-taskgraph-8.0.1/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_cached_tasks.py` & `taskcluster-taskgraph-8.0.1/test/test_util_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_dependencies.py` & `taskcluster-taskgraph-8.0.1/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_docker.py` & `taskcluster-taskgraph-8.0.1/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_parameterization.py` & `taskcluster-taskgraph-8.0.1/test/test_util_parameterization.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
 @pytest.fixture
 def assert_artifact_refs(monkeypatch):
     monkeypatch.setenv("TASKCLUSTER_ROOT_URL", _test_root_url())
 
     def inner(input, output):
         # Clear memoized function
-        get_root_url.clear()
+        get_root_url.cache_clear()
         taskid_for_edge_name = {"edge%d" % n: "tid%d" % n for n in range(1, 4)}
         assert (
             resolve_task_references(
                 "subject", input, "tid-self", "tid-decision", taskid_for_edge_name
             )
             == output
         )
```

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_path.py` & `taskcluster-taskgraph-8.0.1/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_python_path.py` & `taskcluster-taskgraph-8.0.1/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_readonlydict.py` & `taskcluster-taskgraph-8.0.1/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_schema.py` & `taskcluster-taskgraph-8.0.1/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_taskcluster.py` & `taskcluster-taskgraph-8.0.1/test/test_util_taskcluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,53 +24,53 @@
 @pytest.fixture(autouse=True)
 def mock_production_taskcluster_root_url(monkeypatch):
     monkeypatch.setattr(tc, "PRODUCTION_TASKCLUSTER_ROOT_URL", "https://tc.example.com")
 
 
 @pytest.fixture
 def root_url(mock_environ):
-    tc.get_root_url.clear()
+    tc.get_root_url.cache_clear()
     return tc.get_root_url(False)
 
 
 @pytest.fixture
 def proxy_root_url(monkeypatch, mock_environ):
     monkeypatch.setenv("TASK_ID", "123")
     monkeypatch.setenv("TASKCLUSTER_PROXY_URL", "https://taskcluster-proxy.net")
-    tc.get_root_url.clear()
+    tc.get_root_url.cache_clear()
     return tc.get_root_url(True)
 
 
 def test_get_root_url(monkeypatch):
-    tc.get_root_url.clear()
+    tc.get_root_url.cache_clear()
     assert tc.get_root_url(False) == tc.PRODUCTION_TASKCLUSTER_ROOT_URL
 
     custom_url = "https://taskcluster-root.net"
     monkeypatch.setenv("TASKCLUSTER_ROOT_URL", custom_url)
-    tc.get_root_url.clear()
+    tc.get_root_url.cache_clear()
     assert tc.get_root_url(False) == custom_url
 
     # trailing slash is normalized
     monkeypatch.setenv("TASKCLUSTER_ROOT_URL", custom_url + "/")
-    tc.get_root_url.clear()
+    tc.get_root_url.cache_clear()
     assert tc.get_root_url(False) == custom_url
 
     with pytest.raises(RuntimeError):
         tc.get_root_url(True)
 
     task_id = "123"
     monkeypatch.setenv("TASK_ID", task_id)
 
     with pytest.raises(RuntimeError):
         tc.get_root_url(True)
 
     proxy_url = "https://taskcluster-proxy.net"
     monkeypatch.setenv("TASKCLUSTER_PROXY_URL", proxy_url)
     assert tc.get_root_url(True) == proxy_url
-    tc.get_root_url.clear()
+    tc.get_root_url.cache_clear()
 
     # no default set
     monkeypatch.setattr(tc, "PRODUCTION_TASKCLUSTER_ROOT_URL", None)
     monkeypatch.delenv("TASKCLUSTER_ROOT_URL")
     with pytest.raises(RuntimeError):
         tc.get_root_url(False)
 
@@ -378,16 +378,16 @@
             ],
         },
     )
     assert list(tc.list_task_group_incomplete_tasks(tgid)) == ["1", "2", "3"]
 
 
 def test_get_ancestors(responses, root_url):
-    tc.get_task_definition.clear()
-    tc._get_deps.clear()
+    tc.get_task_definition.cache_clear()
+    tc._get_deps.cache_clear()
     base_url = f"{root_url}/api/queue/v1/task"
     responses.add(
         responses.GET,
         f"{base_url}/fff",
         json={
             "dependencies": ["eee", "ddd"],
             "metadata": {
@@ -453,16 +453,16 @@
         "task-ddd": "ddd",
         "task-eee": "eee",
     }
     assert got == expected, f"got: {got}, expected: {expected}"
 
 
 def test_get_ancestors_string(responses, root_url):
-    tc.get_task_definition.clear()
-    tc._get_deps.clear()
+    tc.get_task_definition.cache_clear()
+    tc._get_deps.cache_clear()
     base_url = f"{root_url}/api/queue/v1/task"
     responses.add(
         responses.GET,
         f"{base_url}/fff",
         json={
             "dependencies": ["eee", "ddd"],
             "metadata": {
```

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_templates.py` & `taskcluster-taskgraph-8.0.1/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_time.py` & `taskcluster-taskgraph-8.0.1/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_treeherder.py` & `taskcluster-taskgraph-8.0.1/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_vcs.py` & `taskcluster-taskgraph-8.0.1/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_verify.py` & `taskcluster-taskgraph-8.0.1/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_workertypes.py` & `taskcluster-taskgraph-8.0.1/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.0/test/test_util_yaml.py` & `taskcluster-taskgraph-8.0.1/test/test_util_yaml.py`

 * *Files identical despite different names*

