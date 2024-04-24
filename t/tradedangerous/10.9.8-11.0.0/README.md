# Comparing `tmp/tradedangerous-10.9.8.tar.gz` & `tmp/tradedangerous-11.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tradedangerous-10.9.8.tar", last modified: Fri Feb  5 06:33:03 2021, max compression
+gzip compressed data, was "tradedangerous-11.0.0.tar", last modified: Wed Apr 24 19:04:38 2024, max compression
```

## Comparing `tradedangerous-10.9.8.tar` & `tradedangerous-11.0.0.tar`

### file list

```diff
@@ -1,165 +1,106 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     5447 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1675 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/source/tradedangerous.plugins.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     3350 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/source/tradedangerous.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/source/modules.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     4597 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/installation.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/index.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/develop.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      787 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)      554 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/about.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     4133 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    57370 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/CHANGES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/
--rw-rw-r--   0 travis    (2000) travis    (2000)    32951 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9923 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/transfers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1441 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/corrections.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42292 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tradecalc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)    94739 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/templates/DefaultShipIndex.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8079 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/templates/TradeDangerous.sql
--rw-rw-r--   0 travis    (2000) travis    (2000)      649 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/templates/Added.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    10483 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/templates/RareItem.csv
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14470 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/edcd_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13456 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/netlog_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4224 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/edmc_batch_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23696 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/journal_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7868 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53929 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/eddblink_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42275 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/edapi_plug.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4468 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/export_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5683 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/import_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7716 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/olddata_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8356 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/nav_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14583 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/update_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15742 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/station_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2332 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/buildcache_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3175 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/trade_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/TEMPLATE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3142 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12965 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/buy_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46327 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/run_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9097 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/commandenv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5896 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/parsing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9640 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8924 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/rares_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5458 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/market_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8242 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/local_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7600 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/sell_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23376 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/update_gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7023 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/shipvendor_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4302 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tradeenv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29878 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4727 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      368 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tradeexcept.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/misc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3459 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/edsm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14979 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/edsc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4942 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/prices-json-exp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1843 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/eddb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4929 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/diff-system-csvs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2066 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/coord64.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2127 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/progress.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1681 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/clipboard.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12156 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/eddn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/coord64.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8434 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/checkpricebounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      779 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/derp-sentinel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1785 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/importeddbstats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      859 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/badstations.pl
--rw-rw-r--   0 travis    (2000) travis    (2000)     7593 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/prices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2530 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/fs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7013 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/jsonprices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5186 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12395 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/submit-distances.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2021-02-05 06:32:56.000000 tradedangerous-10.9.8/tradedangerous/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/mfd/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3065 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mfd/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/mfd/saitek/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24748 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mfd/saitek/directoutput.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5912 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mfd/saitek/x52pro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mfd/saitek/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72639 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tradedb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4034 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mapping.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8713 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/csvexport.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1122 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17338 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/edscupdate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14925 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/edsmupdate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6162 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/formatting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    50878 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerouscrest.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)     3324 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/fix-indent.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      406 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/.gitignore
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      961 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/config.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)    10480 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/td-completion.bash
--rwxrwxr-x   0 travis    (2000) travis    (2000)      561 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdrun
--rw-rw-r--   0 travis    (2000) travis    (2000)      338 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/WINDOWS.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)      427 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdbuyfrom
--rw-rw-r--   0 travis    (2000) travis    (2000)    12583 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/getstation.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)     9101 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/README.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2978 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tradebrute.bat
--rwxrwxr-x   0 travis    (2000) travis    (2000)      217 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdupd
--rwxrwxr-x   0 travis    (2000) travis    (2000)      441 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdloc
--rwxrwxr-x   0 travis    (2000) travis    (2000)      202 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdimad
--rw-rw-r--   0 travis    (2000) travis    (2000)     2305 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/trade.bat
--rwxrwxr-x   0 travis    (2000) travis    (2000)      212 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdnav
--rw-rw-r--   0 travis    (2000) travis    (2000)      288 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/TradeDangerous.sln
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/requirements/publish.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/requirements/dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      778 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    16725 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     4409 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/TradeDangerous.pyproj
--rw-rw-r--   0 travis    (2000) travis    (2000)     1542 2021-02-05 06:32:56.000000 tradedangerous-10.9.8/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tests/fixtures/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9026 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Item.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/FDevShipyard.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/ShipVendor.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    42224 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Upgrade.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/UpgradeVendor.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Ship.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     6493 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/System.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/FDevOutfitting.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      757 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Added.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/RareItem.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Category.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    42743 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Station.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  1787951 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/StationItem.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  4416512 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/TradeDangerous.db
--rw-rw-r--   0 travis    (2000) travis    (2000)      211 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_commands.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1107 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2575 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_trade_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1866 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_trade_import_eddblink.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3568 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_bootstrap_commands.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_bootstrap_plugins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3487 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_peek.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_fs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      842 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.681871 tradedangerous-11.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_bootstrap_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_bootstrap_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_peek.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_trade_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.689871 tradedangerous-11.0.0/tradedangerous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35958 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.693871 tradedangerous-11.0.0/tradedangerous/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/TEMPLATE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/buildcache_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/buy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/commandenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/export_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/import_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/local_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/market_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/nav_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/olddata_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/rares_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47650 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/sell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/shipvendor_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16219 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/station_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/trade_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/commands/update_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/csvexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/edscupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/edsmupdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43676 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/jsonprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.693871 tradedangerous-11.0.0/tradedangerous/mfd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mfd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.693871 tradedangerous-11.0.0/tradedangerous/mfd/saitek/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mfd/saitek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mfd/saitek/directoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/mfd/saitek/x52pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/tradedangerous/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/checkpricebounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/coord64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/derp-sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/diff-system-csvs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/eddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/eddn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/edsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/edsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/importeddbstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/prices-json-exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/misc/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/tradedangerous/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42262 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/edapi_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/edcd_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/eddblink_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/edmc_batch_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/journal_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/netlog_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26734 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/plugins/spansh_plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/submit-distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/tradedangerous/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/templates/Added.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/templates/Category.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/templates/RareItem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/templates/TradeDangerous.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42075 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradecalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72220 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradeenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradeexcept.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/tradegui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-24 19:03:29.000000 tradedangerous-11.0.0/tradedangerous/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 19:03:53.000000 tradedangerous-11.0.0/tradedangerous/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:04:38.697871 tradedangerous-11.0.0/tradedangerous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 19:04:38.000000 tradedangerous-11.0.0/tradedangerous.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tradedangerous-10.9.8/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-11.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 10.9.8
+Version: 11.0.0
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
 Project-URL: Source Code, https://github.com/eyeonus/Trade-Dangerous
-Description: 
-        ----------
-        
-        TradeDangerous  
-        Copyright (C) Oliver "kfsone" Smith, July 2014  
-        Copyright (C) Bernd 'Gazelle' Gollesch 2016, 2017  
-        Copyright (C) Jonathan 'eyeonus' Jones 2018, 2019
-        
-        REQUIRES PYTHON 3.4 OR HIGHER.
-        
-        ----------
-        
-        # What is Trade Dangerous? <img align="right" src="https://raw.githubusercontent.com/wiki/eyeonus/Trade-Dangerous/TradeDangerousCrest.png" alt="Trade Dangerous Crest">
-        
-        TradeDangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
-        
-        The TRO is a heavy hitter that can calculate complex routes with multiple stops while taking into account the profits you make along the route 
-        
-        The price data in TradeDangerous is either manually entered or crowd sourced from a website such as [Tromador's Trading Dangerously](http://elite.tromador.com/ "Tromador's Trading Dangerously"), often using a plugin such as the included eddblink.
-        
-        # What can it do for me?
-        
-        You're in a ship with 8 cargo spaces that can make 8.56 ly per jump; you're willing to make upto 2 jumps between stations, and we want to see how much money we can make if in 2 trade stops (hops).
-        
-            trade.py run --credits 5000 --capacity 8 --ly-per 8.56 --jumps 2 --hops 2
-        
-        If we ran this, TD would search the galaxy for trade runs. But it could take us days to reach some of them. So lets say we're currently at Kummer City in the Andere system.
-        
-            trade.py run --from "andere/kummer city"
-                --credits 5000 --capacity 8 --ly-per 8.56 --jumps 2 --hops 2
-        
-        (The above represents a single line)
-        
-        That's a lot to type. TD is designed to support laziness when it comes to typing, so it allows for all kinds of short-cuts.
-        
-            trade.py ru
-                --fr and/kumm     find a station matching 'kumm' in a
-                                  system matching 'and'
-                --cr 5k           'k', 'm' and 'b' are recognized suffixes
-                --cap 8           8 units of cargo
-                --ly 8.56         maximum distance *per jump*
-                --ju 2            maximum 2 jumps
-        
-        The default for hops is 2, so I didn't have to include it.
-        
-        You can also use "=" to connect an option with its values:
-        
-            trade.py ru --fr=and/kumm --cr=5k --cap=8 --ly=8.56 --ju=2
-        
-        With the data at the time I write this, this produces:
-        
-            ANDERE/Kummer City -> ANDERE/Malzberg Vision
-              ANDERE/Kummer City: 6 x Titanium, 2 x Polymers,
-              G 224-46/Lorrah Dock: 7 x Coltan, 1 x Lepidolite,
-              ANDERE/Malzberg Vision +8,032cr (502/ton)
-        
-        This tells us our overall route (line #1), what load to pick up from the first station, what to sell it for and pick up at the second stop and where to finish and unload for our final profit.
-        
-        Note that it could have just told us to pick up 6 Titanium (the max we could afford) or 8 Copper (the highest profit we could fill up with), Instead, TD crunched hard numbers and maximized the earnings of every cargo space AND credit.
-        
-        If you want to give Trade Dangerous a try, look no further than the [Setup Guide](https://github.com/eyeonus/Trade-Dangerous/wiki/Setup-Guide "Setup Guide") and the [User Guide](https://github.com/eyeonus/Trade-Dangerous/wiki/User-Guide "User Guide").
-        
-        Curious about programming with Trade Dangerous/Python? Take the [Python Quick Peek](https://github.com/eyeonus/Trade-Dangerous/wiki/Python-Quick-Peek "Python Quick Peek").
-        
 Keywords: trade,elite,elite-dangerous
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: appJar
+Requires-Dist: ijson
+Requires-Dist: rich
+
+
+----------
+
+TradeDangerous  
+Copyright (C) Oliver "kfsone" Smith, July 2014  
+Copyright (C) Bernd 'Gazelle' Gollesch 2016, 2017  
+Copyright (C) Jonathan 'eyeonus' Jones 2018 - 2021
+
+REQUIRES PYTHON 3.4 OR HIGHER.
+
+----------
+
+# What is Trade Dangerous? <img align="right" src="https://raw.githubusercontent.com/wiki/eyeonus/Trade-Dangerous/TradeDangerousCrest.png" alt="Trade Dangerous Crest">
+
+TradeDangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
+
+The TRO is a heavy hitter that can calculate complex routes with multiple stops while taking into account the profits you make along the route 
+
+The price data in TradeDangerous is either manually entered or crowd sourced from a website such as [Tromador's Trading Dangerously](http://elite.tromador.com/ "Tromador's Trading Dangerously"), often using a plugin such as the included eddblink.
+
+# What can it do for me?
+
+You're in a ship with 8 cargo spaces that can make 8.56 ly per jump; you're willing to make upto 2 jumps between stations, and we want to see how much money we can make if in 2 trade stops (hops).
+
+    trade.py run --credits 5000 --capacity 8 --ly-per 8.56 --jumps 2 --hops 2
+
+If we ran this, TD would search the galaxy for trade runs. But it could take us days to reach some of them. So lets say we're currently at Kummer City in the Andere system.
+
+    trade.py run --from "andere/kummer city"
+        --credits 5000 --capacity 8 --ly-per 8.56 --jumps 2 --hops 2
+
+(The above represents a single line)
+
+That's a lot to type. TD is designed to support laziness when it comes to typing, so it allows for all kinds of short-cuts.
+
+    trade.py ru
+        --fr and/kumm     find a station matching 'kumm' in a
+                          system matching 'and'
+        --cr 5k           'k', 'm' and 'b' are recognized suffixes
+        --cap 8           8 units of cargo
+        --ly 8.56         maximum distance *per jump*
+        --ju 2            maximum 2 jumps
+
+The default for hops is 2, so I didn't have to include it.
+
+You can also use "=" to connect an option with its values:
+
+    trade.py ru --fr=and/kumm --cr=5k --cap=8 --ly=8.56 --ju=2
+
+With the data at the time I write this, this produces:
+
+    ANDERE/Kummer City -> ANDERE/Malzberg Vision
+      ANDERE/Kummer City: 6 x Titanium, 2 x Polymers,
+      G 224-46/Lorrah Dock: 7 x Coltan, 1 x Lepidolite,
+      ANDERE/Malzberg Vision +8,032cr (502/ton)
+
+This tells us our overall route (line #1), what load to pick up from the first station, what to sell it for and pick up at the second stop and where to finish and unload for our final profit.
+
+Note that it could have just told us to pick up 6 Titanium (the max we could afford) or 8 Copper (the highest profit we could fill up with), Instead, TD crunched hard numbers and maximized the earnings of every cargo space AND credit.
+
+If you want to give Trade Dangerous a try, look no further than the [Setup Guide](https://github.com/eyeonus/Trade-Dangerous/wiki/Setup-Guide "Setup Guide") and the [User Guide](https://github.com/eyeonus/Trade-Dangerous/wiki/User-Guide "User Guide").
+
+Curious about programming with Trade Dangerous/Python? Take the [Python Quick Peek](https://github.com/eyeonus/Trade-Dangerous/wiki/Python-Quick-Peek "Python Quick Peek").
```

### Comparing `tradedangerous-10.9.8/tradedangerous/cache.py` & `tradedangerous-11.0.0/tradedangerous/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,26 +16,35 @@
 #   data/TradeDangerous.prices contains a description of the price
 #   database that is intended to be easily editable and commitable to
 #   a source repository.
 #
 #  TODO: Split prices into per-system or per-station files so that
 #  we can tell how old data for a specific system is.
 
-from collections import namedtuple
-from pathlib import Path
-from .tradeexcept import TradeException
+from __future__ import annotations
 
-from . import corrections, utils
+from pathlib import Path
 import csv
-import math
 import os
-from . import prices
 import re
 import sqlite3
 import sys
+import typing
+
+from .tradeexcept import TradeException
+from . import corrections, utils
+from . import prices
+
+
+# For mypy/pylint type checking
+if typing.TYPE_CHECKING:
+    from typing import Any, Optional, TextIO
+    
+    from .tradeenv import TradeEnv
+
 
 ######################################################################
 # Regular expression patterns. Here be draegons.
 # If you add new patterns:
 # - use fragments and re.VERBOSE (see itemPriceRe)
 # - use named captures (?P<name> ...)
 # - include comments
@@ -72,243 +81,284 @@
 |   -               # alias for 0L0
 |   \d+[\?LMH]      # Or <number><level> where level is L(ow), M(ed) or H(igh)
 |   0               # alias for n/a
 |   bug
 """
 newItemPriceRe = re.compile(r"""
 ^
-    {base_f}
+    {itemPriceFrag}
     (
     \s+
         # demand units and level
-        (?P<demand> {qtylvl_f})
+        (?P<demand> {qtyLevelFrag})
     \s+
         # supply units and level
-        (?P<supply> {qtylvl_f})
+        (?P<supply> {qtyLevelFrag})
         # time is optional
         (?:
         \s+
-            {time_f}
+            {timeFrag}
         )?
     )?
 \s*
 $
-""".format(base_f = itemPriceFrag, qtylvl_f = qtyLevelFrag, time_f = timeFrag),
-            re.IGNORECASE + re.VERBOSE)
+""", re.IGNORECASE + re.VERBOSE)
 
 ######################################################################
 # Exception classes
 
 
 class BuildCacheBaseException(TradeException):
     """
     Baseclass for BuildCache exceptions
     Attributes:
         fileName    Name of file being processedStations
         lineNo      Line the error occurred on
         error       Description of the error
     """
     
-    def __init__(self, fromFile, lineNo, error = None):
+    def __init__(self, fromFile: Path, lineNo: int, error: str = None) -> None:
         self.fileName = fromFile.name
         self.lineNo = lineNo
         self.category = "ERROR"
         self.error = error or "UNKNOWN ERROR"
     
-    def __str__(self):
-        return "{}:{} {} {}".format(
-                self.fileName, self.lineNo,
-                self.category,
-                self.error,
-        )
+    def __str__(self) -> str:
+        return f'{self.fileName}:{self.lineNo} {self.category} {self.error}'
 
 
 class UnknownSystemError(BuildCacheBaseException):
     """
     Raised when the file contains an unknown star name.
     """
     
-    def __init__(self, fromFile, lineNo, key):
-        error = 'Unrecognized SYSTEM: "{}"'.format(key)
-        super().__init__(fromFile, lineNo, error)
+    def __init__(self, fromFile: Path, lineNo: int, key: str) -> None:
+        super().__init__(fromFile, lineNo, f'Unrecognized SYSTEM: "{key}"')
 
 
 class UnknownStationError(BuildCacheBaseException):
     """
     Raised when the file contains an unknown star/station name.
     """
     
-    def __init__(self, fromFile, lineNo, key):
-        error = 'Unrecognized STAR/Station: "{}"'.format(key)
-        super().__init__(fromFile, lineNo, error)
+    def __init__(self, fromFile: Path, lineNo: int, key: str) -> None:
+        super().__init__(fromFile, lineNo, f'Unrecognized STAR/Station: "{key}"')
 
 
 class UnknownItemError(BuildCacheBaseException):
     """
     Raised in the case of an item name that we don't know.
     Attributes:
         itemName   Key we tried to look up.
     """
     
-    def __init__(self, fromFile, lineNo, itemName):
-        error = 'Unrecognized item name: "{}"'.format(itemName)
-        super().__init__(fromFile, lineNo, error)
+    def __init__(self, fromFile: Path, lineNo: int, itemName: str) -> None:
+        super().__init__(fromFile, lineNo, f'Unrecognized item name: "{itemName}"')
 
 
 class DuplicateKeyError(BuildCacheBaseException):
     """
         Raised when an item is being redefined.
     """
     
-    def __init__(self, fromFile, lineNo, keyType, keyValue, prevLineNo):
+    def __init__(self, fromFile: Path, lineNo: int, keyType: str, keyValue: str, prevLineNo: int) -> None:
         super().__init__(fromFile, lineNo,
-                "Second occurrance of {keytype} \"{keyval}\", "
-                "previous entry at line {prev}.".format(
-                    keytype = keyType,
-                    keyval = keyValue,
-                    prev = prevLineNo
-                ))
+                         f'Second occurrance of {keyType} "{keyValue}", previous entry at line {prevLineNo}.')
 
 
 class DeletedKeyError(BuildCacheBaseException):
     """
     Raised when a key value in a .csv file is marked as DELETED in the
     corrections file.
     """
     
-    def __init__(self, fromFile, lineNo, keyType, keyValue):
-        super().__init__(fromFile, lineNo,
-                "{} '{}' is marked as DELETED and should not be used.".format(
-                    keyType, keyValue
-        ))
+    def __init__(self, fromFile: Path, lineNo: int, keyType: str, keyValue: str) -> None:
+        super().__init__(
+            fromFile, lineNo,
+            f'{keyType} "{keyValue}" is marked as DELETED and should not be used.'
+        )
 
 
 class DeprecatedKeyError(BuildCacheBaseException):
     """
     Raised when a key value in a .csv file has a correction; the old
     name should not appear in the .csv file.
     """
     
-    def __init__(self, fromFile, lineNo, keyType, keyValue, newValue):
-        super().__init__(fromFile, lineNo,
-                "{} '{}' is deprecated "
-                "and should be replaced with '{}'.".format(
-                    keyType, keyValue, newValue
-        ))
+    def __init__(self, fromFile: Path, lineNo: int, keyType: str, keyValue: str, newValue: str) -> None:
+        super().__init__(
+            fromFile, lineNo,
+            f'{keyType} "{keyValue}" is deprecated and should be replaced with "{newValue}".'
+        )
 
 
 class MultipleStationEntriesError(DuplicateKeyError):
     """ Raised when a station appears multiple times in the same file. """
     
-    def __init__(self, fromFile, lineNo, facility, prevLineNo):
+    def __init__(self, fromFile: Path, lineNo: int, facility: str, prevLineNo: int) -> None:
         super().__init__(fromFile, lineNo, 'station', facility, prevLineNo)
 
 
 class MultipleItemEntriesError(DuplicateKeyError):
     """ Raised when one item appears multiple times in the same station. """
     
-    def __init__(self, fromFile, lineNo, item, prevLineNo):
+    def __init__(self, fromFile: Path, lineNo: int, item: str, prevLineNo: int) -> None:
         super().__init__(fromFile, lineNo, 'item', item, prevLineNo)
 
 
 class SyntaxError(BuildCacheBaseException):
     """
     Raised when an invalid line is read.
     Attributes:
         problem     The problem that occurred
         text        Offending text
     """
     
-    def __init__(self, fromFile, lineNo, problem, text):
-        error = "{},\ngot: '{}'.".format(problem, text.strip())
-        super().__init__(fromFile, lineNo, error)
+    def __init__(self, fromFile: Path, lineNo: int, problem: str, text: str) -> None:
+        super().__init__(fromFile, lineNo, f'{problem},\ngot: "{text.strip()}".')
 
 
 class SupplyError(BuildCacheBaseException):
     """
     Raised when a supply field is incorrectly formatted.
     """
     
-    def __init__(self, fromFile, lineNo, category, problem, value):
-        error = "Invalid {} supply value: {}. Got: {}". \
-                    format(category, problem, value)
-        super().__init__(fromFile, lineNo, error)
+    def __init__(self, fromFile: Path, lineNo: int, category: str, problem: str, value: Any) -> None:
+        super().__init__(fromFile, lineNo, f'Invalid {category} supply value: {problem}. Got: {value}')
+
 
 ######################################################################
 # Helpers
 
 
-def parseSupply(pricesFile, lineNo, category, reading):
+# supply/demand levels are one of '?' for unknown, 'L', 'M' or 'H'
+# for low, medium, or high. We turn these into integer values for
+# ordering convenience, and we include both upper and lower-case
+# so we don't have to sweat ordering.
+#
+SUPPLY_LEVEL_VALUES = {
+    '?':   -1,
+    'L':    1,      'l':    1,
+    'M':    2,      'm':    2,
+    'H':    3,      'h':    3,
+}
+
+
+def parseSupply(pricesFile: Path, lineNo: int, category: str, reading: str) -> tuple[int, int]:
+    """ Parse a supply specifier which is expected to be in the <number><?, L, M, or H>, and
+        returns the units as an integer and a numeric level value suitable for ordering,
+        such that ? = -1, L/l = 0, M/m = 1, H/h = 2 """
+    
+    #   supply_level <- digit+ level;
+    #   digit <- [0-9];
+    #   level <- Unknown / Low / Medium / High;
+    #   Unknown <- '?';
+    #   Low <- 'L';
+    #   Medium <- 'M';
+    #   High <- 'H';
+    if reading == '?':
+        return -1, -1
+    elif reading == '-':
+        return 0, 0
+    
+    # extract the left most digits into unit and the last character into the level reading.
     units, level = reading[0:-1], reading[-1]
-    levelNo = "??LMH".find(level.upper()) - 1
-    if levelNo < -1:
+    
+    # Extract the right most character as the "level" and look up its numeric value.
+    levelNo = SUPPLY_LEVEL_VALUES.get(level)
+    if levelNo is None:
         raise SupplyError(
             pricesFile, lineNo, category, reading,
-            'Unrecognized level suffix: "{}": '
-            "expected one of 'L', 'M', 'H' or '?'".format(
-                level
-            )
+            f'Unrecognized level suffix: "{level}": expected one of "L", "M", "H" or "?"'
         )
+    
+    # Expecting a numeric value in units, e.g. 123? -> (units=123, level=?)
     try:
         unitsNo = int(units)
         if unitsNo < 0:
-            raise ValueError("unsigned unit count")
-        if unitsNo == 0:
-            return 0, 0
-        return unitsNo, levelNo
+            # Use the same code-path as if the units fail to parse.
+            raise ValueError('negative unit count')
     except ValueError:
-        pass
+        raise SupplyError(
+            pricesFile, lineNo, category, reading,
+            f'Unrecognized units/level value: "{level}": expected "-", "?", or a number followed by a level (L, M, H or ?).'
+        ) from None  # don't forward the exception itself
     
-    raise SupplyError(
-        pricesFile, lineNo, category, reading,
-        'Unrecognized units/level value: "{}": '
-        "expected '-', '?', or a number followed "
-        "by a level (L, M, H or ?).".format(
-            level
-        )
-    )
+    # Normalize the units and level when there are no units.
+    if unitsNo == 0:
+        return 0, 0
+    
+    return unitsNo, levelNo
+
 
 ######################################################################
 # Code
 ######################################################################
 
 
-def getSystemByNameIndex(cur):
+def getSystemByNameIndex(cur: sqlite3.Cursor) -> dict[str, int]:
     """ Build station index in STAR/Station notation """
     cur.execute("""
             SELECT system_id, UPPER(system.name)
               FROM System
         """)
     return { name: ID for (ID, name) in cur }
 
 
-def getStationByNameIndex(cur):
+def getStationByNameIndex(cur: sqlite3.Cursor) -> dict[str, int]:
     """ Build station index in STAR/Station notation """
     cur.execute("""
             SELECT station_id,
-                    UPPER(system.name) || '/' || UPPER(station.name)
+                    system.name || '/' || station.name
               FROM System
                    INNER JOIN Station
                       USING (system_id)
         """)
-    return { name: ID for (ID, name) in cur }
+    return { name.upper(): ID for (ID, name) in cur }
 
 
-def getItemByNameIndex(cur):
+def getItemByNameIndex(cur: sqlite3.Cursor) -> dict[str, int]:
     """
         Generate item name index.
     """
     cur.execute("SELECT item_id, UPPER(name) FROM item")
     return { name: itemID for (itemID, name) in cur }
 
 
-def processPrices(tdenv, priceFile, db, defaultZero):
+# The return type of process prices is complicated, should probably have been a type
+# in its own right. I'm going to define some aliases to try and persuade IDEs to be
+# more helpful about what it is trying to return.
+if typing.TYPE_CHECKING:
+    # A list of the IDs of stations that were modified so they can be updated
+    ProcessedStationIds= tuple[tuple[int]]
+    ProcessedItem = tuple[
+        int,                            # station ID
+        int,                            # item ID
+        Optional[int | float |str],     # modified
+        int,                            # demandCR
+        int,                            # demandUnits
+        int,                            # demandLevel
+        int,                            # supplyCr
+        int,                            # supplyUnits
+        int,                            # supplyLevel
+    ]
+    ProcessedItems = list[ProcessedItem]
+    ZeroItems = list[tuple[int, int]]   # stationID, itemID
+
+
+def processPrices(tdenv: TradeEnv, priceFile: Path, db: sqlite3.Connection, defaultZero: bool) -> tuple[ProcessedStationIds, ProcessedItems, ZeroItems, int, int, int, int]:
     """
         Yields SQL for populating the database with prices
         by reading the file handle for price lines.
+        
+        :param tdenv:       The environment we're working in
+        :param priceFile:   File to read
+        :param db:          SQLite3 database to write to
+        :param defaultZero: Whether to create default zero-availability/-demand records for data that's not present
+                            (if this is a partial update, you don't want this to be False)
     """
     
     DEBUG0, DEBUG1 = tdenv.DEBUG0, tdenv.DEBUG1
     DEBUG0("Processing prices file: {}", priceFile)
     
     cur = db.cursor()
     ignoreUnknown = tdenv.ignoreUnknown
@@ -336,83 +386,84 @@
     
     stationID = None
     facility = None
     processedStations = {}
     processedSystems = set()
     processedItems = {}
     stationItemDates = {}
-    itemPrefix = ""
     DELETED = corrections.DELETED
-    items, zeros, buys, sells = [], [], [], []
+    items, zeros = [], []
     
     lineNo, localAdd = 0, 0
     if not ignoreUnknown:
-        
-        def ignoreOrWarn(error):
+        def ignoreOrWarn(error: Exception) -> None:
             raise error
     
     elif not quiet:
         ignoreOrWarn = tdenv.WARN
     
-    def changeStation(matches):
+    def changeStation(matches: re.Match) -> None:
         nonlocal facility, stationID
         nonlocal processedStations, processedItems, localAdd
         nonlocal stationItemDates
         
         # ## Change current station
         stationItemDates = {}
         systemNameIn, stationNameIn = matches.group(1, 2)
         systemName, stationName = systemNameIn.upper(), stationNameIn.upper()
         corrected = False
-        facility = "/".join((systemName, stationName))
+        facility = f'{systemName}/{stationName}'
         
         # Make sure it's valid.
         stationID = DELETED
-        newID = stationByName.get(facility, -1)
+        newID = stationByName.get(facility, -1)  # why -1 and not None?
         DEBUG0("Selected station: {}, ID={}", facility, newID)
         if newID is DELETED:
             DEBUG1("DELETED Station: {}", facility)
             return
+        
         if newID < 0:
             if utils.checkForOcrDerp(tdenv, systemName, stationName):
                 return
             corrected = True
-            altName = sysCorrections.get(systemName, None)
+            altName = sysCorrections.get(systemName)
             if altName is DELETED:
                 DEBUG1("DELETED System: {}", facility)
                 return
             if altName:
                 DEBUG1("SYSTEM '{}' renamed '{}'", systemName, altName)
                 systemName, facility = altName, "/".join((altName, stationName))
             
-            systemID = systemByName.get(systemName, -1)
+            systemID = systemByName.get(systemName, -1)  # why -1 and not None?
             if systemID < 0:
                 ignoreOrWarn(
                     UnknownSystemError(priceFile, lineNo, facility)
                 )
                 return
             
-            altStation = stnCorrections.get(facility, None)
-            if altStation is DELETED:
-                DEBUG1("DELETED Station: {}", facility)
-                return
+            altStation = stnCorrections.get(facility)
             if altStation:
+                if altStation is DELETED:
+                    DEBUG1("DELETED Station: {}", facility)
+                    return
+                
                 DEBUG1("Station '{}' renamed '{}'", facility, altStation)
                 stationName = altStation.upper()
-                facility = "/".join((systemName, stationName))
+                facility = f'{systemName}/{stationName}'
             
             newID = stationByName.get(facility, -1)
             if newID is DELETED:
                 DEBUG1("Renamed station DELETED: {}", facility)
                 return
         
         if newID < 0:
             if not ignoreUnknown:
+                DEBUG0(f'Key value: "{list(stationByName.keys())[list(stationByName.values()).index(128893178)]}"')
                 ignoreOrWarn(
-                        UnknownStationError(priceFile, lineNo, facility)
+                    UnknownStationError(priceFile, lineNo, facility)
                 )
                 return
             name = utils.titleFixup(stationName)
             inscur = db.cursor()
             inscur.execute("""
                 INSERT INTO Station (
                     system_id, name,
@@ -425,16 +476,16 @@
                 ) VALUES (
                     ?, ?, 0, '?', '?', '?', '?',
                     DATETIME('now')
                 )
             """, [systemID, name])
             newID = inscur.lastrowid
             stationByName[facility] = newID
-            tdenv.NOTE("Added local station placeholder for {} (#{})",
-                    facility, newID
+            tdenv.NOTE(
+                "Added local station placeholder for {} (#{})", facility, newID
             )
             localAdd += 1
         elif newID in processedStations:
             # Check for duplicates
             if not corrected:
                 raise MultipleStationEntriesError(
                     priceFile, lineNo, facility,
@@ -447,15 +498,15 @@
         processedItems = {}
         
         cur = db.execute("""
             SELECT item_id, modified
               FROM StationItem
              WHERE station_id = ?
         """, [stationID])
-        stationItemDates = {ID: modified for ID, modified in cur}
+        stationItemDates = dict(cur)
     
     addItem, addZero = items.append, zeros.append
     getItemID = itemByName.get
     newItems, updtItems, ignItems = 0, 0, 0
     
     def processItemLine(matches):
         nonlocal newItems, updtItems, ignItems
@@ -491,15 +542,15 @@
                 return
         
         # Check for duplicate items within the station.
         if itemID in processedItems:
             ignoreOrWarn(
                 MultipleItemEntriesError(
                     priceFile, lineNo,
-                    "{}".format(itemName),
+                    f'{itemName}',
                     processedItems[itemID]
                 )
             )
             return
         
         demandCr, supplyCr = matches.group('sell', 'buy')
         demandCr, supplyCr = int(demandCr), int(supplyCr)
@@ -510,91 +561,74 @@
                 addZero((stationID, itemID))
         else:
             if lastModified:
                 updtItems += 1
             else:
                 newItems += 1
             if demandString:
-                if demandString == "?":
-                    demandUnits, demandLevel = -1, -1
-                elif demandString == "-":
-                    demandUnits, demandLevel = 0, 0
-                else:
-                    demandUnits, demandLevel = parseSupply(
-                        priceFile, lineNo, 'demand', demandString
-                    )
+                demandUnits, demandLevel = parseSupply(
+                    priceFile, lineNo, 'demand', demandString
+                )
             else:
                 demandUnits, demandLevel = defaultUnits, defaultLevel
             
             if demandString and supplyString:
-                if supplyString == "?":
-                    supplyUnits, supplyLevel = -1, -1
-                elif supplyString == "-":
-                    supplyUnits, supplyLevel = 0, 0
-                else:
-                    supplyUnits, supplyLevel = parseSupply(
-                        priceFile, lineNo, 'supply', supplyString
-                    )
+                supplyUnits, supplyLevel = parseSupply(
+                    priceFile, lineNo, 'supply', supplyString
+                )
             else:
                 supplyUnits, supplyLevel = defaultUnits, defaultLevel
             
             if modified == 'now':
                 modified = None  # Use CURRENT_FILESTAMP
             
             addItem((
                 stationID, itemID, modified,
                 demandCr, demandUnits, demandLevel,
                 supplyCr, supplyUnits, supplyLevel,
             ))
         
         processedItems[itemID] = lineNo
     
+    space_cleanup = re.compile(r'\s{2,}').sub
     for line in priceFile:
         lineNo += 1
-        text, _, comment = line.partition('#')
-        text = text.strip()
+        
+        text = line.split('#', 1)[0]                # Discard comments
+        text = space_cleanup(' ', text).strip()     # Remove leading/trailing whitespace, reduce multi-spaces
         if not text:
             continue
         
-        # replace whitespace with single spaces
-        if text.find("  "):
-            # http://stackoverflow.com/questions/2077897
-            text = ' '.join(text.split())
-        
         ########################################
         # ## "@ STAR/Station" lines.
         if text.startswith('@'):
             matches = systemStationRe.match(text)
             if not matches:
-                raise SyntaxError("Unrecognized '@' line: {}".format(# pylint: disable=no-value-for-parameter
-                            text
-                        ))
+                raise SyntaxError(priceFile, lineNo, "Unrecognized '@' line", text)
             changeStation(matches)
             continue
         
         if not stationID:
             # Need a station to process any other type of line.
-            raise SyntaxError(priceFile, lineNo,
-                                "Expecting '@ SYSTEM / Station' line", text)
+            raise SyntaxError(priceFile, lineNo, "Expecting '@ SYSTEM / Station' line", text)
         if stationID == DELETED:
             # Ignore all values from a deleted station/system.
             continue
         
         ########################################
         # ## "+ Category" lines
         if text.startswith('+'):
             # we now ignore these.
             continue
         
         ########################################
         # ## "Item sell buy ..." lines.
         matches = newItemPriceRe.match(text)
         if not matches:
-            raise SyntaxError(priceFile, lineNo,
-                        "Unrecognized line/syntax", text)
+            raise SyntaxError(priceFile, lineNo, "Unrecognized line/syntax", text)
         
         processItemLine(matches)
     
     numSys = len(processedSystems)
     
     if localAdd > 0:
         tdenv.NOTE(
@@ -603,21 +637,22 @@
             "Use 'trade.py export --table Station' "
             "if you /need/ to persist them."
         )
     
     stations = tuple((ID,) for ID in processedStations.keys())
     return stations, items, zeros, newItems, updtItems, ignItems, numSys
 
+
 ######################################################################
 
 
-def processPricesFile(tdenv, db, pricesPath, pricesFh = None, defaultZero = False):
+def processPricesFile(tdenv: TradeEnv, db: sqlite3.Connection, pricesPath: Path, pricesFh: Optional[TextIO] = None, defaultZero: bool = False) -> None:
     tdenv.DEBUG0("Processing Prices file '{}'", pricesPath)
     
-    with pricesFh or pricesPath.open('rU', encoding = 'utf-8') as pricesFh:
+    with pricesFh or pricesPath.open('r', encoding='utf-8') as pricesFh:
         stations, items, zeros, newItems, updtItems, ignItems, numSys = processPrices(
             tdenv, pricesFh, db, defaultZero
         )
     
     if not tdenv.mergeImport:
         db.executemany("""
             DELETE FROM StationItem
@@ -628,37 +663,55 @@
             DELETE FROM StationItem
              WHERE station_id = ?
                AND item_id = ?
         """, zeros)
     removedItems = len(zeros)
     
     if items:
-        db.executemany("""
-            INSERT OR REPLACE INTO StationItem (
-                station_id, item_id, modified,
-                demand_price, demand_units, demand_level,
-                supply_price, supply_units, supply_level
-            ) VALUES (
-                ?, ?, IFNULL(?, CURRENT_TIMESTAMP),
-                ?, ?, ?,
-                ?, ?, ?
-            )
-        """, items)
-    updatedItems = len(items)
+        for item in items:
+            try:
+                db.execute("""
+                    INSERT OR REPLACE INTO StationItem (
+                        station_id, item_id, modified,
+                        demand_price, demand_units, demand_level,
+                        supply_price, supply_units, supply_level
+                    ) VALUES (
+                        ?, ?, IFNULL(?, CURRENT_TIMESTAMP),
+                        ?, ?, ?,
+                        ?, ?, ?
+                    )
+                """, item)
+            except sqlite3.IntegrityError as e:
+                print(e)
+                print(item)
+                raise e
+        # db.executemany("""
+        #     INSERT OR REPLACE INTO StationItem (
+        #         station_id, item_id, modified,
+        #         demand_price, demand_units, demand_level,
+        #         supply_price, supply_units, supply_level
+        #     ) VALUES (
+        #         ?, ?, IFNULL(?, CURRENT_TIMESTAMP),
+        #         ?, ?, ?,
+        #         ?, ?, ?
+        #     )
+        # """, items)
     
     tdenv.DEBUG0("Marking populated stations as having a market")
     db.execute(
         "UPDATE Station SET market = 'Y'"
         " WHERE EXISTS"
             " (SELECT station_id FROM StationItem"
               " WHERE StationItem.station_id = Station.station_id"
              ")"
     )
     
+    tdenv.DEBUG0('Committing...')
     db.commit()
+    db.close()
     
     changes = " and ".join("{} {}".format(v, k) for k, v in {
         "new": newItems,
         "updated": updtItems,
         "removed": removedItems,
     }.items() if v) or "0"
     
@@ -671,14 +724,15 @@
                 len(stations),
                 numSys,
     )
     
     if ignItems:
         tdenv.NOTE("Ignored {} items with old data", ignItems)
 
+
 ######################################################################
 
 
 def depCheck(importPath, lineNo, depType, key, correctKey):
     if correctKey == key:
         return
     if correctKey == corrections.DELETED:
@@ -724,34 +778,35 @@
 
 def processImportFile(tdenv, db, importPath, tableName):
     tdenv.DEBUG0(
         "Processing import file '{}' for table '{}'",
         str(importPath), tableName
     )
     
-    fkeySelectStr = ("("
-            "SELECT {newValue}"
-            " FROM {table}"
-            " WHERE {stmt}"
-            ")"
+    fkeySelectStr = (
+        "("
+        " SELECT {newValue}"
+        " FROM {table}"
+        " WHERE {stmt}"
+        ")"
     )
     uniquePfx = "unq:"
     uniqueLen = len(uniquePfx)
     ignorePfx = "!"
     
-    with importPath.open('rU', encoding = 'utf-8') as importFile:
+    with importPath.open('r', encoding='utf-8') as importFile:
         csvin = csv.reader(
-            importFile, delimiter = ',', quotechar = "'", doublequote = True
+            importFile, delimiter=',', quotechar="'", doublequote=True
         )
         # first line must be the column names
         columnDefs = next(csvin)
         columnCount = len(columnDefs)
         
         # split up columns and values
-        # this is necessqary because the insert might use a foreign key
+        # this is necessary because the insert might use a foreign key
         bindColumns = []
         bindValues = []
         joinHelper = []
         uniqueIndexes = []
         for (cIndex, cName) in enumerate(columnDefs):
             colName, _, srcKey = cName.partition('@')
             # is this a unique index?
@@ -792,30 +847,30 @@
                     stmt = " AND ".join(joinStmt),
                 )
             )
         # now we can make the sql statement
         sql_stmt = """
             INSERT OR REPLACE INTO {table} ({columns}) VALUES({values})
         """.format(
-                table = tableName,
-                columns = ','.join(bindColumns),
-                values = ','.join(bindValues)
-            )
+            table=tableName,
+            columns=','.join(bindColumns),
+            values=','.join(bindValues)
+        )
         tdenv.DEBUG0("SQL-Statement: {}", sql_stmt)
         
         # Check if there is a deprecation check for this table.
         deprecationFn = getattr(
             sys.modules[__name__],
             "deprecationCheck" + tableName,
             None
         )
         
         # import the data
         importCount = 0
-        uniqueIndex = dict()
+        uniqueIndex = {}
         
         for linein in csvin:
             if not linein:
                 continue
             lineNo = csvin.line_num
             if len(linein) == columnCount:
                 tdenv.DEBUG1("       Values: {}", ', '.join(linein))
@@ -894,15 +949,15 @@
     We load both sets of data into an SQLite database, after which we can
     avoid the text-processing overhead by simply checking if the text files
     are newer than the database.
     """
     
     tdenv.NOTE(
         "Rebuilding cache file: this may take a few moments.",
-        file = sys.stderr
+        stderr=True,
     )
     
     dbPath = tdb.dbPath
     sqlPath = tdb.sqlPath
     pricesPath = tdb.pricesPath
     
     # Create an in-memory database to populate with our data.
@@ -912,15 +967,15 @@
     if tempPath.exists():
         tempPath.unlink()
     
     tempDB = sqlite3.connect(str(tempPath))
     tempDB.execute("PRAGMA foreign_keys=ON")
     # Read the SQL script so we are ready to populate structure, etc.
     tdenv.DEBUG0("Executing SQL Script '{}' from '{}'", sqlPath, os.getcwd())
-    with sqlPath.open('rU', encoding = 'utf-8') as sqlFile:
+    with sqlPath.open('r', encoding = 'utf-8') as sqlFile:
         sqlScript = sqlFile.read()
         tempDB.executescript(sqlScript)
     
     # import standard tables
     for (importName, importTable) in tdb.importTables:
         try:
             processImportFile(tdenv, tempDB, Path(importName), importTable)
@@ -938,19 +993,20 @@
     # Parse the prices file
     if pricesPath.exists():
         processPricesFile(tdenv, tempDB, pricesPath)
     else:
         tdenv.NOTE(
                 "Missing \"{}\" file - no price data.",
                     pricesPath,
-                    file = sys.stderr,
+                    stderr=True,
         )
     
     tempDB.commit()
     tempDB.close()
+    tdb.close()
     
     tdenv.DEBUG0("Swapping out db files")
     
     if dbPath.exists():
         if backupPath.exists():
             backupPath.unlink()
         dbPath.rename(backupPath)
@@ -996,12 +1052,12 @@
             db.commit()
     
     tdenv.DEBUG0("Importing data from {}".format(str(path)))
     processPricesFile(tdenv,
             db = tdb.getDB(),
             pricesPath = path,
             pricesFh = pricesFh,
-            )
+    )
     
     # If everything worked, we may need to re-build the prices file.
     if path != tdb.pricesPath:
         regeneratePricesFile(tdb, tdenv)
```

### Comparing `tradedangerous-10.9.8/tradedangerous/transfers.py` & `tradedangerous-11.0.0/tradedangerous/transfers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-from os import getcwd, path
 from collections import deque
 from pathlib import Path
 from .tradeexcept import TradeException
 
 import csv
 import json
-import math
 from .misc import progress as pbar
+import platform  # noqa: F401
 from . import fs
-import platform
 import time
 import subprocess
 import sys
 
 try:
     import requests
     __requests = requests
 except ImportError:
     __requests = None
 
 def import_requests():
     global __requests
-    global platform
     if __requests:
         return __requests
     
     if platform.system() == 'Linux':
         extra = (
             "Ubuntu users: You may be able to install 'pip'\n"
             "with 'apt-get install python3-pip' and requests with\n"
@@ -54,36 +50,34 @@
     )
     # Idiot-proofing: take just the first character in case the user typed
     # 'YES' (upper or lower case) instead of 'Y'.
     if approval[0:1].lower() != 'y':
         raise TradeException("Missing package: 'requests'")
     
     try:
-        import pip
+        import pip  # noqa: F401  # pylint: disable=unused-import
     except ImportError as e:
-        import platform
         raise TradeException(
             "Python 3.4.2 includes a package manager called 'pip', "
             "except it doesn't appear to be installed on your system:\n"
             "{}{}".format(str(e), extra)
         ) from None
     
     # Let's use "The most reliable approach, and the one that is fully supported."
     # Especially since the old way produces an error for me on Python 3.6:
     # "AttributeError: 'module' object has no attribute 'main'"
-    #pip.main(["install", "--upgrade", "requests"])
+    #  pip.main(["install", "--upgrade", "requests"])
     subprocess.check_call([sys.executable, '-m', 'pip', 'install', '--upgrade', 'requests'])
     
     try:
-        import requests
+        import requests  # pylint: disable=redefined-outer-name
         __requests = requests
     except ImportError as e:
         raise TradeException(
-            "The requests module did not install correctly.{}"
-            .format(extra)
+            f"The requests module did not install correctly ({e}).{extra}"
         ) from None
     
     return __requests
 
 ######################################################################
 # Helpers
 
@@ -105,14 +99,15 @@
 
 def download(
             tdenv, url, localFile,
             headers=None,
             backup=False,
             shebang=None,
             chunkSize=4096,
+            timeout=90,
         ):
     """
     Fetch data from a URL and save the output
     to a local file. Returns the response headers.
     
     tdenv:
         TradeEnv we're working under
@@ -126,17 +121,17 @@
     headers:
         dict() of additional HTTP headers to send
     
     shebang:
         function to call on the first line
     """
     
-    requests = import_requests()
+    requests = import_requests()  # pylint: disable=redefined-outer-name
     tdenv.NOTE("Requesting {}".format(url))
-    req = requests.get(url, headers=headers or None, stream=True)
+    req = requests.get(url, headers=headers or None, stream=True, timeout=timeout)
     req.raise_for_status()
     
     encoding = req.headers.get('content-encoding', 'uncompress')
     length = req.headers.get('content-length', None)
     transfer = req.headers.get('transfer-encoding', None)
     if transfer != 'chunked':
         # chunked transfer-encoding doesn't need a content-length
@@ -144,14 +139,22 @@
             print(req.headers)
             raise Exception("Remote server replied with invalid content-length.")
         length = int(length)
         if length <= 0:
             raise TradeException(
                 "Remote server gave an empty response. Please try again later."
             )
+
+    # if the file is being compressed by the server, the headers tell us the
+    # length of the compressed data, but in our loop below we will be receiving
+    # the uncompressed data, which should be larger, which will cause our
+    # download indicators to sit at 100% for a really long time if the file is
+    # heavily compressed and large (e.g spansh 1.5gb compressed vs 9GB uncompressed)
+    if encoding == "gzip" and length:
+        length *= 4
     
     if tdenv.detail > 1:
         if length:
             tdenv.NOTE("Downloading {} {}ed data", makeUnit(length), encoding)
         else:
             tdenv.NOTE("Downloading {} {}ed data", transfer, encoding)
     tdenv.DEBUG0(str(req.headers).replace("{", "{{").replace("}", "}}"))
@@ -224,23 +227,23 @@
     if actPath.exists():
         actPath.unlink()
     tmpPath.rename(actPath)
     
     req.close()
     return req.headers
 
-def get_json_data(url):
+def get_json_data(url, *, timeout: int = 90):
     """
     Fetch JSON data from a URL and return the resulting dictionary.
     
     Displays a progress bar as it downloads.
     """
     
-    requests = import_requests()
-    req = requests.get(url, stream=True)
+    requests = import_requests()  # pylint: disable=redefined-outer-name
+    req = requests.get(url, stream=True, timeout=timeout)
     
     totalLength = req.headers.get('content-length')
     if totalLength is None:
         compression = req.headers.get('content-encoding')
         compression = (compression + "'ed") if compression else "uncompressed"
         print("Downloading {}: {}...".format(compression, url))
         jsData = req.content
@@ -257,31 +260,31 @@
                     makeUnit(value),
                     makeUnit(goal),
             ))
         progBar.clear()
     
     return json.loads(jsData.decode())
 
-class CSVStream(object):
+class CSVStream:
     """
     Provides an iterator that fetches CSV data from a given URL
     and presents it as an iterable of (columns, values).
     
     Example:
         stream = transfers.CSVStream("http://blah.com/foo.csv")
         for cols, vals in stream:
             print("{} = {}".format(cols[0], vals[0]))
     """
     
-    def __init__(self, url, tdenv=None):
+    def __init__(self, url, tdenv=None, *, timeout: int = 90):
         self.url = url
         self.tdenv = tdenv
         if not url.startswith("file:///"):
-            requests = import_requests()
-            self.req = requests.get(self.url, stream=True)
+            requests = import_requests()  # pylint: disable=redefined-outer-name
+            self.req = requests.get(self.url, stream=True, timeout=timeout)
             self.lines = self.req.iter_lines()
         else:
             self.lines = open(url[8:], "rUb")
         self.columns = self.next_line().split(',')
     
     def next_line(self):
         """ Fetch the next line as a text string """
```

### Comparing `tradedangerous-10.9.8/tradedangerous/tools.py` & `tradedangerous-11.0.0/tradedangerous/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,7 +33,8 @@
     for stn in tdb.stationByID.values():
         m = utils.checkForOcrDerp(tdenv, stn.system.dbname, stn.dbname)
         if m:
             print("Match", m.groups(1))
             matches += 1
     if not matches:
         print("Current data is free of known derp")
+    tdb.close()
```

### Comparing `tradedangerous-10.9.8/tradedangerous/corrections.py` & `tradedangerous-11.0.0/tradedangerous/corrections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # Provides an interface for correcting names that
 # have changed in recent versions.
 
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-
 # Arbitrary, negative value to denote something that's been removed.
 DELETED = -111
 
 systems = {
     "PANDAMONIUM": "PANDEMONIUM",
     "ARGETLÁMH": "ARGETLAMH",
     "LíFTHRUTI": "LIFTHRUTI",
@@ -22,15 +20,15 @@
 
 items = {
     'POWER TRANSFER CONDUITS': 'Power Transfer Bus',
     'LOW TEMPERATURE DIAMOND': 'Low Temperature Diamonds',
     'COOLING HOSES': 'Micro-weave Cooling Hoses',
     'METHANOL MONOHYDRATE': 'Methanol Monohydrate Crystals',
     'OCCUPIED CRYOPOD': 'Occupied Escape Pod',
-    'SALVAGEABLE WRECKAGE': 'Wreckage Components', 
+    'SALVAGEABLE WRECKAGE': 'Wreckage Components',
     'POLITICAL PRISONER': 'Political Prisoners',
     'HOSTAGE': 'Hostages',
     "VOID OPAL": "Void Opals",
 }
 
 def correctSystem(oldName):
     try:
```

### Comparing `tradedangerous-10.9.8/tradedangerous/tradecalc.py` & `tradedangerous-11.0.0/tradedangerous/tradecalc.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,21 +35,20 @@
 """
 
 ######################################################################
 # Imports
 
 from collections import defaultdict
 from collections import namedtuple
-from .tradedb import System, Station, Trade, TradeDB, describeAge
+from .tradedb import System, Station, Trade, describeAge
 from .tradedb import Destination
 from .tradeexcept import TradeException
 
 import datetime
 import locale
-import math
 import os
 from .misc import progress as pbar
 import re
 import sys
 import time
 
 locale.setlocale(locale.LC_ALL, '')
@@ -128,15 +127,15 @@
 
 emptyLoad = TradeLoad((), 0, 0, 0)
 
 ######################################################################
 # Classes
 
 
-class Route(object):
+class Route:
     """
     Describes a series of hops where a TradeLoad is picked up at
     one station, the player travels via 0 or more hyperspace
     jumps and docks at a second station where they unload.
     E.g. 10 Algae + 5 Hydrogen at Station A, jump to System2,
     jump to System3, dock at Station B, sell everything, buy gold,
     jump to system4 and sell everything at Station X.
@@ -206,55 +205,53 @@
         if self.score == rhs.score:
             return len(self.jumps) < len(rhs.jumps)
         return self.score > rhs.score
     
     def __eq__(self, rhs):
         return self.score == rhs.score and len(self.jumps) == len(rhs.jumps)
     
-    def str(self, colorize):
+    def text(self, colorize) -> str:
         return "%s -> %s" % (colorize("cyan", self.firstStation.name()), colorize("blue", self.lastStation.name()))
     
     def detail(self, tdenv):
         """
         Return a string describing this route to a given level of detail.
         """
         
         detail, goalSystem = tdenv.detail, tdenv.goalSystem
         
-        colorize = tdenv.colorize if tdenv.color else lambda x, y : y
+        colorize = tdenv.colorize if tdenv.color else lambda x, y: y
         
-        credits = self.startCr + (tdenv.insurance or 0)
+        credits = self.startCr + (tdenv.insurance or 0)  # pylint: disable=redefined-builtin
         gainCr = 0
         route = self.route
         
         hops = self.hops
         
         # TODO: Write as a comprehension, just can't wrap my head
         # around it this morning.
         def genSubValues():
             for hop in hops:
-                for (tr, qty) in hop[0]:
+                for tr, _ in hop[0]:
                     yield len(tr.name(detail))
         
         longestNameLen = max(genSubValues())
         
-        text = self.str(colorize)
+        text = self.text(colorize)
         if detail >= 1:
             text += " (score: {:f})".format(self.score)
         text += "\n"
-        jumpsFmt = ("  Jump {jumps}\n")
-        cruiseFmt = ("  Supercruise to {stn}\n")
+        jumpsFmt = "  Jump {jumps}\n"
+        cruiseFmt = "  Supercruise to {stn}\n"
         distFmt = None
         if detail > 1:
             if detail > 2:
                 text += self.summary() + "\n"
                 if tdenv.maxJumpsPer > 1:
-                    distFmt = (
-                        "  Direct: {dist:0.2f}ly, Trip: {trav:0.2f}ly\n"
-                    )
+                    distFmt = "  Direct: {dist:0.2f}ly, Trip: {trav:0.2f}ly\n"
             hopFmt = (
                 "  Load from "
                 +colorize("cyan", "{station}") + 
                 ":\n{purchases}"
             )
             hopStepFmt = (
                 colorize("lightYellow", "     {qty:>4}") + 
@@ -352,14 +349,16 @@
                     details.append('BMk:' + station.blackMarket)
                 if station.maxPadSize != '?':
                     details.append('Pad:' + station.maxPadSize)
                 if station.planetary != '?':
                     details.append('Plt:' + station.planetary)
                 if station.fleet != '?':
                     details.append('Flc:' + station.fleet)
+                if station.odyssey != '?':
+                    details.append('Ody:' + station.odyssey)
                 if station.shipyard != '?':
                     details.append('Shp:' + station.shipyard)
                 if station.outfitting != '?':
                     details.append('Out:' + station.outfitting)
                 if station.refuel != '?':
                     details.append('Ref:' + station.refuel)
                 details = "{} ({})".format(
@@ -437,15 +436,14 @@
                 if travelled and distFmt and len(self.jumps[i]) > 2:
                     text += distFmt.format(
                         dist = startStn.system.distanceTo(endStn.system),
                         trav = travelled,
                     )
             if dockFmt:
                 stn = route[i + 1]
-                stnName = stn.name()
                 text += dockFmt.format(
                     station = decorateStation(stn),
                     gain = hopGainCr,
                     tongain = hopGainCr / hopTonnes,
                     credits = credits + gainCr + hopGainCr
                 )
             
@@ -465,15 +463,15 @@
         return text
     
     def summary(self):
         """
         Returns a string giving a short summary of this route.
         """
         
-        credits, hops, jumps = self.startCr, self.hops, self.jumps
+        credits, hops, jumps = self.startCr, self.hops, self.jumps  # pylint: disable=redefined-builtin
         ttlGainCr = sum(hop[1] for hop in hops)
         numJumps = sum(
             len(hopJumps) - 1
             for hopJumps in jumps
             if hopJumps  # don't include in-system hops
         )
         return (
@@ -489,15 +487,15 @@
                 gain = ttlGainCr,
                 hopgain = ttlGainCr // len(hops),
                 final = credits + ttlGainCr
             )
         )
 
 
-class TradeCalc(object):
+class TradeCalc:
     """
     Container for accessing trade calculations with common properties.
     """
     
     def __init__(self, tdb, tdenv = None, fit = None, items = None):
         """
         Constructs the TradeCalc object and loads sell/buy data.
@@ -540,30 +538,30 @@
             cutoff = datetime.datetime.now() - maxDays
             wheres.append("(modified >= ?)")
             binds.append(str(cutoff.replace(microsecond = 0)))
         
         if tdenv.avoidItems or items:
             avoidItemIDs = set(item.ID for item in tdenv.avoidItems)
             loadItems = items or tdb.itemByID.values()
-            loadItemIDs = set()
+            loadItemSet = set()
             for item in loadItems:
                 ID = item if isinstance(item, int) else item.ID
                 if ID not in avoidItemIDs:
-                    loadItemIDs.add(str(ID))
-            if not loadItemIDs:
+                    loadItemSet.add(str(ID))
+            if not loadItemSet:
                 raise TradeException("No items to load.")
-            loadItemIDs = ",".join(str(ID) for ID in loadItemIDs)
-            wheres.append("(item_id IN ({}))".format(loadItemIDs))
+            load_ids = ",".join(str(ID) for ID in loadItemSet)
+            wheres.append(f"(item_id IN ({load_ids}))")
         
         demand = self.stationsBuying = defaultdict(list)
         supply = self.stationsSelling = defaultdict(list)
         
         whereClause = " AND ".join(wheres) or "1"
         
-        lastStnID, stnAppend = 0, None
+        lastStnID = 0
         dmdCount, supCount = 0, 0
         stmt = """
                 SELECT  station_id, item_id,
                         strftime('%s', modified),
                         demand_price, demand_units, demand_level,
                         supply_price, supply_units, supply_level
                   FROM  StationItem
@@ -583,27 +581,27 @@
                 lastStnID = stnID
             try:
                 ageS = now - int(timestamp)
             except TypeError:
                 raise BadTimestampError(
                     self.tdb,
                     stnID, itmID, timestamp
-                )
+                ) from None
             if dmdCr > 0:
                 if not minDemand or dmdUnits >= minDemand:
                     dmdAppend((itmID, dmdCr, dmdUnits, dmdLevel, ageS))
                     dmdCount += 1
             if supCr > 0 and supUnits:
                 if not minSupply or supUnits >= minSupply:
                     supAppend((itmID, supCr, supUnits, supLevel, ageS))
                     supCount += 1
         
         tdenv.DEBUG0("Loaded {} buys, {} sells".format(dmdCount, supCount))
     
-    def bruteForceFit(self, items, credits, capacity, maxUnits):
+    def bruteForceFit(self, items, credits, capacity, maxUnits):  # pylint: disable=redefined-builtin
         """
         Brute-force generation of all possible combinations of items.
         This is provided to make it easy to validate the results of future
         variants or optimizations of the fit algorithm.
         """
         
         def _fitCombos(offset, cr, cap, level = 1):
@@ -650,15 +648,15 @@
                     combGain, combCost, combUnits
                 )
             
             return bestLoad
         
         return _fitCombos(0, credits, capacity)
     
-    def fastFit(self, items, credits, capacity, maxUnits):
+    def fastFit(self, items, credits, capacity, maxUnits):  # pylint: disable=redefined-builtin
         """
             Best load calculator using a recursive knapsack-like
             algorithm to find multiple loads and return the best.
             [eyeonus] Left in for the masochists, as this becomes
             horribly slow at stations with many items for sale.
             As in iooks-like-the-program-has-frozen slow.
         """
@@ -749,15 +747,15 @@
                 bestQty += bestSub.units
             return TradeLoad(bestLoad, bestGainCr, bestCostCr, bestQty)
         
         return _fitCombos(0, credits, capacity)
     
     # Mark's test run, to spare searching back through the forum posts for it.
     # python trade.py run --fr="Orang/Bessel Gateway" --cap=720 --cr=11b --ly=24.73 --empty=37.61 --pad=L --hops=2 --jum=3 --loop --summary -vv --progress
-    def simpleFit(self, items, credits, capacity, maxUnits):
+    def simpleFit(self, items, credits, capacity, maxUnits):  # pylint: disable=redefined-builtin
         """
         Simplistic load calculator:
         (The item list is sorted with highest profit margin items in front.)
         Step 1: Fill hold with as much of item1 as possible based on the limiting
                 factors of hold size, supply amount, and available credits.
         
         Step 2: If there is space in the hold and money available, repeat Step 1
@@ -819,15 +817,15 @@
         maxGainCr = max(minGainCr, self.tdenv.maxGainPerTon or sys.maxsize)
         getBuy = {buy[0]: buy for buy in dstBuying}.get
         addTrade = trading.append
         for sell in srcSelling:  # should be the smaller list
             buy = getBuy(sell[0], None)
             if buy:
                 gainCr = buy[1] - sell[1]
-                if gainCr >= minGainCr and gainCr <= maxGainCr:
+                if minGainCr <= gainCr <= maxGainCr:
                     addTrade(Trade(
                         itemIdx[sell[0]],
                         sell[1], gainCr,
                         sell[2], sell[3],
                         buy[2], buy[3],
                         sell[4], buy[4],
                     ))
@@ -856,19 +854,20 @@
         avoidPlaces = getattr(tdenv, 'avoidPlaces', None) or ()
         assert not restrictTo or isinstance(restrictTo, set)
         maxJumpsPer = tdenv.maxJumpsPer
         maxLyPer = tdenv.maxLyPer
         maxPadSize = tdenv.padSize
         planetary = tdenv.planetary
         fleet = tdenv.fleet
+        odyssey = tdenv.odyssey
         noPlanet = tdenv.noPlanet
         maxLsFromStar = tdenv.maxLs or float('inf')
         reqBlackMarket = getattr(tdenv, 'blackMarket', False) or False
         maxAge = getattr(tdenv, 'maxAge') or 0
-        credits = tdenv.credits - (getattr(tdenv, 'insurance', 0) or 0)
+        credits = tdenv.credits - (getattr(tdenv, 'insurance', 0) or 0)  # pylint: disable=redefined-builtin
         fitFunction = self.defaultFit
         capacity = tdenv.capacity
         maxUnits = getattr(tdenv, 'limit') or capacity
         
         bestToDest = {}
         safetyMargin = 1.0 - tdenv.margin
         unique = tdenv.unique
@@ -895,15 +894,15 @@
         if tdenv.direct:
             if goalSystem and not restrictTo:
                 restrictTo = (goalSystem,)
                 restrictStations = set(goalSystem.stations)
             if avoidPlaces:
                 restrictStations = set(
                     stn for stn in restrictStations
-                    if stn not in avoidPlaces and \
+                    if stn not in avoidPlaces and
                         stn.system not in avoidPlaces
                 )
             
             def station_iterator(srcStation):
                 srcSys = srcStation.system
                 srcDist = srcSys.distanceTo
                 for stn in restrictStations:
@@ -924,27 +923,27 @@
                     maxLyPer = maxLyPer,
                     avoidPlaces = avoidPlaces,
                     maxPadSize = maxPadSize,
                     maxLsFromStar = maxLsFromStar,
                     noPlanet = noPlanet,
                     planetary = planetary,
                     fleet = fleet,
+                    odyssey = odyssey,
                 )
         
         prog = pbar.Progress(len(routes), 25)
         connections = 0
         getSelling = self.stationsSelling.get
         for route in routes:
             if tdenv.progress:
                 prog.increment(1)
-            tdenv.DEBUG1("Route = {}", route.str(lambda x, y : y))
+            tdenv.DEBUG1("Route = {}", route.text(lambda x, y: y))
             
             srcStation = route.lastStation
             startCr = credits + int(route.gainCr * safetyMargin)
-            routeJumps = len(route.jumps)
             
             srcSelling = getSelling(srcStation.ID, None)
             srcSelling = tuple(
                 values for values in srcSelling
                 if values[1] <= startCr
             )
             if not srcSelling:
@@ -960,50 +959,34 @@
                 srcGoalDist = srcDistTo(goalSystem)
                 srcOrigDist = srcDistTo(origSystem)
                 origGoalDist = origDistTo(goalSystem)
             
             if unique:
                 uniquePath = route.route
             elif loopInt:
-                uniquePath = route.route[-loopInt:-1]
+                pos_from_end = 0 - loopInt
+                uniquePath = route.route[pos_from_end:-1]
             
-            stations = (
-                dest for dest in station_iterator(srcStation)
-                if dest.station != srcStation
+            stations = (d for d in station_iterator(srcStation)
+              if (d.station != srcStation) and
+                (d.station.blackMarket == 'Y' if reqBlackMarket else True) and
+                (d.station not in uniquePath if uniquePath else True) and
+                (d.station in restrictStations if restrictStations else True) and
+                (d.station.dataAge and d.station.dataAge <= maxAge if maxAge else True) and
+                (((d.system is not srcSystem) if bool(tdenv.unique) else (d.system is goalSystem or d.distLy < srcGoalDist)) if goalSystem else True)
             )
-            if reqBlackMarket:
-                stations = (d for d in stations if d.station.blackMarket == 'Y')
-            if uniquePath:
-                stations = (d for d in stations if d.station not in uniquePath)
-            if restrictStations:
-                stations = (
-                    d for d in stations
-                    if d.station in restrictStations
-                )
-            if maxAge:
-                stations = (d for d in stations if d.station.dataAge)
-                stations = (d for d in stations if d.station.dataAge <= maxAge)
-            if goalSystem:
-                if bool(tdenv.unique):
-                    stations = (
-                        d for d in stations if d.system is not srcSystem
-                    )
-                stations = (
-                    d for d in stations
-                    if d.system is goalSystem or d.distLy < srcGoalDist
-                )
             
             if tdenv.debug >= 1:
                 
                 def annotate(dest):
                     tdenv.DEBUG1(
                         "destSys {}, destStn {}, jumps {}, distLy {}",
                         dest.system.dbname,
                         dest.station.dbname,
-                        "->".join(jump.str() for jump in dest.via),
+                        "->".join(jump.text() for jump in dest.via),
                         dest.distLy
                     )
                     return True
                 
                 stations = (d for d in stations if annotate(d))
             
             for dest in stations:
@@ -1119,11 +1102,11 @@
         
         if connections == 0:
             raise NoHopsError(
                 "No destinations could be reached within the constraints."
             )
         
         result = []
-        for (dst, route, trade, jumps, ly, score) in bestToDest.values():
+        for (dst, route, trade, jumps, _, score) in bestToDest.values():
             result.append(route.plus(dst, trade, jumps, score))
         
         return result
```

### Comparing `tradedangerous-10.9.8/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-11.0.0/tradedangerous/templates/TradeDangerous.sql`

 * *Files 18% similar despite different names*

```diff
@@ -1,304 +1,305 @@
--- Definitions for all of the tables used in the SQLite
--- cache database.
---
--- Source data for TradeDangerous is stored in various
--- ".csv" files which provide relatively constant data
--- such as star names, the list of known tradeable items,
--- etc.
---
--- Per-station price data is sourced from ".prices" files
--- which are designed to be human readable text that
--- closely aproximates the in-game UI.
---
--- When the .SQL file or the .CSV files change, TD will
--- destroy and rebuild the cache next time it is run.
---
--- When the .prices file is changed, only the price data
--- is reset.
---
--- You can edit this file, if you really need to, if you know
--- what you are doing. Or you can use the 'sqlite3' command
--- to edit the .db database and then use the '.dump' command
--- to regenerate this file, except then you'll lose this nice
--- header and I might have to wag my finger at you.
---
--- -Oliver
-
-PRAGMA foreign_keys=ON;
-PRAGMA synchronous=OFF;
-PRAGMA temp_store=MEMORY;
-
-BEGIN TRANSACTION;
-
-
-CREATE TABLE Added
- (
-   added_id INTEGER PRIMARY KEY AUTOINCREMENT,
-   name VARCHAR(40) COLLATE nocase,
-
-   UNIQUE(name)
- );
-
-
-CREATE TABLE System
- (
-   system_id INTEGER PRIMARY KEY,
-   name VARCHAR(40) COLLATE nocase,
-   pos_x DOUBLE NOT NULL,
-   pos_y DOUBLE NOT NULL,
-   pos_z DOUBLE NOT NULL,
-   added_id INTEGER,
-   modified DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
-
-   UNIQUE (system_id),
-
-    FOREIGN KEY (added_id) REFERENCES Added(added_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE
- );
-CREATE INDEX idx_system_by_pos ON System (pos_x, pos_y, pos_z, system_id);
-
-
-CREATE TABLE Station
- (
-   station_id INTEGER PRIMARY KEY,
-   name VARCHAR(40) COLLATE nocase,
-   system_id INTEGER NOT NULL,
-   ls_from_star INTEGER NOT NULL DEFAULT 0
-       CHECK (ls_from_star >= 0),
-   blackmarket TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (blackmarket IN ('?', 'Y', 'N')),
-   max_pad_size TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (max_pad_size IN ('?', 'S', 'M', 'L')),
-   market TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (market IN ('?', 'Y', 'N')),
-   shipyard TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (shipyard IN ('?', 'Y', 'N')),
-   modified DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
-   outfitting TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (outfitting IN ('?', 'Y', 'N')),
-   rearm      TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (rearm      IN ('?', 'Y', 'N')),
-   refuel     TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (refuel     IN ('?', 'Y', 'N')),
-   repair     TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (repair     IN ('?', 'Y', 'N')),
-   planetary  TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (planetary  IN ('?', 'Y', 'N')),
-   type_id INTEGER DEFAULT 0 NOT NULL,
-
-   UNIQUE (station_id),
-
-   FOREIGN KEY (system_id) REFERENCES System(system_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE
- );
-CREATE INDEX idx_station_by_system ON Station (system_id, station_id);
-CREATE INDEX idx_station_by_name ON Station (name);
-
-
-CREATE TABLE Ship
- (
-   ship_id INTEGER PRIMARY KEY,
-   name VARCHAR(40) COLLATE nocase,
-   cost INTEGER NOT NULL,
-   fdev_id INTEGER,
-
-   UNIQUE (ship_id)
- );
-
-
-CREATE TABLE ShipVendor
- (
-   ship_id INTEGER NOT NULL,
-   station_id INTEGER NOT NULL,
-   modified DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
-
-   PRIMARY KEY (ship_id, station_id),
-
-   FOREIGN KEY (ship_id) REFERENCES Ship(ship_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE,
-   FOREIGN KEY (station_id) REFERENCES Station(station_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE
- ) WITHOUT ROWID
-;
-
-
-CREATE TABLE Upgrade
- (
-   upgrade_id INTEGER PRIMARY KEY,
-   name VARCHAR(40) COLLATE nocase,
-   weight NUMBER NOT NULL,
-   cost NUMBER NOT NULL,
-
-   UNIQUE (upgrade_id)
- );
-
-
-CREATE TABLE UpgradeVendor
- (
-   upgrade_id INTEGER NOT NULL,
-   station_id INTEGER NOT NULL,
-   cost INTEGER,
-   modified DATETIME NOT NULL,
-
-   PRIMARY KEY (upgrade_id, station_id),
-
-   FOREIGN KEY (upgrade_id) REFERENCES Upgrade(upgrade_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE,
-   FOREIGN KEY (station_id) REFERENCES Station(station_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE
- ) WITHOUT ROWID
-;
-CREATE INDEX idx_vendor_by_station_id ON UpgradeVendor (station_id);
-
-CREATE TABLE RareItem
- (
-   rare_id INTEGER PRIMARY KEY AUTOINCREMENT,
-   station_id INTEGER NOT NULL,
-   category_id INTEGER NOT NULL,
-   name VARCHAR(40) COLLATE nocase,
-   cost INTEGER,
-   max_allocation INTEGER,
-   illegal TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (illegal IN ('?', 'Y', 'N')),
-   suppressed TEXT(1) NOT NULL DEFAULT '?'
-       CHECK (suppressed IN ('?', 'Y', 'N')),
-
-   UNIQUE (name),
-
-   FOREIGN KEY (station_id) REFERENCES Station(station_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE,
-   FOREIGN KEY (category_id) REFERENCES Category(category_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE
- )
-;
-
-CREATE TABLE Category
- (
-   category_id INTEGER PRIMARY KEY,
-   name VARCHAR(40) COLLATE nocase,
-
-   UNIQUE (category_id)
- );
-
-
-CREATE TABLE Item
- (
-   item_id INTEGER PRIMARY KEY,
-   name VARCHAR(40) COLLATE nocase,
-   category_id INTEGER NOT NULL,
-   ui_order INTEGER NOT NULL DEFAULT 0,
-   avg_price INTEGER,
-   fdev_id INTEGER,
-
-   UNIQUE (item_id),
-   UNIQUE (fdev_id),
-
-   FOREIGN KEY (category_id) REFERENCES Category(category_id)
-    ON UPDATE CASCADE
-    ON DELETE CASCADE
- );
- CREATE INDEX idx_item_by_fdev_id ON Item (fdev_id);
-
-
-CREATE TABLE StationItem
- (
-  station_id INTEGER NOT NULL,
-  item_id INTEGER NOT NULL,
-  demand_price INT NOT NULL,
-  demand_units INT NOT NULL,
-  demand_level INT NOT NULL,
-  supply_price INT NOT NULL,
-  supply_units INT NOT NULL,
-  supply_level INT NOT NULL,
-  modified DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
-  from_live INTEGER DEFAULT 0 NOT NULL,
-
-  PRIMARY KEY (station_id, item_id),
-  FOREIGN KEY (station_id) REFERENCES Station(station_id)
-    ON UPDATE CASCADE ON DELETE CASCADE,
-  FOREIGN KEY (item_id) REFERENCES Item(item_id)
-    ON UPDATE CASCADE ON DELETE CASCADE
-);
-CREATE INDEX si_mod_stn_itm ON StationItem(modified, station_id, item_id);
-CREATE INDEX si_itm_dmdpr ON StationItem(item_id, demand_price) WHERE demand_price > 0;
-CREATE INDEX si_itm_suppr ON StationItem(item_id, supply_price) WHERE supply_price > 0;
-
-CREATE VIEW StationBuying AS
-SELECT  station_id,
-        item_id,
-        demand_price AS price,
-        demand_units AS units,
-        demand_level AS level,
-        modified
-  FROM  StationItem
- WHERE  demand_price > 0
-;
-
-CREATE VIEW StationSelling AS
-SELECT  station_id,
-        item_id,
-        supply_price AS price,
-        supply_units AS units,
-        supply_level AS level,
-        modified
-  FROM  StationItem
- WHERE  supply_price > 0
-;
-
-
---
--- The next two tables (FDevShipyard, FDevOutfitting) are
--- used to map the FDev API IDs to data ready for EDDN.
---
--- The column names are the same as the header line from
--- the EDCD/FDevIDs csv files, so we can just download the
--- files (shipyard.csv, outfitting.csv) and save them
--- as (FDevShipyard.csv, FDevOutfitting.csv) into the
--- data directory.
---
--- see https://github.com/EDCD/FDevIDs
---
--- The commodity.csv is not needed because TD and EDDN
--- are using the same names.
---
--- -Bernd
-
-CREATE TABLE FDevShipyard
- (
-   id INTEGER NOT NULL,
-   symbol VARCHAR(40),
-   name VARCHAR(40) COLLATE nocase,
-
-   UNIQUE (id)
- );
-
-
-CREATE TABLE FDevOutfitting
- (
-   id INTEGER NOT NULL,
-   symbol VARCHAR(40),
-   category CHAR(10)
-      CHECK (category IN ('hardpoint','internal','standard','utility')),
-   name VARCHAR(40) COLLATE nocase,
-   mount CHAR(10)
-      CHECK (mount IN (NULL, 'Fixed','Gimballed','Turreted')),
-   guidance CHAR(10)
-      CHECK (guidance IN (NULL, 'Dumbfire','Seeker','Swarm')),
-   ship VARCHAR(40) COLLATE nocase,
-   class CHAR(1) NOT NULL,
-   rating CHAR(1) NOT NULL,
-   entitlement CHAR(10),
-
-   UNIQUE (id)
- );
-
-
-COMMIT;
+-- Definitions for all of the tables used in the SQLite
+-- cache database.
+--
+-- Source data for TradeDangerous is stored in various
+-- ".csv" files which provide relatively constant data
+-- such as star names, the list of known tradeable items,
+-- etc.
+--
+-- Per-station price data is sourced from ".prices" files
+-- which are designed to be human readable text that
+-- closely aproximates the in-game UI.
+--
+-- When the .SQL file or the .CSV files change, TD will
+-- destroy and rebuild the cache next time it is run.
+--
+-- When the .prices file is changed, only the price data
+-- is reset.
+--
+-- You can edit this file, if you really need to, if you know
+-- what you are doing. Or you can use the 'sqlite3' command
+-- to edit the .db database and then use the '.dump' command
+-- to regenerate this file, except then you'll lose this nice
+-- header and I might have to wag my finger at you.
+--
+-- -Oliver
+
+PRAGMA foreign_keys=ON;
+PRAGMA synchronous=OFF;
+PRAGMA temp_store=MEMORY;
+PRAGMA journal_mode=WAL;
+PRAGMA auto_vacuum=INCREMENTAL;
+
+BEGIN TRANSACTION;
+
+
+CREATE TABLE Added
+ (
+   added_id INTEGER PRIMARY KEY AUTOINCREMENT,
+   name VARCHAR(40) COLLATE nocase,
+
+   UNIQUE(name)
+ );
+
+
+CREATE TABLE System
+ (
+   system_id INTEGER PRIMARY KEY,
+   name VARCHAR(40) COLLATE nocase,
+   pos_x DOUBLE NOT NULL,
+   pos_y DOUBLE NOT NULL,
+   pos_z DOUBLE NOT NULL,
+   added_id INTEGER,
+   modified DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
+
+   UNIQUE (system_id),
+
+    FOREIGN KEY (added_id) REFERENCES Added(added_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE
+ );
+CREATE INDEX idx_system_by_pos ON System (pos_x, pos_y, pos_z, system_id);
+
+
+CREATE TABLE Station
+ (
+   station_id INTEGER PRIMARY KEY,
+   name VARCHAR(40) COLLATE nocase,
+   system_id INTEGER NOT NULL,
+   ls_from_star INTEGER NOT NULL DEFAULT 0
+       CHECK (ls_from_star >= 0),
+   blackmarket TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (blackmarket IN ('?', 'Y', 'N')),
+   max_pad_size TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (max_pad_size IN ('?', 'S', 'M', 'L')),
+   market TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (market IN ('?', 'Y', 'N')),
+   shipyard TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (shipyard IN ('?', 'Y', 'N')),
+   modified DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
+   outfitting TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (outfitting IN ('?', 'Y', 'N')),
+   rearm      TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (rearm      IN ('?', 'Y', 'N')),
+   refuel     TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (refuel     IN ('?', 'Y', 'N')),
+   repair     TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (repair     IN ('?', 'Y', 'N')),
+   planetary  TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (planetary  IN ('?', 'Y', 'N')),
+   type_id INTEGER DEFAULT 0 NOT NULL,
+
+   UNIQUE (station_id),
+
+   FOREIGN KEY (system_id) REFERENCES System(system_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE
+ );
+CREATE INDEX idx_station_by_system ON Station (system_id, station_id);
+CREATE INDEX idx_station_by_name ON Station (name);
+
+
+CREATE TABLE Ship
+ (
+   ship_id INTEGER PRIMARY KEY,
+   name VARCHAR(40) COLLATE nocase,
+   cost INTEGER NOT NULL,
+
+   UNIQUE (ship_id)
+ );
+
+
+CREATE TABLE ShipVendor
+ (
+   ship_id INTEGER NOT NULL,
+   station_id INTEGER NOT NULL,
+   modified DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
+
+   PRIMARY KEY (ship_id, station_id),
+
+   FOREIGN KEY (ship_id) REFERENCES Ship(ship_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE,
+   FOREIGN KEY (station_id) REFERENCES Station(station_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE
+ ) WITHOUT ROWID
+;
+
+
+CREATE TABLE Upgrade
+ (
+   upgrade_id INTEGER PRIMARY KEY,
+   name VARCHAR(40) COLLATE nocase,
+   weight NUMBER NOT NULL,
+   cost NUMBER NOT NULL,
+
+   UNIQUE (upgrade_id)
+ );
+
+
+CREATE TABLE UpgradeVendor
+ (
+   upgrade_id INTEGER NOT NULL,
+   station_id INTEGER NOT NULL,
+   cost INTEGER,
+   modified DATETIME NOT NULL,
+
+   PRIMARY KEY (upgrade_id, station_id),
+
+   FOREIGN KEY (upgrade_id) REFERENCES Upgrade(upgrade_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE,
+   FOREIGN KEY (station_id) REFERENCES Station(station_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE
+ ) WITHOUT ROWID
+;
+CREATE INDEX idx_vendor_by_station_id ON UpgradeVendor (station_id);
+
+CREATE TABLE RareItem
+ (
+   rare_id INTEGER PRIMARY KEY,
+   station_id INTEGER NOT NULL,
+   category_id INTEGER NOT NULL,
+   name VARCHAR(40) COLLATE nocase,
+   cost INTEGER,
+   max_allocation INTEGER,
+   illegal TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (illegal IN ('?', 'Y', 'N')),
+   suppressed TEXT(1) NOT NULL DEFAULT '?'
+       CHECK (suppressed IN ('?', 'Y', 'N')),
+
+   UNIQUE (name),
+
+   FOREIGN KEY (station_id) REFERENCES Station(station_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE,
+   FOREIGN KEY (category_id) REFERENCES Category(category_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE
+ )
+;
+
+CREATE TABLE Category
+ (
+   category_id INTEGER PRIMARY KEY,
+   name VARCHAR(40) COLLATE nocase,
+
+   UNIQUE (category_id)
+ );
+
+
+CREATE TABLE Item
+ (
+   item_id INTEGER PRIMARY KEY,
+   name VARCHAR(40) COLLATE nocase,
+   category_id INTEGER NOT NULL,
+   ui_order INTEGER NOT NULL DEFAULT 0,
+   avg_price INTEGER,
+   fdev_id INTEGER,
+
+   UNIQUE (item_id),
+
+   FOREIGN KEY (category_id) REFERENCES Category(category_id)
+    ON UPDATE CASCADE
+    ON DELETE CASCADE
+ );
+ CREATE INDEX idx_item_by_fdev_id ON Item (fdev_id);
+
+
+CREATE TABLE StationItem
+ (
+  station_id INTEGER NOT NULL,
+  item_id INTEGER NOT NULL,
+  demand_price INT NOT NULL,
+  demand_units INT NOT NULL,
+  demand_level INT NOT NULL,
+  supply_price INT NOT NULL,
+  supply_units INT NOT NULL,
+  supply_level INT NOT NULL,
+  modified DATETIME DEFAULT CURRENT_TIMESTAMP NOT NULL,
+  from_live INTEGER DEFAULT 0 NOT NULL,
+
+  PRIMARY KEY (station_id, item_id),
+  FOREIGN KEY (station_id) REFERENCES Station(station_id)
+    ON UPDATE CASCADE ON DELETE CASCADE,
+  FOREIGN KEY (item_id) REFERENCES Item(item_id)
+    ON UPDATE CASCADE ON DELETE CASCADE
+);
+CREATE INDEX si_mod_stn_itm ON StationItem(modified, station_id, item_id);
+CREATE INDEX si_itm_dmdpr ON StationItem(item_id, demand_price) WHERE demand_price > 0;
+CREATE INDEX si_itm_suppr ON StationItem(item_id, supply_price) WHERE supply_price > 0;
+
+CREATE VIEW StationBuying AS
+SELECT  station_id,
+        item_id,
+        demand_price AS price,
+        demand_units AS units,
+        demand_level AS level,
+        modified
+  FROM  StationItem
+ WHERE  demand_price > 0
+;
+
+CREATE VIEW StationSelling AS
+SELECT  station_id,
+        item_id,
+        supply_price AS price,
+        supply_units AS units,
+        supply_level AS level,
+        modified
+  FROM  StationItem
+ WHERE  supply_price > 0
+;
+
+
+--
+-- The next two tables (FDevShipyard, FDevOutfitting) are
+-- used to map the FDev API IDs to data ready for EDDN.
+--
+-- The column names are the same as the header line from
+-- the EDCD/FDevIDs csv files, so we can just download the
+-- files (shipyard.csv, outfitting.csv) and save them
+-- as (FDevShipyard.csv, FDevOutfitting.csv) into the
+-- data directory.
+--
+-- see https://github.com/EDCD/FDevIDs
+--
+-- The commodity.csv is not needed because TD and EDDN
+-- are using the same names.
+--
+-- -Bernd
+
+CREATE TABLE FDevShipyard
+ (
+   id INTEGER NOT NULL,
+   symbol VARCHAR(40),
+   name VARCHAR(40) COLLATE nocase,
+   entitlement VARCHAR(50),
+
+   UNIQUE (id)
+ );
+
+
+CREATE TABLE FDevOutfitting
+ (
+   id INTEGER NOT NULL,
+   symbol VARCHAR(40),
+   category CHAR(10)
+      CHECK (category IN ('hardpoint','internal','standard','utility')),
+   name VARCHAR(40) COLLATE nocase,
+   mount CHAR(10)
+      CHECK (mount IN (NULL, 'Fixed','Gimballed','Turreted')),
+   guidance CHAR(10)
+      CHECK (guidance IN (NULL, 'Dumbfire','Seeker','Swarm')),
+   ship VARCHAR(40) COLLATE nocase,
+   class CHAR(1) NOT NULL,
+   rating CHAR(1) NOT NULL,
+   entitlement VARCHAR(50),
+
+   UNIQUE (id)
+ );
+
+
+COMMIT;
```

### Comparing `tradedangerous-10.9.8/tradedangerous/templates/Added.csv` & `tradedangerous-11.0.0/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.8/tradedangerous/templates/RareItem.csv` & `tradedangerous-11.0.0/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.8/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-11.0.0/tradedangerous/plugins/edcd_plug.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import csv
 import pathlib
-import random
 
-from .. import cache, tradeenv, transfers, csvexport
+from .. import cache, transfers, csvexport
 from ..tradedb import Category, Item
 from . import PluginException, ImportPluginBase
 
 class ImportPlugin(ImportPluginBase):
     """
     Download and process EDCD CSV-file(s)
     """
@@ -190,28 +189,27 @@
             tdenv.NOTE("Nothing had to be done")
 
 
     def process_fdevids_items(self, localPath, tableName):
         """
             More to do for commodities
         """
-        tdb, tdenv = self.tdb, self.tdenv
+        tdenv = self.tdenv
         tdenv.NOTE("Processing {}", tableName)
         
         itmCount = 0
         catCount = 0
         edcdItems = {}
         edcdCategories = {}
-        with localPath.open('rU', encoding='utf-8') as importFile:
+        with localPath.open('r', encoding='utf-8') as importFile:
             csvIn = csv.reader(
                 importFile, delimiter=',', quotechar="'", doublequote=True
             )
             # first line must be the column names
             columnDefs = next(csvIn)
-            columnCount = len(columnDefs)
             
             tdenv.DEBUG0("columnDefs: {}", columnDefs)
             
             idxMap = {}
             for cIndex, cName in enumerate(columnDefs):
                 idxMap[cName] = cIndex
             tdenv.DEBUG0("idxMap: {}", idxMap)
@@ -231,15 +229,16 @@
                     pass
                 return val
             
             if notGood:
                 tdenv.NOTE("Import stopped.", checkMe, localPath)
             else:
                 for lineIn in csvIn:
-                    if not lineIn: continue
+                    if not lineIn:
+                        continue
                     lineNo = csvIn.line_num
                     tdenv.DEBUG0("LINE {}: {}", lineNo, lineIn)
                     
                     # strip() it do be save
                     edcdId       = lineIn[idxMap['id']].strip()
                     edcdCategory = lineIn[idxMap['category']].strip()
                     edcdName     = lineIn[idxMap['name']].strip()
```

### Comparing `tradedangerous-10.9.8/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-11.0.0/tradedangerous/plugins/netlog_plug.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 import os
 import re
 import pathlib
 import time as _time
-from datetime import datetime, time, timedelta, timezone
+from datetime import datetime, timedelta, timezone
 
-from .. import tradedb, tradeenv, csvexport
+from .. import csvexport
 from . import PluginException, ImportPluginBase
 
 def snapToGrid32(val):
     try:
         val = float(val)
-        if val < 0: corr = -0.5
-        else:       corr = +0.5
+        corr = -0.5 if val < 0 else +0.5
         pos = int(val*32+corr)/32
     except:
         pos = None
         pass
     return pos
 
 
@@ -78,19 +77,19 @@
         # HEADER: Logs/netLog.170430120645.01.log (part 1)
         # HEADER: 2017-04-30 12:06 Mitteleurop�ische Sommerzeit
         # HEADER: ============================================
         # SYSTEM: {10:13:33GMT 407.863s} System:"Huokang" StarPos:(-12.188,35.469,-25.281)ly  NormalFlight
         tdb, tdenv = self.tdb, self.tdenv
         optShow = self.getOption("show")
         
-        oldHeadRegEx = re.compile("^(?P<headDateTime>\d\d-\d\d-\d\d-\d\d:\d\d)\s+(?P<headTZName>.*[^\s])\s+(?P<headTimeGMT>\(.*GMT\))")
-        newHeadRegEx = re.compile("^(?P<headDateTime>\d\d\d\d-\d\d-\d\d\s+\d\d:\d\d)\s+(?P<headTZName>.*[^\s])")
+        oldHeadRegEx = re.compile(r"^(?P<headDateTime>\d\d-\d\d-\d\d-\d\d:\d\d)\s+(?P<headTZName>.*[^\s])\s+(?P<headTimeGMT>\(.*GMT\))")
+        newHeadRegEx = re.compile(r"^(?P<headDateTime>\d\d\d\d-\d\d-\d\d\s+\d\d:\d\d)\s+(?P<headTZName>.*[^\s])")
         
-        sysRegEx  = re.compile('^\{[^\}]+\}\s+System:"(?P<sysName>[^"]+)".*StarPos:\((?P<sysPos>[^)]+)\)ly')
-        dateRegEx = re.compile('^\{(?P<logTime>\d\d:\d\d:\d\d)')
+        sysRegEx  = re.compile(r'^\{[^\}]+\}\s+System:"(?P<sysName>[^"]+)".*StarPos:\((?P<sysPos>[^)]+)\)ly')
+        dateRegEx = re.compile(r'^\{(?P<logTime>\d\d:\d\d:\d\d)')
         
         def calcSeconds(h=0, m=0, s=0):
             return 3600*h + 60*m + s
         
         sysCount = 0
         logSysList = {}
         for filePath in self.filePathList:
@@ -134,15 +133,15 @@
                                     timezone(headTZInfo)
                                 )
                             except:
                                 headDate = None
                                 pass
                         if not headDate:
                             if lineCount > 3:
-                               raise PluginException("Doesn't seem do be a FDEV netLog file")
+                                raise PluginException("Doesn't seem do be a FDEV netLog file")
                         else:
                             statHeader = False
                             if lineCount == 3:
                                 # new format since 2.3, switch to UTC
                                 headDate = headDate.astimezone()
                             tdenv.DEBUG0("   DATE: {}", headDate)
                             headSecs = calcSeconds(headDate.hour, headDate.minute, headDate.second)
@@ -180,14 +179,15 @@
                         lastSecs = logSecs
             sysCount = len(logSysList)
             tdenv.NOTE("Found {} System(s).", sysCount-oldCount)
         
         if not optShow:
             try:
                 idNetLog = tdb.lookupAdded(self.ADDED_NAME)
+                tdenv.DEBUG1("idNetLog = {}", idNetLog)
             except KeyError:
                 tdenv.WARN("Entry '{}' not found in 'Added' table.", self.ADDED_NAME)
                 tdenv.WARN("Trying to add it myself.")
                 db = tdb.getDB()
                 cur = db.cursor()
                 cur.execute(
                     """
```

### Comparing `tradedangerous-10.9.8/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-11.0.0/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import os
-import re
 from pathlib import Path
 
-from .. import tradedb, tradeenv, cache, fs
+from .. import fs
 from ..commands.exceptions import CommandLineError
 from . import PluginException, ImportPluginBase
 
 class ImportPlugin(ImportPluginBase):
     """
     Plugin that imports multiple .price files at once
     """
@@ -59,15 +57,15 @@
             stations = self.file_get_stations(filePath)
             
             # Does not support resolving multiple stations (yet)
             if len(stations) > 1:
                 raise PluginException("EDMC Batch unable to process files with multiple stations. Use normal import.")
             
             for s in stations:
-                if(s in stations_seen):
+                if s in stations_seen:
                     cur_file = stations_seen[s]
                     # Set the newer file as the one we'll use.
                     stations_seen[s] = self.file_get_newer(cur_file, f)
                 else:
                     stations_seen[s] = f
         
         return stations_seen.values()
@@ -77,15 +75,15 @@
     """
     def set_environment(self, files):
         tdenv = self.tdenv
         path_list = files
         fs.ensurefolder(tdenv.tmpDir)
         batchfile = tdenv.tmpDir / Path(self.BATCH_FILE)
         if batchfile.exists():
-                batchfile.unlink()
+            batchfile.unlink()
         # We now have a list of paths. Add all contents to a new file
         temp_file = open(batchfile, "w")
         
         for f in path_list:
             contents = f.read_text()
             temp_file.writelines("# File: {}\n".format(f))
             temp_file.write(contents)
```

### Comparing `tradedangerous-10.9.8/tradedangerous/plugins/journal_plug.py` & `tradedangerous-11.0.0/tradedangerous/plugins/journal_plug.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         pos = None
         pass
     return pos
 
 def getYNfromService(obj, key):
     return "Y" if key in obj else "N"
 
-class JournalStation(object):
+class JournalStation:
     __slots__ = (
         'lsFromStar', 'blackMarket', 'maxPadSize',
         'market', 'shipyard', 'outfitting',
         'rearm', 'refuel', 'repair',
         'planetary', 'modified'
     )
     
@@ -299,14 +299,15 @@
         """
         tdb, tdenv = self.tdb, self.tdenv
         optShow = self.getOption("show")
         
         if not optShow:
             try:
                 idJournal = tdb.lookupAdded(self.ADDED_NAME)
+                tdenv.DEBUG1("idjournal = {}", idJournal)
             except KeyError:
                 tdenv.WARN("Entry '{}' not found in 'Added' table.", self.ADDED_NAME)
                 tdenv.WARN("Trying to add it myself.")
                 db = tdb.getDB()
                 cur = db.cursor()
                 cur.execute(
                     "INSERT INTO Added(name) VALUES(?)",
```

### Comparing `tradedangerous-10.9.8/tradedangerous/plugins/__init__.py` & `tradedangerous-11.0.0/tradedangerous/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class PluginException(Exception):
     """
     Base class for exceptions thrown by plugins.
     """
 
 
-class PluginBase(object):
+class PluginBase:
     """
     Base class for plugin implementation.
     
     To implement a plugin, create a file in the plugins directory
     called "mypluginname_plug.py". This file should implement
     plugin classes derived from the appropriate plugins base,
     e.g. for an import pluggin:
@@ -45,15 +45,15 @@
         for opt in tdenv.pluginOptions or []:
             equals = opt.find('=')
             if equals < 0:
                 key, value = opt, True
             else:
                 key, value = opt[:equals], opt[equals+1:]
             keyName = key.lower()
-            if not keyName in pluginOptions:
+            if keyName not in pluginOptions:
                 if keyName == "help":
                     raise SystemExit(self.usage())
                 
                 if not pluginOptions:
                     raise PluginException(
                         "This plugin does not support any options."
                     )
```

### Comparing `tradedangerous-10.9.8/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-11.0.0/tradedangerous/plugins/edapi_plug.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,15 @@
         self.wfile.write(body_text)
         self.wfile.write(b"</body></html>")
     
     def log_message(self, format, *args):
         pass
 
 
-class OAuthCallbackServer(object):
-    
+class OAuthCallbackServer:
     def __init__(self, hostname, port, handler):
         myServer = HTTPServer
         myServer.callback_code = None
         myServer.callback_state = None
         self.httpd = myServer((hostname, port), handler)
         self.httpd.handle_request()
         self.httpd.server_close()
@@ -132,16 +131,19 @@
         # If force login, kill the authorization
         if self.login:
             self._authorization_set_config({})
         
         # Grab the commander profile
         self.text = []
         self.profile = self.query_capi("/profile")
-        market = self.query_capi("/market")
-        shipyard = self.query_capi("/shipyard")
+        
+        # kfsone: not sure if there was a reason to query these even tho we didn't
+        # use the resulting data.
+        # market = self.query_capi("/market")
+        # shipyard = self.query_capi("/shipyard")
         
         # Grab the market, outfitting and shipyard data if needed
         portServices = self.profile['lastStarport'].get('services')
         if self.profile['commander']['docked'] and portServices:
             if portServices.get('commodities'):
                 res = self.query_capi("/market")
                 if int(res["id"]) == int(self.profile["lastStarport"]["id"]):
@@ -499,15 +501,16 @@
         defOutfitting = getYNfromObject(checkStarport, 'modules')
         tellUserAPIResponse("'Outfitting'", defOutfitting)
         tellUserAPIResponse("'ShipYard'", defShipyard)
         tellUserAPIResponse("'Market'", defMarket)
         
         def warnAPIResponse(checkName, checkYN):
             # no warning if unknown
-            if checkYN == "?": return False
+            if checkYN == "?":
+                return False
             warnText = (
                 "The station should{s} have a {what}, "
                 "but the API did{d} return one."
             )
             if checkYN == "Y":
                 s, d = "", "n't"
             else:
@@ -578,15 +581,15 @@
         if defStation.market != defMarket:
             warning |= warnAPIResponse('market', defStation.market)
         if warning:
             tdenv.WARN("Please update station data with correct values.")
             tdenv.WARN("(Fields will be marked with an leading asterisk '*')")
             askForData = True
         if ((defStation.lsFromStar == 0) or ("?" in defStation)):
-           askForData = True
+            askForData = True
         
         newStation = {}
         for key in defStation._fields:
             newStation[key] = getattr(defStation, key)
         
         if askForData:
             tdenv.NOTE("Values in brackets are the default.")
@@ -808,17 +811,15 @@
         # New or update station data
         station = self.askForStationData(system, stnName = stnName, station = station)
         
         # If a shipyard exists, make the ship lists
         shipCost = {}
         shipList = []
         eddn_ships = []
-        if ((station.shipyard == "Y") and
-            ('ships' in api.profile['lastStarport'])
-        ):
+        if ((station.shipyard == "Y") and ('ships' in api.profile['lastStarport'])):
             if 'shipyard_list' in api.profile['lastStarport']['ships']:
                 if len(api.profile['lastStarport']['ships']['shipyard_list']):
                     for ship in api.profile['lastStarport']['ships']['shipyard_list'].values():
                         shipName = shipMap.mapID(ship['id'], ship['name'])
                         shipCost[shipName] = ship['basevalue']
                         shipList.append(shipName)
                         eddn_ships.append(ship['name'])
@@ -910,17 +911,15 @@
                     "ShipVendor",
                 )
                 tdenv.DEBUG0("{} updated.", csvPath)
         
         # If a market exists, make the item lists
         itemList = []
         eddn_market = []
-        if ((station.market == "Y") and
-            ('commodities' in api.profile['lastStarport'])
-        ):
+        if ((station.market == "Y") and ('commodities' in api.profile['lastStarport'])):
             for commodity in api.profile['lastStarport']['commodities']:
                 if commodity['categoryname'] in cat_ignore:
                     continue
                 
                 if commodity.get('legality', '') != '':
                     # ignore if present and not empty
                     continue
@@ -1042,26 +1041,21 @@
                 con.publishShipyard(
                     sysName,
                     stnName,
                     marketId,
                     eddn_ships
                 )
             
-            if ((station.outfitting == "Y") and
-                ('modules' in api.profile['lastStarport'] and
-                len(api.profile['lastStarport']['modules']))
-            ):
+            if station.outfitting == "Y" and 'modules' in api.profile['lastStarport'] and len(api.profile['lastStarport']['modules']):
                 eddn_modules = []
                 for module in api.profile['lastStarport']['modules'].values():
                     # see: https://github.com/EDSM-NET/EDDN/wiki
                     addModule = False
                     if module['name'].startswith(('Hpt_', 'Int_')) or module['name'].find('_Armour_') > 0:
-                        if module.get('sku', None) in (
-                            None, 'ELITE_HORIZONS_V_PLANETARY_LANDINGS'
-                        ):
+                        if module.get('sku', None) in (None, 'ELITE_HORIZONS_V_PLANETARY_LANDINGS'):
                             if module['name'] != 'Int_PlanetApproachSuite':
                                 addModule = True
                     if addModule:
                         eddn_modules.append(module['name'])
                     elif self.getOption("test"):
                         tdenv.NOTE("Ignored module ID: {}, name: {}", module['id'], module['name'])
                 if eddn_modules:
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/export_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/export_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-
 from ..csvexport import exportTableToFile
-from .parsing import *
+from .parsing import ParseArgument, MutuallyExclusiveGroup
 from .exceptions import CommandLineError
 from pathlib import Path
 
 import sqlite3
 
 ######################################################################
 # TradeDangerous :: Commands :: Export
@@ -118,8 +116,8 @@
         # create CSV files
         lineCount, filePath = exportTableToFile(tdb, cmdenv, tableName, exportPath)
         if cmdenv.deleteEmpty and lineCount == 0:
             # delete file if emtpy
             filePath.unlink()
             cmdenv.DEBUG0("Delete empty file {file}'".format(file=filePath))
     
-    return None
+    return None
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/import_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/import_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-
-from .exceptions import *
-from .parsing import *
+from .exceptions import CommandLineError
+from .parsing import ParseArgument, MutuallyExclusiveGroup
 from itertools import chain
 from pathlib import Path
 
 from .. import cache, plugins, transfers
-import math
 import re
+import sys
 
 try:
     import tkinter
     import tkinter.filedialog as tkfd
     hasTkInter = True
 except ImportError:
     hasTkInter = False
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/olddata_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-from .parsing import *
+from .parsing import (
+    FleetCarrierArgument, MutuallyExclusiveGroup, NoPlanetSwitch,
+    OdysseyArgument, ParseArgument, PadSizeArgument, PlanetaryArgument,
+)
 from ..tradedb import TradeDB
 from ..tradeexcept import TradeException
 
-import itertools
-import math
-import sys
 
 ######################################################################
 # Parser config
 
 name='olddata'
 help='Show oldest data in database.'
 epilog=None
@@ -44,14 +43,15 @@
     ),
     PadSizeArgument(),
     MutuallyExclusiveGroup(
         NoPlanetSwitch(),
         PlanetaryArgument(),
     ),
     FleetCarrierArgument(),
+    OdysseyArgument(),
     ParseArgument('--ls-max',
         help='Only consider stations upto this many ls from their star.',
         metavar='LS',
         dest='maxLs',
         type=int,
         default=0,
     ),
@@ -61,15 +61,14 @@
 # Perform query and populate result set
 
 def run(results, cmdenv, tdb):
     from .commandenv import ResultRow
     
     cmdenv = results.cmdenv
     tdb = cmdenv.tdb
-    srcSystem = cmdenv.nearSystem
     
     results.summary = ResultRow()
     results.limit = cmdenv.limit
     
     fields = [
         "si.station_id",
         "JULIANDAY('NOW') - JULIANDAY(MAX(si.modified))",
@@ -148,35 +147,37 @@
             wheres=whereStr,
             having=haveStr,
     )
     
     cmdenv.DEBUG1(stmt)
     
     padSize = cmdenv.padSize
-    fleet = cmdenv.fleet
     planetary = cmdenv.planetary
+    fleet = cmdenv.fleet
+    odyssey = cmdenv.odyssey
     noPlanet = cmdenv.noPlanet
     mls = cmdenv.maxLs
     
     for (stnID, age, ls, dist2) in tdb.query(stmt):
         cmdenv.DEBUG2("{}:{}:{}", stnID, age, ls)
         row = ResultRow()
         row.station = tdb.stationByID[stnID]
         row.age = age
         if ls:
             row.ls = "{:n}".format(ls)
         else:
             row.ls = "?"
         row.dist = dist2 ** 0.5
         if not padSize or row.station.checkPadSize(padSize):
-            if not fleet or row.station.checkFleet(fleet):
-                if not planetary or row.station.checkPlanetary(planetary):
-                    if not noPlanet or row.station.planetary == 'N':
-                        if not mls or row.station.lsFromStar <= mls:
-                            results.rows.append(row)
+            if not planetary or row.station.checkPlanetary(planetary):
+                if not fleet or row.station.checkFleet(fleet):
+                    if not odyssey or row.station.checkOdyssey(odyssey):
+                        if not noPlanet or row.station.planetary == 'N':
+                            if not mls or row.station.lsFromStar <= mls:
+                                results.rows.append(row)
     
     if cmdenv.route and len(results.rows) > 1:
         def walk(startNode, dist):
             rows = results.rows
             startNode = rows[startNode]
             openList = set(rows)
             path = [startNode]
@@ -233,24 +234,25 @@
                 ColumnFormat("Age/days", '>', '8', '.2f',
                         key=lambda row: row.age)
         ).append(
                 ColumnFormat("StnLs", '>', '10',
                         key=lambda row: row.station.distFromStar())
         ).append(
                 ColumnFormat("Pad", '>', '3',
-                        key=lambda row: \
-                            TradeDB.padSizes[row.station.maxPadSize])
+                        key=lambda row: TradeDB.padSizes[row.station.maxPadSize])
+        ).append(
+                ColumnFormat("Plt", '>', '3',
+                        key=lambda row: TradeDB.planetStates[row.station.planetary])
         ).append(
                 ColumnFormat("Flc", '>', '3',
-                        key=lambda row: \
-                            TradeDB.fleetStates[row.station.fleet])
+                        key=lambda row: TradeDB.fleetStates[row.station.fleet])
         ).append(
-                ColumnFormat("Plt", '>', '3',
-                        key=lambda row: \
-                            TradeDB.planetStates[row.station.planetary]))
+                ColumnFormat("Ody", '>', '3',
+                        key=lambda row: TradeDB.odysseyStates[row.station.odyssey])
+        )
     
     if not cmdenv.quiet:
         heading, underline = rowFmt.heading()
         print(heading, underline, sep='\n')
     
     for row in results.rows:
-        print(rowFmt.format(row))
+        print(rowFmt.format(row))
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/nav_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/nav_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-from .parsing import *
-import math
+from .parsing import (
+    AvoidPlacesArgument, FleetCarrierArgument, MutuallyExclusiveGroup,
+    NoPlanetSwitch, OdysseyArgument, PadSizeArgument, ParseArgument,
+    PlanetaryArgument,
+)
 from ..tradedb import System, Station, TradeDB
 from ..tradeexcept import TradeException
 
+
 ######################################################################
 # Parser config
 
 help='Calculate a route between two systems.'
 name='nav'
 epilog=None
 wantsTradeDB=True
@@ -39,14 +42,15 @@
     ),
     PadSizeArgument(),
     MutuallyExclusiveGroup(
         NoPlanetSwitch(),
         PlanetaryArgument(),
     ),
     FleetCarrierArgument(),
+    OdysseyArgument(),
 ]
 
 ######################################################################
 # Helpers
 
 
 class NoRouteError(TradeException):
@@ -82,21 +86,22 @@
         avoid for avoid in cmdenv.avoidPlaces
         if isinstance(avoid, System)
     ]
     
     route = [ ]
     stationInterval = cmdenv.stationInterval
     for hop in hops:
-        hopRoute = list(tdb.getRoute(
+        try:
+            hopRoute = list(tdb.getRoute(
                 hop[0], hop[1],
                 maxLyPer,
                 avoiding,
                 stationInterval=stationInterval,
                 ))
-        if not hopRoute:
+        except TypeError:
             raise NoRouteError(
                     "No route found between {} and {} "
                     "with a max {}ly/jump limit.".format(
                         hop[0].name(), hop[1].name(),
                         maxLyPer,
             ))
         route = route[:-1] + hopRoute
@@ -105,16 +110,17 @@
                 fromSys=srcSystem,
                 toSys=dstSystem,
                 maxLy=maxLyPer,
             )
     
     lastSys, totalLy, dirLy = srcSystem, 0.00, 0.00
     maxPadSize = cmdenv.padSize
-    fleet = cmdenv.fleet
     planetary = cmdenv.planetary
+    fleet = cmdenv.fleet
+    odyssey = cmdenv.odyssey
     noPlanet = cmdenv.noPlanet
     
     for (jumpSys, dist) in route:
         jumpLy = lastSys.distanceTo(jumpSys)
         totalLy += jumpLy
         if cmdenv.detail:
             dirLy = jumpSys.distanceTo(dstSystem)
@@ -126,17 +132,19 @@
             dirLy=dirLy,
             )
         row.stations = []
         if cmdenv.stations:
             for (station) in jumpSys.stations:
                 if maxPadSize and not station.checkPadSize(maxPadSize):
                     continue
+                if planetary and not station.checkPlanetary(planetary):
+                    continue
                 if fleet and not station.checkFleet(fleet):
                     continue
-                if planetary and not station.checkPlanetary(planetary):
+                if odyssey and not station.checkOdyssey(odyssey):
                     continue
                 if noPlanet and station.planetary != 'N':
                     continue
                 rr = ResultRow(
                     station=station,
                     age=station.itemDataAgeStr,
                 )
@@ -188,52 +196,45 @@
                 ColumnFormat("StnLs", '>', '10',
                     key=lambda row: row.station.distFromStar())
         ).append(
                 ColumnFormat("Age/days", '>', 7,
                         key=lambda row: row.age)
         ).append(
                 ColumnFormat('Mkt', '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.market])
+                    key=lambda row: TradeDB.marketStates[row.station.market])
         ).append(
                 ColumnFormat("BMk", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.blackMarket])
+                    key=lambda row: TradeDB.marketStates[row.station.blackMarket])
         ).append(
                 ColumnFormat("Shp", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.shipyard])
+                    key=lambda row: TradeDB.marketStates[row.station.shipyard])
         ).append(
                 ColumnFormat("Out", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.outfitting])
+                    key=lambda row: TradeDB.marketStates[row.station.outfitting])
         ).append(
                 ColumnFormat("Arm", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.rearm])
+                    key=lambda row: TradeDB.marketStates[row.station.rearm])
         ).append(
                 ColumnFormat("Ref", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.refuel])
+                    key=lambda row: TradeDB.marketStates[row.station.refuel])
         ).append(
                 ColumnFormat("Rep", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.repair])
+                    key=lambda row: TradeDB.marketStates[row.station.repair])
         ).append(
                 ColumnFormat("Pad", '>', '3',
-                    key=lambda row: \
-                        TradeDB.padSizes[row.station.maxPadSize])
+                    key=lambda row: TradeDB.padSizes[row.station.maxPadSize])
         ).append(
                 ColumnFormat("Plt", '>', '3',
-                    key=lambda row: \
-                        TradeDB.planetStates[row.station.planetary])
+                    key=lambda row: TradeDB.planetStates[row.station.planetary])
         ).append(
                 ColumnFormat("Flc", '>', '3',
-                    key=lambda row: \
-                        TradeDB.fleetStates[row.station.fleet])
+                    key=lambda row: TradeDB.fleetStates[row.station.fleet])
+        ).append(
+                ColumnFormat("Ody", '>', '3',
+                    key=lambda row: TradeDB.odysseyStates[row.station.odyssey])
         )
         if cmdenv.detail > 1:
             stnRowFmt.append(
                 ColumnFormat("Itms", ">", 4,
                     key=lambda row: row.station.itemCount)
             )
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/update_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/update_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-from .parsing import *
+from .parsing import MutuallyExclusiveGroup, ParseArgument
 from ..tradeexcept import TradeException
 from .exceptions import CommandLineError
-from ..tradedb import System, Station
+from ..tradedb import System
 from .. import prices, cache
 import subprocess
 import os
 import sys
 import pathlib
 
 ######################################################################
@@ -163,15 +162,16 @@
         ))
 
 
 def getEditorPaths(cmdenv, editorName, envVar, windowsFolders, winExe, nixExe):
     cmdenv.DEBUG0("Locating {} editor", editorName)
     try:
         return os.environ[envVar]
-    except KeyError: pass
+    except KeyError:
+        pass
     
     paths = []
     
     import platform
     system = platform.system()
     if system == 'Windows':
         binary = winExe
@@ -179,15 +179,16 @@
             for version in windowsFolders:
                 paths.append("{}\\{}\\{}".format(os.environ['SystemDrive'], folder, version))
     else:
         binary = nixExe
     
     try:
         paths += os.environ['PATH'].split(os.pathsep)
-    except KeyError: pass
+    except KeyError:
+        pass
     
     for path in paths:
         candidate = os.path.join(path, binary)
         try:
             if pathlib.Path(candidate).exists():
                 return candidate
         except OSError:
@@ -267,16 +268,18 @@
     # Create a temporary text file with a list of the price data.
     tmpPath = getTemporaryPath(cmdenv)
     
     absoluteFilename = None
     dbFilename = tdb.dbFilename
     try:
         elementMask = prices.Element.basic | prices.Element.supply
-        if cmdenv.timestamps: elementMask |= prices.Element.timestamp
-        if cmdenv.all: elementMask |= prices.Element.blanks
+        if cmdenv.timestamps:
+            elementMask |= prices.Element.timestamp
+        if cmdenv.all:
+            elementMask |= prices.Element.blanks
         # Open the file and dump data to it.
         with tmpPath.open("w", encoding = 'utf-8') as tmpFile:
             # Remember the filename so we know we need to delete it.
             absoluteFilename = str(tmpPath.resolve())
             prices.dumpPrices(dbFilename, elementMask,
                     file = tmpFile,
                     stationID = stationID,
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/station_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/station_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 from .commandenv import ResultRow
 from .exceptions import CommandLineError
-from .parsing import *
+from .parsing import MutuallyExclusiveGroup, ParseArgument
 from ..tradedb import AmbiguityError
-from ..tradedb import System, Station
+from ..tradedb import Station
 from ..tradedb import TradeDB
 from .. import utils
 from ..formatting import max_len
 
 from .. import cache
 from .. import csvexport
 import difflib
 import re
-import sys
+
 
 ######################################################################
 # Parser config
 
 help='Add (or update) a station entry'
 name='station'
 epilog=None
@@ -98,14 +97,25 @@
     ),
     ParseArgument(
         '--planetary',
         help='Is the station on a planet (Y or N) or ? if unknown.',
         choices=['Y', 'y', 'N', 'n', '?'],
     ),
     ParseArgument(
+        '--fleet-carrier', '--fc',
+        dest='fleet',
+        help='Is the station a Fleet Carrier (Y or N) or ? if unknown.',
+        choices=['Y', 'y', 'N', 'n', '?'],
+    ),
+    ParseArgument(
+        '--odyssey', '--od',
+        help='Is the station an Odyssey Settlement (Y or N) or ? if unknown.',
+        choices=['Y', 'y', 'N', 'n', '?'],
+    ),
+    ParseArgument(
         '--confirm',
         help='For confirmation suspicious looking station names.',
         metavar='CONFIRMATION CODE',
         type=str,
     ),
     ParseArgument(
         '--no-export',
@@ -229,17 +239,15 @@
     if slashPos > 0:
         sysName, stnName = stnName[:slashPos], stnName[slashPos+1:]
         sysName = sysName.upper()
     else:
         sysName = None
     
     if not stnName:
-        raise CommandLineError("Invalid station name: {}".format(
-                envStnName
-        ))
+        raise CommandLineError("Invalid station name: {stnName}")
     
     if not sysName:
         raise CommandLineError("No system name specified")
     
     cmdenv.system, cmdenv.station = sysName, utils.titleFixup(stnName)
     try:
         system = tdb.lookupSystem(sysName)
@@ -265,14 +273,16 @@
             shipyard=cmdenv.shipyard or '?',
             outfitting=cmdenv.outfitting or '?',
             rearm=cmdenv.rearm or '?',
             refuel=cmdenv.refuel or '?',
             repair=cmdenv.repair or '?',
             maxPadSize=cmdenv.padSize or '?',
             planetary=cmdenv.planetary or '?',
+            fleet=cmdenv.fleet or '?',
+            odyssey=cmdenv.odyssey or '?',
             commit=True,
     )
 
 
 def updateStation(tdb, cmdenv, station):
     return tdb.updateLocalStation(
             station=station,
@@ -282,14 +292,16 @@
             shipyard=cmdenv.shipyard,
             outfitting=cmdenv.outfitting,
             rearm=cmdenv.rearm,
             refuel=cmdenv.refuel,
             repair=cmdenv.repair,
             maxPadSize=cmdenv.padSize,
             planetary=cmdenv.planetary,
+            fleet=cmdenv.fleet,
+            odyssey=cmdenv.odyssey,
             force=True,
             commit=True,
     )
 
 
 def removeStation(tdb, cmdenv, station):
     db = tdb.getDB()
@@ -327,15 +339,14 @@
 
 def run(results, cmdenv, tdb):
     if cmdenv.lsFromStar and cmdenv.lsFromStar < 0:
         raise CommandLineError("Invalid (negative) --ls option")
     
     system, station = checkSystemAndStation(tdb, cmdenv)
     
-    systemName = cmdenv.system
     stationName = cmdenv.station
     
     if cmdenv.add:
         result = addStation(tdb, cmdenv, system, stationName)
         return checkResultAndExportStations(tdb, cmdenv, result)
     elif cmdenv.update:
         result = updateStation(tdb, cmdenv, station)
@@ -348,15 +359,15 @@
     results.summary = ResultRow()
     results.summary.system = station.system
     results.summary.station = station
     
     avgSell = results.summary.avgSelling = tdb.getAverageSelling()
     avgBuy = results.summary.avgBuying = tdb.getAverageBuying()
     
-    class ItemTrade(object):
+    class ItemTrade:
         def __init__(self, ID, price, avgAgainst):
             self.ID, self.item = ID, tdb.itemByID[ID]
             self.price = int(price)
             self.avgTrade = avgAgainst.get(ID, 0)
     
     # Look up all selling and buying by the station
     selling, buying = [], []
@@ -420,14 +431,16 @@
     print("B/Market..:", _detail(station.blackMarket, TradeDB.marketStates))
     print("Shipyard..:", _detail(station.shipyard, TradeDB.marketStates))
     print("Outfitting:", _detail(station.outfitting, TradeDB.marketStates))
     print("Rearm.....:", _detail(station.rearm, TradeDB.marketStates))
     print("Refuel....:", _detail(station.refuel, TradeDB.marketStates))
     print("Repair....:", _detail(station.repair, TradeDB.marketStates))
     print("Planetary.:", _detail(station.planetary, TradeDB.planetStates))
+    print("Fleet.....:", _detail(station.fleet, TradeDB.fleetStates))
+    print("Odyssey...:", _detail(station.odyssey, TradeDB.odysseyStates))
     print("Prices....:", station.itemCount or 'None')
     
     if station.itemCount == 0:
         return
     
     newest, oldest = tdb.query("""
             SELECT JULIANDAY('NOW') - JULIANDAY(MAX(si.modified)),
@@ -471,15 +484,13 @@
 
     longestNameLen = max(
         max_len(results.summary.selling, key=lambda row: row.item.name(cmdenv.detail)),
         max_len(results.summary.buying, key=lambda row: row.item.name(cmdenv.detail)),
     )
     print("Best Buy..:", makeBest(
             results.summary.selling, "Buy from this station", "Sell", longestNameLen,
-            starFn=lambda price, avgCr: \
-                price <= (avgCr * 0.9),
+            starFn=lambda price, avgCr: price <= (avgCr * 0.9),
     ))
     print("Best Sale.:", makeBest(
             results.summary.buying, "Sell to this station", "Cost", longestNameLen,
-            starFn=lambda price, avgCr: \
-                price >= (avgCr * 1.1),
-    ))
+            starFn=lambda price, avgCr: price >= (avgCr * 1.1),
+    ))
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/buildcache_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-import sys
-
+from __future__ import annotations
 from .exceptions import CommandLineError
-from .parsing import *
+from .parsing import ParseArgument
 from ..cache import buildCache
 from ..tradedb import TradeDB
 
 ######################################################################
 # Parser config
 
 help = 'Build TradeDangerous cache file from sources'
@@ -50,24 +48,21 @@
 ######################################################################
 # Helpers
 
 ######################################################################
 # Perform query and populate result set
 
 
-def run(results, cmdenv, tdb):
+def run(results, cmdenv, tdb: TradeDB):
     # Check that the file doesn't already exist.
     if not cmdenv.force:
         if tdb.dbPath.exists():
             raise CommandLineError(
-                    "SQLite3 database '{}' already exists.\n"
-                     "Either remove the file first or use the '-f' option."
-                        .format(tdb.dbFilename))
+                "SQLite3 database '{tdb.dbFilename}' already exists.\n"
+                "Either remove the file first or use the '-f' option.")
     
     if not tdb.sqlPath.exists():
-        raise CommandLineError(
-                    "SQL File does not exist: {}"
-                        .format(tdb.sqlFilename))
+        raise CommandLineError("SQL File does not exist: {tdb.sqlFilename}")
     
     buildCache(tdb, cmdenv)
     
     return None
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/trade_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/trade_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-from .exceptions import *
-from .parsing import *
-from ..tradedb import TradeDB
-from ..tradecalc import TradeCalc, Route
-
-import math
+from .exceptions import CommandLineError
+from .parsing import ParseArgument
+from ..tradecalc import TradeCalc
+from ..formatting import RowFormat, max_len
 
 ######################################################################
 # Parser config
 
 help='Find places to buy a given item within range of a given station.'
 name='trade'
 epilog=None
@@ -61,16 +58,14 @@
     
     return results
 
 #######################################################################
 ## Transform result set into output
 
 def render(results, cmdenv, tdb):
-    from ..formatting import RowFormat, ColumnFormat, max_len
-    
     longestNameLen = max_len(results.rows, key=lambda row: row.item.name(cmdenv.detail))
     
     rowFmt = RowFormat()
     rowFmt.addColumn('Item', '<', longestNameLen,
             key=lambda row: row.item.name(cmdenv.detail))
     rowFmt.addColumn('Profit', '>', 10, 'n',
             key=lambda row: row.gainCr)
@@ -98,8 +93,8 @@
             key=lambda row: (row.dstAge / 86400))
     
     if not cmdenv.quiet:
         heading, underline = rowFmt.heading()
         print(heading, underline, sep='\n')
     
     for row in results.rows:
-        print(rowFmt.format(row))
+        print(rowFmt.format(row))
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-11.0.0/tradedangerous/commands/TEMPLATE.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 from commands.commandenv import ResultRow
 from commands.parsing import *
 from formatting import RowFormat, ColumnFormat
 
 ######################################################################
 # Parser config
 
@@ -55,8 +54,8 @@
     """
     If run() returns a non-None value, the trade.py code will then
     call the corresponding render() function.
     
     This is where you should generate any output from your command.
     """
     
-    ### TODO: Implement
+    ### TODO: Implement
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/exceptions.py` & `tradedangerous-11.0.0/tradedangerous/commands/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 from ..tradeexcept import TradeException
-import sys
+
 
 ######################################################################
 # Exceptions
 
 class UsageError(TradeException):
     def __init__(self, title, usage):
         self.title, self.usage = title, usage
+
     def __str__(self):
         return self.title + "\n\n" + self.usage
 
 
 class CommandLineError(TradeException):
     """
         Raised when you provide invalid input on the command line.
         Attributes:
             errorstr       What to tell the user.
     """
     def __init__(self, errorStr, usage=None):
         self.errorStr, self.usage = errorStr, usage
+ 
     def __str__(self):
         if self.usage:
             return "ERROR: {}\n\n{}".format(self.errorStr, self.usage)
         else:
             return "ERROR: {}".format(self.errorStr)
 
 
@@ -31,27 +32,28 @@
     """
         Raised when a request is made for which no data can be found.
         Attributes:
             errorStr        Describe the problem to the user.
     """
     def __init__(self, errorStr):
         self.errorStr = errorStr
+
     def __str__(self):
-        return "Error: {}\n".format(self.errorStr) + ("""
+        return f"""Error: {self.errorStr}
 Possible causes:
 - No profitable runs or routes meet your criteria,
 - Missing Systems or Stations along the route (see "local -vv"),
 - Missing price data (see "market -vv" or "update -h"),
 
 If you are not sure where to get data from, consider using a crowd-sourcing
 project such as EDDBlink (https://github.com/eyeonus/EDDBlink).
 
 For more help, see the TradeDangerous Wiki:
     https://github.com/eyeonus/Trade-Dangerous/wiki
-""").format(sys.argv[0])
+"""
 
 
 class PadSizeError(CommandLineError):
     """ Raised when an invalid pad-size option is given. """
     def __init__(self, value):
         super().__init__(
             "Invalid --pad-size '{}': Use a combination of one or more "
@@ -65,22 +67,33 @@
 class PlanetaryError(CommandLineError):
     """ Raised when an invalid planetary option is given. """
     def __init__(self, value):
         super().__init__(
             "Invalid --planetary '{}': Use a combination of one or more "
             "from 'Y' for Yes, 'N' for No or '?' for unknown, "
             "e.g. 'YN?' matches any station while 'Y?' matches "
-            "yes or unknown or 'N' matches only planetary stations."
+            "yes or unknown, or 'N' matches only non-planetary stations."
             .format(value)
         )
 
 
 class FleetCarrierError(CommandLineError):
     """ Raised when an invalid fleet-carrier option is given. """
     def __init__(self, value):
         super().__init__(
             "Invalid --fleet-carrier '{}': Use a combination of one or more "
             "from 'Y' for Yes, 'N' for No or '?' for unknown, "
             "e.g. 'YN?' matches any station while 'Y?' matches "
-            "yes or unknown or 'N' matches only fleet-carrier stations."
+            "yes or unknown, or 'N' matches only non-fleet-carrier stations."
+            .format(value)
+        )
+
+class OdysseyError(CommandLineError):
+    """ Raised when an invalid odyssey option is given. """
+    def __init__(self, value):
+        super().__init__(
+            "Invalid --odyssey '{}': Use a combination of one or more "
+            "from 'Y' for Yes, 'N' for No or '?' for unknown, "
+            "e.g. 'YN?' matches any station while 'Y?' matches "
+            "yes or unknown, or 'N' matches only non-odyssey stations."
             .format(value)
         )
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/buy_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/buy_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
+from __future__ import annotations
 from collections import defaultdict
 from .commandenv import ResultRow
-from .exceptions import *
-from .parsing import *
-from ..formatting import RowFormat, ColumnFormat, max_len
-from ..tradedb import TradeDB, AmbiguityError, System, Station
+from .exceptions import CommandLineError, NoDataError
+from ..formatting import RowFormat, max_len
+from ..tradedb import Station, System, TradeDB
+from .parsing import (
+    AvoidPlacesArgument, BlackMarketSwitch, FleetCarrierArgument, MutuallyExclusiveGroup,
+    NoPlanetSwitch, OdysseyArgument, PadSizeArgument, ParseArgument, PlanetaryArgument,
+)
 
-import math
 
 ITEM_MODE = "Item"
 SHIP_MODE = "Ship"
 
 ######################################################################
 # Parser config
 
@@ -55,14 +57,15 @@
     AvoidPlacesArgument(),
     PadSizeArgument(),
     MutuallyExclusiveGroup(
         NoPlanetSwitch(),
         PlanetaryArgument(),
     ),
     FleetCarrierArgument(),
+    OdysseyArgument(),
     BlackMarketSwitch(),
     MutuallyExclusiveGroup(
         ParseArgument(
             '--one-stop', '-1',
             help = 'Only list stations that carry all items listed.',
             action = 'store_true',
             dest = 'oneStop',
@@ -92,25 +95,32 @@
     ParseArgument(
         '--lt',
         help = 'Limit to prices below Ncr',
         metavar = 'N',
         dest = 'lt',
         type = "credits",
     ),
+    ParseArgument('--ls-max',
+        help='Only consider stations upto this many ls from their star.',
+        metavar='LS',
+        dest='maxLs',
+        type=int,
+        default=0,
+    ),
 )
 
 
 def get_lookup_list(cmdenv, tdb):
     # Credit: http://stackoverflow.com/a/952952/257645
     # Turns [['a'],['b','c']] => ['a', 'b', 'c']
     names = [
         name for names in cmdenv.name for name in names.split(',')
     ]
     # We only support searching for one type of purchase a time: ship or item.
-    # Our first match is open ended, but once we have matched one type of
+    # Our first match is open-ended, but once we have matched one type of
     # thing, the remaining arguments are all sourced from the same pool.
     # Thus: [food, cobra, metals] is illegal but [metals, hydrogen] is legal.
     mode = None
     
     queries = {}
     for name in names:
         if mode is not SHIP_MODE:
@@ -257,42 +267,50 @@
         results.summary.ly = maxLy
         distanceFn = nearSystem.distanceTo
     else:
         distanceFn = None
     
     oneStopMode = cmdenv.oneStop
     padSize = cmdenv.padSize
-    fleet = cmdenv.fleet
     planetary = cmdenv.planetary
+    fleet = cmdenv.fleet
+    odyssey = cmdenv.odyssey
     wantNoPlanet = cmdenv.noPlanet
     wantBlackMarket = cmdenv.blackMarket
+    mls = cmdenv.maxLs
     
     stations = defaultdict(list)
     stationByID = tdb.stationByID
     
     cur = sql_query(cmdenv, tdb, queries, mode)
     for (ID, stationID, price, units) in cur:
         station = stationByID[stationID]
         if padSize and not station.checkPadSize(padSize):
             continue
+        if planetary and not station.checkPlanetary(planetary):
+            continue
         if fleet and not station.checkFleet(fleet):
             continue
-        if planetary and not station.checkPlanetary(planetary):
+        if odyssey and not station.checkOdyssey(odyssey):
             continue
         if wantNoPlanet and station.planetary != 'N':
             continue
         if wantBlackMarket and station.blackMarket != 'Y':
             continue
         if station in avoidStations:
             continue
         if station.system in avoidSystems:
             continue
         
         row = ResultRow()
         row.station = station
+        if mls:
+            distanceFromStar = station.lsFromStar
+            if distanceFromStar > mls:
+                continue
         if distanceFn:
             distance = distanceFn(row.station.system)
             if distance > maxLy:
                 continue
             row.dist = distance
         row.item = queries[ID]
         row.price = price
@@ -370,21 +388,20 @@
             key = lambda row: TradeDB.marketStates[row.station.blackMarket])
     stnRowFmt.addColumn("Pad", '>', '3',
             key = lambda row: TradeDB.padSizes[row.station.maxPadSize])
     stnRowFmt.addColumn("Plt", '>', '3',
             key = lambda row: TradeDB.planetStates[row.station.planetary])
     stnRowFmt.addColumn("Flc", '>', '3',
             key = lambda row: TradeDB.fleetStates[row.station.fleet])
+    stnRowFmt.addColumn("Ody", '>', '3',
+            key = lambda row: TradeDB.odysseyStates[row.station.odyssey])
     
     if not cmdenv.quiet:
         heading, underline = stnRowFmt.heading()
         print(heading, underline, sep = '\n')
     
     for row in results.rows:
         print(stnRowFmt.format(row))
     
     if singleMode and cmdenv.detail:
-        print("{:{lnl}} {:>10n}".format(
-                "-- Ship Cost" if mode is SHIP_MODE else "-- Average",
-                results.summary.avg,
-                lnl = maxStnLen,
-        ))
+        msg = "-- Ship Cost" if mode is SHIP_MODE else "-- Average",
+        print(f"{msg:{maxStnLen}} {results.summary.avg:>10n}")
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/run_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/run_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from .commandenv import ResultRow
-from .exceptions import *
-from .parsing import *
+from .exceptions import CommandLineError, NoDataError
+from .parsing import (
+    BlackMarketSwitch, FleetCarrierArgument, MutuallyExclusiveGroup,
+    NoPlanetSwitch, OdysseyArgument, PadSizeArgument, ParseArgument,
+    PlanetaryArgument,
+)
 from itertools import chain
-from ..formatting import RowFormat, ColumnFormat
 from ..tradedb import TradeDB, System, Station, describeAge
 from ..tradecalc import TradeCalc, Route, NoHopsError
 
 import math
+import sys
+
 
 ######################################################################
 # Parser config
 
 help = 'Calculate best trade run.'
 name = 'run'
 epilog = None
@@ -133,14 +138,15 @@
     ),
     PadSizeArgument(),
     MutuallyExclusiveGroup(
         NoPlanetSwitch(),
         PlanetaryArgument(),
     ),
     FleetCarrierArgument(),
+    OdysseyArgument(),
     BlackMarketSwitch(),
     ParseArgument('--ls-penalty', '--lsp',
         help = "Penalty per 1kls stations are from their stars.",
         default = 12.5,
         type = float,
         dest = 'lsPenalty'
     ),
@@ -215,16 +221,15 @@
     ParseArgument('--x52-pro',
         help = 'Enable experimental X52 Pro MFD output.',
         action = 'store_true',
         default = False,
         dest = 'x52pro',
     ),
     ParseArgument('--prune-score',
-        help = 'From the 3rd hop on, only consider routes which have ' \
-            'at least this percentage of the current best route''s score.',
+        help = 'From the 3rd hop on, only consider routes which have at least this percentage of the current best route''s score.',
         dest = 'pruneScores',
         type = float,
         default = 0,
     ),
     ParseArgument('--prune-hops',
         help = 'Changes which hop --prune-score takes effect from.',
         default = 3,
@@ -256,15 +261,15 @@
     ),
 ]
 
 ######################################################################
 # Helpers
 
 
-class Checklist(object):
+class Checklist:
     """
         Class for encapsulating display of a route as a series of
         steps to be 'checked off' as the user passes through them.
     """
     
     def __init__(self, tdb, cmdenv):
         self.tdb = tdb
@@ -289,35 +294,35 @@
             )
         )
     
     def note(self, str, addBreak = True):
         print("(i) {} (i){}".format(str, "\n" if addBreak else ""))
     
     def run(self, route, cr):
-        tdb, mfd = self.tdb, self.mfd
+        mfd = self.mfd
         stations, hops, jumps = route.route, route.hops, route.jumps
         lastHopIdx = len(stations) - 1
         gainCr = 0
         self.stepNo = 0
         
-        heading = "(i) BEGINNING CHECKLIST FOR {} (i)".format(route.str(lambda x, y : y))
+        heading = "(i) BEGINNING CHECKLIST FOR {} (i)".format(route.text(lambda x, y: y))
         print(heading, "\n", '-' * len(heading), "\n\n", sep = '')
         
         cmdenv = self.cmdenv
         if cmdenv.detail:
             print(route.summary())
             print()
         
         for idx in range(lastHopIdx):
             hopNo = idx + 1
             cur, nxt, hop = stations[idx], stations[idx + 1], hops[idx]
             sortedTradeOptions = sorted(
                 hop[0],
-                key = lambda tradeOption: \
-                    tradeOption[1] * tradeOption[0].gainCr, reverse = True
+                key=lambda tradeOption: tradeOption[1] * tradeOption[0].gainCr,
+                reverse=True
             )
             
             # Tell them what they need to buy.
             if cmdenv.detail:
                 self.note("HOP {} of {}".format(hopNo, lastHopIdx))
             
             self.note("Buy at {}".format(cur.name()))
@@ -340,15 +345,15 @@
                     " -> ".join(jump.name() for jump in jumps[idx])
                 )
             )
             if idx < len(hops) and jumps[idx]:
                 for jump in jumps[idx][1:]:
                     self.doStep('Jump to', jump.name())
             if cmdenv.detail:
-                self.doStep('Dock at', nxt.str())
+                self.doStep('Dock at', nxt.text())
             print()
             
             self.note("Sell at {}".format(nxt.name()))
             for (trade, qty) in sortedTradeOptions:
                 self.doStep(
                         'Sell {:n} x'.format(qty),
                         trade.name(),
@@ -408,17 +413,17 @@
             break
         cmdenv.DEBUG1(
             "Ring {}: {}",
             jump,
             [sys.dbname for sys in origins]
         )
         thisJump, origins = origins, set()
-        for sys in thisJump:
-            avoid.add(sys)
-            for stn in sys.stations or ():
+        for system in thisJump:
+            avoid.add(system)
+            for stn in system.stations or ():
                 if stn.ID not in tradingList:
                     cmdenv.DEBUG2(
                         "X {}/{} not in trading list",
                         stn.system.dbname, stn.dbname,
                     )
                     continue
                 if not checkStationSuitability(cmdenv, calc, stn):
@@ -428,15 +433,15 @@
                     )
                     continue
                 cmdenv.DEBUG2(
                     "- {}/{} meets requirements",
                     stn.system.dbname, stn.dbname,
                 )
                 stations.add(stn)
-            for dest, dist in tdb.genSystemsInRange(sys, maxLyPer):
+            for dest, dist in tdb.genSystemsInRange(system, maxLyPer):
                 if dest not in avoid:
                     origins.add(dest)
     
     cmdenv.DEBUG0(
             "Expanded {} stations: {}",
             srcName,
             [stn.name() for stn in stations]
@@ -458,15 +463,15 @@
                 jumps, "s" if jumps > 1 else "",
                 origin.name(),
                 extra,
             )
         )
     
     stations = list(stations)
-    stations.sort(key = lambda stn: stn.ID)
+    stations.sort(key=lambda stn: stn.ID)
     
     return stations
 
 
 def checkForEmptyStationList(category, focusPlace, stationList, jumps):
     if stationList:
         return
@@ -508,22 +513,23 @@
                 place.name(),
                 anchorName,
         ))
 
 
 def checkStationSuitability(cmdenv, calc, station, src = None):
     cmdenv.DEBUG2(
-        "checking {} (ls={}, bm={}, pad={}, plt={}, flc={}, mkt={}, shp={}) "
+        "checking {} (ls={}, bm={}, pad={}, plt={}, flc={}, ody={}, mkt={}, shp={}) "
         "for {} suitability",
         station.name(),
         station.lsFromStar,
         station.blackMarket,
         station.maxPadSize,
         station.planetary,
         station.fleet,
+        station.odyssey,
         station.market,
         station.shipyard,
         src or "any",
     )
     
     if station in cmdenv.avoidPlaces and src != "--from":
         if src:
@@ -577,36 +583,48 @@
                 "You specified: {}, Current data for station: {} ({})\n"
                 "You can use \"trade.py station\" to correct this.".format(
                     src, station.name(),
                     mps, station.maxPadSize,
                     TradeDB.padSizesExt[station.maxPadSize],
             ))
         return False
+    pla = cmdenv.planetary
+    if pla and not station.checkPlanetary(pla):
+        if src:
+            raise CommandLineError(
+                "{} station {} does not meet planetary requirement.\n"
+                "You specified: {}, Current data for station: {} ({})\n"
+                "You can use \"trade.py station\" to correct this.".format(
+                    src, station.name(),
+                    pla, station.planetary,
+                    TradeDB.planetStatesExt[station.planetary],
+            ))
+        return False
     flc = cmdenv.fleet
     if flc and not station.checkFleet(flc):
         if src:
             raise CommandLineError(
                 "{} station {} does not meet fleet carrier requirement.\n"
                 "You specified: {}, Current data for station: {} ({})\n"
                 "You can use \"trade.py station\" to correct this.".format(
                     src, station.name(),
                     flc, station.fleet,
                     TradeDB.fleetStatesExt[station.fleet],
             ))
         return False
-    pla = cmdenv.planetary
-    if pla and not station.checkPlanetary(pla):
+    ody = cmdenv.odyssey
+    if ody and not station.checkOdyssey(ody):
         if src:
             raise CommandLineError(
-                "{} station {} does not meet planetary requirement.\n"
+                "{} station {} does not meet odyssey requirement.\n"
                 "You specified: {}, Current data for station: {} ({})\n"
                 "You can use \"trade.py station\" to correct this.".format(
                     src, station.name(),
-                    pla, station.planetary,
-                    TradeDB.planetStatesExt[station.planetary],
+                    ody, station.odyssey,
+                    TradeDB.odysseyStatesExt[station.odyssey],
             ))
         return False
     np = cmdenv.noPlanet
     if np and station.planetary != 'N':
         if src and src != "--from":
             raise CommandLineError(
                 "{} station {} does not meet no-planet "
@@ -648,24 +666,20 @@
     if not stnList:
         return stnList
     cmdenv.DEBUG0(
         "filtering {} station list: {}",
         src,
         ",".join(station.name() for station in stnList),
         )
-    filtered = tuple(
+    stnList = tuple(
         place for place in stnList
-        if isinstance(place, System) or \
-            checkStationSuitability(cmdenv, calc, place, src)
+        if isinstance(place, System) or checkStationSuitability(cmdenv, calc, place, src)
     )
     if not stnList:
-        raise CommandLineError(
-                "No {} station met your criteria.".format(
-                    src
-        ))
+        raise CommandLineError("No {src} station met your criteria.")
     return stnList
 
 
 def checkOrigins(tdb, cmdenv, calc):
     if cmdenv.origPlace:
         if cmdenv.startJumps and cmdenv.startJumps > 0:
             cmdenv.origins = expandForJumps(
@@ -805,18 +819,31 @@
     if cmdenv.capacity is None:
         raise CommandLineError("Missing '--capacity'")
     if cmdenv.maxLyPer is None and not cmdenv.direct:
         raise CommandLineError("Missing '--ly-per'")
     if cmdenv.capacity < 0:
         raise CommandLineError("Invalid (negative) cargo capacity")
     if cmdenv.capacity > 1500:
-        raise CommandLineError(
-            "Capacity > 1500 not supported (you specified {})"
-            .format(cmdenv.capacity)
-        )
+        cmdenv.WARN("Capacity > 1500 not supported (you specified {})", cmdenv.capacity)
+        cmdenv.WARN("Forcing jumps per hop to 1.")
+        cmdenv.maxJumpsPer = 1
+        if cmdenv.hops > 2:
+            cmdenv.WARN("{} hops? Press [CTRL][C] to quit.", cmdenv.hops)
+        if not cmdenv.supply:
+            cmdenv.WARN("Please provide a '--supply' value.")
+            cmdenv.supply = cmdenv.capacity * 10
+            cmdenv.DEBUG0("'supply' minimum set to {}.", cmdenv.supply)
+        if not cmdenv.demand:
+            cmdenv.WARN("Please provide a '--demand' value.")
+            cmdenv.demand = cmdenv.capacity * 10
+            cmdenv.DEBUG0("'demand' minimum set to {}.", cmdenv.demand)
+    #    raise CommandLineError(
+    #        "Capacity > 1500 not supported (you specified {})"
+    #        .format(cmdenv.capacity)
+    #    )
     
     if cmdenv.limit and cmdenv.limit > cmdenv.capacity:
         raise CommandLineError("'limit' must be <= capacity")
     if cmdenv.limit and cmdenv.limit < 0:
         raise CommandLineError("'limit' can't be negative, silly")
     cmdenv.maxUnits = cmdenv.limit if cmdenv.limit else cmdenv.capacity
     
@@ -938,17 +965,17 @@
     if cmdenv.unique:
         # if there's only one start and stop...
         if len(origins) == 1 and len(destns) == 1:
             if origins[0] is destns[0]:
                 raise CommandLineError("Can't have same from/to with --unique")
         if viaSet:
             if len(origins) == 1 and origins[0] in viaSet:
-                raise("Can't have --from station in --via list with --unique")
+                raise CommandLineError("Can't have --from station in --via list with --unique")
             if len(destns) == 1 and destns[0] in viaSet:
-                raise("Can't have --to station in --via list with --unique")
+                raise CommandLineError("Can't have --to station in --via list with --unique")
     
     if cmdenv.mfd:
         cmdenv.mfd.display("Loading Trades")
     
     if cmdenv.pruneScores and cmdenv.pruneHops:
         if cmdenv.pruneScores > 99:
             raise CommandLineError("--prune-score value percentile exceed 99.")
@@ -1116,15 +1143,14 @@
     
     # Instantiate the calculator object
     calc = TradeCalc(tdb, cmdenv)
     
     validateRunArguments(tdb, cmdenv, calc)
     
     origPlace, viaSet = cmdenv.origPlace, cmdenv.viaSet
-    avoidPlaces = cmdenv.avoidPlaces
     stopStations = cmdenv.destinations
     goalSystem = cmdenv.goalSystem
     maxLs = cmdenv.maxLs
     
     # seed the route table with starting places
     startCr = cmdenv.credits - cmdenv.insurance
     routes = [
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/commandenv.py` & `tradedangerous-11.0.0/tradedangerous/commands/commandenv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-
-from .exceptions import CommandLineError, PadSizeError, PlanetaryError, FleetCarrierError
-from ..tradedb import AmbiguityError, System, Station
+from .exceptions import (
+    CommandLineError, FleetCarrierError, OdysseyError,
+    PadSizeError, PlanetaryError,
+)
+from ..tradedb import AmbiguityError, Station
 from ..tradeenv import TradeEnv
 
 import os
 import pathlib
 import sys
 
 
-class CommandResults(object):
+class CommandResults:
     """
         Encapsulates the results returned by running a command.
     """
     
     def __init__(self, cmdenv):
         self.cmdenv = cmdenv
         self.summary, self.rows = {}, []
     
     def render(self, cmdenv = None, tdb = None):
         cmdenv = cmdenv or self.cmdenv
         tdb = tdb or cmdenv.tdb
         cmdenv._cmd.render(self, cmdenv, tdb)
 
 
-class ResultRow(object):
+class ResultRow:
     
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
 
 class CommandEnv(TradeEnv):
@@ -42,15 +43,15 @@
         self.tdb = None
         self.mfd = None
         self.argv = argv or sys.argv
         
         if self.detail and self.quiet:
             raise CommandLineError("'--detail' (-v) and '--quiet' (-q) are mutually exclusive.")
         
-        self._cmd = cmdModule or __main__
+        self._cmd = cmdModule or getattr("__main__")
         self.wantsTradeDB = getattr(cmdModule, 'wantsTradeDB', True)
         self.usesTradeData = getattr(cmdModule, 'usesTradeData', False)
         
         # We need to relocate to the working directory so that
         # we can load a TradeDB after this without things going
         # pear-shaped
         if not self.cwd and argv[0]:
@@ -73,14 +74,15 @@
         self.checkMFD()
         self.checkFromToNear()
         self.checkAvoids()
         self.checkVias()
         self.checkPadSize()
         self.checkPlanetary()
         self.checkFleet()
+        self.checkOdyssey()
         
         results = CommandResults(self)
         return self._cmd.run(results, self, tdb)
     
     def render(self, results):
         self._cmd.render(self, results, self, self.tdb)
     
@@ -182,15 +184,15 @@
             
             # If it was none of the above, whine about it
             if not (item or place):
                 raise CommandLineError("Unknown item/system/station: {}".format(avoid))
             
             # But if it matched more than once, whine about ambiguity
             if item and place:
-                raise AmbiguityError('Avoidance', avoid, [ item, place.str() ])
+                raise AmbiguityError('Avoidance', avoid, [ item, place.text() ])
         
         self.DEBUG0("Avoiding items {}, places {}",
                     [ item.name() for item in avoidItems ],
                     [ place.name() for place in avoidPlaces ],
         )
     
     def checkVias(self):
@@ -208,45 +210,58 @@
             return
         padSize = ''.join(sorted(list(set(padSize)))).upper()
         if padSize == '?LMS':
             self.padSize = None
             return
         self.padSize = padSize = padSize.upper()
         for value in padSize:
-            if not value in 'SML?':
+            if value not in 'SML?':
                 raise PadSizeError(padSize)
         self.padSize = padSize
     
     def checkPlanetary(self):
         planetary = getattr(self, 'planetary', None)
         if not planetary:
             return
         planetary = ''.join(sorted(list(set(planetary)))).upper()
         if planetary == '?NY':
             self.planetary = None
             return
         self.planetary = planetary = planetary.upper()
         for value in planetary:
-            if not value in 'YN?':
+            if value not in 'YN?':
                 raise PlanetaryError(planetary)
         self.planetary = planetary
     
     def checkFleet(self):
         fleet = getattr(self, 'fleet', None)
         if not fleet:
             return
         fleet = ''.join(sorted(list(set(fleet)))).upper()
         for value in fleet:
-            if not value in 'YN?':
-                raise FleetError(fleet)
+            if value not in 'YN?':
+                raise FleetCarrierError(fleet)
         if fleet == '?NY':
             self.fleet = None
             return
         self.fleet = fleet = fleet.upper()
     
+    def checkOdyssey(self):
+        odyssey = getattr(self, 'odyssey', None)
+        if not odyssey:
+            return
+        odyssey = ''.join(sorted(list(set(odyssey)))).upper()
+        for value in odyssey:
+            if value not in 'YN?':
+                raise OdysseyError(odyssey)
+        if odyssey == '?NY':
+            self.odyssey = None
+            return
+        self.odyssey = odyssey.upper()
+    
     def colorize(self, color, rawText):
         """
         Set up some coloring for readability
         """
         colorMap = {
             "red": "31",
             "green": "32",
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/parsing.py` & `tradedangerous-11.0.0/tradedangerous/commands/parsing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-from .exceptions import PadSizeError, PlanetaryError, FleetCarrierError
+from .exceptions import (
+    FleetCarrierError, OdysseyError, PadSizeError, PlanetaryError,
+)
 
 ######################################################################
 # Parsing Helpers
 
-class ParseArgument(object):
+class ParseArgument:
     """
         Provides argument forwarding so that 'makeSubParser' can take function-like arguments.
     """
     def __init__(self, *args, **kwargs):
         self.args, self.kwargs = args, kwargs
 
 
-class MutuallyExclusiveGroup(object):
+class MutuallyExclusiveGroup:
     def __init__(self, *args):
         self.arguments = list(args)
 
 
 ######################################################################
 # Derived Parsers
 
 
 class CreditParser(int):
     """
     argparse helper for parsing numeric prefixes, i.e.
-    'k' for thousand, 'm' for million and 'b' for billion.
+    'k' for thousands, 'm' for millions and 'b' for billions.
     """
     suffixes = {'k': 10**3, 'm': 10**6, 'b': 10**9}
+
     def __new__(cls, val, **kwargs):
         if isinstance(val, str):
             if val[-1] in CreditParser.suffixes:
                 val = int(float(val[:-1]) * CreditParser.suffixes[val[-1]])
         return super().__new__(cls, val, **kwargs)
 
 
@@ -78,15 +80,15 @@
 class SwitchArgument(ParseArgument):
     def __init__(self, help=None):
         if isinstance(self.switches, (tuple, list)):
             self.args = self.switches
         else:
             self.args = (self.switches,)
         help = help or self.help
-        self.kwargs = {'action':'store_true', 'dest':self.dest, 'help':help}
+        self.kwargs = {'action': 'store_true', 'dest': self.dest, 'help': help}
 
 
 class BlackMarketSwitch(SwitchArgument):
     switches = ['--black-market', '--bm']
     dest = 'blackMarket'
     help = 'Require stations known to have a black market.'
 
@@ -178,18 +180,46 @@
             ),
             'dest': 'fleet',
             'metavar': 'FLEET',
             'type': 'fleet',
             'choices': 'YN?',
         }
 
+class OdysseyArgument(int):
+    """
+    argparse helper for --odyssey
+    """
+    class OdysseyParser(str):
+        def __new__(cls, val, **kwargs):
+            if not isinstance(val, str):
+                raise OdysseyError(val)
+            for v in val:
+                if "YN?".find(v.upper()) < 0:
+                    raise OdysseyError(val.upper())
+            return super().__new__(cls, val, **kwargs)
+    
+    def __init__(self):
+        self.args = ['--odyssey', '--od']
+        self.kwargs = {
+            'help': (
+                'Limit to stations with one of the specified odyssey, '
+                'e.g. --od YN? matches any station, --od Y matches only '
+                'odyssey stations.'
+            ),
+            'dest': 'odyssey',
+            'metavar': 'ODYSSEY',
+            'type': 'odyssey',
+            'choices': 'YN?',
+        }
+
 
 __tdParserHelpers = {
     'credits': CreditParser,
     'padsize': PadSizeArgument.PadSizeParser,
     'planetary': PlanetaryArgument.PlanetaryParser,
     'fleet': FleetCarrierArgument.FleetCarrierParser,
+    'odyssey': OdysseyArgument.OdysseyParser,
 }
 
 def registerParserHelpers(into):
     for typeName, helper in __tdParserHelpers.items():
         into.register('type', typeName, helper)
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/__init__.py` & `tradedangerous-11.0.0/tradedangerous/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 from .commandenv import CommandEnv
 from textwrap import TextWrapper
 
 import argparse  # For parsing command line args.
-import importlib
 import os
 import pathlib
 import sys
 
 thismodule = sys.modules[__name__]
 from . import exceptions
 from . import parsing
@@ -59,15 +57,15 @@
     """
     for option in options:
         if isinstance(option, parsing.MutuallyExclusiveGroup):
             exGrp = (topGroup or group).add_mutually_exclusive_group()
             parsing.registerParserHelpers(exGrp)
             addArguments(exGrp, option.arguments, required, topGroup = group)
         else:
-            assert not required in option.kwargs
+            assert required not in option.kwargs
             if option.args[0][0] == '-':
                 group.add_argument(*(option.args), required = required, **(option.kwargs))
             else:
                 if required:
                     group.add_argument(*(option.args), **(option.kwargs))
                 else:
                     group.add_argument(*(option.args), nargs = '?', **(option.kwargs))
@@ -80,15 +78,15 @@
         for dirname in '.', os.path.expanduser('~'):
             cmdPath = pathlib.Path(dirname) / filename
             if cmdPath.exists():
                 return cmdPath.resolve()
     return None
 
 
-class CommandIndex(object):
+class CommandIndex:
     
     def usage(self, argv):
         """
             Generate the outlying usage text for TD.
             This tells the user the list of current
             commands, generated programatically,
             and the outlying command functionality.
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/rares_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/rares_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 from .commandenv import ResultRow
-from .exceptions import *
-from .parsing import *
-from ..formatting import RowFormat, ColumnFormat, max_len
+from .exceptions import CommandLineError
+from .parsing import (
+    PadSizeArgument, ParseArgument, MutuallyExclusiveGroup, NoPlanetSwitch,
+    PlanetaryArgument, FleetCarrierArgument, OdysseyArgument,
+)
+from ..formatting import RowFormat, max_len
 from ..tradedb import TradeDB
 
-import math
 
 ######################################################################
 # Parser config
 
 # Displayed on the "trade.py --help" command list, etc.
 help='Find rares near your current local.'
 # Should match the name of the module minus the _cmd.py
@@ -44,28 +45,28 @@
     ),
     PadSizeArgument(),
     MutuallyExclusiveGroup(
         NoPlanetSwitch(),
         PlanetaryArgument(),
     ),
     FleetCarrierArgument(),
+    OdysseyArgument(),
     ParseArgument('--price-sort', '-P',
             help='Sort by price not distance.',
             action='store_true',
             default=False,
             dest='sortByPrice',
     ),
     ParseArgument('--reverse', '-r',
             help='Reverse the list.',
             action='store_true',
             default=False,
     ),
     ParseArgument('--away',
-            help='Require "--from" systems to be at least this far ' \
-                    'from primary system',
+            help='Require "--from" systems to be at least this far from primary system',
             metavar='LY',
             default=0,
             type=float,
     ),
     MutuallyExclusiveGroup(
         ParseArgument('--legal',
             help='List only items known to be legal.',
@@ -73,16 +74,15 @@
         ),
         ParseArgument('--illegal',
             help='List only items known to be illegal.',
             action='store_true',
         )
     ),
     ParseArgument('--from',
-            help='Additional systems to range check candidates against, ' \
-                    'requires --away.',
+            help='Additional systems to range check candidates against, requires --away.',
             metavar='SYSTEMNAME',
             action='append',
             dest='awayFrom',
     ),
 ]
 
 ######################################################################
@@ -128,14 +128,15 @@
     # Lookup the system we're currently in.
     start = cmdenv.nearSystem
     # Hoist the padSize, noPlanet and planetary parameter for convenience
     padSize = cmdenv.padSize
     noPlanet = cmdenv.noPlanet
     planetary = cmdenv.planetary
     fleet = cmdenv.fleet
+    odyssey = cmdenv.odyssey
     # How far we're want to cast our net.
     maxLy = float(cmdenv.maxLyPer or 0.)
     
     if cmdenv.illegal:
         wantIllegality = 'Y'
     elif cmdenv.legal:
         wantIllegality = 'N'
@@ -159,24 +160,27 @@
     results.summary.ly = maxLy
     results.summary.awaySystems = awaySystems
     
     distCheckFn = start.distanceTo
     
     # Look through the rares list.
     for rare in tdb.rareItemByID.values():
-        if not rare.illegal in wantIllegality:
+        if rare.illegal not in wantIllegality:
             continue
         if padSize:       # do we care about pad size?
             if not rare.station.checkPadSize(padSize):
                 continue
+        if planetary:     # do we care about planetary?
+            if not rare.station.checkPlanetary(planetary):
+                continue
         if fleet:         # do we care about fleet carrier?
             if not rare.station.checkFleet(fleet):
                 continue
-        if planetary:     # do we care about planetary?
-            if not rare.station.checkPlanetary(planetary):
+        if odyssey:         # do we care about Odyssey?
+            if not rare.station.checkOdyssey(odyssey):
                 continue
         if noPlanet and rare.station.planetary != 'N':
             continue
         rareSys = rare.station.system
         # Find the un-sqrt'd distance to the system.
         dist = distCheckFn(rareSys)
         if maxLy > 0. and dist > maxLy:
@@ -252,14 +256,16 @@
             key=lambda row: TradeDB.marketStates[row.rare.station.blackMarket])
     rowFmt.addColumn("Pad", '>', '3',
             key=lambda row: TradeDB.padSizes[row.rare.station.maxPadSize])
     rowFmt.addColumn("Plt", '>', '3',
             key=lambda row: TradeDB.planetStates[row.rare.station.planetary])
     rowFmt.addColumn("Flc", '>', '3',
             key=lambda row: TradeDB.fleetStates[row.rare.station.fleet])
+    rowFmt.addColumn("Ody", '>', '3',
+            key=lambda row: TradeDB.odysseyStates[row.rare.station.odyssey])
     
     # Print a heading summary if the user didn't use '-q'
     if not cmdenv.quiet:
         heading, underline = rowFmt.heading()
         print(heading, underline, sep='\n')
     
     # Print out our results.
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/market_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/market_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 from .commandenv import ResultRow
-from .exceptions import *
-from .parsing import *
-from ..formatting import RowFormat, ColumnFormat
-from ..tradedb import TradeDB
+from .exceptions import CommandLineError
+from .parsing import (
+    ParseArgument, MutuallyExclusiveGroup,
+)
+from ..formatting import RowFormat
+
 
 ######################################################################
 # Parser config
 
 help='Lists items bought/sold at a given station.'
 name='market'
 epilog=None
@@ -125,16 +126,16 @@
     
     showCategories = (cmdenv.detail > 0)
     
     rowFmt = RowFormat()
     if showCategories:
         rowFmt.prefix = '    '
     
-    sellPred = lambda row: row.sellCr != 0 and row.supply != '-'
-    buyPred = lambda row: row.buyCr != 0 and row.demand != '-'
+    sellPred = lambda row: row.sellCr != 0 and row.supply != '-'    # noqa: E731
+    buyPred = lambda row: row.buyCr != 0 and row.demand != '-'      # noqa: E731
     
     rowFmt.addColumn('Item', '<', longestLen,
             key=lambda row: row.item.name())
     if not cmdenv.selling:
         rowFmt.addColumn('Buying', '>', 7, 'n',
             key=lambda row: row.buyCr,
             pred=buyPred)
@@ -166,8 +167,8 @@
         print(heading, underline, sep='\n')
     
     lastCat = None
     for row in results.rows:
         if showCategories and row.item.category is not lastCat:
             print("+{}".format(row.item.category.name()))
             lastCat = row.item.category
-        print(rowFmt.format(row))
+        print(rowFmt.format(row))
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/local_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/local_cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 from .commandenv import ResultRow
-from .parsing import *
+from .parsing import (
+    ParseArgument, PadSizeArgument, MutuallyExclusiveGroup, NoPlanetSwitch,
+    PlanetaryArgument, FleetCarrierArgument, OdysseyArgument, BlackMarketSwitch,
+    ShipyardSwitch, OutfittingSwitch, RearmSwitch, RefuelSwitch, RepairSwitch,
+)
 from ..formatting import RowFormat, ColumnFormat, max_len
 from itertools import chain
 from ..tradedb import TradeDB
 from ..tradeexcept import TradeException
 
-import math
 
 ######################################################################
 # Parser config
 
 name='local'
 help='Calculate local systems.'
 epilog="See also the 'station' sub-command."
@@ -33,14 +35,15 @@
     ),
     PadSizeArgument(),
     MutuallyExclusiveGroup(
         NoPlanetSwitch(),
         PlanetaryArgument(),
     ),
     FleetCarrierArgument(),
+    OdysseyArgument(),
     ParseArgument('--stations',
             help='Limit to systems which have stations.',
             action='store_true',
     ),
     ParseArgument('--trading',
             help='Limit stations to ones with price data or flagged as having '
                  'a market.',
@@ -76,16 +79,17 @@
     # Calculate the bounding dimensions
     for destSys, dist in tdb.genSystemsInRange(srcSystem, ly):
         distances[destSys] = dist
     
     showStations = cmdenv.detail
     wantStations = cmdenv.stations
     padSize = cmdenv.padSize
-    fleet = cmdenv.fleet
     planetary = cmdenv.planetary
+    fleet = cmdenv.fleet
+    odyssey = cmdenv.odyssey
     wantNoPlanet = cmdenv.noPlanet
     wantTrading = cmdenv.trading
     wantShipYard = cmdenv.shipyard
     wantBlackMarket = cmdenv.blackMarket
     wantOutfitting = cmdenv.outfitting
     wantRearm = cmdenv.rearm
     wantRefuel = cmdenv.refuel
@@ -99,17 +103,19 @@
                 continue
             if wantBlackMarket and station.blackMarket != 'Y':
                 continue
             if wantShipYard and station.shipyard != 'Y':
                 continue
             if padSize and not station.checkPadSize(padSize):
                 continue
+            if planetary and not station.checkPlanetary(planetary):
+                continue
             if fleet and not station.checkFleet(fleet):
                 continue
-            if planetary and not station.checkPlanetary(planetary):
+            if odyssey and not station.checkOdyssey(odyssey):
                 continue
             if wantOutfitting and station.outfitting != 'Y':
                 continue
             if wantRearm and station.rearm != 'Y':
                 continue
             if wantRefuel and station.refuel != 'Y':
                 continue
@@ -178,52 +184,45 @@
                 ColumnFormat("StnLs", '>', maxLsLen,
                     key=lambda row: row.station.distFromStar())
         ).append(
                 ColumnFormat("Age/days", '>', 7,
                         key=lambda row: row.age)
         ).append(
                 ColumnFormat("Mkt", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.market])
+                    key=lambda row: TradeDB.marketStates[row.station.market])
         ).append(
                 ColumnFormat("BMk", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.blackMarket])
+                    key=lambda row: TradeDB.marketStates[row.station.blackMarket])
         ).append(
                 ColumnFormat("Shp", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.shipyard])
+                    key=lambda row: TradeDB.marketStates[row.station.shipyard])
         ).append(
                 ColumnFormat("Out", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.outfitting])
+                    key=lambda row: TradeDB.marketStates[row.station.outfitting])
         ).append(
                 ColumnFormat("Arm", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.rearm])
+                    key=lambda row: TradeDB.marketStates[row.station.rearm])
         ).append(
                 ColumnFormat("Ref", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.refuel])
+                    key=lambda row: TradeDB.marketStates[row.station.refuel])
         ).append(
                 ColumnFormat("Rep", '>', '3',
-                    key=lambda row: \
-                        TradeDB.marketStates[row.station.repair])
+                    key=lambda row: TradeDB.marketStates[row.station.repair])
         ).append(
                 ColumnFormat("Pad", '>', '3',
-                    key=lambda row: \
-                        TradeDB.padSizes[row.station.maxPadSize])
+                    key=lambda row: TradeDB.padSizes[row.station.maxPadSize])
         ).append(
                 ColumnFormat("Plt", '>', '3',
-                    key=lambda row: \
-                        TradeDB.planetStates[row.station.planetary])
+                    key=lambda row: TradeDB.planetStates[row.station.planetary])
         ).append(
                 ColumnFormat("Flc", '>', '3',
-                    key=lambda row: \
-                        TradeDB.fleetStates[row.station.fleet])
+                    key=lambda row: TradeDB.fleetStates[row.station.fleet])
+        ).append(
+                ColumnFormat("Ody", '>', '3',
+                    key=lambda row: TradeDB.odysseyStates[row.station.odyssey])
         )
         if cmdenv.detail > 1:
             stnRowFmt.append(
                 ColumnFormat("Itms", ">", 4,
                     key=lambda row: row.station.itemCount)
             )
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/sell_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/sell_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-from .exceptions import *
-from .parsing import *
+from .commandenv import ResultRow
+from .exceptions import CommandLineError, NoDataError
+from .parsing import (
+    AvoidPlacesArgument, BlackMarketSwitch, FleetCarrierArgument,
+    MutuallyExclusiveGroup, NoPlanetSwitch, OdysseyArgument,
+    PadSizeArgument, ParseArgument, PlanetaryArgument,
+)
 from ..tradedb import TradeDB, System, Station
+from ..formatting import RowFormat
 
-import math
 
 ######################################################################
 # Parser config
 
 help='Find places to sell a given item within range of a given station.'
 name='sell'
 epilog=None
@@ -36,14 +40,15 @@
     AvoidPlacesArgument(),
     PadSizeArgument(),
     MutuallyExclusiveGroup(
         NoPlanetSwitch(),
         PlanetaryArgument(),
     ),
     FleetCarrierArgument(),
+    OdysseyArgument(),
     BlackMarketSwitch(),
     ParseArgument('--limit',
             help='Maximum number of results to list.',
             default=None,
             type=int,
     ),
     ParseArgument('--price-sort', '-P',
@@ -65,17 +70,15 @@
             type="credits",
     ),
 ]
 
 ######################################################################
 # Perform query and populate result set
 
-def run(results, cmdenv, tdb):
-    from .commandenv import ResultRow
-    
+def run(results, cmdenv, tdb: TradeDB):
     if cmdenv.lt and cmdenv.gt:
         if cmdenv.lt <= cmdenv.gt:
             raise CommandLineError("--gt must be lower than --lt")
     
     item = tdb.lookupItem(cmdenv.item)
     cmdenv.DEBUG0("Looking up item {} (#{})", item.name(), item.ID)
     
@@ -136,24 +139,27 @@
     cmdenv.DEBUG0('SQL: {}', stmt)
     cur = tdb.query(stmt, bindValues)
     
     stationByID = tdb.stationByID
     padSize = cmdenv.padSize
     planetary = cmdenv.planetary
     fleet = cmdenv.fleet
+    odyssey = cmdenv.odyssey
     wantNoPlanet = cmdenv.noPlanet
     wantBlackMarket = cmdenv.blackMarket
     
     for (stationID, priceCr, demand) in cur:
         station = stationByID[stationID]
         if padSize and not station.checkPadSize(padSize):
             continue
+        if planetary and not station.checkPlanetary(planetary):
+            continue
         if fleet and not station.checkFleet(fleet):
             continue
-        if planetary and not station.checkPlanetary(planetary):
+        if odyssey and not station.checkOdyssey(odyssey):
             continue
         if wantNoPlanet and station.planetary != 'N':
             continue
         if wantBlackMarket and station.blackMarket != 'Y':
             continue
         if station in avoidStations:
             continue
@@ -168,14 +174,16 @@
                 continue
             row.dist = distance
         row.price = priceCr
         row.demand = demand
         row.age = station.itemDataAgeStr
         results.rows.append(row)
     
+    cur.close()
+    
     if not results.rows:
         raise NoDataError("No available items found")
     
     results.summary.sort = "Price"
     results.rows.sort(key=lambda result: result.demand, reverse=True)
     results.rows.sort(key=lambda result: result.price, reverse=True)
     if nearSystem and not cmdenv.sortByPrice:
@@ -189,16 +197,14 @@
     return results
 
 
 #######################################################################
 ## Transform result set into output
 
 def render(results, cmdenv, tdb):
-    from ..formatting import RowFormat, ColumnFormat
-    
     longestNamed = max(results.rows, key=lambda result: len(result.station.name()))
     longestNameLen = len(longestNamed.station.name())
     
     stnRowFmt = RowFormat()
     stnRowFmt.addColumn('Station', '<', longestNameLen,
             key=lambda row: row.station.name())
     stnRowFmt.addColumn('Cost', '>', 10, 'n',
@@ -218,14 +224,16 @@
             key=lambda row: TradeDB.marketStates[row.station.blackMarket])
     stnRowFmt.addColumn("Pad", '>', '3',
             key=lambda row: TradeDB.padSizes[row.station.maxPadSize])
     stnRowFmt.addColumn("Plt", '>', '3',
             key=lambda row: TradeDB.planetStates[row.station.planetary])
     stnRowFmt.addColumn("Flc", '>', '3',
             key=lambda row: TradeDB.fleetStates[row.station.fleet])
+    stnRowFmt.addColumn("Ody", '>', '3',
+            key=lambda row: TradeDB.odysseyStates[row.station.odyssey])
     
     if not cmdenv.quiet:
         heading, underline = stnRowFmt.heading()
         print(heading, underline, sep='\n')
     
     for row in results.rows:
         print(stnRowFmt.format(row))
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/update_gui.py` & `tradedangerous-11.0.0/tradedangerous/commands/update_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import tkinter as tk
 import tkinter.messagebox as mbox
-import tkinter.ttk as ttk
 import sqlite3
 import re
-from pathlib import Path
 
 """
 This is a crude attempt at a GUI for updating trade prices.
 It needs a lot of love to be less... Shitty.
 
 TODO:
 . Add a way to add a new line,
@@ -40,15 +38,15 @@
 "SAVING:\n"
 "To save your data, click one of the window's close buttons.\n"
 "\n"
 "NAVIGATION:\n"
 "- Use Tab, Shift-Tab, Up/Down Arrow and Enter to navigate.\n"
 )
 
-class Item(object):
+class Item:
     """ Describe a listed, tradeable item """
     
     def __init__(self, ID, catID, name, displayNo):
         self.ID, self.catID, self.name = ID, catID, name
         self.displayNo = displayNo
 
 
@@ -691,15 +689,15 @@
                 if paying and not demand:
                     demand = "?"
                 
                 if asking == 0:
                     supply = "-"
                 elif not supply:
                     supply = "?"
-                elif re.match('^\d+$', supply):
+                elif re.match(r"^\d+$", supply):
                     if int(supply) != 0:
                         supply += '?'
             
             txt += ("     {item:<30s} "
                     "{paying:>10} "
                     "{asking:>10} "
                     "{demand:>10} "
```

### Comparing `tradedangerous-10.9.8/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-11.0.0/tradedangerous/commands/shipvendor_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 from .commandenv import ResultRow
 from .exceptions import CommandLineError
-from .parsing import *
+from .parsing import MutuallyExclusiveGroup, ParseArgument
 from ..formatting import RowFormat, ColumnFormat, max_len
 from itertools import chain
-from ..tradedb import AmbiguityError
-from ..tradedb import System, Station
-from ..tradedb import TradeDB
+from ..tradedb import Station
 
 # Original by Dirk Wilhelm
 
 from .. import csvexport
-import re
-import sys
 
 ######################################################################
 # Parser config
 
 help = 'List, add or update available ships to a station'
 name = 'shipvendor'
 epilog = None
@@ -207,14 +202,16 @@
         return None
     
     # We've checked that everything should be good.
     dataToExport = False
     for ship in ships.values():
         if action(tdb, cmdenv, station, ship):
             dataToExport = True
+
+    cmdenv.DEBUG0("dataToExport = {}", dataToExport)
     
     maybeExportToCSV(tdb, cmdenv)
     
     return None
 
 ######################################################################
 # Transform result set into output
```

### Comparing `tradedangerous-10.9.8/tradedangerous/gui.py` & `tradedangerous-11.0.0/tradedangerous/gui.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,99 @@
+#!/usr/bin/env python3
 # --------------------------------------------------------------------
-# Copyright (C) Oliver 'kfsone' Smith 2014 <oliver@kfs.org>:
-# Copyright (C) Bernd 'Gazelle' Gollesch 2016, 2017
-# Copyright (C) Jonathan 'eyeonus' Jones 2018, 2019
+# Copyright (C) Jonathan 'eyeonus' Jones 2018-2022
 #
 # You are free to use, redistribute, or even print and eat a copy of
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
-# TradeDangerous :: Command Line App :: Main Module
-#
-# TradeDangerous is a powerful set of tools for traders in Frontier
-# Development's game "Elite: Dangerous". It's main function is
-# calculating the most profitable trades between either individual
-# stations or working out "profit runs".
-#
-# I wrote TD because I realized that the best trade run - in terms
-# of the "average profit per stop" was rarely as simple as going
-# Chango -> Dahan -> Chango.
-#
-# E:D's economy is complex; sometimes you can make the most profit
-# by trading one item A->B and flying a second item B->A.
-# But more often you need to fly multiple stations, especially since
-# as you are making money different trade options are coming into
-# your affordable range.
-#
-# END USERS: If you are a user looking to find out how to use TD,
-# please consult the file "README.md".
-#
-# DEVELOPERS: If you are a programmer who wants TD to do something
-# cool, please see the TradeDB and TradeCalc modules. TD is designed
-# to empower other programmers to do cool stuff.
-
-from __future__ import absolute_import
-from __future__ import with_statement
-from __future__ import print_function
-from __future__ import division
-from __future__ import unicode_literals
+# TradeDangerous :: GUI App :: Main Module
+# 
+# Where all the graphics happens. Uses TD CLI under the hood.
+# 
+# Current features:
+# ----------------
+# Drop-down list of all available TD commands
+# Fully populated list of all arguments and switches for each command
+# Automatic setting of default value for the above which have one
+# Procedural generation of all above for future proofing in the 
+#   event of new import plugins, switches, arguments, commands(?)
+# RAM resident save-state: altered values retain new value while main
+#    window remains open
+# 
+# Planned features:
+# ----------------
+# Code overhaul to utilize tk directly rather than via appJar
+# User-defined initial values AKA tdrc files (.tdrc_run, .tdrc_trade, ..)
+# Profiles AKA fromfiles (+ship1, +ship2, ..)
+# Select-able output text
+# graphical render of results
+# send results to new window
+# individual always-on-top for every window
+# Data retrieval from CMDR's journal
+
 import os
 import sys
 import traceback
 import threading
 
 from pathlib import Path
+
 from appJar import gui
 import appJar
+
+# from tkinter import *
+# import tkinter.font as font
+# import tkinter.scrolledtext as scrolledtext
+# from tkinter.ttk import *
+
 from . import commands
 from . import plugins
 from .commands import exceptions
 from .version import __version__
 
 from . import tradedb
 from .plugins import PluginException
 
+# ==================
+# BEGIN appJar fixes
+# ==================
+
 WIDGET_NAMES = appJar.appjar.WIDGET_NAMES
 WidgetManager = appJar.appjar.WidgetManager
-# Plugins available to the 'import' command are stored here.
-# The list is populated by scanning the plugin folder directly,
-# so it updates automagically at start as plugins are added or removed.
-#
-# Any other command with available plugins must have a similar list.
-importPlugs = [ plug.name[0:plug.name.find('_plug.py')]
-             for plug in os.scandir(sys.modules['tradedangerous.plugins'].__path__[0])
-             if plug.name.endswith("_plug.py")
-             ]
-
 
 def get(self, widgetType, title):
     return eval('self.get' + str(widgetType) + '("' + str(title) + '")')
 
 
 gui.get = get
 
-
 # @Override
-def _populateSpinBox(self, spin, vals, reverse = True):
+def _populateSpinBox(self, spin, vals, reverse = False):
     # make sure it's a list
-    #  reverse it, so the spin box functions properly
-    # if reverse:
-    #    vals = list(vals)
-    #    vals.reverse()
+    if reverse:
+        vals = list(vals)
+        vals.reverse()
     vals = tuple(vals)
     spin.config(values = vals)
 
 
 gui._populateSpinBox = _populateSpinBox
 
 
 # @Override
 def setSpinBoxPos(self, title, pos, callFunction = True):
     spin = self.widgetManager.get(WIDGET_NAMES.SpinBox, title)
     vals = spin.cget("values")  # .split()
     vals = self._getSpinBoxValsAsList(vals)
     pos = int(pos)
     if pos < 0 or pos >= len(vals):
-        raise Exception("Invalid position: " + str(pos) + ". No position in SpinBox: " + 
-                    title + "=" + str(vals))
+        raise RuntimeError(
+            f"Invalid position: {pos}. No position in SpinBox: {title}={vals}"
+        )
     #    pos = len(vals) - 1 - pos
     val = vals[pos]
     self._setSpinBoxVal(spin, val, callFunction)
 
 
 gui.setSpinBoxPos = setSpinBoxPos
 
@@ -133,18 +128,18 @@
 #            newOptions.append(item)
 #    
 #    options = newOptions
     
     # get the longest string length
     try:
         maxSize = len(str(max(options, key = len)))
-    except:
+    except:  # noqa: E722
         try:
             maxSize = len(str(max(options)))
-        except:
+        except:  # noqa: E722
             maxSize = 0
     
     # increase if ticks
     if kind == "ticks":
         if len(title) > maxSize:
             maxSize = len(title)
     
@@ -179,49 +174,331 @@
 #        if val.startswith("-") or len(val) == 0:
 #            val = None
         return val
 
 
 gui.getOptionBox = getOptionBox
 
+# ================
+# END appJar fixes
+# ================
 
-def main(argv = None):
-    
-    class IORedirector(object):
-        
-        def __init__(self, TEXT_INFO):
-            self.TEXT_INFO = TEXT_INFO
-    
-    class StdoutRedirector(IORedirector):
+
+
+# Plugins available to the 'import' command are stored here.
+# The list is populated by scanning the plugin folder directly,
+# so it updates automagically at start as plugins are added or removed.
+#
+# Any other command with available plugins must have a similar list.
+importPlugs = [ plug.name[0:plug.name.find('_plug.py')]
+             for plug in os.scandir(sys.modules['tradedangerous.plugins'].__path__[0])
+             if plug.name.endswith("_plug.py")
+             ]
+
+widgets = dict()
+
+# All available commands
+Commands = ['help'] + [ cmd for cmd, module in sorted(commands.commandIndex.items()) ]
+# Used to run TD cli commands.
+cmdenv = commands.CommandIndex().parse
+# 'help' output, required & optional arguments, for each command
+cmdHelp = {}
+
+# Path of the database
+dbS = str(Path((os.environ.get('TD_DATA') or os.path.join(os.getcwd(), 'data')) / Path('TradeDangerous.db')))
+# Path of the current working directory
+cwdS = str(Path(os.getcwd()))
+
+def changeCWD():
+    """
+    Opens a folder select dialog for choosing the current working directory.
+    """
+    cwd = filedialog.askdirectory(title = "Select the top-level folder for TD to work in...",
+                                  initialdir = argVals['--cwd'])
+    # cwd = win.directoryBox("Select the top-level folder for TD to work in...", dirName = argVals['--cwd'])
+    if cwd:
+        argVals['--cwd'] = str(Path(cwd))
+    widgets['cwd']['text'] = argVals['--cwd']
+
+def changeDB():
+    """
+    Opens a file select dialog for choosing the database file.
+    """
+    db = filedialog.askopenfilename(title = "Select the TD database file to use...",
+                                    initialdir = str(Path(argVals['--db']).parent),
+                                    filetypes = [('Data Base File', '*.db')])
+    if db:
+        argVals['--db'] = str(Path(db))
+    widgets['db']['text'] = argVals['--db']        
+
+
+# A dict of all arguments in TD (mostly auto-generated)
+# Manually add the global arguments for now, maybe figure out how to auto-populate them as well.
+allArgs = {
+    '--debug': { 'help': 'Enable/raise level of diagnostic output.',
+                'default':  0, 'required': False, 'action': 'count',
+                'widget': {'type':'combo', 'values': ['', '-w', '-ww', '-www']}
+                },
+    '--detail':{ 'help': 'Increase level of detail in output.',
+                'default': 0, 'required': False, 'action': 'count',
+                'excludes': ['--quiet'], 'widget': {'type':'combo', 'values': ['', '-v', '-vv', '-vvv']}
+                },
+    '--quiet':{ 'help': 'Reduce level of detail in output.',
+               'default': 0, 'required': False, 'action': 'count',
+               'excludes': ['--detail'], 'widget': {'type':'combo', 'values': ['', '-q', '-qq', '-qqq']}
+               },
+    '--db':{ 'help': 'Specify location of the SQLite database.',
+            'default': dbS, 'dest': 'dbFilename', 'type': str,
+            'widget': {'type':'button', 'func':changeDB}
+            },
+    '--cwd':{ 'help': 'Change the working directory file accesses are made from.',
+             'default': cwdS, 'type': str, 'required': False,
+             'widget': {'type':'button', 'func':changeCWD}
+             },
+    '--link-ly':{ 'help': 'Maximum lightyears between systems to be considered linked.',
+                 'default': '30',
+                 'widget': {'type':'entry', 'sub':'numeric'}
+                 }
+    }
+
+# Used to save the value of the arguments.
+argVals = {'--debug': '',
+           '--detail': '',
+           '--quiet': '',
+           '--db': dbS,
+           '--cwd': cwdS,
+           '--link-ly': '30'
+           }
+
+def buildArgDicts():
+    """
+    Procedurally generates the contents of allArgs and argVals
+    """
+    try:
+        cmdenv(['help'])
+    except exceptions.UsageError as e:
+        cmdHelp['help'] = str(e)
+    for cmd in Commands:
+        # print(cmd)
+        if cmd == 'help':
+            continue
+        try:
+            cmdenv(['trade', cmd, '-h'])
+        except exceptions.UsageError as e:
+            cmdHelp[cmd] = str(e)
+        index = commands.commandIndex[cmd]
         
-        def write(self, string):
-            self.TEXT_INFO.config(text = self.TEXT_INFO.cget('text').rsplit('\r', 1)[0] + string)
+        allArgs[cmd] = {'req': {}, 'opt': {}}
+        if index.arguments:
+            for arg in index.arguments:
+                # print(arg.args[0])
+                argVals[arg.args[0]] = arg.kwargs.get('default') or None
+                
+                allArgs[cmd]['req'][arg.args[0]] = {kwarg: arg.kwargs[kwarg] for kwarg in arg.kwargs}
+                allArgs[cmd]['req'][arg.args[0]]['widget'] = chooseType(arg)
+        # print(allArgs[cmd]['req'])
         
-        def flush(self):
-            
-            sys.__stdout__.flush()
+        if index.switches:
+            for arg in index.switches:
+                try:
+                    argVals[arg.args[0]] = arg.kwargs.get('default') or None
+                    
+                    allArgs[cmd]['opt'][arg.args[0]] = {kwarg: arg.kwargs[kwarg] for kwarg in arg.kwargs}
+                    allArgs[cmd]['opt'][arg.args[0]]['widget'] = chooseType(arg)
+                    
+                    if arg.args[0] == '--option':
+                        # Currently only the 'import' cmd has the '--plug' option,
+                        # but this could no longer be the case in future.
+                        if cmd == 'import':
+                            plugOptions = {
+                                plug: plugins.load(cmdenv(['trade', cmd, '--plug', plug, '-O', 'help']).plug,
+                                                    "ImportPlugin").pluginOptions for plug in importPlugs
+                                }
+                            allArgs[cmd]['opt'][arg.args[0]]['options'] = plugOptions
+                
+                except AttributeError:
+                    for argGrp in arg.arguments:
+                        argVals[argGrp.args[0]] = argGrp.kwargs.get('default') or None
+                        
+                        allArgs[cmd]['opt'][argGrp.args[0]] = {kwarg: argGrp.kwargs[kwarg] for kwarg in argGrp.kwargs}
+                        allArgs[cmd]['opt'][argGrp.args[0]]['widget'] = chooseType(argGrp)
+                        
+                        allArgs[cmd]['opt'][argGrp.args[0]]['excludes'] = [excl.args[0] for excl in arg.arguments 
+                                                                   if excl.args[0] != argGrp.args[0]]
+                        if argGrp.args[0] == '--plug':
+                            # Currently only the 'import' cmd has the '--plug' option,
+                            # but this could no longer be the case in the future.
+                            if cmd == 'import':
+                                allArgs[cmd]['opt'][argGrp.args[0]]['plugins'] = importPlugs
+
+
+def optWindow():
+    """
+    Opens a window listing all of the options for the currently selected plugin.
+    """
+    # with win.subWindow("Plugin Options", modal = True) as sw:
+    #     win.emptyCurrentContainer()
+    #     optDict = {}
+    #     if argVals['--option']:
+    #         for option in enumerate(argVals['--option'].split(',')):
+    #             if '=' in option[1]:
+    #                 optDict[option[1].split('=')[0]] = option[1].split('=')[1]
+    #             else:
+    #                 if option[1] != '':
+    #                     optDict[option[1]] = True
+    #     # print(optDict)
+    #     if not win.combo('--plug'):
+    #         win.message('No import plugin chosen.', width = 170, colspan = 10)
+    #     else:
+    #         plugOpts = allArgs['import']['opt']['--option']['options'][win.combo('--plug')]
+    #         for option in plugOpts:
+    #             # print(option + ': ' + plugOpts[option])
+    #             if '=' in plugOpts[option]:
+    #                 win.entry(option, optDict.get(option) or '', label = True, sticky = 'ew', colspan = 10, tooltip = plugOpts[option])
+    #             else:
+    #                 win.check(option, optDict.get(option) or False, sticky = 'ew', colspan = 10, tooltip = plugOpts[option])
+    #         # print(plugOpts)
+    #     win.button("Done", setOpts, column = 8)
+    #     win.button("Cancel", sw.hide, row = 'p', column = 9)
+    #     sw.show()
+
+def chooseType(arg):
+    """
+    Choose what type of widget to make for the passed argument
+    """
+    if arg.kwargs.get('action') == 'store_true' or arg.kwargs.get('action') == 'store_const':
+        return {'type':'check'}
+    if arg.kwargs.get('type') == int:
+        return {'type':'spin', 'min': 0, 'max': 4096}
+    if arg.kwargs.get('choices'):
+        return {'type':'ticks', 'values':[val for val in arg.kwargs.get('choices')]}
+    if arg.args[0] == '--plug':
+        return {'type':'combo', 'values': [''] + importPlugs}
+    if arg.args[0] == '--option':
+        return {'type':'option', 'func': optWindow}
+    if arg.kwargs.get('type') == float:
+        return {'type':'numeric'}
+    if arg.kwargs.get('type') == 'credits':
+        return {'type':'credits'}
+    return {'type':'entry'}
+
+def addWidget(type, parent = None, cpos = 0, rpos = 0, **kwargs):
+    """
+    Adds a new tk widget and configures it based on passed parameters
+    """
+    cspan = kwargs.pop('colspan', None)
+    rspan = kwargs.pop('rowspan', None)
+    
+    if type == 'combo':
+        widget = Combobox(parent, textvariable = kwargs.pop('textvariable', None))
+        if 'bind' in kwargs:
+            widget.bind('<<ComboboxSelected>>', kwargs['bind'] )
+    
+    elif type == 'ticks':
+        widget = Listbox(parent, listvariable = kwargs.pop('listvariable', None), 
+                         selectmode = kwargs.pop('selectmode', None), height = kwargs.pop('height', None))
+    
+    elif type == 'stext':
+        widget = scrolledtext.ScrolledText(parent, textvariable = kwargs.pop('textvariable', None))
+    
+    elif type == 'button':
+        widget = Button(parent, text = kwargs.pop('text', None), textvariable = kwargs.pop('textvariable', None), command = kwargs.pop('func', None))
+    
+    elif type == 'frame':
+        widget = Frame(parent, textvariable = kwargs.pop('textvariable', None))
+    
+    elif type == 'tab':
+        widget = Notebook(parent, textvariable = kwargs.pop('textvariable', None))
+    
+    elif type == 'label':
+        widget = Label(parent, text = kwargs.pop('text', None), textvariable = kwargs.pop('textvariable', None))
+    
+    elif type == 'check':
+        widget = Checkbutton(parent, text = kwargs.pop('text', None), variable = kwargs.pop('textvariable', None), 
+                             onvalue = kwargs.pop('onvalue', None), offvalue = kwargs.pop('offvalue', None), 
+                             command = kwargs.pop('func', None))
+    
+    elif type == 'spin':
+        widget = Spinbox(parent, from_ = kwargs.pop('min', None), to = kwargs.pop('max', None), textvariable = kwargs.pop('textvariable', None))
+    
+    else: # default for unimplemented types
+        widget = Entry(parent, textvariable = kwargs.pop('textvariable', None))
+    
+    if 'font' in kwargs:
+        widget['font'] = kwargs['font']
+    if 'sticky' in kwargs:
+        widget.sticky = kwargs['sticky']
+    if 'values' in kwargs:
+        widget['values'] = kwargs['values']
+    if 'width' in kwargs:
+        widget.width = kwargs['width']
+    if 'justify' in kwargs:
+        widget['justify'] = kwargs['justify']
+    if 'height' in kwargs:
+        widget['height'] = kwargs['height']
+    if 'default' in kwargs:
+        try:
+            widget.set(kwargs['default'])
+        except Exception as e:
+            try:
+                widget.insert(0, kwargs['default'])
+            except:
+                widget.insert(kwargs['default'][0], kwargs['default'][1])
+    
+    if 'state' in kwargs:
+        widget['state'] = kwargs['state']
+    
+    widget.grid(column = cpos, row = rpos, columnspan = cspan, rowspan = rspan)
     
-    def chooseType(arg):
-        if arg.kwargs.get('action') == 'store_true' or arg.kwargs.get('action') == 'store_const':
-            return {'type':'check'}
-        if arg.kwargs.get('type') == int:
-            return {'type':'spin', 'range': 4096}
-        if arg.kwargs.get('choices'):
-            return {'type':'combo', 'sub':'ticks', 'list':[val for val in arg.kwargs.get('choices')]}
-        if arg.args[0] == '--plug':
-            return {'type':'combo', 'list': [''] + importPlugs}
-        if arg.args[0] == '--option':
-            return {'type':'option'}
-        if arg.kwargs.get('type') == float:
-            return {'type':'entry', 'sub':'numeric'}
-        if arg.kwargs.get('type') == 'credits':
-            return {'type':'entry', 'sub':'credits'}
-        return {'type':'entry'}
+    if 'tab' in kwargs:
+        parent.add(widget, text = kwargs['tab'])
     
-    def makeWidget(name, arg, sticky = 'ew', label = True, **kwargs):
+    return widget
+
+def addWidgetFromArg(name, arg, parent):
+    """
+    Creates a labeled widget for an argument.
+    """
+    widgets[name] = Frame(parent)
+    
+    kwargs = arg['widget']
+    kwargs['textvariable'] = argVals[name]
+    type = kwargs.pop('type', None)
+    
+    sub = kwargs.pop('sub', None)
+    if type == 'ticks':
+        kwargs['height'] = len(kwargs['values'])
+        argVals[name] = value = kwargs.pop('values', None)
+        kwargs['listvariable'] = argVals[name]
+        kwargs['selectmode'] = 'extended'
+    #numeric
+    if type == 'numeric':
+        pass
+    #credits
+    if type == 'credits':
+        pass
+    
+    if type == 'check':
+        kwargs['text'] = name
+        kwargs['columnspan'] = 3
+    else:
+        if type == 'option':
+            label = Button(widgets[name], text = name, command = kwargs.pop('func', None))
+            type = 'entry'
+        else:
+            label = Label(widgets[name], text = name)
+        label.grid(column = 0, row = 0)
+        kwargs['rpos'] = 0
+        kwargs['cpos'] = 1
+        kwargs['columnspan'] = 2
+    
+    addWidget(type, widgets[name], **kwargs)
+    widgets[name].grid()
+    
+    def makeWidgets(name, arg, sticky = 'ew', label = True, **kwargs):
         kwargs['sticky'] = sticky
         kwargs['label'] = label
         kwargs['change'] = updArgs
         kwargs['tooltip'] = arg['help']
         if arg == allArgs.get(name):
             kwargs['colspan'] = 1
         else:
@@ -240,15 +517,15 @@
             kwargs['item'] = argVals[name] or arg.get('default') or 0
             win.spin(name, 0 - widget['range'], endValue = widget['range'], **kwargs)
         elif widget['type'] == 'combo':
             kwargs['sticky'] = 'w'
             if widget.get('sub'):
                 kwargs['kind'] = widget['sub']
                 kwargs.pop('label')
-            win.combo(name, widget['list'], **kwargs)
+            win.combo(name, widget['values'], **kwargs)
             
             # If we're switching to the 'station' command from another command,
             # this argument needs to be cleared from allArgs to not mess things up.
             if not widget.get('sub'):
                 if argVals[name] != str:
                     argVals[name] = None
                 default = '?' if arg.get('choices') else ''
@@ -275,16 +552,105 @@
                 if widget.get('sub') == 'credits':
                     # TODO: Handle 'credits' type.
                     pass
                 else:
                     kwargs['kind'] = 'numeric'
             
             win.entry(name, argVals[name] or arg.get('default'), **kwargs)
+
+
+def updateCommandBox(args = None):
+    """
+    Updates the argument panes when the selected command is changed.
+    """
+    
+    cmd = widgets['Command'].get()
+    
+    widgets['helpPane']['state'] = 'normal'
+    widgets['helpPane'].delete(0.0, 'end')
+    widgets['helpPane'].insert(0.0, cmdHelp[cmd])
+    widgets['helpPane']['state'] = 'disabled'
+    
+    # Hide all of the widgets currently displayed in 'req' and 'opt'
+    for widget in widgets['req'].winfo_children():
+        widget.grid_forget()
+    
+    for widget in widgets['opt'].winfo_children():
+        widget.grid_forget()
+    
+    # Nothing more needs done for the 'help' command.
+    if cmd == 'help':
+        return
+    
+    # The 'station' command has arguments with the same names
+    # as arguments for other command, such as 'planetary',
+    # but in 'station' they are to set the value, whereas
+    # in the other command they are used to exclude certain values,
+    # meaning that 'station' needs unique names to prevent conflicts.
+    prepend = ''
+    if cmd == 'station':
+        prepend = cmd + '~'
+    else:
+        prepend = ''
+    #That was a lot of explanation for 5 lines of code.
+    
+    # Show the widgets for all required arguments of the current command
+    # If the argument's widget does not exist, make it.
+    if allArgs[cmd]['req']:
+        if not 'Required:' in widgets:
+            widgets['Required:'] = addWidget('label', widgets['req'], sticky = 'nw', text = 'Required:')
+        else:
+            widgets['Required:'].grid()
+        
+        i = 0
+        for key in allArgs[cmd]['req']:
+            i += 1
+            if not (prepend + key) in widgets:
+                addWidgetFromArg(prepend + key, allArgs[cmd]['req'][key], widgets['req'])
+            else:
+                widgets[prepend + key].grid(column = 0, row = i)
+    
+    if allArgs[cmd]['opt']:
+        if not 'Optional:' in widgets:
+            widgets['Optional:'] = addWidget('label', widgets['opt'], sticky = 'nw', text = 'Optional:')
+        else:
+            widgets['Optional:'].grid()
+        
+        i=0
+        for key in allArgs[cmd]['opt']:
+            i+=1
+            if not (prepend + key) in widgets:
+                addWidgetFromArg(prepend + key, allArgs[cmd]['opt'][key], widgets['opt'])
+            else:
+                widgets[prepend + key].grid(column =  0, row = i)
+
+
+
+# Setup the CLI interface and build the main window
+def main(argv = None):
     
+    class IORedirector:
+        
+        def __init__(self, TEXT_INFO):
+            self.TEXT_INFO = TEXT_INFO
+    
+    class StdoutRedirector(IORedirector):
+        
+        def write(self, string):
+            self.TEXT_INFO.config(text = self.TEXT_INFO.cget('text').rsplit('\r', 1)[0] + string)
+        
+        def flush(self):
+            
+            sys.__stdout__.flush()
+    
+    #TODO: Implement in tk
     def setOpts():
+        """
+        Sets the main window options entry to the checked values in the options window.
+        """
         sw = win.widgetManager.get(WIDGET_NAMES.SubWindow, "Plugin Options")
         plugOpts = allArgs['import']['opt']['--option']['options'].get(win.combo('--plug'))
         argStr = ''
         # print(plugOpts)
         if plugOpts:
             for option in plugOpts:
                 # print(option + ': ' + plugOpts[option])
@@ -294,15 +660,19 @@
                 elif win.check(option):
                     argStr = argStr + option + ','
             # print(argStr)
             argStr = argStr.rsplit(',', 1)[0]
             win.entry('--option', argStr)
         sw.hide()
     
+    #TODO: Implement in tk
     def optionsWin():
+        """
+        Opens a window listing all of the options for the currently selected plugin.
+        """
         with win.subWindow("Plugin Options", modal = True) as sw:
             win.emptyCurrentContainer()
             optDict = {}
             if argVals['--option']:
                 for option in enumerate(argVals['--option'].split(',')):
                     if '=' in option[1]:
                         optDict[option[1].split('=')[0]] = option[1].split('=')[1]
@@ -321,15 +691,19 @@
                     else:
                         win.check(option, optDict.get(option) or False, sticky = 'ew', colspan = 10, tooltip = plugOpts[option])
                 # print(plugOpts)
             win.button("Done", setOpts, column = 8)
             win.button("Cancel", sw.hide, row = 'p', column = 9)
             sw.show()
     
+    #TODO: Implement in tk
     def updArgs(name):
+        """
+        Updates the value of argVals[name] when the linked widget's value is changed in the window.
+        """
         
         def getWidgetType(name):
             for widgetType in [WIDGET_NAMES.Entry, WIDGET_NAMES.Button, WIDGET_NAMES.CheckBox,
                                WIDGET_NAMES.RadioButton, WIDGET_NAMES.SpinBox, WIDGET_NAMES.OptionBox]:
                 try:
                     win.widgetManager.get(widgetType, name)
                     return WIDGET_NAMES.widgets[widgetType]
@@ -351,71 +725,50 @@
             try:
                 excluded = allArgs[win.combo("Command")]['opt'][name].get('excludes')
                 argBase = allArgs[win.combo("Command")]['opt']
             except KeyError:
                 excluded = None
         
         # Reset any arguments excluded by this one if it's been set.
-        
-        # print("'" + str(argVals[name]) + "': " + str(argVals[name] == True)
-        #       + "': " + str(not argVals[name]) + " : " + str(not not argVals[name])
-        #      )
-        
-        # Apparently, with strings, 'not not ""' != '""' when considered as a boolean.
         if excluded and not not argVals[name]:
             for exclude in excluded:
                 widgetType = argBase[exclude]['widget']['type']
                 if widgetType == 'combo':
                     win.combo(exclude, mode = 'clear', callFunction = False)
                 elif widgetType == 'spin':
                     win.spin(exclude, mode = 'clear', callFunction = False)
                 elif widgetType == 'entry':
                     win.setEntry(exclude, '', callFunction = False)
                 elif widgetType == 'check':
                     win.check(exclude, False, callFunction = False)
     
+    #TODO: REMOVE
     def updCmd():
+        """
+        Updates the argument panes when the selected command is changed.
+        """
         cmd = win.combo("Command")
         # print(cmd)
         
         win.message("helpText", cmdHelp[cmd])
         win.emptyScrollPane('req')
         win.emptyScrollPane('opt')
         if cmd == 'help':
             return
         if allArgs[cmd]['req']:
             with win.scrollPane('req', disabled = 'horizontal'):
                 win.label('Required:', sticky = 'w')
                 for key in allArgs[cmd]['req']:
-                    makeWidget(key, allArgs[cmd]['req'][key])
+                    makeWidgets(key, allArgs[cmd]['req'][key])
         
         if allArgs[cmd]['opt']:
             with win.scrollPane('opt', disabled = 'horizontal'):
                 win.label('Optional:', sticky = 'w')
                 for key in allArgs[cmd]['opt']:
-                    makeWidget(key, allArgs[cmd]['opt'][key])
-    
-    def changeCWD():
-        """
-        Opens a folder select dialog.
-        """
-        cwd = win.directoryBox("Select the top-level folder for TD to work in...", dirName = argVals['--cwd'])
-        if cwd:
-            argVals['--cwd'] = str(Path(cwd))
-        win.label('cwd', argVals['--cwd'])
-    
-    def changeDB():
-        """
-        Opens a file select dialog.
-        """
-        db = win.openBox("Select the TD database file to use...", dirName = str(Path(argVals['--db']).parent),
-                          fileTypes = [('Data Base File', '*.db')])
-        if db:
-            argVals['--db'] = str(Path(db))
-        win.label('db', argVals['--db'])
+                    makeWidgets(key, allArgs[cmd]['opt'][key])
     
     def runTD():
         """
         Executes the TD command selected in the GUI.
         """
         
         from . import tradeexcept
@@ -516,130 +869,132 @@
                 result = getVals(arg, allArgs)
                 if result:
                     argv = argv + result
         
         win.message('outputText', '')
         threading.Thread(target = runTrade, name = "TDThread", daemon = True).start()
     
-    # All available commands
-    Commands = ['help'] + [ cmd for cmd, module in sorted(commands.commandIndex.items()) ]
-    # Used to run TD cli commands.
-    cmdenv = commands.CommandIndex().parse
-    # 'help' output, required & optional arguments, for each command
-    cmdHelp = {}
-    
-    dbS = str(Path((os.environ.get('TD_DATA') or os.path.join(os.getcwd(), 'data')) / Path('TradeDangerous.db')))
-    cwdS = str(Path(os.getcwd()))
-    allArgs = {
-        '--debug': { 'help': 'Enable/raise level of diagnostic output.',
-                    'default':  0, 'required': False, 'action': 'count',
-                    'widget': {'type':'combo', 'list': ['', '-w', '-ww', '-www']}
-                    },
-        '--detail':{ 'help': 'Increase level of detail in output.',
-                    'default': 0, 'required': False, 'action': 'count',
-                    'excludes': ['--quiet'], 'widget': {'type':'combo', 'list': ['', '-v', '-vv', '-vvv']}
-                    },
-        '--quiet':{ 'help': 'Reduce level of detail in output.',
-                   'default': 0, 'required': False, 'action': 'count',
-                   'excludes': ['--detail'], 'widget': {'type':'combo', 'list': ['', '-q', '-qq', '-qqq']}
-                   },
-        '--db':{ 'help': 'Specify location of the SQLite database.',
-                'default': dbS, 'dest': 'dbFilename', 'type': str,
-                'widget': {'type':'button', 'func':changeDB}
-                },
-        '--cwd':{ 'help': 'Change the working directory file accesses are made from.',
-                 'default': cwdS, 'type': str, 'required': False,
-                 'widget': {'type':'button', 'func':changeCWD}
-                 },
-        '--link-ly':{ 'help': 'Maximum lightyears between systems to be considered linked.',
-                     'default': 30,
-                     'widget': {'type':'entry', 'sub':'numeric'}
-                     }
-        }
-    
-    # Used to save the value of the arguments.
-    argVals = {'--debug': '',
-               '--detail': '',
-               '--quiet': '',
-               '--db': dbS,
-               '--cwd': cwdS,
-               '--link-ly': 30
-               }
-    
+    # TODO: replace
+    def makeWidgets(name, arg, sticky = 'ew', label = True, **kwargs):
+        kwargs['sticky'] = sticky
+        kwargs['label'] = label
+        kwargs['change'] = updArgs
+        kwargs['tooltip'] = arg['help']
+        if arg == allArgs.get(name):
+            kwargs['colspan'] = 1
+        else:
+            kwargs['colspan'] = 9
+        
+        widget = arg['widget']
+        # print(name + ': ' + str(widget))
+        if widget['type'] == 'button':
+            kwargs.pop('change')
+            kwargs.pop('label')
+            kwargs.pop('colspan')
+            win.button(name, widget['func'], **kwargs)
+        elif widget['type'] == 'check':
+            win.check(name, argVals[name] or arg.get('default'), text = name, **kwargs)
+        elif widget['type'] == 'spin':
+            kwargs['item'] = argVals[name] or arg.get('default') or 0
+            win.spin(name, widget['min'] - widget['max'], endValue = widget['max'], **kwargs)
+        elif widget['type'] == 'combo':
+            kwargs['sticky'] = 'w'
+            if widget.get('sub'):
+                kwargs['kind'] = widget['sub']
+                kwargs.pop('label')
+            win.combo(name, widget['values'], **kwargs)
+            
+            # If we're switching to the 'station' command from another command,
+            # this argument needs to be cleared from allArgs to not mess things up.
+            if not widget.get('sub'):
+                if argVals[name] != str:
+                    argVals[name] = None
+                default = '?' if arg.get('choices') else ''
+                win.combo(name, argVals[name] or arg.get('default') or default, callFunction = False)
+            else:
+            # If we're switching to another command from the 'station' command,
+            # this argument needs to be cleared from allArgs to not mess things up.
+                if argVals[name] == str:
+                    argVals[name] = None
+                if argVals[name]:
+                    for val in argVals[name]:
+                        win.setOptionBox(name, val, value = argVals[name][val], callFunction = False)
+        
+        elif widget['type'] == 'option':
+            kwargs.pop('change')
+            kwargs.pop('label')
+            kwargs.pop('colspan')
+            win.button('optionButton', optionsWin, name = '--option', **kwargs)
+            kwargs['sticky'] = sticky
+            kwargs['change'] = updArgs
+            win.entry(name, argVals[name] or arg.get('default'), row = 'p' , column = 1, colspan = 9, **kwargs)
+        elif widget['type'] == 'entry':
+            if widget.get('sub'):
+                if widget.get('sub') == 'credits':
+                    # TODO: Handle 'credits' type.
+                    pass
+                else:
+                    kwargs['kind'] = 'numeric'
+            
+            win.entry(name, argVals[name] or arg.get('default'), **kwargs)
+
+
     sys.argv = ['trade']
     if not argv:
         argv = sys.argv
     if sys.hexversion < 0x03040200:
         raise SystemExit(
             "Sorry: TradeDangerous requires Python 3.4.2 or higher.\n"
             "For assistance, see:\n"
             "\tBug Tracker: https://github.com/eyeonus/Trade-Dangerous/issues\n"
             "\tDocumentation: https://github.com/eyeonus/Trade-Dangerous/wiki\n"
             "\tEDForum Thread: https://forums.frontier.co.uk/showthread.php/441509\n"
             )
     
-    try:
-        cmdenv(['help'])
-    except exceptions.UsageError as e:
-        cmdHelp['help'] = str(e)
-    for cmd in Commands:
-        # print(cmd)
-        if cmd == 'help':
-            continue
-        try:
-            cmdenv(['trade', cmd, '-h'])
-        except exceptions.UsageError as e:
-            cmdHelp[cmd] = str(e)
-        index = commands.commandIndex[cmd]
-        
-        allArgs[cmd] = {'req': {}, 'opt': {}}
-        if index.arguments:
-            for arg in index.arguments:
-                # print(arg.args[0])
-                argVals[arg.args[0]] = arg.kwargs.get('default') or None
-                
-                allArgs[cmd]['req'][arg.args[0]] = {kwarg : arg.kwargs[kwarg] for kwarg in arg.kwargs}
-                allArgs[cmd]['req'][arg.args[0]]['widget'] = chooseType(arg)
-        # print(allArgs[cmd]['req'])
-        
-        if index.switches:
-            for arg in index.switches:
-                try:
-                    argVals[arg.args[0]] = arg.kwargs.get('default') or None
-                    
-                    allArgs[cmd]['opt'][arg.args[0]] = {kwarg : arg.kwargs[kwarg] for kwarg in arg.kwargs}
-                    allArgs[cmd]['opt'][arg.args[0]]['widget'] = chooseType(arg)
-                    
-                    if arg.args[0] == '--option':
-                        # Currently only the 'import' cmd has the '--plug' option,
-                        # but this could no longer be the case in future.
-                        if cmd == 'import':
-                            plugOptions = {
-                                plug: plugins.load(cmdenv(['trade', cmd, '--plug', plug, '-O', 'help']).plug,
-                                                    "ImportPlugin").pluginOptions for plug in importPlugs
-                                }
-                            allArgs[cmd]['opt'][arg.args[0]]['options'] = plugOptions
-                
-                except AttributeError:
-                    for argGrp in arg.arguments:
-                        argVals[argGrp.args[0]] = argGrp.kwargs.get('default') or None
-                        
-                        allArgs[cmd]['opt'][argGrp.args[0]] = {kwarg : argGrp.kwargs[kwarg] for kwarg in argGrp.kwargs}
-                        allArgs[cmd]['opt'][argGrp.args[0]]['widget'] = chooseType(argGrp)
-                        
-                        allArgs[cmd]['opt'][argGrp.args[0]]['excludes'] = [excl.args[0] for excl in arg.arguments 
-                                                                   if excl.args[0] != argGrp.args[0]]
-                        if argGrp.args[0] == '--plug':
-                            # Currently only the 'import' cmd has the '--plug' option,
-                            # but this could no longer be the case in future.
-                            if cmd == 'import':
-                                allArgs[cmd]['opt'][argGrp.args[0]]['plugins'] = importPlugs
-        # print(allArgs[cmd]['opt'])
-    # print(allArgs)
-    # print(argVals)
+    
+    buildArgDicts()
+
+#    window = Tk()
+#    window.title('Trade Dangerous GUI (Beta), TD v.%s' % (__version__,))
+#    window.iconbitmap(resource_filename(__name__, "../tradedangerouscrest.ico"))
+#    
+#    widgets['Command'] = addWidget('combo', window, 3, 0, values = Commands, bind = updateCommandBox, 
+#                width = 10, state = 'readonly', height = len(Commands), default = Commands[0], columnspan = 4,
+#                justify = 'center', sticky = 'ew', tooltip = 'Trade Dangerous command to run.')
+#    widgets['req'] = addWidget('frame', window, 0, 1, width = 200, height = 175, columnspan = 10, sdir = 'v')
+#    widgets['opt'] = addWidget('frame', window, 0, 2, width = 200, height = 345, columnspan = 10, sdir = 'v')
+#    
+#    widgets['tabFrame'] = addWidget('tab', window, 10, 1, rowspan = 2, columnspan = 40, width = 560, height = 520)
+#    widgets [ 'helpPane'] = addWidget('stext', widgets['tabFrame'], width = 80, font = font.Font(family = 'Courier New', size=10),
+#              #'fixed', 'oemfixed', 'ansifixed', 'systemfixed', 'TkFixedFont'
+#              default = (0.0, cmdHelp['help']), state = 'disabled', tab = 'Help')
+#    widgets['outPane'] = addWidget('stext', widgets['tabFrame'], width = 80, state = 'disabled', tab = 'Output')
+#    
+#        makeWidget('--link-ly', allArgs['--link-ly'], sticky = 'w', width = 4, row = 3, column = 2)
+#        
+#        makeWidget('--quiet', allArgs['--quiet'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 46)
+#        
+#        makeWidget('--detail', allArgs['--detail'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 47)
+#        
+#        makeWidget('--debug', allArgs['--debug'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 48)
+#        
+#        win.button('Run', runTD, tooltip = 'Execute the selected command.',
+#                   sticky = 'w', row = 3, column = 49)
+#        
+#        makeWidget('--cwd', allArgs['--cwd'], width = 4, row = 4, column = 0)
+#        with win.scrollPane('CWD', disabled = 'vertical', row = 4, column = 1, colspan = 49) as pane:
+#            pane.configure(width = 500, height = 20)
+#            win.label('cwd', argVals['--cwd'], sticky = 'w')
+#        
+#        makeWidget('--db', allArgs['--db'], width = 4, row = 5, column = 0)
+#        with win.scrollPane('DB', disabled = 'vertical', row = 5, column = 1, colspan = 49) as pane:
+#            pane.configure(width = 500, height = 20)
+#            win.label('db', argVals['--db'], sticky = 'w')
+#    
+#    window.mainloop()
     
     with gui('Trade Dangerous GUI (Beta), TD v.%s' % (__version__,), inPadding = 1) as win:
         win.setFont(size = 8, family = 'Courier')
         win.combo('Command', Commands, change = updCmd, tooltip = 'Trade Dangerous command to run.',
                   stretch = 'none', sticky = 'ew', width = 10, row = 0, column = 0, colspan = 5)
         with win.scrollPane('req', disabled = 'horizontal', row = 1, column = 0, colspan = 10) as pane:
             pane.configure(width = 200, height = 75)
@@ -656,34 +1011,34 @@
             
             with win.tab('Output'):
                 with win.scrollPane('outPane', disabled = 'horizontal') as pane:
                     pane.configure(width = 560, height = 420)
                     win.message('outputText', '')
                     win.widgetManager.get(WIDGET_NAMES.Message, 'outputText').config(width = 560)
         
-        makeWidget('--link-ly', allArgs['--link-ly'], sticky = 'w', width = 4, row = 3, column = 2)
+        makeWidgets('--link-ly', allArgs['--link-ly'], sticky = 'w', width = 4, row = 3, column = 2)
         
-        makeWidget('--quiet', allArgs['--quiet'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 46)
+        makeWidgets('--quiet', allArgs['--quiet'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 46)
         
-        makeWidget('--detail', allArgs['--detail'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 47)
+        makeWidgets('--detail', allArgs['--detail'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 47)
         
-        makeWidget('--debug', allArgs['--debug'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 48)
+        makeWidgets('--debug', allArgs['--debug'], sticky = 'e', disabled = ':', width = 1, row = 3, column = 48)
         
         win.button('Run', runTD, tooltip = 'Execute the selected command.',
                    sticky = 'w', row = 3, column = 49)
         
-        makeWidget('--cwd', allArgs['--cwd'], width = 4, row = 4, column = 0)
+        makeWidgets('--cwd', allArgs['--cwd'], width = 4, row = 4, column = 0)
         with win.scrollPane('CWD', disabled = 'vertical', row = 4, column = 1, colspan = 49) as pane:
             pane.configure(width = 500, height = 20)
-            win.label('cwd', argVals['--cwd'], sticky = 'w')
+            widgets['cwd'] = win.label('cwd', argVals['--cwd'], sticky = 'w')
         
-        makeWidget('--db', allArgs['--db'], width = 4, row = 5, column = 0)
+        makeWidgets('--db', allArgs['--db'], width = 4, row = 5, column = 0)
         with win.scrollPane('DB', disabled = 'vertical', row = 5, column = 1, colspan = 49) as pane:
             pane.configure(width = 500, height = 20)
-            win.label('db', argVals['--db'], sticky = 'w')
+            widgets['db'] = win.label('db', argVals['--db'], sticky = 'w')
     
     # End of window
 
 
 def trade(argv):
     """
     This method represents the trade command.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tradedangerous-10.9.8/tradedangerous/cli.py` & `tradedangerous-11.0.0/tradedangerous/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,19 +27,14 @@
 # END USERS: If you are a user looking to find out how to use TD,
 # please consult the file "README.md".
 #
 # DEVELOPERS: If you are a programmer who wants TD to do something
 # cool, please see the TradeDB and TradeCalc modules. TD is designed
 # to empower other programmers to do cool stuff.
 
-from __future__ import absolute_import
-from __future__ import with_statement
-from __future__ import print_function
-from __future__ import division
-from __future__ import unicode_literals
 import os
 import traceback
 
 from . import commands
 from .commands import exceptions
 from .plugins import PluginException
 
@@ -54,15 +49,15 @@
     if sys.hexversion < 0x03040200:
         raise SystemExit(
             "Sorry: TradeDangerous requires Python 3.4.2 or higher.\n"
             "For assistance, see:\n"
             "\tBug Tracker: https://github.com/eyeonus/Trade-Dangerous/issues\n"
             "\tDocumentation: https://github.com/eyeonus/Trade-Dangerous/wiki\n"
             "\tEDForum Thread: https://forums.frontier.co.uk/showthread.php/441509\n"
-            )
+        )
     from . import tradeexcept
     
     try:
         try:
             if "CPROF" in os.environ:
                 import cProfile
                 cProfile.run("trade(argv)")
@@ -74,15 +69,15 @@
                 raise e
             sys.exit(1)
         except tradeexcept.TradeException as e:
             print("%s: %s" % (argv[0], str(e)))
             if 'EXCEPTIONS' in os.environ:
                 raise e
             sys.exit(1)
-    except (UnicodeEncodeError, UnicodeDecodeError) as e:
+    except (UnicodeEncodeError, UnicodeDecodeError):
         print("-----------------------------------------------------------")
         print("ERROR: Unexpected unicode error in the wild!")
         print()
         print(traceback.format_exc())
         print(
             "Please report this bug (http://kfs.org/td/issues). You may be "
             "able to work around it by using the '-q' parameter. Windows "
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/edsm.py` & `tradedangerous-11.0.0/tradedangerous/misc/edsm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 #! /usr/bin/env python
 
 """
 based on edsc.py
 uses EDSM - https://www.edsm.net/api
 """
 
-from __future__ import absolute_import
-from __future__ import with_statement
-from __future__ import print_function
-from __future__ import division
-from __future__ import unicode_literals
-
 import json
-import os
 
 try:
     import requests
 except ImportError as e:
     import pip
     print("ERROR: Unable to load the Python 'requests' package.")
     approval = input(
@@ -43,15 +36,15 @@
             if error:
                 print("ERR:", error)
             print(file=fh)
     except FileNotFoundError:
         pass
 
 
-class EDSMQueryBase(object):
+class EDSMQueryBase:
     """
     Base class for creating an EDSM Query class, do not use directly.
     
     Derived class must declare "apiCall" which is appended to baseURL
     to form the query URL.
     """
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/edsc.py` & `tradedangerous-11.0.0/tradedangerous/misc/edsc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 #! /usr/bin/env python3
 
-from __future__ import absolute_import
-from __future__ import with_statement
-from __future__ import print_function
-from __future__ import division
-from __future__ import unicode_literals
-
-from collections import defaultdict, namedtuple
-from urllib.parse import urlencode
+from collections import namedtuple
 from urllib.request import Request, urlopen
 
 import json
-import os
 
 try:
     import requests
 except ImportError as e:
     import pip
     print("ERROR: Unable to load the Python 'requests' package.")
     approval = input(
@@ -41,15 +33,15 @@
             if error:
                 print("ERR:", error)
             print(file=fh)
     except FileNotFoundError:
         pass
 
 
-class EDSCQueryBase(object):
+class EDSCQueryBase:
     """
     Base class for creating an EDSC Query class, do not use directly.
     
     Derived class must declare "apiCall" which is appended to baseURL
     to form the query URL.
     """
     
@@ -112,15 +104,15 @@
 
 
 class Status(namedtuple('Status', [
         'source', 'code', 'msg', 'lhs', 'rhs'
         ])):
     pass
 
-class StarSubmissionResult(object):
+class StarSubmissionResult:
     """
     Translates a response the json we get back from EDSC when
     we submit a StarSubmission into something less awful to
     work with.
     
     Attributes:
         valid
@@ -224,25 +216,25 @@
         errPairs = set()
         for ent in distArray:
             lhsName = ent['system1'].upper()
             rhsName = ent['system2'].upper()
             code = int(ent['status']['statusnum'])
             msg = ent['status']['msg']
             if code in [301, 302, 303, 304]:
-                if not lhsName in self.distances:
+                if lhsName not in self.distances:
                     self.distances[lhsName] = {}
                 try:
                     rhsDists = self.distances[rhsName]
                     if lhsName in rhsDists:
                         continue
                 except KeyError:
                     pass
                 dist = float(ent['dist'])
                 self.distances[lhsName][rhsName] = dist
-                if not lhsName in self.systems:
+                if lhsName not in self.systems:
                     self.systems[lhsName] = (code, None)
             else:
                 if (lhsName,rhsName,code) in errPairs:
                     continue
                 if (rhsName,lhsName,code) in errPairs:
                     continue
                 errPairs.add((lhsName,rhsName,code))
@@ -331,15 +323,15 @@
         try:
             return self.codeMap[code]
         except KeyError:
             return "Error #{} (unknown)".format(code)
 
 
 
-class StarSubmission(object):
+class StarSubmission:
     baseURL = "http://edstarcoordinator.com/api.asmx/"
     apiCall = "SubmitDistances"
     
     def __init__(
             self, star,
             test=False, commander=None,
             refs=None, distances=None,
@@ -427,14 +419,15 @@
         try:
             innerData = respData['d']
         except KeyError:
             raise SubmissionError("Server Error: " + resp)
         
         return innerData
 
+
 if __name__ == "__main__":
     print("Requesting recent, non-test, coords-known, cr >= 2 stars")
     edsq = StarQuery(test=False, confidence=2, known=1)
     data = edsq.fetch()
     
     if edsq.status['statusnum'] != 0:
         raise Exception("Query failed: {} ({})".format(
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-11.0.0/tradedangerous/misc/prices-json-exp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #! /usr/bin/env python
 
 # Experimental module to generate a JSON version of the .prices file.
 
-# Set to True to allow export of systems that don't have any station data
-emptySystems = True
-# Set to True to allow export of stations that don't have prices
-emptyStations = True
-
 import sqlite3
 import json
 import time
 import collections
 import os
 
+
+# Set to True to allow export of systems that don't have any station data
+emptySystems = True
+# Set to True to allow export of stations that don't have prices
+emptyStations = True
+
 conn = sqlite3.connect("data/TradeDangerous.db")
 
+
 def collectItemData(db):
     """
     Builds a flat, array of item names that serves as a table of items.
     Station Price Data refers to this table by position in the array.
     As a result, we also need a mapping for itemID -> tableID
     """
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/eddb.py` & `tradedangerous-11.0.0/tradedangerous/misc/eddb.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,24 @@
     import misc.eddb
     for sysdata in misc.eddb.SystemsQuery():
         print(sysdata)
 
 Original author: oliver@kfs.org
 """
 
-import json
-import sys
 import transfers
 
 BASE_URL = "http://eddb.io/archive/v3/"
 COMMODITIES_JSON = BASE_URL + "commodities.json"
 SYSTEMS_JSON = BASE_URL + "systems.json"
 STATIONS_EXT_JSON = BASE_URL + "stations.json"
 STATIONS_LITE_JSON = BASE_URL + "stations_lite.json"
 
 
-class EDDBQuery(object):
+class EDDBQuery:
     """
     Base class for querying an EDDB data set and converting the
     JSON results into an iterable stream.
     
     Example:
         for entity in EDDBQuery():
             print(entity)
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-11.0.0/tradedangerous/misc/diff-system-csvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,24 +25,26 @@
     def __str__(self):
         return "{},{},{}".format(self.x, self.y, self.z)
 
 
 class Item(namedtuple('Item', [ 'norm', 'name', 'loc' ])):
     pass
 
+
 normalizeRe = re.compile('[^A-Za-z0-9\' ]')
 
+
 def readFile(filename):
     path = Path(filename)
     if not path.exists():
         raise SystemExit("File not found: {}".format(filename))
     
     names, locs = dict(), dict()
     
-    with path.open("rU", encoding="utf-8") as fh:
+    with path.open("r", encoding="utf-8") as fh:
         csvin = csv.reader(fh, delimiter=',', quotechar='\'', doublequote=True)
         # skip headings
         next(csvin)
         
         for line in csvin:
             name = line[0]
             x = float(line[1])
@@ -67,14 +69,15 @@
                             filename, locs[item.loc].name, name, item.loc
                         ))
             else:
                 locs[item.loc] = item
     
     return names, locs
 
+
 oldNames, oldLocs = readFile(sys.argv[1])
 newNames, newLocs = readFile(sys.argv[2])
 
 for oldName, oldItem in oldNames.items():
     try:
         # Look the item up in the new names dict
         newItem = newNames[oldItem.norm]
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/progress.py` & `tradedangerous-11.0.0/tradedangerous/misc/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-class Progress(object):
+class Progress:
     """
     Helper class that describes a simple text-based progress bar.
     """
     
     def __init__(self, maxValue, width, start=0, prefix=""):
         """
         Arguments:
@@ -64,8 +64,8 @@
     def clear(self):
         """
         Remove the current progress bar, if any
         """
         if self.textLen:
             fin = "\r{:{width}}\r".format('', width=self.textLen)
             sys.stdout.write(fin)
-            sys.stdout.flush()
+            sys.stdout.flush()
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/clipboard.py` & `tradedangerous-11.0.0/tradedangerous/misc/clipboard.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 
 if 'NOTK' not in os.environ:
     try:
         from tkinter import Tk
         
-        class SystemNameClip(object):
+        class SystemNameClip:
             """
             A cross-platform wrapper for copying system names into
             the clipboard such that they can be pasted into the E:D
             galaxy search - which means forcing them into lower case
             because E:D's search doesn't work with upper case
             characters.
             """
@@ -37,14 +37,13 @@
     except ImportError:
         print(
                 "WARNING: This feature expects you to have 'tkinter' package "
                 "installed to work. It is either not installed or broken.\n"
                 "Set the environment variable 'NOTK' to disable this warning."
         )
         
-        class SystemNameClip(object):
+        class SystemNameClip:
             """
             Dummy implementation when tkinter is not available.
             """
             def copy_text(self, text):
                 pass
-
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/eddn.py` & `tradedangerous-11.0.0/tradedangerous/misc/eddn.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,20 +82,20 @@
         'uploader',
         'software',
         'version',
         ])):
     pass
 
 
-class Listener(object):
+class Listener:
     """
     Provides an object that will listen to the Elite Dangerous Data Network
     firehose and capture messages for later consumption.
     
-    Rather than individual upates, prices are captured across a window of
+    Rather than individual updates, prices are captured across a window of
     between minBatchTime and maxBatchTime. When a new update is received,
     Rather than returning individual messages, messages are captured across
     a window of potentially several seconds and returned to the caller in
     batches.
     
     Attributes:
         zmqContext          Context this object is associated with,
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/coord64.py` & `tradedangerous-11.0.0/tradedangerous/misc/coord64.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 #   "1gA:Oi:-Go"
 #
 # A reversing function is also provided.
 #
 # Original Author: Oliver "kfsone" Smith <oliver@kfs.org>
 # Released under the "use it with attribution" license.
 
-from __future__ import print_function, division
 import string
 
+
 alphabet = string.digits + string.ascii_lowercase + string.ascii_uppercase + '_.'
 precision = 100.
 
+
 def coord_to_d64(coord):
     i = int(abs(coord * precision))
     
     digits = ""
     while True:
         digits = alphabet[i & 63] + digits
         i >>= 6   # divides by 64, or one digit
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-11.0.0/tradedangerous/misc/checkpricebounds.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
             colorama.Fore.RESET,
             sep="",
         )
     
     if stations:
         print()
         print("Generating", deletePrices)
-        now = tdb.query("SELECT CURRENT_TIMESTAMP").fetchone()[0];
+        now = tdb.query("SELECT CURRENT_TIMESTAMP").fetchone()[0]
         with open(deletePrices, "w", encoding="utf-8") as fh:
             print("# Deletions based on {} prices".format(
                 table,
             ), file=fh)
             for stnID, items in stations.items():
                 station = tdb.stationByID[stnID]
                 print(file=fh)
@@ -171,16 +171,14 @@
                 print(deletion[0], '; --', deletion[1], file=fh)
                 if doDeletions:
                     db.execute(deletion[0])
             if doDeletions:
                 db.commit()
 
 def main():
-    doDeletions = False
-    
     parser = argparse.ArgumentParser(
         description='Check for prices that are outside reasonable bounds.'
     )
     parser.add_argument(
         '--percentile',
         help='Set cutoff percentile',
         type=float,
@@ -280,9 +278,10 @@
         table,
         margin=argv.margin,
         doDeletions=argv.delete,
         percentile=argv.percentile,
         errorFilter=errorFilter,
     )
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-11.0.0/tradedangerous/misc/derp-sentinel.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
             continue
         bef, aft = text[:i], text[i+1:]
         for mutant in mutators[char]:
             t2 = bef + mutant + aft
             yield t2
             yield from mutate(str(t2), i+len(mutant))
 
+
 for name in names:
     for mutant in mutate(name, 0):
         if mutant in names:
             print("{} <-> {}".format(name, mutant))
-
```

### Comparing `tradedangerous-10.9.8/tradedangerous/misc/importeddbstats.py` & `tradedangerous-11.0.0/tradedangerous/misc/importeddbstats.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         if not stationList:
             continue
         name = eddbStn['name'].upper()
         tdStn = stationList.get(name, None)
         if tdStn:
             yield tdStn, eddbStn
 
+
 updateStation = tdb.updateLocalStation
 
 bool_trans = { None: '?', 0: 'N', 1: 'Y' }
 
 updates = 0
 for tdStn, eddbStn in matching_stations():
     mps = eddbStn['max_landing_pad_size'] or '?'
@@ -46,8 +47,8 @@
             commit=False,
             ):
         updates += 1
 
 if updates:
     tdb.getDB().commit()
     csvexport.exportTableToFile(tdb, tdb.tdenv, "Station")
-    print("Updated Station.csv: {} updates".format(updates))
+    print("Updated Station.csv: {} updates".format(updates))
```

### Comparing `tradedangerous-10.9.8/tradedangerous/prices.py` & `tradedangerous-11.0.0/tradedangerous/prices.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,24 @@
 #
 # You are free to use, redistribute, or even print and eat a copy of
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 # TradeDangerous :: Modules :: Generate TradeDangerous.prices
 
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-
 import sys
-import os
-import re
 import sqlite3
 
 
-class Element(object):
-    basic     = (1 << 0)
-    supply    = (1 << 1)
-    timestamp = (1 << 2)
-    full      = (basic | supply | timestamp)
-    blanks    = (1 <<31)
+class Element:      # TODO: enum?
+    basic     = 1 << 0
+    supply    = 1 << 1
+    timestamp = 1 << 2
+    full      = basic | supply | timestamp
+    blanks    = 1 <<31
 
 
 ######################################################################
 # Main
 
 def dumpPrices(
             dbPath,             # Path() or str
@@ -38,28 +34,28 @@
     ):
     """
         Generate a prices list using data from the DB.
         If stationID is not none, only the specified station is dumped.
         If file is not none, outputs to the given file handle.
     """
     
-    withTimes  = (elementMask & Element.timestamp)
-    getBlanks  = (elementMask & Element.blanks)
+    withTimes  = elementMask & Element.timestamp
+    getBlanks  = elementMask & Element.blanks
     
     conn = sqlite3.connect(str(dbPath))
     conn.execute("PRAGMA foreign_keys=ON")
     cur  = conn.cursor()
     
-    systems = { ID: name for (ID, name) in cur.execute("SELECT system_id, name FROM System") }
+    systems = dict(cur.execute("SELECT system_id, name FROM System"))
     stations = {
         ID: [ name, systems[sysID] ]
         for (ID, name, sysID)
         in cur.execute("SELECT station_id, name, system_id FROM Station")
     }
-    categories = { ID: name for (ID, name) in cur.execute("SELECT category_id, name FROM Category") }
+    categories = dict(cur.execute("SELECT category_id, name FROM Category"))
     items = {
         ID: [ name, catID, categories[catID] ]
         for (ID, name, catID)
         in cur.execute("SELECT item_id, name, category_id FROM Item")
     }
     
     # find longest item name
@@ -114,17 +110,18 @@
         defDemand=defaultDemandVal,
         itemJoin=itemJoin,
     )
     if debug:
         print(sql)
     cur.execute(sql)
     
-    lastSys, lastStn, lastCat = None, None, None
+    lastStn, lastCat = None, None
     
-    if not file: file = sys.stdout
+    if not file:
+        file = sys.stdout
     
     if stationID:
         stationSet = str(stations[stationID])
     else:
         stationSet = "ALL Systems/Stations"
     
     file.write(
@@ -222,11 +219,13 @@
                     fromStn, toStn,
                     demandStr, supplyStr,
                     modified
                 )
     
     file.write(output)
 
-if __name__ == "__main__":
-    import tradedb
-    tdb = tradedb.TradeDB(load=False)
-    dumpPrices(tdb.dbPath, elementMask=Element.full)
+
+# if __name__ == "__main__":
+#     import tradedb
+# 
+#     tdb = tradedb.TradeDB(load=False)
+#     dumpPrices(tdb.dbPath, elementMask=Element.full)
```

### Comparing `tradedangerous-10.9.8/tradedangerous/fs.py` & `tradedangerous-11.0.0/tradedangerous/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module should handle filesystem related operations
 """
 from shutil import copy as shcopy
-from os import makedirs, path, utime
+from os import makedirs
 from pathlib import Path
 
 __all__ = ['copy', 'copyallfiles', 'touch', 'ensurefolder']
 
 def pathify(*args):
     if len(args) > 1 or not isinstance(args[0], Path):
         return Path(*args)
@@ -21,27 +21,27 @@
     srcPath = pathify(src).resolve()
     dstPath = pathify(dst)
     shcopy(str(srcPath), str(dstPath))
     return dstPath
 
 def copy_if_newer(src, dst):
     """
-    copy src to dst if src is newer 
+    copy src to dst if src is newer
     takes string or Path object as input
     returns Path(dst) on success
     returns Path(src) if not newer
     raises FileNotFoundError if src does not exist
     """
     srcPath = pathify(src).resolve()
     dstPath = pathify(dst)
-    if dstPath.exists() and not (dstPath.stat().st_mtime < srcPath.stat().st_mtime):
+    if dstPath.exists() and dstPath.stat().st_mtime >= srcPath.stat().st_mtime:
         return srcPath
-    else:
-        shcopy(str(srcPath), str(dstPath))
-        return dstPath
+
+    shcopy(str(srcPath), str(dstPath))
+    return dstPath
 
 def copyallfiles(srcdir, dstdir):
     """
     Copies all files in srcdir to dstdir
     """
     srcPath = pathify(srcdir)
     dstPath = pathify(dstdir)
```

### Comparing `tradedangerous-10.9.8/tradedangerous/jsonprices.py` & `tradedangerous-11.0.0/tradedangerous/jsonprices.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,33 +20,26 @@
     if not system:
         try:
             system = tdb.lookupSystem(name)
         except LookupError:
             pass
     
     if system:
-        if (system.posX != x or system.posY != y or system.posZ != z):
+        if system.posX != x or system.posY != y or system.posZ != z:
             raise Exception("System {} position mismatch: "
                     "Got {},{},{} expected {},{},{}".format(
                         name,
                         x, y, z,
                         system.posX, system.posY, system.posZ
             ))
         return system
     
-    newSystem = "@{} [{}, {}, {}]".format(
-            name, x, y, z
-    )
-    
     candidates = []
     for candidate in tdb.systemByID.values():
-        if (candidate.posX == x and
-                candidate.posY == y and
-                candidate.posZ == z
-                ):
+        if candidate.posX == x and candidate.posY == y and candidate.posZ == z:
             candidates.append(candidate)
     
     if len(candidates) == 1:
         candidate = candidates[0]
         if candidate.casefold() != name.casefold():
             if not tdenv.quiet:
                 print("System name mismatch: "
@@ -57,18 +50,17 @@
                             candidate.dbname,
                             candidate.posX,
                             candidate.posY,
                             candidate.posZ,
                 ))
         return candidates[0]
     
-    if len(candidates):
-        raise Exception("System {} matches co-ordinates for systems: {}" +
-                ','.join([system.name for system in candidates])
-                )
+    if candidates:
+        options = ', '.join([s.name for s in candidates])
+        raise RuntimeError(f"System {system.name} matches co-ordinates for systems: {options}")
     
     if tdenv.addUnknown:
         return tdb.addLocalSystem(name, x, y, z)
     
     return None
 
 def lookup_station(
@@ -87,15 +79,15 @@
     if not station:
         if not tdenv.addUnknown:
             return None
         station = tdb.addLocalStation(system, name)
     
     # Now set the parameters
     tdb.updateLocalStation(
-            stn, lsFromStar, blackMarket, maxPadSize
+            station, lsFromStar, blackMarket, maxPadSize
     )
     return station
 
 def load_prices_json(
         tdb,
         tdenv,
         jsonText
@@ -112,15 +104,15 @@
     
     stnData = data['stn']
     stnName = stnData['name']
     lsFromStar = stnData['ls']
     
     try:
         blackMarket = stnData['bm'].upper()
-        if not blackMarket in [ 'Y', 'N' ]:
+        if blackMarket not in [ 'Y', 'N' ]:
             blackMarket = '?'
     except KeyError:
         blackMarket = '?'
     
     system = lookup_system(
             tdb, tdenv,
             sysName,
@@ -133,15 +125,15 @@
             print("NOTE: Ignoring unknown system: {} [{},{},{}]".format(
                     sysName,
                     pos[0], pos[1], pos[2],
             ))
         return
     if system.dbname != sysName and tdenv.detail:
         print("NOTE: Treating '{}' as '{}'".format(
-                name, system.dbname
+                sysName, system.dbname
         ))
     tdenv.DEBUG1("- System: {}", system.dbname)
     
     station = lookup_station(
             tdb, tdenv,
             system,
             stnName,
```

### Comparing `tradedangerous-10.9.8/tradedangerous/utils.py` & `tradedangerous-11.0.0/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.8/tradedangerous/submit-distances.py` & `tradedangerous-11.0.0/tradedangerous/submit-distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,16 @@
 """
 
 #
 # NOTE: This tool is very hacky. If someone wants to clean it up,
 # and submit a diff, that'd be greatly appreciated!
 #
 
-from __future__ import print_function
-
 import argparse
-import json
-import math
 import os
-import pathlib
-import platform
 import random
 import re
 import sys
 import tradedb
 import tradeenv
 
 from misc.edsc import StarSubmission, StarSubmissionResult, SubmissionError
@@ -48,30 +42,31 @@
         "Do you want me to try and install it with the package manager (y/n)? "
     )
     if approval.lower() != 'y':
         print("You didn't type 'y' so I'm giving up.")
         raise e
     import pip
     pip.main(["install", "--upgrade", "requests"])
-    import requests
+    import requests  # noqa: F401
 
 standardStars = [
     "SOL",
     "NEW YEMBO",
     "VESUVIT",
     "HIP 79884",
     "ASELLUS AUSTRALIS",
 ]
 
 ############################################################################
 
 
 class UsageError(Exception):
     def __init__(self, argv, error):
-       self.argv, self.error = argv, error
+        self.argv, self.error = argv, error
+        
     def __str__(self):
         return error + "\n" + argv.format_usage()
 
 def parse_arguments():
     parser = argparse.ArgumentParser(
         description='Submit star distances to the EDSC project.',
     )
@@ -180,15 +175,15 @@
     ], num)
     
     return destinations
 
 def get_outliers(argv):
     outliers = set()
     try:
-        with open(argv.extraFile, "rU", encoding="utf-8") as input:
+        with open(argv.extraFile, "r", encoding="utf-8") as input:
             for line in input:
                 name = line.partition('#')[0].strip().upper()
                 if name and name != argv.origin:
                     outliers.add(name)
     except FileNotFoundError:
         pass
     outliers = list(outliers)
```

### Comparing `tradedangerous-10.9.8/tradedangerous/trade.py` & `tradedangerous-11.0.0/tradedangerous/trade.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 #!/usr/bin/env python3
 # --------------------------------------------------------------------
 # Copyright (C) Oliver 'kfsone' Smith 2014 <oliver@kfs.org>:
 # Copyright (C) Bernd 'Gazelle' Gollesch 2016, 2017
-# Copyright (C) Jonathan 'eyeonus' Jones 2018, 2019
+# Copyright (C) Jonathan 'eyeonus' Jones 2018-2022
 #
 # You are free to use, redistribute, or even print and eat a copy of
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 # TradeDangerous :: Command Line App :: Main Module
-#
+# 
+# This is the main entry point into the native TD CLI.
+# 
 # TradeDangerous is a powerful set of tools for traders in Frontier
 # Development's game "Elite: Dangerous". It's main function is
 # calculating the most profitable trades between either individual
 # stations or working out "profit runs".
-#
+# 
 # I wrote TD because I realized that the best trade run - in terms
 # of the "average profit per stop" was rarely as simple as going
 # Chango -> Dahan -> Chango.
-#
+# 
 # E:D's economy is complex; sometimes you can make the most profit
 # by trading one item A->B and flying a second item B->A.
 # But more often you need to fly multiple stations, especially since
 # as you are making money different trade options are coming into
 # your affordable range.
-#
+# 
 # END USERS: If you are a user looking to find out how to use TD,
 # please consult the file "README.md".
-#
+# 
 # DEVELOPERS: If you are a programmer who wants TD to do something
 # cool, please see the TradeDB and TradeCalc modules. TD is designed
 # to empower other programmers to do cool stuff.
+from __future__ import annotations
 
-from tradedangerous import cli, gui
+from tradedangerous import cli
 
+import sys
+    
 
-def main(argv = None):
-    import sys
-    if 1 < len(sys.argv) and sys.argv[1] == 'gui':
-        gui.main()
-    else:
-        cli.main(sys.argv)
+def main(argv: list[tuple] = None) -> None:
+    """ Entry point for the TradeDangerous command-line app. """
+    if argv is None:
+        argv = sys.argv
+    cli.main(argv)
 
 
 if __name__ == "__main__":
-    import sys
-    if 1 < len(sys.argv) and sys.argv[1] == 'gui':
-        gui.main()
-    else:
-        cli.main(sys.argv)
-    
+    cli.main(sys.argv)
```

### Comparing `tradedangerous-10.9.8/tradedangerous/version.py` & `tradedangerous-11.0.0/tradedangerous/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '10.9.8'
+__version__ = '11.0.0'
```

### Comparing `tradedangerous-10.9.8/tradedangerous/mfd/__init__.py` & `tradedangerous-11.0.0/tradedangerous/mfd/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # Copyright (C) Oliver 'kfsone' Smith 2014 <oliver@kfs.org>:
 #  You are free to use, redistribute, or even print and eat a copy of
 #  this software so long as you include this copyright notice.
 #  I guarantee there is at least one bug neither of us knew about.
-#---------------------------------------------------------------------
+# ---------------------------------------------------------------------
 # TradeDangerous :: Modules :: Multi-function display wrapper
 #
 #   Multi-Function Display wrappers
 
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-
 ######################################################################
 # imports
 
 import sys
 import time
 
 
@@ -24,15 +22,15 @@
         Throw when no instance of a device cannot be found.
     """
     pass
 
 ######################################################################
 # classes
 
-class DummyMFD(object):
+class DummyMFD:
     """
         Base class for the MFD drivers, implemented as no-ops so that
         you can always use all MFD functions without conditionals.
     """
     
     def __init__(self):
         pass
```

### Comparing `tradedangerous-10.9.8/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-11.0.0/tradedangerous/mfd/saitek/directoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,23 @@
 DirectOutput_SetString
 
 DirectOutput_StartServer
 DirectOutput_CloseServer
 
 """
 
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-
-from mfd import MissingDeviceError
+from tradedangerous.mfd import MissingDeviceError
 
 import ctypes
 import ctypes.wintypes
 import logging
 import os
 import platform
+import sys
+import time
 
 S_OK = 0x00000000
 E_HANDLE = 0x80070006
 E_INVALIDARG = 0x80070057
 E_OUTOFMEMORY = 0x8007000E
 E_PAGENOTACTIVE = -0xfbffff        # Something munges it from it's actual value
 E_BUFFERTOOSMALL = -0xfc0000
@@ -80,16 +80,15 @@
 ERROR_DEV_NOT_EXIST = 55
 
 SOFTBUTTON_SELECT = 0x00000001
 SOFTBUTTON_UP = 0x00000002
 SOFTBUTTON_DOWN = 0x00000004
 
 
-class DirectOutput(object):
-    
+class DirectOutput:
     def __init__(self, dll_path):
         """
         Creates python object to interact with DirecOutput.dll
         
         Required Arguments:
         dll_path -- String containing DirectOutput.dll location.
         
@@ -160,47 +159,47 @@
         Required Arugments:
         device_handle -- ID of device
         function -- Function to call when a soft button changes
         
         Returns:
         S_OK: The call completed successfully.
         E_HANDLE: The device handle specified is invalid.
-        
         """
+        
         logging.debug("DirectOutput.RegisterSoftButtonCallback({}, {})".format(device_handle, function))
-        return self.DirectOutputDLL.DirectOutput_RegisterSoftButtonCallback(device_handle, function, 0)
+        return self.DirectOutputDLL.DirectOutput_RegisterSoftButtonCallback(ctypes.wintypes.HANDLE(device_handle), function, 0)
     
     def RegisterPageCallback(self, device_handle, function):
         """
         Registers a function to be called when page changes
         
         Required Arugments:
         device_handle -- ID of device
         function -- Function to call when a page changes
         
         Returns:
         S_OK: The call completed successfully.
         E_HANDLE: The device handle specified is invalid.
         """
         logging.debug("DirectOutput.RegisterPageCallback({}, {})".format(device_handle,function))
-        return self.DirectOutputDLL.DirectOutput_RegisterPageCallback(device_handle, function, 0)
+        return self.DirectOutputDLL.DirectOutput_RegisterPageCallback(ctypes.wintypes.HANDLE(device_handle), function, 0)
     
     def SetProfile(self, device_handle, profile):
         """
         Sets the profile used on the device.
         
         Required Arguments:
         device_handle -- ID of device
         profile -- full path of the profile to activate. passing None will clear the profile.
         """
         logging.debug("DirectOutput.SetProfile({}, {})".format(device_handle, profile))
         if profile:
-            return self.DirectOutputDLL.DirectOutput_SetProfile(device_handle, len(profile), ctypes.wintypes.LPWSTR(profile))
+            return self.DirectOutputDLL.DirectOutput_SetProfile(ctypes.wintypes.HANDLE(device_handle), len(profile), ctypes.wintypes.LPWSTR(profile))
         else:
-            return self.DirectOutputDLL.DirectOutput_SetProfile(device_handle, 0, 0)
+            return self.DirectOutputDLL.DirectOutput_SetProfile(ctypes.wintypes.HANDLE(device_handle), 0, 0)
     
     def AddPage(self, device_handle, page, name, active):
         """
         Adds a page to the MFD
         
         Required Arguments:
         device_handle -- ID of device
@@ -212,15 +211,15 @@
         S_OK: The call completed successfully.
         E_OUTOFMEMORY: Insufficient memory to complete the request.
         E_INVALIDARG: The dwPage parameter already exists.
         E_HANDLE: The device handle specified is invalid.
         
         """
         logging.debug("DirectOutput.AddPage({}, {}, {}, {})".format(device_handle, page, name, active))
-        return self.DirectOutputDLL.DirectOutput_AddPage(device_handle, page, active)
+        return self.DirectOutputDLL.DirectOutput_AddPage(ctypes.wintypes.HANDLE(device_handle), page, active)
     
     def RemovePage(self, device_handle, page):
         """
         Removes a page from the MFD
         
         Required Arguments:
         device_handle -- ID of device
@@ -229,15 +228,15 @@
         Returns:
         S_OK: The call completed successfully.
         E_INVALIDARG: The dwPage argument does not reference a valid page id.
         E_HANDLE: The device handle specified is invalid.
         
         """
         logging.debug("DirectOutput.RemovePage({}, {})".format(device_handle, page))
-        return self.DirectOutputDLL.DirectOutput_RemovePage(device_handle, page)
+        return self.DirectOutputDLL.DirectOutput_RemovePage(ctypes.wintypes.HANDLE(device_handle), page)
     
     def SetLed(self, device_handle, page, led, value):
         """
         Sets LED state on a given page
         
         Required Arguments:
         device_handle -- ID of device
@@ -248,15 +247,15 @@
         Returns:
         S_OK: The call completes successfully.
         E_INVALIDARG: The dwPage argument does not reference a valid page id, or the dwLed argument does not specifiy a valid LED id.
         E_HANDLE: The device handle specified is invalid
         
         """
         logging.debug("DirectOutput.SetLed({}, {}, {}, {})".format(device_handle, page, led, value))
-        return self.DirectOutputDLL.DirectOutput_SetLed(device_handle, page, led, value)
+        return self.DirectOutputDLL.DirectOutput_SetLed(ctypes.wintypes.HANDLE(device_handle), page, led, value)
 
 
     def SetString(self, device_handle, page, line, string):
         """
         Sets a string to display on the MFD
         
         Required Arguments:
@@ -269,20 +268,20 @@
         S_OK: The call completes successfully.
         E_INVALIDARG: The dwPage argument does not reference a valid page id, or the dwString argument does not reference a valid string id.
         E_OUTOFMEMORY: Insufficient memory to complete the request.
         E_HANDLE: The device handle specified is invalid.
         
         """
         logging.debug("DirectOutput.SetString({}, {}, {}, {})".format(device_handle, page, line, string))
-        return self.DirectOutputDLL.DirectOutput_SetString(device_handle, page, line, len(string), ctypes.wintypes.LPWSTR(string))
+        return self.DirectOutputDLL.DirectOutput_SetString(ctypes.wintypes.HANDLE(device_handle), page, line, len(string), ctypes.wintypes.LPWSTR(string))
 
 
-class DirectOutputDevice(object):
+class DirectOutputDevice:
     
-    class Buttons(object):
+    class Buttons:
         
         select, up, down = False, False, False
         
         def __init__(self, bitmask):
             self.bitmask = bitmask
             if bitmask == 1:
                 self.select = True
@@ -324,15 +323,15 @@
         if platform.machine().endswith('86'):
             # 32-bit machine, nothing to worry about
             pass
         elif platform.machine().endswith('64'):
             # 64-bit machine, are we a 32-bit python?
             if platform.architecture()[0] == '32bit':
                 prog_dir = os.environ["ProgramFiles(x86)"]
-        dll_path = os.path.join(prog_dir, "Saitek\\DirectOutput\\DirectOutput.dll")
+        dll_path = os.path.join(prog_dir, "Logitech\\DirectOutput\\DirectOutput.dll")
         
         self.application_name = name or DirectOutputDevice.application_name
         self.debug_level = debug_level
         
         try:
             logging.debug("DirectOutputDevice -> DirectOutput: {}".format(dll_path))
             self.direct_output = DirectOutput(dll_path)
@@ -654,16 +653,14 @@
 if __name__ == '__main__':
     # If you want it to go to a file?
     # logging.basicConfig(filename='directoutput.log', filemode='w', level=logging.DEBUG, format='%(asctime)s %(name)s [%(filename)s:%(lineno)d] %(message)s')
     # If you want less verbose logging?
     # logging.basicConfig(level=logging.INFO, format='%(asctime)s %(name)s [%(filename)s:%(lineno)d] %(message)s')
     logging.basicConfig(level=logging.DEBUG, format='%(asctime)s %(name)s [%(filename)s:%(lineno)d] %(message)s')
     
-    import time, sys
-    
     device = DirectOutputDevice(debug_level=1)
     print("Device initialized")
     
     device.AddPage(0, "Test", True)
     print("Test Page added")
     
     device.SetString(0, 0, "Test String")
@@ -671,11 +668,11 @@
     
     device.AddPage(1, "Other", False)
     device.AddPage(2, "Another", False)
     
     while True:
         try:
             time.sleep(1)
-        except:
-            #This is used to catch Ctrl+C, calling finish method is *very* important to de-initalize device.
+        except:  # noqa: E722
+            # This is used to catch Ctrl+C, calling finish method is *very* important to de-initalize device.
             device.finish()
             sys.exit()
```

### Comparing `tradedangerous-10.9.8/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-11.0.0/tradedangerous/mfd/saitek/x52pro.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 Description: Python class implementing specific functions for Saitek X52 Pro
 
 
 TODO:
     * Error handling and exceptions
 """
 
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
+from tradedangerous.mfd.saitek.directoutput import DirectOutputDevice
 
-from mfd.saitek.directoutput import DirectOutputDevice
+import sys
+import time
 
 
 class X52Pro(DirectOutputDevice):
-    class Page(object):
+    class Page:
         _lines = [ str(), str(), str() ]
         _leds  = dict()
         
         def __init__(self, device, page_id, name, active):
             self.device = device
             self.page_id = page_id
             self.name = name
@@ -41,15 +42,15 @@
         
         def __setitem__(self, key, value):
             self._lines[key] = value
             if self.active:
                 self.device.SetString(self.page_id, key, value)
         
         def activate(self):
-            if self.active == True:
+            if self.active is True:
                 return
             self.device.AddPage(self.page_id, self.name, 1)
         
         def refresh(self):
             # Resend strings to the display
             for lineNo, string in enumerate(self._lines):
                 self.device.SetString(self.page_id, lineNo, string)
@@ -168,16 +169,14 @@
     print("Adding second page")
     x52.add_page("Page2", active=False)
     x52.pages["Page2"][0] = "Second Page Is Right Here"
     x52.pages["Page2"][1] = "-- Page 2 [1]"
     
     print("Looping")
     
-    import time, sys
-    
     loopNo = 0
     while True:
         try:
             loopNo += 1
             x52.pages["Page1"][2] = "Loop #" + str(loopNo)
             time.sleep(0.25)
             x52.pages["Page1"].fire_a("red")
@@ -190,8 +189,7 @@
             fireToggle = ~fireToggle
             x52.pages["Page1"].fire(fireToggle)
             x52.pages["Page1"].throttle_axis(~fireToggle)
         except Exception as e:
             print(e)
             x52.finish()
             sys.exit()
-
```

### Comparing `tradedangerous-10.9.8/tradedangerous/tradedb.py` & `tradedangerous-11.0.0/tradedangerous/tradedb.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,48 +45,40 @@
     abe = tdb.lookupPlace("sol/abraham lincoln")
     abe = tdb.lookupPlace("@sol/abrahamlincoln")
     james = tdb.lookupPlace("shin/jamesmem")
 """
 
 ######################################################################
 # Imports
+from __future__ import annotations
 
-
-from collections import namedtuple, defaultdict
+from collections import namedtuple
+from contextlib import closing
+from math import sqrt as math_sqrt
 from pathlib import Path
-from .tradeenv import TradeEnv
-from .tradeexcept import TradeException
-
-from . import cache, fs
 import heapq
 import itertools
 import locale
-import math
-import os
 import re
 import sqlite3
 import sys
+import typing
+
+from .tradeenv import TradeEnv
+from .tradeexcept import TradeException
+from . import cache, fs
+
+if typing.TYPE_CHECKING:
+    from typing import Generator
+    from typing import Optional, Union
 
-haveNumpy = False
-try:
-    import numpy
-    import numpy.linalg
-    haveNumpy = True
-except (KeyError, ImportError):
-    pass
-if not haveNumpy:
-    class numpy(object):
-        array = False
-        float32 = False
-        ascontiguousarray = False
-        class linalg(object):
-            norm = False
 
 locale.setlocale(locale.LC_ALL, '')
 
+
 ######################################################################
 # Classes
 
 class AmbiguityError(TradeException):
     """
         Raised when a search key could match multiple entities.
         Attributes:
@@ -110,110 +102,72 @@
                 key(c) for c in anyMatch[:10]
             ] + ["..."])
         else:
             opportunities = ", ".join(
                 key(c) for c in anyMatch[0:-1]
             )
             opportunities += " or " + key(anyMatch[-1])
-        return '{} "{}" could match {}'.format(
-            self.lookupType, str(self.searchKey),
-            opportunities
-        )
+        return f'{self.lookupType} "{self.searchKey}" could match {opportunities}'
 
 class SystemNotStationError(TradeException):
     """
         Raised when a station lookup matched a System but
         could not be automatically reduced to a Station.
     """
-    pass
+    pass  # pylint: disable=unnecessary-pass  # (it's not)
+
 
 ######################################################################
 
 
-def makeStellarGridKey(x, y, z):
+def make_stellar_grid_key(x: float, y: float, z: float) -> int:
     """
     The Stellar Grid is a map of systems based on their Stellar
     co-ordinates rounded down to 32lys. This makes it much easier
     to find stars within rectangular volumes.
     """
     return (int(x) >> 5, int(y) >> 5, int(z) >> 5)
 
-class System(object):
+
+class System:
     """
     Describes a star system which may contain one or more Station objects.
     
     Caution: Do not use _rangeCache directly, use TradeDB.genSystemsInRange.
     """
     
     __slots__ = (
         'ID',
         'dbname', 'posX', 'posY', 'posZ', 'pos', 'stations',
         'addedID',
         '_rangeCache'
     )
     
-    class RangeCache(object):
+    class RangeCache:
         """
         Lazily populated cache of neighboring systems.
         """
         def __init__(self):
             self.systems = []
-            self.probedLy = 0.
+            self.probed_ly = 0.
     
-    def __init__(
-            self, ID, dbname, posX, posY, posZ, addedID,
-            ary=numpy.array,
-            nptype=numpy.float32,
-            ):
+    def __init__(self, ID, dbname, posX, posY, posZ, addedID) -> None:
         self.ID = ID
         self.dbname = dbname
         self.posX, self.posY, self.posZ = posX, posY, posZ
-        if ary:
-            self.pos = ary([posX, posY, posZ], nptype)
         self.addedID = addedID or 0
         self.stations = ()
         self._rangeCache = None
     
     @property
-    def system(self):
+    def system(self) -> 'System':
+        """ Returns self for compatibility with the undefined 'Positional' interface. """
         return self
     
-    def distToSq(self, other):
-        """
-        Returns the square of the distance between two systems.
-        
-        It is slightly cheaper to calculate the square of the
-        distance between two points, so when you are primarily
-        doing distance checks you can use this less expensive
-        distance query and only perform a sqrt (** 0.5) on the
-        distances that fall within your constraint.
-        
-        Args:
-            other:
-                The other System to measure the distance between.
-        
-        Returns:
-            Distance in light years to the power of 2 (i.e. squared).
-        
-        Example:
-            # Calculate which of [systems] is within 12 ly
-            # of System "target".
-            maxLySq = 12 ** 2   # Maximum of 12 ly.
-            inRange = []
-            for sys in systems:
-                if sys.distToSq(target) <= maxLySq:
-                    inRange.append(sys)
-        """
-        return (
-            (self.posX - other.posX) ** 2 +
-            (self.posY - other.posY) ** 2 +
-            (self.posZ - other.posZ) ** 2
-        )
-    
-    def distanceTo(self, other):
+    def distanceTo(self, other: 'System') -> float:
         """
         Returns the distance (in ly) between two systems.
         
         NOTE: If you are primarily testing/comparing
         distances, consider using "distToSq" for the test.
         
         Returns:
@@ -221,104 +175,90 @@
         
         Example:
             print("{} -> {}: {} ly".format(
                 lhs.name(), rhs.name(),
                 lhs.distanceTo(rhs),
             ))
         """
-        return (
-            (self.posX - other.posX) ** 2 +
-            (self.posY - other.posY) ** 2 +
-            (self.posZ - other.posZ) ** 2
-        ) ** 0.5  # fast sqrt
-    
-    if haveNumpy:
-        def all_distances(
-                self, iterable,
-                ary=numpy.ascontiguousarray, norm=numpy.linalg.norm,
-                ):
-            """
-            Takes a list of systems and returns their distances from this system.
-            """
-            return numpy.linalg.norm(
-                ary([s.pos for s in iterable]) - self.pos,
-                ord=2, axis=1.
-            )
+        dx, dy, dz = self.posX - other.posX, self.posY - other.posY, self.posZ - other.posZ
+        return math_sqrt(dx * dx + dy * dy + dz * dz)
     
-    def getStation(self, stationName):
+    def getStation(self, name: str) -> 'Optional[Station]':
         """
         Quick case-insensitive lookup of a station name within the
         stations in this system.
         
         Returns:
             Station() object if a match is found,
             otherwise None.
         """
-        upperName = stationName.upper()
+        name = name.upper()
         for station in self.stations:
-            if station.dbname.upper() == upperName:
+            if station.name == name:
                 return station
         return None
     
-    def name(self, detail=0):
+    def name(self, detail: int = 0) -> str:     # pylint: disable=unused-argument
+        """ Returns the display name for this System."""
         return self.dbname
     
-    def str(self):
+    def text(self) -> str:
         return self.dbname
 
 ######################################################################
 
 class Destination(namedtuple('Destination', [
         'system', 'station', 'via', 'distLy'
         ])):
     pass
 
 class DestinationNode(namedtuple('DestinationNode', [
         'system', 'via', 'distLy'
         ])):
     pass
 
-class Station(object):
+class Station:
     """
     Describes a station (trading or otherwise) in a system.
     
     For obtaining trade information for a given station see one of:
         TradeCalc.getTrades        (fast and cheap)
     """
     __slots__ = (
         'ID', 'system', 'dbname',
         'lsFromStar', 'market', 'blackMarket', 'shipyard', 'maxPadSize',
         'outfitting', 'rearm', 'refuel', 'repair', 'planetary','fleet',
-        'itemCount', 'dataAge',
+        'odyssey', 'itemCount', 'dataAge',
     )
     
     def __init__(
             self, ID, system, dbname,
             lsFromStar, market, blackMarket, shipyard, maxPadSize,
-            outfitting, rearm, refuel, repair, planetary, fleet,
+            outfitting, rearm, refuel, repair, planetary, fleet, odyssey,
             itemCount=0, dataAge=None,
             ):
         self.ID, self.system, self.dbname = ID, system, dbname
         self.lsFromStar = int(lsFromStar)
         self.market = market if itemCount == 0 else 'Y'
         self.blackMarket = blackMarket
         self.shipyard = shipyard
         self.maxPadSize = maxPadSize
         self.outfitting = outfitting
         self.rearm = rearm
         self.refuel = refuel
         self.repair = repair
         self.planetary = planetary
         self.fleet = fleet
+        self.odyssey = odyssey
         self.itemCount = itemCount
         self.dataAge = dataAge
         system.stations = system.stations + (self,)
     
-    def name(self, detail=0):
-        return '%s/%s' % (self.system.dbname, self.dbname)
+    def name(self, detail: int = 0) -> str:  # pylint: disable=unused-argument
+        return f"{self.system.dbname}/{self.dbname}"
     
     def checkPadSize(self, maxPadSize):
         """
         Tests if the Station's max pad size matches one of the
         values in 'maxPadSize'.
         
         Args:
@@ -373,80 +313,83 @@
         return (not planetary or self.planetary in planetary)
     
     def checkFleet(self, fleet):
         """
         Same as checkPlanetary, but for fleet carriers.
         """
         return (not fleet or self.fleet in fleet)
-    
-    
-    def distFromStar(self, addSuffix=False):
+
+
+    def checkOdyssey(self, odyssey):
+        """
+        Same as checkPlanetary, but for Odyssey.
+        """
+        return (not odyssey or self.odyssey in odyssey)
+
+
+    def distFromStar(self, addSuffix: bool = False) -> str:
         """
         Returns a textual description of the distance from this
         Station to the parent star.
         
         Args:
             addSuffix[=False]:
                 Always add a unit suffix (ls, Kls, ly)
         """
         ls = self.lsFromStar
         if not ls:
-            if addSuffix:
-                return "Unk"
-            else:
-                return '?'
+            return "Unk" if addSuffix else "?"
+        
+        suffix = "ls" if addSuffix else ""
+        
         if ls < 1000:
-            suffix = 'ls' if addSuffix else ''
-            return '{:n}'.format(ls)+suffix
+            return f"{ls:n}{suffix}"
         if ls < 10000:
-            suffix = 'ls' if addSuffix else ''
-            return '{:.2f}K'.format(ls / 1000)+suffix
+            return f"{ls / 1000:.2f}K{suffix}"
         if ls < 1000000:
-            suffix = 'ls' if addSuffix else ''
-            return '{:n}K'.format(int(ls / 1000))+suffix
-        return '{:.2f}ly'.format(ls / (365*24*60*60))
+            return f"{int(ls / 1000):n}K{suffix}"
+        return f'{ls / (365*24*60*60):.2f}ly'
     
     @property
-    def isTrading(self):
+    def isTrading(self) -> bool:
         """
         True if the station is thought to be trading.
         
         A station is considered 'trading' if it has an item count > 0 or
         if it's "market" column is flagged 'Y'.
         """
         return (self.itemCount > 0 or self.market == 'Y')
     
     @property
     def itemDataAgeStr(self):
         """ Returns the age in days of item data if present, else "-". """
         if self.itemCount and self.dataAge:
-            return "{:7.2f}".format(self.dataAge)
+            return f"{self.dataAge:7.2f}"
         return "-"
     
-    def str(self):
-        return '%s/%s' % (self.system.dbname, self.dbname)
+    def text(self) -> str:
+        return f"{self.system.dbname}/{self.dbname}"
 
 ######################################################################
 
 
 class Ship(namedtuple('Ship', (
-        'ID', 'dbname', 'cost', 'fdevID', 'stations'
+        'ID', 'dbname', 'cost', 'stations'
         ))):
     """
     Ship description.
     
     Attributes:
-        ID          -- The database ID
+        ID          -- FDevID as provided by the companion API.
         dbname      -- The name as present in the database
         cost        -- How many credits to buy
-        fdevID      -- FDevID as provided by the companion API.
         stations    -- List of Stations ship is sold at.
     """
     
-    def name(self, detail=0):
+    def name(self, detail=0):   # pylint: disable=unused-argument
         return self.dbname
 
 ######################################################################
 
 
 class Category(namedtuple('Category', (
         'ID', 'dbname', 'items'
@@ -466,21 +409,21 @@
             List of Item objects within this category.
     
     Member Functions:
         name()
             Returns the display name for this Category.
     """
     
-    def name(self, detail=0):
+    def name(self, detail=0):   # pylint: disable=unused-argument
         return self.dbname.upper()
 
 ######################################################################
 
 
-class Item(object):
+class Item:
     """
     A product that can be bought/sold in the game.
     
     Attributes:
         ID       -- Database ID.
         dbname   -- Name as it appears in-game and in the DB.
         category -- Reference to the category.
@@ -542,15 +485,15 @@
     """
     def name(self, detail=0):
         return self.item.name(detail=detail)
 
 ######################################################################
 
 
-class TradeDB(object):
+class TradeDB:
     """
     Encapsulation for the database layer.
     
     Attributes:
         dataPath
             Path() to the data directory
         dbPath
@@ -612,102 +555,109 @@
         ('Item.csv', 'Item'),
         ('RareItem.csv', 'RareItem'),
         ('FDevShipyard.csv', 'FDevShipyard'),
         ('FDevOutfitting.csv', 'FDevOutfitting'),
     )
     
     # Translation matrixes for attributes -> common presentation
-    marketStates = planetStates = fleetStates = {'?': '?', 'Y': 'Yes', 'N': 'No'}
-    marketStatesExt = planetStatesExt = fleetStatesExt = {'?': 'Unk', 'Y': 'Yes', 'N': 'No'}
+    marketStates = planetStates = fleetStates = odysseyStates = {'?': '?', 'Y': 'Yes', 'N': 'No'}
+    marketStatesExt = planetStatesExt = fleetStatesExt = odysseyStatesExt = {'?': 'Unk', 'Y': 'Yes', 'N': 'No'}
     padSizes = {'?': '?', 'S': 'Sml', 'M': 'Med', 'L': 'Lrg'}
     padSizesExt = {'?': 'Unk', 'S': 'Sml', 'M': 'Med', 'L': 'Lrg'}
     
     def __init__(
             self,
             tdenv=None,
             load=True,
             debug=None,
             ):
-        self.conn = None
-        self.cur = None
+        self.conn: sqlite3.Connection = None
         self.tradingCount = None
         
         tdenv = tdenv or TradeEnv(debug=(debug or 0))
         self.tdenv = tdenv
         
         self.templatePath = Path(tdenv.templateDir).resolve()
         self.dataPath = dataPath = fs.ensurefolder(tdenv.dataDir)
+        self.csvPath = fs.ensurefolder(tdenv.csvDir)
         
-        fs.copy_if_newer((self.templatePath / Path("Added.csv")), (self.dataPath / Path("Added.csv")))
-        fs.copy_if_newer((self.templatePath / Path("RareItem.csv")), (self.dataPath / Path("RareItem.csv")))
+        fs.copy_if_newer((self.templatePath / Path("Added.csv")), (self.csvPath / Path("Added.csv")))
+        fs.copy_if_newer((self.templatePath / Path("RareItem.csv")), (self.csvPath / Path("RareItem.csv")))
+        fs.copy_if_newer((self.templatePath / Path("Category.csv")), (self.csvPath / Path("Category.csv")))
         fs.copy_if_newer((self.templatePath / Path("TradeDangerous.sql")), (self.dataPath / Path("TradeDangerous.sql")))
         
         self.dbPath = Path(tdenv.dbFilename or dataPath / TradeDB.defaultDB)
         self.sqlPath = dataPath / Path(tdenv.sqlFilename or TradeDB.defaultSQL)
         pricePath = Path(tdenv.pricesFilename or TradeDB.defaultPrices)
         self.pricesPath = dataPath / pricePath
         self.importTables = [
-            (str(dataPath / Path(fn)), tn)
+            (str(self.csvPath / Path(fn)), tn)
             for fn, tn in TradeDB.defaultTables
         ]
         self.importPaths = {tn: tp for tp, tn in self.importTables}
         
         self.dbFilename = str(self.dbPath)
         self.sqlFilename = str(self.sqlPath)
         self.pricesFilename = str(self.pricesPath)
         
         self.avgSelling, self.avgBuying = None, None
         self.tradingStationCount = 0
+        self.addedByID = None
+        self.systemByID = None
+        self.systemByName = None
+        self.stellarGrid = None
+        self.stationByID = None
+        self.shipByID = None
+        self.categoryByID = None
+        self.itemByID = None
+        self.itemByName = None
+        self.itemByFDevID = None
+        self.rareItemByID = None
+        self.rareItemByName = None
         
         if load:
             self.reloadCache()
             self.load(maxSystemLinkLy=tdenv.maxSystemLinkLy)
     
     @staticmethod
     def calculateDistance2(lx, ly, lz, rx, ry, rz):
         """
         Returns the distance in ly between two points.
         """
-        dX = (lx - rx)
-        dY = (ly - ry)
-        dZ = (lz - rz)
-        distSq = (dX ** 2) + (dY ** 2) + (dZ ** 2)
-        return distSq
+        dx, dy, dz = lx - rx, ly - ry, lz - rz
+        return (dx * dx) + (dy * dy) + (dz * dz)
     
     @staticmethod
     def calculateDistance(lx, ly, lz, rx, ry, rz):
         """
         Returns the distance in ly between two points.
         """
-        dX = (lx - rx)
-        dY = (ly - ry)
-        dZ = (lz - rz)
-        distSq = (dX ** 2) + (dY ** 2) + (dZ ** 2)
-        return distSq ** 0.5
+        dx, dy, dz = lx - rx, ly - ry, lz - rz
+        return math_sqrt((dx * dx) + (dy * dy) + (dz * dz))
     
     ############################################################
     # Access to the underlying database.
     
-    def getDB(self):
+    def getDB(self) -> sqlite3.Connection:
         if self.conn:
             return self.conn
         self.tdenv.DEBUG1("Connecting to DB")
         conn = sqlite3.connect(self.dbFilename)
         conn.execute("PRAGMA foreign_keys=ON")
         conn.execute("PRAGMA synchronous=OFF")
         conn.execute("PRAGMA temp_store=MEMORY")
+        conn.execute("PRAGMA auto_vacuum=INCREMENTAL")
+        
         conn.create_function('dist2', 6, TradeDB.calculateDistance2)
+        self.conn = conn
         return conn
     
     def query(self, *args):
         """ Perform an SQL query on the DB and return the cursor. """
-        conn = self.getDB()
-        cur = conn.cursor()
-        cur.execute(*args)
-        return cur
+        return self.getDB().execute(*args)
     
     def queryColumn(self, *args):
         """ perform an SQL query and return a single column. """
         return self.query(args).fetchone()[0]
     
     def reloadCache(self):
         """
@@ -756,18 +706,18 @@
         """
         Loads the Added table as a simple dictionary
         """
         stmt = """
             SELECT added_id, name
               FROM Added
         """
-        self.cur.execute(stmt)
         addedByID = {}
-        for ID, name in self.cur:
-            addedByID[ID] = name
+        with closing(self.query(stmt)) as cur:
+            for ID, name in cur:
+                addedByID[ID] = name
         self.addedByID = addedByID
         self.tdenv.DEBUG1("Loaded {:n} Addeds", len(addedByID))
     
     def lookupAdded(self, name):
         name = name.lower()
         for ID, added in self.addedByID.items():
             if added.lower() == name:
@@ -788,19 +738,20 @@
         """
         stmt = """
                 SELECT system_id,
                        name, pos_x, pos_y, pos_z,
                        added_id
                   FROM System
             """
-        self.cur.execute(stmt)
+        
         systemByID, systemByName = {}, {}
-        for (ID, name, posX, posY, posZ, addedID) in self.cur:
-            system = System(ID, name, posX, posY, posZ, addedID)
-            systemByID[ID] = systemByName[name.upper()] = system
+        with closing(self.getDB().execute(stmt)) as cur:
+            for (ID, name, posX, posY, posZ, addedID) in cur:
+                system = System(ID, name, posX, posY, posZ, addedID)
+                systemByID[ID] = systemByName[name.upper()] = system
         
         self.systemByID, self.systemByName = systemByID, systemByName
         self.tdenv.DEBUG1("Loaded {:n} Systems", len(systemByID))
     
     def lookupSystem(self, key):
         """
         Look up a System object by it's name.
@@ -898,15 +849,15 @@
         return True
     
     def removeLocalSystem(
             self, system,
             commit=True,
         ):
         """ Removes a system and it's stations from the local DB. """
-        for stn in self.stations:
+        for stn in self.stations():
             self.removeLocalStation(stn, commit=False)
         db = self.getDB()
         db.execute("""
             DELETE FROM System WHERE system_id = ?
         """, [
             system.ID
         ])
@@ -925,17 +876,17 @@
         del system
     
     def __buildStellarGrid(self):
         """
         Divides the galaxy into a fixed-sized grid allowing us to
         aggregate small numbers of stars by locality.
         """
-        stellarGrid = self.stellarGrid = dict()
+        stellarGrid = self.stellarGrid = {}
         for system in self.systemByID.values():
-            key = makeStellarGridKey(system.posX, system.posY, system.posZ)
+            key = make_stellar_grid_key(system.posX, system.posY, system.posZ)
             try:
                 grid = stellarGrid[key]
             except KeyError:
                 grid = stellarGrid[key] = []
             grid.append(system)
     
     def genStellarGrid(self, system, ly):
@@ -956,37 +907,40 @@
                     The *SQUARE* of the distance in light-years
                     between system and candidate.
         """
         if self.stellarGrid is None:
             self.__buildStellarGrid()
         
         sysX, sysY, sysZ = system.posX, system.posY, system.posZ
-        lwrBound = makeStellarGridKey(sysX - ly, sysY - ly, sysZ - ly)
-        uprBound = makeStellarGridKey(sysX + ly, sysY + ly, sysZ + ly)
-        lySq = ly ** 2
+        lwrBound = make_stellar_grid_key(sysX - ly, sysY - ly, sysZ - ly)
+        uprBound = make_stellar_grid_key(sysX + ly, sysY + ly, sysZ + ly)
+        lySq = ly * ly  # in 64-bit python, ** invokes a function call making it 4x expensive as *.
         stellarGrid = self.stellarGrid
         for x in range(lwrBound[0], uprBound[0]+1):
             for y in range(lwrBound[1], uprBound[1]+1):
                 for z in range(lwrBound[2], uprBound[2]+1):
                     try:
                         grid = stellarGrid[(x, y, z)]
                     except KeyError:
                         continue
                     for candidate in grid:
-                        distSq = (candidate.posX - sysX) ** 2
+                        delta = candidate.posX - sysX
+                        distSq = delta * delta
                         if distSq > lySq:
                             continue
-                        distSq += (candidate.posY - sysY) ** 2
+                        delta = candidate.posY - sysY
+                        distSq += delta * delta
                         if distSq > lySq:
                             continue
-                        distSq += (candidate.posZ - sysZ) ** 2
+                        delta = candidate.posZ - sysZ
+                        distSq += delta * delta
                         if distSq > lySq:
                             continue
                         if candidate is not system:
-                            yield candidate, distSq ** 0.5
+                            yield candidate, math_sqrt(distSq)
     
     def genSystemsInRange(self, system, ly, includeSelf=False):
         """
         Yields Systems within a given radius of a specified System.
         Results are sorted by distance and cached for subsequent
         queries in the same run.
         
@@ -1002,40 +956,40 @@
             (candidate, distLy)
                 candidate:
                     System that was found,
                 distLy:
                     The distance in lightyears between system and candidate.
         """
         
-        cache = system._rangeCache
-        if not cache:
-            cache = system._rangeCache = System.RangeCache()
-        cachedSystems = cache.systems
+        cur_cache = system._rangeCache  # pylint: disable=protected-access
+        if not cur_cache:
+            cur_cache = system._rangeCache = System.RangeCache()
+        cached_systems = cur_cache.systems
         
-        if ly > cache.probedLy:
+        if ly > cur_cache.probed_ly:
             # Consult the database for stars we haven't seen.
-            cachedSystems = cache.systems = list(
+            cached_systems = cur_cache.systems = list(
                 self.genStellarGrid(system, ly)
             )
-            cachedSystems.sort(key=lambda ent: ent[1])
-            cache.probedLy = ly
+            cached_systems.sort(key=lambda ent: ent[1])
+            cur_cache.probed_ly = ly
         
         if includeSelf:
             yield system, 0.
         
-        if cache.probedLy > ly:
+        if cur_cache.probed_ly > ly:
             # Cache may contain values outside our view
-            for sys, dist in cachedSystems:
+            for candidate, dist in cached_systems:
                 if dist <= ly:
-                    yield sys, dist
+                    yield candidate, dist
         else:
             # No need to be conditional inside the loop
-            yield from cachedSystems
+            yield from cached_systems
     
-    def getRoute(self, origin, dest, maxJumpLy, avoiding=[], stationInterval=0):
+    def getRoute(self, origin, dest, maxJumpLy, avoiding=None, stationInterval=0):
         """
         Find a shortest route between two systems with an additional
         constraint that each system be a maximum of maxJumpLy from
         the previous system.
         
         Args:
             origin:
@@ -1069,14 +1023,17 @@
             
             The route should be:
                 
                 [(System(A), 0), (System(B), 7), System(C), 15)]
         
         """
         
+        if avoiding is None:
+            avoiding = []
+        
         if isinstance(origin, Station):
             origin = origin.system
         if isinstance(dest, Station):
             dest = dest.system
         
         if origin == dest:
             return ((origin, 0), (dest, 0))
@@ -1105,20 +1062,19 @@
         getDist  = distances.get
         
         destID = dest.ID
         sysByID = self.systemByID
         
         maxPadSize = self.tdenv.padSize
         if not maxPadSize:
-            checkStations = lambda system: bool(system.stations())
+            def checkStations(system: System) -> bool:  # pylint: disable=function-redefined, missing-docstring
+                return bool(system.stations())
         else:
-            checkStations = lambda system: any(
-                stn for stn in system.stations
-                if stn.checkPadSize(maxPadSize)
-            )
+            def checkStations(system: System) -> bool:  # pylint: disable=function-redefined, missing-docstring
+                return any(stn for stn in system.stations if stn.checkPadSize(maxPadSize))
         
         while openSet:
             weight, curDist, curSysID, stnDist = heappop(openSet)
             # If we reached 'goal' we've found the shortest path.
             if curSysID == destID:
                 break
             if curDist >= distTo:
@@ -1168,15 +1124,15 @@
         path.reverse()
         
         return path
     
     ############################################################
     # Station data.
     
-    def stations(self):
+    def stations(self) -> 'Generator[Station, None, None]':
         """ Iterate through the list of stations. """
         yield from self.stationByID.values()
     
     def _loadStations(self):
         """
         Populate the Station list.
         Station constructor automatically adds itself to the System object.
@@ -1184,49 +1140,53 @@
         """
         stmt = """
             SELECT  station_id, system_id, name,
                     ls_from_star, market, blackmarket, shipyard,
                     max_pad_size, outfitting, rearm, refuel, repair, planetary, type_id
               FROM  Station
         """
-        self.cur.execute(stmt)
+        
         stationByID = {}
         systemByID = self.systemByID
         self.tradingStationCount = 0
         # Fleet Carriers are station type 24.
+        # Odyssey settlements are station type 25.
         # Storing as a list allows easy expansion if needed.
-        fc_types = [24]
-        for (
-            ID, systemID, name,
-            lsFromStar, market, blackMarket, shipyard,
-            maxPadSize, outfitting, rearm, refuel, repair, planetary, type_id
-        ) in self.cur:
-            isFleet = 'Y' if int(type_id) in fc_types else 'N'
-            station = Station(
-                ID, systemByID[systemID], name,
+        types = {'fleet-carrier':[24,],'odyssey':[25,],}
+        with closing(self.query(stmt)) as cur:
+            for (
+                ID, systemID, name,
                 lsFromStar, market, blackMarket, shipyard,
-                maxPadSize, outfitting, rearm, refuel, repair, planetary, isFleet, 
-                0, None,
-            )
-            stationByID[ID] = station
+                maxPadSize, outfitting, rearm, refuel, repair, planetary, type_id
+            ) in cur:
+                isFleet = 'Y' if int(type_id) in types['fleet-carrier'] else 'N'
+                isOdyssey = 'Y' if int(type_id) in types['odyssey'] else 'N'
+                station = Station(
+                    ID, systemByID[systemID], name,
+                    lsFromStar, market, blackMarket, shipyard,
+                    maxPadSize, outfitting, rearm, refuel, repair, planetary, isFleet, isOdyssey,
+                    0, None,
+                )
+                stationByID[ID] = station
         
         tradingCount = 0
         stmt = """
             SELECT  station_id,
                     COUNT(*) AS item_count,
                     AVG(JULIANDAY('now') - JULIANDAY(modified))
               FROM  StationItem
              GROUP  BY 1
              HAVING item_count > 0
         """
-        for ID, itemCount, dataAge in self.cur.execute(stmt):
-            station = stationByID[ID]
-            station.itemCount = itemCount
-            station.dataAge = dataAge
-            tradingCount += 1
+        with closing(self.query(stmt)) as cur:
+            for ID, itemCount, dataAge in cur:
+                station = stationByID[ID]
+                station.itemCount = itemCount
+                station.dataAge = dataAge
+                tradingCount += 1
         
         self.stationByID = stationByID
         self.tradingStationCount = tradingCount
         self.tdenv.DEBUG1("Loaded {:n} Stations", len(stationByID))
         self.stellarGrid = None
     
     def addLocalStation(
@@ -1239,14 +1199,16 @@
             shipyard,
             maxPadSize,
             outfitting,
             rearm,
             refuel,
             repair,
             planetary,
+            fleet,
+            odyssey,
             modified='now',
             commit=True,
             ):
         """
         Add a station to the local cache and memory copy.
         """
         
@@ -1264,33 +1226,41 @@
         assert shipyard in "?YN"
         assert maxPadSize in "?SML"
         assert outfitting in "?YN"
         assert rearm in "?YN"
         assert refuel in "?YN"
         assert repair in "?YN"
         assert planetary in '?YN'
+        assert fleet in '?YN'
+        assert odyssey in '?YN'
+        
+        type_id = 0
+        if fleet == 'Y':
+            type_id = 24
+        if odyssey == 'Y':
+            type_id = 25
         
         db = self.getDB()
         cur = db.cursor()
         cur.execute("""
             INSERT INTO Station (
                 name, system_id,
                 ls_from_star, market, blackmarket, shipyard, max_pad_size,
-                outfitting, rearm, refuel, repair, planetary,
+                outfitting, rearm, refuel, repair, planetary, type_id,
                 modified
             ) VALUES (
                 ?, ?,
                 ?, ?, ?, ?, ?,
-                ?, ?, ?, ?, ?,
+                ?, ?, ?, ?, ?, ?,
                 DATETIME(?)
             )
         """, [
             name, system.ID,
             lsFromStar, market, blackMarket, shipyard, maxPadSize,
-            outfitting, rearm, refuel, repair, planetary,
+            outfitting, rearm, refuel, repair, planetary, type_id,
             modified,
         ])
         ID = cur.lastrowid
         station = Station(
             ID, system, name,
             lsFromStar=lsFromStar,
             market=market,
@@ -1299,14 +1269,15 @@
             maxPadSize=maxPadSize,
             outfitting=outfitting,
             rearm=rearm,
             refuel=refuel,
             repair=repair,
             planetary=planetary,
             fleet='?',
+            odyssey='?',
             itemCount=0, dataAge=0,
         )
         self.stationByID[ID] = station
         if commit:
             db.commit()
         self.tdenv.NOTE(
             "{} (#{}) added to {}: "
@@ -1330,26 +1301,28 @@
             shipyard=None,
             maxPadSize=None,
             outfitting=None,
             rearm=None,
             refuel=None,
             repair=None,
             planetary=None,
+            fleet=None,
+            odyssey=None,
             modified='now',
             force=False,
             commit=True,
             ):
         """
         Alter the properties of a station in-memory and in the DB.
         """
         changes = []
         
         def _changed(label, old, new):
             changes.append(
-                "{}('{}'=>'{}')".format(label, old, new)
+                f"{label}('{old}'=>'{new}')"
             )
         
         if name is not None:
             if force or name.upper() != station.dbname.upper():
                 _changed("name", station.dbname, name)
                 station.dbname = name
         
@@ -1375,14 +1348,15 @@
         _check_setting("shp", "shipyard", shipyard, TradeDB.marketStates)
         _check_setting("out", "outfitting", outfitting, TradeDB.marketStates)
         _check_setting("arm", "rearm", rearm, TradeDB.marketStates)
         _check_setting("ref", "refuel", refuel, TradeDB.marketStates)
         _check_setting("rep", "repair", repair, TradeDB.marketStates)
         _check_setting("plt", "planetary", planetary, TradeDB.planetStates)
         _check_setting("flc", "fleet", fleet, TradeDB.fleetStates)
+        _check_setting("ody", "odyssey", odyssey, TradeDB.odysseyStates)
         
         if not changes:
             return False
         
         db = self.getDB()
         db.execute("""
             UPDATE Station
@@ -1478,15 +1452,15 @@
             station
             @system    [explicitly a system name]
             /station   [explicitly a station name]
             system/station
             @system/station
         """
         
-        if isinstance(name, System) or isinstance(name, Station):
+        if isinstance(name, (System, Station)):
             return name
         
         slashPos = name.find('/')
         if slashPos < 0:
             slashPos = name.find('\\')
         nameOff = 1 if name.startswith('@') else 0
         if slashPos > nameOff:
@@ -1545,15 +1519,16 @@
                     if subPos == 0:
                         if placeNameNorm[nameNormLen] == ' ':
                             # first word
                             wordMatch.append(place)
                         else:
                             anyMatch.append(place)
                         continue
-                    elif subPos > 0:
+                    
+                    if subPos > 0:
                         if placeNameNorm[subPos] == ' ' and \
                                 placeNameNorm[subPos + nameNormLen] == ' ':
                             wordMatch.append(place)
                         else:
                             anyMatch.append(place)
                         continue
                 
@@ -1570,32 +1545,33 @@
                         closeMatch.append(place)
                     continue
                 if placeNameTrimmed.find(nameTrimmed) >= 0:
                     anyMatch.append(place)
         
         if sysName:
             try:
-                sys = self.systemByName[sysName]
-                exactMatch = [sys]
+                system = self.systemByName[sysName]
+                exactMatch = [system]
             except KeyError:
                 lookup(sysName, self.systemByID.values())
+        
         if stnName:
             # Are we considering the name as a station?
             # (we don't if they type, e,g '@aulin')
             # compare against nameOff to allow '@/station'
             if slashPos > nameOff + 1:
                 # "sys/station"; the user should have specified a system
                 # name and we should be able to narrow down which
                 # stations we compare against. Check first if there are
                 # any matches.
                 stationCandidates = []
-                for sys in itertools.chain(
+                for system in itertools.chain(
                         exactMatch, closeMatch, wordMatch, anyMatch
                         ):
-                    stationCandidates += sys.stations
+                    stationCandidates += system.stations
                 # Clear out the candidate lists
                 exactMatch = []
                 closeMatch = []
                 wordMatch = []
                 anyMatch = []
             else:
                 # Consider against all station names
@@ -1611,15 +1587,15 @@
                 return matchSet[0]
         
         # Nothing matched
         if not any([exactMatch, closeMatch, wordMatch, anyMatch]):
             # Note: this was a TradeException and may need to be again,
             # but then we need to catch that error in commandenv
             # when we process avoids
-            raise LookupError("Unrecognized place: {}".format(name))
+            raise LookupError(f"Unrecognized place: {name}")
         
         # More than one match
         raise AmbiguityError(
             'System/Station', name,
             exactMatch + closeMatch + wordMatch + anyMatch,
             key=lambda place: place.name()
         )
@@ -1629,29 +1605,24 @@
         Look up a Station object by it's name or system.
         """
         if isinstance(name, Station):
             return name
         if isinstance(name, System):
             # When given a system with only one station, return the station.
             if len(name.stations) != 1:
-                raise SystemNotStationError(
-                    "System '%s' has %d stations, "
-                    "please specify a station instead." % (
-                        name.str(), len(name.stations)
-                    )
-                )
+                raise SystemNotStationError(f"System '{name}' has {len(name.stations)} stations, please specify a station instead.")
             return name.stations[0]
         
         if system:
             system = self.lookupSystem(system)
             return TradeDB.listSearch(
                 "Station", name, system.stations,
                 key=lambda system: system.dbname)
         
-        stationID, station, systemID, system = None, None, None, None
+        station, system = None, None
         try:
             system = TradeDB.listSearch(
                 "System", name, self.systemByID.values(),
                 key=lambda system: system.dbname
             )
         except LookupError:
             pass
@@ -1660,17 +1631,15 @@
                 "Station", name, self.stationByID.values(),
                 key=lambda station: station.dbname
             )
         except LookupError:
             pass
         # If neither matched, we have a lookup error.
         if not (station or system):
-            raise LookupError(
-                "'%s' did not match any station or system." % (name)
-            )
+            raise LookupError(f"'{name}' did not match any station or system.")
         
         # If we matched both a station and a system, make sure they resovle to
         # the same station otherwise we have an ambiguity. Some stations have
         # the same name as their star system (Aulin/Aulin Enterprise)
         if system and station and system != station.system:
             raise AmbiguityError(
                 'Station', name, [system.name(), station.name()]
@@ -1679,32 +1648,30 @@
         if station:
             return station
         
         # If we only matched a system name, ensure that it's a single station
         # system otherwise they need to specify a station name.
         if len(system.stations) != 1:
             raise SystemNotStationError(
-                "System '%s' has %d stations, "
-                "please specify a station instead." % (
-                    system.name(), len(system.stations)
-                )
+                f"System '{system.name()}' has {len(system.stations)} stations, please specify a station instead."
             )
         return system.stations[0]
     
     def getDestinations(
             self,
             origin,
             maxJumps=None,
             maxLyPer=None,
             avoidPlaces=None,
             maxPadSize=None,
             maxLsFromStar=0,
             noPlanet=False,
             planetary=None,
             fleet=None,
+            odyssey=None,
             ):
         """
         Gets a list of the Station destinations that can be reached
         from this Station within the specified constraints.
         Limits to stations we are trading with if trading is True.
         """
         
@@ -1777,45 +1744,24 @@
         # need stations to terminate at.
         def path_iter_fn():
             for node in pathList.values():
                 if node.distLy >= 0.0:
                     for station in node.system.stations:
                         yield node, station
         
-        path_iter = iter(path_iter_fn())
-        if noPlanet:
-            path_iter = iter(
-                (node, station) for (node, station) in path_iter
-                if station.planetary == 'N'
-            )
-        if avoidPlaces:
-            path_iter = iter(
-                (node, station) for (node, station) in path_iter
-                if station not in avoidPlaces
-            )
-        if maxPadSize:
-            path_iter = iter(
-                (node, station) for (node, station) in path_iter
-                if station.checkPadSize(maxPadSize)
-            )
-        if planetary:
-            path_iter = iter(
-                (node, station) for (node, station) in path_iter
-                if station.checkPlanetary(planetary)
-            )
-        if fleet:
-            path_iter = iter(
-                (node, station) for (node, station) in path_iter
-                if station.checkFleet(fleet)
-            )
-        if maxLsFromStar:
-            path_iter = iter(
-                (node, stn) for (node, stn) in path_iter
-                if stn.lsFromStar > 0 and stn.lsFromStar <= maxLsFromStar
-            )
+        path_iter = iter(
+          (node, station) for (node, station) in path_iter_fn()
+          if (station.planetary == 'N' if noPlanet else True) and
+            (station not in avoidPlaces if avoidPlaces else True) and
+            (station.checkPadSize(maxPadSize) if maxPadSize else True) and
+            (station.checkPlanetary(planetary) if planetary else True) and
+            (station.checkFleet(fleet) if fleet else True) and
+            (station.checkOdyssey(odyssey) if odyssey else True) and
+            (station.lsFromStar > 0 and station.lsFromStar <= maxLsFromStar if maxLsFromStar else True)
+        )
         for node, stn in path_iter:
             yield Destination(node.system, stn, node.via, node.distLy)
     
     ############################################################
     # Ship data.
     
     def ships(self):
@@ -1824,21 +1770,20 @@
     
     def _loadShips(self):
         """
         Populate the Ship list.
         CAUTION: Will orphan previously loaded objects.
         """
         stmt = """
-            SELECT ship_id, name, cost, fdev_id
+            SELECT ship_id, name, cost
               FROM Ship
         """
-        self.cur.execute(stmt)
         self.shipByID = {
             row[0]: Ship(*row, stations=[])
-            for row in self.cur
+            for row in self.query(stmt)
         }
         
         self.tdenv.DEBUG1("Loaded {} Ships", len(self.shipByID))
     
     def lookupShip(self, name):
         """
         Look up a ship by name
@@ -1863,18 +1808,19 @@
         Populate the list of item categories.
         CAUTION: Will orphan previously loaded objects.
         """
         stmt = """
             SELECT category_id, name
               FROM Category
         """
-        self.categoryByID = {
-            ID: Category(ID, name, [])
-            for (ID, name) in self.cur.execute(stmt)
-        }
+        with closing(self.query(stmt)) as cur:
+            self.categoryByID = {
+                ID: Category(ID, name, [])
+                for (ID, name) in cur
+            }
         
         self.tdenv.DEBUG1("Loaded {} Categories", len(self.categoryByID))
     
     def lookupCategory(self, name):
         """
         Look up a category by name
         """
@@ -1894,27 +1840,28 @@
         CAUTION: Will orphan previously loaded objects.
         """
         stmt = """
             SELECT item_id, name, category_id, avg_price, fdev_id
               FROM Item
         """
         itemByID, itemByName, itemByFDevID = {}, {}, {}
-        for ID, name, categoryID, avgPrice, fdevID in self.cur.execute(stmt):
-            category = self.categoryByID[categoryID]
-            item = Item(
-                ID, name, category,
-                '{}/{}'.format(category.dbname, name),
-                avgPrice, fdevID
-            )
-            itemByID[ID] = item
-            itemByName[name] = item
-            if fdevID:
-                itemByFDevID[fdevID] = item
-            
-            category.items.append(item)
+        with closing(self.query(stmt)) as cur:
+            for ID, name, categoryID, avgPrice, fdevID in cur:
+                category = self.categoryByID[categoryID]
+                item = Item(
+                    ID, name, category,
+                    f"{category.dbname}/{name}",
+                    avgPrice, fdevID
+                )
+                itemByID[ID] = item
+                itemByName[name] = item
+                if fdevID:
+                    itemByFDevID[fdevID] = item
+                
+                category.items.append(item)
         
         self.itemByID = itemByID
         self.itemByName = itemByName
         self.itemByFDevID = itemByFDevID
         
         self.tdenv.DEBUG1(
             "Loaded {:n} Items",
@@ -1932,15 +1879,15 @@
         )
     
     def getAverageSelling(self):
         """
         Query the database for average selling prices of all items.
         """
         if not self.avgSelling:
-            self.avgSelling = {itemID: 0 for itemID in self.itemByID.keys()}
+            self.avgSelling = {itemID: 0 for itemID in self.itemByID}
             self.avgSelling.update({
                 ID: int(cr)
                 for ID, cr in self.getDB().execute("""
                     SELECT  i.item_id, IFNULL(AVG(supply_price), 0)
                       FROM  Item AS i
                             LEFT OUTER JOIN StationItem AS si ON (
                                 i.item_id = si.item_id AND si.supply_price > 0
@@ -1952,15 +1899,15 @@
         return self.avgSelling
     
     def getAverageBuying(self):
         """
         Query the database for average buying prices of all items.
         """
         if not self.avgBuying:
-            self.avgBuying = {itemID: 0 for itemID in self.itemByID.keys()}
+            self.avgBuying = {itemID: 0 for itemID in self.itemByID}
             self.avgBuying.update({
                 ID: int(cr)
                 for ID, cr in self.getDB().execute("""
                     SELECT  i.item_id, IFNULL(AVG(demand_price), 0)
                       FROM  Item AS i
                             LEFT OUTER JOIN StationItem AS si ON (
                                 i.item_id = si.item_id AND si.demand_price > 0
@@ -1979,42 +1926,42 @@
         Populate the RareItem list.
         """
         stmt = """
             SELECT  rare_id, station_id, category_id, name,
                     cost, max_allocation, illegal, suppressed
               FROM  RareItem
         """
-        self.cur.execute(stmt)
-        
+
+
         rareItemByID, rareItemByName = {}, {}
         stationByID = self.stationByID
-        for (
-            ID, stnID, catID, name,
-            cost, maxAlloc, illegal, suppressed
-        ) in self.cur:
-            station = stationByID[stnID]
-            category = self.categoryByID[catID]
-            rare = RareItem(
-                ID, station, name, cost, maxAlloc, illegal, suppressed,
-                category, '{}/{}'.format(category.dbname, name)
-            )
-            rareItemByID[ID] = rareItemByName[name] = rare
+        with closing(self.query(stmt)) as cur:
+            for (
+                ID, stnID, catID, name,
+                cost, maxAlloc, illegal, suppressed
+            ) in cur:
+                station = stationByID[stnID]
+                category = self.categoryByID[catID]
+                rare = RareItem(
+                    ID, station, name, cost, maxAlloc, illegal, suppressed,
+                    category, f"{category.dbname}/{name}"
+                )
+                rareItemByID[ID] = rareItemByName[name] = rare
         self.rareItemByID = rareItemByID
         self.rareItemByName = rareItemByName
         
         self.tdenv.DEBUG1(
             "Loaded {:n} RareItems",
             len(rareItemByID)
         )
     
     ############################################################
     # Price data.
     
     def close(self):
-        self.cur = None
         if self.conn:
             self.conn.close()
         self.conn = None
     
     def load(self, maxSystemLinkLy=None):
         """
             Populate/re-populate this instance of TradeDB with data.
@@ -2022,17 +1969,16 @@
             taken references to:
                 tdb.load()
                 x = tdb.lookupPlace("Aulin")
                 tdb.load() # x now points to an orphan Aulin
         """
         
         self.tdenv.DEBUG1("Loading data")
-        
-        self.conn = conn = self.getDB()
-        self.cur = conn.cursor()
+
+
         
         self._loadAdded()
         self._loadSystems()
         self._loadStations()
         self._loadShips()
         self._loadCategories()
         self._loadItems()
@@ -2069,15 +2015,15 @@
             pass
         
         normTrans = TradeDB.normalizeTrans
         trimTrans = TradeDB.trimTrans
         needle = lookup.translate(normTrans).translate(trimTrans)
         partialMatch, wordMatch = [], []
         # make a regex to match whole words
-        wordRe = re.compile(r'\b{}\b'.format(lookup), re.IGNORECASE)
+        wordRe = re.compile(f"\\b{lookup}\\b", re.IGNORECASE)
         # describe a match
         for entry in values:
             entryKey = key(entry)
             normVal = entryKey.translate(normTrans).translate(trimTrans)
             if normVal.find(needle) > -1:
                 # If this is an exact match, ignore ambiguities.
                 if len(normVal) == len(needle):
@@ -2100,20 +2046,18 @@
             if len(partialMatch) > 1:
                 raise AmbiguityError(
                     listType, lookup, partialMatch,
                     key=lambda item: item.key,
                 )
             return partialMatch[0].value
         # No matches
-        raise LookupError(
-            "Error: '%s' doesn't match any %s" % (lookup, listType)
-        )
+        raise LookupError(f"Error: '{lookup}' doesn't match any {listType}")
     
     @staticmethod
-    def normalizedStr(text):
+    def normalizedStr(text: str) -> str:
         """
             Returns a case folded, sanitized version of 'str' suitable for
             performing simple and partial matches against. Removes various
             punctuation characters that don't contribute to name uniqueness.
             NOTE: No-longer removes whitespaces or apostrophes.
         """
         return text.translate(
@@ -2121,24 +2065,23 @@
         ).translate(
             TradeDB.trimTrans
         )
 
 ######################################################################
 # Assorted helpers
 
-def describeAge(ageInSeconds):
+def describeAge(ageInSeconds: Union[float, int]) -> str:
     """
     Turns an age (in seconds) into a text representation.
     """
     hours = int(ageInSeconds / 3600)
     if hours < 1:
         return "<1 hr"
     if hours == 1:
         return "1 hr"
     if hours < 48:
-        return str(hours) + " hrs"
+        return f"{hours} hrs"
     days = int(hours / 24)
     if days < 90:
-        return str(days) + " days"
+        return f"{days} days"
     
-    months = int(days / 31)
-    return str(months) + " mths"
+    return f"{int(days / 31)} mths"
```

### Comparing `tradedangerous-10.9.8/tradedangerous/mapping.py` & `tradedangerous-11.0.0/tradedangerous/mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # Mapping class for FDEV-IDs to TD names
 #
 
-class FDEVMappingBase(object):
+class FDEVMappingBase:
     """
     Base class to map FDEV-IDs to TD names, do not use directly.
     
     Derived class must declare "tableName" and "colNames" which are used
     to select the ID->Name mapping from the database.
     
     "colNames" is a list() of columns. The first one must be the idColumn.
@@ -63,15 +63,16 @@
         for line in curs:
             ID = line[0]
             if self._colCount == 1:
                 entries[ID] = line[1]
             else:
                 entries[ID] = {}
                 for i, val in enumerate(line[1:], start=1):
-                    if val: entries[ID][self.colNames[i]] = val
+                    if val:
+                        entries[ID][self.colNames[i]] = val
             self.tdenv.DEBUG2("{}: {}".format(ID, str(entries[ID]).replace("{", "{{").replace("}", "}}")))
         self.entries = entries
         self.tdenv.DEBUG1("Loaded {:n} {}-Mappings".format(len(entries), self.tableName))
     
     def addUnknown(self, wrong, right):
         # add Entries by name with unknown IDs
         if isinstance(wrong, (str,int,tuple)):
@@ -122,10 +123,10 @@
     colNames  = [ 'id', 'name' ]
 
 class FDEVMappingOutfitting(FDEVMappingBase):
     """
         Maps ID to EDDN outfitting
     """
     tableName = "FDevOutfitting"
-    colNames  = [ 'id', 'category' , 'name', 'mount',
+    colNames  = [ 'id', 'category', 'name', 'mount',
                   'guidance', 'ship', 'class', 'rating'
                 ]
```

### Comparing `tradedangerous-10.9.8/tradedangerous/csvexport.py` & `tradedangerous-11.0.0/tradedangerous/csvexport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-
 from pathlib import Path
 from .tradeexcept import TradeException
 
 import csv
 import os
 import sqlite3
 
@@ -30,17 +28,18 @@
 # for some tables the first two columns will be reversed
 reverseList = []
 
 ######################################################################
 # Helpers
 ######################################################################
 
-def search_keyList(list, val):
-    for row in list:
-        if row['from'] == row['to'] == val: return row
+def search_keyList(items, val):
+    for row in items:
+        if row['from'] == row['to'] == val:
+            return row
 
 def getUniqueIndex(conn, tableName):
     """ return all unique columns """
     idxCursor = conn.cursor()
     unqIndex = []
     for idxRow in idxCursor.execute("PRAGMA index_list('%s')" % tableName):
         if idxRow['unique']:
@@ -95,56 +94,57 @@
     
     return keyStmt
 
 ######################################################################
 # Code
 ######################################################################
 
-def exportTableToFile(tdb, tdenv, tableName, dataPath=None):
+def exportTableToFile(tdb, tdenv, tableName, csvPath=None):
     """
-        Generate the csv file for tableName in dataPath
+        Generate the csv file for tableName in csvPath
         returns lineCount, exportPath
     """
     
     # path for csv file
-    dataPath = dataPath or tdb.dataPath
-    if not dataPath.is_dir():
-        raise TradeException("Save location '{}' not found.".format(str(dataPath)))
+    csvPath = csvPath or tdb.csvPath
+    if not csvPath.is_dir():
+        raise TradeException("Save location '{}' not found.".format(str(csvPath)))
     
     # connect to the database
     conn = tdb.getDB()
     conn.row_factory = sqlite3.Row
     
     # prefix for unique/ignore columns
     uniquePfx = "unq:"
     ignorePfx = "!"
     
     # create CSV files
-    exportPath = (dataPath / Path(tableName)).with_suffix(".csv")
+    exportPath = (csvPath / Path(tableName)).with_suffix(".csv")
     tdenv.DEBUG0("Export Table '{table}' to '{file}'".format(
                     table=tableName, file=str(exportPath)
                     ))
     
     lineCount = 0
     with exportPath.open("w", encoding='utf-8', newline="\n") as exportFile:
         exportOut = csv.writer(exportFile, delimiter=",", quotechar="'", doublequote=True, quoting=csv.QUOTE_NONNUMERIC, lineterminator="\n")
         
         cur = conn.cursor()
         
         # check for single PRIMARY KEY
         pkCount = 0
         for columnRow in cur.execute("PRAGMA table_info('%s')" % tableName):
             # count the columns of the primary key
-            if columnRow['pk'] > 0: pkCount += 1
+            if columnRow['pk'] > 0:
+                pkCount += 1
         
         # build column list
         columnList = []
         for columnRow in cur.execute("PRAGMA table_info('%s')" % tableName):
             # if there is only one PK column, ignore it
-            #if columnRow['pk'] > 0 and pkCount == 1: continue
+            # if columnRow['pk'] > 0 and pkCount == 1: continue
             columnList.append(columnRow)
         
         if len(columnList) == 0:
             raise TradeException("No columns to export for table '{}'.".format(tableName))
         
         # reverse the first two columns for some tables
         if tableName in reverseList:
@@ -195,15 +195,15 @@
                     csvHead += [ uniquePfx + col['name'] ]
                     stmtOrder += [ "{}.{}".format(tableName, col['name']) ]
                 else:
                     csvHead += [ col['name'] ]
                 stmtColumn += [ "{}.{}".format(tableName, col['name']) ]
         
         # build the SQL statement
-        sqlStmt = "SELECT {} FROM {}".format(",".join(stmtColumn)," ".join(stmtTable))
+        sqlStmt = "SELECT {} FROM {}".format(",".join(stmtColumn), " ".join(stmtTable))
         if len(stmtOrder) > 0:
             sqlStmt += " ORDER BY {}".format(",".join(stmtOrder))
         tdenv.DEBUG1("SQL: %s" % sqlStmt)
         
         # finally generate the csv file
         # write header line without quotes
         exportFile.write("{}\n".format(",".join(csvHead)))
```

### Comparing `tradedangerous-10.9.8/tradedangerous/__init__.py` & `tradedangerous-11.0.0/tradedangerous/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #
 # You are free to use, redistribute, or even print and eat a copy of
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """
-TradeDangerous is set of powerful trading tools for Elite Dangerous,
+TradeDangerous is a set of powerful trading tools for Elite Dangerous,
 organized around one of the most powerful trade run optimizers available.
 
 The TRO is a heavy hitter that can calculate complex routes with multiple stops
 while taking into account the profits you make along the route
-The price data in TradeDangerous is either manually entered or crowd sourced
+The price data in TradeDangerous is either manually entered or crowd-sourced
 from a website such as [Tromador's Trading Dangerously](http://elite.ripz.org "Tromador's Trading Dangerously"), often using a plugin such as the included eddblink.
 """
-from .version import *
+from .version import *          # noqa: F401, F403
 
-from .tradeenv import TradeEnv
+from .tradeenv import TradeEnv  # noqa: F401
```

### Comparing `tradedangerous-10.9.8/tradedangerous/edscupdate.py` & `tradedangerous-11.0.0/tradedangerous/edscupdate.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 differs from the star name in the galaxy map.
 
 For each star you can type "y" to accept the star, "n" to skip it
 or "q" to stop recording.
 """
 
 import argparse
-import math
 import misc.clipboard
 import misc.edsc
 import os
 import random
 import re
 import sys
 import tradedb
@@ -154,15 +153,15 @@
             '--confidence',
             required=False,
             help='Specify minimum confidence level.',
             type=int,
             default=2,
     )
     grp = parser.add_mutually_exclusive_group()
-    if grp: # for indentation
+    if grp:  # for indentation
         grp.add_argument(
                 '--random',
                 action='store_true',
                 required=False,
                 help='Show systems in random order, maximum of --max-systems.',
         )
         grp.add_argument(
@@ -293,15 +292,15 @@
     # is it in the database?
     cur = tdb.query("""
         SELECT name, pos_x, pos_y, pos_z
           FROM System
          WHERE pos_x BETWEEN ? and ?
            AND pos_y BETWEEN ? and ?
            AND pos_z BETWEEN ? and ?
-    """, [ 
+    """, [
         x - 0.5, x + 0.5,
         y - 0.5, y + 0.5,
         z - 0.5, z + 0.5,
     ])
     for mname, mx, my, mz in cur:
         print(
                 "! @{} [{},{},{}] matches coords for "
@@ -341,15 +340,15 @@
         response=r,
     )
     print(str(result))
 
 def get_extras():
     extras = set()
     try:
-        with open("data/extra-stars.txt", "rU", encoding="utf-8") as fh:
+        with open("data/extra-stars.txt", "r", encoding="utf-8") as fh:
             for line in fh:
                 name = line.partition('#')[0].strip().upper()
                 if name:
                     extras.add(name)
     except FileNotFoundError:
         pass
     return extras
@@ -387,17 +386,15 @@
     
     if edsq.status['statusnum'] != 0:
         raise Exception("Query failed: {} ({})".format(
                     edsq.status['msg'],
                     edsq.status['statusnum'],
                 ))
     
-    date = data['date']
     systems = data['systems']
-    
     print("{} results".format(len(systems)))
     # Filter out systems we already know that match the EDSC data.
     systems = [
         sysinfo for sysinfo in systems if is_change(tdb, sysinfo)
     ]
     print("{} deltas".format(len(systems)))
     
@@ -530,15 +527,15 @@
                 correction = float(ok[1:])
                 submit_distance(argv, name, correction)
                 if not name.upper() in extras:
                     add_to_extras(argv, name)
                 continue
             if ok.startswith('='):
                 name = ok[1:].strip().upper()
-                if not name in extras:
+                if name not in extras:
                     add_to_extras(argv, name)
                 ok = 'y'
             if ok.lower() != 'y':
                 continue
             
             if argv.add:
                 tdb.addLocalSystem(
@@ -551,14 +548,15 @@
             
             print("'{}',{},{},{},'Release 1.00-EDStar','{}'".format(
                 name, x, y, z, created,
             ), file=output)
             
             submit_distance(argv, name, distance)
 
+
 if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
         print("^C")
     except UsageError as e:
         print("ERROR: {}\nSee {} --help for usage help.".format(
```

### Comparing `tradedangerous-10.9.8/tradedangerous/edsmupdate.py` & `tradedangerous-11.0.0/tradedangerous/edsmupdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 differs from the star name in the galaxy map.
 
 For each star you can type "y" to accept the star, "n" to skip it
 or "q" to stop recording.
 """
 
 import argparse
-import math
 import misc.clipboard
 import misc.edsm
 import os
 import random
 import re
 import sys
 import tradedb
@@ -63,15 +62,15 @@
             '--cmdr',
             required=False,
             help='Specify your commander name.',
             type=str,
             default=os.environ.get('CMDR', None),
     )
     grp = parser.add_mutually_exclusive_group()
-    if grp: # for indentation
+    if grp:  # for indentation
         grp.add_argument(
                 '--random',
                 action='store_true',
                 required=False,
                 help='Show systems in random order, maximum of --max-systems.',
         )
         grp.add_argument(
@@ -234,15 +233,15 @@
         x, y, z
     )
     return float("{:.2f}".format(distance))
 
 def get_extras():
     extras = set()
     try:
-        with open("data/extra-stars.txt", "rU", encoding="utf-8") as fh:
+        with open("data/extra-stars.txt", "r", encoding="utf-8") as fh:
             for line in fh:
                 name = line.partition('#')[0].strip().upper()
                 if name:
                     extras.add(name)
     except FileNotFoundError:
         pass
     return extras
@@ -267,15 +266,15 @@
                 "*exact* name for a system that TD already knows.\n"
                 "Did you forget to put double-quotes around the reference "
                 "system name?"
                 .format(argv.refSystem)
             )
     
     if not argv.date:
-       argv.date = tdb.query("SELECT MAX(modified) FROM System").fetchone()[0]
+        argv.date = tdb.query("SELECT MAX(modified) FROM System").fetchone()[0]
     dateRe = re.compile(r'^20\d\d-(0[1-9]|1[012])-(0[1-9]|[12]\d|3[01]) ([01]\d|2[0123]):[0-5]\d:[0-5]\d$')
     if not dateRe.match(argv.date):
         raise UsageError(
                 "Invalid date: '{}', expecting YYYY-MM-DD HH:MM:SS format."
                 .format(argv.date)
         )
     print("start date: {}".format(argv.date))
@@ -436,15 +435,15 @@
                     ok = "y"
             else:
                 ok = input(prompt)
             if ok.lower() == 'q':
                 break
             if ok.startswith('='):
                 name = ok[1:].strip().upper()
-                if not name in extras:
+                if name not in extras:
                     add_to_extras(argv, name)
                 ok = 'y'
             if ok.lower() != 'y':
                 continue
             
             if argv.add:
                 print("Add {:>6}: {:>12} {} {}".format(current, sysinfo['id'], created, name))
@@ -458,14 +457,15 @@
             
             print("'{}',{},{},{},'EDSM','{}'".format(
                 name, x, y, z, created,
             ), file=output)
         if argv.add and not commit:
             tdb.getDB().commit()
 
+
 if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
         print("^C")
     except UsageError as e:
         print("ERROR: {}\nSee {} --help for usage help.".format(
```

### Comparing `tradedangerous-10.9.8/tradedangerous/formatting.py` & `tradedangerous-11.0.0/tradedangerous/formatting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,26 @@
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
+"""
+Provides a library of mechanisms for formatting output text to ensure consistency across
+TradeDangerous and plugin tools,
+"""
+from __future__ import annotations
+
 import itertools
+import typing
+
+if typing.TYPE_CHECKING:
+    from typing import Any, Callable, Optional
 
-class ColumnFormat(object):
+class ColumnFormat:
     """
         Describes formatting of a column to be populated with data.
         
         Member Functions:
             
-            str()
+            text()
                 Applies all formatting (except qualifier) to the name to
                 produce a correctly sized title field.
             
             format(value)
                 Applies all formatting to key(value) to produce a correctly
                 sized value field.
         
@@ -43,66 +52,63 @@
                 ColumnFormat("Dist", ">",  "6", ".2f",
                         pre='[',
                         post=']'
                         key=lambda item:item['dist']),
             ]
             rows = [ {'name':'Bob', 'dist':1.5}, {'name':'John', 'dist':23}]
             # print titles
-            print(*[col.str() for col in cols])
+            print(*[col.text() for col in cols])
             for row in rows:
                 print(*[col.format(row) for col in cols])
         Produces:
             Name   [ Dist]
             Bob    [ 1.30]
             John   [23.00]
     
     """
+    name:       str                 # name of the column
+    align:      str                 # format's alignment specifier
+    width:      int                 # width specifier
+    qualifier:  Optional[str]       # optional format type specifier e.g. '.2f', 's', 'n'
+    pre:        Optional[str]       # prefix to the column
+    post:       Optional[str]       # postfix to the column
+    key:        Callable            # function to retrieve the printable name of the item
+    pred:       Callable            # predicate: return False to leave this column blank
+    
     def __init__(
             self,
             name,
             align,
             width,
             qualifier=None,
             pre=None,
             post=None,
             key=lambda item: item,
             pred=lambda item: True,
-            ):
+            ) -> None:
         self.name = name
         self.align = align
         self.width = max(int(width), len(name))
         self.qualifier = qualifier or ''
         self.key = key
         self.pre = pre or ''
         self.post = post or ''
         self.pred = pred
     
-    def str(self):
-        return '{pre}{title:{align}{width}}{post}'.format(
-                title=self.name,
-                align=self.align, width=self.width,
-                pre=self.pre, post=self.post,
-            )
-    
-    def format(self, value):
-        if self.pred(value):
-            return '{pre}{value:{align}{width}{qual}}{post}'.format(
-                    value=self.key(value),
-                    align=self.align, width=self.width,
-                    qual=self.qualifier,
-                    pre=self.pre, post=self.post,
-                )
-        else:
-            return '{pre}{value:{align}{width}}{post}'.format(
-                value="",
-                align=self.align, width=self.width,
-                pre=self.pre, post=self.post,
-            )
+    def __str__(self) -> str:
+        return f'{self.pre}{self.name:{self.align}{self.width}}{self.post}'
+    text = __str__
+    
+    def format(self, value: str) -> str:
+        """ Returns the string formatted with a specific value"""
+        if not self.pred(value):
+            return f'{self.pre}{"":{self.align}{self.width}}{self.post}'
+        return f'{self.pre}{self.key(value):{self.align}{self.width}{self.qualifier}}{self.post}'
 
-class RowFormat(object):
+class RowFormat:
     """
         Describes an ordered collection of ColumnFormats
         for dispay data from rows, such that calling
           rowFmt.format(rowData)
         will return the result of formatting each column
         against rowData.
         
@@ -113,79 +119,86 @@
                 If 'after' is specified, tries to insert
                 the new column immediately after the first
                 column who's name matches after.
             
             insert(pos, newCol)
                 Inserts a ColumnFormatter at position pos in the list
             
-            str()
+            text()
                 Returns a list of all the column headings
             
             format(rowData):
                 Returns a list of applying rowData to all
                 of the columns
     
     """
-    def __init__(self, prefix=None):
+    columns:        list[ColumnFormat]
+    prefix:         str
+    
+    def __init__(self, prefix: Optional[str] = None):
         self.columns = []
         self.prefix = prefix or ""
     
-    def addColumn(self, *args, **kwargs):
+    def addColumn(self, *args, **kwargs) -> None:
         self.append(ColumnFormat(*args, **kwargs))
     
-    def append(self, column, after=None):
+    def append(self, column: ColumnFormat, after: Optional[str] = None) -> 'RowFormat':
         columns = self.columns
         if after:
             for idx, col in enumerate(columns, 1):
                 if col.name == after:
                     columns.insert(idx, column)
                     return self
         columns.append(column)
         return self
     
-    def insert(self, pos, column):
+    def insert(self, pos: int, column: Optional[ColumnFormat]) -> None:
         if column is not None:
             self.columns.insert(pos, column)
     
-    def str(self):
-        return self.prefix + ' '.join(col.str() for col in self.columns)
+    def __str__(self) -> str:
+        return f"{self.prefix} {' '.join(str(col) for col in self.columns)}"
     
-    def heading(self):
-        headline = self.str()
+    text = __str__  # alias
+    
+    def heading(self) -> tuple[str, str]:
+        """ Returns a title and the appropriate underline for that text. """
+        headline = f"{self}"
         return headline, '-' * len(headline)
     
-    def format(self, rowData):
-        return self.prefix + ' '.join(col.format(rowData) for col in self.columns)
+    def format(self, row_data: Optional[Any]) -> str:
+        return f"{self.prefix} {' '.join(col.format(row_data) for col in self.columns)}"
 
 def max_len(iterable, key=lambda item: item):
     iterable, readahead = itertools.tee(iter(iterable))
     try:
         next(readahead)
     except StopIteration:
         return 0
     return max(len(key(item)) for item in iterable)
 
+
 if __name__ == '__main__':
     rowFmt = RowFormat(). \
                 append(ColumnFormat("Name", '<', '8', key=lambda row: row['name'])). \
                 append(ColumnFormat("Dist", '>', '6', '.2f', pre='[', post=']', key=lambda row: row['dist']))
     
     rows = [
         { 'name': 'Bob', 'dist': 6.2, 'age': 30 },
         { 'name': 'Dave', 'dist': 42, 'age': 18 },
     ]
     
     def present():
-        rowTitle = rowFmt.str()
+        rowTitle = rowFmt.text()
         print(rowTitle)
         print('-' * len(rowTitle))
         for row in rows:
             print(rowFmt.format(row))
     
     print("Simple usage:")
     present()
     
     print()
     print("Adding age ColumnFormat:")
     
     rowFmt.append(after='Name', col=ColumnFormat("Age", '>', 3, pre='|', post='|', key=lambda row: row['age']))
-    present()
+    present()
```

### Comparing `tradedangerous-10.9.8/PKG-INFO` & `tradedangerous-11.0.0/tradedangerous.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 10.9.8
+Version: 11.0.0
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
 Project-URL: Source Code, https://github.com/eyeonus/Trade-Dangerous
-Description: 
-        ----------
-        
-        TradeDangerous  
-        Copyright (C) Oliver "kfsone" Smith, July 2014  
-        Copyright (C) Bernd 'Gazelle' Gollesch 2016, 2017  
-        Copyright (C) Jonathan 'eyeonus' Jones 2018, 2019
-        
-        REQUIRES PYTHON 3.4 OR HIGHER.
-        
-        ----------
-        
-        # What is Trade Dangerous? <img align="right" src="https://raw.githubusercontent.com/wiki/eyeonus/Trade-Dangerous/TradeDangerousCrest.png" alt="Trade Dangerous Crest">
-        
-        TradeDangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
-        
-        The TRO is a heavy hitter that can calculate complex routes with multiple stops while taking into account the profits you make along the route 
-        
-        The price data in TradeDangerous is either manually entered or crowd sourced from a website such as [Tromador's Trading Dangerously](http://elite.tromador.com/ "Tromador's Trading Dangerously"), often using a plugin such as the included eddblink.
-        
-        # What can it do for me?
-        
-        You're in a ship with 8 cargo spaces that can make 8.56 ly per jump; you're willing to make upto 2 jumps between stations, and we want to see how much money we can make if in 2 trade stops (hops).
-        
-            trade.py run --credits 5000 --capacity 8 --ly-per 8.56 --jumps 2 --hops 2
-        
-        If we ran this, TD would search the galaxy for trade runs. But it could take us days to reach some of them. So lets say we're currently at Kummer City in the Andere system.
-        
-            trade.py run --from "andere/kummer city"
-                --credits 5000 --capacity 8 --ly-per 8.56 --jumps 2 --hops 2
-        
-        (The above represents a single line)
-        
-        That's a lot to type. TD is designed to support laziness when it comes to typing, so it allows for all kinds of short-cuts.
-        
-            trade.py ru
-                --fr and/kumm     find a station matching 'kumm' in a
-                                  system matching 'and'
-                --cr 5k           'k', 'm' and 'b' are recognized suffixes
-                --cap 8           8 units of cargo
-                --ly 8.56         maximum distance *per jump*
-                --ju 2            maximum 2 jumps
-        
-        The default for hops is 2, so I didn't have to include it.
-        
-        You can also use "=" to connect an option with its values:
-        
-            trade.py ru --fr=and/kumm --cr=5k --cap=8 --ly=8.56 --ju=2
-        
-        With the data at the time I write this, this produces:
-        
-            ANDERE/Kummer City -> ANDERE/Malzberg Vision
-              ANDERE/Kummer City: 6 x Titanium, 2 x Polymers,
-              G 224-46/Lorrah Dock: 7 x Coltan, 1 x Lepidolite,
-              ANDERE/Malzberg Vision +8,032cr (502/ton)
-        
-        This tells us our overall route (line #1), what load to pick up from the first station, what to sell it for and pick up at the second stop and where to finish and unload for our final profit.
-        
-        Note that it could have just told us to pick up 6 Titanium (the max we could afford) or 8 Copper (the highest profit we could fill up with), Instead, TD crunched hard numbers and maximized the earnings of every cargo space AND credit.
-        
-        If you want to give Trade Dangerous a try, look no further than the [Setup Guide](https://github.com/eyeonus/Trade-Dangerous/wiki/Setup-Guide "Setup Guide") and the [User Guide](https://github.com/eyeonus/Trade-Dangerous/wiki/User-Guide "User Guide").
-        
-        Curious about programming with Trade Dangerous/Python? Take the [Python Quick Peek](https://github.com/eyeonus/Trade-Dangerous/wiki/Python-Quick-Peek "Python Quick Peek").
-        
 Keywords: trade,elite,elite-dangerous
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: appJar
+Requires-Dist: ijson
+Requires-Dist: rich
+
+
+----------
+
+TradeDangerous  
+Copyright (C) Oliver "kfsone" Smith, July 2014  
+Copyright (C) Bernd 'Gazelle' Gollesch 2016, 2017  
+Copyright (C) Jonathan 'eyeonus' Jones 2018 - 2021
+
+REQUIRES PYTHON 3.4 OR HIGHER.
+
+----------
+
+# What is Trade Dangerous? <img align="right" src="https://raw.githubusercontent.com/wiki/eyeonus/Trade-Dangerous/TradeDangerousCrest.png" alt="Trade Dangerous Crest">
+
+TradeDangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
+
+The TRO is a heavy hitter that can calculate complex routes with multiple stops while taking into account the profits you make along the route 
+
+The price data in TradeDangerous is either manually entered or crowd sourced from a website such as [Tromador's Trading Dangerously](http://elite.tromador.com/ "Tromador's Trading Dangerously"), often using a plugin such as the included eddblink.
+
+# What can it do for me?
+
+You're in a ship with 8 cargo spaces that can make 8.56 ly per jump; you're willing to make upto 2 jumps between stations, and we want to see how much money we can make if in 2 trade stops (hops).
+
+    trade.py run --credits 5000 --capacity 8 --ly-per 8.56 --jumps 2 --hops 2
+
+If we ran this, TD would search the galaxy for trade runs. But it could take us days to reach some of them. So lets say we're currently at Kummer City in the Andere system.
+
+    trade.py run --from "andere/kummer city"
+        --credits 5000 --capacity 8 --ly-per 8.56 --jumps 2 --hops 2
+
+(The above represents a single line)
+
+That's a lot to type. TD is designed to support laziness when it comes to typing, so it allows for all kinds of short-cuts.
+
+    trade.py ru
+        --fr and/kumm     find a station matching 'kumm' in a
+                          system matching 'and'
+        --cr 5k           'k', 'm' and 'b' are recognized suffixes
+        --cap 8           8 units of cargo
+        --ly 8.56         maximum distance *per jump*
+        --ju 2            maximum 2 jumps
+
+The default for hops is 2, so I didn't have to include it.
+
+You can also use "=" to connect an option with its values:
+
+    trade.py ru --fr=and/kumm --cr=5k --cap=8 --ly=8.56 --ju=2
+
+With the data at the time I write this, this produces:
+
+    ANDERE/Kummer City -> ANDERE/Malzberg Vision
+      ANDERE/Kummer City: 6 x Titanium, 2 x Polymers,
+      G 224-46/Lorrah Dock: 7 x Coltan, 1 x Lepidolite,
+      ANDERE/Malzberg Vision +8,032cr (502/ton)
+
+This tells us our overall route (line #1), what load to pick up from the first station, what to sell it for and pick up at the second stop and where to finish and unload for our final profit.
+
+Note that it could have just told us to pick up 6 Titanium (the max we could afford) or 8 Copper (the highest profit we could fill up with), Instead, TD crunched hard numbers and maximized the earnings of every cargo space AND credit.
+
+If you want to give Trade Dangerous a try, look no further than the [Setup Guide](https://github.com/eyeonus/Trade-Dangerous/wiki/Setup-Guide "Setup Guide") and the [User Guide](https://github.com/eyeonus/Trade-Dangerous/wiki/User-Guide "User Guide").
+
+Curious about programming with Trade Dangerous/Python? Take the [Python Quick Peek](https://github.com/eyeonus/Trade-Dangerous/wiki/Python-Quick-Peek "Python Quick Peek").
```

### Comparing `tradedangerous-10.9.8/README.md` & `tradedangerous-11.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 ----------
 
 TradeDangerous  
 Copyright (C) Oliver "kfsone" Smith, July 2014  
 Copyright (C) Bernd 'Gazelle' Gollesch 2016, 2017  
-Copyright (C) Jonathan 'eyeonus' Jones 2018, 2019
+Copyright (C) Jonathan 'eyeonus' Jones 2018 - 2021
 
 REQUIRES PYTHON 3.4 OR HIGHER.
 
 ----------
 
 # What is Trade Dangerous? <img align="right" src="https://raw.githubusercontent.com/wiki/eyeonus/Trade-Dangerous/TradeDangerousCrest.png" alt="Trade Dangerous Crest">
```

### Comparing `tradedangerous-10.9.8/LICENSE` & `tradedangerous-11.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.8/setup.py` & `tradedangerous-11.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 package = "tradedangerous"
 
 exec(open("tradedangerous/version.py").read())  # pylint: disable=W0122
 
 setup(name = package,
         version = __version__,  # pylint: disable=E0602
-        install_requires = ["requests", "appJar"],
+        install_requires = ["requests", "appJar", "ijson", "rich"],
         setup_requires = ["pytest-runner"],
         tests_require = ["pytest"],
         packages = ['tradedangerous', 'tradedangerous.commands', 'tradedangerous.mfd', 'tradedangerous.mfd.saitek', 'tradedangerous.misc', 'tradedangerous.plugins'],
         url = "https://github.com/eyeonus/Trade-Dangerous",
         project_urls = {
             "Bug Tracker": "https://github.com/eyeonus/Trade-Dangerous/issues",
             "Documentation": "https://github.com/eyeonus/Trade-Dangerous/wiki",
@@ -41,20 +41,25 @@
         author_email = "eyeonus@gmail.com",
         description = "Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.",
         long_description = long_description,
         long_description_content_type = "text/markdown",
         keywords = ["trade", "elite", "elite-dangerous"],
         classifiers = [
             "Programming Language :: Python :: 3",
-            "License :: OSI Approved :: MIT License",
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
             "Operating System :: OS Independent",
         ],
         license = "MPL",
         test_suite = "tests",
-        package_data = {"tradedangerous": ["templates/TradeDangerous.sql", "templates/Added.csv", "templates/RareItem.csv", "templates/DefaultShipIndex.json"]},
+        package_data = {"tradedangerous": ["templates/TradeDangerous.sql", "templates/Added.csv", "templates/Category.csv", "templates/RareItem.csv"]},
         entry_points = {
             "console_scripts": [
-                "trade=tradedangerous.trade:main"
+                "trade=tradedangerous.trade:main",
+                "tradegui=tradedangerous.tradegui:main"
             ]
         },
         zip_safe = False
 )
```

### Comparing `tradedangerous-10.9.8/tests/test_commands.py` & `tradedangerous-11.0.0/tests/test_commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #! /usr/bin/env python
 # pytest
 
-from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
-import sys
 import pytest
 from tradedangerous import commands
 from tradedangerous.commands.exceptions import UsageError, CommandLineError
 
 @pytest.fixture
 def cmd():
     return commands.CommandIndex()
 
+
 prog = "trade.py"
 
-class TestCommands(object):
+
+class TestCommands:
     
     def test_dashh(self, cmd):
         with pytest.raises(UsageError):
             cmd.parse([prog, '-h'])
     
     def test_local_dashh(self, cmd):
         with pytest.raises(UsageError):
@@ -35,8 +35,8 @@
         with pytest.raises(CommandLineError):
             cmd.parse([prog, 'local', '-v'])
     
     def test_local_validsys(self, cmd):
         cmd.parse([prog, 'local', 'ibootis'])
     
     def test_local_validsys_dashv(self, cmd):
-        cmd.parse([prog, 'local', 'ibootis', '-v'])
+        cmd.parse([prog, 'local', 'ibootis', '-v'])
```

### Comparing `tradedangerous-10.9.8/tests/test_cache.py` & `tradedangerous-11.0.0/tests/test_cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from collections import namedtuple
 
 from tradedangerous import cache
 
 FakeFile = namedtuple('FakeFile', ['name'])
 
-class TestCache(object):
+class TestCache:
     def test_parseSupply(self):
         fil = FakeFile('faked-file.prices')
         reading = '897H'
         demandUnits, demandLevel = cache.parseSupply(
             fil,
             10,
             'demand',
```

### Comparing `tradedangerous-10.9.8/tests/test_trade_run.py` & `tradedangerous-11.0.0/tests/test_trade_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import re
 import io
 
 import pytest
 
 from tradedangerous.cli import trade
-from tradedangerous.commands.exceptions import UsageError
-from tradedangerous import tools
+
 from .helpers import copy_fixtures, regex_findin, replace_stdin
 
 PROG = "trade"
 
 
 def setup_module():
     copy_fixtures()
 
 
-class TestTradeRun(object):
+class TestTradeRun:
     def test_run1(self, capsys):
         trade([PROG, "run", "--capacity=10", "--credits=10000", "--from=sol/abr", "--jumps-per=3", "--ly-per=10.5", "--no-planet"])
         captured = capsys.readouterr()
         assert "Sol/Abraham Lincoln: 10 x Hydrogen Fuel," in captured.out
         assert "Sol/Burnell Station: 2 x Silver," in captured.out
         assert "560cr (213/ton)" in captured.out
-
-
+    
+    @pytest.mark.slow
     def test_run2(self, capsys):
-        trade([PROG, "run", "-vv", "--progress", "--empty=82",
+        trade([
+            PROG, "run", "-vv", "--progress", "--empty=82",
             "--cap=212", "--jumps=4", "--cr=2153796", "--from=sol/abr",
             "--hops=6", "--ls-m=8000", "--sup=10000",
             "--pad=L", "--ly=25", "--prune-hop=3", "--prune-sc=40"])
         captured = capsys.readouterr()
         assert regex_findin(r"=> est [\d\s,]+cr total", captured.out)
     
+    @pytest.mark.slow
     def test_run3(self, capsys):
         """Testing --checklist
         """
         # monkeypatch.setattr('sys.stdin', io.StringIO('100'))
         STEPS = 37
         with replace_stdin(io.StringIO('\n' * STEPS)):
-            trade([PROG, "run", "-vv", "--progress", "--empty=82", "--checklist",
+            trade([
+                PROG, "run", "-vv", "--progress", "--empty=82", "--checklist",
                 "--cap=212", "--jumps=4", "--cr=2153796", "--from=sol/abr",
                 "--hops=6", "--ls-m=8000", "--sup=10000",
                 "--pad=L", "--ly=25", "--prune-hop=3", "--prune-sc=40"])
-        
         captured = capsys.readouterr()
         # with capsys.disabled():
         #      print("Here")
         #      print(captured.out)
         #      print("to Here")
         assert "BEGINNING CHECKLIST FOR Sol/Abraham Lincoln -> LHS 449/Fisher Point" in captured.out
         assert "35 : Sell 212 x Polymers"
```

### Comparing `tradedangerous-10.9.8/tests/test_trade.py` & `tradedangerous-11.0.0/tests/test_trade.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,84 @@
-import re
-
 import pytest
 
 from tradedangerous.cli import trade
 from tradedangerous.commands.exceptions import UsageError
 from .helpers import copy_fixtures, regex_findin, remove_fixtures
 
 PROG = "trade"
 
+
 def setup_module():
     copy_fixtures()
 
+
 def teardown_module():
     remove_fixtures()
 
-class TestTrade(object):
+
+class TestTrade:
     def test_local_help(self):
         with pytest.raises(UsageError):
             trade([PROG, "local", "-h"])
     
     def test_local_sol(self, capsys):
         trade([PROG, "local", "--ly=10", "--detail", "sol"])
         captured = capsys.readouterr()
         assert "Sol       0" in captured.out
         assert "Ehrlich City" in captured.out
-
-
+    
     def test_sell(self, capsys):
         trade([PROG, "sell", "--near=sol", "hydrogen fuel"])
         captured = capsys.readouterr()
         assert "Sol/Mars High" in captured.out
-
-
+    
     def test_buy(self, capsys):
         trade([PROG, "buy", "--near=sol", "hydrogen fuel"])
         captured = capsys.readouterr()
         assert "Cost      Units DistLy Age/days" in captured.out
-
-
+    
     def test_export_station(self, capsys):
         trade([PROG, "export", "-T", "System"])
         captured = capsys.readouterr()
         assert "NOTE: Export Table 'System'" in captured.out
         # TODO: check that System.csv has a fresh date
-
-
+    
     def test_station_remove(self, capsys):
-        #"Dekker's Yard"
+        # "Dekker's Yard"
         trade([PROG, "station", "-rm", "sol/dekkers"])
         captured = capsys.readouterr()
-        assert regex_findin("NOTE: Sol/Dekker's Yard \(#\d+\) removed", captured.out)
-
-
+        assert regex_findin(r"NOTE: Sol/Dekker's Yard \(#\d+\) removed", captured.out)
+    
     def test_station_add(self, capsys):
-        #"Dekker's Yard"
-        trade([PROG, "station", "--add", "--ls-from-star=5",
+        # "Dekker's Yard"
+        trade([
+            PROG, "station", "--add", "--ls-from-star=5",
             "--market=Y",
             "--black-market=?",
             "--outfitting=?",
             "--pad-size=s",
             "--rearm=?",
             "--refuel=Y",
             "--repair=?",
             "--no-export",
             "sol/Dangerous Delight"])
         captured = capsys.readouterr()
-        assert regex_findin("NOTE: Sol/Dangerous Delight \(#\d+\) added", captured.out)
-
-
+        assert regex_findin(r"NOTE: Sol/Dangerous Delight \(#\d+\) added", captured.out)
+    
     def test_nav(self, capsys):
         trade([PROG, "nav", "--ly-per=50", "sol", "Shinrarta Dezhra"])
         captured = capsys.readouterr()
         assert "System            JumpLy" in captured.out
         assert "Shinrarta Dezhra   47" in captured.out
-
-
+    
     def test_market(self, capsys):
         trade([PROG, "market", "sol/abr"])
         captured = capsys.readouterr()
-        assert "Item                          Buying Selling   Supply" in captured.out
+        assert regex_findin("Item[ ]{3,}Buying Selling[ ]{2,}Supply", captured.out)
         assert "Hydrogen Fuel" in captured.out
-        assert "Water                            323" in captured.out
+        assert regex_findin("Water[ ]{3,}323", captured.out)
     
     @pytest.mark.slow
     def test_import_edcd(self, capsys):
-        #trade import -P=edcd --opt=commodity
         trade([PROG, "import", "-P=edcd", "--opt=commodity"])
         captured = capsys.readouterr()
-        # with capsys.disabled():
-        #     print("Here")
-        #     print(captured.out)
-        #     print("to Here")
-        assert "NOTE: Nothing had to be done" in captured.out
         assert regex_findin(r"NOTE: Found \d+ item\(s\)", captured.out)
-    
-    @pytest.mark.slow
-    def test_import_maddavo(self, capsys):
-        #trade import -P maddavo -i -O use2d
-        trade([PROG, "import", "-P=maddavo", "-i", "--opt=use2d"])
-        captured = capsys.readouterr()
-        # with capsys.disabled():
-        #     print("Here")
-        #     print(captured.out)
-        #     print("to Here")
-        assert regex_findin(r"NOTE: Import complete: \d+ items over \d+ stations in \d+ systems", captured.out)
```

### Comparing `tradedangerous-10.9.8/tests/test_bootstrap_commands.py` & `tradedangerous-11.0.0/tests/test_bootstrap_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 class TestBootstrapCommands(unittest.TestCase):
     def test_import_commands(self):
         from tradedangerous import commands
         
         self.assertIn('buildcache', commands.commandIndex)
         self.assertIn('buy', commands.commandIndex)
 
-
     def test_import_buildcache_cmd(self):
         from tradedangerous.commands import buildcache_cmd
     
     def test_import_buy(self):
         from tradedangerous.commands import buy_cmd
     
     def test_import_import_cmd(self):
@@ -43,8 +42,10 @@
         from tradedangerous.commands import shipvendor_cmd
     
     def test_import_station_cmd(self):
         from tradedangerous.commands import station_cmd
     
     def test_import_update_cmd(self):
         from tradedangerous.commands import update_cmd
-
+    
+    def test_import_update_gui(self):
+        from tradedangerous.commands import update_gui
```

### Comparing `tradedangerous-10.9.8/tests/test_bootstrap_plugins.py` & `tradedangerous-11.0.0/tests/test_bootstrap_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-class TestBootstrapPlugins(object):
+class TestBootstrapPlugins:
     def test_import_traded(self):
         import tradedangerous as td
     
     def test_import_plugins(self):
         from tradedangerous import plugins
     
     def test_import_plugins_eddblink(self):
```

### Comparing `tradedangerous-10.9.8/tests/test_peek.py` & `tradedangerous-11.0.0/tests/test_peek.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 import random
 
 import pytest
 
 from tradedangerous.tradedb import TradeDB, Station, System
-from .helpers import is_initialized, copy_fixtures
+from .helpers import copy_fixtures
 
-ORIGIN='Shinrarta Dezhra'
-tdb = None
+ORIGIN = 'Shinrarta Dezhra'
+# tdb = None
 
 def setup_module():
     copy_fixtures()
 
-def route_to_closest(tdb, origin, destinations, maxLy=15):
+def route_to_closest(tdb: TradeDB, origin, destinations, maxLy=15):
     closest = min(destinations, key=lambda candidate: candidate.distanceTo(origin))
     print("Closest:", closest.name(), closest.distanceTo(origin))
     route = tdb.getRoute(origin, closest, maxLy)
     if not route:
         print("No route found.")
     else:
         print("Route:", ", ".join(system.name() for system, distance in route))
     return route
 
-class TestPeek(object):
+def should_skip() -> bool:
+    return False  # os.getenv("CI") != None
+
+
+class TestPeek:
     """
     Tests based on https://github.com/eyeonus/Trade-Dangerous/wiki/Python-Quick-Peek
     """
-    def test_quick_origin(self, tdb):
+    
+    @pytest.mark.skipif(should_skip(), reason="does not work with CI")
+    def test_quick_origin(self, tdb: TradeDB):
         # Look up a particular system
         origin = tdb.lookupSystem(ORIGIN)
         
         assert 55.71875 == origin.posX
         assert 17.59375 == origin.posY
         assert 27.15625, origin.posZ
         
@@ -45,29 +51,30 @@
 
         # Look up a station in a particular system
         sol = tdb.lookupSystem("sol")
         abe2 = tdb.lookupStation("Abraham Lincoln", sol)
         
         assert abe1 == abe2
     
+    @pytest.mark.skipif(should_skip(), reason="does not work with CI")
     def test_quick_lookupPlace(self, tdb):
         # Look up a system or station using the flexible naming mechanism
         phoenix = tdb.lookupPlace("dunyach")
         assert str(type(phoenix)) == "<class 'tradedangerous.tradedb.Station'>"  # tell me what type of thing "phoenix" is...
         
         sol = tdb.lookupPlace("@sol")
         assert str(type(sol)) == "<class 'tradedangerous.tradedb.System'>"
         
         lave = tdb.lookupPlace("stein")
         assert isinstance(lave, System)
         
         abe = tdb.lookupPlace("sol/hamlinc")
         assert isinstance(abe, Station)
-
-
+    
+    @pytest.mark.skipif(should_skip(), reason="does not work with CI")
     def test_quick_five(self, tdb):
         systemTable = tdb.systemByID.values()
         visitMe = random.sample(list(systemTable), 5)
         origin = tdb.lookupPlace(ORIGIN)
         # Call distanceTo(origin) on every member of visitMe and
         # then retrieve the one with the lowest distance.
         closest = min(visitMe, key=lambda candidate: candidate.distanceTo(origin))
@@ -77,24 +84,26 @@
         ))
         route = tdb.getRoute(origin, closest, 15)
         if not route:
             print("Shame, couldn't find a route.")
         else:
             # Route is a list of Systems. Turn it into a list of
             # System names...
-            routeNames = [ system.name() for system, distance in route ]
+            routeNames = [system.name() for system, distance in route]
             print("Route:", routeNames)
         
         route_to_closest(tdb, origin, visitMe)
         route_to_closest(tdb, origin, visitMe, 20)
         
         # lets change origin
         origin = tdb.lookupSystem("Toolfa")
         route_to_closest(tdb, origin, visitMe)
     
+    @pytest.mark.skipif(should_skip(), reason="does not work with CI")
     def test_three_different(self, tdb):
         # lets try a different route:
         sol = tdb.lookupSystem("sol")
         lhs = tdb.lookupSystem("lhs 380")
         bhr = tdb.lookupSystem("bhritzameno")
         
-        result = route_to_closest(tdb, sol, [ lhs, bhr ])
+        route_to_closest(tdb, sol, [lhs, bhr])
+
```

### Comparing `tradedangerous-10.9.8/tests/test_fs.py` & `tradedangerous-11.0.0/tests/test_fs.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     fs.ensurefolder(tdenv.tmpDir)
 
 @pytest.fixture
 def tdenv():
     return TradeEnv()
 
 
-class TestFS(object):
+class TestFS:
     
     def test_copy(self, tdenv):
         src = fs.pathify(tdenv.templateDir, 'TradeDangerous.sql')
         dst = fs.pathify(tdenv.tmpDir, src.name)
         fs.copy(src, dst)
         assert dst.exists() and dst.is_file()
     
@@ -31,14 +31,15 @@
         if flagfile.exists():
             flagfile.unlink()
         
         def action():
             self.result = True
         
         flag = fs.ensureflag(flagfile, action)
-        assert self.result == True
+        assert self.result is True
+        assert flag is not None
     
     def test_copyallfiles(self, tdenv):
         setup_module()
         fs.copyallfiles(tdenv.templateDir, tdenv.tmpDir)
         test = Path(tdenv.tmpDir, 'Added.csv')
         assert test.exists() and test.is_file()
```

### Comparing `tradedangerous-10.9.8/tests/test_utils.py` & `tradedangerous-11.0.0/tests/test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import pytest
+import pytest   # noqa: F401
 
 from tradedangerous import utils
 from tradedangerous import TradeEnv
 
 
-class TestUtils(object):
+class TestUtils:    # should inherit from TestCase
     # TODO: Test 'von' etc.
     
     def test_titleFixup_s(self):
         assert "Smith's" == utils.titleFixup("smith's")
     
     def test_titleFixup_mc(self):
         assert 'McDonald' == utils.titleFixup('mcdonald')
```

