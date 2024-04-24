# Comparing `tmp/murfey-0.9.8.tar.gz` & `tmp/murfey-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murfey-0.9.8.tar", last modified: Mon Nov  6 15:38:44 2023, max compression
+gzip compressed data, was "murfey-0.9.9.tar", last modified: Mon Nov 13 10:39:08 2023, max compression
```

## Comparing `murfey-0.9.8.tar` & `murfey-0.9.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.916767 murfey-0.9.8/
--rw-r--r--   0 vsts      (1001) docker     (127)     1481 2023-11-06 15:38:35.000000 murfey-0.9.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      179 2023-11-06 15:38:35.000000 murfey-0.9.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2463 2023-11-06 15:38:44.916767 murfey-0.9.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1698 2023-11-06 15:38:35.000000 murfey-0.9.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      206 2023-11-06 15:38:35.000000 murfey-0.9.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1748 2023-11-06 15:38:44.916767 murfey-0.9.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      190 2023-11-06 15:38:35.000000 murfey-0.9.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.904767 murfey-0.9.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.904767 murfey-0.9.8/src/murfey/
--rw-r--r--   0 vsts      (1001) docker     (127)       97 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       85 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.904767 murfey-0.9.8/src/murfey/bootstrap/
--rw-r--r--   0 vsts      (1001) docker     (127)     4237 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/bootstrap/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.908767 murfey-0.9.8/src/murfey/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      951 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/cli/db_sessions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      919 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/cli/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2621 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/cli/transfer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.908767 murfey-0.9.8/src/murfey/client/
--rw-r--r--   0 vsts      (1001) docker     (127)    10967 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15120 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/analyser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1586 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/context.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.908767 murfey-0.9.8/src/murfey/client/contexts/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4577 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/contexts/fib.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22025 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/contexts/spa.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41087 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/contexts/tomo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1466 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/customlogging.py
--rw-r--r--   0 vsts      (1001) docker     (127)      546 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/gain_ref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3878 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/instance_environment.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13406 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/rsync.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.912767 murfey-0.9.8/src/murfey/client/tui/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      127 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26939 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/app.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5935 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/controller.css
--rw-r--r--   0 vsts      (1001) docker     (127)      179 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/forms.py
--rw-r--r--   0 vsts      (1001) docker     (127)      318 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/launcher.css
--rw-r--r--   0 vsts      (1001) docker     (127)     5280 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/progress.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40329 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/screens.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2188 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/tui/status_bar.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2594 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/update.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9857 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/watchdir.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3746 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/watchdir_multigrid.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5669 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/client/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.912767 murfey-0.9.8/src/murfey/server/
--rw-r--r--   0 vsts      (1001) docker     (127)    85752 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39220 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/api.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8109 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/bootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2403 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31662 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/demo_api.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2670 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/gain.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12726 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/ispyb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1393 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)      930 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/murfey_db.py
--rw-r--r--   0 vsts      (1001) docker     (127)      905 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/prometheus.py
--rw-r--r--   0 vsts      (1001) docker     (127)       85 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5058 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/server/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.912767 murfey-0.9.8/src/murfey/templates/
--rw-r--r--   0 vsts      (1001) docker     (127)      671 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/templates/activevisits.html
--rw-r--r--   0 vsts      (1001) docker     (127)      891 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/templates/base.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1148 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/templates/bootstrap.html
--rw-r--r--   0 vsts      (1001) docker     (127)      242 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/templates/home.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.912767 murfey-0.9.8/src/murfey/templates/images/
--rw-r--r--   0 vsts      (1001) docker     (127)   131288 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/templates/images/diamond.png
--rw-r--r--   0 vsts      (1001) docker     (127)    14468 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/templates/images/icon_268.png
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.912767 murfey-0.9.8/src/murfey/templates/static/
--rw-r--r--   0 vsts      (1001) docker     (127)     1420 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/templates/static/styles.css
--rw-r--r--   0 vsts      (1001) docker     (127)      726 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/templates/visit.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.916767 murfey-0.9.8/src/murfey/util/
--rw-r--r--   0 vsts      (1001) docker     (127)     4205 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/db.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3262 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/dummy_setup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1032 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/eer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1309 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/file_monitor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/mdoc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6114 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/models.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6530 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/rsync.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/spa_params.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3355 2023-11-06 15:38:35.000000 murfey-0.9.8/src/murfey/util/state.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 15:38:44.904767 murfey-0.9.8/src/murfey.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2463 2023-11-06 15:38:44.000000 murfey-0.9.8/src/murfey.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2183 2023-11-06 15:38:44.000000 murfey-0.9.8/src/murfey.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-06 15:38:44.000000 murfey-0.9.8/src/murfey.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      205 2023-11-06 15:38:44.000000 murfey-0.9.8/src/murfey.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-06 15:38:44.000000 murfey-0.9.8/src/murfey.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      302 2023-11-06 15:38:44.000000 murfey-0.9.8/src/murfey.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        7 2023-11-06 15:38:44.000000 murfey-0.9.8/src/murfey.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.071388 murfey-0.9.9/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1481 2023-11-13 10:38:59.000000 murfey-0.9.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      179 2023-11-13 10:38:59.000000 murfey-0.9.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2463 2023-11-13 10:39:08.071388 murfey-0.9.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1698 2023-11-13 10:38:59.000000 murfey-0.9.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      206 2023-11-13 10:38:59.000000 murfey-0.9.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1748 2023-11-13 10:39:08.071388 murfey-0.9.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      190 2023-11-13 10:38:59.000000 murfey-0.9.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.059388 murfey-0.9.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.063388 murfey-0.9.9/src/murfey/
+-rw-r--r--   0 vsts      (1001) docker     (127)       97 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       85 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.063388 murfey-0.9.9/src/murfey/bootstrap/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4237 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/bootstrap/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.063388 murfey-0.9.9/src/murfey/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      951 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/cli/db_sessions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      919 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/cli/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2621 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/cli/transfer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.063388 murfey-0.9.9/src/murfey/client/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10967 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15182 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/analyser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1586 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/context.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.067388 murfey-0.9.9/src/murfey/client/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4577 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/contexts/fib.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22823 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/contexts/spa.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41087 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/contexts/tomo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1466 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/customlogging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      546 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/gain_ref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3878 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/instance_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13457 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/rsync.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.067388 murfey-0.9.9/src/murfey/client/tui/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      127 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27141 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/app.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5935 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/controller.css
+-rw-r--r--   0 vsts      (1001) docker     (127)      179 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      318 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/launcher.css
+-rw-r--r--   0 vsts      (1001) docker     (127)     5280 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40319 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/screens.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2188 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/tui/status_bar.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2594 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/update.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9857 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/watchdir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3746 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/watchdir_multigrid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5669 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/client/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.067388 murfey-0.9.9/src/murfey/server/
+-rw-r--r--   0 vsts      (1001) docker     (127)    85826 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39392 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/api.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8109 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/bootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2403 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31693 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/demo_api.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2670 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/gain.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12726 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/ispyb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1393 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      930 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/murfey_db.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      905 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/prometheus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       85 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5058 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/server/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.071388 murfey-0.9.9/src/murfey/templates/
+-rw-r--r--   0 vsts      (1001) docker     (127)      671 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/templates/activevisits.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      891 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/templates/base.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1148 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/templates/bootstrap.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      242 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/templates/home.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.071388 murfey-0.9.9/src/murfey/templates/images/
+-rw-r--r--   0 vsts      (1001) docker     (127)   131288 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/templates/images/diamond.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    14468 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/templates/images/icon_268.png
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.071388 murfey-0.9.9/src/murfey/templates/static/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1420 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/templates/static/styles.css
+-rw-r--r--   0 vsts      (1001) docker     (127)      726 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/templates/visit.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.071388 murfey-0.9.9/src/murfey/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4205 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13125 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/db.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3262 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/dummy_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1032 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/eer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1309 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/file_monitor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/mdoc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6114 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6530 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/rsync.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/spa_params.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3355 2023-11-13 10:38:59.000000 murfey-0.9.9/src/murfey/util/state.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-13 10:39:08.063388 murfey-0.9.9/src/murfey.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2463 2023-11-13 10:39:08.000000 murfey-0.9.9/src/murfey.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2183 2023-11-13 10:39:08.000000 murfey-0.9.9/src/murfey.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-13 10:39:08.000000 murfey-0.9.9/src/murfey.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      205 2023-11-13 10:39:08.000000 murfey-0.9.9/src/murfey.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-13 10:39:08.000000 murfey-0.9.9/src/murfey.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      302 2023-11-13 10:39:08.000000 murfey-0.9.9/src/murfey.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        7 2023-11-13 10:39:08.000000 murfey-0.9.9/src/murfey.egg-info/top_level.txt
```

### Comparing `murfey-0.9.8/LICENSE` & `murfey-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/PKG-INFO` & `murfey-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.9.8
+Version: 0.9.9
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.9.8/README.md` & `murfey-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/setup.cfg` & `murfey-0.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = murfey
 description = Client-Server architecture hauling Cryo-EM data
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.9.8
+version = 0.9.9
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
```

### Comparing `murfey-0.9.8/src/murfey/bootstrap/__main__.py` & `murfey-0.9.9/src/murfey/bootstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/cli/db_sessions.py` & `murfey-0.9.9/src/murfey/cli/db_sessions.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/cli/dummy.py` & `murfey-0.9.9/src/murfey/cli/dummy.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/cli/transfer.py` & `murfey-0.9.9/src/murfey/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/__init__.py` & `murfey-0.9.9/src/murfey/client/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/analyser.py` & `murfey-0.9.9/src/murfey/client/analyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from typing import Type
 
 from murfey.client.context import Context
 from murfey.client.contexts.spa import SPAContext, SPAModularContext
 from murfey.client.contexts.tomo import TomographyContext
 from murfey.client.instance_environment import MurfeyInstanceEnvironment
-from murfey.client.rsync import RSyncerUpdate
+from murfey.client.rsync import RSyncerUpdate, TransferResult
 from murfey.client.tui.forms import FormDependency
 from murfey.util import Observer, get_machine_config
 from murfey.util.models import ProcessingParametersSPA, ProcessingParametersTomo
 
 logger = logging.getLogger("murfey.client.analyser")
 
 spa_form_dependencies: dict = {
@@ -321,15 +321,15 @@
                 #     )
                 break
         else:
             return data_file.with_suffix(".xml")
         return base_dir / self._environment.visit / mid_dir / file_name
 
     def enqueue(self, rsyncer: RSyncerUpdate):
-        if not self._stopping:
+        if not self._stopping and rsyncer.outcome == TransferResult.SUCCESS:
             absolute_path = (self._basepath / rsyncer.file_path).resolve()
             self.queue.put(absolute_path)
 
     def start(self):
         if self.thread.is_alive():
             raise RuntimeError("Analyser already running")
         if self._stopping:
```

### Comparing `murfey-0.9.8/src/murfey/client/context.py` & `murfey-0.9.9/src/murfey/client/context.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/contexts/fib.py` & `murfey-0.9.9/src/murfey/client/contexts/fib.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/contexts/spa.py` & `murfey-0.9.9/src/murfey/client/contexts/spa.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, OrderedDict
 
 import requests
 import xmltodict
 
+import murfey.util.eer
 from murfey.client.context import Context, ProcessingParameter
 from murfey.client.instance_environment import (
     MovieID,
     MovieTracker,
     MurfeyID,
     MurfeyInstanceEnvironment,
 )
@@ -66,15 +67,15 @@
             default=True,
         ),
         ProcessingParameter(
             "particle_diameter", "Particle Diameter (Angstroms)", default=None
         ),
         ProcessingParameter("use_cryolo", "Use crYOLO Autopicking", default=True),
         ProcessingParameter("symmetry", "Symmetry Group", default="C1"),
-        ProcessingParameter("eer_grouping", "EER Grouping", default=20),
+        ProcessingParameter("eer_fractionation", "EER Fractionation", default=20),
         ProcessingParameter(
             "mask_diameter", "Mask Diameter (2D classification)", default=190
         ),
         ProcessingParameter("boxsize", "Box Size", default=256),
         ProcessingParameter("downscale", "Downscale Extracted Particles", default=True),
         ProcessingParameter(
             "small_boxsize", "Downscaled Extracted Particle Size (pixels)", default=128
@@ -164,19 +165,22 @@
                         ][dose_index]["a:Value"]["#text"]
                     )
                     * (1e-20),
                     2,
                 )  # convert e / m^2 to e / A^2
             except ValueError:
                 metadata["total_exposed_dose"] = 1
-            num_fractions = int(
-                data["MicroscopeImage"]["microscopeData"]["acquisition"]["camera"][
-                    "CameraSpecificInput"
-                ]["a:KeyValueOfstringanyType"][2]["a:Value"]["b:NumberOffractions"]
-            )
+            try:
+                num_fractions = int(
+                    data["MicroscopeImage"]["microscopeData"]["acquisition"]["camera"][
+                        "CameraSpecificInput"
+                    ]["a:KeyValueOfstringanyType"][2]["a:Value"]["b:NumberOffractions"]
+                )
+            except (KeyError, IndexError):
+                pass
             metadata["c2aperture"] = data["MicroscopeImage"]["CustomData"][
                 "a:KeyValueOfstringanyType"
             ][3]["a:Value"]["#text"]
             metadata["exposure_time"] = data["MicroscopeImage"]["microscopeData"][
                 "acquisition"
             ]["camera"]["ExposureTime"]
             metadata["slit_width"] = data["MicroscopeImage"]["microscopeData"][
@@ -303,14 +307,28 @@
             else None
         ) or 0
         metadata["estimate_particle_diameter"] = (
             environment.data_collection_parameters.get("estimate_particle_diameter")
             if environment
             else None
         ) or True
+        images_disc_index: int = 0
+        for i, p in enumerate(metadata_file.parts):
+            if p.startswith("Images-Disc"):
+                images_disc_index = i
+        if images_disc_index:
+            data_file = (
+                Path("/".join(metadata_file.parts[: images_disc_index - 2]))
+                / "/".join(metadata_file.parts[images_disc_index - 1 : -1])
+                / metadata_file.with_suffix(".eer").name
+            )
+            if data_file.is_file():
+                metadata["num_eer_frames"] = murfey.util.eer.num_frames(
+                    metadata_file.parent.parent / metadata_file.parent.name / data_file
+                )
         return metadata
 
 
 class SPAModularContext(_SPAContext):
     def post_transfer(
         self,
         transferred_file: Path,
```

### Comparing `murfey-0.9.8/src/murfey/client/contexts/tomo.py` & `murfey-0.9.9/src/murfey/client/contexts/tomo.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/customlogging.py` & `murfey-0.9.9/src/murfey/client/customlogging.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/gain_ref.py` & `murfey-0.9.9/src/murfey/client/gain_ref.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/instance_environment.py` & `murfey-0.9.9/src/murfey/client/instance_environment.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/rsync.py` & `murfey-0.9.9/src/murfey/client/rsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,16 @@
         """
         previously_transferred = self._files_transferred
 
         next_file: RSyncerUpdate | None = None
         transfer_success: set[Path] = set()
         successful_updates: list[RSyncerUpdate] = []
 
+        files = [f for f in files if f.is_file()]
+
         def parse_stdout(line: str):
             nonlocal next_file
 
             if not line:
                 return
 
             if chr(13) in line:
```

### Comparing `murfey-0.9.8/src/murfey/client/tui/app.py` & `murfey-0.9.9/src/murfey/client/tui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,14 +607,21 @@
             for a in self.analysers.values():
                 a.stop()
         if self._multigrid_watcher:
             self._multigrid_watcher.stop()
         self.exit()
         exit()
 
+    def clean_up_quit(self) -> None:
+        requests.delete(
+            f"{self._environment.url.geturl()}/clients/{self._environment.client_id}/session"
+        )
+        self.exit()
+        exit()
+
     async def action_clear(self) -> None:
         machine_config = get_machine_config(
             str(self._environment.url.geturl()), demo=self._environment.demo
         )
         if self.rsync_processes and machine_config.get("allow_removal"):
             sources = "\n".join(str(k) for k in self.rsync_processes.keys())
             prompt = f"Remove files from the following: {sources}"
```

### Comparing `murfey-0.9.8/src/murfey/client/tui/controller.css` & `murfey-0.9.9/src/murfey/client/tui/controller.css`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/tui/progress.py` & `murfey-0.9.9/src/murfey/client/tui/progress.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/tui/screens.py` & `murfey-0.9.9/src/murfey/client/tui/screens.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,16 +317,15 @@
             if cfg.get("modular_spa"):
                 self._context = SPAContext
             else:
                 self._context = SPAModularContext
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "quit":
-            self.app.exit()
-            exit()
+            self.app.clean_up_quit()
         elif event.button.id == "add":
             self._add_directory(self._dir_tree._selected_path)
         elif event.button.id == "launch":
             text = self.app._visit
             visit_path = ""
             transfer_routes = {}
             for s, defd in self.app._default_destinations.items():
```

### Comparing `murfey-0.9.8/src/murfey/client/tui/status_bar.py` & `murfey-0.9.9/src/murfey/client/tui/status_bar.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/update.py` & `murfey-0.9.9/src/murfey/client/update.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/watchdir.py` & `murfey-0.9.9/src/murfey/client/watchdir.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/watchdir_multigrid.py` & `murfey-0.9.9/src/murfey/client/watchdir_multigrid.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/client/websocket.py` & `murfey-0.9.9/src/murfey/client/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/server/__init__.py` & `murfey-0.9.9/src/murfey/server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,15 +580,15 @@
             selection_stash = _db.exec(
                 select(db.SelectionStash).where(db.SelectionStash.pj_id == pj_id)
             ).all()
             for s in selection_stash:
                 _register_class_selection(
                     {
                         "session_id": s.session_id,
-                        "class_selection_score": s.class_selection_score,
+                        "class_selection_score": s.class_selection_score or 0,
                     },
                     _db=_db,
                     demo=demo,
                 )
                 _db.delete(s)
                 _db.commit()
 
@@ -774,15 +774,15 @@
                 "particles_file": first_class2d.particles_file,
                 "class2d_dir": message["job_dir"],
                 "batch_is_complete": first_class2d.complete,
                 "batch_size": first_class2d.batch_size,
                 "particle_diameter": relion_params.particle_diameter,
                 "mask_diameter": relion_params.mask_diameter or 0,
                 "combine_star_job_number": feedback_params.star_combination_job,
-                "autoselect_min_score": feedback_params.class_selection_score,
+                "autoselect_min_score": feedback_params.class_selection_score or 0,
                 "autoproc_program_id": message["program_id"],
                 "pix_size": relion_params.angpix,
                 "fm_dose": relion_params.dose_per_frame,
                 "kv": relion_params.voltage,
                 "gain_ref": relion_params.gain_ref,
                 "nr_iter": default_spa_parameters.nr_iter_2d,
                 "nr_classes": default_spa_parameters.nr_classes_2d,
@@ -1192,15 +1192,15 @@
             "parameters": {
                 "particles_file": class2d_message["particles_file"],
                 "class2d_dir": f"{class2d_message['class2d_dir']}{feedback_params.next_job:03}",
                 "batch_is_complete": True,
                 "particle_diameter": relion_params.particle_diameter,
                 "mask_diameter": relion_params.mask_diameter or 0,
                 "combine_star_job_number": feedback_params.star_combination_job,
-                "autoselect_min_score": feedback_params.class_selection_score,
+                "autoselect_min_score": feedback_params.class_selection_score or 0,
                 "picker_id": feedback_params.picker_ispyb_id,
                 "class_uuids": class_uuids,
                 "class2d_grp_uuid": class2d_grp_uuid,
                 "pix_size": relion_params.angpix,
                 "fm_dose": relion_params.dose_per_frame,
                 "kv": relion_params.voltage,
                 "gain_ref": relion_params.gain_ref,
@@ -1278,15 +1278,15 @@
                 "particles_file": saved_message.particles_file,
                 "class2d_dir": f"{saved_message.class2d_dir}{feedback_params.next_job:03}",
                 "batch_is_complete": True,
                 "batch_size": saved_message.batch_size,
                 "particle_diameter": relion_params.particle_diameter,
                 "mask_diameter": relion_params.mask_diameter or 0,
                 "combine_star_job_number": feedback_params.star_combination_job,
-                "autoselect_min_score": feedback_params.class_selection_score,
+                "autoselect_min_score": feedback_params.class_selection_score or 0,
                 "picker_id": feedback_params.picker_ispyb_id,
                 "class_uuids": _2d_class_murfey_ids(
                     saved_message.particles_file, _app_id(pj_id, _db), _db
                 ),
                 "class2d_grp_uuid": saved_message.murfey_id,
                 "pix_size": relion_params.angpix,
                 "fm_dose": relion_params.dose_per_frame,
@@ -1334,22 +1334,22 @@
         )
     ).one()
     _db.expunge(feedback_params)
 
     if feedback_params.picker_ispyb_id is None:
         selection_stash = db.SelectionStash(
             pj_id=pj_id,
-            class_selection_score=message["class_selection_score"],
+            class_selection_score=message["class_selection_score"] or 0,
         )
         _db.add(selection_stash)
         _db.commit()
         _db.close()
         return
 
-    feedback_params.class_selection_score = message.get("class_selection_score")
+    feedback_params.class_selection_score = message.get("class_selection_score") or 0
     feedback_params.hold_class2d = False
     next_job = feedback_params.next_job
     if demo:
         for saved_message in class2d_db:
             # Send all held Class2D messages on with the selection score added
             _db.expunge(saved_message)
             particles_file = saved_message.particles_file
@@ -1799,17 +1799,17 @@
                         db.ClientEnvironment.client_id == message["client_id"]
                     )
                 )
                 .one()
                 .session_id
             )
             stashed_files = murfey_db.exec(
-                select(db.PreprocessStash).where(
-                    db.PreprocessStash.client_id == message["client_id"]
-                )
+                select(db.PreprocessStash)
+                .where(db.PreprocessStash.client_id == message["client_id"])
+                .where(db.PreprocessStash.tag == message["tag"])
             ).all()
             if not stashed_files:
                 if _transport_object:
                     _transport_object.transport.ack(header)
                 return None
             machine_config = get_machine_config()
             collected_ids = murfey_db.exec(
```

### Comparing `murfey-0.9.8/src/murfey/server/api.py` & `murfey-0.9.9/src/murfey/server/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,14 +605,16 @@
         db.commit()
         db.close()
 
         if not mrc_out.parent.exists():
             Path(secure_filename(str(mrc_out))).parent.mkdir(
                 parents=True, exist_ok=True
             )
+        if not Path(proc_file.path).is_file():
+            return proc_file
         zocalo_message = {
             "recipes": ["em-spa-preprocess"],
             "parameters": {
                 "feedback_queue": machine_config.feedback_queue,
                 "dcid": detached_ids[1],
                 "kv": proc_params["voltage"],
                 "autoproc_program_id": detached_ids[3],
@@ -627,28 +629,30 @@
                 "gain_ref": str(machine_config.rsync_basepath / proc_params["gain_ref"])
                 if proc_params["gain_ref"]
                 else proc_params["gain_ref"],
                 "downscale": proc_params["downscale"],
                 "picker_uuid": murfey_ids[1],
                 "session_id": session_id,
                 "particle_diameter": proc_params["particle_diameter"] or 0,
+                "fm_int_file": proc_file.eer_fractionation_file,
             },
         }
         # log.info(f"Sending Zocalo message {zocalo_message}")
         if _transport_object:
             _transport_object.send("processing_recipe", zocalo_message)
         else:
             log.error(
                 f"Pe-processing was requested for {sanitise(ppath.name)} but no Zocalo transport object was found"
             )
             return proc_file
 
     else:
         for_stash = PreprocessStash(
             file_path=str(proc_file.path),
+            tag=proc_file.tag,
             client_id=client_id,
             image_number=proc_file.image_number,
             mrc_out=str(mrc_out),
         )
         db.add(for_stash)
         db.commit()
         db.close()
```

### Comparing `murfey-0.9.8/src/murfey/server/bootstrap.py` & `murfey-0.9.9/src/murfey/server/bootstrap.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/server/config.py` & `murfey-0.9.9/src/murfey/server/config.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/server/demo_api.py` & `murfey-0.9.9/src/murfey/server/demo_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,14 +596,15 @@
             demo=True,
         )
         prom.preprocessed_movies.labels(processing_job=1).inc()
 
     else:
         for_stash = PreprocessStash(
             file_path=str(proc_file.path),
+            tag=proc_file.tag,
             client_id=client_id,
             image_number=proc_file.image_number,
             mrc_out=str(mrc_out),
         )
         db.add(for_stash)
         db.commit()
```

### Comparing `murfey-0.9.8/src/murfey/server/gain.py` & `murfey-0.9.9/src/murfey/server/gain.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/server/ispyb.py` & `murfey-0.9.9/src/murfey/server/ispyb.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/server/main.py` & `murfey-0.9.9/src/murfey/server/main.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/server/murfey_db.py` & `murfey-0.9.9/src/murfey/server/murfey_db.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/server/prometheus.py` & `murfey-0.9.9/src/murfey/server/prometheus.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/server/websocket.py` & `murfey-0.9.9/src/murfey/server/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/templates/activevisits.html` & `murfey-0.9.9/src/murfey/templates/activevisits.html`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/templates/base.html` & `murfey-0.9.9/src/murfey/templates/base.html`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/templates/bootstrap.html` & `murfey-0.9.9/src/murfey/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/templates/images/diamond.png` & `murfey-0.9.9/src/murfey/templates/images/diamond.png`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/templates/images/icon_268.png` & `murfey-0.9.9/src/murfey/templates/images/icon_268.png`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/templates/static/styles.css` & `murfey-0.9.9/src/murfey/templates/static/styles.css`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/templates/visit.html` & `murfey-0.9.9/src/murfey/templates/visit.html`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/util/__init__.py` & `murfey-0.9.9/src/murfey/util/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/util/db.py` & `murfey-0.9.9/src/murfey/util/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     class3ds: List["Class3D"] = Relationship(
         back_populates="processing_job", sa_relationship_kwargs={"cascade": "delete"}
     )
 
 
 class PreprocessStash(SQLModel, table=True):  # type: ignore
     file_path: str = Field(primary_key=True)
+    tag: str = Field(primary_key=True)
     client_id: int = Field(primary_key=True, foreign_key="clientenvironment.client_id")
     image_number: int
     mrc_out: str
     client: Optional[ClientEnvironment] = Relationship(
         back_populates="preprocess_stashes"
     )
```

### Comparing `murfey-0.9.8/src/murfey/util/dummy_setup.py` & `murfey-0.9.9/src/murfey/util/dummy_setup.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/util/eer.py` & `murfey-0.9.9/src/murfey/util/eer.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/util/file_monitor.py` & `murfey-0.9.9/src/murfey/util/file_monitor.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/util/mdoc.py` & `murfey-0.9.9/src/murfey/util/mdoc.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/util/models.py` & `murfey-0.9.9/src/murfey/util/models.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/util/rsync.py` & `murfey-0.9.9/src/murfey/util/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey/util/state.py` & `murfey-0.9.9/src/murfey/util/state.py`

 * *Files identical despite different names*

### Comparing `murfey-0.9.8/src/murfey.egg-info/PKG-INFO` & `murfey-0.9.9/src/murfey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.9.8
+Version: 0.9.9
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.9.8/src/murfey.egg-info/SOURCES.txt` & `murfey-0.9.9/src/murfey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

