# Comparing `tmp/tradedangerous-11.0.0.tar.gz` & `tmp/tradedangerous-11.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradedangerous-11.0.0.tar", last modified: Wed Apr 24 19:04:38 2024, max compression
+gzip compressed data, was "tradedangerous-11.0.1.tar", last modified: Wed Apr 24 20:34:24 2024, max compression
```

## Comparing `tradedangerous-11.0.0.tar` & `tradedangerous-11.0.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.681871 tradedangerous-11.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_bootstrap_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_bootstrap_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_peek.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_trade_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.689871 tradedangerous-11.0.0/tradedangerous/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35958 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.693871 tradedangerous-11.0.0/tradedangerous/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/TEMPLATE.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/buildcache_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/buy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/commandenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/export_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/import_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/local_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/market_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/nav_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/olddata_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/rares_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/sell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/shipvendor_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/station_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/trade_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/update_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/csvexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/edscupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/edsmupdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/jsonprices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.693871 tradedangerous-11.0.0/tradedangerous/mfd/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mfd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.693871 tradedangerous-11.0.0/tradedangerous/mfd/saitek/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mfd/saitek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mfd/saitek/directoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mfd/saitek/x52pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/tradedangerous/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/checkpricebounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/coord64.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/derp-sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/diff-system-csvs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/eddb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/eddn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/edsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/edsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/importeddbstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/prices-json-exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/tradedangerous/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/edapi_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/edcd_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/eddblink_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/edmc_batch_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/journal_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/netlog_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26734 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/spansh_plug.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/prices.py
--rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/submit-distances.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/tradedangerous/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/templates/Added.csv
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/templates/Category.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/templates/RareItem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/templates/TradeDangerous.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/trade.py
--rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradecalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradeenv.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradeexcept.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradegui.py
--rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 19:03:53.000000 tradedangerous-11.0.0/tradedangerous/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/tradedangerous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.342886 tradedangerous-11.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-24 20:34:24.342886 tradedangerous-11.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 20:34:24.342886 tradedangerous-11.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.326886 tradedangerous-11.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.330886 tradedangerous-11.0.1/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36028 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.334886 tradedangerous-11.0.1/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-24 20:29:09.000000 tradedangerous-11.0.1/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.334886 tradedangerous-11.0.1/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.334886 tradedangerous-11.0.1/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.338886 tradedangerous-11.0.1/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.338886 tradedangerous-11.0.1/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21965 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26734 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.338886 tradedangerous-11.0.1/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/tradegui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-24 20:29:10.000000 tradedangerous-11.0.1/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 20:29:33.000000 tradedangerous-11.0.1/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:24.338886 tradedangerous-11.0.1/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-24 20:34:24.000000 tradedangerous-11.0.1/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 20:34:24.000000 tradedangerous-11.0.1/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:34:24.000000 tradedangerous-11.0.1/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 20:34:24.000000 tradedangerous-11.0.1/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:34:24.000000 tradedangerous-11.0.1/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 20:34:24.000000 tradedangerous-11.0.1/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 20:34:24.000000 tradedangerous-11.0.1/tradedangerous.egg-info/top_level.txt
```

### Comparing `tradedangerous-11.0.0/LICENSE` & `tradedangerous-11.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/PKG-INFO` & `tradedangerous-11.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.0.0
+Version: 11.0.1
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.0.0/README.md` & `tradedangerous-11.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/setup.py` & `tradedangerous-11.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_bootstrap_commands.py` & `tradedangerous-11.0.1/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_bootstrap_plugins.py` & `tradedangerous-11.0.1/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_cache.py` & `tradedangerous-11.0.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_commands.py` & `tradedangerous-11.0.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_fs.py` & `tradedangerous-11.0.1/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_peek.py` & `tradedangerous-11.0.1/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_trade.py` & `tradedangerous-11.0.1/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_trade_run.py` & `tradedangerous-11.0.1/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tests/test_utils.py` & `tradedangerous-11.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/__init__.py` & `tradedangerous-11.0.1/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/cache.py` & `tradedangerous-11.0.1/tradedangerous/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,31 +81,32 @@
 |   -               # alias for 0L0
 |   \d+[\?LMH]      # Or <number><level> where level is L(ow), M(ed) or H(igh)
 |   0               # alias for n/a
 |   bug
 """
 newItemPriceRe = re.compile(r"""
 ^
-    {itemPriceFrag}
+    {base_f}
     (
     \s+
         # demand units and level
-        (?P<demand> {qtyLevelFrag})
+        (?P<demand> {qtylvl_f})
     \s+
         # supply units and level
-        (?P<supply> {qtyLevelFrag})
+        (?P<supply> {qtylvl_f})
         # time is optional
         (?:
         \s+
-            {timeFrag}
+            {time_f}
         )?
     )?
 \s*
 $
-""", re.IGNORECASE + re.VERBOSE)
+""".format(base_f = itemPriceFrag, qtylvl_f = qtyLevelFrag, time_f = timeFrag),
+            re.IGNORECASE + re.VERBOSE)
 
 ######################################################################
 # Exception classes
 
 
 class BuildCacheBaseException(TradeException):
     """
```

### Comparing `tradedangerous-11.0.0/tradedangerous/cli.py` & `tradedangerous-11.0.1/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.0.1/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/__init__.py` & `tradedangerous-11.0.1/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/commandenv.py` & `tradedangerous-11.0.1/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/exceptions.py` & `tradedangerous-11.0.1/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/parsing.py` & `tradedangerous-11.0.1/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.0.1/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/commands/update_gui.py` & `tradedangerous-11.0.1/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/corrections.py` & `tradedangerous-11.0.1/tradedangerous/corrections.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/csvexport.py` & `tradedangerous-11.0.1/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/edscupdate.py` & `tradedangerous-11.0.1/tradedangerous/edscupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/edsmupdate.py` & `tradedangerous-11.0.1/tradedangerous/edsmupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/formatting.py` & `tradedangerous-11.0.1/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/fs.py` & `tradedangerous-11.0.1/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/gui.py` & `tradedangerous-11.0.1/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/jsonprices.py` & `tradedangerous-11.0.1/tradedangerous/jsonprices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/mapping.py` & `tradedangerous-11.0.1/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/mfd/__init__.py` & `tradedangerous-11.0.1/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.0.1/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.0.1/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.0.1/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/clipboard.py` & `tradedangerous-11.0.1/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/coord64.py` & `tradedangerous-11.0.1/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.0.1/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.0.1/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/eddb.py` & `tradedangerous-11.0.1/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/eddn.py` & `tradedangerous-11.0.1/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/edsc.py` & `tradedangerous-11.0.1/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/edsm.py` & `tradedangerous-11.0.1/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.0.1/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.0.1/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/misc/progress.py` & `tradedangerous-11.0.1/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/plugins/__init__.py` & `tradedangerous-11.0.1/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.0.1/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.0.1/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-11.0.1/tradedangerous/plugins/eddblink_plug.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
         
         # Run 'listings' by default:
         # If no options, or if only 'force', and/or 'skipvend',
         # have been passed, enable 'listings'.
         default = True
         for option in self.options:
             # if not option in ('force', 'fallback', 'skipvend', 'progbar'):
-            if option not in ('force', 'skipvend', 'prices'):
+            if option not in ('force', 'skipvend'):
                 default = False
         if default:
             self.options["listings"] = True
         
         # We can probably safely assume that the plugin has never been run if
         # the prices file doesn't exist, since the plugin always generates it.
         if not (self.tdb.dataPath / Path("TradeDangerous.prices")).exists():
```

### Comparing `tradedangerous-11.0.0/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.0.1/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.0.1/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.0.1/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/plugins/spansh_plug.py` & `tradedangerous-11.0.1/tradedangerous/plugins/spansh_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/prices.py` & `tradedangerous-11.0.1/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/submit-distances.py` & `tradedangerous-11.0.1/tradedangerous/submit-distances.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/templates/Added.csv` & `tradedangerous-11.0.1/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.0.1/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.0.1/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/tools.py` & `tradedangerous-11.0.1/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/trade.py` & `tradedangerous-11.0.1/tradedangerous/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/tradecalc.py` & `tradedangerous-11.0.1/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/tradedb.py` & `tradedangerous-11.0.1/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/tradeenv.py` & `tradedangerous-11.0.1/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/tradegui.py` & `tradedangerous-11.0.1/tradedangerous/tradegui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/transfers.py` & `tradedangerous-11.0.1/tradedangerous/transfers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/utils.py` & `tradedangerous-11.0.1/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-11.0.0/tradedangerous/version.py` & `tradedangerous-11.0.1/tradedangerous/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '11.0.0'
+__version__ = '11.0.1'
```

### Comparing `tradedangerous-11.0.0/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.0.1/tradedangerous.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 11.0.0
+Version: 11.0.1
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-11.0.0/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-11.0.1/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

