# Comparing `tmp/ragu-0.1.31.tar.gz` & `tmp/ragu-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragu-0.1.31.tar", last modified: Tue Apr 23 21:25:59 2024, max compression
+gzip compressed data, was "ragu-0.1.32.tar", last modified: Wed Apr 24 18:47:38 2024, max compression
```

## Comparing `ragu-0.1.31.tar` & `ragu-0.1.32.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.641100 ragu-0.1.31/
--rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.31/LICENSE.txt
--rw-r--r--   0 btober     (501) staff       (20)    47505 2024-04-23 21:25:59.640848 ragu-0.1.31/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     6295 2024-04-19 17:28:40.000000 ragu-0.1.31/README.md
--rw-r--r--   0 btober     (501) staff       (20)      942 2024-04-23 21:25:07.000000 ragu-0.1.31/pyproject.toml
--rw-r--r--   0 btober     (501) staff       (20)       38 2024-04-23 21:25:59.641133 ragu-0.1.31/setup.cfg
--rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.31/setup.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.612553 ragu-0.1.31/src/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.613818 ragu-0.1.31/src/ragu/
--rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/__init__.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.614678 ragu-0.1.31/src/ragu/bin/
--rw-r--r--   0 btober     (501) staff       (20)     2574 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/bin/ragu.py
--rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/config.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.612711 ragu-0.1.31/src/ragu/dat/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.614804 ragu-0.1.31/src/ragu/dat/mars/
--rw-r--r--   0 btober     (501) staff       (20) 33196562 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/dat/mars/mega90n000eb.tif
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.634570 ragu-0.1.31/src/ragu/ingest/
--rw-r--r--   0 btober     (501) staff       (20)     5750 2024-04-19 16:57:42.000000 ragu-0.1.31/src/ragu/ingest/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     2411 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_cresis_rds.py
--rw-r--r--   0 btober     (501) staff       (20)     2454 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_cresis_snow.py
--rw-r--r--   0 btober     (501) staff       (20)     3123 2024-04-23 21:24:25.000000 ragu-0.1.31/src/ragu/ingest/ingest_groundhog.py
--rw-r--r--   0 btober     (501) staff       (20)     3366 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_gssi.py
--rw-r--r--   0 btober     (501) staff       (20)     2562 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_lrs.py
--rw-r--r--   0 btober     (501) staff       (20)     2896 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_marsis.py
--rw-r--r--   0 btober     (501) staff       (20)     2474 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_marsis_ipc.py
--rw-r--r--   0 btober     (501) staff       (20)     5780 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_oibAK.py
--rw-r--r--   0 btober     (501) staff       (20)    14181 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_pulseekko.py
--rw-r--r--   0 btober     (501) staff       (20)     2537 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_rimfax.py
--rw-r--r--   0 btober     (501) staff       (20)     2931 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_sharad.py
--rw-r--r--   0 btober     (501) staff       (20)     3640 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_template.py
--rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/ingest/ingest_uaf_kentech.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.634911 ragu-0.1.31/src/ragu/nav/
--rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/nav/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/nav/gps.py
--rw-r--r--   0 btober     (501) staff       (20)    21420 2024-04-22 00:33:24.000000 ragu-0.1.31/src/ragu/nav/navparse.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.636890 ragu-0.1.31/src/ragu/radar/
--rw-r--r--   0 btober     (501) staff       (20)     7814 2024-04-23 21:24:56.000000 ragu-0.1.31/src/ragu/radar/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/radar/flags.py
--rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/radar/pick.py
--rw-r--r--   0 btober     (501) staff       (20)    14029 2024-04-19 16:55:41.000000 ragu-0.1.31/src/ragu/radar/processing.py
--rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/raguError.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.639328 ragu-0.1.31/src/ragu/recs/
--rw-r--r--   0 btober     (501) staff       (20)  1079564 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/recs/20190928-235534_compiled.jpg
--rw-r--r--   0 btober     (501) staff       (20)    16176 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/recs/basemap_icon.png
--rw-r--r--   0 btober     (501) staff       (20)    92542 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/recs/bulb.jpg
--rw-r--r--   0 btober     (501) staff       (20)    21590 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/recs/ragu_logo.png
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.639809 ragu-0.1.31/src/ragu/tools/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/tools/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/tools/constants.py
--rw-r--r--   0 btober     (501) staff       (20)     9245 2024-04-19 16:56:13.000000 ragu-0.1.31/src/ragu/tools/export.py
--rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/tools/utils.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.640520 ragu-0.1.31/src/ragu/ui/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/ui/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)    16621 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/ui/basemap.py
--rw-r--r--   0 btober     (501) staff       (20)    68791 2024-04-19 16:46:29.000000 ragu-0.1.31/src/ragu/ui/gui.py
--rw-r--r--   0 btober     (501) staff       (20)    71060 2024-04-23 21:19:13.000000 ragu-0.1.31/src/ragu/ui/impick.py
--rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/ui/notepad.py
--rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/ui/wvpick.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.614524 ragu-0.1.31/src/ragu.egg-info/
--rw-r--r--   0 btober     (501) staff       (20)    47505 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     1369 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/SOURCES.txt
--rw-r--r--   0 btober     (501) staff       (20)        1 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/dependency_links.txt
--rw-r--r--   0 btober     (501) staff       (20)       44 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/entry_points.txt
--rw-r--r--   0 btober     (501) staff       (20)       64 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/requires.txt
--rw-r--r--   0 btober     (501) staff       (20)       10 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/top_level.txt
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.958103 ragu-0.1.32/
+-rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.32/LICENSE.txt
+-rw-r--r--   0 btober     (501) staff       (20)    47505 2024-04-24 18:47:38.957847 ragu-0.1.32/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     6295 2024-04-19 17:28:40.000000 ragu-0.1.32/README.md
+-rw-r--r--   0 btober     (501) staff       (20)      942 2024-04-24 18:42:50.000000 ragu-0.1.32/pyproject.toml
+-rw-r--r--   0 btober     (501) staff       (20)       38 2024-04-24 18:47:38.958138 ragu-0.1.32/setup.cfg
+-rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.32/setup.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.924973 ragu-0.1.32/src/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.926223 ragu-0.1.32/src/ragu/
+-rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/__init__.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.926993 ragu-0.1.32/src/ragu/bin/
+-rw-r--r--   0 btober     (501) staff       (20)     2574 2024-02-24 23:44:42.000000 ragu-0.1.32/src/ragu/bin/ragu.py
+-rw-r--r--   0 btober     (501) staff       (20)     2112 2024-04-24 18:46:05.000000 ragu-0.1.32/src/ragu/config.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.925122 ragu-0.1.32/src/ragu/dat/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.927086 ragu-0.1.32/src/ragu/dat/mars/
+-rw-r--r--   0 btober     (501) staff       (20) 33196562 2024-02-24 23:44:42.000000 ragu-0.1.32/src/ragu/dat/mars/mega90n000eb.tif
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.951122 ragu-0.1.32/src/ragu/ingest/
+-rw-r--r--   0 btober     (501) staff       (20)     5750 2024-04-19 16:57:42.000000 ragu-0.1.32/src/ragu/ingest/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     2411 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_cresis_rds.py
+-rw-r--r--   0 btober     (501) staff       (20)     2454 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_cresis_snow.py
+-rw-r--r--   0 btober     (501) staff       (20)     3089 2024-04-24 18:40:40.000000 ragu-0.1.32/src/ragu/ingest/ingest_groundhog.py
+-rw-r--r--   0 btober     (501) staff       (20)     3366 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_gssi.py
+-rw-r--r--   0 btober     (501) staff       (20)     2562 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_lrs.py
+-rw-r--r--   0 btober     (501) staff       (20)     2896 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_marsis.py
+-rw-r--r--   0 btober     (501) staff       (20)     2474 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_marsis_ipc.py
+-rw-r--r--   0 btober     (501) staff       (20)     5780 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_oibAK.py
+-rw-r--r--   0 btober     (501) staff       (20)    14181 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_pulseekko.py
+-rw-r--r--   0 btober     (501) staff       (20)     2537 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_rimfax.py
+-rw-r--r--   0 btober     (501) staff       (20)     2931 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_sharad.py
+-rw-r--r--   0 btober     (501) staff       (20)     3640 2024-04-19 16:41:20.000000 ragu-0.1.32/src/ragu/ingest/ingest_template.py
+-rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/ingest/ingest_uaf_kentech.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.951816 ragu-0.1.32/src/ragu/nav/
+-rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/nav/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/nav/gps.py
+-rw-r--r--   0 btober     (501) staff       (20)    21420 2024-04-22 00:33:24.000000 ragu-0.1.32/src/ragu/nav/navparse.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.952634 ragu-0.1.32/src/ragu/radar/
+-rw-r--r--   0 btober     (501) staff       (20)     7814 2024-04-23 21:24:56.000000 ragu-0.1.32/src/ragu/radar/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/radar/flags.py
+-rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/radar/pick.py
+-rw-r--r--   0 btober     (501) staff       (20)    14029 2024-04-19 16:55:41.000000 ragu-0.1.32/src/ragu/radar/processing.py
+-rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/raguError.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.954878 ragu-0.1.32/src/ragu/recs/
+-rw-r--r--   0 btober     (501) staff       (20)  1079564 2024-02-24 23:44:42.000000 ragu-0.1.32/src/ragu/recs/20190928-235534_compiled.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    16176 2024-02-24 23:44:42.000000 ragu-0.1.32/src/ragu/recs/basemap_icon.png
+-rw-r--r--   0 btober     (501) staff       (20)    92542 2024-02-24 23:44:42.000000 ragu-0.1.32/src/ragu/recs/bulb.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    21590 2024-02-24 23:44:42.000000 ragu-0.1.32/src/ragu/recs/ragu_logo.png
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.955673 ragu-0.1.32/src/ragu/tools/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/tools/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/tools/constants.py
+-rw-r--r--   0 btober     (501) staff       (20)     9245 2024-04-19 16:56:13.000000 ragu-0.1.32/src/ragu/tools/export.py
+-rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/tools/utils.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.957372 ragu-0.1.32/src/ragu/ui/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/ui/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)    16621 2024-02-24 23:44:42.000000 ragu-0.1.32/src/ragu/ui/basemap.py
+-rw-r--r--   0 btober     (501) staff       (20)    68990 2024-04-24 18:42:36.000000 ragu-0.1.32/src/ragu/ui/gui.py
+-rw-r--r--   0 btober     (501) staff       (20)    71060 2024-04-23 21:19:13.000000 ragu-0.1.32/src/ragu/ui/impick.py
+-rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/ui/notepad.py
+-rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.32/src/ragu/ui/wvpick.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-24 18:47:38.926900 ragu-0.1.32/src/ragu.egg-info/
+-rw-r--r--   0 btober     (501) staff       (20)    47505 2024-04-24 18:47:38.000000 ragu-0.1.32/src/ragu.egg-info/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     1369 2024-04-24 18:47:38.000000 ragu-0.1.32/src/ragu.egg-info/SOURCES.txt
+-rw-r--r--   0 btober     (501) staff       (20)        1 2024-04-24 18:47:38.000000 ragu-0.1.32/src/ragu.egg-info/dependency_links.txt
+-rw-r--r--   0 btober     (501) staff       (20)       44 2024-04-24 18:47:38.000000 ragu-0.1.32/src/ragu.egg-info/entry_points.txt
+-rw-r--r--   0 btober     (501) staff       (20)       64 2024-04-24 18:47:38.000000 ragu-0.1.32/src/ragu.egg-info/requires.txt
+-rw-r--r--   0 btober     (501) staff       (20)       10 2024-04-24 18:47:38.000000 ragu-0.1.32/src/ragu.egg-info/top_level.txt
```

### Comparing `ragu-0.1.31/LICENSE.txt` & `ragu-0.1.32/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/PKG-INFO` & `ragu-0.1.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.31
+Version: 0.1.32
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ragu-0.1.31/README.md` & `ragu-0.1.32/README.md`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/pyproject.toml` & `ragu-0.1.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ragu"
-version = "0.1.31"
+version = "0.1.32"
 description = "Radar Analysis Graphical Utility (RAGU)"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 authors = [
      {name = "Brandon Tober", email = "tobers.brandon@gmail.com"},
      {name = "Michael Christoffersen", email = "mchristo28@gmail.com"},
```

### Comparing `ragu-0.1.31/src/ragu/bin/ragu.py` & `ragu-0.1.32/src/ragu/bin/ragu.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/config.py` & `ragu-0.1.32/src/ragu/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     config.set('nav', 'body', 'earth')
     config.set('nav', '# str navcrs: crs string')
     config.set('nav', '# wgs84 projection string for earth: +proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs')
     config.set('nav', '# longlat projection string for mars: +proj=longlat +a=3396190 +b=3376200 +no_defs')
     config.set('nav', 'crs', 'proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs')
 
     config.add_section('output')
+    config.set('output', '# float asep: antenna separation in meters (optional)')
+    config.set('output', 'asep', '')
     config.set('output', '# float eps_r: relative permittivity (dielectric constant), required for plotting in depth and calculating layer thickness')
     config.set('output', 'eps_r', '3.15')
     config.set('output','# bool amp: export pick amplitudes')
     config.set('output','amp', 'True')
     config.set('output','# bool csv: export csv file of picks')
     config.set('output','csv', 'True')
     config.set('output','# bool gpkg: export geopackage of picks')
```

### Comparing `ragu-0.1.31/src/ragu/dat/mars/mega90n000eb.tif` & `ragu-0.1.32/src/ragu/dat/mars/mega90n000eb.tif`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/__init__.py` & `ragu-0.1.32/src/ragu/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_cresis_rds.py` & `ragu-0.1.32/src/ragu/ingest/ingest_cresis_rds.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_cresis_snow.py` & `ragu-0.1.32/src/ragu/ingest/ingest_cresis_snow.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_groundhog.py` & `ragu-0.1.32/src/ragu/ingest/ingest_groundhog.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,14 @@
     rdata.geocrs = navcrs
     rdata.xyzcrs = navparse.xyzsys[body]
     rdata.navdf = navparse.getnav_groundhog(fpath, navcrs, body)
 
     # if rx and tx each have gps, we'll store antenna sep per trace
     if "asep" in rdata.navdf:
         rdata.asep = rdata.navdf["asep"].to_numpy()
-    else:
-        rdata.asep = 50
 
     # groudnhog rx triggers on arrival of airwave - get number of traces pre-trigger to vertically shift the data accordingly
     try:
         pt = f["raw/rx0"].attrs["pre_trig"]
     except KeyError:
         pt = f["raw/rx0"].attrs["pre_trigger"]
```

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_gssi.py` & `ragu-0.1.32/src/ragu/ingest/ingest_gssi.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_lrs.py` & `ragu-0.1.32/src/ragu/ingest/ingest_lrs.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_marsis.py` & `ragu-0.1.32/src/ragu/ingest/ingest_marsis.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_marsis_ipc.py` & `ragu-0.1.32/src/ragu/ingest/ingest_marsis_ipc.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_oibAK.py` & `ragu-0.1.32/src/ragu/ingest/ingest_oibAK.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_pulseekko.py` & `ragu-0.1.32/src/ragu/ingest/ingest_pulseekko.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_rimfax.py` & `ragu-0.1.32/src/ragu/ingest/ingest_rimfax.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_sharad.py` & `ragu-0.1.32/src/ragu/ingest/ingest_sharad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_template.py` & `ragu-0.1.32/src/ragu/ingest/ingest_template.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ingest/ingest_uaf_kentech.py` & `ragu-0.1.32/src/ragu/ingest/ingest_uaf_kentech.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/nav/gps.py` & `ragu-0.1.32/src/ragu/nav/gps.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/nav/navparse.py` & `ragu-0.1.32/src/ragu/nav/navparse.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/radar/__init__.py` & `ragu-0.1.32/src/ragu/radar/__init__.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/radar/pick.py` & `ragu-0.1.32/src/ragu/radar/pick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/radar/processing.py` & `ragu-0.1.32/src/ragu/radar/processing.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/recs/20190928-235534_compiled.jpg` & `ragu-0.1.32/src/ragu/recs/20190928-235534_compiled.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/recs/basemap_icon.png` & `ragu-0.1.32/src/ragu/recs/basemap_icon.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/recs/bulb.jpg` & `ragu-0.1.32/src/ragu/recs/bulb.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/recs/ragu_logo.png` & `ragu-0.1.32/src/ragu/recs/ragu_logo.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/tools/export.py` & `ragu-0.1.32/src/ragu/tools/export.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/tools/utils.py` & `ragu-0.1.32/src/ragu/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ui/basemap.py` & `ragu-0.1.32/src/ragu/ui/basemap.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ui/gui.py` & `ragu-0.1.32/src/ragu/ui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,25 +483,30 @@
             self.open_dfile(temp_loadName)
 
 
     # open_dat loads the data file and passes to other modules
     def open_dfile(self, f_loadName=None, switch=False, direction="Right"):
             # if input selected, clear impick canvas, ingest data and pass to impick
             try:
+            # for fuck in ['bananas']:
                 if f_loadName:
                     # switch to profile tab
                     if self.tab == "Waveform":
                         self.nb.select(self.nb.tabs()[0])
                     self.f_loadName = f_loadName
                     # update and save project file
                     self.proj.update_paths(self.f_loadName, self.map_loadName, self.notepad._notepad__get_file())
                     self.proj.save()
                     # ingest the data
                     self.igst = ingest(self.f_loadName)
                     self.rdata = self.igst.read(self.conf["path"]["simPath"], self.conf["nav"]["crs"], self.conf["nav"]["body"])
+                    try:
+                        self.rdata.asep =  float(self.conf["output"]["asep"])
+                    except:
+                        pass
                     self.impick.clear_canvas()  
                     self.impick.set_vars()
                     self.impick.load(self.rdata)
                     # set existing horizons
                     for horizon in self.rdata.pick.horizons.keys():
                         self.impick.set_picks(horizon=horizon)
                     self.impick.set_pickState(state=False)
```

### Comparing `ragu-0.1.31/src/ragu/ui/impick.py` & `ragu-0.1.32/src/ragu/ui/impick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ui/notepad.py` & `ragu-0.1.32/src/ragu/ui/notepad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu/ui/wvpick.py` & `ragu-0.1.32/src/ragu/ui/wvpick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.31/src/ragu.egg-info/PKG-INFO` & `ragu-0.1.32/src/ragu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.31
+Version: 0.1.32
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ragu-0.1.31/src/ragu.egg-info/SOURCES.txt` & `ragu-0.1.32/src/ragu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

