# Comparing `tmp/fixinventorylib-4.0.2.tar.gz` & `tmp/fixinventorylib-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventorylib-4.0.2.tar", last modified: Fri Apr 12 12:16:05 2024, max compression
+gzip compressed data, was "fixinventorylib-4.0.3.tar", last modified: Wed Apr 24 10:33:58 2024, max compression
```

## Comparing `fixinventorylib-4.0.2.tar` & `fixinventorylib-4.0.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.116392 fixinventorylib-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 12:16:05.116392 fixinventorylib-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.112392 fixinventorylib-4.0.2/fixinventorylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 12:16:05.000000 fixinventorylib-4.0.2/fixinventorylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 12:16:05.000000 fixinventorylib-4.0.2/fixinventorylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:16:05.000000 fixinventorylib-4.0.2/fixinventorylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:12:41.000000 fixinventorylib-4.0.2/fixinventorylib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-12 12:16:05.000000 fixinventorylib-4.0.2/fixinventorylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 12:16:05.000000 fixinventorylib-4.0.2/fixinventorylib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.104392 fixinventorylib-4.0.2/fixlib/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.108392 fixinventorylib-4.0.2/fixlib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.108392 fixinventorylib-4.0.2/fixlib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    49945 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.108392 fixinventorylib-4.0.2/fixlib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/durations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.108392 fixinventorylib-4.0.2/fixlib/graph/
--rw-r--r--   0 runner    (1001) docker     (127)    28662 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17747 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.108392 fixinventorylib-4.0.2/fixlib/log/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)    33802 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.108392 fixinventorylib-4.0.2/fixlib/web/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.112392 fixinventorylib-4.0.2/fixlib/web/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)    39028 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/fixlib/x509.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 12:16:05.116392 fixinventorylib-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:05.112392 fixinventorylib-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-12 12:11:48.000000 fixinventorylib-4.0.2/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.530955 fixinventorylib-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-24 10:33:58.530955 fixinventorylib-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.530955 fixinventorylib-4.0.3/fixinventorylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-24 10:33:58.000000 fixinventorylib-4.0.3/fixinventorylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 10:33:58.000000 fixinventorylib-4.0.3/fixinventorylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:33:58.000000 fixinventorylib-4.0.3/fixinventorylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:24.000000 fixinventorylib-4.0.3/fixinventorylib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 10:33:58.000000 fixinventorylib-4.0.3/fixinventorylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 10:33:58.000000 fixinventorylib-4.0.3/fixinventorylib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.522955 fixinventorylib-4.0.3/fixlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.522955 fixinventorylib-4.0.3/fixlib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.522955 fixinventorylib-4.0.3/fixlib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50057 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.526955 fixinventorylib-4.0.3/fixlib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.526955 fixinventorylib-4.0.3/fixlib/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    28662 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17747 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.526955 fixinventorylib-4.0.3/fixlib/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33802 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.526955 fixinventorylib-4.0.3/fixlib/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.526955 fixinventorylib-4.0.3/fixlib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39028 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/fixlib/x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 10:33:58.530955 fixinventorylib-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:58.530955 fixinventorylib-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-24 10:29:20.000000 fixinventorylib-4.0.3/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 10:29:21.000000 fixinventorylib-4.0.3/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 10:29:21.000000 fixinventorylib-4.0.3/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-24 10:29:21.000000 fixinventorylib-4.0.3/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-04-24 10:29:21.000000 fixinventorylib-4.0.3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-24 10:29:21.000000 fixinventorylib-4.0.3/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-24 10:29:21.000000 fixinventorylib-4.0.3/test/test_x509.py
```

### Comparing `fixinventorylib-4.0.2/PKG-INFO` & `fixinventorylib-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorylib
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix Inventory common library.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fixinventory/tree/main/fixlib
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fixinventorylib-4.0.2/README.md` & `fixinventorylib-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixinventorylib.egg-info/PKG-INFO` & `fixinventorylib-4.0.3/fixinventorylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorylib
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix Inventory common library.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fixinventory/tree/main/fixlib
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fixinventorylib-4.0.2/fixinventorylib.egg-info/SOURCES.txt` & `fixinventorylib-4.0.3/fixinventorylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/args.py` & `fixinventorylib-4.0.3/fixlib/args.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/asynchronous/utils.py` & `fixinventorylib-4.0.3/fixlib/asynchronous/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/asynchronous/web/runner.py` & `fixinventorylib-4.0.3/fixlib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/asynchronous/web/ws_handler.py` & `fixinventorylib-4.0.3/fixlib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/baseplugin.py` & `fixinventorylib-4.0.3/fixlib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/baseresources.py` & `fixinventorylib-4.0.3/fixlib/baseresources.py`

 * *Files 1% similar despite different names*

```diff
@@ -787,14 +787,18 @@
 @define(eq=False, slots=False)
 class BaseRegion(BaseResource):
     kind: ClassVar[str] = "region"
     kind_display: ClassVar[str] = "Region"
     kind_description: ClassVar[str] = "A region."
     metadata: ClassVar[Dict[str, Any]] = {"icon": "region", "group": "control"}
 
+    long_name: Optional[str] = None
+    latitude: Optional[float] = None
+    longitude: Optional[float] = None
+
     def _keys(self) -> Tuple[Any, ...]:
         if self._graph is None:
             raise RuntimeError(f"_keys() called on {self.rtdname} before resource was added to graph")
         return self.kind, self.cloud().id, self.account().id, self.region().id, self.zone().id, self.id, self.name
 
     def region(self, graph: Optional[Any] = None) -> BaseRegion:
         return self
```

### Comparing `fixinventorylib-4.0.2/fixlib/config.py` & `fixinventorylib-4.0.3/fixlib/config.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/__init__.py` & `fixinventorylib-4.0.3/fixlib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/actions.py` & `fixinventorylib-4.0.3/fixlib/core/actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import threading
 import time
 from contextlib import suppress, AbstractContextManager
+from itertools import islice
 from logging import Logger
 from queue import Queue
 
 from websocket import WebSocketApp, WebSocket  # type: ignore
 import requests
 import json
 from concurrent.futures import ThreadPoolExecutor
@@ -14,15 +15,15 @@
 
 from fixlib.core.progress import Progress, ProgressDone
 from fixlib.logger import log
 from fixlib.event import EventType, remove_event_listener, add_event_listener, Event
 from fixlib.args import ArgumentParser
 from fixlib.jwt import encode_jwt_to_headers
 from fixlib.core.ca import TLSData
-from typing import Callable, Dict, Optional, List, Any
+from typing import Callable, Dict, Optional, List, Any, Set
 
 from fixlib.types import Json
 from fixlib.utils import utc_str
 
 
 @define(frozen=True)
 class CoreFeedback:
@@ -80,14 +81,69 @@
     def with_context(self, *context: str) -> "CoreFeedback":
         return evolve(self, context=list(context))
 
     def child_context(self, *context: str) -> "CoreFeedback":
         return self.with_context(*(self.context + list(context)))
 
 
+@define
+class ErrorSummary:
+    error: str
+    message: str
+    info: bool
+    region: Optional[str] = None
+    service_actions: Dict[str, Set[str]] = field(factory=dict)
+
+
+class ErrorAccumulator:
+    def __init__(self) -> None:
+        self.regional_errors: Dict[Optional[str], Dict[str, ErrorSummary]] = {}
+
+    def add_error(
+        self, as_info: bool, error_kind: str, service: str, action: str, message: str, region: Optional[str] = None
+    ) -> None:
+        if region not in self.regional_errors:
+            self.regional_errors[region] = {}
+        regional_errors = self.regional_errors[region]
+
+        key = f"{error_kind}:{message}:{as_info}"
+        if key not in regional_errors:
+            regional_errors[key] = ErrorSummary(error_kind, message, as_info, region, {service: {action}})
+        else:
+            summary = regional_errors[key]
+            if service not in summary.service_actions:
+                summary.service_actions[service] = {action}
+            else:
+                summary.service_actions[service].add(action)
+
+    def report_region(self, core_feedback: CoreFeedback, region: Optional[str]) -> None:
+        if regional_errors := self.regional_errors.get(region):
+            # reset errors for this region
+            self.regional_errors[region] = {}
+            # add region as context
+            feedback = core_feedback.child_context(region) if region else core_feedback
+            # send to core
+            for err in regional_errors.values():
+                srv_acts = []
+                for service, actions in islice(err.service_actions.items(), 10):
+                    suffix = " and more" if len(actions) > 3 else ""
+                    srv_acts.append(service + ": " + ", ".join(islice(actions, 3)) + suffix)
+                message = f"[{err.error}] {err.message} Services and actions affected: {', '.join(srv_acts)}"
+                if len(err.service_actions) > 10:
+                    message += " and more..."
+                if err.info:
+                    feedback.info(message)
+                else:
+                    feedback.error(message)
+
+    def report_all(self, core_feedback: CoreFeedback) -> None:
+        for region in self.regional_errors.keys():
+            self.report_region(core_feedback, region)
+
+
 class SuppressWithFeedback(AbstractContextManager[None]):
     def __init__(self, message: str, feedback: CoreFeedback, logger: Optional[Logger] = None) -> None:
         self.message = message
         self.feedback = feedback
         self.logger = logger
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Optional[bool]:
```

### Comparing `fixinventorylib-4.0.2/fixlib/core/ca.py` & `fixinventorylib-4.0.3/fixlib/core/ca.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/config.py` & `fixinventorylib-4.0.3/fixlib/core/config.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/custom_command.py` & `fixinventorylib-4.0.3/fixlib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/events.py` & `fixinventorylib-4.0.3/fixlib/core/events.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/model_check.py` & `fixinventorylib-4.0.3/fixlib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/model_export.py` & `fixinventorylib-4.0.3/fixlib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/progress.py` & `fixinventorylib-4.0.3/fixlib/core/progress.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/search.py` & `fixinventorylib-4.0.3/fixlib/core/search.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/core/tasks.py` & `fixinventorylib-4.0.3/fixlib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/durations.py` & `fixinventorylib-4.0.3/fixlib/durations.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/event.py` & `fixinventorylib-4.0.3/fixlib/event.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/graph/__init__.py` & `fixinventorylib-4.0.3/fixlib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/graph/graph_extensions.py` & `fixinventorylib-4.0.3/fixlib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/json.py` & `fixinventorylib-4.0.3/fixlib/json.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/json_bender.py` & `fixinventorylib-4.0.3/fixlib/json_bender.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/jwt.py` & `fixinventorylib-4.0.3/fixlib/jwt.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/lock.py` & `fixinventorylib-4.0.3/fixlib/lock.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/logger.py` & `fixinventorylib-4.0.3/fixlib/logger.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/parse_util.py` & `fixinventorylib-4.0.3/fixlib/parse_util.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/proc.py` & `fixinventorylib-4.0.3/fixlib/proc.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/threading.py` & `fixinventorylib-4.0.3/fixlib/threading.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/tree.py` & `fixinventorylib-4.0.3/fixlib/tree.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/utils.py` & `fixinventorylib-4.0.3/fixlib/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/__init__.py` & `fixinventorylib-4.0.3/fixlib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/metrics.py` & `fixinventorylib-4.0.3/fixlib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/static/android-chrome-192x192.png` & `fixinventorylib-4.0.3/fixlib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/static/android-chrome-512x512.png` & `fixinventorylib-4.0.3/fixlib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/static/apple-touch-icon.png` & `fixinventorylib-4.0.3/fixlib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/static/favicon-16x16.png` & `fixinventorylib-4.0.3/fixlib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/static/favicon-32x32.png` & `fixinventorylib-4.0.3/fixlib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/static/index.html` & `fixinventorylib-4.0.3/fixlib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/static/mstile-150x150.png` & `fixinventorylib-4.0.3/fixlib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/web/static/picnic.min.css` & `fixinventorylib-4.0.3/fixlib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/fixlib/x509.py` & `fixinventorylib-4.0.3/fixlib/x509.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/pyproject.toml` & `fixinventorylib-4.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventorylib"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{ name = "Some Engineering Inc." }]
 description = "Fix Inventory common library."
 license = { text = "AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
```

### Comparing `fixinventorylib-4.0.2/test/test_args.py` & `fixinventorylib-4.0.3/test/test_args.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_baseresources.py` & `fixinventorylib-4.0.3/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_config.py` & `fixinventorylib-4.0.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_graph.py` & `fixinventorylib-4.0.3/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_graph_extensions.py` & `fixinventorylib-4.0.3/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_json.py` & `fixinventorylib-4.0.3/test/test_json.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_jwt.py` & `fixinventorylib-4.0.3/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_plugin.py` & `fixinventorylib-4.0.3/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_tree.py` & `fixinventorylib-4.0.3/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_utils.py` & `fixinventorylib-4.0.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_web.py` & `fixinventorylib-4.0.3/test/test_web.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.2/test/test_x509.py` & `fixinventorylib-4.0.3/test/test_x509.py`

 * *Files identical despite different names*

