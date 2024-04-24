# Comparing `tmp/amuse-huayno-2023.5.0.tar.gz` & `tmp/amuse-huayno-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-huayno-2023.5.0.tar", last modified: Wed May 17 10:18:58 2023, max compression
+gzip compressed data, was "amuse-huayno-2024.4.0.tar", last modified: Wed Apr 24 16:32:25 2024, max compression
```

## Comparing `amuse-huayno-2023.5.0.tar` & `amuse-huayno-2024.4.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:58.406110 amuse-huayno-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-huayno-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:18:58.405941 amuse-huayno-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       59 2022-11-22 11:55:14.000000 amuse-huayno-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:58.396801 amuse-huayno-2023.5.0/amuse_huayno.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:18:56.000000 amuse-huayno-2023.5.0/amuse_huayno.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     2090 2023-05-17 10:18:58.000000 amuse-huayno-2023.5.0/amuse_huayno.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:18:56.000000 amuse-huayno-2023.5.0/amuse_huayno.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:18:56.000000 amuse-huayno-2023.5.0/amuse_huayno.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:18:56.000000 amuse-huayno-2023.5.0/amuse_huayno.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-huayno-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:18:58.406158 amuse-huayno-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1777 2022-11-22 11:55:14.000000 amuse-huayno-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:58.395243 amuse-huayno-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:58.395296 amuse-huayno-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:58.395346 amuse-huayno-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:58.398651 amuse-huayno-2023.5.0/src/amuse/community/huayno/
--rw-r--r--   0 rieder     (501) staff       (20)     3683 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    13587 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/interface.c
--rw-r--r--   0 rieder     (501) staff       (20)    14167 2023-03-14 13:48:49.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)     2640 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/readme.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:58.404316 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/
--rw-r--r--   0 rieder     (501) staff       (20)     1233 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)      246 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/common.h
--rw-r--r--   0 rieder     (501) staff       (20)    20756 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve.c
--rw-r--r--   0 rieder     (501) staff       (20)     5898 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve.h
--rw-r--r--   0 rieder     (501) staff       (20)     9090 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_bs.c
--rw-r--r--   0 rieder     (501) staff       (20)      182 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_bs.h
--rw-r--r--   0 rieder     (501) staff       (20)    19000 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_cc.c
--rw-r--r--   0 rieder     (501) staff       (20)      304 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_cc.h
--rw-r--r--   0 rieder     (501) staff       (20)    15707 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_cl.c
--rw-r--r--   0 rieder     (501) staff       (20)      265 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_cl.h
--rw-r--r--   0 rieder     (501) staff       (20)     2804 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_error_control.c
--rw-r--r--   0 rieder     (501) staff       (20)      104 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_error_control.h
--rw-r--r--   0 rieder     (501) staff       (20)     5019 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_kepler.c
--rw-r--r--   0 rieder     (501) staff       (20)       84 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_kepler.h
--rw-r--r--   0 rieder     (501) staff       (20)     4145 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_kern.cl
--rw-r--r--   0 rieder     (501) staff       (20)     4259 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_ok.c
--rw-r--r--   0 rieder     (501) staff       (20)      381 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_ok.h
--rw-r--r--   0 rieder     (501) staff       (20)    12574 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_sf.c
--rw-r--r--   0 rieder     (501) staff       (20)     1547 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_sf.h
--rw-r--r--   0 rieder     (501) staff       (20)     3676 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_shared.c
--rw-r--r--   0 rieder     (501) staff       (20)      928 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_shared.h
--rw-r--r--   0 rieder     (501) staff       (20)     4726 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_shared_collisions.c
--rw-r--r--   0 rieder     (501) staff       (20)      331 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_shared_collisions.h
--rw-r--r--   0 rieder     (501) staff       (20)    10838 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/integrators_shared.h
--rw-r--r--   0 rieder     (501) staff       (20)     8872 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/simple_hash.c
--rw-r--r--   0 rieder     (501) staff       (20)     1112 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/simple_hash.h
--rw-r--r--   0 rieder     (501) staff       (20)     1635 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/simple_map.c
--rw-r--r--   0 rieder     (501) staff       (20)      542 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/simple_map.h
--rw-r--r--   0 rieder     (501) staff       (20)    16275 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/universal_kepler_solver.h
--rw-r--r--   0 rieder     (501) staff       (20)     7448 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/universal_variable_kepler.c
--rw-r--r--   0 rieder     (501) staff       (20)      133 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/src/universal_variable_kepler.h
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:18:56.000000 amuse-huayno-2023.5.0/src/amuse/community/huayno/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:58.405654 amuse-huayno-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-huayno-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-huayno-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-huayno-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:25.146858 amuse-huayno-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-huayno-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1217 2024-04-24 16:32:25.146641 amuse-huayno-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       59 2022-11-22 11:55:14.000000 amuse-huayno-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:25.146304 amuse-huayno-2024.4.0/amuse_huayno.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1217 2024-04-24 16:32:24.000000 amuse-huayno-2024.4.0/amuse_huayno.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     2091 2024-04-24 16:32:25.000000 amuse-huayno-2024.4.0/amuse_huayno.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:24.000000 amuse-huayno-2024.4.0/amuse_huayno.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:24.000000 amuse-huayno-2024.4.0/amuse_huayno.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:24.000000 amuse-huayno-2024.4.0/amuse_huayno.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-huayno-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:25.146913 amuse-huayno-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1581 2024-04-24 15:35:29.000000 amuse-huayno-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:25.135225 amuse-huayno-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:25.135275 amuse-huayno-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:25.135325 amuse-huayno-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:25.138172 amuse-huayno-2024.4.0/src/amuse/community/huayno/
+-rw-r--r--   0 rieder     (501) staff       (20)     3683 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:24.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13507 2024-04-24 15:35:29.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/interface.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14167 2023-03-14 13:48:49.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2640 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/readme.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:25.144583 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     1233 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      246 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/common.h
+-rw-r--r--   0 rieder     (501) staff       (20)    20756 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5898 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve.h
+-rw-r--r--   0 rieder     (501) staff       (20)     9090 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_bs.c
+-rw-r--r--   0 rieder     (501) staff       (20)      182 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_bs.h
+-rw-r--r--   0 rieder     (501) staff       (20)    19000 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_cc.c
+-rw-r--r--   0 rieder     (501) staff       (20)      304 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_cc.h
+-rw-r--r--   0 rieder     (501) staff       (20)    15707 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_cl.c
+-rw-r--r--   0 rieder     (501) staff       (20)      265 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_cl.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2804 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_error_control.c
+-rw-r--r--   0 rieder     (501) staff       (20)      104 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_error_control.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5019 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_kepler.c
+-rw-r--r--   0 rieder     (501) staff       (20)       84 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_kepler.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4145 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_kern.cl
+-rw-r--r--   0 rieder     (501) staff       (20)     4259 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_ok.c
+-rw-r--r--   0 rieder     (501) staff       (20)      381 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_ok.h
+-rw-r--r--   0 rieder     (501) staff       (20)    12574 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_sf.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1547 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_sf.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3676 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_shared.c
+-rw-r--r--   0 rieder     (501) staff       (20)      928 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_shared.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4726 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_shared_collisions.c
+-rw-r--r--   0 rieder     (501) staff       (20)      331 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_shared_collisions.h
+-rw-r--r--   0 rieder     (501) staff       (20)    10838 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/integrators_shared.h
+-rw-r--r--   0 rieder     (501) staff       (20)     8872 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/simple_hash.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1112 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/simple_hash.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1635 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/simple_map.c
+-rw-r--r--   0 rieder     (501) staff       (20)      542 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/simple_map.h
+-rw-r--r--   0 rieder     (501) staff       (20)    16275 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/universal_kepler_solver.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7448 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/universal_variable_kepler.c
+-rw-r--r--   0 rieder     (501) staff       (20)      133 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/src/amuse/community/huayno/src/universal_variable_kepler.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:25.146087 amuse-huayno-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-huayno-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-huayno-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-huayno-2024.4.0/support/version.py
```

### Comparing `amuse-huayno-2023.5.0/PKG-INFO` & `amuse-huayno-2024.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-huayno
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Huayno
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the Huyano community code for AMUSE.
```

### Comparing `amuse-huayno-2023.5.0/amuse_huayno.egg-info/PKG-INFO` & `amuse-huayno-2024.4.0/amuse_huayno.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-huayno
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Huayno
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the Huyano community code for AMUSE.
```

### Comparing `amuse-huayno-2023.5.0/amuse_huayno.egg-info/SOURCES.txt` & `amuse-huayno-2024.4.0/amuse_huayno.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 amuse_huayno.egg-info/PKG-INFO
 amuse_huayno.egg-info/SOURCES.txt
 amuse_huayno.egg-info/dependency_links.txt
 amuse_huayno.egg-info/requires.txt
 amuse_huayno.egg-info/top_level.txt
 src/amuse/community/huayno/Makefile
 src/amuse/community/huayno/__init__.py
+src/amuse/community/huayno/_version.py
 src/amuse/community/huayno/interface.c
 src/amuse/community/huayno/interface.py
 src/amuse/community/huayno/readme.txt
-src/amuse/community/huayno/version.py
 src/amuse/community/huayno/src/Makefile
 src/amuse/community/huayno/src/common.h
 src/amuse/community/huayno/src/evolve.c
 src/amuse/community/huayno/src/evolve.h
 src/amuse/community/huayno/src/evolve_bs.c
 src/amuse/community/huayno/src/evolve_bs.h
 src/amuse/community/huayno/src/evolve_cc.c
```

### Comparing `amuse-huayno-2023.5.0/setup.py` & `amuse-huayno-2024.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.huayno.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/huayno/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/huayno/_version.py",
+}
 
 setup(
     name=name,
     use_scm_version=use_scm_version,
     setup_requires=setup_requires,
-    version=version,
     classifiers=classifiers,
     url=url,
     author_email=author_email,
     author=author,
     license=license_,
     description=description,
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     install_requires=install_requires,
-    python_requires=">=3.5",
+    python_requires=">=3.7",
     cmdclass=mapping_from_command_name_to_command_class,
     ext_modules=extensions,
     package_dir={
         'amuse.community.huayno': 'src/amuse/community/huayno',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/Makefile` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/interface.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/interface.c`

 * *Files 2% similar despite different names*

```diff
@@ -570,19 +570,14 @@
   int err;
   err=LOOKUPSYMBOL(,_lookup)( &lookup, id,&p);
   if(err!=0) return err;
   *pot=mainsys.part[p].pot;
   return 0;
 }
 
-int set_acceleration(int id, double ax, double ay, double az)
-{
-  return -2;
-}
-
 int get_acceleration(int id, double *ax, double *ay, double *az)
 {
   return -2;
 }
 
 int get_indices_of_colliding_particles(int *p1,int*p2)
 {
```

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/interface.py` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/readme.txt` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/readme.txt`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/Makefile` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve.h` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve.h`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_bs.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_bs.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_cc.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_cc.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_cl.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_cl.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_error_control.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_error_control.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_kepler.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_kepler.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_kern.cl` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_kern.cl`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_ok.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_ok.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_sf.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_sf.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_sf.h` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_sf.h`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_shared.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_shared.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_shared.h` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_shared.h`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/evolve_shared_collisions.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/evolve_shared_collisions.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/integrators_shared.h` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/integrators_shared.h`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/simple_hash.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/simple_hash.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/simple_hash.h` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/simple_hash.h`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/simple_map.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/simple_map.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/simple_map.h` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/simple_map.h`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/universal_kepler_solver.h` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/universal_kepler_solver.h`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/src/amuse/community/huayno/src/universal_variable_kepler.c` & `amuse-huayno-2024.4.0/src/amuse/community/huayno/src/universal_variable_kepler.c`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/support/__init__.py` & `amuse-huayno-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/support/classifiers.py` & `amuse-huayno-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/support/config.py` & `amuse-huayno-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/support/generate_main.py` & `amuse-huayno-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/support/getsp.class` & `amuse-huayno-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/support/getsp.java` & `amuse-huayno-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/support/misc.py` & `amuse-huayno-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-huayno-2023.5.0/support/setup_codes.py` & `amuse-huayno-2024.4.0/support/setup_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 import configparser
 
 from subprocess import Popen, PIPE, STDOUT
 
 from glob import glob
 
 from distutils.dir_util import create_tree
-# from distutils import log
-import logging
+from distutils import log
 from distutils import spawn
 from distutils import file_util
 from distutils.errors import DistutilsError
 from distutils.command.clean import clean
 from setuptools.command.install import install
 from setuptools import Command
 from setuptools.command.build import build
@@ -556,37 +555,37 @@
         if not os.path.exists(lib_binbuilddir):
             self.mkpath(lib_binbuilddir)
 
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
 
-            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
+            self.announce("will copy worker: {0}".format(srcdir), level=log.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level=logging.INFO)
+            self.announce(shortname, level=log.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
 
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                         continue
 
-                # self.announce("will copy worker: {0}".format(name), level = logging.INFO)
+                # self.announce("will copy worker: {0}".format(name), level = log.INFO)
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_binbuilddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=log.WARN)
             
             # also copy file or dir named data
             path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
                 self.copy_file(path, topath)
             if os.path.isdir(path):
@@ -599,19 +598,19 @@
             worker_code_re = re.compile(r'(([a-zA-Z0-9]+_)*)?worker(_[a-zA-Z0-9]+)?')
         worker_so_re = re.compile(r'(([a-zA-Z0-9]+_)*)?cython(_[a-zA-Z0-9]+)?.so')
 
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
 
-            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
+            self.announce("will copy worker: {0}".format(srcdir), level=log.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level=logging.INFO)
+            self.announce(shortname, level=log.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
 
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
@@ -620,15 +619,15 @@
                         continue
 
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=log.WARN)
             
             # also copy file or dir named data
             path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
                 self.copy_file(path, topath)
             if os.path.isdir(path):
@@ -712,15 +711,15 @@
         result = list(set(result))
 
         return result
 
     def call(self, arguments, buildlogfile=None, **keyword_arguments):
         stringio = []
 
-        self.announce(' '.join(arguments), logging.DEBUG)
+        self.announce(' '.join(arguments), log.DEBUG)
 
         process = Popen(
             arguments,
             stdout=PIPE,
             stderr=STDOUT,
             **keyword_arguments
         )
@@ -728,24 +727,24 @@
         while True:
             line = process.stdout.readline()
             if len(line) == 0:
                 break
 
             if buildlogfile is not None:
                 buildlogfile.write(line)
-            self.announce(line[:-1].decode("utf-8"), logging.DEBUG)
+            self.announce(line[:-1].decode("utf-8"), log.DEBUG)
             stringio.append(str(line, 'utf-8'))
 
         result = process.wait()
         content = ''.join(stringio)
 
         if result != 0:
-            self.announce("error in call, tail output:\n", logging.INFO)
-            self.announce(''.join(stringio[-100:]), logging.INFO)
-            self.announce("-"*80, logging.INFO)
+            self.announce("error in call, tail output:\n", log.INFO)
+            self.announce(''.join(stringio[-100:]), log.INFO)
+            self.announce("-"*80, log.INFO)
 
         return result, content
 
     def build_environment(self):
         environment = self.environment.copy()
         environment.update(os.environ)
         path = os.path.join(environment["MUSE_PACKAGE_DIR"], "src")
@@ -880,16 +879,16 @@
         build = list()
         lib_build = list()
         lib_not_build = list()
         environment = self.build_environment()
 
         buildlog = 'build.log'
 
-        self.announce("building libraries and community codes", level=logging.INFO)
-        self.announce("build, for logging, see '{0}'".format(buildlog), level=logging.INFO)
+        self.announce("building libraries and community codes", level=log.INFO)
+        self.announce("build, for logging, see '{0}'".format(buildlog), level=log.INFO)
 
         with open(buildlog, "w") as output:
             output.write('*'*100)
             output.write('\n')
             output.write('Building libraries and codes\n')
             output.write('*'*100)
             output.write('\n')
@@ -898,28 +897,28 @@
             self.copy_build_prereq_to_build_dir()
             self.copy_lib_to_build_dir()
 
         for x in self.makefile_paths(self.lib_dir):
 
             shortname = x[len(self.lib_dir) + 1:] + '-library'
             starttime = datetime.datetime.now()
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=log.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
 
             endtime = datetime.datetime.now()
             if returncode == 2:
-                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=logging.DEBUG)
+                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=log.DEBUG)
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(x[len(self.lib_dir) + 1:])
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(x[len(self.lib_dir) + 1:])
                 else:
                     lib_not_build.append(shortname)
             else:
-                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=logging.DEBUG)
+                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=log.DEBUG)
                 lib_build.append(shortname)
 
         if not self.codes_dir == self.codes_src_dir:
             self.copy_codes_to_build_dir()
 
         # environment.update(self.environment)
         makefile_paths = list(self.makefile_paths(self.codes_dir))
@@ -933,24 +932,24 @@
             # to distribute mesa, it will make the
             # download size from about 100mb size
             # to > 1Gb size.
             #
             # Could we remove some of the data files from mesa?
             #
             if not self.inplace and shortname == 'mesa':
-                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=logging.INFO)
+                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=log.INFO)
                 continue
 
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=log.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
             endtime = datetime.datetime.now()
             if returncode > 0:
                 self.announce(
                     "[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(shortname)
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(shortname)
                 elif self.are_python_imports_needed(outputlog):
                     are_python_imports_needed.append(shortname)
@@ -960,40 +959,40 @@
                 if self.is_mpi_enabled():
                     continue
             else:
                 build.append(shortname)
                 is_built = True
                 self.announce(
                     "[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
 
             if not self.variant:
                 continue
 
             special_targets = self.get_special_targets(shortname, x, environment)
             for target, target_name in special_targets:
                 starttime = datetime.datetime.now()
                 self.announce(
                     "[{2:%H:%M:%S}] building {0} - {1}".format(shortname, target_name, starttime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
                 returncode, outputlog = self.run_make_on_directory(shortname, x, target, environment)
                 endtime = datetime.datetime.now()
                 if returncode > 0:
                     specials_list = not_build_special.setdefault(shortname,[])
                     specials_list.append(target_name)
                     self.announce(
                         "[{3:%H:%M:%S}] building {0} - {1}, failed, see {2!r} for error log".format(shortname, target_name, buildlog, endtime),
-                        level=logging.DEBUG
+                        level=log.DEBUG
                     )
                 else:
                     build_to_special_targets.setdefault(shortname, list()).append(target_name)
                     self.announce(
-                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=logging.DEBUG
+                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=log.DEBUG
                     )
 
         # if supportrc["framework_install"]:
         #     self.copy_config_to_build_dir()
 
         if not self.codes_dir == self.codes_src_dir:
             # self.copy_worker_codes_to_build_dir()
@@ -1028,17 +1027,17 @@
             not_build
             or not_build_special
             or is_download_needed
             or is_cuda_needed
             or are_python_imports_needed
         ):
             if not_build:
-                level = logging.WARN
+                level = log.WARN
             else:
-                level = logging.INFO
+                level = log.INFO
             if not_build:
                 self.announce(
                     "Community codes not built (because of errors/ missing libraries):",
                     level=level
                 )
                 self.announce("="*80,  level=level)
                 for x in not_build:
@@ -1061,26 +1060,26 @@
                     self.announce(
                         f' * {x} , make {x}.code DOWNLOAD_CODES=1', level=level
                     )
 
             self.announce("="*80,  level=level)
 
         if build:
-            level = logging.INFO
+            level = log.INFO
             self.announce("Community codes built",  level=level)
             self.announce("="*80,  level=level)
             for x in build:
                 if x in build_to_special_targets:
                     y = build_to_special_targets[x]
                     self.announce('* {0} ({1})'.format(x, ','.join(y)), level=level)
                 else:
                     self.announce('* {0}'.format(x),  level=level)
             self.announce("="*80,  level=level)
 
-        level = logging.INFO
+        level = log.INFO
         self.announce(
             "{0} out of {1} codes built, {2} out of {3} libraries built".format(
                 len(build), 
                 len(build) + len(not_build), 
                 len(lib_build), 
                 len(lib_build) + len(lib_not_build)
             ),
```

