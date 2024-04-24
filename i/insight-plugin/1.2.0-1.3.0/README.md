# Comparing `tmp/insight_plugin-1.2.0.tar.gz` & `tmp/insight_plugin-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insight_plugin-1.2.0.tar", last modified: Wed Apr 10 10:32:33 2024, max compression
+gzip compressed data, was "insight_plugin-1.3.0.tar", last modified: Wed Apr 24 10:37:10 2024, max compression
```

## Comparing `insight_plugin-1.2.0.tar` & `insight_plugin-1.3.0.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.977923 insight_plugin-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-10 10:32:33.977923 insight_plugin-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18895 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/features/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/analysis/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin/features/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/checksum_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/command_line_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/common_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/docker_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/dockerspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/plugin_spec_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    23952 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/schema_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/temp_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/common/template_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/create/help/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/connection_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/help_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/help/input_output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/json_generation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/plugin_to_helpmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/create/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/export/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/export/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/export/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/export/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/interactive/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/interactive/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/interactive/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/interactive/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/linter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/linter/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.961923 insight_plugin-1.2.0/insight_plugin/features/refresh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/refresh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/refresh/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/run/bash_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/run/run_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/run/server_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/samples/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/samples/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/validate/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/version/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/version/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/helpmd_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/input_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/version/util/yaml_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/features/view/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/features/view/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/.dockerignore.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/Makefile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/templates/assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/assessment/assessment.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/templates/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/bin/plugin.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.965923 insight_plugin-1.2.0/insight_plugin/templates/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/action.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/connection.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/schema.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/__init__.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/plugin/util/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/plugin/util/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/requirements.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/setup.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.969923 insight_plugin-1.2.0/insight_plugin/templates/unit_test/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/unit_test/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/insight_plugin/templates/unit_test/test_action.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.957923 insight_plugin-1.2.0/insight_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 10:32:33.000000 insight_plugin-1.2.0/insight_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:32:33.977923 insight_plugin-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1430 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/
--rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/connection/
--rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/connection/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/connection/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/triggers/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/triggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:33.973923 insight_plugin-1.2.0/tests/resources/export_test_base64/unit_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/unit_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/resources/export_test_base64/unit_test/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_gen_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_help_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_json_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_semver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_spec_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_temp_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-10 10:32:16.000000 insight_plugin-1.2.0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.574485 insight_plugin-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.550485 insight_plugin-1.3.0/insight_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18895 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin/features/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/analysis/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin/features/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/checksum_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/command_line_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/common_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/docker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/dockerspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/plugin_spec_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24186 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/schema_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/temp_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/common/template_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/create/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/connection_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/help_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/help/input_output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/json_generation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/plugin_to_helpmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/create/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/export/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/export/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/export/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/export/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/interactive/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/interactive/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/interactive/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/interactive/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/linter/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/refresh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/refresh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/refresh/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-24 10:36:48.000000 insight_plugin-1.3.0/insight_plugin/features/run/bash_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/run/run_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/run/server_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.558485 insight_plugin-1.3.0/insight_plugin/features/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/samples/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/samples/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/validate/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/version/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/helpmd_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/input_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/version/util/yaml_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/features/view/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/features/view/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/.dockerignore.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/Makefile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/assessment/assessment.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/bin/plugin.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.562485 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/action.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/connection.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/schema.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/__init__.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/plugin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/plugin/util/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/requirements.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/setup.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.566485 insight_plugin-1.3.0/insight_plugin/templates/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/unit_test/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/insight_plugin/templates/unit_test/test_action.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.554485 insight_plugin-1.3.0/insight_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 10:37:10.000000 insight_plugin-1.3.0/insight_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:37:10.574485 insight_plugin-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1430 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       67 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/connection/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/connection/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/triggers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/triggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      469 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:37:10.570485 insight_plugin-1.3.0/tests/resources/export_test_base64/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/unit_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/resources/export_test_base64/unit_test/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_gen_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_help_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_json_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_semver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_spec_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_temp_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-24 10:36:49.000000 insight_plugin-1.3.0/tests/util.py
```

### Comparing `insight_plugin-1.2.0/LICENSE` & `insight_plugin-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/PKG-INFO` & `insight_plugin-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight_plugin
-Version: 1.2.0
+Version: 1.3.0
 Summary: Plugin tooling for the Rapid7 Insight platform
 Home-page: https://github.com/rapid7/insight-plugin
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `insight_plugin-1.2.0/README.md` & `insight_plugin-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/__main__.py` & `insight_plugin-1.3.0/insight_plugin/__main__.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/constants.py` & `insight_plugin-1.3.0/insight_plugin/constants.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/analysis/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/analysis/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/builder.py` & `insight_plugin-1.3.0/insight_plugin/features/common/builder.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/checksum_util.py` & `insight_plugin-1.3.0/insight_plugin/features/common/checksum_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/command_line_util.py` & `insight_plugin-1.3.0/insight_plugin/features/common/command_line_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/common_feature.py` & `insight_plugin-1.3.0/insight_plugin/features/common/common_feature.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/docker_util.py` & `insight_plugin-1.3.0/insight_plugin/features/common/docker_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/dockerspec.py` & `insight_plugin-1.3.0/insight_plugin/features/common/dockerspec.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/exceptions.py` & `insight_plugin-1.3.0/insight_plugin/features/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/logging_util.py` & `insight_plugin-1.3.0/insight_plugin/features/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/plugin_spec_util.py` & `insight_plugin-1.3.0/insight_plugin/features/common/plugin_spec_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     # TODO: Have a discussion on if this should be its own file with the team
     ACTIONS: Final = "actions"
     CONNECTIONS: Final = "connection"
     DEFAULT: Final = "default"
     DESCRIPTION: Final = "description"
     ENUM: Final = "enum"
     EXAMPLE: Final = "example"
+    PLACEHOLDER: Final = "placeholder"
+    TOOLTIP: Final = "tooltip"
     FILENAME: Final = "plugin.spec.yaml"
     FILEPATH: Final = "filepath"
     HELP: Final = "help"
     ITEMS: Final = "items"
     INPUT: Final = "input"
     KEY_FEATURES: Final = "key_features"
     LINKS: Final = "links"
```

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/schema_util.py` & `insight_plugin-1.3.0/insight_plugin/features/common/schema_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -436,14 +436,18 @@
             SchemaUtil.try_add(PluginSpecConstants.TITLE, items, parent_object[key])
             # Set the current parameter description if one exists.
             SchemaUtil.try_add(
                 PluginSpecConstants.DESCRIPTION, items, parent_object[key]
             )
             # Set the current parameter default if one exists.
             SchemaUtil.try_add(PluginSpecConstants.DEFAULT, items, parent_object[key])
+            # Set placeholder
+            SchemaUtil.try_add(PluginSpecConstants.PLACEHOLDER, items, parent_object[key])
+            # Set tooltip
+            SchemaUtil.try_add(PluginSpecConstants.TOOLTIP, items, parent_object[key])
             # If the current parameter is an array (it has items contents), set the items object dict.
             if array_items[SchemaConstants.ITEMS]:
                 SchemaUtil.try_add(
                     SchemaConstants.ITEMS, array_items, parent_object[key]
                 )
             # Set the current parameter enums if a list of strings exists.
             SchemaUtil.try_add(PluginSpecConstants.ENUM, items, parent_object[key])
```

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/temp_file_util.py` & `insight_plugin-1.3.0/insight_plugin/features/common/temp_file_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/common/template_util.py` & `insight_plugin-1.3.0/insight_plugin/features/common/template_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/create/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/help/components.py` & `insight_plugin-1.3.0/insight_plugin/features/create/help/components.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/help/connection_help.py` & `insight_plugin-1.3.0/insight_plugin/features/create/help/connection_help.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/help/constants.py` & `insight_plugin-1.3.0/insight_plugin/features/create/help/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
         "Name",
         "Type",
         "Default",
         "Required",
         "Description",
         "Enum",
         "Example",
+        "Placeholder",
+        "Tooltip"
     ]
     OUTPUT_HEADERS = [
         "Name",
         "Type",
         "Required",
         "Description",
         "Example",
```

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/help/help_util.py` & `insight_plugin-1.3.0/insight_plugin/features/create/help/help_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
                     key,
                     item.get(PluginSpecConstants.TYPE, "None"),
                     item.get(PluginSpecConstants.DEFAULT, "None"),
                     item.get(PluginSpecConstants.REQUIRED, "None"),
                     item.get(PluginSpecConstants.DESCRIPTION, "None"),
                     item.get(PluginSpecConstants.ENUM, "None"),
                     item.get(PluginSpecConstants.EXAMPLE, "None"),
+                    item.get(PluginSpecConstants.PLACEHOLDER, "None"),
+                    item.get(PluginSpecConstants.TOOLTIP, "None")
                 ]
             elif table_type == TableHeaders.OUTPUT_HEADERS:
                 next_row = [
                     key,
                     item.get(PluginSpecConstants.TYPE, "None"),
                     item.get(PluginSpecConstants.REQUIRED, "None"),
                     item.get(PluginSpecConstants.DESCRIPTION, "None"),
```

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/help/input_output_helpers.py` & `insight_plugin-1.3.0/insight_plugin/features/create/help/input_output_helpers.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/json_generation_util.py` & `insight_plugin-1.3.0/insight_plugin/features/create/json_generation_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/plugin_to_helpmd.py` & `insight_plugin-1.3.0/insight_plugin/features/create/plugin_to_helpmd.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/create/util.py` & `insight_plugin-1.3.0/insight_plugin/features/create/util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/export/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/export/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/interactive/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/interactive/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/interactive/util/util.py` & `insight_plugin-1.3.0/insight_plugin/features/interactive/util/util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/linter/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/linter/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/refresh/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/refresh/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/run/bash_controller.py` & `insight_plugin-1.3.0/insight_plugin/features/run/bash_controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/run/run_controller.py` & `insight_plugin-1.3.0/insight_plugin/features/run/run_controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/run/server_controller.py` & `insight_plugin-1.3.0/insight_plugin/features/run/server_controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/samples/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/samples/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/samples/util/constants.py` & `insight_plugin-1.3.0/insight_plugin/features/samples/util/constants.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/samples/util/util.py` & `insight_plugin-1.3.0/insight_plugin/features/samples/util/util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/validate/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/validate/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/version/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/version/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/version/util/helpmd_util.py` & `insight_plugin-1.3.0/insight_plugin/features/version/util/helpmd_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/version/util/input_util.py` & `insight_plugin-1.3.0/insight_plugin/features/version/util/input_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/version/util/version_util.py` & `insight_plugin-1.3.0/insight_plugin/features/version/util/version_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/version/util/yaml_util.py` & `insight_plugin-1.3.0/insight_plugin/features/version/util/yaml_util.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/features/view/controller.py` & `insight_plugin-1.3.0/insight_plugin/features/view/controller.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/Dockerfile.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/Makefile.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/Makefile.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/assessment/assessment.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/assessment/assessment.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/bin/plugin.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/bin/plugin.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/action.py.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/action.py.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -16,10 +16,11 @@
         # START INPUT BINDING - DO NOT REMOVE - ANY INPUTS BELOW WILL UPDATE WITH YOUR PLUGIN SPEC AFTER REGENERATION
         {% for parameter in inputs.keys()|sort -%}
         {{ parameter.lower().replace("-", "_") }} = params.get(Input.{{ parameter.upper().replace("-", "") }})
         {% endfor -%}
         # END INPUT BINDING - DO NOT REMOVE
 
         return {
-            {% for parameter in outputs.keys()|sort -%}Output.{{ parameter.upper().replace("-", "") }}: None,
-            {% endfor %}
+        {%- for parameter in outputs.keys()|sort %}
+            Output.{{ parameter.upper().replace("-", "") }}: None,
+        {%- endfor %}
         }
```

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/plugin/actions/action/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/plugin/connection/connection.py.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/plugin/connection/connection.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/plugin/tasks/task/task.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/schema.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/plugin/triggers/trigger/trigger.py.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -19,11 +19,12 @@
         {{ parameter.lower().replace("-", "_") }} = params.get(Input.{{ parameter.upper().replace("-", "") }})
         {% endfor -%}
         # END INPUT BINDING - DO NOT REMOVE
 
         while True:
             # TODO: Implement trigger functionality
             self.send({
-                {% for parameter in outputs.keys()|sort -%}Output.{{ parameter.upper().replace("-", "") }}: None,
-                {% endfor %}
+            {%- for parameter in outputs.keys()|sort %}
+                Output.{{ parameter.upper().replace("-", "") }}: None,
+            {%- endfor %}
             })
             time.sleep(5)
```

### Comparing `insight_plugin-1.2.0/insight_plugin/templates/unit_test/test_action.py.jinja` & `insight_plugin-1.3.0/insight_plugin/templates/unit_test/test_action.py.jinja`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/insight_plugin.egg-info/PKG-INFO` & `insight_plugin-1.3.0/insight_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight-plugin
-Version: 1.2.0
+Version: 1.3.0
 Summary: Plugin tooling for the Rapid7 Insight platform
 Home-page: https://github.com/rapid7/insight-plugin
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `insight_plugin-1.2.0/insight_plugin.egg-info/SOURCES.txt` & `insight_plugin-1.3.0/insight_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/pyproject.toml` & `insight_plugin-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/setup.py` & `insight_plugin-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py` & `insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/action.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py` & `insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/decode/schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py` & `insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/action.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py` & `insight_plugin-1.3.0/tests/resources/export_test_base64/komand_base64/actions/encode/schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_checksum.py` & `insight_plugin-1.3.0/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_create.py` & `insight_plugin-1.3.0/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_export.py` & `insight_plugin-1.3.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_gen_samples.py` & `insight_plugin-1.3.0/tests/test_gen_samples.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_help_creation.py` & `insight_plugin-1.3.0/tests/test_help_creation.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_interactive.py` & `insight_plugin-1.3.0/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_json_generate.py` & `insight_plugin-1.3.0/tests/test_json_generate.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_refresh.py` & `insight_plugin-1.3.0/tests/test_refresh.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_run.py` & `insight_plugin-1.3.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_schema.py` & `insight_plugin-1.3.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_semver.py` & `insight_plugin-1.3.0/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/test_spec_order.py` & `insight_plugin-1.3.0/tests/test_spec_order.py`

 * *Files identical despite different names*

### Comparing `insight_plugin-1.2.0/tests/util.py` & `insight_plugin-1.3.0/tests/util.py`

 * *Files identical despite different names*

