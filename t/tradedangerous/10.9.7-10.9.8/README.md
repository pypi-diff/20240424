# Comparing `tmp/tradedangerous-10.9.7.tar.gz` & `tmp/tradedangerous-10.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tradedangerous-10.9.7.tar", last modified: Fri Feb  5 05:56:08 2021, max compression
+gzip compressed data, was "dist/tradedangerous-10.9.8.tar", last modified: Fri Feb  5 06:33:03 2021, max compression
```

## Comparing `tradedangerous-10.9.7.tar` & `tradedangerous-10.9.8.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      580 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     5447 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/conf.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1675 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/source/tradedangerous.plugins.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     3350 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/source/tradedangerous.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/source/modules.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     4597 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/installation.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/index.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/develop.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      787 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)      554 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/docs/about.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     4133 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    57370 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/CHANGES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous/
--rw-rw-r--   0 travis    (2000) travis    (2000)    32951 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9923 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/transfers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1473 2021-02-05 05:56:01.000000 tradedangerous-10.9.7/tradedangerous/corrections.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42292 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/tradecalc.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)    94739 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/templates/DefaultShipIndex.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8079 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/templates/TradeDangerous.sql
--rw-rw-r--   0 travis    (2000) travis    (2000)      649 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/templates/Added.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    10483 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/templates/RareItem.csv
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous/plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14470 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/plugins/edcd_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13456 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/plugins/netlog_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4224 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/plugins/edmc_batch_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23696 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/plugins/journal_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7868 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/plugins/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53929 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/plugins/eddblink_plug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42275 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/plugins/edapi_plug.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4468 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/export_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5683 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/import_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7716 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/olddata_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8356 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/nav_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14583 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/update_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15742 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/station_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2332 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/buildcache_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3175 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/trade_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/TEMPLATE.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3142 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12965 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/buy_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46327 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/run_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9097 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/commandenv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5896 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/parsing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9640 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8924 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/rares_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5458 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/market_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8242 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/local_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7600 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/sell_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23376 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/update_gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7023 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/commands/shipvendor_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4302 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/tradeenv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29878 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4727 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      368 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/tradeexcept.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous/misc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3459 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/edsm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14979 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/edsc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4942 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/prices-json-exp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1843 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/eddb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4929 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/diff-system-csvs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2066 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/coord64.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     2127 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/progress.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1681 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/clipboard.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12156 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/eddn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/coord64.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8434 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/checkpricebounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      779 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/derp-sentinel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1785 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/importeddbstats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      859 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/misc/badstations.pl
--rw-rw-r--   0 travis    (2000) travis    (2000)     7593 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/prices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2530 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/fs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7013 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/jsonprices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5186 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12395 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/submit-distances.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2021-02-05 05:56:01.000000 tradedangerous-10.9.7/tradedangerous/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous/mfd/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3065 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/mfd/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tradedangerous/mfd/saitek/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24748 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/mfd/saitek/directoutput.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5912 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/mfd/saitek/x52pro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/mfd/saitek/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72639 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/tradedb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4034 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/mapping.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8713 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/csvexport.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1122 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17338 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/edscupdate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14925 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/edsmupdate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6162 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerous/formatting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    50878 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tradedangerouscrest.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)     3324 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/fix-indent.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      406 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/.gitignore
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)      961 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/config.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)    10480 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/td-completion.bash
--rwxrwxr-x   0 travis    (2000) travis    (2000)      561 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/tdrun
--rw-rw-r--   0 travis    (2000) travis    (2000)      338 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/WINDOWS.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)      427 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/tdbuyfrom
--rw-rw-r--   0 travis    (2000) travis    (2000)    12583 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/getstation.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)     9101 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/README.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2978 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/tradebrute.bat
--rwxrwxr-x   0 travis    (2000) travis    (2000)      217 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/tdupd
--rwxrwxr-x   0 travis    (2000) travis    (2000)      441 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/tdloc
--rwxrwxr-x   0 travis    (2000) travis    (2000)      202 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/tdimad
--rw-rw-r--   0 travis    (2000) travis    (2000)     2305 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/trade.bat
--rwxrwxr-x   0 travis    (2000) travis    (2000)      212 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/scripts/tdnav
--rw-rw-r--   0 travis    (2000) travis    (2000)      288 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/TradeDangerous.sln
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/requirements/publish.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/requirements/dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      778 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    16725 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     4409 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/TradeDangerous.pyproj
--rw-rw-r--   0 travis    (2000) travis    (2000)     1365 2021-02-05 05:56:01.000000 tradedangerous-10.9.7/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 05:56:08.000000 tradedangerous-10.9.7/tests/fixtures/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9026 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/Item.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/FDevShipyard.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/ShipVendor.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    42224 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/Upgrade.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/UpgradeVendor.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/Ship.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     6493 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/System.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/FDevOutfitting.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      757 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/Added.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/RareItem.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/Category.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    42743 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/Station.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  1787951 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/StationItem.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  4416512 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/fixtures/TradeDangerous.db
--rw-rw-r--   0 travis    (2000) travis    (2000)      211 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_commands.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1107 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2575 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_trade_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1866 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_trade_import_eddblink.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3568 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_bootstrap_commands.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_bootstrap_plugins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3487 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_peek.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_fs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      842 2021-02-05 05:55:42.000000 tradedangerous-10.9.7/tests/test_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      580 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5447 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/conf.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/docs/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1675 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/source/tradedangerous.plugins.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3350 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/source/tradedangerous.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/source/modules.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4597 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/installation.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      646 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/index.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/develop.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      787 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)      554 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/docs/about.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4133 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       53 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    57370 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/CHANGES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32951 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9923 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/transfers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1441 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/corrections.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42292 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tradecalc.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    94739 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/templates/DefaultShipIndex.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8079 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/templates/TradeDangerous.sql
+-rw-rw-r--   0 travis    (2000) travis    (2000)      649 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/templates/Added.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10483 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/templates/RareItem.csv
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/plugins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14470 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/edcd_plug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13456 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/netlog_plug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4224 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/edmc_batch_plug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23696 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/journal_plug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7868 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53929 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/eddblink_plug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42275 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/plugins/edapi_plug.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4468 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/export_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5683 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/import_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7716 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/olddata_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8356 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/nav_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14583 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/update_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15742 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/station_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2332 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/buildcache_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3175 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/trade_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2124 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/TEMPLATE.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3142 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12965 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/buy_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46327 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/run_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9097 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/commandenv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5896 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/parsing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9640 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8924 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/rares_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5458 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/market_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8242 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/local_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7600 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/sell_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23376 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/update_gui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7023 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/commands/shipvendor_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4302 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tradeenv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29878 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/gui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4727 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      368 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tradeexcept.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/misc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3459 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/edsm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14979 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/edsc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4942 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/prices-json-exp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1843 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/eddb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4929 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/diff-system-csvs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2066 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/coord64.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2127 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/progress.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1681 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/clipboard.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12156 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/eddn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/coord64.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8434 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/checkpricebounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      779 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/derp-sentinel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1785 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/importeddbstats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      859 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/misc/badstations.pl
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7593 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/prices.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2530 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/fs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7013 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/jsonprices.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5186 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12395 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/submit-distances.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      646 2021-02-05 06:32:56.000000 tradedangerous-10.9.8/tradedangerous/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/mfd/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3065 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mfd/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tradedangerous/mfd/saitek/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24748 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mfd/saitek/directoutput.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5912 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mfd/saitek/x52pro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mfd/saitek/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72639 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/tradedb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4034 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/mapping.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8713 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/csvexport.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1122 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17338 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/edscupdate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14925 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/edsmupdate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6162 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerous/formatting.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4634 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50878 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tradedangerouscrest.ico
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3324 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      359 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tox.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/fix-indent.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      406 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/.gitignore
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      961 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/config.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10480 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/td-completion.bash
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      561 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdrun
+-rw-rw-r--   0 travis    (2000) travis    (2000)      338 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/WINDOWS.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      427 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdbuyfrom
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12583 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/getstation.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9101 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/README.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2978 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tradebrute.bat
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      217 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdupd
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      441 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdloc
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      202 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdimad
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2305 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/trade.bat
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      212 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/scripts/tdnav
+-rw-rw-r--   0 travis    (2000) travis    (2000)      288 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/TradeDangerous.sln
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/requirements/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/requirements/publish.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       55 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/requirements/dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      778 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16725 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4409 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/TradeDangerous.pyproj
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1542 2021-02-05 06:32:56.000000 tradedangerous-10.9.8/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tests/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-05 06:33:03.000000 tradedangerous-10.9.8/tests/fixtures/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9026 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Item.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/FDevShipyard.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/ShipVendor.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42224 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Upgrade.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/UpgradeVendor.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Ship.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6493 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/System.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/FDevOutfitting.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      757 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Added.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      119 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/RareItem.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      250 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Category.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42743 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/Station.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1787951 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/StationItem.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)  4416512 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/fixtures/TradeDangerous.db
+-rw-rw-r--   0 travis    (2000) travis    (2000)      211 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_commands.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1107 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2575 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_trade_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1866 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_trade_import_eddblink.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3568 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_bootstrap_commands.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_bootstrap_plugins.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3487 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_peek.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_fs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      842 2021-02-05 06:32:38.000000 tradedangerous-10.9.8/tests/test_utils.py
```

### Comparing `tradedangerous-10.9.7/docs/Makefile` & `tradedangerous-10.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/docs/conf.py` & `tradedangerous-10.9.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/docs/source/tradedangerous.plugins.md` & `tradedangerous-10.9.8/docs/source/tradedangerous.plugins.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/docs/source/tradedangerous.md` & `tradedangerous-10.9.8/docs/source/tradedangerous.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/docs/installation.md` & `tradedangerous-10.9.8/docs/installation.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/docs/index.md` & `tradedangerous-10.9.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/docs/develop.md` & `tradedangerous-10.9.8/docs/develop.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/docs/make.bat` & `tradedangerous-10.9.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/docs/about.md` & `tradedangerous-10.9.8/docs/about.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous.egg-info/PKG-INFO` & `tradedangerous-10.9.8/tradedangerous.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 10.9.7
+Version: 10.9.8
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-10.9.7/tradedangerous.egg-info/SOURCES.txt` & `tradedangerous-10.9.8/tradedangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/CHANGES.txt` & `tradedangerous-10.9.8/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/cache.py` & `tradedangerous-10.9.8/tradedangerous/cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/transfers.py` & `tradedangerous-10.9.8/tradedangerous/transfers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/tools.py` & `tradedangerous-10.9.8/tradedangerous/tools.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/corrections.py` & `tradedangerous-10.9.8/tradedangerous/corrections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-# Provides an interface for correcting star/station names that
+# Provides an interface for correcting names that
 # have changed in recent versions.
 
 from __future__ import absolute_import, with_statement, print_function, division, unicode_literals
 
 # Arbitrary, negative value to denote something that's been removed.
 DELETED = -111
 
 systems = {
     "PANDAMONIUM": "PANDEMONIUM",
     "ARGETLÁMH": "ARGETLAMH",
     "LíFTHRUTI": "LIFTHRUTI",
     "MANTóAC": "MANTOAC",
     "NANTóAC": "NANTOAC",
-
-#ADD_SYSTEMS_HERE
 }
 
 stations = {
 }
 
 categories = {
 }
```

### Comparing `tradedangerous-10.9.7/tradedangerous/tradecalc.py` & `tradedangerous-10.9.8/tradedangerous/tradecalc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/templates/DefaultShipIndex.json` & `tradedangerous-10.9.8/tradedangerous/templates/DefaultShipIndex.json`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/templates/TradeDangerous.sql` & `tradedangerous-10.9.8/tradedangerous/templates/TradeDangerous.sql`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/templates/Added.csv` & `tradedangerous-10.9.8/tradedangerous/templates/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/templates/RareItem.csv` & `tradedangerous-10.9.8/tradedangerous/templates/RareItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/plugins/edcd_plug.py` & `tradedangerous-10.9.8/tradedangerous/plugins/edcd_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/plugins/netlog_plug.py` & `tradedangerous-10.9.8/tradedangerous/plugins/netlog_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/plugins/edmc_batch_plug.py` & `tradedangerous-10.9.8/tradedangerous/plugins/edmc_batch_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/plugins/journal_plug.py` & `tradedangerous-10.9.8/tradedangerous/plugins/journal_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/plugins/__init__.py` & `tradedangerous-10.9.8/tradedangerous/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/plugins/eddblink_plug.py` & `tradedangerous-10.9.8/tradedangerous/plugins/eddblink_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/plugins/edapi_plug.py` & `tradedangerous-10.9.8/tradedangerous/plugins/edapi_plug.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/export_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/export_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/import_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/olddata_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/olddata_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/nav_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/nav_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/update_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/update_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/station_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/station_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/buildcache_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/buildcache_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/trade_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/trade_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/TEMPLATE.py` & `tradedangerous-10.9.8/tradedangerous/commands/TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/exceptions.py` & `tradedangerous-10.9.8/tradedangerous/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/buy_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/buy_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/run_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/run_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/commandenv.py` & `tradedangerous-10.9.8/tradedangerous/commands/commandenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/parsing.py` & `tradedangerous-10.9.8/tradedangerous/commands/parsing.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/__init__.py` & `tradedangerous-10.9.8/tradedangerous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/rares_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/rares_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/market_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/market_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/local_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/local_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/sell_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/sell_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/update_gui.py` & `tradedangerous-10.9.8/tradedangerous/commands/update_gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/commands/shipvendor_cmd.py` & `tradedangerous-10.9.8/tradedangerous/commands/shipvendor_cmd.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/tradeenv.py` & `tradedangerous-10.9.8/tradedangerous/tradeenv.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/gui.py` & `tradedangerous-10.9.8/tradedangerous/gui.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/cli.py` & `tradedangerous-10.9.8/tradedangerous/cli.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/edsm.py` & `tradedangerous-10.9.8/tradedangerous/misc/edsm.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/edsc.py` & `tradedangerous-10.9.8/tradedangerous/misc/edsc.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/prices-json-exp.py` & `tradedangerous-10.9.8/tradedangerous/misc/prices-json-exp.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/eddb.py` & `tradedangerous-10.9.8/tradedangerous/misc/eddb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/diff-system-csvs.py` & `tradedangerous-10.9.8/tradedangerous/misc/diff-system-csvs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/coord64.js` & `tradedangerous-10.9.8/tradedangerous/misc/coord64.js`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/progress.py` & `tradedangerous-10.9.8/tradedangerous/misc/progress.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/clipboard.py` & `tradedangerous-10.9.8/tradedangerous/misc/clipboard.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/eddn.py` & `tradedangerous-10.9.8/tradedangerous/misc/eddn.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/coord64.py` & `tradedangerous-10.9.8/tradedangerous/misc/coord64.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/checkpricebounds.py` & `tradedangerous-10.9.8/tradedangerous/misc/checkpricebounds.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/derp-sentinel.py` & `tradedangerous-10.9.8/tradedangerous/misc/derp-sentinel.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/importeddbstats.py` & `tradedangerous-10.9.8/tradedangerous/misc/importeddbstats.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/misc/badstations.pl` & `tradedangerous-10.9.8/tradedangerous/misc/badstations.pl`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/prices.py` & `tradedangerous-10.9.8/tradedangerous/prices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/fs.py` & `tradedangerous-10.9.8/tradedangerous/fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/jsonprices.py` & `tradedangerous-10.9.8/tradedangerous/jsonprices.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/utils.py` & `tradedangerous-10.9.8/tradedangerous/utils.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/submit-distances.py` & `tradedangerous-10.9.8/tradedangerous/submit-distances.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/trade.py` & `tradedangerous-10.9.8/tradedangerous/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/version.py` & `tradedangerous-10.9.8/tradedangerous/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # this software so long as you include this copyright notice.
 # I guarantee there is at least one bug neither of us knew about.
 # --------------------------------------------------------------------
 
 """just keeper of current version"""
 
 # TODO: remember to update tests when version changes
-__version__ = '10.9.7'
+__version__ = '10.9.8'
```

### Comparing `tradedangerous-10.9.7/tradedangerous/mfd/__init__.py` & `tradedangerous-10.9.8/tradedangerous/mfd/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/mfd/saitek/directoutput.py` & `tradedangerous-10.9.8/tradedangerous/mfd/saitek/directoutput.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/mfd/saitek/x52pro.py` & `tradedangerous-10.9.8/tradedangerous/mfd/saitek/x52pro.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/tradedb.py` & `tradedangerous-10.9.8/tradedangerous/tradedb.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/mapping.py` & `tradedangerous-10.9.8/tradedangerous/mapping.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/csvexport.py` & `tradedangerous-10.9.8/tradedangerous/csvexport.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/__init__.py` & `tradedangerous-10.9.8/tradedangerous/__init__.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/edscupdate.py` & `tradedangerous-10.9.8/tradedangerous/edscupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/edsmupdate.py` & `tradedangerous-10.9.8/tradedangerous/edsmupdate.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tradedangerous/formatting.py` & `tradedangerous-10.9.8/tradedangerous/formatting.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/PKG-INFO` & `tradedangerous-10.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradedangerous
-Version: 10.9.7
+Version: 10.9.8
 Summary: Trade-Dangerous is a set of powerful trading tools for Elite Dangerous, organized around one of the most powerful trade run optimizers available.
 Home-page: https://github.com/eyeonus/Trade-Dangerous
 Author: eyeonus
 Author-email: eyeonus@gmail.com
 License: MPL
 Project-URL: Bug Tracker, https://github.com/eyeonus/Trade-Dangerous/issues
 Project-URL: Documentation, https://github.com/eyeonus/Trade-Dangerous/wiki
```

### Comparing `tradedangerous-10.9.7/tradedangerouscrest.ico` & `tradedangerous-10.9.8/tradedangerouscrest.ico`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/README.md` & `tradedangerous-10.9.8/README.md`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/scripts/config.sh` & `tradedangerous-10.9.8/scripts/config.sh`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/scripts/td-completion.bash` & `tradedangerous-10.9.8/scripts/td-completion.bash`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/scripts/tdrun` & `tradedangerous-10.9.8/scripts/tdrun`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/scripts/getstation.sh` & `tradedangerous-10.9.8/scripts/getstation.sh`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/scripts/README.txt` & `tradedangerous-10.9.8/scripts/README.txt`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/scripts/tradebrute.bat` & `tradedangerous-10.9.8/scripts/tradebrute.bat`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/scripts/trade.bat` & `tradedangerous-10.9.8/scripts/trade.bat`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/trade.py` & `tradedangerous-10.9.8/trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/TradeDangerous.sln` & `tradedangerous-10.9.8/TradeDangerous.sln`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/.travis.yml` & `tradedangerous-10.9.8/.travis.yml`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/LICENSE` & `tradedangerous-10.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/TradeDangerous.pyproj` & `tradedangerous-10.9.8/TradeDangerous.pyproj`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/CHANGELOG.md` & `tradedangerous-10.9.8/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v10.9.8 (2021-02-05)
+### Fix
+* Update the build semantic, you jerk ([`8ca4e39`](https://github.com/eyeonus/Trade-Dangerous/commit/8ca4e392f7949e106636a1fee90a0d381b8a03e0))
+
 ## v10.9.7 (2021-02-05)
 ### Fix
 * Add 'VOID OPAL' to corrections ([`f208023`](https://github.com/eyeonus/Trade-Dangerous/commit/f20802319a503f569d836c8d46ca7231779f5024))
 
 ## v10.9.6 (2021-01-18)
 ### Fix
 * Edmc_batch_plug Path issues ([#83](https://github.com/eyeonus/Trade-Dangerous/issues/83)) ([`ef06684`](https://github.com/eyeonus/Trade-Dangerous/commit/ef06684e0534d1d969658e9b55f3a752c502475e))
```

### Comparing `tradedangerous-10.9.7/setup.py` & `tradedangerous-10.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/fixtures/Item.csv` & `tradedangerous-10.9.8/tests/fixtures/Item.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/fixtures/Upgrade.csv` & `tradedangerous-10.9.8/tests/fixtures/Upgrade.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/fixtures/Ship.csv` & `tradedangerous-10.9.8/tests/fixtures/Ship.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/fixtures/System.csv` & `tradedangerous-10.9.8/tests/fixtures/System.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/fixtures/Added.csv` & `tradedangerous-10.9.8/tests/fixtures/Added.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/fixtures/Station.csv` & `tradedangerous-10.9.8/tests/fixtures/Station.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/fixtures/StationItem.csv` & `tradedangerous-10.9.8/tests/fixtures/StationItem.csv`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/fixtures/TradeDangerous.db` & `tradedangerous-10.9.8/tests/fixtures/TradeDangerous.db`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_commands.py` & `tradedangerous-10.9.8/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_cache.py` & `tradedangerous-10.9.8/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_trade_run.py` & `tradedangerous-10.9.8/tests/test_trade_run.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_trade_import_eddblink.py` & `tradedangerous-10.9.8/tests/test_trade_import_eddblink.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_trade.py` & `tradedangerous-10.9.8/tests/test_trade.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_bootstrap_commands.py` & `tradedangerous-10.9.8/tests/test_bootstrap_commands.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_bootstrap_plugins.py` & `tradedangerous-10.9.8/tests/test_bootstrap_plugins.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_peek.py` & `tradedangerous-10.9.8/tests/test_peek.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_fs.py` & `tradedangerous-10.9.8/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/conftest.py` & `tradedangerous-10.9.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/helpers.py` & `tradedangerous-10.9.8/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `tradedangerous-10.9.7/tests/test_utils.py` & `tradedangerous-10.9.8/tests/test_utils.py`

 * *Files identical despite different names*

