# Comparing `tmp/runtimepy-4.2.0.tar.gz` & `tmp/runtimepy-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-4.2.0.tar", last modified: Mon Apr 22 04:32:19 2024, max compression
+gzip compressed data, was "runtimepy-4.2.1.tar", last modified: Tue Apr 23 07:48:09 2024, max compression
```

## Comparing `runtimepy-4.2.0.tar` & `runtimepy-4.2.1.tar`

### file list

```diff
@@ -1,304 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.640229 runtimepy-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 04:29:49.000000 runtimepy-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-22 04:32:19.636229 runtimepy-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-22 04:29:49.000000 runtimepy-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-22 04:29:49.000000 runtimepy-4.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.600229 runtimepy-4.2.0/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9270 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/channel/environment/command/
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/command/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/command/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/environment/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/channel/event/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/event/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.604229 runtimepy-4.2.0/runtimepy/codec/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/codec/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.608229 runtimepy-4.2.0/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.608229 runtimepy-4.2.0/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.608229 runtimepy-4.2.0/runtimepy/data/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/css/bootstrap_extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/dummy_load.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/factories.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.608229 runtimepy-4.2.0/runtimepy/data/js/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/audio.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.612229 runtimepy-4.2.0/runtimepy/data/js/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/App.js
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/ChannelTable.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/Plot.js
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/PlotManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/PlotModalManager.js
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/TabFilter.js
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/TabInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/WindowHashManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/classes/WorkerInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/init.js
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.612229 runtimepy-4.2.0/runtimepy/data/js/tab/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/tab/env.js
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/tab/sound.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.612229 runtimepy-4.2.0/runtimepy/data/js/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/unused/pyodide.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/js/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ChannelCommand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/FindFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/PeerProcessConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/StructConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/has_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/schemas/has_request_flag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/server_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/data/server_dev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/enum/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/message/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/message/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/message/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/message/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/metrics/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/metrics/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/metrics/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.616229 runtimepy-4.2.0/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/async_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/config/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/housekeeping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/imports/
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/imports/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/arbiter/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/tcp/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.620229 runtimepy-4.2.0/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/request_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/http/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/app/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/app/env/
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/tab/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/env/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/app/tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.624229 runtimepy-4.2.0/runtimepy/net/server/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/server/websocket/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/stream/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/stream/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/stream/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/stream/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/tcp/http/
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/udp/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.628229 runtimepy-4.2.0/runtimepy/primitives/array/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/primitives/serializable/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/serializable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/serializable/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/serializable/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/serializable/prefixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/primitives/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/primitives/types/int.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/sample/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/sample/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/sample/program.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.632229 runtimepy-4.2.0/runtimepy/subprocess/
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/subprocess/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/basic/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/task/trig/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/task/trig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/tui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-22 04:29:49.000000 runtimepy-4.2.0/runtimepy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 04:32:19.000000 runtimepy-4.2.0/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 04:32:19.640229 runtimepy-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-22 04:29:49.000000 runtimepy-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 04:32:19.636229 runtimepy-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-22 04:29:49.000000 runtimepy-4.2.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-22 04:29:49.000000 runtimepy-4.2.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-22 04:29:49.000000 runtimepy-4.2.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.860686 runtimepy-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 07:45:42.000000 runtimepy-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-23 07:48:09.860686 runtimepy-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-23 07:45:42.000000 runtimepy-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 07:45:42.000000 runtimepy-4.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.824686 runtimepy-4.2.1/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.824686 runtimepy-4.2.1/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.824686 runtimepy-4.2.1/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.828686 runtimepy-4.2.1/runtimepy/channel/environment/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/command/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/command/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/environment/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.828686 runtimepy-4.2.1/runtimepy/channel/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/event/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.828686 runtimepy-4.2.1/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.828686 runtimepy-4.2.1/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.828686 runtimepy-4.2.1/runtimepy/codec/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/codec/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.828686 runtimepy-4.2.1/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.828686 runtimepy-4.2.1/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.832686 runtimepy-4.2.1/runtimepy/data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/css/bootstrap_extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/dummy_load.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/factories.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.832686 runtimepy-4.2.1/runtimepy/data/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/audio.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.832686 runtimepy-4.2.1/runtimepy/data/js/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/App.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/ChannelTable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/Plot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/PlotManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/PlotModalManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/TabFilter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/TabInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/WindowHashManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/classes/WorkerInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.832686 runtimepy-4.2.1/runtimepy/data/js/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/tab/env.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/tab/sound.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.832686 runtimepy-4.2.1/runtimepy/data/js/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/unused/pyodide.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/js/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.836686 runtimepy-4.2.1/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/ChannelCommand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/FindFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/PeerProcessConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/StructConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/has_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/schemas/has_request_flag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/server_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/data/server_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.836686 runtimepy-4.2.1/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/enum/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.836686 runtimepy-4.2.1/runtimepy/message/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/message/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/message/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/message/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.840686 runtimepy-4.2.1/runtimepy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/metrics/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/metrics/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/metrics/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.840686 runtimepy-4.2.1/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mixins/async_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mixins/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mixins/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mixins/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.840686 runtimepy-4.2.1/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.840686 runtimepy-4.2.1/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.840686 runtimepy-4.2.1/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.844686 runtimepy-4.2.1/runtimepy/net/arbiter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/config/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.844686 runtimepy-4.2.1/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.844686 runtimepy-4.2.1/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/housekeeping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.844686 runtimepy-4.2.1/runtimepy/net/arbiter/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/imports/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.844686 runtimepy-4.2.1/runtimepy/net/arbiter/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/tcp/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.844686 runtimepy-4.2.1/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.844686 runtimepy-4.2.1/runtimepy/net/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/http/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/http/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/http/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/http/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.844686 runtimepy-4.2.1/runtimepy/net/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.848686 runtimepy-4.2.1/runtimepy/net/server/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.848686 runtimepy-4.2.1/runtimepy/net/server/app/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/bootstrap/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/bootstrap/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.848686 runtimepy-4.2.1/runtimepy/net/server/app/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/env/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.848686 runtimepy-4.2.1/runtimepy/net/server/app/env/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/env/tab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/env/tab/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/env/tab/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/env/tab/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/env/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/app/tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.848686 runtimepy-4.2.1/runtimepy/net/server/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.848686 runtimepy-4.2.1/runtimepy/net/server/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/server/websocket/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.848686 runtimepy-4.2.1/runtimepy/net/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/stream/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.848686 runtimepy-4.2.1/runtimepy/net/stream/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/stream/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/stream/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/tcp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/tcp/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/net/tcp/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/tcp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/tcp/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/udp/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/primitives/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.852686 runtimepy-4.2.1/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/primitives/serializable/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/serializable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/serializable/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/serializable/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/serializable/prefixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/primitives/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/types/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/types/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/primitives/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/sample/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/sample/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/subprocess/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/subprocess/peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/subprocess/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/subprocess/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/task/basic/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/task/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.856686 runtimepy-4.2.1/runtimepy/task/trig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/task/trig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.860686 runtimepy-4.2.1/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.860686 runtimepy-4.2.1/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.860686 runtimepy-4.2.1/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/tui/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/tui/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/tui/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/tui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-23 07:45:42.000000 runtimepy-4.2.1/runtimepy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.860686 runtimepy-4.2.1/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-23 07:48:09.000000 runtimepy-4.2.1/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-23 07:48:09.000000 runtimepy-4.2.1/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:48:09.000000 runtimepy-4.2.1/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 07:48:09.000000 runtimepy-4.2.1/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 07:48:09.000000 runtimepy-4.2.1/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 07:48:09.000000 runtimepy-4.2.1/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:48:09.860686 runtimepy-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-23 07:45:42.000000 runtimepy-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:48:09.860686 runtimepy-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 07:45:42.000000 runtimepy-4.2.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 07:45:42.000000 runtimepy-4.2.1/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-23 07:45:42.000000 runtimepy-4.2.1/tests/test_resources.py
```

### Comparing `runtimepy-4.2.0/LICENSE` & `runtimepy-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/PKG-INFO` & `runtimepy-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.2.0
+Version: 4.2.1
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,17 +13,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: websockets
 Requires-Dist: vcorelib>=3.2.4
 Requires-Dist: svgen>=0.6.6
+Requires-Dist: websockets
 Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=e23f54e60d0c62ebc1be3cae63bc7678
+    hash=ebb5664a436fde952d2499fe582fccd3
     =====================================
 -->
 
-# runtimepy ([4.2.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.2.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.2.0/README.md` & `runtimepy-4.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=e23f54e60d0c62ebc1be3cae63bc7678
+    hash=ebb5664a436fde952d2499fe582fccd3
     =====================================
 -->
 
-# runtimepy ([4.2.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.2.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.2.0/pyproject.toml` & `runtimepy-4.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "4.2.0"
+version = "4.2.1"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-4.2.0/runtimepy/app.py` & `runtimepy-4.2.1/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/__init__.py` & `runtimepy-4.2.1/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/array.py` & `runtimepy-4.2.1/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/base.py` & `runtimepy-4.2.1/runtimepy/channel/environment/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 
         # Register fields.
         self.fields = _BitFieldsManager(channels.names, self.enums)
         if fields:
             for field in fields:
                 self.fields.add(field)
 
+        self.to_add: list[_BitFields] = []
+
         # Keep a mapping of each channel's name and integer identifier to the
         # underlying enumeration.
         self.channel_enums: dict[_AnyChannel, _RuntimeEnum] = {
             chan: self.enums[chan.enum]
             for chan in self.channels.items.values()
             if chan.is_enum
         }
@@ -278,7 +280,24 @@
         chan = self.get(key)
         if chan is not None:
             prim = chan[0].raw
         else:
             prim = self.fields[key].raw
 
         return prim.age_ns()
+
+    def add_field(self, field: _BitField, namespace: Namespace = None) -> str:
+        """Add a bit field to the environment."""
+
+        result = self.fields.add_field(field)
+        if result is not None:
+            self.to_add.append(result)
+
+        return self.namespace(name=field.name, namespace=namespace)
+
+    def finalize(self, strict: bool = True) -> None:
+        """Finalize this instance."""
+
+        for fields in self.to_add:
+            self.fields.add(fields)
+
+        super().finalize(strict=strict)
```

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/command/__init__.py` & `runtimepy-4.2.1/runtimepy/channel/environment/command/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from runtimepy.channel.environment.base import FieldOrChannel
 from runtimepy.channel.environment.command.processor import (
     ChannelCommandProcessor,
     CommandHook,
     EnvironmentMap,
 )
 from runtimepy.channel.registry import ParsedEvent
-from runtimepy.mapping import DEFAULT_PATTERN, name_search
+from runtimepy.mapping import DEFAULT_PATTERN
+from runtimepy.util import name_search
 
 # Declared so we re-export FieldOrChannel after moving where it's declared.
 __all__ = [
     "CommandHook",
     "FieldOrChannel",
     "EnvironmentMap",
     "GLOBAL",
@@ -111,15 +112,15 @@
 
     def read_event_stream(
         self, env: str, path: str = EVENT_OUT
     ) -> Iterator[ParsedEvent]:
         """Reade events from a specific environment."""
 
         with self.valid_root.joinpath(env, path).open("rb") as path_fd:
-            yield from self[env].env.channels.parse_event_stream(path_fd)
+            yield from self[env].env.parse_event_stream(path_fd)
 
     def export(self, env: str) -> Path:
         """Export an environment to a sub-directory of the root directory."""
 
         out = self.valid_root.joinpath(env)
         out.mkdir(exist_ok=True, parents=True)
```

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/command/parser.py` & `runtimepy-4.2.1/runtimepy/channel/environment/command/parser.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/command/processor.py` & `runtimepy-4.2.1/runtimepy/channel/environment/command/processor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/command/result.py` & `runtimepy-4.2.1/runtimepy/channel/environment/command/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/create.py` & `runtimepy-4.2.1/runtimepy/channel/environment/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 from runtimepy.channel.environment.base import ChannelResult as _ChannelResult
 from runtimepy.enum import RuntimeEnum as _RuntimeEnum
 from runtimepy.enum.registry import DEFAULT_ENUM_PRIMITIVE
 from runtimepy.enum.types import EnumTypelike as _EnumTypelike
 from runtimepy.mapping import EnumMappingData as _EnumMappingData
 from runtimepy.primitives import ChannelScaling, Primitive
 from runtimepy.primitives import Primitivelike as _Primitivelike
-from runtimepy.primitives.field import BitField
-from runtimepy.primitives.field.fields import BitFields
 from runtimepy.registry.name import RegistryKey as _RegistryKey
 
 
 class CreateChannelEnvironment(_BaseChannelEnvironment):
     """An environment extension for creating channels."""
 
     def channel(
@@ -180,19 +178,7 @@
             self.namespace(name=name, namespace=namespace),
             kind=kind,
             items=items,
             primitive=primitive,
         )
         assert result is not None, f"Can't create enum '{name}'!"
         return result
-
-    def add_field(self, field: BitField, namespace: _Namespace = None) -> str:
-        """Add a bit field to the environment."""
-
-        fields = BitFields.new()
-        fields.claim_field(field)
-
-        name = self.namespace(name=field.name, namespace=namespace)
-
-        self.fields.add(fields)
-
-        return name
```

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/file.py` & `runtimepy-4.2.1/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/environment/sample.py` & `runtimepy-4.2.1/runtimepy/channel/environment/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/event/__init__.py` & `runtimepy-4.2.1/runtimepy/channel/event/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,22 +40,23 @@
 
     @contextmanager
     def registered(
         self,
         stream: BinaryIO,
         flush: bool = False,
         channel: ChannelMetrics = None,
+        force: bool = False,
     ) -> Iterator[None]:
         """Register a stream as a managed context."""
 
         assert not self.streaming, "Already streaming!"
 
         def callback(_, __) -> None:
             """Emit a change event to the stream."""
-            self._poll(stream, flush=flush, channel=channel)
+            self._poll(stream, flush=flush, channel=channel, force=force)
 
         # Poll immediately.
         self.prev_ns = 0
 
         self._poll(stream, flush=flush, channel=channel)
 
         raw = self.primitive
@@ -67,27 +68,28 @@
         self.streaming = False
 
     def _poll(
         self,
         stream: BinaryIO,
         flush: bool = False,
         channel: ChannelMetrics = None,
+        force: bool = False,
     ) -> int:
         """
         Poll this event so that if the underlying channel has changed since the
         last write, we write another event.
         """
 
         written = 0
 
         # Check timestamp and update header if necessary.
         raw = self.primitive
         curr_ns = raw.last_updated_ns
 
-        if curr_ns - self.prev_ns >= self.min_period_ns:
+        if force or curr_ns - self.prev_ns >= self.min_period_ns:
             self.prev_ns = curr_ns
             self.header["timestamp"] = curr_ns
 
             # Write header then value.
             array = self.header.array
             written += array.to_stream(stream)
             written += raw.to_stream(stream, byte_order=array.byte_order)
```

### Comparing `runtimepy-4.2.0/runtimepy/channel/event/header.py` & `runtimepy-4.2.1/runtimepy/channel/event/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/channel/registry.py` & `runtimepy-4.2.1/runtimepy/channel/registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # built-in
 from contextlib import ExitStack, contextmanager
 from typing import Any as _Any
 from typing import BinaryIO, Iterable, Iterator, NamedTuple
 from typing import Optional as _Optional
-from typing import Union, cast
+from typing import Union
 
 # third-party
 from vcorelib.io import ByteFifo
 from vcorelib.io.types import JsonObject as _JsonObject
 
 # internal
 from runtimepy.channel import AnyChannel as _AnyChannel
@@ -146,51 +146,7 @@
             for name, chan in self.search(pattern, exact=exact):
                 stack.enter_context(
                     chan.event.registered(stream, flush=flush, channel=channel)
                 )
                 names.append(name)
 
             yield names
-
-    def parse_event_stream(self, stream: BinaryIO) -> Iterator[ParsedEvent]:
-        """Parse individual events from a stream."""
-
-        # Ingest stream.
-        self.event_fifo.ingest(stream.read())
-
-        ident = -1
-        name = ""
-
-        keep_going = True
-        while keep_going:
-            keep_going = False
-
-            # Read header.
-            if not self.header_ready:
-                read_size = self.event_header.size
-                data = self.event_fifo.pop(read_size)
-                if data is not None:
-                    self.event_header.array.update(data)
-
-                    # Update local variables.
-                    ident = cast(int, self.event_header["identifier"])
-                    name = self.names.name(ident)  # type: ignore
-                    assert name is not None, ident
-
-                    # Update state.
-                    self.header_ready = True
-                    keep_going = True
-            else:
-                kind = self[name].type
-                data = self.event_fifo.pop(kind.size)
-                if data is not None:
-                    yield ParsedEvent(
-                        name,
-                        cast(int, self.event_header["timestamp"]),
-                        kind.decode(
-                            data, byte_order=self.event_header.array.byte_order
-                        ),
-                    )
-
-                    # Update state.
-                    self.header_ready = False
-                    keep_going = True
```

### Comparing `runtimepy-4.2.0/runtimepy/codec/protocol/__init__.py` & `runtimepy-4.2.1/runtimepy/codec/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/codec/protocol/base.py` & `runtimepy-4.2.1/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/codec/protocol/json.py` & `runtimepy-4.2.1/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/codec/system/__init__.py` & `runtimepy-4.2.1/runtimepy/codec/system/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/commands/all.py` & `runtimepy-4.2.1/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/commands/arbiter.py` & `runtimepy-4.2.1/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/commands/common.py` & `runtimepy-4.2.1/runtimepy/commands/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/commands/server.py` & `runtimepy-4.2.1/runtimepy/commands/server.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/commands/task.py` & `runtimepy-4.2.1/runtimepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/commands/tui.py` & `runtimepy-4.2.1/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/css/bootstrap_extra.css` & `runtimepy-4.2.1/runtimepy/data/css/bootstrap_extra.css`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/dummy_load.yaml` & `runtimepy-4.2.1/runtimepy/data/dummy_load.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,29 @@
   - {name: sample3, factory: Sample, period_s: 1.1}
 
   # Sinusoids.
   - {name: wave1, factory: sinusoid, period_s: 0.01}
   - {name: wave2, factory: sinusoid, period_s: 0.02}
   - {name: wave3, factory: sinusoid, period_s: 0.03}
 
+  # Drive interactions with runtime entities that won't otherwise be polled.
+  - {name: app, factory: SampleApp, period_s: 0.25}
+
+# UDP JSON clients.
+clients:
+  - factory: udp_json
+    name: udp_json_client
+    defer: true
+    kwargs:
+      remote_addr: [localhost, "$udp_json"]
+  - factory: udp_json
+    name: udp_json_server
+    kwargs:
+      local_addr: [localhost, "$udp_json"]
+
 # Add some sample structs.
 structs:
   - name: example.struct1
     factory: sample_struct
     # Not actually used.
     config: &cfg
       a: 1
```

### Comparing `runtimepy-4.2.0/runtimepy/data/factories.yaml` & `runtimepy-4.2.1/runtimepy/data/factories.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   - {name: runtimepy.net.factories.RuntimepyHttp}
   - {name: runtimepy.net.factories.RuntimepyWebsocketJson}
   - {name: runtimepy.net.factories.RuntimepyWebsocketData}
 
   # Useful tasks.
   - {name: runtimepy.task.trig.Sinusoid}
   - {name: runtimepy.task.sample.Sample}
+  - {name: runtimepy.task.sample.SampleApp}
 
   # Useful structs.
   - {name: runtimepy.net.arbiter.info.SampleStruct}
   - {name: runtimepy.net.server.struct.UiState}
 
   # Useful subprocess peer interfaces.
   - {name: runtimepy.sample.peer.SamplePeer}
```

### Comparing `runtimepy-4.2.0/runtimepy/data/favicon.ico` & `runtimepy-4.2.1/runtimepy/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/JsonConnection.js` & `runtimepy-4.2.1/runtimepy/data/js/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/audio.js` & `runtimepy-4.2.1/runtimepy/data/js/audio.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/App.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/App.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/ChannelTable.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/ChannelTable.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/JsonConnection.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/Plot.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/Plot.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/PlotManager.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/PlotManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/PlotModalManager.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/PlotModalManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/TabFilter.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/TabFilter.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/TabInterface.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/TabInterface.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/classes/WindowHashManager.js` & `runtimepy-4.2.1/runtimepy/data/js/classes/WindowHashManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/tab/sound.js` & `runtimepy-4.2.1/runtimepy/data/js/tab/sound.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/unused/pyodide.js` & `runtimepy-4.2.1/runtimepy/data/js/unused/pyodide.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/util.js` & `runtimepy-4.2.1/runtimepy/data/js/util.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/js/worker.js` & `runtimepy-4.2.1/runtimepy/data/js/worker.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-4.2.1/runtimepy/data/schemas/BitFields.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,17 @@
       additionalProperties: false
 
       properties:
         name:
           type: string
           pattern: "^[a-z0-9-_.]+$"
 
+        commandable:
+          type: boolean
+
         description:
           type: string
 
         index:
           type: integer
           minimum: 0
```

### Comparing `runtimepy-4.2.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-4.2.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/schemas/FindFile.yaml` & `runtimepy-4.2.1/runtimepy/data/schemas/FindFile.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/data/server_base.yaml` & `runtimepy-4.2.1/runtimepy/data/server_base.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/entry.py` & `runtimepy-4.2.1/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/enum/__init__.py` & `runtimepy-4.2.1/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/enum/registry.py` & `runtimepy-4.2.1/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/enum/types.py` & `runtimepy-4.2.1/runtimepy/enum/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/mapping.py` & `runtimepy-4.2.1/runtimepy/mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 A module implementing a generic, two-way mapping interface.
 """
 
 # built-in
-import re
 from typing import Generic as _Generic
-from typing import Iterable, Iterator
+from typing import Iterator
 from typing import MutableMapping as _MutableMapping
 from typing import Optional as _Optional
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.logging import LoggerMixin
 
 # internal
 from runtimepy.mixins.regex import RegexMixin as _RegexMixin
+from runtimepy.util import name_search
 
 # This determines types that are valid as keys.
 T = _TypeVar("T", int, bool)
 
 KeyToName = _MutableMapping[T, str]
 NameToKey = _MutableMapping[str, T]
 MappingKey = _Union[str, T]
@@ -35,26 +35,14 @@
     BoolMappingData,
     _MutableMapping[str, bool],
     _MutableMapping[str, int],
 ]
 DEFAULT_PATTERN = ".*"
 
 
-def name_search(
-    names: Iterable[str], pattern: str, exact: bool = False
-) -> Iterator[str]:
-    """A simple name searching method."""
-
-    compiled = re.compile(pattern)
-    for name in names:
-        if compiled.search(name) is not None:
-            if not exact or name == pattern:
-                yield name
-
-
 class TwoWayNameMapping(_RegexMixin, LoggerMixin, _Generic[T]):
     """A class interface for managing two-way mappings."""
 
     def __init__(
         self,
         mapping: KeyToName[T] = None,
         reverse: NameToKey[T] = None,
```

### Comparing `runtimepy-4.2.0/runtimepy/message/__init__.py` & `runtimepy-4.2.1/runtimepy/message/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/message/handlers.py` & `runtimepy-4.2.1/runtimepy/message/handlers.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/message/interface.py` & `runtimepy-4.2.1/runtimepy/message/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,29 +35,15 @@
     DEFAULT_LOOPBACK,
     DEFAULT_TIMEOUT,
     RESERVED_KEYS,
     MessageHandler,
     T,
     TypedHandler,
 )
-from runtimepy.util import ListLogger
-
-
-class Identifier:
-    """A simple message indentifier interface."""
-
-    def __init__(self) -> None:
-        """Initialize this instance."""
-        self.curr_id: int = 1
-
-    def __call__(self) -> int:
-        """Get the next identifier."""
-        curr = self.curr_id
-        self.curr_id += 2
-        return curr
+from runtimepy.util import Identifier, ListLogger
 
 
 class JsonMessageInterface:
     """A JSON messaging interface class."""
 
     logger: LoggerType
     processor: MessageProcessor
@@ -107,21 +93,37 @@
             self.meta["handlers"],
         )
 
     def _register_handlers(self) -> None:
         """Register connection-specific command handlers."""
 
         # Extra handlers.
+        self.basic_handler("poll", self._poll_handler)
         self.typed_handler("find_file", FindFile, find_file_request_handler)
         self.typed_handler(
             "channel_command",
             ChannelCommand,
             channel_env_handler(ENVIRONMENTS.data, self.command),
         )
 
+    async def poll_handler(self) -> None:
+        """Poll this instance."""
+
+    async def _poll_handler(
+        self, outbox: JsonMessage, inbox: JsonMessage
+    ) -> None:
+        """Handle a 'poll' message."""
+
+        await self.poll_handler()
+
+        # Handle loopback.
+        val = inbox.get("loopback", 0)
+        if val > 0:
+            outbox["loopback"] = val - 1
+
     def typed_handler(
         self, key: str, kind: type[T], handler: TypedHandler[T]
     ) -> None:
         """Register a typed handler."""
 
         assert self.targets.register(key, (key, handler, kind))
```

### Comparing `runtimepy-4.2.0/runtimepy/message/types.py` & `runtimepy-4.2.1/runtimepy/message/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/metrics/channel.py` & `runtimepy-4.2.1/runtimepy/metrics/channel.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/metrics/connection.py` & `runtimepy-4.2.1/runtimepy/metrics/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/metrics/task.py` & `runtimepy-4.2.1/runtimepy/metrics/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/mixins/async_command.py` & `runtimepy-4.2.1/runtimepy/mixins/async_command.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/mixins/enum.py` & `runtimepy-4.2.1/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/mixins/environment.py` & `runtimepy-4.2.1/runtimepy/mixins/environment.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/mixins/finalize.py` & `runtimepy-4.2.1/runtimepy/mixins/finalize.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/mixins/logging.py` & `runtimepy-4.2.1/runtimepy/mixins/logging.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/mixins/psutil.py` & `runtimepy-4.2.1/runtimepy/mixins/psutil.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/mixins/regex.py` & `runtimepy-4.2.1/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/__init__.py` & `runtimepy-4.2.1/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/apps/__init__.py` & `runtimepy-4.2.1/runtimepy/net/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/__init__.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/base.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/config/__init__.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/config/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/config/codec.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/config/codec.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/config/util.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/config/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/factory/task.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/imports/__init__.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/imports/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/imports/util.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/imports/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/info.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/result.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/task.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/tcp/__init__.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/tcp/json.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/tcp/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/udp.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/arbiter/websocket.py` & `runtimepy-4.2.1/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/backoff.py` & `runtimepy-4.2.1/runtimepy/net/backoff.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/connection.py` & `runtimepy-4.2.1/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/factories/__init__.py` & `runtimepy-4.2.1/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/http/__init__.py` & `runtimepy-4.2.1/runtimepy/net/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/http/common.py` & `runtimepy-4.2.1/runtimepy/net/http/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/http/header.py` & `runtimepy-4.2.1/runtimepy/net/http/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/http/request_target.py` & `runtimepy-4.2.1/runtimepy/net/http/request_target.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/http/response.py` & `runtimepy-4.2.1/runtimepy/net/http/response.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/http/state.py` & `runtimepy-4.2.1/runtimepy/net/http/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/http/version.py` & `runtimepy-4.2.1/runtimepy/net/http/version.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/manager.py` & `runtimepy-4.2.1/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/mixin.py` & `runtimepy-4.2.1/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/__init__.py` & `runtimepy-4.2.1/runtimepy/net/server/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/__init__.py` & `runtimepy-4.2.1/runtimepy/net/server/app/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/base.py` & `runtimepy-4.2.1/runtimepy/net/server/app/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/__init__.py` & `runtimepy-4.2.1/runtimepy/net/server/app/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/elements.py` & `runtimepy-4.2.1/runtimepy/net/server/app/bootstrap/elements.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/bootstrap/tabs.py` & `runtimepy-4.2.1/runtimepy/net/server/app/bootstrap/tabs.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/create.py` & `runtimepy-4.2.1/runtimepy/net/server/app/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/env/__init__.py` & `runtimepy-4.2.1/runtimepy/net/server/app/env/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/env/modal.py` & `runtimepy-4.2.1/runtimepy/net/server/app/env/modal.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/env/tab/__init__.py` & `runtimepy-4.2.1/runtimepy/net/server/app/env/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/env/tab/base.py` & `runtimepy-4.2.1/runtimepy/net/server/app/env/tab/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/env/tab/html.py` & `runtimepy-4.2.1/runtimepy/net/server/app/env/tab/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/env/tab/message.py` & `runtimepy-4.2.1/runtimepy/net/server/app/env/tab/message.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/env/widgets.py` & `runtimepy-4.2.1/runtimepy/net/server/app/env/widgets.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/files.py` & `runtimepy-4.2.1/runtimepy/net/server/app/files.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/placeholder.py` & `runtimepy-4.2.1/runtimepy/net/server/app/placeholder.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/sound.py` & `runtimepy-4.2.1/runtimepy/net/server/app/sound.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/app/tab.py` & `runtimepy-4.2.1/runtimepy/net/server/app/tab.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/html.py` & `runtimepy-4.2.1/runtimepy/net/server/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/json.py` & `runtimepy-4.2.1/runtimepy/net/server/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/struct/__init__.py` & `runtimepy-4.2.1/runtimepy/net/server/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/websocket/__init__.py` & `runtimepy-4.2.1/runtimepy/net/server/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/server/websocket/state.py` & `runtimepy-4.2.1/runtimepy/net/server/websocket/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/stream/__init__.py` & `runtimepy-4.2.1/runtimepy/net/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/stream/base.py` & `runtimepy-4.2.1/runtimepy/net/stream/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/stream/json/__init__.py` & `runtimepy-4.2.1/runtimepy/net/stream/json/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/stream/string.py` & `runtimepy-4.2.1/runtimepy/net/stream/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/tcp/connection.py` & `runtimepy-4.2.1/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/tcp/create.py` & `runtimepy-4.2.1/runtimepy/net/tcp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/tcp/http/__init__.py` & `runtimepy-4.2.1/runtimepy/net/tcp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/tcp/protocol.py` & `runtimepy-4.2.1/runtimepy/net/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-4.2.1/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-4.2.1/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/udp/connection.py` & `runtimepy-4.2.1/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/udp/create.py` & `runtimepy-4.2.1/runtimepy/net/udp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/udp/protocol.py` & `runtimepy-4.2.1/runtimepy/net/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/util.py` & `runtimepy-4.2.1/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/net/websocket/connection.py` & `runtimepy-4.2.1/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/__init__.py` & `runtimepy-4.2.1/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/array/__init__.py` & `runtimepy-4.2.1/runtimepy/primitives/array/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/base.py` & `runtimepy-4.2.1/runtimepy/primitives/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,43 +16,53 @@
 # internal
 from runtimepy.primitives.byte_order import (
     DEFAULT_BYTE_ORDER as _DEFAULT_BYTE_ORDER,
 )
 from runtimepy.primitives.byte_order import ByteOrder as _ByteOrder
 from runtimepy.primitives.scaling import ChannelScaling, Numeric, apply, invert
 from runtimepy.primitives.types import AnyPrimitiveType as _AnyPrimitiveType
+from runtimepy.util import Identifier
 
 T = _TypeVar("T", bool, int, float)
 
 # Current value first, new value next.
 PrimitiveChangeCallaback = _Callable[[T, T], None]
 
+IDENT = Identifier()
+IDENT.curr_id = 0
+IDENT.scale = 1
+
 
 class Primitive(_Generic[T]):
     """A simple class for storing and underlying primitive value."""
 
     # Use network byte-order by default.
     byte_order: _ByteOrder = _DEFAULT_BYTE_ORDER
 
     # Nominally set the primitive type at the class level.
     kind: _AnyPrimitiveType
 
+    def __hash__(self) -> int:
+        """A hash for this instance."""
+        return self._hash
+
     def __init__(
         self, value: T = None, scaling: ChannelScaling = None
     ) -> None:
         """Initialize this primitive."""
 
         self.raw = self.kind.instance()
         self.curr_callback: int = 0
         self.callbacks: dict[int, tuple[PrimitiveChangeCallaback[T], bool]] = (
             {}
         )
         self(value=value)
         self.last_updated_ns: int = default_time_ns()
         self.scaling = scaling
+        self._hash = IDENT()
 
     def age_ns(self, now: int = None) -> int:
         """Get the age of this primitive's value in nanoseconds."""
 
         if now is None:
             now = default_time_ns()
```

### Comparing `runtimepy-4.2.0/runtimepy/primitives/bool.py` & `runtimepy-4.2.1/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/byte_order.py` & `runtimepy-4.2.1/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/field/__init__.py` & `runtimepy-4.2.1/runtimepy/primitives/field/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
             "name": self.name,
             "index": self.index,
             "width": self.width,
             "value": self(),
         }
         if self.is_enum:
             result["enum"] = self.enum
+        if self.commandable:
+            result["commandable"] = True
         return result
 
 
 class BitFlag(BitField):
     """A bit field that is always a single bit."""
 
     def __init__(
```

### Comparing `runtimepy-4.2.0/runtimepy/primitives/field/fields.py` & `runtimepy-4.2.1/runtimepy/primitives/field/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,33 +50,43 @@
 
         # Load initial fields and flags.
         for item in _cast(list[dict[str, int]], data["fields"]):
             name: str = _cast(str, item.get("name", ""))
             index: _Optional[int] = item.get("index")
             width: int = item["width"]
             value: int = int(item["value"])
+            commandable: bool = bool(item.get("commandable", False))
             enum = item.get("enum")
             desc: _Optional[str] = _cast(str, item.get("description"))
 
             # Fields without names are considered padding.
             if not name:
                 assert value == 0, "Can't set padding to non-zero value!"
                 assert enum is None, f"Enum '{enum}' specified for padding!"
                 item["index"] = self.pad(width=width, index=index)
                 continue
 
             if width == 1:
                 flag = self.flag(
-                    name, index=index, enum=enum, description=desc
+                    name,
+                    index=index,
+                    enum=enum,
+                    description=desc,
+                    commandable=commandable,
                 )
                 flag(value)
                 item["index"] = flag.index
             else:
                 field = self.field(
-                    name, width, index=index, enum=enum, description=desc
+                    name,
+                    width,
+                    index=index,
+                    enum=enum,
+                    description=desc,
+                    commandable=commandable,
                 )
                 field(value)
                 item["index"] = field.index
 
         self._finalized: bool = _cast(bool, data["finalized"])
 
     @property
@@ -128,21 +138,22 @@
 
     def flag(
         self,
         name: str,
         index: int = None,
         enum: _RegistryKey = None,
         description: str = None,
+        **kwargs,
     ) -> _BitFlag:
         """Create a new bit flag."""
 
         index = self._claim_bits(1, index=index)
 
         result = _BitFlag(
-            name, self.raw, index, enum=enum, description=description
+            name, self.raw, index, enum=enum, description=description, **kwargs
         )
 
         self.fields[name] = result
         self.by_index[index] = result
         return result
 
     def _claim_bits(self, width: int, index: int = None) -> int:
@@ -191,27 +202,29 @@
     def field(
         self,
         name: str,
         width: int,
         index: int = None,
         enum: _RegistryKey = None,
         description: str = None,
+        **kwargs,
     ) -> _BitField:
         """Create a new bit field."""
 
         assert width != 1, "Use bit-flags for single-width fields!"
 
         return self.claim_field(
             _BitField(
                 name,
                 self.raw,
                 self._claim_bits(width, index=index),
                 width,
                 enum=enum,
                 description=description,
+                **kwargs,
             )
         )
 
     @classmethod
     def new(cls: type[T], value: _Primitivelike = "uint8") -> T:
         """Create a new bit-field storage entity."""
```

### Comparing `runtimepy-4.2.0/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-4.2.1/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/field/manager/base.py` & `runtimepy-4.2.1/runtimepy/primitives/field/manager/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from vcorelib.io.types import EncodeResult as _EncodeResult
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.paths import Pathlike as _Pathlike
 
 # internal
 from runtimepy.enum import RuntimeEnum as _RuntimeEnum
 from runtimepy.enum.registry import EnumRegistry as _EnumRegistry
-from runtimepy.primitives import StrToBool
+from runtimepy.primitives import AnyPrimitive, StrToBool
 from runtimepy.primitives.field import BitField as _BitField
 from runtimepy.primitives.field import BitFlag as _BitFlag
 from runtimepy.primitives.field.fields import BitFields as _BitFields
 from runtimepy.registry.name import NameRegistry as _NameRegistry
 from runtimepy.registry.name import RegistryKey as _RegistryKey
 
 
@@ -57,14 +57,15 @@
         self.registry = registry
         self.enums = enums
 
         if fields is None:
             fields = []
 
         self.fields: list[_BitFields] = []
+        self.by_primitive: dict[AnyPrimitive, _BitFields] = {}
         self.lookup: dict[str, int] = {}
         self.enum_lookup: dict[str, _RuntimeEnum] = {}
 
         # Add initial fields.
         for field in fields:
             self.add(field)
 
@@ -191,7 +192,24 @@
     def __getitem__(self, key: _RegistryKey) -> _BitField:
         """Attempt to get a bit-field."""
 
         result = self.get_field(key)
         if result is None:
             raise KeyError(f"No field '{key}'!")
         return result
+
+    def add_field(self, field: _BitField) -> _Optional[_BitFields]:
+        """Add a bit field to the environment."""
+
+        prim = field.raw
+        new_primitive = prim not in self.by_primitive
+        new_fields = None
+
+        if new_primitive:
+            new_fields = _BitFields.new()
+            new_fields.raw = prim
+            self.by_primitive[prim] = new_fields
+
+        self.by_primitive[prim].claim_field(field)
+
+        # self.add(new_fields, finalize=False)
+        return new_fields
```

### Comparing `runtimepy-4.2.0/runtimepy/primitives/float.py` & `runtimepy-4.2.1/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/int.py` & `runtimepy-4.2.1/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/scaling.py` & `runtimepy-4.2.1/runtimepy/primitives/scaling.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/serializable/base.py` & `runtimepy-4.2.1/runtimepy/primitives/serializable/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/serializable/fixed.py` & `runtimepy-4.2.1/runtimepy/primitives/serializable/fixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/serializable/prefixed.py` & `runtimepy-4.2.1/runtimepy/primitives/serializable/prefixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/string.py` & `runtimepy-4.2.1/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/types/__init__.py` & `runtimepy-4.2.1/runtimepy/primitives/types/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/types/base.py` & `runtimepy-4.2.1/runtimepy/primitives/types/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/types/bool.py` & `runtimepy-4.2.1/runtimepy/primitives/types/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/types/bounds.py` & `runtimepy-4.2.1/runtimepy/primitives/types/bounds.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/types/float.py` & `runtimepy-4.2.1/runtimepy/primitives/types/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/primitives/types/int.py` & `runtimepy-4.2.1/runtimepy/primitives/types/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/registry/__init__.py` & `runtimepy-4.2.1/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/registry/bool.py` & `runtimepy-4.2.1/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/registry/item.py` & `runtimepy-4.2.1/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/registry/name.py` & `runtimepy-4.2.1/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/sample/peer.py` & `runtimepy-4.2.1/runtimepy/sample/peer.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/sample/program.py` & `runtimepy-4.2.1/runtimepy/sample/program.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/schemas.py` & `runtimepy-4.2.1/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/struct/__init__.py` & `runtimepy-4.2.1/runtimepy/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/subprocess/__init__.py` & `runtimepy-4.2.1/runtimepy/subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/subprocess/interface.py` & `runtimepy-4.2.1/runtimepy/subprocess/interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -175,22 +175,24 @@
         if data:
             count = len(data)
             self.stderr_metrics.increment(count)
 
             # Parse channel events.
             if self.peer is not None:
                 with BytesIO(data) as stream:
-                    for event in self.peer.env.channels.parse_event_stream(
-                        stream
-                    ):
+                    for event in self.peer.env.parse_event_stream(stream):
                         self.peer.env.ingest(event)
             else:
                 self.logger.warning("Dropped %d bytes of telemetry.", count)
 
     async def handle_stdout(self, data: bytes) -> None:
         """Handle messages from stdout."""
 
         if data:
             self.stdout_metrics.increment(len(data))
 
             for msg in self.processor.messages(data):
                 await self.process_json(msg)
+
+    async def poll_handler(self) -> None:
+        """Handle a 'poll' message."""
+        self.struct.poll()
```

### Comparing `runtimepy-4.2.0/runtimepy/subprocess/peer.py` & `runtimepy-4.2.1/runtimepy/subprocess/peer.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
                 elif task.done():
                     task = None
 
                 keep_going = await self.service_queues()
 
                 if keep_going:
                     await asyncio.sleep(self.poll_period_s)
-                    self.poll_metrics()
 
             except asyncio.CancelledError:
                 keep_going = False
 
     @asynccontextmanager
     async def _context(self: T) -> AsyncIterator[T]:
         """A managed context for the peer."""
```

### Comparing `runtimepy-4.2.0/runtimepy/subprocess/program.py` & `runtimepy-4.2.1/runtimepy/subprocess/program.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     struct_type: Type[RuntimeStruct] = SampleStruct
 
     @contextmanager
     def streaming_events(self) -> Iterator[None]:
         """Stream events to the stream output."""
 
-        with self.struct.env.channels.registered(
+        with self.struct.env.registered(
             self.stream_output, flush=True, channel=self.stream_metrics
         ):
             yield
 
     def write(self, data: bytes, addr: tuple[str, int] = None) -> None:
         """Write data."""
 
@@ -177,7 +177,13 @@
 
         # Don't respond to keyboard interrupt.
         signal.signal(signal.SIGINT, signal.SIG_IGN)
 
         async with cls.running(name, config, argv) as (io_task, main_task, _):
             await main_task
             await io_task
+
+    async def poll_handler(self) -> None:
+        """Handle a 'poll' message."""
+
+        self.struct.poll()
+        self.poll_metrics()
```

### Comparing `runtimepy-4.2.0/runtimepy/subprocess/protocol.py` & `runtimepy-4.2.1/runtimepy/subprocess/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/task/asynchronous.py` & `runtimepy-4.2.1/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/task/basic/manager.py` & `runtimepy-4.2.1/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/task/basic/periodic.py` & `runtimepy-4.2.1/runtimepy/task/basic/periodic.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/task/sample.py` & `runtimepy-4.2.1/runtimepy/task/sample.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,7 +42,36 @@
         return True
 
 
 class Sample(TaskFactory[SampleTask]):
     """A TUI application factory."""
 
     kind = SampleTask
+
+
+class SampleAppTask(ArbiterTask):
+    """A base TUI application."""
+
+    app: AppInfo
+
+    async def init(self, app: AppInfo) -> None:
+        """Initialize this task with application information."""
+        self.app = app
+
+    async def dispatch(self) -> bool:
+        """Dispatch an iteration of this task."""
+
+        for name, struct in self.app.structs.items():
+            if "struct" in name:
+                struct.poll()
+
+        # Send poll message to peer process.
+        for peer in self.app.peers.values():
+            peer.send_json({"poll": {"loopback": 1}})
+
+        return True
+
+
+class SampleApp(TaskFactory[SampleAppTask]):
+    """A TUI application factory."""
+
+    kind = SampleAppTask
```

### Comparing `runtimepy-4.2.0/runtimepy/task/trig/__init__.py` & `runtimepy-4.2.1/runtimepy/task/trig/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/tui/channels/__init__.py` & `runtimepy-4.2.1/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/tui/cursor.py` & `runtimepy-4.2.1/runtimepy/tui/cursor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/tui/mixin.py` & `runtimepy-4.2.1/runtimepy/tui/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/tui/mock.py` & `runtimepy-4.2.1/runtimepy/tui/mock.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/tui/task.py` & `runtimepy-4.2.1/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/runtimepy/util.py` & `runtimepy-4.2.1/runtimepy/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A module implementing package utilities.
 """
 
 # built-in
 import logging
-from typing import NamedTuple
+import re
+from typing import Iterable, Iterator, NamedTuple
 
 # third-party
 from vcorelib.logging import DEFAULT_TIME_FORMAT
 
 
 class StrToBool(NamedTuple):
     """A container for results when converting strings to boolean."""
@@ -70,7 +71,34 @@
     """
 
     parts = module_path.split(".")
     assert len(parts) > 1, module_path
 
     item = parts.pop()
     return ".".join(parts), item
+
+
+def name_search(
+    names: Iterable[str], pattern: str, exact: bool = False
+) -> Iterator[str]:
+    """A simple name searching method."""
+
+    compiled = re.compile(pattern)
+    for name in names:
+        if compiled.search(name) is not None:
+            if not exact or name == pattern:
+                yield name
+
+
+class Identifier:
+    """A simple message indentifier interface."""
+
+    def __init__(self) -> None:
+        """Initialize this instance."""
+        self.curr_id: int = 1
+        self.scale = 2
+
+    def __call__(self) -> int:
+        """Get the next identifier."""
+        curr = self.curr_id
+        self.curr_id += self.scale
+        return curr
```

### Comparing `runtimepy-4.2.0/runtimepy.egg-info/PKG-INFO` & `runtimepy-4.2.1/runtimepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.2.0
+Version: 4.2.1
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,17 +13,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: websockets
 Requires-Dist: vcorelib>=3.2.4
 Requires-Dist: svgen>=0.6.6
+Requires-Dist: websockets
 Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=e23f54e60d0c62ebc1be3cae63bc7678
+    hash=ebb5664a436fde952d2499fe582fccd3
     =====================================
 -->
 
-# runtimepy ([4.2.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.2.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.2.0/runtimepy.egg-info/SOURCES.txt` & `runtimepy-4.2.1/runtimepy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 runtimepy/channel/registry.py
 runtimepy/channel/environment/__init__.py
 runtimepy/channel/environment/array.py
 runtimepy/channel/environment/base.py
 runtimepy/channel/environment/create.py
 runtimepy/channel/environment/file.py
 runtimepy/channel/environment/sample.py
+runtimepy/channel/environment/telemetry.py
 runtimepy/channel/environment/command/__init__.py
 runtimepy/channel/environment/command/parser.py
 runtimepy/channel/environment/command/processor.py
 runtimepy/channel/environment/command/result.py
 runtimepy/channel/event/__init__.py
 runtimepy/channel/event/header.py
 runtimepy/codec/__init__.py
```

### Comparing `runtimepy-4.2.0/setup.py` & `runtimepy-4.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/tests/test_entry.py` & `runtimepy-4.2.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.2.0/tests/test_mapping.py` & `runtimepy-4.2.1/tests/test_mapping.py`

 * *Files identical despite different names*

