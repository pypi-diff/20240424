# Comparing `tmp/autogenstudio-0.0.56rc2.tar.gz` & `tmp/autogenstudio-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogenstudio-0.0.56rc2.tar", last modified: Tue Apr 23 22:21:44 2024, max compression
+gzip compressed data, was "autogenstudio-0.0.9a0.tar", last modified: Wed Dec  6 21:25:08 2023, max compression
```

## Comparing `autogenstudio-0.0.56rc2.tar` & `autogenstudio-0.0.9a0.tar`

### file list

```diff
@@ -1,105 +1,35 @@
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.882222 autogenstudio-0.0.56rc2/
--rw-r--r--   0 victordibia   (501) staff       (20)      361 2024-04-17 23:09:07.000000 autogenstudio-0.0.56rc2/.gitignore
--rw-r--r--   0 victordibia   (501) staff       (20)      421 2024-03-21 23:47:34.000000 autogenstudio-0.0.56rc2/Dockerfile
--rw-r--r--   0 victordibia   (501) staff       (20)      210 2024-03-19 16:11:36.000000 autogenstudio-0.0.56rc2/MANIFEST.in
--rw-r--r--   0 victordibia   (501) staff       (20)    12938 2024-04-23 22:21:44.881262 autogenstudio-0.0.56rc2/PKG-INFO
--rw-r--r--   0 victordibia   (501) staff       (20)    12008 2024-04-23 18:30:57.000000 autogenstudio-0.0.56rc2/README.md
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:42.072218 autogenstudio-0.0.56rc2/autogenstudio/
--rw-r--r--   0 victordibia   (501) staff       (20)      116 2024-04-17 21:37:11.000000 autogenstudio-0.0.56rc2/autogenstudio/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)     9484 2024-04-17 23:42:28.000000 autogenstudio-0.0.56rc2/autogenstudio/chatmanager.py
--rw-r--r--   0 victordibia   (501) staff       (20)     1734 2024-04-17 23:18:50.000000 autogenstudio-0.0.56rc2/autogenstudio/cli.py
--rw-r--r--   0 victordibia   (501) staff       (20)     9395 2024-04-18 04:21:09.000000 autogenstudio-0.0.56rc2/autogenstudio/datamodel.py
--rw-r--r--   0 victordibia   (501) staff       (20)    18422 2024-04-23 21:27:36.000000 autogenstudio-0.0.56rc2/autogenstudio/dbmanager.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:42.247066 autogenstudio-0.0.56rc2/autogenstudio/utils/
--rw-r--r--   0 victordibia   (501) staff       (20)       21 2024-04-17 23:11:03.000000 autogenstudio-0.0.56rc2/autogenstudio/utils/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)    24868 2024-04-17 19:14:33.000000 autogenstudio-0.0.56rc2/autogenstudio/utils/dbdefaults.json
--rw-r--r--   0 victordibia   (501) staff       (20)    17496 2024-04-23 18:57:27.000000 autogenstudio-0.0.56rc2/autogenstudio/utils/utils.py
--rw-r--r--   0 victordibia   (501) staff       (20)       71 2024-04-23 22:20:38.000000 autogenstudio-0.0.56rc2/autogenstudio/version.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:42.265368 autogenstudio-0.0.56rc2/autogenstudio/web/
--rw-r--r--   0 victordibia   (501) staff       (20)        0 2024-03-19 16:11:36.000000 autogenstudio-0.0.56rc2/autogenstudio/web/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)    13417 2024-04-23 21:25:49.000000 autogenstudio-0.0.56rc2/autogenstudio/web/app.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.240410 autogenstudio-0.0.56rc2/autogenstudio/web/ui/
--rw-r--r--   0 victordibia   (501) staff       (20)  1494844 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/318ce576f236b79fd96f75904c13f6e55c3eee57-f0efba87fdae2b725532.js
--rw-r--r--   0 victordibia   (501) staff       (20)     1173 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/318ce576f236b79fd96f75904c13f6e55c3eee57-f0efba87fdae2b725532.js.LICENSE.txt
--rw-r--r--   0 victordibia   (501) staff       (20)  5013995 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/318ce576f236b79fd96f75904c13f6e55c3eee57-f0efba87fdae2b725532.js.map
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.299462 autogenstudio-0.0.56rc2/autogenstudio/web/ui/404/
--rw-r--r--   0 victordibia   (501) staff       (20)    44116 2024-04-23 21:16:16.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/404/index.html
--rw-r--r--   0 victordibia   (501) staff       (20)    44120 2024-04-23 21:16:16.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/404.html
--rw-r--r--   0 victordibia   (501) staff       (20)   232598 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/app-b8234a0a29c4d22184ed.js
--rw-r--r--   0 victordibia   (501) staff       (20)      512 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/app-b8234a0a29c4d22184ed.js.LICENSE.txt
--rw-r--r--   0 victordibia   (501) staff       (20)   952112 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/app-b8234a0a29c4d22184ed.js.map
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.322560 autogenstudio-0.0.56rc2/autogenstudio/web/ui/build/
--rw-r--r--   0 victordibia   (501) staff       (20)    54133 2024-04-23 21:16:16.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/build/index.html
--rw-r--r--   0 victordibia   (501) staff       (20)      432 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/chunk-map.json
--rw-r--r--   0 victordibia   (501) staff       (20)      807 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/component---src-pages-404-tsx-9cfc00764f659a099247.js
--rw-r--r--   0 victordibia   (501) staff       (20)     2006 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/component---src-pages-404-tsx-9cfc00764f659a099247.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)   176871 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/component---src-pages-build-tsx-9223b5a8e35582cfcab4.js
--rw-r--r--   0 victordibia   (501) staff       (20)   655130 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/component---src-pages-build-tsx-9223b5a8e35582cfcab4.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)     4156 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/component---src-pages-gallery-index-tsx-120f318117531bdd081d.js
--rw-r--r--   0 victordibia   (501) staff       (20)    12739 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/component---src-pages-gallery-index-tsx-120f318117531bdd081d.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)    13894 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/component---src-pages-index-tsx-a4a2b11c89e33f346282.js
--rw-r--r--   0 victordibia   (501) staff       (20)    41358 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/component---src-pages-index-tsx-a4a2b11c89e33f346282.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)     1539 2024-04-23 21:13:24.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/favicon-32x32.png
--rw-r--r--   0 victordibia   (501) staff       (20)   140385 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/framework-3b041e76ed3d1ab0eeef.js
--rw-r--r--   0 victordibia   (501) staff       (20)      721 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/framework-3b041e76ed3d1ab0eeef.js.LICENSE.txt
--rw-r--r--   0 victordibia   (501) staff       (20)   355268 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/framework-3b041e76ed3d1ab0eeef.js.map
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.425045 autogenstudio-0.0.56rc2/autogenstudio/web/ui/gallery/
--rw-r--r--   0 victordibia   (501) staff       (20)    47709 2024-04-23 21:16:16.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/gallery/index.html
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.478554 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/
--rw-r--r--   0 victordibia   (501) staff       (20)     7211 2024-04-23 21:13:23.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/icon-144x144.png
--rw-r--r--   0 victordibia   (501) staff       (20)    10299 2024-04-23 21:13:24.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/icon-192x192.png
--rw-r--r--   0 victordibia   (501) staff       (20)    15443 2024-04-23 21:13:24.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/icon-256x256.png
--rw-r--r--   0 victordibia   (501) staff       (20)    26979 2024-04-23 21:13:24.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/icon-384x384.png
--rw-r--r--   0 victordibia   (501) staff       (20)     2296 2024-04-23 21:13:23.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/icon-48x48.png
--rw-r--r--   0 victordibia   (501) staff       (20)    39636 2024-04-23 21:13:24.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/icon-512x512.png
--rw-r--r--   0 victordibia   (501) staff       (20)     3358 2024-04-23 21:13:23.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/icon-72x72.png
--rw-r--r--   0 victordibia   (501) staff       (20)     4475 2024-04-23 21:13:23.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/icons/icon-96x96.png
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:41.865811 autogenstudio-0.0.56rc2/autogenstudio/web/ui/images/
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.480183 autogenstudio-0.0.56rc2/autogenstudio/web/ui/images/svgs/
--rw-r--r--   0 victordibia   (501) staff       (20)    10553 2024-04-23 21:16:05.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/images/svgs/welcome.svg
--rw-r--r--   0 victordibia   (501) staff       (20)    51780 2024-04-23 21:16:16.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/index.html
--rw-r--r--   0 victordibia   (501) staff       (20)      839 2024-04-23 21:13:24.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/manifest.webmanifest
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.525603 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.529433 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/404/
--rw-r--r--   0 victordibia   (501) staff       (20)      120 2024-04-23 21:16:05.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/404/page-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.532280 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/404.html/
--rw-r--r--   0 victordibia   (501) staff       (20)      124 2024-04-23 21:16:05.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/404.html/page-data.json
--rw-r--r--   0 victordibia   (501) staff       (20)       50 2024-04-23 21:16:05.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/app-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.536290 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/build/
--rw-r--r--   0 victordibia   (501) staff       (20)      230 2024-04-23 21:16:05.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/build/page-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.542122 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/gallery/
--rw-r--r--   0 victordibia   (501) staff       (20)      240 2024-04-23 21:16:05.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/gallery/page-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.546561 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/index/
--rw-r--r--   0 victordibia   (501) staff       (20)      224 2024-04-23 21:16:05.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/page-data/index/page-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.560560 autogenstudio-0.0.56rc2/autogenstudio/web/ui/sitemap/
--rw-r--r--   0 victordibia   (501) staff       (20)      627 2024-04-23 21:16:16.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/sitemap/sitemap-0.xml
--rw-r--r--   0 victordibia   (501) staff       (20)      187 2024-04-23 21:16:16.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/sitemap/sitemap-index.xml
--rw-r--r--   0 victordibia   (501) staff       (20)    39604 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/styles.8e0191eae5ed2105c413.css
--rw-r--r--   0 victordibia   (501) staff       (20)     3998 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/webpack-runtime-60e414b2ea07955f8932.js
--rw-r--r--   0 victordibia   (501) staff       (20)    18697 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/webpack-runtime-60e414b2ea07955f8932.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)     2543 2024-04-23 21:15:22.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/webpack.stats.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.770240 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.878666 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/debug/
--rw-r--r--   0 victordibia   (501) staff       (20)    28104 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/debug/partytown-atomics.js
--rw-r--r--   0 victordibia   (501) staff       (20)    17511 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/debug/partytown-media.js
--rw-r--r--   0 victordibia   (501) staff       (20)    27197 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/debug/partytown-sandbox-sw.js
--rw-r--r--   0 victordibia   (501) staff       (20)     1995 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/debug/partytown-sw.js
--rw-r--r--   0 victordibia   (501) staff       (20)    82089 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/debug/partytown-ww-atomics.js
--rw-r--r--   0 victordibia   (501) staff       (20)    81649 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/debug/partytown-ww-sw.js
--rw-r--r--   0 victordibia   (501) staff       (20)     3341 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/debug/partytown.js
--rw-r--r--   0 victordibia   (501) staff       (20)    28273 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/partytown-atomics.js
--rw-r--r--   0 victordibia   (501) staff       (20)     5689 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/partytown-media.js
--rw-r--r--   0 victordibia   (501) staff       (20)    29137 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/partytown-sw.js
--rw-r--r--   0 victordibia   (501) staff       (20)     1384 2024-04-23 21:13:15.000000 autogenstudio-0.0.56rc2/autogenstudio/web/ui/~partytown/partytown.js
--rw-r--r--   0 victordibia   (501) staff       (20)    10791 2024-04-18 18:15:41.000000 autogenstudio-0.0.56rc2/autogenstudio/workflowmanager.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-04-23 22:21:44.879995 autogenstudio-0.0.56rc2/autogenstudio.egg-info/
--rw-r--r--   0 victordibia   (501) staff       (20)    12938 2024-04-23 22:21:41.000000 autogenstudio-0.0.56rc2/autogenstudio.egg-info/PKG-INFO
--rw-r--r--   0 victordibia   (501) staff       (20)     3810 2024-04-23 22:21:41.000000 autogenstudio-0.0.56rc2/autogenstudio.egg-info/SOURCES.txt
--rw-r--r--   0 victordibia   (501) staff       (20)        1 2024-04-23 22:21:41.000000 autogenstudio-0.0.56rc2/autogenstudio.egg-info/dependency_links.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       56 2024-04-23 22:21:41.000000 autogenstudio-0.0.56rc2/autogenstudio.egg-info/entry_points.txt
--rw-r--r--   0 victordibia   (501) staff       (20)      159 2024-04-23 22:21:41.000000 autogenstudio-0.0.56rc2/autogenstudio.egg-info/requires.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       14 2024-04-23 22:21:41.000000 autogenstudio-0.0.56rc2/autogenstudio.egg-info/top_level.txt
--rw-r--r--   0 victordibia   (501) staff       (20)     1486 2024-04-23 16:45:48.000000 autogenstudio-0.0.56rc2/pyproject.toml
--rw-r--r--   0 victordibia   (501) staff       (20)        2 2024-03-19 16:11:36.000000 autogenstudio-0.0.56rc2/requirements.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       38 2024-04-23 22:21:44.882365 autogenstudio-0.0.56rc2/setup.cfg
--rw-r--r--   0 victordibia   (501) staff       (20)       38 2024-03-19 16:11:36.000000 autogenstudio-0.0.56rc2/setup.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.866963 autogenstudio-0.0.9a0/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      342 2023-12-06 21:04:40.000000 autogenstudio-0.0.9a0/.gitignore
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      152 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/MANIFEST.in
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     7308 2023-12-06 21:25:08.866963 autogenstudio-0.0.9a0/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6592 2023-12-06 20:46:34.000000 autogenstudio-0.0.9a0/README.md
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       83 2023-12-06 20:49:20.000000 autogenstudio-0.0.9a0/autogenstudio/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2284 2023-12-06 20:43:55.000000 autogenstudio-0.0.9a0/autogenstudio/chatmanager.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      862 2023-12-06 20:49:48.000000 autogenstudio-0.0.9a0/autogenstudio/cli.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4036 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/datamodel.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/utils/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       44 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/utils/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)    12441 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/utils/dbutils.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)    15392 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/utils/utils.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       43 2023-12-04 03:29:11.000000 autogenstudio-0.0.9a0/autogenstudio/version.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/web/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/autogenstudio/web/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     9262 2023-12-06 20:44:10.000000 autogenstudio-0.0.9a0/autogenstudio/web/app.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/web/skills/
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/web/skills/global/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1329 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/autogenstudio/web/skills/global/fetch_profile.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2444 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/autogenstudio/web/skills/global/find_papers_arxiv.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1965 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/web/skills/global/generate_images.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4676 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/workflowmanager.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio.egg-info/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     7308 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      758 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       56 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/entry_points.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       77 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/requires.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       14 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/top_level.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1355 2023-12-06 20:48:09.000000 autogenstudio-0.0.9a0/pyproject.toml
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        2 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/requirements.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-12-06 21:25:08.866963 autogenstudio-0.0.9a0/setup.cfg
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/setup.py
```

### Comparing `autogenstudio-0.0.56rc2/autogenstudio/utils/utils.py` & `autogenstudio-0.0.9a0/autogenstudio/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,28 @@
+import ast
 import base64
 import hashlib
+from typing import List, Dict, Tuple, Union
 import os
-import re
 import shutil
-from datetime import datetime
-from pathlib import Path
-from typing import Any, Dict, List, Tuple, Union
-
-from dotenv import load_dotenv
-
-from autogen.coding import DockerCommandLineCodeExecutor, LocalCommandLineCodeExecutor
-from autogen.oai.client import ModelClient, OpenAIWrapper
-
-from ..datamodel import Agent, AgentType, CodeExecutionConfigTypes, Model, Skill, Workflow, WorkflowAgentLink
-from ..dbmanager import DBManager
-from ..version import APP_NAME
+import re
+import autogen
+from ..datamodel import AgentConfig, AgentFlowSpec, AgentWorkFlowConfig, LLMConfig
 
 
 def md5_hash(text: str) -> str:
     """
     Compute the MD5 hash of a given text.
 
     :param text: The string to hash
     :return: The MD5 hash of the text
     """
     return hashlib.md5(text.encode()).hexdigest()
 
 
-def check_and_cast_datetime_fields(obj: Any) -> Any:
-    if hasattr(obj, "created_at") and isinstance(obj.created_at, str):
-        obj.created_at = str_to_datetime(obj.created_at)
-
-    if hasattr(obj, "updated_at") and isinstance(obj.updated_at, str):
-        obj.updated_at = str_to_datetime(obj.updated_at)
-
-    return obj
-
-
-def str_to_datetime(dt_str: str) -> datetime:
-    if dt_str[-1] == "Z":
-        # Replace 'Z' with '+00:00' for UTC timezone
-        dt_str = dt_str[:-1] + "+00:00"
-    return datetime.fromisoformat(dt_str)
-
-
-def clear_folder(folder_path: str) -> None:
-    """
-    Clear the contents of a folder.
-
-    :param folder_path: The path to the folder to clear.
-    """
-    # exit if the folder does not exist
-    if not os.path.exists(folder_path):
-        return
-    # exit if the folder does not exist
-    if not os.path.exists(folder_path):
-        return
-    for file in os.listdir(folder_path):
-        file_path = os.path.join(folder_path, file)
-        if os.path.isfile(file_path):
-            os.remove(file_path)
-        elif os.path.isdir(file_path):
-            shutil.rmtree(file_path)
-
-
 def get_file_type(file_path: str) -> str:
     """
 
 
     Get file type   determined by the file extension. If the file extension is not
     recognized, 'unknown' will be used as the file type.
 
@@ -109,48 +64,30 @@
         ".scala",
         ".lua",
         ".pl",
         ".sql",
         ".config",
     }
 
-    # Supported spreadsheet extensions
-    CSV_EXTENSIONS = {".csv", ".xlsx"}
-
     # Supported image extensions
-    IMAGE_EXTENSIONS = {
-        ".png",
-        ".jpg",
-        ".jpeg",
-        ".gif",
-        ".bmp",
-        ".tiff",
-        ".svg",
-        ".webp",
-    }
-    # Supported (web) video extensions
-    VIDEO_EXTENSIONS = {".mp4", ".webm", ".ogg", ".mov", ".avi", ".wmv"}
+    IMAGE_EXTENSIONS = {".png", ".jpg", ".jpeg", ".gif", ".bmp", ".tiff", ".svg", ".webp"}
 
     # Supported PDF extension
     PDF_EXTENSION = ".pdf"
 
     # Determine the file extension
     _, file_extension = os.path.splitext(file_path)
 
     # Determine the file type based on the extension
     if file_extension in CODE_EXTENSIONS:
         file_type = "code"
-    elif file_extension in CSV_EXTENSIONS:
-        file_type = "csv"
     elif file_extension in IMAGE_EXTENSIONS:
         file_type = "image"
     elif file_extension == PDF_EXTENSION:
         file_type = "pdf"
-    elif file_extension in VIDEO_EXTENSIONS:
-        file_type = "video"
     else:
         file_type = "unknown"
 
     return file_type
 
 
 def serialize_file(file_path: str) -> Tuple[str, str]:
@@ -167,150 +104,199 @@
 
     file_type = get_file_type(file_path)
 
     # Read the file and encode its contents
     try:
         with open(file_path, "rb") as file:
             file_content = file.read()
-            base64_encoded_content = base64.b64encode(
-                file_content).decode("utf-8")
+            base64_encoded_content = base64.b64encode(file_content).decode("utf-8")
     except Exception as e:
-        raise IOError(f"An error occurred while reading the file: {e}") from e
+        raise IOError(f"An error occurred while reading the file: {e}")
 
     return base64_encoded_content, file_type
 
 
-def get_modified_files(start_timestamp: float, end_timestamp: float, source_dir: str) -> List[Dict[str, str]]:
-    """
-    Identify files from source_dir that were modified within a specified timestamp range.
-    The function excludes files with certain file extensions and names.
+def get_modified_files(
+    start_timestamp: float, end_timestamp: float, source_dir: str, dest_dir: str
+) -> List[Dict[str, str]]:
+    """
+    Copy files from source_dir that were modified within a specified timestamp range
+    to dest_dir, renaming files if they already exist there. The function excludes
+    files with certain file extensions and names.
 
-    :param start_timestamp: The floating-point number representing the start timestamp to filter modified files.
-    :param end_timestamp: The floating-point number representing the end timestamp to filter modified files.
+    :param start_timestamp: The start timestamp to filter modified files.
+    :param end_timestamp: The end timestamp to filter modified files.
     :param source_dir: The directory to search for modified files.
+    :param dest_dir: The destination directory to copy modified files to.
 
-    :return: A list of dictionaries with details of relative file paths that were modified.
-             Dictionary format: {path: "", name: "", extension: "", type: ""}
+    :return: A list of dictionaries with details of file paths in dest_dir that were modified and copied over.
+             Dictionary format: {path: "", name: "", extension: ""}
              Files with extensions "__pycache__", "*.pyc", "__init__.py", and "*.cache"
              are ignored.
     """
     modified_files = []
     ignore_extensions = {".pyc", ".cache"}
     ignore_files = {"__pycache__", "__init__.py"}
 
-    # Walk through the directory tree
     for root, dirs, files in os.walk(source_dir):
-        # Update directories and files to exclude those to be ignored
+        # Excluding the directory "__pycache__" if present
         dirs[:] = [d for d in dirs if d not in ignore_files]
-        files[:] = [f for f in files if f not in ignore_files and os.path.splitext(f)[
-            1] not in ignore_extensions]
 
         for file in files:
             file_path = os.path.join(root, file)
-            file_mtime = os.path.getmtime(file_path)
+            file_ext = os.path.splitext(file)[1]
+            file_name = os.path.basename(file)
 
-            # Verify if the file was modified within the given timestamp range
-            if start_timestamp <= file_mtime <= end_timestamp:
-                file_relative_path = (
-                    "files/user" +
-                    file_path.split(
-                        "files/user", 1)[1] if "files/user" in file_path else ""
-                )
-                file_type = get_file_type(file_path)
+            if file_ext in ignore_extensions or file_name in ignore_files:
+                continue
 
+            file_mtime = os.path.getmtime(file_path)
+            if start_timestamp < file_mtime < end_timestamp:
+                dest_file_path = os.path.join(dest_dir, file)
+                copy_idx = 1
+                while os.path.exists(dest_file_path):
+                    base, extension = os.path.splitext(file)
+                    # Handling potential name conflicts by appending a number
+                    dest_file_path = os.path.join(dest_dir, f"{base}_{copy_idx}{extension}")
+                    copy_idx += 1
+
+                # Copying the modified file to the destination directory
+                shutil.copy2(file_path, dest_file_path)
+
+                # Extract user id from the dest_dir and file path
+                uid = dest_dir.split("/")[-1]
+                relative_file_path = os.path.relpath(dest_file_path, start=dest_dir)
+                file_type = get_file_type(dest_file_path)
                 file_dict = {
-                    "path": file_relative_path,
-                    "name": os.path.basename(file),
-                    # Remove the dot
-                    "extension": os.path.splitext(file)[1].lstrip("."),
+                    "path": f"files/user/{uid}/{relative_file_path}",
+                    "name": file_name,
+                    "extension": file_ext.replace(".", ""),
                     "type": file_type,
                 }
                 modified_files.append(file_dict)
-
-    # Sort the modified files by extension
+    # sort by extension
     modified_files.sort(key=lambda x: x["extension"])
     return modified_files
 
 
-def init_app_folders(app_file_path: str) -> Dict[str, str]:
+def init_webserver_folders(root_file_path: str) -> Dict[str, str]:
     """
     Initialize folders needed for a web server, such as static file directories
-    and user-specific data directories. Also load any .env file if it exists.
+    and user-specific data directories.
 
     :param root_file_path: The root directory where webserver folders will be created
     :return: A dictionary with the path of each created folder
     """
-
-    app_name = f".{APP_NAME}"
-    default_app_root = os.path.join(os.path.expanduser("~"), app_name)
-    if not os.path.exists(default_app_root):
-        os.makedirs(default_app_root, exist_ok=True)
-    app_root = os.environ.get("AUTOGENSTUDIO_APPDIR") or default_app_root
-
-    if not os.path.exists(app_root):
-        os.makedirs(app_root, exist_ok=True)
-
-    # load .env file if it exists
-    env_file = os.path.join(app_root, ".env")
-    if os.path.exists(env_file):
-        print(f"Loading environment variables from {env_file}")
-        load_dotenv(env_file)
-
-    files_static_root = os.path.join(app_root, "files/")
-    static_folder_root = os.path.join(app_file_path, "ui")
+    files_static_root = os.path.join(root_file_path, "files/")
+    static_folder_root = os.path.join(root_file_path, "ui")
+    workdir_root = os.path.join(root_file_path, "workdir")
+    skills_dir = os.path.join(root_file_path, "skills")
+    user_skills_dir = os.path.join(skills_dir, "user")
+    global_skills_dir = os.path.join(skills_dir, "global")
 
     os.makedirs(files_static_root, exist_ok=True)
     os.makedirs(os.path.join(files_static_root, "user"), exist_ok=True)
     os.makedirs(static_folder_root, exist_ok=True)
+    os.makedirs(workdir_root, exist_ok=True)
+    os.makedirs(skills_dir, exist_ok=True)
+    os.makedirs(user_skills_dir, exist_ok=True)
+    os.makedirs(global_skills_dir, exist_ok=True)
+
     folders = {
         "files_static_root": files_static_root,
         "static_folder_root": static_folder_root,
-        "app_root": app_root,
+        "workdir_root": workdir_root,
+        "skills_dir": skills_dir,
+        "user_skills_dir": user_skills_dir,
+        "global_skills_dir": global_skills_dir,
     }
-    print(f"Initialized application data folder: {app_root}")
     return folders
 
 
-def get_skills_from_prompt(skills: List[Skill], work_dir: str) -> str:
+def skill_from_folder(folder: str) -> List[Dict[str, str]]:
     """
-    Create a prompt with the content of all skills and write the skills to a file named skills.py in the work_dir.
+    Given a folder, return a dict of the skill (name, python file content). Only python files are considered.
+
+    :param folder: The folder to search for skills
+    :return: A list of dictionaries, each representing a skill
+    """
+
+    skills = []
+    for root, dirs, files in os.walk(folder):
+        for file in files:
+            if file.endswith(".py"):
+                skill_name = file.split(".")[0]
+                skill_file_path = os.path.join(root, file)
+                with open(skill_file_path, "r", encoding="utf-8") as f:
+                    skill_content = f.read()
+                skills.append({"name": skill_name, "content": skill_content, "file_name": file})
+    return skills
+
+
+def get_all_skills(user_skills_path: str, global_skills_path: str, dest_dir: str = None) -> List[Dict[str, str]]:
+    """
+    Get all skills from the user and global skills directories. If dest_dir, copy all skills to dest_dir.
+
+    :param user_skills_path: The path to the user skills directory
+    :param global_skills_path: The path to the global skills directory
+    :param dest_dir: The destination directory to copy all skills to
+    :return: A dictionary of user and global skills
+    """
+    user_skills = skill_from_folder(user_skills_path)
+    os.makedirs(user_skills_path, exist_ok=True)
+    global_skills = skill_from_folder(global_skills_path)
+    skills = {
+        "user": user_skills,
+        "global": global_skills,
+    }
+
+    if dest_dir:
+        # chcek if dest_dir exists
+        if not os.path.exists(dest_dir):
+            os.makedirs(dest_dir)
+        # copy all skills to dest_dir
+        for skill in user_skills + global_skills:
+            skill_file_path = os.path.join(dest_dir, skill["file_name"])
+            with open(skill_file_path, "w", encoding="utf-8") as f:
+                f.write(skill["content"])
+
+    return skills
 
-    :param skills: A dictionary skills
+
+def get_skills_prompt(skills: List[Dict[str, str]]) -> str:
+    """
+    Get a prompt with the content of all skills.
+
+    :param skills: A dictionary of user and global skills
     :return: A string containing the content of all skills
     """
+    user_skills = skills["user"]
+    global_skills = skills["global"]
+    all_skills = user_skills + global_skills
 
-    instruction = """
+    prompt = """
 
-While solving the task you may use functions below which will be available in a file called skills.py .
-To use a function skill.py in code, IMPORT THE FUNCTION FROM skills.py  and then use the function.
+While solving the task you may use functions in the files below.
+To use a function from a file in code, import the file and then use the function.
 If you need to install python packages, write shell code to
 install via pip and use --quiet option.
 
          """
-    prompt = ""  # filename:  skills.py
-    for skill in skills:
+    for skill in all_skills:
         prompt += f"""
 
-##### Begin of {skill.name} #####
+##### Begin of {skill["file_name"]} #####
 
-{skill.content}
+{skill["content"]}
 
-#### End of {skill.name} ####
+#### End of {skill["file_name"]} ####
 
         """
 
-    # check if work_dir exists
-    if not os.path.exists(work_dir):
-        os.makedirs(work_dir)
-
-    # overwrite skills.py in work_dir
-    with open(os.path.join(work_dir, "skills.py"), "w", encoding="utf-8") as f:
-        f.write(prompt)
-
-    return instruction + prompt
+    return prompt
 
 
 def delete_files_in_folder(folders: Union[str, List[str]]) -> None:
     """
     Delete all files and directories in the specified folders.
 
     :param folders: A list of folders or a single folder string
@@ -337,168 +323,131 @@
                     # Remove the directory and all its content
                     shutil.rmtree(path)
             except Exception as e:
                 # Print the error message and skip
                 print(f"Failed to delete {path}. Reason: {e}")
 
 
+def get_default_agent_config(work_dir: str, skills_suffix: str = "") -> AgentWorkFlowConfig:
+    """
+    Get a default agent flow config .
+    """
+
+    llm_config = LLMConfig(
+        config_list=[{"model": "gpt-4"}],
+        temperature=0,
+    )
+
+    USER_PROXY_INSTRUCTIONS = """If the request has been addressed sufficiently, summarize the answer and end with the word TERMINATE. Otherwise, ask a follow-up question.
+        """
+
+    userproxy_spec = AgentFlowSpec(
+        type="userproxy",
+        config=AgentConfig(
+            name="user_proxy",
+            human_input_mode="NEVER",
+            system_message=USER_PROXY_INSTRUCTIONS,
+            code_execution_config={
+                "work_dir": work_dir,
+                "use_docker": False,
+            },
+            max_consecutive_auto_reply=10,
+            llm_config=llm_config,
+            is_termination_msg=lambda x: x.get("content", "").rstrip().endswith("TERMINATE"),
+        ),
+    )
+
+    assistant_spec = AgentFlowSpec(
+        type="assistant",
+        config=AgentConfig(
+            name="primary_assistant",
+            system_message=autogen.AssistantAgent.DEFAULT_SYSTEM_MESSAGE + skills_suffix,
+            llm_config=llm_config,
+        ),
+    )
+
+    flow_config = AgentWorkFlowConfig(
+        name="default",
+        sender=userproxy_spec,
+        receiver=assistant_spec,
+        type="default",
+    )
+
+    return flow_config
+
+
 def extract_successful_code_blocks(messages: List[Dict[str, str]]) -> List[str]:
     """
     Parses through a list of messages containing code blocks and execution statuses,
     returning the array of code blocks that executed successfully and retains
     the backticks for Markdown rendering.
 
     Parameters:
     messages (List[Dict[str, str]]): A list of message dictionaries containing 'content' and 'role' keys.
 
     Returns:
     List[str]: A list containing the code blocks that were successfully executed, including backticks.
     """
     successful_code_blocks = []
-    # Regex pattern to capture code blocks enclosed in triple backticks.
-    code_block_regex = r"```[\s\S]*?```"
+    code_block_regex = r"```[\s\S]*?```"  # Regex pattern to capture code blocks enclosed in triple backticks.
 
-    for i, row in enumerate(messages):
-        message = row["message"]
+    for i, message in enumerate(messages):
         if message["role"] == "user" and "execution succeeded" in message["content"]:
-            if i > 0 and messages[i - 1]["message"]["role"] == "assistant":
-                prev_content = messages[i - 1]["message"]["content"]
+            if i > 0 and messages[i - 1]["role"] == "assistant":
+                prev_content = messages[i - 1]["content"]
                 # Find all matches for code blocks
                 code_blocks = re.findall(code_block_regex, prev_content)
-                # Add the code blocks with backticks
-                successful_code_blocks.extend(code_blocks)
+                successful_code_blocks.extend(code_blocks)  # Add the code blocks with backticks
 
     return successful_code_blocks
 
 
-def sanitize_model(model: Model):
+def create_skills_from_code(dest_dir: str, skills: Union[str, List[str]]) -> None:
     """
-    Sanitize model dictionary to remove None values and empty strings and only keep valid keys.
-    """
-    if isinstance(model, Model):
-        model = model.model_dump()
-    valid_keys = ["model", "base_url", "api_key", "api_type", "api_version"]
-    # only add key if value is not None
-    sanitized_model = {k: v for k, v in model.items() if (
-        v is not None and v != "") and k in valid_keys}
-    return sanitized_model
-
-
-def test_model(model: Model):
-    """
-    Test the model endpoint by sending a simple message to the model and returning the response.
-    """
-
-    sanitized_model = sanitize_model(model)
-    client = OpenAIWrapper(config_list=[sanitized_model])
-    response = client.create(
-        messages=[{"role": "user", "content": "2+2="}], cache_seed=None)
-    return response.choices[0].message.content
-
-
-def load_code_execution_config(code_execution_type: CodeExecutionConfigTypes, work_dir: str):
+    Create skills from a list of code blocks.
+    Parameters:
+    dest_dir (str): The destination directory to copy all skills to.
+    skills (Union[str, List[str]]): A list of strings containing code blocks.
     """
-    Load the code execution configuration based on the code execution type.
 
-    :param code_execution_type: The code execution type.
-    :param work_dir: The working directory to store code execution files.
-    :return: The code execution configuration.
-
-    """
-    work_dir = Path(work_dir)
-    work_dir.mkdir(exist_ok=True)
-    executor = None
-    if code_execution_type == CodeExecutionConfigTypes.local:
-        executor = LocalCommandLineCodeExecutor(work_dir=work_dir)
-    elif code_execution_type == CodeExecutionConfigTypes.docker:
-        executor = DockerCommandLineCodeExecutor(work_dir=work_dir)
-    elif code_execution_type == CodeExecutionConfigTypes.none:
-        return False
-    else:
-        raise ValueError(f"Invalid code execution type: {code_execution_type}")
-    code_execution_config = {
-        "executor": executor,
-    }
-    return code_execution_config
+    # Ensure skills is a list
+    if isinstance(skills, str):
+        skills = [skills]
 
+    # Check if dest_dir exists
+    if not os.path.exists(dest_dir):
+        os.makedirs(dest_dir)
 
-def workflow_from_id(workflow_id: int, dbmanager: DBManager):
-    workflow = dbmanager.get(Workflow, filters={"id": workflow_id}).data
-    if not workflow or len(workflow) == 0:
-        raise ValueError("The specified workflow does not exist.")
-    workflow = workflow[0].model_dump(mode="json")
-    workflow_agent_links = dbmanager.get(WorkflowAgentLink, filters={
-                                         "workflow_id": workflow_id}).data
-
-    def dump_agent(agent: Agent):
-        exclude = []
-        if agent.type != AgentType.groupchat:
-            exclude = [
-                "admin_name",
-                "messages",
-                "max_round",
-                "admin_name",
-                "speaker_selection_method",
-                "allow_repeat_speaker",
-            ]
-        return agent.model_dump(warnings=False, mode="json", exclude=exclude)
-
-    def get_agent(agent_id):
-        agent: Agent = dbmanager.get(Agent, filters={"id": agent_id}).data[0]
-        agent_dict = dump_agent(agent)
-        agent_dict["skills"] = [Skill.model_validate(
-            skill.model_dump(mode="json")) for skill in agent.skills]
-        model_exclude = [
-            "id",
-            "agent_id",
-            "created_at",
-            "updated_at",
-            "user_id",
-            "description",
-        ]
-        models = [model.model_dump(mode="json", exclude=model_exclude)
-                  for model in agent.models]
-        agent_dict["models"] = [model.model_dump(
-            mode="json") for model in agent.models]
-
-        if len(models) > 0:
-            agent_dict["config"]["llm_config"] = agent_dict.get(
-                "config", {}).get("llm_config", {})
-            llm_config = agent_dict["config"]["llm_config"]
-            if llm_config:
-                llm_config["config_list"] = models
-            agent_dict["config"]["llm_config"] = llm_config
-        agent_dict["agents"] = [get_agent(agent.id) for agent in agent.agents]
-        return agent_dict
-
-    for link in workflow_agent_links:
-        agent_dict = get_agent(link.agent_id)
-        workflow[link.agent_type] = agent_dict
-    return workflow
-
-
-def summarize_chat_history(task: str, messages: List[Dict[str, str]], client: ModelClient):
-    """
-    Summarize the chat history using the model endpoint and returning the response.
-    """
-
-    summarization_system_prompt = f"""
-    You are a helpful assistant that is able to review the chat history between a set of agents (userproxy agents, assistants etc) as they try to address a given TASK and provide a summary. Be SUCCINCT but also comprehensive enough to allow others (who cannot see the chat history) understand and recreate the solution.
-
-    The task requested by the user is:
-    ===
-    {task}
-    ===
-    The summary should focus on extracting the actual solution to the task from the chat history (assuming the task was addressed) such that any other agent reading the summary will understand what the actual solution is. Use a neutral tone and DO NOT directly mention the agents. Instead only focus on the actions that were carried out (e.g. do not say 'assistant agent generated some code visualization code ..'  instead say say 'visualization code was generated ..' ).
-    """
-    summarization_prompt = [
-        {
-            "role": "system",
-            "content": summarization_system_prompt,
-        },
-        {
-            "role": "user",
-            "content": f"Summarize the following chat history. {str(messages)}",
-        },
-    ]
-    response = client.create(messages=summarization_prompt, cache_seed=None)
-    return response.choices[0].message.content
+    for skill in skills:
+        # Attempt to parse the code and extract the top-level function name
+        try:
+            parsed = ast.parse(skill)
+            function_name = None
+            for node in parsed.body:
+                if isinstance(node, ast.FunctionDef):
+                    function_name = node.name
+                    break
+
+            if function_name is None:
+                raise ValueError("No top-level function definition found.")
+
+            # Sanitize the function name for use as a file name
+            function_name = "".join(ch for ch in function_name if ch.isalnum() or ch == "_")
+            skill_file_name = f"{function_name}.py"
+
+        except (ValueError, SyntaxError):
+            skill_file_name = "new_skill.py"
+
+        # If the generated/sanitized name already exists, append an index
+        skill_file_path = os.path.join(dest_dir, skill_file_name)
+        index = 1
+        while os.path.exists(skill_file_path):
+            base, ext = os.path.splitext(skill_file_name)
+            if base.endswith(f"_{index - 1}"):
+                base = base.rsplit("_", 1)[0]
+
+            skill_file_path = os.path.join(dest_dir, f"{base}_{index}{ext}")
+            index += 1
+
+        # Write the skill to the file
+        with open(skill_file_path, "w", encoding="utf-8") as f:
+            f.write(skill)
```

### Comparing `autogenstudio-0.0.56rc2/pyproject.toml` & `autogenstudio-0.0.9a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autogenstudio"
 authors = [
-  { name="AutoGen Team", email="autogen@microsoft.com" },
+  { name="Autogen Team", email="autogen@microsoft.com" },
 ]
-description = "AutoGen Studio"
+description = "Autogen Studio"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.9, <3.13"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 dependencies = [
     "pydantic",
     "fastapi",
     "typer",
     "uvicorn",
     "arxiv",
-    "pyautogen[gemini]>=0.2.0",
-    "python-dotenv",
-    "websockets",
-    "numpy < 2.0.0",
-    "sqlmodel",
-    "psycopg",
+    "pyautogen==0.2.0"
 ]
-optional-dependencies = {web = ["fastapi", "uvicorn"], database = ["psycopg"]}
+optional-dependencies = {web = ["fastapi", "uvicorn"]}
 
 dynamic = ["version"]
 
 [tool.setuptools]
 include-package-data = true
```

