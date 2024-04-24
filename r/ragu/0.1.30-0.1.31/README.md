# Comparing `tmp/ragu-0.1.30.tar.gz` & `tmp/ragu-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragu-0.1.30.tar", last modified: Fri Apr 19 16:36:20 2024, max compression
+gzip compressed data, was "ragu-0.1.31.tar", last modified: Tue Apr 23 21:25:59 2024, max compression
```

## Comparing `ragu-0.1.30.tar` & `ragu-0.1.31.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.580006 ragu-0.1.30/
--rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.30/LICENSE.txt
--rw-r--r--   0 btober     (501) staff       (20)    47233 2024-04-19 16:36:20.579730 ragu-0.1.30/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     6022 2024-03-29 15:25:52.000000 ragu-0.1.30/README.md
--rw-r--r--   0 btober     (501) staff       (20)      942 2024-04-19 16:29:45.000000 ragu-0.1.30/pyproject.toml
--rw-r--r--   0 btober     (501) staff       (20)       38 2024-04-19 16:36:20.580078 ragu-0.1.30/setup.cfg
--rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.30/setup.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.522058 ragu-0.1.30/src/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.524100 ragu-0.1.30/src/ragu/
--rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/__init__.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.526336 ragu-0.1.30/src/ragu/bin/
--rw-r--r--   0 btober     (501) staff       (20)     2574 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/bin/ragu.py
--rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/config.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.522252 ragu-0.1.30/src/ragu/dat/
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.526889 ragu-0.1.30/src/ragu/dat/mars/
--rw-r--r--   0 btober     (501) staff       (20) 33196562 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/dat/mars/mega90n000eb.tif
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.570591 ragu-0.1.30/src/ragu/ingest/
--rw-r--r--   0 btober     (501) staff       (20)     5753 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ingest/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     2411 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_cresis_rds.py
--rw-r--r--   0 btober     (501) staff       (20)     2454 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_cresis_snow.py
--rw-r--r--   0 btober     (501) staff       (20)     3005 2024-04-05 18:35:16.000000 ragu-0.1.30/src/ragu/ingest/ingest_groundhog.py
--rw-r--r--   0 btober     (501) staff       (20)     3366 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_gssi.py
--rw-r--r--   0 btober     (501) staff       (20)     2562 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_lrs.py
--rw-r--r--   0 btober     (501) staff       (20)     2896 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_marsis.py
--rw-r--r--   0 btober     (501) staff       (20)     2474 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_marsis_ipc.py
--rw-r--r--   0 btober     (501) staff       (20)     5780 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_oibAK.py
--rw-r--r--   0 btober     (501) staff       (20)    14181 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_pulseekko.py
--rw-r--r--   0 btober     (501) staff       (20)     2537 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_rimfax.py
--rw-r--r--   0 btober     (501) staff       (20)     2931 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_sharad.py
--rw-r--r--   0 btober     (501) staff       (20)     3640 2024-03-29 15:04:24.000000 ragu-0.1.30/src/ragu/ingest/ingest_template.py
--rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ingest/ingest_uaf_kentech.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.571337 ragu-0.1.30/src/ragu/nav/
--rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/nav/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/nav/gps.py
--rw-r--r--   0 btober     (501) staff       (20)    21336 2024-03-29 14:58:23.000000 ragu-0.1.30/src/ragu/nav/navparse.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.572252 ragu-0.1.30/src/ragu/radar/
--rw-r--r--   0 btober     (501) staff       (20)     7657 2024-03-29 15:06:16.000000 ragu-0.1.30/src/ragu/radar/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/radar/flags.py
--rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/radar/pick.py
--rw-r--r--   0 btober     (501) staff       (20)    14075 2024-04-19 16:27:32.000000 ragu-0.1.30/src/ragu/radar/processing.py
--rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/raguError.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.577005 ragu-0.1.30/src/ragu/recs/
--rw-r--r--   0 btober     (501) staff       (20)  1079564 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/recs/20190928-235534_compiled.jpg
--rw-r--r--   0 btober     (501) staff       (20)    16176 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/recs/basemap_icon.png
--rw-r--r--   0 btober     (501) staff       (20)    92542 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/recs/bulb.jpg
--rw-r--r--   0 btober     (501) staff       (20)    21590 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/recs/ragu_logo.png
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.577777 ragu-0.1.30/src/ragu/tools/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/tools/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/tools/constants.py
--rw-r--r--   0 btober     (501) staff       (20)     9427 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/tools/export.py
--rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/tools/utils.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.579275 ragu-0.1.30/src/ragu/ui/
--rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ui/__init__.py
--rw-r--r--   0 btober     (501) staff       (20)    16621 2024-02-24 23:44:42.000000 ragu-0.1.30/src/ragu/ui/basemap.py
--rw-r--r--   0 btober     (501) staff       (20)    68791 2024-04-19 16:28:48.000000 ragu-0.1.30/src/ragu/ui/gui.py
--rw-r--r--   0 btober     (501) staff       (20)    70973 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ui/impick.py
--rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ui/notepad.py
--rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.30/src/ragu/ui/wvpick.py
-drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-19 16:36:20.525744 ragu-0.1.30/src/ragu.egg-info/
--rw-r--r--   0 btober     (501) staff       (20)    47233 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/PKG-INFO
--rw-r--r--   0 btober     (501) staff       (20)     1369 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/SOURCES.txt
--rw-r--r--   0 btober     (501) staff       (20)        1 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/dependency_links.txt
--rw-r--r--   0 btober     (501) staff       (20)       44 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/entry_points.txt
--rw-r--r--   0 btober     (501) staff       (20)       64 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/requires.txt
--rw-r--r--   0 btober     (501) staff       (20)       10 2024-04-19 16:36:20.000000 ragu-0.1.30/src/ragu.egg-info/top_level.txt
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.641100 ragu-0.1.31/
+-rw-r--r--   0 btober     (501) staff       (20)    35149 2023-07-08 00:09:50.000000 ragu-0.1.31/LICENSE.txt
+-rw-r--r--   0 btober     (501) staff       (20)    47505 2024-04-23 21:25:59.640848 ragu-0.1.31/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     6295 2024-04-19 17:28:40.000000 ragu-0.1.31/README.md
+-rw-r--r--   0 btober     (501) staff       (20)      942 2024-04-23 21:25:07.000000 ragu-0.1.31/pyproject.toml
+-rw-r--r--   0 btober     (501) staff       (20)       38 2024-04-23 21:25:59.641133 ragu-0.1.31/setup.cfg
+-rw-r--r--   0 btober     (501) staff       (20)       91 2023-07-08 14:00:18.000000 ragu-0.1.31/setup.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.612553 ragu-0.1.31/src/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.613818 ragu-0.1.31/src/ragu/
+-rw-r--r--   0 btober     (501) staff       (20)        0 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/__init__.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.614678 ragu-0.1.31/src/ragu/bin/
+-rw-r--r--   0 btober     (501) staff       (20)     2574 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/bin/ragu.py
+-rw-r--r--   0 btober     (501) staff       (20)     1993 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/config.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.612711 ragu-0.1.31/src/ragu/dat/
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.614804 ragu-0.1.31/src/ragu/dat/mars/
+-rw-r--r--   0 btober     (501) staff       (20) 33196562 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/dat/mars/mega90n000eb.tif
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.634570 ragu-0.1.31/src/ragu/ingest/
+-rw-r--r--   0 btober     (501) staff       (20)     5750 2024-04-19 16:57:42.000000 ragu-0.1.31/src/ragu/ingest/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     2411 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_cresis_rds.py
+-rw-r--r--   0 btober     (501) staff       (20)     2454 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_cresis_snow.py
+-rw-r--r--   0 btober     (501) staff       (20)     3123 2024-04-23 21:24:25.000000 ragu-0.1.31/src/ragu/ingest/ingest_groundhog.py
+-rw-r--r--   0 btober     (501) staff       (20)     3366 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_gssi.py
+-rw-r--r--   0 btober     (501) staff       (20)     2562 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_lrs.py
+-rw-r--r--   0 btober     (501) staff       (20)     2896 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_marsis.py
+-rw-r--r--   0 btober     (501) staff       (20)     2474 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_marsis_ipc.py
+-rw-r--r--   0 btober     (501) staff       (20)     5780 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_oibAK.py
+-rw-r--r--   0 btober     (501) staff       (20)    14181 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_pulseekko.py
+-rw-r--r--   0 btober     (501) staff       (20)     2537 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_rimfax.py
+-rw-r--r--   0 btober     (501) staff       (20)     2931 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_sharad.py
+-rw-r--r--   0 btober     (501) staff       (20)     3640 2024-04-19 16:41:20.000000 ragu-0.1.31/src/ragu/ingest/ingest_template.py
+-rw-r--r--   0 btober     (501) staff       (20)     2444 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/ingest/ingest_uaf_kentech.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.634911 ragu-0.1.31/src/ragu/nav/
+-rw-r--r--   0 btober     (501) staff       (20)      153 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/nav/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)     5086 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/nav/gps.py
+-rw-r--r--   0 btober     (501) staff       (20)    21420 2024-04-22 00:33:24.000000 ragu-0.1.31/src/ragu/nav/navparse.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.636890 ragu-0.1.31/src/ragu/radar/
+-rw-r--r--   0 btober     (501) staff       (20)     7814 2024-04-23 21:24:56.000000 ragu-0.1.31/src/ragu/radar/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      505 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/radar/flags.py
+-rw-r--r--   0 btober     (501) staff       (20)     1185 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/radar/pick.py
+-rw-r--r--   0 btober     (501) staff       (20)    14029 2024-04-19 16:55:41.000000 ragu-0.1.31/src/ragu/radar/processing.py
+-rw-r--r--   0 btober     (501) staff       (20)      225 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/raguError.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.639328 ragu-0.1.31/src/ragu/recs/
+-rw-r--r--   0 btober     (501) staff       (20)  1079564 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/recs/20190928-235534_compiled.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    16176 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/recs/basemap_icon.png
+-rw-r--r--   0 btober     (501) staff       (20)    92542 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/recs/bulb.jpg
+-rw-r--r--   0 btober     (501) staff       (20)    21590 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/recs/ragu_logo.png
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.639809 ragu-0.1.31/src/ragu/tools/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/tools/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)      481 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/tools/constants.py
+-rw-r--r--   0 btober     (501) staff       (20)     9245 2024-04-19 16:56:13.000000 ragu-0.1.31/src/ragu/tools/export.py
+-rw-r--r--   0 btober     (501) staff       (20)     9845 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/tools/utils.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.640520 ragu-0.1.31/src/ragu/ui/
+-rw-r--r--   0 btober     (501) staff       (20)      152 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/ui/__init__.py
+-rw-r--r--   0 btober     (501) staff       (20)    16621 2024-02-24 23:44:42.000000 ragu-0.1.31/src/ragu/ui/basemap.py
+-rw-r--r--   0 btober     (501) staff       (20)    68791 2024-04-19 16:46:29.000000 ragu-0.1.31/src/ragu/ui/gui.py
+-rw-r--r--   0 btober     (501) staff       (20)    71060 2024-04-23 21:19:13.000000 ragu-0.1.31/src/ragu/ui/impick.py
+-rw-r--r--   0 btober     (501) staff       (20)    10803 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/ui/notepad.py
+-rw-r--r--   0 btober     (501) staff       (20)    23544 2023-07-08 00:09:51.000000 ragu-0.1.31/src/ragu/ui/wvpick.py
+drwxr-xr-x   0 btober     (501) staff       (20)        0 2024-04-23 21:25:59.614524 ragu-0.1.31/src/ragu.egg-info/
+-rw-r--r--   0 btober     (501) staff       (20)    47505 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/PKG-INFO
+-rw-r--r--   0 btober     (501) staff       (20)     1369 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/SOURCES.txt
+-rw-r--r--   0 btober     (501) staff       (20)        1 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/dependency_links.txt
+-rw-r--r--   0 btober     (501) staff       (20)       44 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/entry_points.txt
+-rw-r--r--   0 btober     (501) staff       (20)       64 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/requires.txt
+-rw-r--r--   0 btober     (501) staff       (20)       10 2024-04-23 21:25:59.000000 ragu-0.1.31/src/ragu.egg-info/top_level.txt
```

### Comparing `ragu-0.1.30/LICENSE.txt` & `ragu-0.1.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/PKG-INFO` & `ragu-0.1.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.30
+Version: 0.1.31
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -747,20 +747,17 @@
   <img src="https://github.com/btobers/RAGU/raw/master/src/ragu/recs/20190928-235534_compiled.jpg" height="500"><br>
 </p>
 
 #### Processing Script:
 A file log/processing script may also be exported to keep track of and easily repeat any data processing steps. Example processing script:
 ```
 ### RAGU processing log ###
-import sys
-# change dir to RAGU code directory
-sys.path.append('/home/user/code/RAGU/code')
-from ingest import ingest
+from ragu import ingest
 
-igst = ingest("/home/user/data/ARES/20140524-200130.h5")
+igst = ingest.ingest("/home/user/data/ARES/20140524-200130.h5")
 rdata = igst.read("","+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs","earth")
 rdata.lowpass(order=5, cf=1250000.0)
 rdata.tpowGain(power=1.2)
 ```
 
 ## Running RAGU
 
@@ -778,28 +775,40 @@
 - pandas
 - geopandas
 - pyproj
 - rasterio
 - h5py
 
 ### Setup
-**Nonte: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
+**Note: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
 
 1. Install ragu via [PyPi](https://pypi.org/project/ragu/)
 
 ```
-$ pip install ragu
+pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
-$ ragu
+ragu
 ```
 **Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/raw/master/src/docs/config.ini).
 
+#### Development
+If you are interested in helping to develop RAGU, we recommend forking [RAGU's github repository](https://github.com/btobers/RAGU) and then [cloning the github repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) onto your local machine.
+
+Note, if RAGU was already installed via PyPI, first uninstall:
+```
+pip uninstall ragu
+````
+
+You can then use pip to install your locally cloned fork of RAGU in 'editable' mode to easily facilitate development like so:
+```
+pip install -e /path/to/your/RAGU/clone
+```
 
 ## Notes
 Several auxiliary tools which RAGU users may find useful can be found at [radar_tools](https://github.com/btobers/radar_tools)
 
 ### Future Development
 Additional dataset ingesters:
 - Segy
@@ -813,18 +822,13 @@
 - depth conversion
 - dielectric extraction
 - pick amplitude tracking
 
 General:
 pyproj.transform is deprecated going from pyproj v1 to v2. Ragu.nav.navparse needs to be updated accordingly.
 
-### Collaboration
-
-Interested in contributing in the development of RAGU, or if you would like to use RAGU for interpreting a radar dataset that is not currently supported - Reach out to tobers.brandon@gmail.com
-
-
 ### Publications
 
 A list of publications that cite RAGU:
 
 1. Loso, Michael G., Christopher F. Larsen, Brandon S. Tober, Michael Christoffersen, Mark Fahnestock, John W. Holt, and Martin Truffer. “Quo Vadis, Alsek? Climate-Driven Glacier Retreat May Change the Course of a Major River Outlet in Southern Alaska.” Geomorphology 384 (July 1, 2021): 107701. https://doi.org/10.1016/j.geomorph.2021.107701.
 2. Tober, B. S., J. W. Holt, M. S. Christoffersen, M. Truffer, C. F. Larsen, D. J. Brinkerhoff, and S. A. Mooneyham. “Comprehensive Radar Mapping of Malaspina Glacier (Sít’ Tlein), Alaska—The World’s Largest Piedmont Glacier—Reveals Potential for Instability.” Journal of Geophysical Research: Earth Surface 128, no. 3 (2023): e2022JF006898. https://doi.org/10.1029/2022JF006898.
```

### Comparing `ragu-0.1.30/README.md` & `ragu-0.1.31/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,20 +51,17 @@
   <img src="https://github.com/btobers/RAGU/raw/master/src/ragu/recs/20190928-235534_compiled.jpg" height="500"><br>
 </p>
 
 #### Processing Script:
 A file log/processing script may also be exported to keep track of and easily repeat any data processing steps. Example processing script:
 ```
 ### RAGU processing log ###
-import sys
-# change dir to RAGU code directory
-sys.path.append('/home/user/code/RAGU/code')
-from ingest import ingest
+from ragu import ingest
 
-igst = ingest("/home/user/data/ARES/20140524-200130.h5")
+igst = ingest.ingest("/home/user/data/ARES/20140524-200130.h5")
 rdata = igst.read("","+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs","earth")
 rdata.lowpass(order=5, cf=1250000.0)
 rdata.tpowGain(power=1.2)
 ```
 
 ## Running RAGU
 
@@ -82,28 +79,40 @@
 - pandas
 - geopandas
 - pyproj
 - rasterio
 - h5py
 
 ### Setup
-**Nonte: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
+**Note: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
 
 1. Install ragu via [PyPi](https://pypi.org/project/ragu/)
 
 ```
-$ pip install ragu
+pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
-$ ragu
+ragu
 ```
 **Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/raw/master/src/docs/config.ini).
 
+#### Development
+If you are interested in helping to develop RAGU, we recommend forking [RAGU's github repository](https://github.com/btobers/RAGU) and then [cloning the github repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) onto your local machine.
+
+Note, if RAGU was already installed via PyPI, first uninstall:
+```
+pip uninstall ragu
+````
+
+You can then use pip to install your locally cloned fork of RAGU in 'editable' mode to easily facilitate development like so:
+```
+pip install -e /path/to/your/RAGU/clone
+```
 
 ## Notes
 Several auxiliary tools which RAGU users may find useful can be found at [radar_tools](https://github.com/btobers/radar_tools)
 
 ### Future Development
 Additional dataset ingesters:
 - Segy
@@ -117,18 +126,13 @@
 - depth conversion
 - dielectric extraction
 - pick amplitude tracking
 
 General:
 pyproj.transform is deprecated going from pyproj v1 to v2. Ragu.nav.navparse needs to be updated accordingly.
 
-### Collaboration
-
-Interested in contributing in the development of RAGU, or if you would like to use RAGU for interpreting a radar dataset that is not currently supported - Reach out to tobers.brandon@gmail.com
-
-
 ### Publications
 
 A list of publications that cite RAGU:
 
 1. Loso, Michael G., Christopher F. Larsen, Brandon S. Tober, Michael Christoffersen, Mark Fahnestock, John W. Holt, and Martin Truffer. “Quo Vadis, Alsek? Climate-Driven Glacier Retreat May Change the Course of a Major River Outlet in Southern Alaska.” Geomorphology 384 (July 1, 2021): 107701. https://doi.org/10.1016/j.geomorph.2021.107701.
-2. Tober, B. S., J. W. Holt, M. S. Christoffersen, M. Truffer, C. F. Larsen, D. J. Brinkerhoff, and S. A. Mooneyham. “Comprehensive Radar Mapping of Malaspina Glacier (Sít’ Tlein), Alaska—The World’s Largest Piedmont Glacier—Reveals Potential for Instability.” Journal of Geophysical Research: Earth Surface 128, no. 3 (2023): e2022JF006898. https://doi.org/10.1029/2022JF006898.
+2. Tober, B. S., J. W. Holt, M. S. Christoffersen, M. Truffer, C. F. Larsen, D. J. Brinkerhoff, and S. A. Mooneyham. “Comprehensive Radar Mapping of Malaspina Glacier (Sít’ Tlein), Alaska—The World’s Largest Piedmont Glacier—Reveals Potential for Instability.” Journal of Geophysical Research: Earth Surface 128, no. 3 (2023): e2022JF006898. https://doi.org/10.1029/2022JF006898.
```

### Comparing `ragu-0.1.30/pyproject.toml` & `ragu-0.1.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ragu"
-version = "0.1.30"
+version = "0.1.31"
 description = "Radar Analysis Graphical Utility (RAGU)"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE.txt"}
 authors = [
      {name = "Brandon Tober", email = "tobers.brandon@gmail.com"},
      {name = "Michael Christoffersen", email = "mchristo28@gmail.com"},
```

### Comparing `ragu-0.1.30/src/ragu/bin/ragu.py` & `ragu-0.1.31/src/ragu/bin/ragu.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/config.py` & `ragu-0.1.31/src/ragu/config.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/dat/mars/mega90n000eb.tif` & `ragu-0.1.31/src/ragu/dat/mars/mega90n000eb.tif`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/__init__.py` & `ragu-0.1.31/src/ragu/ingest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
             print("File reader for format {} not built yet".format(self.ftype))
             exit(1)
 
         print("----------------------------------------")
         print("Loaded: " + self.rdata.fn)
 
         # add ingest commands to log
-        self.rdata.log('self.igst = ingest("{}")'.format(self.fpath))
-        self.rdata.log('self.rdata = igst.read("{}","{}","{}")'.format(simpath,navcrs,body))
+        self.rdata.log('igst = ingest.ingest("{}")'.format(self.fpath))
+        self.rdata.log('rdata = igst.read("{}","{}","{}")'.format(simpath,navcrs,body))
 
         return self.rdata
 
 
     # import_pick is a method of the ingester class which loads in existing picks from a text file
     def import_pick(self, fpath, uid):
         if fpath.endswith("csv"):
```

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_cresis_rds.py` & `ragu-0.1.31/src/ragu/ingest/ingest_cresis_rds.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_cresis_snow.py` & `ragu-0.1.31/src/ragu/ingest/ingest_cresis_snow.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_groundhog.py` & `ragu-0.1.31/src/ragu/ingest/ingest_groundhog.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,69 +21,75 @@
     rdata = garlic(fpath)
     rdata.fn = fpath.split("/")[-1][:-3]
     rdata.dtype = "groundhog"
 
     # read in .h5 file
     f = h5py.File(rdata.fpath, "r")                      
 
-    # groundhog h5 radar data group structure        
-    # |-raw
-    # |  |-rx0
-    # |  |-gps0
-    # |  |-rxFix0    
-    # |  |-txFix0
-
     # pull necessary raw group data
-    rdata.fs = f["raw"].attrs["fs"]                                         # sampling frequency
-    rdata.dt = 1/rdata.fs                                                   # sampling interval, sec
-    rdata.prf = f["raw"].attrs["prf"]                                       # pulse repition frequency, Hz
+    rdata.fs = f["raw/rx0"].attrs["fs"]                             # sampling frequency
+    rdata.dt = 1/rdata.fs
+    try:                                                            # sampling interval, sec
+        rdata.prf = f["raw/rx0"].attrs["prf"]                       # pulse repition frequency, Hz
+    except KeyError:
+        rdata.prf = 0
     rdata.nchan = 1
 
     # pull radar proc and sim arrayss
-    rdata.set_dat(f["raw/rx0"][:].astype(float))                                          # pulse compressed array
-    rdata.set_proc(np.abs(rdata.get_dat()))
+    if("restack" in f.keys()):
+        rdata.set_dat(f["restack/rx0"][:].astype(float))
+    else:
+        rdata.set_dat(f["raw/rx0"][:].astype(float))
+
+    # want to plot positive and negative amplitude values - don't dB 
+    rdata.dbit = False
+    rdata.set_proc(rdata.get_dat())
     rdata.snum, rdata.tnum = rdata.get_dat().shape
 
     rdata.set_twtt()
 
     # parse nav
     rdata.geocrs = navcrs
     rdata.xyzcrs = navparse.xyzsys[body]
     rdata.navdf = navparse.getnav_groundhog(fpath, navcrs, body)
 
     # if rx and tx each have gps, we'll store antenna sep per trace
     if "asep" in rdata.navdf:
         rdata.asep = rdata.navdf["asep"].to_numpy()
     else:
-        rdata.asep = 100
+        rdata.asep = 50
 
     # groudnhog rx triggers on arrival of airwave - get number of traces pre-trigger to vertically shift the data accordingly
-    pt = f["raw"].attrs["pre_trig"]
+    try:
+        pt = f["raw/rx0"].attrs["pre_trig"]
+    except KeyError:
+        pt = f["raw/rx0"].attrs["pre_trigger"]
+
     rdata.flags.sampzero = pt+1
     rdata.tzero_shift()
 
     # define surface horizon name to set index to zeros
     rdata.pick.horizons["srf"] = np.zeros(rdata.tnum)
     rdata.pick.set_srf("srf")
 
     # srf_elev is the same as GPS recorded elev
     rdata.set_srfElev(dat = rdata.navdf["elev"].to_numpy())
 
     rdata.info["Signal Type"] = "Impulse" 
     rdata.info["Sampling Frequency [MHz]"] = rdata.fs * 1e-6
     rdata.info["PRF [kHz]"] = rdata.prf * 1e-3
-    rdata.info["Stack"] = f["raw"].attrs["stack"]
+    rdata.info["Stack"] = f["raw/rx0"].attrs["stack"]
     rdata.info["Antenna Separation [m]"] = round(np.nanmean(rdata.asep))
 
     f.close()                                                   # close the file
 
     rdata.check_attrs()
 
     # try:
-    #     rdata.filter(btype='lowpass', lowcut=None, highcut=4e6, order=5, direction=0)
+    #     rdata.filter(btype='lowpass', lowcut=None, highcut=3e6, order=5, direction=0)
     # except:
     #     pass
     # try:
     #     rdata.filter(btype='lowpass', lowcut=None, highcut=.4, order=5, direction=1)
     # except:
     #     pass
```

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_gssi.py` & `ragu-0.1.31/src/ragu/ingest/ingest_gssi.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_lrs.py` & `ragu-0.1.31/src/ragu/ingest/ingest_lrs.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_marsis.py` & `ragu-0.1.31/src/ragu/ingest/ingest_marsis.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_marsis_ipc.py` & `ragu-0.1.31/src/ragu/ingest/ingest_marsis_ipc.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_oibAK.py` & `ragu-0.1.31/src/ragu/ingest/ingest_oibAK.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_pulseekko.py` & `ragu-0.1.31/src/ragu/ingest/ingest_pulseekko.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_rimfax.py` & `ragu-0.1.31/src/ragu/ingest/ingest_rimfax.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_sharad.py` & `ragu-0.1.31/src/ragu/ingest/ingest_sharad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_template.py` & `ragu-0.1.31/src/ragu/ingest/ingest_template.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ingest/ingest_uaf_kentech.py` & `ragu-0.1.31/src/ragu/ingest/ingest_uaf_kentech.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/nav/gps.py` & `ragu-0.1.31/src/ragu/nav/gps.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/nav/navparse.py` & `ragu-0.1.31/src/ragu/nav/navparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,18 @@
             nav_tx["lon"].to_numpy(),
             nav_tx["lat"].to_numpy(),
             nav_tx["hgt"].to_numpy(),
         )
         df["asep"] = np.sqrt((rx_df['x']-tx_df['x'])**2 + (rx_df['y']-tx_df['y'])**2 + (rx_df['z']-tx_df['z'])**2)
 
     elif "rxFix0" in k:
-        df = pd.DataFrame(h5[grp]["rxFix0"][:])        
+        df = pd.DataFrame(h5[grp]["rxFix0"][:])
+    elif "ppp0" in k:
+        df = pd.DataFrame(h5[grp]["ppp0"][:])
+        df["asep"] = 50
     else:
         df = pd.DataFrame(h5[grp]["gps0"][:])
         df["asep"] = 50
     
     try:
         df.rename(columns={"hgt": "elev"}, inplace=True)
     except:
```

### Comparing `ragu-0.1.30/src/ragu/radar/__init__.py` & `ragu-0.1.31/src/ragu/radar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
         self.sPyramid = None
         #: radar flags object
         self.flags = flags()
         # geographic crs string
         self.geocrs = None
         # xyz crs string
         self.xyzcrs = None
+        # bool: store data as power in decibels
+        self.dbit = True
 
         # per-trace attributes
         #: navigation dataframe consisting of [lon, lat, hgt, x, y, z, dist], where each field is of type and size np.ndarray(tnum,)
         self.navdf = None
     
         # sample-wise attributes
         #: np.ndarray(snum,) The two way travel time to each sample, in us
@@ -166,21 +168,24 @@
     def set_out(self, dat):
         self.out = dat
         return
 
 
     # convert amplitude array to dB log scale
     def dBscale(self, dat):
-        # convert to power
-        pow = np.power(dat.astype(float), 2)
-        # mask zero-power values
-        pow[pow == 0] = np.nan
-        # dB it
-        dB = 10*np.log10(pow)
-        return dB
+        if self.dbit:
+            # convert to power
+            pow = np.power(dat.astype(float), 2)
+            # mask zero-power values
+            pow[pow == 0] = np.nan
+            # dB it
+            out = 10*np.log10(pow)
+        else:
+            out = dat
+        return out
 
 
     def genPyramids(self, dat):
         # downsample in fast time by 2^0, 2^1, 2^2, 2^3
         pyramid = []
         # add pyramid arrays to list
         if (self.dtype == "oibak") or (self.dtype == "cresis_snow") or (self.dtype == "cresis_rds"):
```

### Comparing `ragu-0.1.30/src/ragu/radar/pick.py` & `ragu-0.1.31/src/ragu/radar/pick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/radar/processing.py` & `ragu-0.1.31/src/ragu/radar/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         self.flags.sampzero = np.nanmean(utils.get_srf(np.abs(self.dat), "Impulse")).astype(int)
 
     if self.flags.sampzero > 0:
         self.tzero_shift()
         # log
         out = '# Time zero shifted to:\n# sample:\t {}\n# time:\t\t {} nanoseconds'\
         .format(self.flags.sampzero,(self.flags.sampzero * self.dt * 1e9))
-        self.log("self.rdata.set_tzero()" + "\n" + out)
+        self.log("rdata.set_tzero()" + "\n" + out)
         print(out)
 
     return
 
 
 def tzero_shift(self):
     # shift 2d proc data array so first row is time zero sample - use nan to fill bottom samples
@@ -99,15 +99,15 @@
     self.navdf.dist = navparse.euclid_dist(self.navdf.x.to_numpy(), self.navdf.y.to_numpy(), self.navdf.z.to_numpy())
 
     # reverse picks
     for h in self.pick.horizons.keys():
         self.pick.horizons[h] = np.flip(self.pick.horizons[h])
 
     # log
-    self.log("self.rdata.rgram_reverse()")
+    self.log("rdata.rgram_reverse()")
     print("# radargram reversed, to undo simply repeat reverse operation")
 
     return
 
 def flatten(self):
     # flatten radargram by rolling each trace so that the surface is at sample zero
     amp = self.proc.get_curr_amp()
@@ -120,30 +120,30 @@
     # loop through all traces and roll according to surface sample
     for i, col in enumerate(amp.T):
         out[i] = np.roll(col, shift = -self.flags.sampzero[i])
 
     self.set_proc(out.T)
 
     # log
-    self.log("self.rdata.flatten()")
+    self.log("rdata.flatten()")
     print("# data array flattened ")
 
     return
 
 
 def vertical_roll(self, samples=0):
     # roll 2d proc data array vertically to fix mismatch
     amp = self.proc.get_curr_amp()
     self.proc.set_prev_amp(amp)
     self.proc.set_prev_dB(self.proc.get_curr_dB())
     out = np.roll(amp, shift=samples, axis=0)
     self.set_proc(out)
 
     # log
-    self.log("self.rdata.vertical_roll(samples={})".format(samples))
+    self.log("rdata.vertical_roll(samples={})".format(samples))
     print("# data array rolled by {} samples".format(samples))
 
     return
 
 
 def removeSlidingMeanFFT(self, window):
     # background noise removal using sliding mean in frequency space
@@ -177,15 +177,15 @@
 
     for i in range(amp.shape[1] - window // 2, amp.shape[1]):
         mean[:, i] = mt
 
     out = np.subtract(amp, mean)
     self.set_proc(out)
     # log
-    self.log("self.rdata.removeSlidingMeanFFT(window={})".format(window))
+    self.log("rdata.removeSlidingMeanFFT(window={})".format(window))
     print("# Background removal completed wtih a window size of {} traces".format(window))
 
     return 
 
 
 def butter(btype="lowpass", lowcut=None, highcut=None, fs=None, order=5):
     nyq = 0.5 * fs
@@ -209,15 +209,15 @@
     amp = self.proc.get_curr_amp()
     self.proc.set_prev_amp(amp)
     self.proc.set_prev_dB(self.proc.get_curr_dB())
     analytic_signal = signal.hilbert(amp, axis=0)
     amplitude_envelope = np.abs(analytic_signal)
     self.set_proc(amplitude_envelope)
     # log
-    self.log("self.rdata.hilbertxform()")
+    self.log("rdata.hilbertxform()")
     print("# hilbert transform applied applied")
 
     return 
 
 
 def filter(self, btype="lowpass", lowcut=None, highcut=None, order=5, direction=0):
     # apply low pass filter to data array
@@ -239,15 +239,15 @@
     out = signal.filtfilt(b, a, amp, axis=direction)
     out[idx] = np.nan
     # out[:-self.flags.sampzero,:] = signal.filtfilt(b, a, np.abs(amp[:-self.flags.sampzero:,:]), axis=direction)
     # out[-self.flags.sampzero:,:] = np.nan
     # use amplitude of lp filtered data to reset as pc array
     self.set_proc(out)
     # log
-    self.log("self.rdata.filter(btype='{}', lowcut={}, highcut={}, order={}, direction={})".format(btype, lowcut, highcut, order, direction))
+    self.log("rdata.filter(btype='{}', lowcut={}, highcut={}, order={}, direction={})".format(btype, lowcut, highcut, order, direction))
     print("# filter applied: btype='{}', lowcut={}, highcut={}, order={}, direction={}".format(btype, lowcut, highcut, order, direction))
 
     return
 
 
 def restack(self, intrvl=None,thold=None):
     # get coordinate transformation
@@ -307,32 +307,31 @@
         self.navdf["twtt_wind"] = 0.0
     else:
         self.navdf["twtt_wind"] = np.nan
 
     self.snum, self.tnum = rstack.shape
     self.set_proc(rstack)
     # log
-    self.log("self.rdata.restack(intrvl={},thold={})".format(intrvl,thold))
+    self.log("rdata.restack(intrvl={},thold={})".format(intrvl,thold))
     print("# data restacked at an interval of {} m, with a minimum distance threshold of {} m".format(intrvl,thold))
     
     return
 
-
 def tpowGain(self, power):
     # t-power gain to each trace with the given exponent.
     amp = self.proc.get_curr_amp()
     self.proc.set_prev_amp(amp)
     self.proc.set_prev_dB(self.proc.get_curr_dB())
     twtt = np.arange(self.snum)*self.dt
     factor = np.reshape(twtt**(float(power)),(len(twtt),1))
     factmat = np.matlib.repmat(factor,1,self.tnum)
     out = np.multiply(amp,factmat)
     self.set_proc(out)
     # log
-    self.log("self.rdata.tpowGain(power={})".format(power))
+    self.log("rdata.tpowGain(power={})".format(power))
     print("# time^{} gain applied".format(power))
 
     return
 
 
 def undo(self):
     # undo last processing step
```

### Comparing `ragu-0.1.30/src/ragu/recs/20190928-235534_compiled.jpg` & `ragu-0.1.31/src/ragu/recs/20190928-235534_compiled.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/recs/basemap_icon.png` & `ragu-0.1.31/src/ragu/recs/basemap_icon.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/recs/bulb.jpg` & `ragu-0.1.31/src/ragu/recs/bulb.jpg`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/recs/ragu_logo.png` & `ragu-0.1.31/src/ragu/recs/ragu_logo.png`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/tools/export.py` & `ragu-0.1.31/src/ragu/tools/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,12 +201,11 @@
     np.savetxt(fpath, dat, fmt="%s", delimiter=",")
     print("data exported successfully:\t" + fpath)
 
 
 # log is a method to export the processing log as a python script
 def log(fpath, log):
     with open(fpath,"w") as ofile:
-        cdir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        ofile.write("### RAGU processing log ###\nimport sys\n# change dir to RAGU code directory\nsys.path.append('{}')\nfrom ingest import ingest\n\n".format(cdir))
+        ofile.write("### RAGU processing log ###\nfrom ragu import ingest\n\n")
         for _i in log:
-            ofile.write(_i.replace("self.","") + "\n")
+            ofile.write(_i + "\n")
         ofile.close()
```

### Comparing `ragu-0.1.30/src/ragu/tools/utils.py` & `ragu-0.1.31/src/ragu/tools/utils.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ui/basemap.py` & `ragu-0.1.31/src/ragu/ui/basemap.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ui/gui.py` & `ragu-0.1.31/src/ragu/ui/gui.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ui/impick.py` & `ragu-0.1.31/src/ragu/ui/impick.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,16 +308,17 @@
         # set color range
         self.set_crange()
 
 
     # set radar and sim array bounds for setting image color limits - just doing this once based off original arrays, not pyramids
     def set_crange(self):
         # get clim bounds - take 10th percentile for min, ignore nd values
-        self.mindB_data = np.floor(np.nanpercentile(self.rdata.proc.get_curr_dB(),10))
-        self.maxdB_data = np.nanmax(self.rdata.proc.get_curr_dB())
+        self.mindB_data = np.floor(np.nanpercentile(self.rdata.proc.get_curr_dB(),1))
+        self.maxdB_data = np.ceil(np.nanpercentile(self.rdata.proc.get_curr_dB(),99))
+        # self.maxdB_data = np.nanmax(self.rdata.proc.get_curr_dB())
 
         if self.rdata.flags.sim:
             self.mindB_sim = np.floor(np.nanpercentile(self.rdata.sim,10))
             self.maxdB_sim = np.nanmax(self.rdata.sim)
             self.sim_crange = self.maxdB_sim - self.mindB_sim
             self.im_sim.set_clim([self.mindB_sim, self.maxdB_sim])
```

### Comparing `ragu-0.1.30/src/ragu/ui/notepad.py` & `ragu-0.1.31/src/ragu/ui/notepad.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu/ui/wvpick.py` & `ragu-0.1.31/src/ragu/ui/wvpick.py`

 * *Files identical despite different names*

### Comparing `ragu-0.1.30/src/ragu.egg-info/PKG-INFO` & `ragu-0.1.31/src/ragu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragu
-Version: 0.1.30
+Version: 0.1.31
 Summary: Radar Analysis Graphical Utility (RAGU)
 Author-email: Brandon Tober <tobers.brandon@gmail.com>, Michael Christoffersen <mchristo28@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -747,20 +747,17 @@
   <img src="https://github.com/btobers/RAGU/raw/master/src/ragu/recs/20190928-235534_compiled.jpg" height="500"><br>
 </p>
 
 #### Processing Script:
 A file log/processing script may also be exported to keep track of and easily repeat any data processing steps. Example processing script:
 ```
 ### RAGU processing log ###
-import sys
-# change dir to RAGU code directory
-sys.path.append('/home/user/code/RAGU/code')
-from ingest import ingest
+from ragu import ingest
 
-igst = ingest("/home/user/data/ARES/20140524-200130.h5")
+igst = ingest.ingest("/home/user/data/ARES/20140524-200130.h5")
 rdata = igst.read("","+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs","earth")
 rdata.lowpass(order=5, cf=1250000.0)
 rdata.tpowGain(power=1.2)
 ```
 
 ## Running RAGU
 
@@ -778,28 +775,40 @@
 - pandas
 - geopandas
 - pyproj
 - rasterio
 - h5py
 
 ### Setup
-**Nonte: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
+**Note: Prior to installation, one may first wish to create an anaconda environment from which to install ragu**.
 
 1. Install ragu via [PyPi](https://pypi.org/project/ragu/)
 
 ```
-$ pip install ragu
+pip install ragu
 ```
 
 2. To run ragu, call ragu from the command line to initialize the GUI:
 ```
-$ ragu
+ragu
 ```
 **Nonte: The first time ragu is run on your machine, a configuration file will be created at *~/RAGU/config.ini*.** This configuration file can be edited to set appropriate data paths, data coordinate reference system, and output preferences. Path variables may be left blank, but must remain uncommented. An example ragu configuration file can be found [here](https://github.com/btobers/RAGU/raw/master/src/docs/config.ini).
 
+#### Development
+If you are interested in helping to develop RAGU, we recommend forking [RAGU's github repository](https://github.com/btobers/RAGU) and then [cloning the github repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) onto your local machine.
+
+Note, if RAGU was already installed via PyPI, first uninstall:
+```
+pip uninstall ragu
+````
+
+You can then use pip to install your locally cloned fork of RAGU in 'editable' mode to easily facilitate development like so:
+```
+pip install -e /path/to/your/RAGU/clone
+```
 
 ## Notes
 Several auxiliary tools which RAGU users may find useful can be found at [radar_tools](https://github.com/btobers/radar_tools)
 
 ### Future Development
 Additional dataset ingesters:
 - Segy
@@ -813,18 +822,13 @@
 - depth conversion
 - dielectric extraction
 - pick amplitude tracking
 
 General:
 pyproj.transform is deprecated going from pyproj v1 to v2. Ragu.nav.navparse needs to be updated accordingly.
 
-### Collaboration
-
-Interested in contributing in the development of RAGU, or if you would like to use RAGU for interpreting a radar dataset that is not currently supported - Reach out to tobers.brandon@gmail.com
-
-
 ### Publications
 
 A list of publications that cite RAGU:
 
 1. Loso, Michael G., Christopher F. Larsen, Brandon S. Tober, Michael Christoffersen, Mark Fahnestock, John W. Holt, and Martin Truffer. “Quo Vadis, Alsek? Climate-Driven Glacier Retreat May Change the Course of a Major River Outlet in Southern Alaska.” Geomorphology 384 (July 1, 2021): 107701. https://doi.org/10.1016/j.geomorph.2021.107701.
 2. Tober, B. S., J. W. Holt, M. S. Christoffersen, M. Truffer, C. F. Larsen, D. J. Brinkerhoff, and S. A. Mooneyham. “Comprehensive Radar Mapping of Malaspina Glacier (Sít’ Tlein), Alaska—The World’s Largest Piedmont Glacier—Reveals Potential for Instability.” Journal of Geophysical Research: Earth Surface 128, no. 3 (2023): e2022JF006898. https://doi.org/10.1029/2022JF006898.
```

### Comparing `ragu-0.1.30/src/ragu.egg-info/SOURCES.txt` & `ragu-0.1.31/src/ragu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

