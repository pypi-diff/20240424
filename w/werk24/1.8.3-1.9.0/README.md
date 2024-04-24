# Comparing `tmp/werk24-1.8.3.tar.gz` & `tmp/werk24-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/werk24-1.8.3.tar", last modified: Thu Dec 14 09:18:20 2023, max compression
+gzip compressed data, was "dist/werk24-1.9.0.tar", last modified: Wed Jan 24 09:54:42 2024, max compression
```

## Comparing `werk24-1.8.3.tar` & `werk24-1.9.0.tar`

### file list

```diff
@@ -1,124 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-12-14 09:18:11.000000 werk24-1.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-14 09:18:11.000000 werk24-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-12-14 09:18:11.000000 werk24-1.8.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2023-12-14 09:18:20.000000 werk24-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-12-14 09:18:11.000000 werk24-1.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 09:18:20.000000 werk24-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-12-14 09:18:11.000000 werk24-1.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   366380 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/assets/fonts/STIX2Text-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (127)   238007 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/assets/fonts/STIX_2.0.2_license.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/assets/images/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/assets/images/favicon-24x24.png
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/assets/images/favicon-256x256.png
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/assets/images/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/assets/images/favicon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/assets/images/logo-625.png
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/cli/health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/cli/support.py
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/cli/techread.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/cli/w24cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/event_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/event_illustrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/gdt_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/json_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/measure_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (127)    23860 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/w24gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/gui/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/alphabet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)    37071 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/ask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/base_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/bom_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/chamfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/depth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/models/feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/feature/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/feature/chamfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/feature/knurl.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/font.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/fraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/gdt.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/general_tolerances.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/geometric_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/helpdesk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/hole_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/icon.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/leader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/location.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/note.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/paper_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/part_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/physical_quantity.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/projection_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24/models/property/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/abbe_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/bubbles_and_inclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/cleanness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/color.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/corrosion_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/fraunhofer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/glass_homogeneity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/hardness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/refractive_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/stress_birefringence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/striae.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/surface_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/property/weight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/revision_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9531 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/roughness.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/size.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9978 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/techread.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/test_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)    12444 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/thread_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/title_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/tolerance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/typed_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/value.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/view.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/models/weight.py
--rw-r--r--   0 runner    (1001) docker     (127)    32342 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/techread_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/techread_client_https.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/techread_client_wss.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-14 09:18:11.000000 werk24-1.8.3/werk24/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2023-12-14 09:18:19.000000 werk24-1.8.3/werk24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-12-14 09:18:20.000000 werk24-1.8.3/werk24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 09:18:19.000000 werk24-1.8.3/werk24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-14 09:18:19.000000 werk24-1.8.3/werk24.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-14 09:18:19.000000 werk24-1.8.3/werk24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-14 09:18:19.000000 werk24-1.8.3/werk24.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-24 09:54:31.000000 werk24-1.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-24 09:54:31.000000 werk24-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-24 09:54:31.000000 werk24-1.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-01-24 09:54:42.000000 werk24-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-01-24 09:54:31.000000 werk24-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 09:54:42.000000 werk24-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-01-24 09:54:31.000000 werk24-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   366380 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/assets/fonts/STIX2Text-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   238007 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/assets/fonts/STIX_2.0.2_license.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/assets/images/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/assets/images/favicon-24x24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/assets/images/favicon-256x256.png
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/assets/images/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/assets/images/favicon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/assets/images/logo-625.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/cli/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/cli/support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/cli/techread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/cli/w24cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/alphabet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/base_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/bom_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/chamfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/depth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24/models/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/feature/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/feature/chamfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/feature/knurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/fraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/gdt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/general_tolerances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/geometric_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/helpdesk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/hole_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/leader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/paper_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/part_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/physical_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/projection_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24/models/property/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/abbe_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/bubbles_and_inclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/cleanness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/corrosion_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/fraunhofer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/glass_homogeneity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/hardness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/refractive_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/stress_birefringence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/striae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/surface_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/property/weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/revision_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/roughness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-01-24 09:54:31.000000 werk24-1.9.0/werk24/models/techread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/test_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/thread_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/title_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/typed_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/models/weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34076 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/techread_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/techread_client_https.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/techread_client_wss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-24 09:54:32.000000 werk24-1.9.0/werk24/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-24 09:54:42.000000 werk24-1.9.0/werk24.egg-info/top_level.txt
```

### Comparing `werk24-1.8.3/PKG-INFO` & `werk24-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werk24
-Version: 1.8.3
+Version: 1.9.0
 Summary: Werk24 Client to read PDF- and Image-based Technical Drawings / Engineering Drawings
 Home-page: https://werk24.io
 Author: W24 Service GmbH
 Author-email: info@werk24.io
 License: commercial
 Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
@@ -116,8 +116,7 @@
 Keywords: Digitisation,Digitization,Engineering Drawing,Engineering Drawings,Technical Drawing,Technical Drawings,CAD,CAD Drawing,Data Extraction,Information Extraction,Model Based Definition,EN10027,ISO2768,Title Block,General Tolerances,Material,Drawing ID,Drawing Designation,Product Manufacturing Information,PMI,Scanned Document,Bill of Material,BOM,Anonymiziation,RFQ,GD&T,General Dimensioning and Toleration,Vectorization
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Provides-Extra: gui
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: werk24 Version: 1.8.3 Summary: Werk24 Client to
+Metadata-Version: 2.1 Name: werk24 Version: 1.9.0 Summary: Werk24 Client to
 read PDF- and Image-based Technical Drawings / Engineering Drawings Home-page:
 https://werk24.io Author: W24 Service GmbH Author-email: info@werk24.io
 License: commercial Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
                                    _[_W_e_r_k_2_4_]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
 pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
@@ -41,8 +41,8 @@
 Extraction,Model Based Definition,EN10027,ISO2768,Title Block,General
 Tolerances,Material,Drawing ID,Drawing Designation,Product Manufacturing
 Information,PMI,Scanned Document,Bill of
 Material,BOM,Anonymiziation,RFQ,GD&T,General Dimensioning and
 Toleration,Vectorization Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Image Recognition Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown Provides-Extra: gui
+Description-Content-Type: text/markdown
```

### Comparing `werk24-1.8.3/README.md` & `werk24-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/setup.py` & `werk24-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,31 +30,27 @@
     author_email="info@werk24.io",
     description="Werk24 Client to read PDF- and Image-based "
     "Technical Drawings / Engineering Drawings",
     url="https://werk24.io",
     entry_points={
         "console_scripts": [
             "w24cli=werk24.cli.w24cli:main",
-            "w24gui=werk24.gui.w24gui:main",
-        ]
+        ],
     },
-    extras_require={"gui": ["PyQt5", "pillow"]},
     license="commercial",
     packages=[
         "werk24",
         "werk24.cli",
-        "werk24.gui",
         "werk24.models",
     ],
     include_package_data=True,
     package_data={"werk24": ["assets/*"]},
     install_requires=[
         "aiohttp >= 3.8.3",
         "boto3 >= 1.14.44",
-        "devtools>=0.9.0,<1.0",
         "pydantic>=2.5.1",
         "pydantic-extra-types>=2.1.0",
         "python-dotenv>=0.10.1,<1.0",
         "websockets >= 10.3",
         "pint >= 0.21",
     ],
     classifiers=[
```

### Comparing `werk24-1.8.3/werk24/assets/fonts/STIX2Text-Regular.otf` & `werk24-1.9.0/werk24/assets/fonts/STIX2Text-Regular.otf`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/assets/fonts/STIX_2.0.2_license.pdf` & `werk24-1.9.0/werk24/assets/fonts/STIX_2.0.2_license.pdf`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/assets/images/favicon-256x256.png` & `werk24-1.9.0/werk24/assets/images/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/assets/images/favicon-32x32.png` & `werk24-1.9.0/werk24/assets/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/assets/images/favicon-48x48.png` & `werk24-1.9.0/werk24/assets/images/favicon-48x48.png`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/assets/images/logo-625.png` & `werk24-1.9.0/werk24/assets/images/logo-625.png`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/auth_client.py` & `werk24-1.9.0/werk24/auth_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,229 +1,247 @@
-""" Module handling the authentication
-"""
-import base64
-import hashlib
-import hmac
-import time
-from typing import Optional, Tuple
-
-import boto3
-from botocore import UNSIGNED
-from botocore.client import Config
-from botocore.exceptions import ClientError
-
-from werk24.exceptions import UnauthorizedException
-
-
-class AuthClient:
-    """Client Module that handles the authentication
-    with AWS Cognito.
-
-    Raises:
-        UnauthorizedException: Raised when the user credentials are not
-            accepted by AWS Cognito
-
-        RuntimeError: Raised when the server behaves in a very unexpected
-            way; e.g., when AWS changed the protocol
-    """
-
-    def __init__(
-        self,
-        cognito_region: str,
-        cognito_identity_pool_id: str,
-        cognito_user_pool_id: str,
-        cognito_client_id: str,
-        cognito_client_secret: str,
-    ):
-        # store the settings
-        self._cognito_region = cognito_region
-        self._cognito_identity_pool_id = cognito_identity_pool_id
-        self._cognito_user_pool_id = cognito_user_pool_id
-        self._cognito_client_id = cognito_client_id
-        self._cognito_client_secret = cognito_client_secret
-
-        # make empty references to the username and password
-        self.username: Optional[str] = None
-        self._password: Optional[str] = None
-
-        # make an empty reference ot the jwt_token
-        self.token: Optional[str] = None
-        self.expires_at: Optional[float] = None
-        self.refresh_token: Optional[str] = None
-
-    def register(self, username: str, password: str) -> None:
-        """Store the username and password locally so
-        that it can be used to obtain the token
-
-        Arguments:
-            username {str} -- Username
-            password {str} -- Password
-        """
-        self.username = username
-        self._password = password
-
-    def _get_generic_identity(self) -> Tuple[str, str]:
-        """The AWS Cognito User Pools can only be accessed with
-        credentials (even if they are generic). This function
-        calls the AWS Cognito IDENTITY POOL to obtain the generic
-        and unpriviledged credientials
-
-        Raises:
-            UnauthorizedException: Raise when we are not able to
-                obtain unpriviledged credentials
-
-        Returns:
-            Tuple[str, str] -- Access Key, Secret Key Tuple
-        """
-
-        # make the identity client
-        try:
-            identity_client = boto3.client(
-                "cognito-identity",
-                config=Config(signature_version=UNSIGNED),
-                region_name=self._cognito_region,
-            )
-
-            # get a new identity id
-            identity_response = identity_client.get_id(
-                IdentityPoolId=self._cognito_identity_pool_id
-            )
-            identity_id = identity_response["IdentityId"]
-
-            # obtain the associated credentials
-            credentials_response = identity_client.get_credentials_for_identity(
-                IdentityId=identity_id
-            )
-            credentials = credentials_response["Credentials"]
-
-        except KeyError:
-            raise UnauthorizedException("Invalid Cognito configuration")
-
-        except ClientError:  # pylint: disable=try-except-raise
-            raise
-
-        # get the access key / secret key
-        access_key = credentials.get("AccessKeyId")
-        secret_key = credentials.get("SecretKey")
-        if access_key is None or secret_key is None:
-            raise UnauthorizedException(
-                "Unable to obtain Access and Secret Key from " "Cognito Identity Pool"
-            )
-
-        # that's it
-        return access_key, secret_key
-
-    def _make_cognito_client(self) -> boto3.session.Session.client:
-        """Make the Cognito Client to communicate with
-        AWS Cognito
-
-        Returns:
-            boto3.session.Session.client -- Boto3 Client
-        """
-
-        try:
-            # before we can aws cognito USER POOL client, we need
-            # to obtain a generic identity from the IDENTIY POOL
-            access_key, secret_key = self._get_generic_identity()
-
-            # with this information, we can now generate the client
-            return boto3.client(
-                "cognito-idp",
-                region_name=self._cognito_region,
-                aws_access_key_id=access_key,
-                aws_secret_access_key=secret_key,
-            )
-        except ClientError:
-            raise UnauthorizedException("Cognito IDP Client Error")
-
-    def _make_cognito_secret_hash(self, username: str) -> str:
-        """Make the keyed-hash message authentication code (HMAC) calculated
-        using the secret key of a user pool client and username plus the client
-        ID in the message.
-
-        Arguments:
-            username {str} -- Username
-
-        Returns:
-            str -- Cognito Secret Hash
-        """
-
-        # make the message
-        message = username + self._cognito_client_id
-
-        # make the secret
-        dig = hmac.new(
-            self._cognito_client_secret.encode("UTF-8"),
-            msg=message.encode("UTF-8"),
-            digestmod=hashlib.sha256,
-        ).digest()
-
-        # turn the secret into a str object
-        return base64.b64encode(dig).decode()
-
-    def login(self) -> None:
-        """Login with AWS Cognito
-
-        Raises:
-            UnauthorizedException: Raised when the user credentials
-                were not accepted by Cognito
-        """
-        if self.token is None or self._token_has_expired():
-            self._login()
-
-    def _token_has_expired(self, slack_minutes: int = 60) -> bool:
-        """Check whether the token has already expired
-
-        Returns:
-            bool: True if exptired, False otherwise.
-        """
-        if self.expires_at is None:
-            return True
-
-        return time.time() > self.expires_at - slack_minutes
-
-    def _login(self):
-        """Preform the login with AWS Cognito
-
-        Raises:
-            UnauthorizedException: Raised when the user is not authorized
-                or something went wrong during the authentication process.
-        """
-
-        # there is no point in trying to log in if there is no
-        # username or password
-        if self.username is None or self._password is None:
-            raise UnauthorizedException("No username / password provided")
-
-        # make the connection to aws
-        cognito_client = self._make_cognito_client()
-
-        # make the authentication data
-        auth_data = {
-            "USERNAME": self.username,
-            "PASSWORD": self._password,
-            "SECRET_HASH": self._make_cognito_secret_hash(self.username),
-        }
-
-        # get the jwt token from AWS cognito
-        try:
-            resp = cognito_client.initiate_auth(
-                AuthFlow="USER_PASSWORD_AUTH",
-                AuthParameters=auth_data,
-                ClientId=self._cognito_client_id,
-            )
-
-        # We will receive an error message directly from AWS Cognito
-        # if anything goes wrong. The error message will be valuable,
-        # as it allows the user to differentiate between disabled
-        # accounts and incorrect credentials
-        except cognito_client.exceptions.NotAuthorizedException:
-            raise UnauthorizedException()
-
-        # store the jwt token
-        try:
-            result = resp["AuthenticationResult"]
-            self.token = result["IdToken"]
-            self.expires_at = time.time() + int(result["ExpiresIn"])
-            self.refresh_token = result["RefreshToken"]
-        except KeyError:
-            raise UnauthorizedException("Unable to obtain JWT Token from AWS Cognito.")
+""" Module handling the authentication
+"""
+import base64
+import hashlib
+import hmac
+import time
+from typing import Optional, Tuple
+
+import boto3
+from botocore import UNSIGNED
+from botocore.client import Config
+from botocore.exceptions import ClientError
+
+from werk24.exceptions import UnauthorizedException
+
+
+class AuthClient:
+    """Client Module that handles the authentication
+    with AWS Cognito.
+
+    Raises:
+        UnauthorizedException: Raised when the user credentials are not
+            accepted by AWS Cognito
+
+        RuntimeError: Raised when the server behaves in a very unexpected
+            way; e.g., when AWS changed the protocol
+    """
+
+    def __init__(
+        self,
+        cognito_region: Optional[str],
+        cognito_identity_pool_id: Optional[str],
+        cognito_user_pool_id: Optional[str],
+        cognito_client_id: Optional[str],
+        cognito_client_secret: Optional[str],
+        username: Optional[str],
+        password: Optional[str],
+        api_token: Optional[str],
+    ):
+        # store the settings
+        self._cognito_region = cognito_region
+        self._cognito_identity_pool_id = cognito_identity_pool_id
+        self._cognito_user_pool_id = cognito_user_pool_id
+        self._cognito_client_id = cognito_client_id
+        self._cognito_client_secret = cognito_client_secret
+
+        # make empty references to the username and password
+        self.cognito_username: Optional[str] = username
+        self._cognito_password: Optional[str] = password
+
+        # make an empty reference ot the jwt_token
+        self.coginto_token: Optional[str] = None
+        self.cognito_token_expires_at: Optional[float] = None
+        self.cognito_refresh_token: Optional[str] = None
+
+        # store the api token
+        self.api_token = api_token
+
+    def _get_generic_identity(self) -> Tuple[str, str]:
+        """The AWS Cognito User Pools can only be accessed with
+        credentials (even if they are generic). This function
+        calls the AWS Cognito IDENTITY POOL to obtain the generic
+        and unpriviledged credientials
+
+        Raises:
+            UnauthorizedException: Raise when we are not able to
+                obtain unpriviledged credentials
+
+        Returns:
+            Tuple[str, str] -- Access Key, Secret Key Tuple
+        """
+
+        # make the identity client
+        try:
+            identity_client = boto3.client(
+                "cognito-identity",
+                config=Config(signature_version=UNSIGNED),
+                region_name=self._cognito_region,
+            )
+
+            # get a new identity id
+            identity_response = identity_client.get_id(
+                IdentityPoolId=self._cognito_identity_pool_id
+            )
+            identity_id = identity_response["IdentityId"]
+
+            # obtain the associated credentials
+            credentials_response = identity_client.get_credentials_for_identity(
+                IdentityId=identity_id
+            )
+            credentials = credentials_response["Credentials"]
+
+        except KeyError:
+            raise UnauthorizedException("Invalid Cognito configuration")
+
+        except ClientError:  # pylint: disable=try-except-raise
+            raise
+
+        # get the access key / secret key
+        access_key = credentials.get("AccessKeyId")
+        secret_key = credentials.get("SecretKey")
+        if access_key is None or secret_key is None:
+            raise UnauthorizedException(
+                "Unable to obtain Access and Secret Key from " "Cognito Identity Pool"
+            )
+
+        # that's it
+        return access_key, secret_key
+
+    def _make_cognito_client(self) -> boto3.session.Session.client:
+        """Make the Cognito Client to communicate with
+        AWS Cognito
+
+        Returns:
+            boto3.session.Session.client -- Boto3 Client
+        """
+
+        try:
+            # before we can aws cognito USER POOL client, we need
+            # to obtain a generic identity from the IDENTIY POOL
+            access_key, secret_key = self._get_generic_identity()
+
+            # with this information, we can now generate the client
+            return boto3.client(
+                "cognito-idp",
+                region_name=self._cognito_region,
+                aws_access_key_id=access_key,
+                aws_secret_access_key=secret_key,
+            )
+        except ClientError:
+            raise UnauthorizedException("Cognito IDP Client Error")
+
+    def _make_cognito_secret_hash(self, username: str) -> str:
+        """Make the keyed-hash message authentication code (HMAC) calculated
+        using the secret key of a user pool client and username plus the client
+        ID in the message.
+
+        Arguments:
+            username {str} -- Username
+
+        Returns:
+            str -- Cognito Secret Hash
+        """
+
+        # make the message
+        message = username + self._cognito_client_id
+
+        # make the secret
+        dig = hmac.new(
+            self._cognito_client_secret.encode("UTF-8"),
+            msg=message.encode("UTF-8"),
+            digestmod=hashlib.sha256,
+        ).digest()
+
+        # turn the secret into a str object
+        return base64.b64encode(dig).decode()
+
+    def login(self) -> None:
+        """Login with AWS Cognito
+
+        Raises:
+            UnauthorizedException: Raised when the user credentials
+                were not accepted by Cognito
+        """
+        # If we are have an API Token, we don't need to login
+        if self.api_token is not None:
+            return
+
+        # Otherwise trigger the Cognito Login.
+        if self.coginto_token is None or self._token_has_expired():
+            self._login()
+
+    def _token_has_expired(self, slack_minutes: int = 60) -> bool:
+        """Check whether the token has already expired
+
+        Returns:
+            bool: True if exptired, False otherwise.
+        """
+        if self.cognito_token_expires_at is None:
+            return True
+
+        return time.time() > self.cognito_token_expires_at - slack_minutes
+
+    def _login(self):
+        """Preform the login with AWS Cognito
+
+        Raises:
+            UnauthorizedException: Raised when the user is not authorized
+                or something went wrong during the authentication process.
+        """
+
+        # there is no point in trying to log in if there is no
+        # username or password
+        if self.cognito_username is None or self._cognito_password is None:
+            raise UnauthorizedException("No username / password provided")
+
+        # make the connection to aws
+        cognito_client = self._make_cognito_client()
+
+        # make the authentication data
+        auth_data = {
+            "USERNAME": self.cognito_username,
+            "PASSWORD": self._cognito_password,
+            "SECRET_HASH": self._make_cognito_secret_hash(self.cognito_username),
+        }
+
+        # get the jwt token from AWS cognito
+        try:
+            resp = cognito_client.initiate_auth(
+                AuthFlow="USER_PASSWORD_AUTH",
+                AuthParameters=auth_data,
+                ClientId=self._cognito_client_id,
+            )
+
+        # We will receive an error message directly from AWS Cognito
+        # if anything goes wrong. The error message will be valuable,
+        # as it allows the user to differentiate between disabled
+        # accounts and incorrect credentials
+        except cognito_client.exceptions.NotAuthorizedException:
+            raise UnauthorizedException()
+
+        # store the jwt token
+        try:
+            result = resp["AuthenticationResult"]
+            self.coginto_token = result["IdToken"]
+            self.cognito_token_expires_at = time.time() + int(result["ExpiresIn"])
+            self.cognito_refresh_token = result["RefreshToken"]
+        except KeyError:
+            raise UnauthorizedException("Unable to obtain JWT Token from AWS Cognito.")
+
+    def get_auth_headers(self) -> dict:
+        """Get the Authentication Headers.
+
+        There are two authentication methods at the moment.
+        You can either go through AWS Cognito or you can
+        use the API Token. We will gradually phase out the
+        AWS Cognito authentication method. It's too slow
+        and too cumbersome.
+
+        Returns:
+        -------
+        dict: Authentication Headers
+        """
+        if self.api_token is not None:
+            return {"Authorization": "Token " + self.api_token}
+        else:
+            return {"Authorization": "Bearer " + self.coginto_token}
```

### Comparing `werk24-1.8.3/werk24/cli/health_check.py` & `werk24-1.9.0/werk24/cli/health_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         client = utils.make_client()
 
     except LicenseError:
         return {"License Information": "NOT FOUND"}
 
     return {
         "License Information": "FOUND",
-        "Username": client._auth_client.username,
     }
 
 
 def get_module_info() -> dict:
     """Get module information.
     Returns:
         dict: A dictionary containing the module information.
```

### Comparing `werk24-1.8.3/werk24/cli/support.py` & `werk24-1.9.0/werk24/cli/support.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/cli/techread.py` & `werk24-1.9.0/werk24/cli/techread.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import json
 import logging
 import os
 from collections import namedtuple
 from typing import Any, Dict, List, Optional
 
 from dotenv import load_dotenv
-from pydantic import UUID4
 
 from werk24.cli import utils
 from werk24.exceptions import RequestTooLargeException
 from werk24.models.ask import (
     W24AskCanvasThumbnail,
     W24AskPageThumbnail,
     W24AskPartFamilyCharacterization,
@@ -26,14 +25,15 @@
     W24AskVariantGDTs,
     W24AskVariantMeasures,
     W24AskVariantRadii,
     W24AskDebug,
     W24AskVariantRoughnesses,
     W24AskVariantThreadElements,
 )
+from werk24.exceptions import ServerException
 from werk24.models.techread import (
     W24TechreadException,
     W24TechreadMessageSubtypeError,
     W24TechreadMessageSubtypeProgress,
     W24TechreadMessageType,
 )
 from werk24.techread_client import LICENSE_LOCATIONS, Hook
@@ -142,16 +142,17 @@
     payload_dict: Dict[str, Any],
     payload_bytes: Optional[bytes],
     exceptions: List[W24TechreadException],
 ) -> None:
     """Store the CAD file the current directory
 
     Args:
-        payload_dict (Dict[str, Any]): Payload Dictionary
-        payload_bytes (bytes): CAD that we received as response
+    ----
+    payload_dict (Dict[str, Any]): Payload Dictionary
+    payload_bytes (bytes): CAD that we received as response
     """
     logger.info(f"Ask Variant CAD\n{payload_dict}")
 
     # print potential exceptions
     if exceptions:
         _log_exceptions(exceptions)
 
@@ -160,84 +161,88 @@
         _store_variant_cad_payload(payload_dict, payload_bytes)
 
 
 def _log_exceptions(exceptions: List[W24TechreadException]) -> None:
     """Log the encountered exceptions as warnings
 
     Args:
-        exceptions (List[W24TechreadException]): List of
-            encountered exceptions. Can be an empty list.
+    ----
+    exceptions (List[W24TechreadException]): List of
+        encountered exceptions. Can be an empty list.
     """
     for cur_exception in exceptions:
         logger.warn(cur_exception)
 
 
 def _store_variant_cad_payload(
     payload_dict: Dict[str, Any], payload_bytes: bytes
 ) -> None:
     """Store the CAD file with the knowledge that
     the payload exists
 
     Args:
-        payload_dict (Dict[str, Any]): Payload Dictionary
-        payload_bytes (bytes): CAD response
+    ----
+    payload_dict (Dict[str, Any]): Payload Dictionary
+    payload_bytes (bytes): CAD response
     """
     # make the filename
     variant_id = payload_dict.get("variant_id")
     filename = f"./w24_ask_variant_cad_{variant_id}.dxf"
 
     # and write the content
     with open(filename, "wb+") as file_handle:
         file_handle.write(payload_bytes)
 
     # tell the user
     logger.info(f"CAD response stored in {filename}")
 
 
-def _get_drawing(file_path: str) -> Optional[bytes]:
-    """Get the bytes of the file that shall be
-    read.
+def _get_drawing(file_path: str) -> Optional[io.BufferedReader]:
+    """Get the bytes of the file that shall be read.
 
     Args:
-        file_path (str): path to the input file
+    ----
+    file_path (str): path to the input file
 
     Returns:
-        bytes: content of the fiel
+    -------
+    io.BufferedReader: file handle to the input file
     """
     try:
-        with open(file_path, "rb") as filehandle:
-            return filehandle.read()
+        return open(file_path, "rb")
     except FileNotFoundError:
         print(f"File {file_path} not found")
         return None
 
 
 def _print_payload(log_text: str, payload_dict: Dict[str, Any]) -> None:
     """Display the payload dictionary in a format that
     is easy for humans to read
 
     Args:
-        log_text (str): Headline info
-        payload_dict (Dict[str, Any]): Payload dictionary
+    ----
+    log_text (str): Headline info
+    payload_dict (Dict[str, Any]): Payload dictionary
     """
     print(log_text)
     payload_json = json.dumps(payload_dict, indent=4)
     print(payload_json)
 
 
 def _show_image(log_text: str, image_bytes: bytes) -> None:
     """Display a debug image. The function relies on
     the PIL functionality of Image.show(). The
     actual behavior will thus be different across platforms
 
     Args:
-        log_text (str): Log Text that we want to write back
-            to the command line interface
-        image_bytes (bytes): byte representation of the image
-            that is to be displayed
+    ----
+    log_text (str): Log Text that we want to write back
+        to the command line interface
+    image_bytes (bytes): byte representation of the image
+        that is to be displayed
     """
 
     # Import the PIL at runtime to make sure that
     # you can still use the client without the need
     # to install Pillow
     try:
         from PIL import Image  # pylint: disable=import-outside-toplevel
@@ -263,48 +268,40 @@
 
 
 async def main(args: argparse.Namespace) -> None:
     """
     Run the Techread command with the CLI arguments
 
     Args:
-        args(argparse.Namespace): CLI args generated by
+    ----
+    args(argparse.Namespace): CLI args generated by
         argparse
     """
-
-    # interpret the sub-account as UUID4 and stop if that
-    # does not conform to the correct pattern.
-    try:
-        if args.sub_account is not None:
-            sub_account = UUID4(args.sub_account)
-        else:
-            sub_account = None
-
-    except ValueError:
-        logger.error("Sub-Account ID does not conform to UUID4-pattern")
-        return
-
     # make the hooks from the arguments
     hooks = _make_hooks_from_args(args)
 
     # get the client instance and handle
     # potential errors
     client = utils.make_client()
 
-    async with client as session:
-        # get the drawing
-        drawing_bytes = _get_drawing(args.input_file)
-        if drawing_bytes is None:
-            return
+    # get the drawing
+    drawing = _get_drawing(args.input_file)
+    if drawing is None:
+        return
 
+    async with client as session:
         # and make the request
         try:
-            await session.read_drawing_with_hooks(
-                drawing_bytes, hooks, sub_account=sub_account
+            await session.read_drawing_with_hooks(drawing, hooks, sub_account=None)
+            drawing.close()
+        except ServerException as exception:
+            message = "Server Error. Please contact werk24 support: " + str(
+                exception.args
             )
+            logger.error(message)
 
         except RequestTooLargeException:
             message = (
                 "Request was too large to be processed. "
                 + "Please check the documentation for current limits."
             )
             logger.error(message)
@@ -338,16 +335,16 @@
         c_hook = Hook(
             ask=W24AskPartFamilyCharacterization(part_family_id=args.part_family_id),
             function=lambda m: _print_payload(
                 "Part Family Characterization", m.payload_dict
             ),
         )
         hooks.append(c_hook)
+
     if args.debug_key is not None:
         c_hook = Hook(
             ask=W24AskDebug(debug_key=args.debug_key),
-            # function=lambda m: _print_payload("Ask Debug", m.payload_dict),
             function=lambda m: _open_in_webbrowser(m.payload_url),
         )
         hooks.append(c_hook)
 
     return hooks
```

### Comparing `werk24-1.8.3/werk24/cli/w24cli.py` & `werk24-1.9.0/werk24/cli/w24cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 """ Command Line Interface for W24
 """
 import argparse
 import asyncio
 
-import werk24.cli.auth
 import werk24.cli.health_check
 import werk24.cli.support
 import werk24.cli.techread
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(prog="w24cli")
     subparsers = parser.add_subparsers(
         dest="service", help="Service. Currently supported: techread, auth, support"
     )
     subparsers.required = True
 
-    _add_auth_parser(subparsers)
     _add_support_parser(subparsers)
     _add_techread_parser(subparsers)
 
     args = parser.parse_args()
     if args.service == "techread":
         asyncio.run(werk24.cli.techread.main(args))
 
-    elif args.service == "auth":
-        asyncio.run(werk24.cli.auth.main(args))
-
     elif args.service == "support":
         asyncio.run(werk24.cli.support.main(args))
 
     elif args.service == "health_check":
         asyncio.run(werk24.cli.health_check.main(args))
 
 
@@ -44,34 +39,20 @@
     )
 
     create_parser = support_subparsers.add_parser(
         "create-helpdesk-task", help="Create a new help desk task"
     )
 
     create_parser.add_argument("--request-id", action="store", required=True)
-
     create_parser.add_argument("--observed-outcome", action="store", required=True)
-
     create_parser.add_argument("--expected-outcome", action="store", required=True)
-
     create_parser.add_argument("--comment", action="store")
-
     create_parser.add_argument("--importance", action="store", required=True)
 
 
-def _add_auth_parser(subparsers):
-    parser_auth = subparsers.add_parser(
-        "auth", help="Interact with the authentication service"
-    )
-
-    parser_auth.add_argument(
-        "--ask-jwt-token", help="Obtain a valid JWT token", action="store_true"
-    )
-
-
 def _add_techread_parser(subparsers):
     parser_techread = subparsers.add_parser(
         "techread", help="Submit a Technical Drawing to Werk24 for analysis"
     )
 
     parser_techread.add_argument(
         "input_file", help="path to the file that is to be analyzed"
```

### Comparing `werk24-1.8.3/werk24/exceptions.py` & `werk24-1.9.0/werk24/exceptions.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/alphabet.py` & `werk24-1.9.0/werk24/models/alphabet.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/angle.py` & `werk24-1.9.0/werk24/models/angle.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/ask.py` & `werk24-1.9.0/werk24/models/ask.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .leader import W24Leader
 from .material import W24Material
 from .measure import W24Measure
 from .radius import W24Radius
 from .revision_table import W24RevisionTable
 from .roughness import W24Roughness
 from .thread_element import W24ThreadElement
+from .roughness import W24GeneralRoughness, W24RoughnessReference
 
 
 class W24AskType(str, Enum):
     """List of all Ask Type supported by the current
     API version. This list will grow with future releases.
 
     """
@@ -175,16 +176,14 @@
         system load is low.
     """
 
     ask_type: W24AskType
     is_training: bool = False
 
 
-
-
 class W24AskThumbnail(W24Ask):
     """Base model for features that request a thumbnail.
 
     Attributes:
 
         file_format: File format in which you wish to obtain
             the result. Currently only JPEG is supported.
@@ -774,23 +773,31 @@
 
         radii (List[W24Radius]): List of the detected Radii. Note: in the
             PMIExtract, the position will not be returned.
 
         roughnesses (List[W24Roughness]): List of the detected
             roughnesses. Note: in the PMIExtract, the position will not
             be returned.
+        general_roughnesses (List[W24GeneralRoughness]): List of the detected
+            general roughnesses. Note: in the PMIExtract, the position will not
+            be returned.
+        reference_roughnesses (List[W24RoughnessReference]): List of the
+            detected reference roughnesses. Note: in the PMIExtract, the position will not
+            be returned.
     """
 
     variant_id: UUID4
     material: Optional[W24Material]
     general_tolerances: Optional[W24GeneralTolerances]
     measures: List[W24Measure]
     gdts: List[W24GDT]
     radii: List[W24Radius]
     roughnesses: List[W24Roughness]
+    general_roughnesses: List[W24GeneralRoughness] = []
+    reference_roughnesses: List[W24RoughnessReference] = []
 
 
 class W24AskVariantThreadElements(W24Ask):
     """Ask object to obtain the thread elements"""
 
     ask_type: W24AskType = W24AskType.VARIANT_THREAD_ELEMENTS
 
@@ -1075,30 +1082,33 @@
             # Standard info that you would inject into the
             # color cells.
             "designation",
             "drawing_number",
             "part_number",
             "material",
             # Misc.
+            "do_not_scale",
             "software",
             "sheet_number",
             "scale",
             "version",
             "paper_size",
         },
     )
 
     meta_data: W24RebrandingMetaData = Field(
         description=("Metadata that you want to set for the resulting pdf file."),
         default=W24RebrandingMetaData(),
     )
 
+
 class W24AskExcelSummary(W24Ask):
     ask_type: W24AskType = W24AskType.EXCEL_SUMMARY
 
+
 W24AskUnion = Union[
     W24AskCanvasThumbnail,
     W24AskNotes,
     W24AskPageThumbnail,
     W24AskPartFamilyCharacterization,
     W24AskProductPMIExtract,
     W24AskRevisionTable,
```

### Comparing `werk24-1.8.3/werk24/models/base_feature.py` & `werk24-1.9.0/werk24/models/base_feature.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/bom_table.py` & `werk24-1.9.0/werk24/models/bom_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/chamfer.py` & `werk24-1.9.0/werk24/models/chamfer.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/depth.py` & `werk24-1.9.0/werk24/models/depth.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 
 
 class W24DepthThroughType(str, Enum):
     """Through Type specified on ASME drawings.
     """
     THRU = "THRU"
     THRU_ALL = "THRU_ALL"
+
+
 class W24Depth(BaseModel):
     """ Depth object that describes the details of the
     depth of a drilling or thread
 
     Attributes:
         blurb: String for human consumption
 
         depth: Depth of the drilling or thread in the units
             of the parent object
     """
     blurb: str
 
-    depth: Decimal
+    depth: Optional[Decimal] = None
 
     through_type: Optional[W24DepthThroughType] = None
```

### Comparing `werk24-1.8.3/werk24/models/feature/base.py` & `werk24-1.9.0/werk24/models/feature/base.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/feature/knurl.py` & `werk24-1.9.0/werk24/models/feature/knurl.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/file_format.py` & `werk24-1.9.0/werk24/models/file_format.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/font.py` & `werk24-1.9.0/werk24/models/font.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/gdt.py` & `werk24-1.9.0/werk24/models/gdt.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/general_tolerances.py` & `werk24-1.9.0/werk24/models/general_tolerances.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,25 +153,25 @@
     """Tolerance Class which matches an individual attribute
     of the General Tolerances to a tolerance property and
     tolerance table
 
     Attributes:
         blurb: Tolerance class label for human consumption
 
-        raw_ocr_blurb: Tolerance note text as annotated on 
+        raw_ocr_blurb: Tolerance note text as annotated on
             the drawing.
 
         property: Property that is being tolerated
 
         table: Rows of the tolerance table that correspond
             to the selected tolerance class
     """
 
     blurb: str
-    raw_ocr_blurb: str
+    raw_ocr_blurb: str = ""
     property: W24ToleranceProperty
     table: List[W24ToleranceTableItem]
 
 
 class W24GeneralTolerances(W24BaseFeatureModel):
     """
     General Tolerances on the Title Block of the Technical Drawing.
```

### Comparing `werk24-1.8.3/werk24/models/geometric_shape.py` & `werk24-1.9.0/werk24/models/geometric_shape.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/helpdesk.py` & `werk24-1.9.0/werk24/models/helpdesk.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/hole_feature.py` & `werk24-1.9.0/werk24/models/hole_feature.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/leader.py` & `werk24-1.9.0/werk24/models/leader.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/location.py` & `werk24-1.9.0/werk24/models/location.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/material.py` & `werk24-1.9.0/werk24/models/material.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/measure.py` & `werk24-1.9.0/werk24/models/measure.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/note.py` & `werk24-1.9.0/werk24/models/note.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/paper_size.py` & `werk24-1.9.0/werk24/models/paper_size.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/part_family.py` & `werk24-1.9.0/werk24/models/part_family.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/physical_quantity.py` & `werk24-1.9.0/werk24/models/physical_quantity.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/property/abbe_number.py` & `werk24-1.9.0/werk24/models/property/abbe_number.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,44 +13,64 @@
         discriminators = ("abbe_tolerance_type",)
 
     blurb: str
     abbe_tolerance_type: Any
 
 
 class W24PropertyAbbeToleranceValue(W24PropertyAbbeTolerance):
+    """ Abbe Tolerance Value """
     abbe_tolerance_type: Literal["VALUE"] = "VALUE"
     blurb: str = Field(examples=["±0.8%"])
-    deviation_upper: Optional[Decimal] = Field(examples=[Decimal("0.8")])
-    deviation_lower: Optional[Decimal] = Field(examples=[Decimal("-0.8")])
+    deviation_upper: Optional[Decimal] = Field(
+        examples=[Decimal("0.8")], default=None)
+    deviation_lower: Optional[Decimal] = Field(
+        examples=[Decimal("-0.8")], default=None)
 
 
 class W24PropertyAbbeToleranceStep(W24PropertyAbbeTolerance):
+    """ Abbe Tolerance Step """
     abbe_tolerance_type: Literal["STEP"] = "STEP"
     blurb: str = Field(examples=["Step 3", "Step 0.5"])
     step: Decimal = Field(examples=[Decimal("3"), Decimal("0.5")])
 
 
+class W24PropertyAbbeToleranceFreeText(W24PropertyAbbeTolerance):
+    """ Abbe Tolerance Free Text """
+    free_text: str
+    variation_type: Literal["FREETEXT"] = "FREETEXT"
+
+
 W24PropertyAbbeToleranceType = Union[
-    W24PropertyAbbeToleranceValue, W24PropertyAbbeToleranceStep
+    W24PropertyAbbeToleranceValue,
+    W24PropertyAbbeToleranceStep,
+    W24PropertyAbbeToleranceFreeText,
 ]
 
 
 class W24PropertyAbbeValue(W24Property):
     property_type: Literal["ABBE_NUMBER"] = "ABBE_NUMBER"
 
 
 class W24PropertyAbbeValueNumberValue(W24PropertyAbbeValue):
+    """ Abbe Value Number """
     property_subtype: Literal["VALUE"] = "VALUE"
 
     blurb: str = Field(examples=["vd = 34.70 ±0.8%", "ve = 57.27 ±0.5%"])
 
-    line: Optional[W24FraunhoferLine] = Field(
-        examples=[
-            W24FraunhoferLine.D_LINE,
-            W24FraunhoferLine.E_LINE,
-        ],
-    )
-    value: Optional[Decimal] = Field(examples=[Decimal("34.70")])
-    tolerance: Optional[W24PropertyAbbeToleranceType]
-
-
-W24PropertyAbbeValueType = W24PropertyAbbeValueNumberValue
+    line: Optional[W24FraunhoferLine] = Field(examples=[
+        W24FraunhoferLine.D_LINE,
+        W24FraunhoferLine.E_LINE,
+    ], default=None)
+    value: Optional[Decimal] = Field(examples=[Decimal("34.70")], default=None)
+    tolerance: Optional[W24PropertyAbbeToleranceType] = Field(default=None)
+
+
+class W24PropertyAbbeValueFreeText(W24PropertyAbbeValue):
+    """ Abbe Value Free Text """
+    free_text: str
+    variation_type: Literal["FREETEXT"] = "FREETEXT"
+
+
+W24PropertyAbbeValueType = Union[
+    W24PropertyAbbeValueNumberValue,
+    W24PropertyAbbeValueFreeText,
+]
```

### Comparing `werk24-1.8.3/werk24/models/property/bubbles_and_inclusions.py` & `werk24-1.9.0/werk24/models/property/bubbles_and_inclusions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 from decimal import Decimal
-from typing import Literal, Union
+from typing import Literal, Union, Optional
 
 from pydantic import Field
 
 from werk24.models.property.base import W24Property
 from werk24.models.value import W24PhysicalQuantity, ureg
 
 
 class W24PropertyBubblesAndInclusions(W24Property):
-    """Parent for all Glas Homogeneity Properties"""
+    """Parent for all Bubbles and Inclusions Properties"""
 
     property_type: Literal["BUBBLES_AND_INCLUSIONS"] = "BUBBLES_AND_INCLUSIONS"
 
 
-class W24PropertyBubblesAndInclusionSchottGrade(W24PropertyBubblesAndInclusions):
+class W24PropertyBubblesAndInclusionsSchottGrade(W24PropertyBubblesAndInclusions):
+    """Bubbles and Inclusions Schott Grade"""
+
     property_subtype: Literal["SCHOTT_GRADE"] = "SCHOTT_GRADE"
     blurb: str = Field(examples=["Standard", "VB", "EVB"])
     grade: str = Field(examples=["Standard", "VB", "EVB"])
 
 
-class W24PropertyBubblesAndInclusionIso10110Grade(W24PropertyBubblesAndInclusions):
+class W24PropertyBubblesAndInclusionsIso10110Grade(W24PropertyBubblesAndInclusions):
+    """Bubbles and Inclusions ISO 10110 Grade"""
+
     property_subtype: Literal["ISO_10110_GRADE"] = "ISO_10110_GRADE"
     blurb: str = Field(examples=["1/3 x 0.5"])
     number_of_largest_permissible_bubbles: int = Field(examples=[3])
     largest_permissible_bubble_grade: Decimal = Field(examples=[Decimal("0.5")])
 
 
 class W24PropertyBubblesAndInclusionsIso10110Limits(W24PropertyBubblesAndInclusions):
+    """Bubbles and Inclusions ISO 10110 Limits"""
+
     property_subtype: Literal["ISO_10110_LIMITS"] = "ISO_10110_LIMITS"
     blurb: str = Field(examples=["30/100 cm3 & 0.1mm2/100cm3"])
-    number_of_largest_permissible_bubbles: int = Field(examples=[30])
+    number_of_largest_permissible_bubbles: Optional[int] = Field(
+        examples=[30], default=None
+    )
     total_cross_section: W24PhysicalQuantity = Field(
         examples=[W24PhysicalQuantity(blurb="0.1mm2", value=0.1 * ureg.mm**2)]
     )
     test_volume: W24PhysicalQuantity = Field(
         examples=[W24PhysicalQuantity(blurb="100cm3", value=100 * ureg.cm**3)]
     )
 
 
+class W24PropertyBubblesAndInclusionsFreeText(W24PropertyBubblesAndInclusions):
+    """Bubbles and Inclusions Free Text"""
+
+    free_text: str
+    variation_type: Literal["FREETEXT"] = "FREETEXT"
+
+
 W24PropertyBubblesAndInclusionsType = Union[
-    W24PropertyBubblesAndInclusionSchottGrade,
-    W24PropertyBubblesAndInclusionIso10110Grade,
+    W24PropertyBubblesAndInclusionsFreeText,
+    W24PropertyBubblesAndInclusionsIso10110Grade,
     W24PropertyBubblesAndInclusionsIso10110Limits,
+    W24PropertyBubblesAndInclusionsSchottGrade,
 ]
```

### Comparing `werk24-1.8.3/werk24/models/property/cleanness.py` & `werk24-1.9.0/werk24/models/property/cleanness.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/property/color.py` & `werk24-1.9.0/werk24/models/property/color.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/property/corrosion_resistance.py` & `werk24-1.9.0/werk24/models/property/corrosion_resistance.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/property/fraunhofer.py` & `werk24-1.9.0/werk24/models/property/fraunhofer.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/property/glass_homogeneity.py` & `werk24-1.9.0/werk24/models/property/glass_homogeneity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from werk24.models.property.base import W24Property
-from typing import Literal, Union
+from typing import Literal, Union, Optional
 from pydantic import Field, BaseModel
 from decimal import Decimal
 from werk24.models.value import W24PhysicalQuantity, ureg
 
 
 class W24Iso10110Grade(BaseModel):
     """ISO 10110 Grade.
 
     This model contains information about both, the
     homogeneity and the striae and is thus used by
     both models.
     """
 
     blurb: str = Field(examples=["2/3;1"])
-    homogeneity_grade: str = Field(examples=["3"])
-    striae_grade: str = Field(examples=["1"])
+    homogeneity_grade: Optional[str] = Field(examples=["3"], default=None)
+    striae_grade: Optional[str] = Field(examples=["1"], default=None)
 
 
 class W24Iso10110Limits(BaseModel):
     """ISO 10110 Limits for Homogeneity and Wavefront"""
 
     blurb: str = Field(examples=["5* 10^-6; <15nm"])
     tolerance_limit: Decimal = Field(examples=[Decimal(str("50e-6"))])
-    striae_wavefront_deviation_tolerance_limit: W24PhysicalQuantity = Field(
-        examples=[W24PhysicalQuantity(blurb="15nm", value=15 * ureg.nm)]
+    striae_wavefront_deviation_tolerance_limit: Optional[W24PhysicalQuantity] = Field(
+        examples=[W24PhysicalQuantity(blurb="15nm", value=15 * ureg.nm)],
+        default=None
     )
 
 
 class W24PropertyGlasHomogeneity(W24Property):
     # WORKAROUND FOR TYPO
     pass
 
@@ -68,13 +69,21 @@
 
     property_subtype: Literal["ISO_10110_NH_GRADE"] = "ISO_10110_NH_GRADE"
     blurb: str = Field(examples=["NH040"])
     grade: str = Field(examples=["NH040"])
     tolerance_limit: Decimal = Field(examples=[Decimal(str("40e-6"))])
 
 
+class W24PropertyGlassHomogeneityFreeText(W24PropertyGlassHomogeneity):
+    """Homogeneity Free Text"""
+
+    free_text: str
+    variation_type: Literal["FREETEXT"] = "FREETEXT"
+
+
 W24PropertyGlassHomogeneityType = Union[
     W24PropertyGlassHomogeneitySchottGrade,
     W24PropertyGlassHomogeneityIso10110Grade,
     W24PropertyGlassHomogeneityIso10110ToleranceLimit,
     W24PropertyGlassHomogeneityIso10110NhGrade,
+    W24PropertyGlassHomogeneityFreeText,
 ]
```

### Comparing `werk24-1.8.3/werk24/models/property/hardness.py` & `werk24-1.9.0/werk24/models/property/hardness.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/property/material.py` & `werk24-1.9.0/werk24/models/property/material.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/property/refractive_index.py` & `werk24-1.9.0/werk24/models/property/refractive_index.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 
     refractive_tolerance_type: Any
 
 
 class W24PropertyRefractiveToleranceValue(W24PropertyRefractiveTolerance):
     refractive_tolerance_type: Literal["VALUE"] = "VALUE"
     blurb: str = Field(examples=["±0.0005"])
-    deviation_upper: Optional[Decimal] = Field(examples=[Decimal("0.0005")])
-    deviation_lower: Optional[Decimal] = Field(examples=[Decimal("-0.0005")])
+    deviation_upper: Optional[Decimal] = Field(
+        examples=[Decimal("0.0005")], default=None)
+    deviation_lower: Optional[Decimal] = Field(
+        examples=[Decimal("-0.0005")], default=None)
 
 
 class W24PropertyRefractiveToleranceStep(W24PropertyRefractiveTolerance):
     refractive_tolerance_type: Literal["STEP"] = "STEP"
     blurb: str = Field(examples=["Step 3", "Step 0.5"])
     step: Decimal = Field(examples=[Decimal("3"), Decimal("0.5")])
 
@@ -38,53 +40,77 @@
     class Config:
         discriminators = ("variation_type",)
 
     variation_type: Any
 
 
 class W24PropertyRefractiveVariationSchottGrade(W24PropertyRefractiveVariation):
+    """ Refractive Variation Schott Grade """
     variation_type: Literal["SCHOTT_GRADE"] = "SCHOTT_GRADE"
     blurb: str = Field(examples=("LN", "LH1", "LH2"))
     grade: str = Field(examples=["LN", "LH1", "LH2"])
 
 
 class W24PropertyRefractiveVariationIso12123(W24PropertyRefractiveVariation):
+    """ Refractive Variation ISO 12123 """
     variation_type: Literal["ISO_12123"] = "ISO_12123"
     blurb: str = Field(examples=("NV20", "NV10", "NV05"))
     grade: str = Field(examples=["NV20", "NV10", "NV05"])
 
 
+class W24PropertyRefractiveVariationFreeText(W24PropertyRefractiveVariation):
+    """ Refractive Variation Free Text """
+    free_text: str
+    variation_type: Literal["FREETEXT"] = "FREETEXT"
+
+
 W24PropertyRefractiveVariationType = Union[
     W24PropertyRefractiveVariationSchottGrade,
     # W24PropertyRefractiveVariationIso12123
     None,
+    W24PropertyRefractiveVariationFreeText,
 ]
 
 
 class W24PropertyRefractiveIndex(W24Property):
+    """ Parent for all Refractive Index """
     property_type: Literal["REFRACTIVE_INDEX"] = "REFRACTIVE_INDEX"
 
 
 class W24PropertyRefractiveIndexValue(W24PropertyRefractiveIndex):
+    """ Refractive Index Value """
     property_subtype: Literal["VALUE"] = "VALUE"
 
     blurb: str = Field(
         examples=[
             "nd = 1.72047 ±0.0005",
             "ne = 1.57487 ±0.0005",
         ]
     )
 
     line: Optional[W24FraunhoferLine] = Field(
         examples=[
             W24FraunhoferLine.D_LINE,
             W24FraunhoferLine.E_LINE,
-        ]
+        ],
+        default=None
     )
     value: Decimal = Field(examples=[Decimal("1.72047")])
-    tolerance: Optional[W24PropertyRefractiveToleranceType]
+    tolerance: Optional[W24PropertyRefractiveToleranceType] = Field(
+        default=None)
     variation: Optional[W24PropertyRefractiveVariationType] = Field(
-        examples=[W24PropertyRefractiveVariationSchottGrade(blurb="NV20", grade="NV20")]
+        examples=[W24PropertyRefractiveVariationSchottGrade(
+            blurb="NV20", grade="NV20")],
+        default=None
     )
 
 
-W24PropertyRefractiveIndexType = W24PropertyRefractiveIndexValue
+class W24PropertyRefractiveIndexFreeText(W24PropertyRefractiveIndex):
+    """ Refractive Index Free Text """
+    free_text: str
+    variation_type: Literal["FREETEXT"] = "FREETEXT"
+
+
+W24PropertyRefractiveIndexType = Union[
+    W24PropertyRefractiveIndexValue,
+    W24PropertyRefractiveIndexFreeText,
+]
```

### Comparing `werk24-1.8.3/werk24/models/property/stress_birefringence.py` & `werk24-1.9.0/werk24/models/property/stress_birefringence.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,31 @@
 
 class W24PropertyStressBirefringenceIso10110Value(W24PropertyStressBirefringence):
     """ISO 10110 Stress Birefringence Value"""
 
     property_subtype: Literal["ISO_10110_VALUE"] = "ISO_10110_VALUE"
     blurb: str = Field(examples=["0/8"])
     value: W24PhysicalQuantity = Field(
-        examples=[W24PhysicalQuantity(blurb="8nm/cm", value=8 * ureg.nm / ureg.cm)]
+        examples=[W24PhysicalQuantity(
+            blurb="8nm/cm", value=8 * ureg.nm / ureg.cm)]
     )
 
 
 class W24PropertyStressBirefringenceIso10110Grade(W24PropertyStressBirefringence):
     """ISO 10110 Stress Birefringence Grade"""
 
     property_subtype: Literal["ISO_10110_GRADE"] = "ISO_10110_GRADE"
     blurb: str = Field(examples=["SB20", "SB02"])
     grade: str = Field(examples=["SB20", "SB02"])
 
 
+class W24PropertyStressBirefringenceFreeText(W24PropertyStressBirefringence):
+    """Stress Birefringence Free Text"""
+    free_text: str
+    variation_type: Literal["FREETEXT"] = "FREETEXT"
+
+
 W24PropertyStressBirefringenceType = Union[
     W24PropertyStressBirefringenceIso10110Value,
     W24PropertyStressBirefringenceIso10110Grade,
+    W24PropertyStressBirefringenceFreeText,
 ]
```

### Comparing `werk24-1.8.3/werk24/models/property/striae.py` & `werk24-1.9.0/werk24/models/property/striae.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,27 +59,35 @@
     """Striae Grade following ISO 12123"""
 
     property_subtype: Literal["ISO_12123"] = "ISO_12123"
     blurb: str = Field(examples=["SW60", "SW10"])
     grade: str = Field(examples=["SW60", "SW10"])
 
 
+class W24PropertyStriaeFreeText(W24PropertyStriae):
+    """Striae Free Text"""
+
+    free_text: str
+    variation_type: Literal["FREETEXT"] = "FREETEXT"
+
 # class W24PropertyStriaeMilG174B(W24PropertyStriae):
 #     """
 #     Striae Grade following MIL G 174 B.
 
 #     The MIL-G-174 B categorizes striae in a piece of raw
 #     glass according to its intensity but without any
 #     reference to the striae area and sample thickness.
 #     The striae are categorized by four reference samples
 #     of cord-like striae into four classes A to D.
 #     (See SCHOTT TIE 25)
 #     """
 
+
 #     property_subtype: Literal["MIL_G_1748_B"] = "MIL_G_1748_B"
 #     grade: str
 W24PropertyStriaeType = Union[
     W24PropertyStriaeSchottGrade,
     W24PropertyStriaeIso10110Grade,
     W24PropertyStriaeIso10110Limits,
     W24PropertyStriaeIso12123,
+    W24PropertyStriaeFreeText,
 ]
```

### Comparing `werk24-1.8.3/werk24/models/property/surface_area.py` & `werk24-1.9.0/werk24/models/property/surface_area.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/property/weight.py` & `werk24-1.9.0/werk24/models/property/weight.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/radius.py` & `werk24-1.9.0/werk24/models/radius.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/revision_table.py` & `werk24-1.9.0/werk24/models/revision_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/roughness.py` & `werk24-1.9.0/werk24/models/roughness.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,119 +6,130 @@
 from pydantic import UUID4, BaseModel
 
 from .base_feature import W24BaseFeatureModel
 from .unit import W24UnitSystem
 
 
 class W24RoughnessStandard(str, Enum):
-    """ Most standards that define the surface roughness use
+    """Most standards that define the surface roughness use
     very similar symbols. However, the position of the fields
     varies.
 
     The standards listed here are understood and supported
     by the API.
 
     NOTE: the ISO 1302 standard exists in four different versions,
     these releases substantially modified the position and
     structure of the roughness symbols.
 
     NOTE: this list is not exhaustive, many countries have specified
     their own standards over the years. Do not hesitate to reach
     out if you wish us to implement another standard.
 
+    NOTE: REFERENCE is a special value that is used when the
+    drawing specified a reference roughness. For example: w√.
+
     """
+
     ISO_1302_1978 = "ISO 1302:1978"
     ISO_1302_1992 = "ISO 1302:1992"
     ISO_1302_2002 = "ISO 1302:2002"
     ISO_21920_1_2021 = "ISO 21920-1:2021"
     ASME_Y14_36_1978 = "ASME Y14.36-1978"
     ASME_Y14_36M_1996 = "ASME Y14.36M-1996"
     ASME_Y14_36_2018 = "ASME Y14.36-2018"
+    REFERENCE = "REFERENCE"
 
 
 class W24RoughnessMaterialRemovalType(str, Enum):
-    """ Most standard allow the designer to specify
+    """Most standard allow the designer to specify
     whether material removal is required or prohibited.
 
     By default both options are allowed.
     """
+
     UNSPECIFIED = "UNSPECIFIED"
     PROHIBITED = "PROHIBITED"
     REQUIRED = "REQUIRED"
 
 
 class W24RoughnessDirectionOfLay(str, Enum):
-    """ The lay of the roughness limits the
+    """The lay of the roughness limits the
     manufacturing process and is sometimes
     required for the application.
     """
+
     PARALLEL = "="
     PERPENDICULAR = "⟂"
     CROSS = "X"
     MULTIDIRECTIONAL = "M"
     CIRCULAR = "C"
     RADIAL = "R"
     PROTUBERANT = "P"
 
 
 class W24RoughnessAcceptanceCriterion(str, Enum):
-    """ The designer can specify whether to apply
+    """The designer can specify whether to apply
     the 16%-rule, the maximum- or medium- rule
     when deciding whether a surface complies with
     the specifications.
     """
+
     SIXTEEN_PERCENT = "16%"
     MAXIMUM = "max"
     MEAN = "mean"
 
 
 class W24RoughnessConditionType(str, Enum):
-    """ Roughnesses can specify, the
+    """Roughnesses can specify, the
     upper limit, the lower limit and the
     average.
     """
+
     UPPER = "U"
     LOWER = "L"
     AVERAGE = "A"
 
 
 class W24RoughnessFilterType(str, Enum):
-    """ When measuring the roughness, different
+    """When measuring the roughness, different
     filter types will result in different results.
     To reduce this source of ambiguity, the
     designer can specify the filter to be used.
 
     NOTE: this list is not exhaustive. If you
     need us to support another filter method,
     please reach out.
     """
+
     GAUSSIAN = "G"
     ROBUST_GAUSSIAN = "RG"
     SPLINE = "S"
-    TWO_RC = "\"2RC\""
+    TWO_RC = '"2RC"'
 
 
 class W24RoughnessGrade(BaseModel):
-    """ ISO Roughness Grade
+    """ISO Roughness Grade
 
     Attributes:
         blurb: String representation for human consumption
 
         grade: Roughness Grade in the range N01 to N12.
             Valid values are N01, N0, N1, N2, N3, N4, N5,
             N6, N7, N8, N9, N10, N11, N12, N13, N14
 
     """
+
     blurb: str
 
     grade: str
 
 
 class W24RoughnessParameter(str, Enum):
-    """ Roughness Parameter that is specified.
+    """Roughness Parameter that is specified.
 
     NOTE: this list is not exhaustive, but
     covers the most frequently used parameters.
     """
 
     # ASME
     AA = "AA"
@@ -169,15 +180,15 @@
 
 class W24RoughnessEvaluationLengthType(str, Enum):
     LENGTH = "LENGTH"
     LAMBDA_C_MULTIPLE = "LAMBDA_C_MULTIPLE"
 
 
 class W24RoughnessEvaluationLength(BaseModel):
-    """ For sophisticated application, the sample needs
+    """For sophisticated application, the sample needs
     to be taken over a longer distances. This is specified the
     either the sampling length in millimeter (ISO 3012:1974,
     ISO 3012:1978, ISO 3012:1992) or as multiple of the main lambda
     (ISO 3012:2002 and ISO 3012:2021).
 
 
     Attributes:
@@ -187,24 +198,25 @@
         length: evaluation length in the specified units.
 
         length_unit: Millimeter for both the ISO and ASME standards
 
         lambda_c_multiple: multiple of the main cutoff lambda_c
 
     """
+
     evaluation_length_type: W24RoughnessEvaluationLengthType
 
     length: Optional[Decimal]
     length_unit: Optional[W24UnitLength]
 
     lambda_c_multiple: Optional[Decimal]
 
 
 class W24RoughnessCondition(BaseModel):
-    """ Roughness Label
+    """Roughness Label
 
     Attributes:
         blurb: String representation of the Roughness for human
             consumption.
 
         condition_type: Roughness Side that is specified (upper or lower).
             We automatically determine this value depending on
@@ -241,14 +253,15 @@
         value_limit: Specification limit
 
         roughness_grade: ISO roughness grade that the roughness specifications
             correspond to. IMPORTANT: this allows you to deal with
             all the standards in a simple way.
 
     """
+
     blurb: str
 
     condition_type: Optional[W24RoughnessConditionType]
 
     filter_type: Optional[W24RoughnessFilterType]
 
     lambda_s: Optional[Decimal]
@@ -263,37 +276,39 @@
 
     value: Optional[Decimal]
 
     roughness_grade: Optional[W24RoughnessGrade]
 
 
 class W24ManufacturingMethod(BaseModel):
-    """ Manufacturing method specified on the drawing.
+    """Manufacturing method specified on the drawing.
     Currently only the blurb is available.
 
     Attributes:
         blurb: Manufacturing method as specified on the
             drawing
     """
+
     blurb: str
 
 
 class W24RoughnessWaviness(BaseModel):
-    """ Roughness Waviness as defined in the ASME-Y14-36
+    """Roughness Waviness as defined in the ASME-Y14-36
 
     Attributes:
         waviness_height: Waviness height in inch
         waviness_width: Waviness width in inch
     """
+
     waviness_height: Decimal
     waviness_width: Decimal
 
 
 class W24RoughnessLabel(BaseModel):
-    """ Roughness Label
+    """Roughness Label
 
     Attributes:
         blurb: String for human consumption
 
         blurb_html: HTML for human consumption. The complex structure of the
             symbol makes this necessary.
 
@@ -318,15 +333,18 @@
 
         unit_system: Unit system that is used for the roughness.
             We are not using the explicit units as the different
             attributes have different units (e.g, micro and nano meters)
 
         waviness: Waviness defined in ASME standards
 
+        variable: Roughness variable that is used in roughness references.
+
     """
+
     blurb: str
 
     blurb_html: str
 
     standard: W24RoughnessStandard
 
     machining_allowance: Optional[Decimal]
@@ -341,19 +359,66 @@
 
     conditions: List[W24RoughnessCondition]
 
     unit_system: W24UnitSystem
 
     waviness: Optional[W24RoughnessWaviness]
 
+    variable: Optional[str] = None
+
 
 class W24Roughness(W24BaseFeatureModel):
-    """ Roughness object
+    """Roughness object
 
     Attributes:
         roughness_id: Unique UUID4 identifier
 
         label: RoughnessLabel
     """
-    roughness_id: UUID4
 
+    roughness_id: UUID4
     label: W24RoughnessLabel
+
+
+class W24RoughnessReference(W24BaseFeatureModel):
+    """Roughness Reference
+
+    Attributes:
+    ----------
+    blurb: String for human consumption
+
+    reference_label: Placeholder for the roughness.
+        We are using a reference label here to allow
+        the full scope of the roughness to be specified.
+        Sometimes we see a pure "material removal not
+        permitted" symbol as placeholder.
+
+    reference_value: Meaning of the roughness_label,
+        explaining what surface roughness is applicable
+        when the roughness_label is specified on a
+        workpiece.
+
+    """
+
+    blurb: str
+    reference_label: W24RoughnessLabel
+    reference_value: W24RoughnessLabel
+
+
+class W24GeneralRoughness(W24BaseFeatureModel):
+    """General Roughness object
+
+    Attributes:
+    ----------
+    blurb: String for human consumption
+
+    general_roughnesses: Surface Roughness Specification
+        required for all surfaces of a workpiece. Unless
+        any deviation is specified.
+
+    deviating_roughnesses: Indicates deviations from
+        the general surface roughness requirements.
+    """
+
+    blurb: str
+    general_roughnesses: List[W24RoughnessLabel]
+    deviating_roughnesses: List[W24RoughnessLabel]
```

### Comparing `werk24-1.8.3/werk24/models/size.py` & `werk24-1.9.0/werk24/models/size.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/techread.py` & `werk24-1.9.0/werk24/models/techread.py`

 * *Files 3% similar despite different names*

```diff
@@ -333,7 +333,26 @@
     # in use. This configuration at least suppresses the warning.
     # See https://docs.pydantic.dev/latest/api/config/#pydantic.config.ConfigDict.protected_namespaces
     model_config = ConfigDict(protected_namespaces=())
 
     drawing_presigned_post: W24PresignedPost
 
     model_presigned_post: W24PresignedPost
+
+
+class W24TechreadWithCallbackPayload(BaseModel):
+    """Payload that is sent to the API to trigger a read with callback.
+
+    Attributes:
+    ----------
+    asks: List of asks
+
+    callback_url: Callback URL that will be called once the
+        processing is completed.
+
+    max_pages: Maximum number of pages that shall be processed.
+    """
+
+    asks: List[W24AskUnion] = []
+    callback_url: HttpUrl
+    max_pages: int = 5
+    drawing_filename: Optional[str] = None
```

### Comparing `werk24-1.8.3/werk24/models/test_dimension.py` & `werk24-1.9.0/werk24/models/test_dimension.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/thread.py` & `werk24-1.9.0/werk24/models/thread.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/thread_element.py` & `werk24-1.9.0/werk24/models/thread_element.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/title_block.py` & `werk24-1.9.0/werk24/models/title_block.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from werk24.models.property.color import W24PropertyColor
 
 from .base_feature import W24BaseFeatureModel
 from .general_tolerances import W24GeneralTolerances
 from .language import W24Language
 from .material import W24Material
 from .weight import W24Weight
+from .roughness import W24GeneralRoughness, W24RoughnessReference
 
 
 class W24TitleBlockItem(W24BaseFeatureModel):
     """Per-Language caption or value
 
     Attributes:
 
@@ -46,15 +47,16 @@
 
     captions: List[W24TitleBlockItem]
     values: List[W24TitleBlockItem]
 
 
 class W24IdentifierType(str, Enum):
     """List of Identifier Types supported by Werk24"""
-    ASSEMBLY_NAME  = "ASSEMBLY_NAME "
+
+    ASSEMBLY_NAME = "ASSEMBLY_NAME "
     ASSEMBLY_NUMBER = "ASSEMBLY_NUMBER"
     CAGE_CODE = "CAGE_CODE"
     CONTRACT_NUMBER = "CONTRACT_NUMBER"
     CUSTOMER_NAME = "CUSTOMER_NAME"
     CUSTOMER_NUMBER = "CUSTOMER_NUMBER"
     DOCUMENT_NUMBER = "DOCUMENT_NUMBER"
     DRAWING_NUMBER = "DRAWING_NUMBER"
@@ -63,37 +65,43 @@
     ITEM_NUMER = "ITEM_NUMER"
     MANUFACTURER_NAME = "MANUFACTURER_NAME"
     MANUFACTURER_NUMBER = "MANUFACTURER_NUMBER"
     NUMBER = "NUMBER"
     ORDER_NAME = "ORDER_NAME"
     ORDER_NUMBER = "ORDER_NUMBER"
 
+
 class W24IdentifierStakeholder(str, Enum):
     """List of Stakeholders that can be identified by Werk24"""
+
     SUPPLIER = "SUPPLIER"
     OWNER = "OWNER"
     CUSTOMER = "CUSTOMER"
 
+
 class W24IdentifierPeriod(str, Enum):
     """List of Period Identifiers that can be identified by Werk24"""
+
     PREVIOUS = "PREVIOUS"
     CURRENT = "CURRENT"
     FUTURE = "FUTURE"
 
+
 class W24IdentifierPair(W24CaptionValuePair):
     """Caption-Value Pair for Identifies
 
     Attributes:
         identifier_type (W24IdentifierType) Type of identifier.
     """
 
     identifier_type: W24IdentifierType
     stakeholder: Optional[W24IdentifierStakeholder] = None
     period: Optional[W24IdentifierPeriod] = None
 
+
 class W24FileExtensionType(str, Enum):
     """
     Enum of the extension types.
 
     For example, pdf and idw extensions will be mapped to
     DRAWING, while step and stl extensions will be mapped
     to MODEL.
@@ -192,14 +200,20 @@
 
         colors: List of colors detected on the TitleBlock or in the
             canvas notes.
 
         bom_table: Reference to the Bill of Material Table. None
             if you are running on an old client or when no BOM
             table was found.
+
+        general_roughnesses (List[W24GeneralRoughness]): List of the detected
+            general roughnesses.
+
+        reference_roughnesses (List[W24RoughnessReference]): List of the
+            detected reference roughnesses.
     """
 
     designation: Optional[W24CaptionValuePair]
 
     drawing_id: Optional[W24CaptionValuePair]
     part_ids: List[W24CaptionValuePair] = []
     reference_ids: List[W24IdentifierPair] = []
@@ -213,107 +227,10 @@
 
     filename_drawing: Optional[W24Filename] = None
 
     colors: List[W24PropertyColor] = []
 
     bom_table: Optional[W24BomTable] = None
 
-    @validator("designation", pre=True)
-    def designation_validator(
-        cls, raw: Dict[str, Any]
-    ) -> Optional[W24CaptionValuePair]:
-        """
-        Workaround to deal with the transition period
-        while we move from the single-value to the multi-value
-        pairs.
-
-        This code can be removed after we complete the
-        transition.
-
-        Args:
-
-            raw (Dict[str, Any]): Unparsed value returned
-                from the API
-
-        Returns:
-
-            W24CaptionValuePair: Parse value-caption pair
-        """
-        return cls._parse_caption_value_pair(raw)
-
-    @validator("drawing_id", pre=True)
-    def drawing_id_validator(cls, raw: Dict[str, Any]) -> Optional[W24CaptionValuePair]:
-        """
-        Workaround to deal with the transition period
-        while we move from the single-value to the multi-value
-        pairs.
-
-        This code can be removed after we complete the
-        transition.
-
-        Args:
-
-            raw (Dict[str, Any]): Unparsed value returned
-                from the API
-
-        Returns:
-
-            W24CaptionValuePair: Parse value-caption pair
-        """
-        return cls._parse_caption_value_pair(raw)
-
-    @validator("reference_ids", pre=True)
-    def reference_ids_validator(
-        cls, raw: List[Dict[str, Any]]
-    ) -> List[W24CaptionValuePair]:
-        """
-        Workaround to deal with the transition period
-        while we move from the single-value to the multi-value
-        pairs.
-
-        This code can be removed after we complete the
-        transition.
-
-        Args:
-
-            raw (List[Dict[str, Any]]): Unparsed value returned
-                from the API
-
-        Returns:
-
-            List[W24CaptionValuePair]: Parse value-caption pair
-        """
-        result = [cls._parse_caption_value_pair(e) for e in raw]
-        return [r for r in result if r is not None]
-
-    @staticmethod
-    def _parse_caption_value_pair(
-        raw: Optional[Dict[str, Any]]
-    ) -> Optional[W24CaptionValuePair]:
-        """
-        Workaround to deal with the transition period
-        while we move from the single-value to the multi-value
-        pairs.
-
-        This code can be removed after we complete the
-        transition.
-
-        Args:
-
-            raw (Dict[str, Any]): Unparsed value returned
-                from the API
-
-        Returns:
-
-            W24CaptionValuePair: Parse value-caption pair
-        """
-        if isinstance(raw, W24CaptionValuePair):
-            return raw
-
-        if raw is None:
-            return None
-
-        if "value" in raw.keys():
-            raw["values"] = [{"language": None, "text": raw.get("value")}]
-            del raw["value"]
+    general_roughnesses: List[W24GeneralRoughness] = []
 
-        return W24CaptionValuePair.parse_obj(raw)
+    reference_roughnesses: List[W24RoughnessReference] = []
```

### Comparing `werk24-1.8.3/werk24/models/tolerance.py` & `werk24-1.9.0/werk24/models/tolerance.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/typed_model.py` & `werk24-1.9.0/werk24/models/typed_model.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/unit.py` & `werk24-1.9.0/werk24/models/unit.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/value.py` & `werk24-1.9.0/werk24/models/value.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/view.py` & `werk24-1.9.0/werk24/models/view.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/models/weight.py` & `werk24-1.9.0/werk24/models/weight.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24/techread_client.py` & `werk24-1.9.0/werk24/techread_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,50 +12,50 @@
     # obtain the thumbnail of a page
     drawing_bytes = open(...,"r").read()
     client = W24TechreadClient.make_from_env()
     await client.read_drawing_with_hooks(
         drawing_bytes,
         [Hook(
                 ask=W24AskPageThumbnail(),
-                callback=lambda msg: print("Received Thumbnail of Page")
+                function=lambda msg: print("Received Thumbnail of Page")
         ]))
 """
 import logging
+from io import BufferedReader
 import os
 import uuid
-from asyncio import gather, iscoroutinefunction
+from asyncio import iscoroutinefunction
 from types import TracebackType
 from typing import (
     AsyncGenerator,
     AsyncIterator,
     Callable,
     Dict,
     List,
     Optional,
     Type,
     Union,
     Tuple,
 )
+from werk24.auth_client import AuthClient
 
 import dotenv
 from pydantic import UUID4, BaseModel
 
-from werk24.auth_client import AuthClient
 from werk24.exceptions import (
     BadRequestException,
     LicenseError,
     RequestTooLargeException,
     ServerException,
     UnsupportedMediaType,
 )
 from werk24.models.ask import W24Ask
 from werk24.models.helpdesk import W24HelpdeskTask
 from werk24.models.techread import (
     W24TechreadAction,
-    W24TechreadBaseResponse,
     W24TechreadException,
     W24TechreadExceptionLevel,
     W24TechreadExceptionType,
     W24TechreadInitResponse,
     W24TechreadMessage,
     W24TechreadMessageSubtype,
     W24TechreadMessageType,
@@ -63,85 +63,86 @@
 )
 from werk24.techread_client_https import TechreadClientHttps
 from werk24.techread_client_wss import TechreadClientWss
 
 # make the logger
 logger = logging.getLogger("w24_techread_client")
 
-ENVIRONS = [
-    "W24TECHREAD_VERSION",
-    "W24TECHREAD_AUTH_CLIENT_ID",
-    "W24TECHREAD_AUTH_CLIENT_SECRET",
-    "W24TECHREAD_AUTH_IDENTITY_POOL_ID",
-    "W24TECHREAD_AUTH_USER_POOL_ID",
-    "W24TECHREAD_AUTH_USERNAME",
-    "W24TECHREAD_AUTH_PASSWORD",
-    "W24TECHREAD_AUTH_REGION",
-]
-""" List of the environment variables used by the
-client """
-
 
 EXCEPTION_MAP = {
     RequestTooLargeException: W24TechreadExceptionType.DRAWING_FILE_SIZE_TOO_LARGE,
     BadRequestException: W24TechreadExceptionType.DRAWING_FILE_SIZE_TOO_LARGE,
 }
 """ Map to translate the local exceptions to official
 W24Exceptions. This allows us to mock consistent responses
 even when the files are rejected before they reach the API
 """
 
+# Default Authentication Region
 DEFAULT_AUTH_REGION = "eu-central-1"
+
+# Default Endpoints
 DEFAULT_SERVER_WSS = "ws-api.w24.co"
-DEFAULT_SUPPORT_BASE_URL = "support.w24.co"
+DEFAULT_SERVER_HTTPS = "support.w24.co"
 
+# List of the Locations where we are looking for the license file
+# if the user does not specify a path.
 LICENSE_LOCATIONS = (".werk24", "werk24_license.txt")
 
 LICENSE_ERROR_TEXT = """
+--------------------------------------------------------------------------------
 
-////////////////////////////////////////////////////////////////////////////////
+####   ####   #### ########### ##########    ####   #####     ##################
+####  #####  ####  ####        ####   #####  ####  ####     #####   #####  #####
+ #### ###### ####  ####        ####    ####  #########     ##### ##  ###   #####
+ #### ###### ####  ##########  ###########   ########      ######## ### #  #####
+  ###### #######   ####        ##########    ##########    ###### ####      ####
+  ######  ######   ####        ####   ####   ####  #####   #####     ####  #####
+   ####   #####    ########### ####    ####  ####   #####  ###################
 
-,.'xWWx'.,kWWd'.;0O,..'',,,,:Ox'..',,'',:lOWNo..:0MXd,.'lKWMNOc'.,;;'....';,....
-l..lXK:...cXKc..oNO,..o0KKKKXNx'.'dKKOc...;0No..;OOc..:kNMMXl'.'oOOOO:..;kKd'...
-k,.,kx'...,kx,.;OMO,..:dddxkXWx'.'xXX0c...:0No..,:,.'oXWMMMO,..,lc;kXl.:kKNk'...
-Xc..:;.;l,.::..lNMO,..,ccccoKWx'..,;,'.';l0WNo.......lKMMMMO,....;x0o,:00ONO;...
-Wk'....dKl....,OMMO,.'dNWWWWWWx'.'okl'.,:xNMNo..'ld:..:OWMMO,..'oKXkl;cxxOWKc...
-MKc...;0WO,...lXMMO,..;oooooxKx'.,OMNd'..,dNNo..;0MKl'.,dNMO,..,oxxddc'..;oc..;x
-MWd'..lNMXl..'xWMMO,........;Ox'.,OMMNo...,kNo..:0MMKc..,xWO,................c0W
-
-////////////////////////////////////////////////////////////////////////////////
-
-Thank you for your interest ist Werk24.
+--------------------------------------------------------------------------------
+Dear Valued Client, We appreciate your interest in Werk24.
 
 _General Information_
-Werk24 is a commercial company focusing on information extraction from
-Technical Documents. The client you are running right now allows you to to
-communicate with our server infrastructure.
+Werk24 is a specialized commercial company dedicated to extracting information
+from technical documents. The python client you are currently using is designed
+to facilitate seamless interaction with our advanced server infrastructure.
 
 _License File_
 We were unable to locate a license file, please schedule a first meeting with
 us to learn about the possibilities of our Technology:
 
 
         >>> https://werk24.io/schedule-a-call?w24cli_license_error <<<
 
 
 Thank you.
-
-////////////////////////////////////////////////////////////////////////////////
+--------------------------------------------------------------------------------
 """
 
 
 class Hook(BaseModel):
-    """Small Object to keep the callback requests.
-    You can either register a callback request to an
-    ask or a message_type.
+    """
+    A Utility class to register callback requests for a specific message_type or W24Ask.
 
-    If you register an ask, be sure to use a complete W24Ask
-    definition; not just the ask type.
+    The 'Hook' object is used for handling and maintaining callback requests. Registering
+    an 'ask' should include a complete W24Ask definition, not just the ask type.
+
+    Attributes:
+    ----------
+    message_type (Optional[W24TechreadMessageType]): Specifies the type of the message.
+    message_subtype (Optional[W24TechreadMessageSubtype]): Specifies the subtype of the message.
+    ask (Optional[W24Ask]): The complete definition of W24Ask, if any.
+    function (Callable): The callback function to be invoked when the resulting information
+        is available.
+
+    Note:
+    ----
+    Either a message_type or an ask must be registered. Be careful when registering an ask;
+    a complete W24Ask definition is required, not just the ask type.
     """
 
     message_type: Optional[W24TechreadMessageType] = None
     message_subtype: Optional[W24TechreadMessageSubtype] = None
     ask: Optional[W24Ask] = None
     function: Callable
 
@@ -153,98 +154,91 @@
     """
 
     def __init__(
         self,
         techread_server_wss: str,
         techread_version: str,
         development_key: str = None,
-        support_base_url: str = DEFAULT_SUPPORT_BASE_URL,
+        support_base_url: str = DEFAULT_SERVER_HTTPS,
     ):
-        """Initialize a new W24TechreadClient. If you wonder
-        about any of the attributes, have a look at the .env
-        file that we provided to you. They contain all the
-        information that you will need.
-
-        Arguments:
-
-            techread_server_wss {str} -- domain name that
-                is being used by the websocket client
+        """Initialize a new W24TechreadClient.
 
-            techread_version {str} -- version that you want to
-                connect to
+        If you wonder about any of the attributes, have a
+        look at the .env file that we provided to you.
+        They contain all the information that you will need.
 
-            development_key {str} -- key that allows you to submit
-                your request to one of the internal architectures.
-                You can try guessing or bruteforcing this key;
-                we'll just charge you for every request you submit and
-                transfer the money to the holiday bonus account.
+        Args:
+        ----
+        techread_server_wss {str} -- domain name that
+            is being used by the websocket client
+
+        techread_version {str} -- version that you want to
+            connect to
+
+        development_key {str} -- key that allows you to submit
+            your request to one of the internal architectures.
+            You can try guessing or bruteforcing this key;
+            we'll just charge you for every request you submit and
+            transfer the money to the holiday bonus account.
         """
-
-        # save the development_key
         self._development_key = development_key
 
         # Create an empty reference to the authentication
-        # service (currently AWS Cognito)
+        # service necessary for the Cognito Authentication.
         self._auth_client: Optional[AuthClient] = None
 
-        # Initialize an instance of the HTTPS client
+        # HTTP Client
         self._techread_client_https = TechreadClientHttps(
-            techread_version, support_base_url
+            techread_version,
+            support_base_url,
         )
 
-        # Initialize an instance of the WEBSOCKET client
+        # WSS Client
         self._techread_client_wss = TechreadClientWss(
             techread_server_wss, techread_version
         )
 
     async def __aenter__(self) -> "W24TechreadClient":
         """Create the HTTPS and WSS sessions
 
         Raises:
-            RuntimeError: Exception is raised if
-                you tried to enter a session before
-                calling the register() method
+        ------
+        RuntimeError: Exception is raised if
+            you tried to enter a session before
+            calling the register() method
 
         Returns:
-            W24TechreadClient -- Version of self with
-                active sessions
+        -------
+        W24TechreadClient -- Version of self with
+            active sessions
         """
-
-        # enter the https session
         await self._techread_client_https.__aenter__()
-
-        # enter the wss session
         await self._techread_client_wss.__aenter__()
-
-        # return the "entered" version of self
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         """Ensure that the sessions are closed"""
-
-        # close the HTTPS session
         await self._techread_client_https.__aexit__(exc_type, exc_value, traceback)
-
-        # close the WSS session
         await self._techread_client_wss.__aexit__(exc_type, exc_value, traceback)
 
     def register(
         self,
-        cognito_region: str,
-        cognito_identity_pool_id: str,
-        cognito_user_pool_id: str,
-        cognito_client_id: str,
-        cognito_client_secret: str,
-        username: str,
-        password: str,
+        cognito_region: Optional[str] = None,
+        cognito_identity_pool_id: Optional[str] = None,
+        cognito_user_pool_id: Optional[str] = None,
+        cognito_client_id: Optional[str] = None,
+        cognito_client_secret: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        token: Optional[str] = None,
     ) -> None:
         """
         Register with the authentication
         service (i.e., lazy login)
 
         Arguments:
             cognito_region {str} -- Physical region
@@ -259,172 +253,153 @@
         # to the authentication service
         self._auth_client = AuthClient(
             cognito_region,
             cognito_identity_pool_id,
             cognito_user_pool_id,
             cognito_client_id,
             cognito_client_secret,
+            username,
+            password,
+            token,
         )
-
-        # register username and password
-        self._auth_client.register(username, password)
-
+        self._auth_client.login()
         # tell the techread clients about it
         self._techread_client_https.register_auth_client(self._auth_client)
         self._techread_client_wss.register_auth_client(self._auth_client)
 
         # ensure that we have a token
         try:
             self._auth_client.login()  # type: ignore
         except AttributeError as exc:
             raise RuntimeError(
                 "No connection to the authentication service was "
                 + "established. Please call register()"
             ) from exc
 
-    @property
-    def username(self) -> Optional[str]:
-        """
-        Make the username accessible to the CLI and GUI.
-
-        Returns:
-            str: username of the currently registered user
-        """
-        if self._auth_client is None:
-            return None
-
-        return self._auth_client.username
-
     async def read_drawing(
         self,
-        drawing: bytes,
+        drawing: Union[BufferedReader, bytes],
         asks: List[W24Ask],
         model: bytes = None,
         max_pages: int = 1,
         drawing_filename: Optional[str] = None,
         sub_account: Optional[UUID4] = None,
     ) -> AsyncIterator[W24TechreadMessage]:
         """
         Send a Technical Drawing to the W24 API to read it.
 
-        Arguments:
-            drawing (bytes): binary representation of a technical drawing.
-                Please refer to the API - documentation to learn which mime
-                types are supported.
-
-            model (bytes): binary representation of the 3d model (typically
-                step)
-                Please refer to the API - documentation to learn which mime
-                types are supported. Defaults to None.
-
-            asks (List[W24Ask]): List of Asks that are requested from the API.
-                They must derive from the W24Ask object. Refer to the API
-                documentation for a full list of supported W24AskTypes
-
-            max_pages (int): Maximum number of pages that are being processed
-                of the submitted file. This protects platform users from
-                costly requests caused by a user uploading a single file with
-                many pages.
-
-            drawing_filename (str|None): Optional information about the
-                filename of the drawing. Frequently this contains information
-                about the drawing id and you can make that information
-                available to us through this parameter. If you don't know the
-                filename, don't worry, it will still work.
-
-            sub_account (UUID4|None): Optional specification of the sub-account
-                that the request should be attributed to. Sub-accounts allow
-                you to manage several customers at the same time and receiving
-                separate positions on the monthly invoice.
+        Args:
+        ----
+        drawing (bytes): binary representation of a technical drawing.
+            Please refer to the API - documentation to learn which mime
+            types are supported.
+
+        model (bytes): binary representation of the 3d model (typically
+            step). This is currently not being used and may come back
+            later again.
+
+        asks (List[W24Ask]): List of Asks that are requested from the API.
+            They must derive from the W24Ask object. Refer to the API
+            documentation for a full list of supported W24AskTypes
+
+        max_pages (int): Maximum number of pages that are being processed
+            of the submitted file. This protects platform users from
+            costly requests caused by a user uploading a single file with
+            many pages.
+
+        drawing_filename (str|None): Optional information about the
+            filename of the drawing. Frequently this contains information
+            about the drawing id and you can make that information
+            available to us through this parameter. If you don't know the
+            filename, don't worry, it will still work.
+
+        sub_account (UUID4|None): Optional specification of the sub-account
+            that the request should be attributed to. Sub-accounts allow
+            you to manage several customers at the same time and receiving
+            separate positions on the monthly invoice.
 
         Yields:
-            W24TechreadMessage -- Response object obtained from the API
-                that indicates the state of your request. Be sure to pass this
-                to the read_drawing_listen method
+        ------
+        W24TechreadMessage -- Response object obtained from the API
+            that indicates the state of your request. Be sure to pass this
+            to the read_drawing_listen method
 
         Raises:
-            DrawingTooLarge -- Exception is raised when the drawing was too
-                large to be processed. At the time of writing. The upload
-                limit lies at 6 MB (including overhead).
+        ------
+        DrawingTooLarge -- Exception is raised when the drawing was too
+            large to be processed. At the time of writing. The upload
+            limit lies at 6 MB (including overhead).
+
+        UnsupportedMediaType -- Exception is raised when the drawing or
+            model is submitted in any data type other than bytes.
 
-            UnsupportedMediaType -- Exception is raised when the drawing or
-                model is submitted in any data type other than bytes.
         """
+        # give us some debug information
+        logger.info("API method read_drawing() called")
 
         # quickly check whether the input type is bytes. If it is string,
         # the presigned-AWS post interestingly returns a 403 error_code
         # without additional information. We want to inform the caller
         # that they submitted the wrong data type.
         # See Github Issue #13
-        if not isinstance(drawing, bytes):
-            raise UnsupportedMediaType("Drawing bytes requires 'bytes' type")
-
-        # the same is true for the model bytes
-        if model is not None and not isinstance(model, bytes):
-            raise UnsupportedMediaType("Model bytes requires 'bytes' type")
-
-        # give us some debug information
-        logger.info("API method read_drawing() called")
-
-        # tell us when a development key is being used
-        if self._development_key:  # pragma: no cover
-            logger.info("Using development key %s***", self._development_key[:8])
+        if not isinstance(drawing, BufferedReader) and not isinstance(drawing, bytes):
+            raise UnsupportedMediaType(
+                "Drawing bytes requires 'bytes' or 'BufferedReader' type"
+            )
 
         # send the initiation command
         init_message, init_response = await self.init_request(
             asks, max_pages, drawing_filename, sub_account
         )
+
         yield init_message
 
         # stop if the response is unsuccessful.
         if not init_response.is_successful:
             return
 
         # Start reading the file
         async for message in self.read_request(init_response, asks, drawing, model):
             yield message
 
     async def read_request(
         self,
         init_response: W24TechreadInitResponse,
         asks: List[W24Ask],
-        drawing: bytes,
+        drawing: Union[bytes, BufferedReader],
         model: Optional[bytes] = None,
     ) -> None:
         """
         Read the request after obtaining the init_response.
 
         This is helpful when we want to perform the reading
         in the background or in a separate thread.
 
-        Arguments:
-            init_response (W24TechreadInitResponse): InitResponse that
-                was obtained from the init_request method
-            asks (List[W24Ask]): List of asks that we are asking for.
-                This is only used for error handling here.
-            drawing (bytes): Drawing bytes that shall be uploaded
-            model (Optional[bytes], optional): Optional model bytes.
-                Defaults to None.
+        Args:
+        ----
+        init_response (W24TechreadInitResponse): InitResponse that
+            was obtained from the init_request method
+        asks (List[W24Ask]): List of asks that we are asking for.
+            This is only used for error handling here.
+        drawing (bytes): Drawing bytes that shall be uploaded
+        model (Optional[bytes], optional): Optional model bytes.
+            Defaults to None.
 
         Yields:
-            W24TechreadMessage: Messages that are received after the
-                request was submitted
+        ------
+        W24TechreadMessage: Messages that are received after the
+            request was submitted
         """
         # upload drawing and model. We can do that in parallel.
         # If your user uploads them separately, you could also
         # upload them separately to Werk24.
         try:
-            upload_drawing = self._techread_client_https.upload_associated_file(
+            await self._techread_client_https.upload_associated_file(
                 init_response.drawing_presigned_post, drawing
             )
-            upload_model = self._techread_client_https.upload_associated_file(
-                init_response.model_presigned_post, model
-            )
-
-            await gather(upload_drawing, upload_model)
 
         # explicitly reraise the exception if the payload is too
         # large
         except (BadRequestException, RequestTooLargeException) as exception:
             async for message in self._trigger_asks_exception(asks, exception):
                 yield message
             return
@@ -460,61 +435,70 @@
         1. The server has a couple of 100ms to
            reserves some resources for you, and
         2. The server will create a new request_id
            that you will need when uploading the
            associated files
 
         Args:
-            asks (List[W24Ask]): List of asks that
-                we are asking for in this request
+        ----
+        asks (List[W24Ask]): Asks for this request.
+        max_pages (int): Maximum pages to be read.
+        drawing_filename (Optional[str]): Filename of the drawing, if any.
+        sub_account (Optional[UUID4]): Sub-account ID, if any.
 
-            max_pages (int): Maximum number of pages
-                that shall be read.
-
-            drawing_filename (Optional[str]): Optional
-                filename of the drawing.
+        Returns:
+        -------
+        Tuple[W24TechreadMessage, W24TechreadInitResponse]: Received
+            message and init response.
         """
         request = W24TechreadRequest(
             asks=asks,
             development_key=self._development_key,
             max_pages=max_pages,
             drawing_filename=drawing_filename,
             sub_account=sub_account,
         )
 
         await self._techread_client_wss.send_command(
-            W24TechreadAction.INITIALIZE.value, request.json()
+            W24TechreadAction.INITIALIZE.value,
+            request.model_dump_json(),
         )
-
         message = await self._techread_client_wss.recv_message()
         logger.info("Received request_id %s", message.request_id)
-        response = W24TechreadInitResponse.parse_obj(message.payload_dict)
+
+        try:
+            response = W24TechreadInitResponse.model_validate(message.payload_dict)
+        except ValueError as exception:
+            error_message = message.payload_dict.get("message")
+            if error_message is not None:
+                raise ServerException(error_message) from exception
+
         return message, response
 
     async def _send_command_read(self) -> AsyncGenerator[W24TechreadMessage, None]:
-        """Send the request request to the backend
-        and yield the resulting messages
+        """
+        Send the request request to the backend
+        and yield the resulting messages.
 
         Yields:
-            W24TechreadMessage: Receiving messages
+        ------
+        W24TechreadMessage: Receiving messages
         """
 
         # submit the request the to the API
         await self._techread_client_wss.send_command(W24TechreadAction.READ.value, "{}")
         logger.info("Techread request submitted")
 
         # Wait for incoming messages from the server.
         # They will tell you when the individual
         # asks become available. The socket returns
         # strings of jsonified W24TechreadMessage objects.
         #
-        # The loop will stop when the websocket is
-        # closed
+        # The loop will stop when the websocket is closed
         async for message in self._techread_client_wss.listen():
-            # check whether we need to download something
             if message.payload_url is not None:
                 message.payload_bytes = (
                     await self._techread_client_https.download_payload(
                         message.payload_url
                     )
                 )
 
@@ -523,38 +507,44 @@
             yield message
 
     @staticmethod
     async def _trigger_asks_exception(
         asks: List[W24Ask],
         exception_raw: Union[BadRequestException, RequestTooLargeException],
     ) -> AsyncGenerator[W24TechreadMessage, None]:
-        """Trigger exceptions for all the submitted asks.
+        """
+        Trigger exceptions for all the submitted asks.
+
         This helps us to mock consistent exception handling
         behavior even when the files are rejected before they
         reach the API.
 
         Args:
-            asks (List[W24Ask]): List of all submitted asks
-            exception (RequestTooLargeException): Exception
-                that shall be pushed
+        ----
+        asks (List[W24Ask]): List of all submitted asks
+        exception (RequestTooLargeException): Exception
+            that shall be pushed
 
         Yields:
-            W24TechreadMessage: Exception message
+        ------
+        W24TechreadMessage: Exception message
         """
 
         # get the exception type from the MAP
         try:
             exception_type = EXCEPTION_MAP[type(exception_raw)]
 
         # if we see an exception that we were not supposed
         # to handle, there must have been a developer passing
         # a new exception type. Let's tell her by rasing
         # a runtime error
-        except KeyError:
-            raise RuntimeError(f"Unknown exception type passed: {type(exception_raw)}")
+        except KeyError as exception:
+            raise RuntimeError(
+                "Unknown exception type passed: %s" % type(exception_raw)
+            ) from exception
 
         # translate the exception into an official exception
         exception = W24TechreadException(
             exception_level=W24TechreadExceptionLevel.ERROR,
             exception_type=exception_type,
         )
 
@@ -563,111 +553,130 @@
             yield W24TechreadMessage(
                 request_id=uuid.uuid4(),
                 message_type=W24TechreadMessageType.ASK,
                 message_subtype=cur_ask.ask_type,
                 exceptions=[exception],
             )
 
-    @staticmethod
-    def _get_license_environs(license_path: Optional[str]) -> Dict[str, str]:
+    @classmethod
+    def _get_license_environs(cls, license_path: Optional[str]) -> Dict[str, str]:
         """Get the environment variables
         Where we either select the variables from the license
         files. If that fails we fall back to the true environment
         variables.
 
         NOTE: We do not want to mix the sources.
 
         Args:
-            license_path (Optional[str]): Path of the license files
+        ----
+        license_path (Optional[str]): Path of the license files
 
         Returns:
-            Dict[str,str]: Key, Value pairs for the environment variables
+        -------
+        Dict[str,str]: Key, Value pairs for the environment variables
+
+        Raises:
+        ------
+        LicenseError: If the defined license path doesn't exist or if
+            relevant environment variable isn't found
         """
 
         # Mimick the old default value of .werk24
         if license_path is None:
-            for c_location in LICENSE_LOCATIONS:
-                if os.path.exists(c_location):
-                    license_path = c_location
-                    break
+            license_path = next(filter(os.path.exists, LICENSE_LOCATIONS), None)
 
         # First priority: look for the local license path
         if license_path is not None:
-            if os.path.exists(license_path):
-                environs_raw = {
-                    k: v
-                    for k, v in dotenv.dotenv_values(license_path).items()
-                    if v is not None
-                }
+            environs_raw = {
+                k: v for k, v in dotenv.dotenv_values(license_path).items() if v
+            }
 
-            # if the caller defined a license path, but it does not
-            # exist, raise the exception
-            else:
-                raise LicenseError(LICENSE_ERROR_TEXT)
+        # if the caller defined a license path, but it does not exist, raise the exception
+        elif license_path and not os.path.exists(license_path):
+            raise LicenseError(LICENSE_ERROR_TEXT)
 
         # Second priority: use the environment variables
         else:
             environs_raw = dict(os.environ)
 
-        # filter the environment variables to only include the
-        # ones that are relevant to us and return
-        try:
-            return {cur_key: environs_raw[cur_key] for cur_key in ENVIRONS}
-        except KeyError:
-            raise LicenseError(LICENSE_ERROR_TEXT)
+        return environs_raw
+
+    @classmethod
+    def make_from_token(
+        cls,
+        token: str,
+        region: Optional[str] = None,
+        server_https: Optional[str] = None,
+        server_wss: Optional[str] = None,
+        version: str = "v2",
+    ) -> "W24TechreadClient":
+        # create a reference to the client
+        server_https = server_https or DEFAULT_SERVER_HTTPS
+        server_wss = server_wss or DEFAULT_SERVER_WSS
+        client = W24TechreadClient(server_wss, version)
+
+        # register the credentials. This will in effect
+        # only set the variabels in the authorizer. It will
+        # not trigger a network request
+        client.register(cognito_region=region, token=token)
+
+        # return the client
+        return client
 
     @classmethod
     def make_from_env(
         cls,
         license_path: Optional[str] = None,
         auth_region: Optional[str] = None,
         server_https: Optional[str] = None,
         server_wss: Optional[str] = None,
         version: str = "v2",
     ) -> "W24TechreadClient":
         """Small helper function that creates a new
         W24TechreadClient from the environment info.
 
-        Arguments:
-            license_path:{Optional[str]} -- path to the License file.
-                By default we are looking for a .werk24 or werk24_license.txt
-                file in the current cwd. If argument is set to None, we are
-                not loading any file and relying on the ENVIRONMENT variables only
-
-            auth_region: {Optional[str]} -- AWS Region of the Authentication
-                Service.
-                Takes priority over environ W24TECHREAD_AUTH_REGION and
-                DEFAULT_AUTH_REGION
-
-            server_https: {Optional[str]} -- HTTPS endpoint of the Werk24 API.
-                Takes priority over environ W24TECHREAD_SERVER_HTTPS and
-                DEFAULT_SEVER_HTTPS
-
-            version: {Optional[str]} -- Version of the Werk24 API.
-                Takes priority over environ W24TECHREAD_VERSION and
-                DEfAULT_VERSION
+        Args:
+        ----
+        license_path:{Optional[str]} -- path to the License file.
+            By default we are looking for a .werk24 or werk24_license.txt
+            file in the current cwd. If argument is set to None, we are
+            not loading any file and relying on the ENVIRONMENT variables only
+
+        auth_region: {Optional[str]} -- AWS Region of the Authentication
+            Service.
+            Takes priority over environ W24TECHREAD_AUTH_REGION and
+            DEFAULT_AUTH_REGION
+
+        server_https: {Optional[str]} -- HTTPS endpoint of the Werk24 API.
+            Takes priority over environ W24TECHREAD_SERVER_HTTPS and
+            DEFAULT_SEVER_HTTPS
+
+        version: {Optional[str]} -- Version of the Werk24 API.
+            Takes priority over environ W24TECHREAD_VERSION and
+            DEfAULT_VERSION
 
         Raises:
-            FileNotFoundError -- Raised when you pass a path to a license file
-                that does not exist
-            UnauthorizedException -- Raised when the credentials were not
-                accepted by the API
+        ------
+        FileNotFoundError -- Raised when you pass a path to a license file
+            that does not exist
+        UnauthorizedException -- Raised when the credentials were not
+            accepted by the API
 
         Returns:
-            W24TechreadClient -- The techread Client
+        -------
+        W24TechreadClient -- The techread Client
         """
-
         # get the license variables from the environment variables and
         # the license file.
         environs = cls._get_license_environs(license_path)
 
         # define a small helper function that finds the first valid
         # value in the supplied list of possible values
         def pick_env(var: Optional[str], env_key: str, default: str) -> str:
-            return var or environs.get(env_key) or default
+            return var or environs.get(env_key, default)
 
         # then make sure we use the correct priorities
         auth_region = pick_env(
             auth_region, "W24TECHREAD_AUTH_REGION", DEFAULT_AUTH_REGION
         )
 
         server_wss = pick_env(
@@ -681,59 +690,112 @@
             client = W24TechreadClient(server_wss, version)
 
             # register the credentials. This will in effect
             # only set the variabels in the authorizer. It will
             # not trigger a network request
             client.register(
                 auth_region,
-                environs["W24TECHREAD_AUTH_IDENTITY_POOL_ID"],
-                environs["W24TECHREAD_AUTH_USER_POOL_ID"],
-                environs["W24TECHREAD_AUTH_CLIENT_ID"],
-                environs["W24TECHREAD_AUTH_CLIENT_SECRET"],
-                environs["W24TECHREAD_AUTH_USERNAME"],
-                environs["W24TECHREAD_AUTH_PASSWORD"],
+                environs.get("W24TECHREAD_AUTH_IDENTITY_POOL_ID"),
+                environs.get("W24TECHREAD_AUTH_USER_POOL_ID"),
+                environs.get("W24TECHREAD_AUTH_CLIENT_ID"),
+                environs.get("W24TECHREAD_AUTH_CLIENT_SECRET"),
+                environs.get("W24TECHREAD_AUTH_USERNAME"),
+                environs.get("W24TECHREAD_AUTH_PASSWORD"),
+                environs.get("W24TECHREAD_AUTH_TOKEN"),
             )
 
         except KeyError:
             raise LicenseError(LICENSE_ERROR_TEXT)
 
         # return the client
         return client
 
+    async def read_drawing_with_callback(
+        self,
+        drawing: Union[BufferedReader, bytes],
+        asks: List[W24Ask],
+        callback_url: str,
+        max_pages: int = 5,
+        drawing_filename: Optional[str] = None,
+    ) -> UUID4:
+        """Read the Drawings and register a callback URL.
+
+        This method is useful if you want to separate the
+        initialization from the upload and read stages.
+
+        You can simply specify the callback URL that shall
+        receive the message responses. This function will
+        return after sending the request to the API. The
+        callback URL will be called asynchronously. Keep
+        in mind that the callback speed depends on your
+        service level.
+
+        Args:
+        ----
+        drawing (Union[BufferedReader, bytes]): Drawing that you want to process
+        asks (List[W24Ask]): List of all the information that you want to obtain
+        callback_url (str): URL that shall receive the callback requests
+        max_pages (int, optional): Maximum number of pages that shall be processed.
+            Defaults to 5.
+        drawing_filename (Optional[str], optional): Filename of the drawing.
+            Defaults to None.
+
+        Raises:
+        ------
+        ServerException: Raised when the server returns an ERROR message
+
+        Returns:
+        -------
+        UUID4: Request ID of the request
+        """
+        # send the request to the API
+        try:
+            return await self._techread_client_https.read_drawing_with_callback(
+                drawing,
+                asks,
+                callback_url,
+                max_pages=max_pages,
+                drawing_filename=drawing_filename,
+            )
+        except ServerException:
+            raise
+
     async def read_drawing_with_hooks(
         self,
-        drawing_bytes: bytes,
+        drawing: Union[BufferedReader, bytes],
         hooks: List[Hook],
-        max_pages: int = 1,
+        max_pages: int = 5,
         drawing_filename: Optional[str] = None,
         sub_account: Optional[UUID4] = None,
     ) -> None:
-        """Send the drawing to the API (can be PDF or image)
+        """
+        Send the drawing to the API (can be PDF or image)
         and register a number of callbacks that are triggered
         once the asks become available.
 
-        Arguments:
-            drawing_bytes {bytes} -- Technical Drawing as Image or PDF
-            hooks {List[Hook]} -- List of Callback you want to obtain
+        Args:
+        ----
+        drawing_bytes {bytes} -- Technical Drawing as Image or PDF
+        hooks {List[Hook]} -- List of Callback you want to obtain
 
         Raises:
-            ServerException -- Raised when the server returns an ERROR
-                message
+        ------
+        ServerException -- Raised when the server returns an ERROR message
         """
 
         # filter the callback requests to only contain
         # the ask types
         asks_list = [cur_ask.ask for cur_ask in hooks if cur_ask.ask is not None]
 
         try:
             # send out the request and make a generator
             # that triggers when the result of an ask
             # becomes available
             async for message in self.read_drawing(
-                drawing_bytes,
+                drawing,
                 asks_list,
                 max_pages=max_pages,
                 drawing_filename=drawing_filename,
                 sub_account=sub_account,
             ):
                 await self.call_hooks_for_message(message, hooks)
 
@@ -743,30 +805,28 @@
 
     async def call_hooks_for_message(
         self, message: W24TechreadMessage, hooks: List[Hook]
     ) -> None:
         """
         Call the hook function for the response message.
 
-        Arguments:
-            message {W24TechreadMessage} -- Message returned from the
-                read_drawing method
+        Args:
+        ----
+        message (W24TechreadMessage): Message returned from the
+            read_drawing method
 
-            hooks {List[Hook]} -- List of hooks from which we need to
-                pick the suited one
+        hooks (List[Hook]): List of hooks from which we need to
+            pick the suited one
 
         Raises:
-            ServerException: raised when the server returns an ERROR
-                message
+        ------
+        ServerException: raised when the server returns an ERROR
+            message
         """
-
-        # get the hook function that corresponds to the message
         hook_function = self._get_hook_function_for_message(message, hooks)
-
-        # if no hook is registered, ignore
         if hook_function is None:
             return
 
         # if the hook_function is not callable, we want to warn the user,
         # rather than throwing an exception
         if not callable(hook_function):
             logger.warning(
@@ -777,52 +837,42 @@
                 message.message_type,
             )
             return
 
         # if everything went well, we call the trigger with
         # the message as payload. Be sure to call the
         # function asymmetrically if supported
-        if iscoroutinefunction(hook_function):
-            await hook_function(message)
-        else:
-            hook_function(message)
+        await hook_function(message) if iscoroutinefunction(
+            hook_function
+        ) else hook_function(message)
 
     @staticmethod
     def _get_hook_function_for_message(
         message: W24TechreadMessage, hooks: List[Hook]
     ) -> Optional[Callable]:
         """
         Get the hook function that corresponds to the message type.
 
-        Arguments:
-            message {W24TechreadMessage} -- Message returned from the
-                read_drawing method
-
-            hooks {List[Hook]} -- List of hooks from which we need to
-                pick the suited one
+        Args:
+        ----
+        message {W24TechreadMessage} -- Message returned from the read_drawing method
+        hooks {List[Hook]} -- List of hooks from which we need to pick the suited one
 
         Returns:
-            Optional[Callable] -- Hook function that should be called
+        -------
+        Optional[Callable] -- Hook function that should be called
         """
 
-        # because we allow the user to define the ask in the hook,
-        # we need to make some extra effort when filtering
-        if message.message_type == W24TechreadMessageType.ASK:
-
-            def hook_filter(hook: Hook) -> bool:
+        def hook_filter(hook: Hook) -> bool:
+            if message.message_type == W24TechreadMessageType.ASK:
                 return (
                     hook.ask is not None
                     and message.message_subtype.value == hook.ask.ask_type.value
                 )
-
-        # if the message is of any other type, we just need to
-        # compare the the message_type and message_subtype
-        else:
-
-            def hook_filter(hook: Hook) -> bool:
+            else:
                 return (
                     hook.message_type is not None
                     and hook.message_subtype is not None
                     and message.message_type == hook.message_type
                     and message.message_subtype == hook.message_subtype
                 )
 
@@ -842,38 +892,41 @@
         return None
 
     async def create_helpdesk_task(self, task: W24HelpdeskTask) -> W24HelpdeskTask:
         """
         Create a Helpdesk ticket.
 
         Args:
-            task (W24HelpdeskTask): Helpdesk task to be created
+        ----
+        task (W24HelpdeskTask): Helpdesk task to be created
 
         Raises:
-            BadRequestException: Raised when the request body
-                cannot be interpreted. This normally indicates
-                that the API version has been updated and that
-                we missed a corner case. If you encounter this
-                exception, it is very likely our mistake. Please
-                get in touch!
-
-            UnauthorizedException: Raised when the token
-                or the requested file have expired
-
-            ResourceNotFoundException: Raised when you are requesting
-                an endpoint that does not exist. Again, you should
-                not encounter this, but if you do, let us know.
-
-            RequestTooLargeException: Raised when the status
-                code was 413
-
-            UnsupportedMediaTypException: Raised when the file you
-                submitted cannot be read(because its media type
-                is not supported by the API).
+        ------
+        BadRequestException: Raised when the request body
+            cannot be interpreted. This normally indicates
+            that the API version has been updated and that
+            we missed a corner case. If you encounter this
+            exception, it is very likely our mistake. Please
+            get in touch!
+
+        UnauthorizedException: Raised when the token
+            or the requested file have expired
+
+        ResourceNotFoundException: Raised when you are requesting
+            an endpoint that does not exist. Again, you should
+            not encounter this, but if you do, let us know.
+
+        RequestTooLargeException: Raised when the status
+            code was 413
+
+        UnsupportedMediaTypException: Raised when the file you
+            submitted cannot be read(because its media type
+            is not supported by the API).
 
-            ServerException: Raised for all other status codes
-                that are not 2xx
+        ServerException: Raised for all other status codes
+            that are not 2xx
 
         Returns:
-            W24HelpdeskTask: Created helpdesk task with an updated task_id.
+        -------
+        W24HelpdeskTask: Created helpdesk task with an updated task_id.
         """
         return await self._techread_client_https.create_helpdesk_task(task)
```

### Comparing `werk24-1.8.3/werk24/techread_client_https.py` & `werk24-1.9.0/werk24/techread_client_https.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 """ HTTPS-part of the Werk24 client
 """
+import uuid
+import json
 import urllib.parse
+from pydantic import UUID4
+from werk24.models.techread import W24TechreadWithCallbackPayload
+from werk24.models.ask import W24AskUnion
+from typing import List
 from types import TracebackType
 from typing import Dict, Optional, Type
-
+from io import BufferedReader
 import aiohttp
 from pydantic import HttpUrl
-
+from typing import Union
+from werk24.auth_client import AuthClient
 from werk24.exceptions import (
     BadRequestException,
     RequestTooLargeException,
     ResourceNotFoundException,
     ServerException,
     UnauthorizedException,
     UnsupportedMediaType,
 )
 from werk24.models.helpdesk import W24HelpdeskTask
 from werk24.models.techread import W24PresignedPost
 
-from .auth_client import AuthClient
+
+EXCEPTION_CLASSES = {
+    range(200, 300): None,
+    range(400, 401): BadRequestException,
+    range(401, 403): UnauthorizedException,
+    range(404, 405): ResourceNotFoundException,
+    range(413, 414): RequestTooLargeException,
+    range(415, 416): UnsupportedMediaType,
+    range(300, 400): ServerException,
+    range(500, 600): ServerException,
+    range(416, 500): ServerException,
+}
 
 
 class TechreadClientHttps:
 
     """Translation map from the server response
     to the W24TechreadArchitectureStatus enum
     """
@@ -35,159 +53,162 @@
             techread_server_https {str} -- Domain of the Techread https server
             techread_version {str} -- Techread Version
             support_base_url {str} -- Base URL for support requests
         """
         self._techread_version = techread_version
         self._techread_session_https: Optional[aiohttp.ClientSession] = None
         self._auth_client: Optional[AuthClient] = None
-        self._support_base_url = support_base_url
+        self.support_base_url = support_base_url
 
     async def __aenter__(self) -> "TechreadClientHttps":
-        """Create a new HTTP session that is being used for the whole
-        connection. Be sure to keep the session alive.
+        """
+        Create a new HTTP session that is being used for the whole connection.
+        Be sure to keep the session alive.
 
         Raises:
-            RuntimeError  -- Raise when the developer enters the session
-                without having called register_auth_client()
+        ------
+        RuntimeError: Exception raised when the developer tries to start the
+            session without a token.
 
         Returns:
-            TechreadClientHttps -- TechreadClientHttps version with active
-                session
+        -------
+        TechreadClientHttps: Instance of the class itself with active session.
         """
+        if self._auth_client is None:
+            raise RuntimeError("No AuthClient was registered")
+
         self._techread_session_https = aiohttp.ClientSession()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
-        """Close the session"""
-        if self._techread_session_https is not None:
+        """
+        Close the session.
+
+        Args:
+        ----
+        exc_type (Optional[Type[BaseException]]): The type of exception that
+            caused the context manager to be exited.
+        exc_value (Optional[BaseException]): The instance of the exception that
+            caused the exit.
+        traceback (Optional[TracebackType]): A traceback from the exception.
+
+        Returns:
+        --------
+        None
+        """
+        if self._techread_session_https:
             await self._techread_session_https.close()
+            self._techread_session_https = None
 
     def register_auth_client(self, auth_client: AuthClient) -> None:
         """Register the reference to the authentication service
 
         Arguments:
             auth_client {AuthClient} -- Reference to Authentication
                 client
         """
         self._auth_client = auth_client
 
     async def upload_associated_file(
-        self, presigned_post: W24PresignedPost, content: Optional[bytes]
+        self,
+        presigned_post: W24PresignedPost,
+        content: Optional[Union[bytes, BufferedReader]],
     ) -> None:
-        """Upload an associated file to the API.
-        This can either be a technical drawing or a
-        3D model. Potentially we will sometime extend
-        this to also include cover pages.
-
-        NOTE: the complete message size must not be
-        larger than 10 MB
-
-        Arguments:
-            request_id {str} -- UUID4 request id that you obtained
-                from the websocket
+        """
+        Uploads an associated file to the API.
 
-            filetype {str} -- filetype that we want to upload.
-                currently supported: drawing, model
+        This can either be a technical drawing or a 3D model.
+        NOTE: The complete message size must not be larger than 10 MB.
 
-            content {bytes} -- content of the file as bytes
+        Args:
+        ----
+        presigned_post (W24PresignedPost): Presigned post object for
+            file upload.
+        content (Optional[bytes]): Content of the file as bytes.
 
         Raises:
+        -------
+        Various exceptions based on the issues with API, authentication
+            or the requested file.
 
-            BadRequestException: Raised when the request body
-                cannot be interpreted. This normally indicates
-                that the API version has been updated and that
-                we missed a corner case. If you encounter this
-                exception, it is very likely our mistake. Please
-                get in touch!
-
-            UnauthorizedException: Raised when the token
-                or the requested file have expired
-
-            ResourceNotFoundException: Raised when you are requesting
-                an endpoint that does not exist. Again, you should
-                not encounter this, but if you do, let us know.
-
-            RequestTooLargeException: Raised when the status
-                code was 413
-
-            UnsupportedMediaTypException: Raised when the file you
-                submitted cannot be read (because its media type
-                is not supported by the API).
-
-            ServerException: Raised for all other status codes
-                that are not 2xx
+        Returns:
+        --------
+        None
         """
         # ignore if payload is empty
         if content is None:
             return
 
         # generate the form data by merging the presigned
         # fields with the file
         form = aiohttp.FormData()
         for key, value in presigned_post.fields_.items():
             form.add_field(key, value)
         form.add_field("file", content)
 
         # create a new fresh session that does not
         # carry the authentication token
-        async with aiohttp.ClientSession() as sess:
-            async with sess.post(str(presigned_post.url), data=form) as resp:
-                # check the status code of the response and
-                # raise the appropriate exception
-                self._raise_for_status(str(presigned_post.url), resp.status)
+        presigned_post_str = str(presigned_post.url)
+        async with aiohttp.ClientSession() as session:
+            async with session.post(presigned_post_str, data=form) as response:
+                self._raise_for_status(presigned_post_str, response.status)
 
     async def download_payload(self, payload_url: HttpUrl) -> bytes:
         """Return the payload from the server
 
-        Arguments:
-            payload_url {HttpUrl} -- Url of the payload
+        Args:
+        ----
+        payload_url {HttpUrl} -- Url of the payload
 
         Raises:
-            RuntimeError: Hard Error that is raised when
-                the function is asked to download a payload
-                from an untrusted source.
-                This provides some sort of protection against
-                payload-injection and token-theft. When you
-                see this error showing up, you should
-                definitely INVESTIGATE AND LET US KNOW
-                IMMEDIATELY!!!
-                Call all our numbers on a Sunday morning
-                at 3am if it must be. Even if its Christmas
-                and Easter on the same day.
+        ------
+        RuntimeError: Hard Error that is raised when
+            the function is asked to download a payload
+            from an untrusted source.
+            This provides some sort of protection against
+            payload-injection and token-theft. When you
+            see this error showing up, you should
+            definitely INVESTIGATE AND LET US KNOW
+            IMMEDIATELY!!!
+            Call all our numbers on a Sunday morning
+            at 3am if it must be. Even if its Christmas
+            and Easter on the same day.
+
+        BadRequestException: Raised when the request body
+            cannot be interpreted. This normally indicates
+            that the API version has been updated and that
+            we missed a corner case. If you encounter this
+            exception, it is very likely our mistake. Please
+            get in touch!
+
+        UnauthorizedException: Raised when the token
+            or the requested file have expired
+
+        ResourceNotFoundException: Raised when you are requesting
+            an endpoint that does not exist. Again, you should
+            not encounter this, but if you do, let us know.
+
+        RequestTooLargeException: Raised when the status
+            code was 413
+
+        UnsupportedMediaTypException: Raised when the file you
+            submitted cannot be read (because its media type
+            is not supported by the API).
 
-            BadRequestException: Raised when the request body
-                cannot be interpreted. This normally indicates
-                that the API version has been updated and that
-                we missed a corner case. If you encounter this
-                exception, it is very likely our mistake. Please
-                get in touch!
+        ServerException: Raised for all other status codes
+            that are not 2xx
 
-            UnauthorizedException: Raised when the token
-                or the requested file have expired
-
-            ResourceNotFoundException: Raised when you are requesting
-                an endpoint that does not exist. Again, you should
-                not encounter this, but if you do, let us know.
-
-            RequestTooLargeException: Raised when the status
-                code was 413
-
-            UnsupportedMediaTypException: Raised when the file you
-                submitted cannot be read (because its media type
-                is not supported by the API).
-
-            ServerException: Raised for all other status codes
-                that are not 2xx
         Returns:
-            bytes -- Payload
+        -------
+        bytes -- Payload
         """
         # send the get request to the endpoint
         try:
             response = await self._get(payload_url)
 
         # reraise the exceptions
         except (
@@ -255,147 +276,202 @@
             raise exception
 
         # if the call was successful, return
         return response
 
     @staticmethod
     def _raise_for_status(url: str, status_code: int) -> None:
-        """Raise the correct exception depending on the
-        status code
+        """Raise the correct exception depending on the status code.
 
-        Arguments:
-            url {str} - - requested url
-            status_code {int} - - response status code
+        Args:
+        ----
+        url (str): The requested URL
+        status_code (int): The received response status code
 
         Raises:
-            BadRequestException: Raised when the request body
-                cannot be interpreted. This normally indicates
-                that the API version has been updated and that
-                we missed a corner case. If you encounter this
-                exception, it is very likely our mistake. Please
-                get in touch!
+        ------
+        BadRequestException: Raised when the request body
+            cannot be interpreted. This normally indicates
+            that the API version has been updated and that
+            we missed a corner case. If you encounter this
+            exception, it is very likely our mistake. Please
+            get in touch!
+
+        UnauthorizedException: Raised when the token
+            or the requested file have expired
+
+        ResourceNotFoundException: Raised when you are requesting
+            an endpoint that does not exist. Again, you should
+            not encounter this, but if you do, let us know.
+
+        RequestTooLargeException: Raised when the status
+            code was 413
+
+        UnsupportedMediaTypException: Raised when the file you
+            submitted cannot be read(because its media type
+            is not supported by the API).
+
+        ServerException: Raised for all other status codes
+            that are not 2xx
+        """
+        for key, exception_class in EXCEPTION_CLASSES.items():
+            if status_code in key:
+                if exception_class is not None:
+                    raise exception_class(
+                        f"Request failed '{url}' with code {status_code}"
+                    )
+                return None
 
-            UnauthorizedException: Raised when the token
-                or the requested file have expired
-
-            ResourceNotFoundException: Raised when you are requesting
-                an endpoint that does not exist. Again, you should
-                not encounter this, but if you do, let us know.
-
-            RequestTooLargeException: Raised when the status
-                code was 413
-
-            UnsupportedMediaTypException: Raised when the file you
-                submitted cannot be read(because its media type
-                is not supported by the API).
-
-            ServerException: Raised for all other status codes
-                that are not 2xx
-
-        """
-
-        # raise a bad request exception if the status
-        # code 400 was returned. This normally indicates
-        # that the API has been updated and the integration
-        # tests have missed a case
-        if status_code == 400:
-            raise BadRequestException()
-
-        # raise an unauthorized exception if the
-        # status code is
-        # * 401 (Unauthorized) or
-        # * 403 (Forbidden)
-        if status_code in {401, 403}:
-            raise UnauthorizedException()
-
-        # NOTE: a 404 does not occur, as the
-        # server does not want to tell you
-        # whether the file does not exist
-        # or whether your token is wrong.
-        # Makes brute force attacks more expensive.
-        # We deal with it anyway so we can change
-        # in the future
-        if status_code == 404:
-            raise ResourceNotFoundException()
-
-        # if the status code is 413, you have submitted
-        # a file that is too large.
-        if status_code == 413:
-            raise RequestTooLargeException()
-
-        # if the status code is 415, you have submitted
-        # a file whose media type is not supported by the API
-        if status_code == 415:
-            raise UnsupportedMediaType()
-
-        # If the resposne code is anything other
-        # than unauthorized or 200 (OK), we trigger
-        # a ServerException.
-        if not 200 <= status_code <= 299:
-            raise ServerException(f"Request failed '{url}' with code {status_code}")
+        # If the resposne code is anything other than unauthorized or 200 (OK), we trigger a ServerException.
+        raise ServerException(f"Request failed '{url}' with code {status_code}")
 
     async def create_helpdesk_task(self, task: W24HelpdeskTask) -> W24HelpdeskTask:
         """
         Create a Helpdesk ticket.
 
         Args:
-            task (W24HelpdeskTask): Helpdesk task to be created
+        ----
+        task (W24HelpdeskTask): Helpdesk task to be created
 
         Raises:
-            BadRequestException: Raised when the request body
-                cannot be interpreted. This normally indicates
-                that the API version has been updated and that
-                we missed a corner case. If you encounter this
-                exception, it is very likely our mistake. Please
-                get in touch!
-
-            UnauthorizedException: Raised when the token
-                or the requested file have expired
+        ------
+        BadRequestException: Raised when the request body
+            cannot be interpreted. This normally indicates
+            that the API version has been updated and that
+            we missed a corner case. If you encounter this
+            exception, it is very likely our mistake. Please
+            get in touch!
+
+        UnauthorizedException: Raised when the token
+            or the requested file have expired
+
+        ResourceNotFoundException: Raised when you are requesting
+            an endpoint that does not exist. Again, you should
+            not encounter this, but if you do, let us know.
+
+        RequestTooLargeException: Raised when the status
+            code was 413
+
+        UnsupportedMediaTypException: Raised when the file you
+            submitted cannot be read(because its media type
+            is not supported by the API).
 
-            ResourceNotFoundException: Raised when you are requesting
-                an endpoint that does not exist. Again, you should
-                not encounter this, but if you do, let us know.
-
-            RequestTooLargeException: Raised when the status
-                code was 413
-
-            UnsupportedMediaTypException: Raised when the file you
-                submitted cannot be read(because its media type
-                is not supported by the API).
-
-            ServerException: Raised for all other status codes
-                that are not 2xx
+        ServerException: Raised for all other status codes
+            that are not 2xx
 
         Returns:
-            W24HelpdeskTask: Created helpdesk task with an updated task_id.
+        -------
+        W24HelpdeskTask: Created helpdesk task with an updated task_id.
         """
         headers = self._make_helpdesk_headers()
         url = self._make_support_url("helpdesk/create-task")
         async with aiohttp.ClientSession(headers=headers) as session:
             response = await session.post(url, json=task.json())
             self._raise_for_status(url, response.status)
 
         # return the updated task
         return W24HelpdeskTask.parse_raw(await response.text())
 
     def _make_support_url(self, path: str) -> str:
         """Make the support url for the help desk requests.
 
-        Arguments:
-            path {str} -- Path to the endpoint
+        Args:
+        ----
+        path (str): Path to the endpoint
 
         Returns:
-            str -- URL to the endpoint
+        -------
+        str: URL to the endpoint
         """
-        return urllib.parse.urljoin(f"https://{self._support_base_url}", path)
+        return urllib.parse.urljoin(f"https://{self.support_base_url}", path)
 
     def _make_helpdesk_headers(self) -> Dict[str, str]:
         """
         Make the headers for the help desk requests.
 
         Simply the authorization header at this stage.
 
         Returns:
-            Dict[str, str]: Help desk headers
+        -------
+        Dict[str, str]: Help desk headers
+        """
+        return self._auth_client.get_headers()
+
+    async def read_drawing_with_callback(
+        self,
+        drawing: Union[BufferedReader, bytes],
+        asks: List[W24AskUnion],
+        callback_url: str,
+        max_pages: int = 5,
+        drawing_filename: Optional[str] = None,
+    ) -> UUID4:
         """
-        headers = {"Authorization": f"Bearer {self._auth_client.token}"}
-        return headers
+        Read a drawing with a callback.
+
+        Args:
+        ----
+        drawing (Union[BufferedReader, bytes]): Drawing to be read
+        asks (List[W24Ask]): List of asks
+        callback_url (str): Callback URL
+        max_pages (int, optional): Maximum number of pages to be read.
+            Defaults to 5.
+        drawing_filename (Optional[str], optional): Filename of the drawing.
+            Defaults to None.
+
+        Raises:
+        ------
+        BadRequestException: Raised when the request body
+            cannot be interpreted. This normally indicates
+            that the API version has been updated and that
+            we missed a corner case. If you encounter this
+            exception, it is very likely our mistake. Please
+            get in touch!
+
+        UnauthorizedException: Raised when the token
+            or the requested file have expired
+
+        ResourceNotFoundException: Raised when you are requesting
+            an endpoint that does not exist. Again, you should
+            not encounter this, but if you do, let us know.
+
+        RequestTooLargeException: Raised when the status
+            code was 413
+
+        UnsupportedMediaTypException: Raised when the file you
+            submitted cannot be read(because its media type
+            is not supported by the API).
+
+        ServerException: Raised for all other status codes
+            that are not 2xx
+
+        Returns:
+        -------
+        UUID4: Request ID
+        """
+
+        # Set a default drawing filename if none is provided
+        drawing_filename = drawing_filename or "drawing.pdf"
+
+        # create the form data
+        data = aiohttp.FormData()
+        data.add_field("drawing", drawing, filename=drawing_filename)
+        data.add_field(
+            "asks",
+            json.dumps([ask.model_dump(mode="json") for ask in asks]),
+        )
+        data.add_field("callback_url", callback_url)
+        data.add_field("max_pages", str(max_pages))
+        data.add_field("client_version", self._techread_version)
+        data.add_field("drawing_filename", drawing_filename)
+
+        # send the request
+        headers = self._auth_client.get_auth_headers()
+        url = self._make_support_url("techread/read-with-callback")
+        async with aiohttp.ClientSession(headers=headers) as session:
+            response = await session.post(url, data=data)
+            response_json = await response.json(content_type=None)
+            self._raise_for_status(url, response.status)
+
+        try:
+            return uuid.UUID(response_json["request_id"])
+        except (ValueError, KeyError):
+            raise BadRequestException(f"Request failed: {response_json}")
```

### Comparing `werk24-1.8.3/werk24/techread_client_wss.py` & `werk24-1.9.0/werk24/techread_client_wss.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,62 +5,47 @@
 from typing import Optional, Type, AsyncGenerator
 
 import websockets
 from pydantic import ValidationError
 from websockets.client import WebSocketClientProtocol
 from werk24.exceptions import ServerException, UnauthorizedException
 from werk24.models.techread import W24TechreadCommand, W24TechreadMessage
-
-from .auth_client import AuthClient
+from werk24.auth_client import AuthClient
 
 
 class TechreadClientWss:
     """TechreadClient subpart that handles the websocket
     communication with the server.
     """
 
     def __init__(self, techread_server_wss: str, techread_version: str):
-        self._auth_client: Optional[AuthClient] = None
         self._techread_server_wss = techread_server_wss
         self._techread_version = techread_version
         self._techread_session_wss: Optional[WebSocketClientProtocol] = None
+        self.endpoint = f"wss://{self._techread_server_wss}/{self._techread_version}"
+        self._auth_client = None
 
     async def __aenter__(self) -> "TechreadClientWss":
-        """Enter the session with the wss server
+        """
+        Enter the session with the wss server
 
         Raises:
-            RuntimeError  -- Raise when the developer enters the session
-                without having called register_auth_client()
+        ------
+        RuntimeError  -- Raise when the developer enters the session
+            without having specified a token
 
         Returns:
-            TechreadClientWss -- instance with activated session
+        -------
+        TechreadClientWss -- instance with activated session
         """
-
-        # make sure that we have an AuthClient
-        if self._auth_client is None:
-            raise RuntimeError(
-                "You need to call register_auth_client() before you can start"
-                + " the session"
-            )
-
-        # make the endpoint
-        endpoint = "wss://{}/{}".format(
-            self._techread_server_wss, self._techread_version
-        )
-
-        # make the ehaders
-        headers = [("Authorization", f"Bearer {self._auth_client.token}")]
-
-        # now make the session
+        headers = self._auth_client.get_auth_headers()
         self._techread_session_wss = await websockets.connect(
-            endpoint,
+            self.endpoint,
             extra_headers=headers,
         )
-
-        # return ourselfves
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
@@ -105,85 +90,81 @@
                 "You need to call enter the profile before sending a command"
             )
 
         # make the command
         command = W24TechreadCommand(action=action, message=message)
 
         # send the the command
-        await self._techread_session_wss.send(command.json())
+        await self._techread_session_wss.send(command.model_dump_json())
 
     async def recv_message(self) -> W24TechreadMessage:
         """Receive a message from the websocket and interpret
         the result as W24TechreadMessage
 
         Raises:
-            RuntimeError  -- Raise when the developer tries to send a command
-                without entering the profile
+        ------
+        RuntimeError: When trying to send a command without having entered the profile.
 
         Returns:
-            W24TechreadMessage -- interpreted message
+        -------
+        W24TechreadMessage: interpreted message
         """
 
         # make sure that we have an AuthClient
         if self._techread_session_wss is None:
             raise RuntimeError(
                 "You need to call enter the profile before receiving command"
             )
 
-        # wait for the websocket to say something
+        # wait for the websocket to say something and interpret the message
         message_raw = str(await self._techread_session_wss.recv())
-
-        # process the message
         message = await self._process_message(message_raw)
-
-        # and finally return
         return message
 
     @staticmethod
     async def _process_message(message_raw: str) -> W24TechreadMessage:
         """Interpret the raw websocket message and
         turn it into a W24TechreadMessage
 
-        Arguments:
-            message_raw {str} -- Raw message
+        Args:
+        message_raw (str): Raw message
 
         Raises:
-            UnauthorizedException: Exception is raised
-                when you requested an action that you
-                have no privileges for (or that does
-                not exist)
+        ------
+        UnauthorizedException: Exception is raised
+            when you requested an action that you
+            have no privileges for (or that does
+            not exist)
 
-            ServerException: Exception is raised when
-                the server did not respond as expected
+        ServerException: Exception is raised when
+            the server did not respond as expected
 
         Returns:
-            W24TeachreadMessage -- interpreted message
+        -------
+        W24TeachreadMessage: interpreted message
         """
-        # interpret and return
         try:
-            message = W24TechreadMessage.parse_raw(message_raw)
+            return W24TechreadMessage.model_validate_json(message_raw)
 
-        # if that fails, we are probably receiving a
-        # message from the gateway directly
-        except ValidationError:
+        except ValidationError as exception:
             # The Gateway responds with the format
             # {"message": str, "connectionId":str, "requestId":str}
             # Obtain the message
             response = json.loads(message_raw)
-            message = response.get("message")
+            error_message = response.get("message")
 
             # raise a specific exception if the
             # requested action was forbidden
-            if message == "Forbidden":
-                raise UnauthorizedException("Requested Action forbidden")
+            if error_message == "Forbidden":
+                raise UnauthorizedException("Requested Action forbidden") from exception
 
             # otherwise fail with an UnknownException
-            raise ServerException(f"Unexpected server response '{message_raw}'.")
-
-        return message
+            raise ServerException(
+                f"Unexpected server response '{message_raw}'."
+            ) from exception
 
     async def listen(self) -> AsyncGenerator[W24TechreadMessage, None]:
         """Simple generator that waits for
         messages on the websocket, interprets
         them and yields them
 
         Yields:
```

### Comparing `werk24-1.8.3/werk24/utils.py` & `werk24-1.9.0/werk24/utils.py`

 * *Files identical despite different names*

### Comparing `werk24-1.8.3/werk24.egg-info/PKG-INFO` & `werk24-1.9.0/werk24.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werk24
-Version: 1.8.3
+Version: 1.9.0
 Summary: Werk24 Client to read PDF- and Image-based Technical Drawings / Engineering Drawings
 Home-page: https://werk24.io
 Author: W24 Service GmbH
 Author-email: info@werk24.io
 License: commercial
 Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
@@ -116,8 +116,7 @@
 Keywords: Digitisation,Digitization,Engineering Drawing,Engineering Drawings,Technical Drawing,Technical Drawings,CAD,CAD Drawing,Data Extraction,Information Extraction,Model Based Definition,EN10027,ISO2768,Title Block,General Tolerances,Material,Drawing ID,Drawing Designation,Product Manufacturing Information,PMI,Scanned Document,Bill of Material,BOM,Anonymiziation,RFQ,GD&T,General Dimensioning and Toleration,Vectorization
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Provides-Extra: gui
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: werk24 Version: 1.8.3 Summary: Werk24 Client to
+Metadata-Version: 2.1 Name: werk24 Version: 1.9.0 Summary: Werk24 Client to
 read PDF- and Image-based Technical Drawings / Engineering Drawings Home-page:
 https://werk24.io Author: W24 Service GmbH Author-email: info@werk24.io
 License: commercial Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
                                    _[_W_e_r_k_2_4_]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
 pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
@@ -41,8 +41,8 @@
 Extraction,Model Based Definition,EN10027,ISO2768,Title Block,General
 Tolerances,Material,Drawing ID,Drawing Designation,Product Manufacturing
 Information,PMI,Scanned Document,Bill of
 Material,BOM,Anonymiziation,RFQ,GD&T,General Dimensioning and
 Toleration,Vectorization Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Image Recognition Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown Provides-Extra: gui
+Description-Content-Type: text/markdown
```

### Comparing `werk24-1.8.3/werk24.egg-info/SOURCES.txt` & `werk24-1.9.0/werk24.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,29 +22,19 @@
 werk24/assets/images/favicon-16x16.png
 werk24/assets/images/favicon-24x24.png
 werk24/assets/images/favicon-256x256.png
 werk24/assets/images/favicon-32x32.png
 werk24/assets/images/favicon-48x48.png
 werk24/assets/images/logo-625.png
 werk24/cli/__init__.py
-werk24/cli/auth.py
 werk24/cli/health_check.py
 werk24/cli/support.py
 werk24/cli/techread.py
 werk24/cli/utils.py
 werk24/cli/w24cli.py
-werk24/gui/__init__.py
-werk24/gui/event_feed.py
-werk24/gui/event_illustrator.py
-werk24/gui/gdt_table.py
-werk24/gui/json_editor.py
-werk24/gui/measure_table.py
-werk24/gui/style.py
-werk24/gui/w24gui.py
-werk24/gui/worker.py
 werk24/models/__init__.py
 werk24/models/alignment.py
 werk24/models/alphabet.py
 werk24/models/angle.py
 werk24/models/ask.py
 werk24/models/base_feature.py
 werk24/models/bom_table.py
```

