# Comparing `tmp/amuse-mmams-2023.5.0.tar.gz` & `tmp/amuse-mmams-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-mmams-2023.5.0.tar", last modified: Wed May 17 10:19:16 2023, max compression
+gzip compressed data, was "amuse-mmams-2024.4.0.tar", last modified: Wed Apr 24 16:32:36 2024, max compression
```

## Comparing `amuse-mmams-2023.5.0.tar` & `amuse-mmams-2024.4.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.614417 amuse-mmams-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-mmams-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1183 2023-05-17 10:19:16.614220 amuse-mmams-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       58 2022-11-22 11:55:14.000000 amuse-mmams-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.603469 amuse-mmams-2023.5.0/amuse_mmams.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1183 2023-05-17 10:19:15.000000 amuse-mmams-2023.5.0/amuse_mmams.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     2859 2023-05-17 10:19:16.000000 amuse-mmams-2023.5.0/amuse_mmams.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:15.000000 amuse-mmams-2023.5.0/amuse_mmams.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:15.000000 amuse-mmams-2023.5.0/amuse_mmams.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:15.000000 amuse-mmams-2023.5.0/amuse_mmams.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-mmams-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:16.614476 amuse-mmams-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1770 2022-11-22 11:55:14.000000 amuse-mmams-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.601500 amuse-mmams-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.601552 amuse-mmams-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.601602 amuse-mmams-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.604385 amuse-mmams-2023.5.0/src/amuse/community/mmams/
--rw-r--r--   0 rieder     (501) staff       (20)     2094 2023-03-14 13:48:49.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       29 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     8976 2023-03-14 13:48:49.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/interface.cc
--rw-r--r--   0 rieder     (501) staff       (20)    27837 2023-03-14 13:48:49.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/interface.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.601729 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.604553 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/
--rw-r--r--   0 rieder     (501) staff       (20)     1450 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/CMakeLists.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.604918 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/
--rw-r--r--   0 rieder     (501) staff       (20)       27 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/CMakeLists.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.605620 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/eos/
--rw-r--r--   0 rieder     (501) staff       (20)      272 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/eos/CMakeLists.txt
--rw-r--r--   0 rieder     (501) staff       (20)     4789 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/eos/eos.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    10896 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/eos/eos.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.605957 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/gsl/
--rw-r--r--   0 rieder     (501) staff       (20)     1598 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/gsl/gslInterp.h
--rw-r--r--   0 rieder     (501) staff       (20)     1254 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/gsl/gslSpline.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.606496 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/include/
--rw-r--r--   0 rieder     (501) staff       (20)    12882 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/include/stdinc.h
--rw-r--r--   0 rieder     (501) staff       (20)     2457 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/include/units.h
--rw-r--r--   0 rieder     (501) staff       (20)     6444 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/include/vector.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.610334 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/
--rw-r--r--   0 rieder     (501) staff       (20)     1601 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/CMakeLists.txt
--rw-r--r--   0 rieder     (501) staff       (20)      626 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_energy.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3831 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_energy_gsl.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2879 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_extra.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      704 2023-03-14 13:48:49.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mass_loss.cpp
--rw-r--r--   0 rieder     (501) staff       (20)       54 2023-03-14 13:48:49.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mass_loss.h
--rw-r--r--   0 rieder     (501) staff       (20)     7702 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4724 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_consistently.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    14980 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_gsl.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    15187 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_gsl_adaptive.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     8692 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mixing.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2046 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mmas.h
--rw-r--r--   0 rieder     (501) staff       (20)     4002 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mmas2.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     8137 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/shock_heating.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      221 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/solve_hse.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      375 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/sort.h
--rw-r--r--   0 rieder     (501) staff       (20)     1112 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/sort_entropy.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3043 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/void.usm
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.610897 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/std/
--rw-r--r--   0 rieder     (501) staff       (20)      211 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/std/CMakeLists.txt
--rw-r--r--   0 rieder     (501) staff       (20)    12934 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/std/pgetopt.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     1949 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/std/trapfpe.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.612216 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/
--rw-r--r--   0 rieder     (501) staff       (20)      499 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/CMakeLists.txt
--rw-r--r--   0 rieder     (501) staff       (20)     2251 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/chemical_composition.h
--rw-r--r--   0 rieder     (501) staff       (20)     3651 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/ez2usm.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3307 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/mass_shell.h
--rw-r--r--   0 rieder     (501) staff       (20)     3060 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/usm.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     1389 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/usm.h
--rw-r--r--   0 rieder     (501) staff       (20)     4064 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/usm2col.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3900 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/usm2quad.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:15.000000 amuse-mmams-2023.5.0/src/amuse/community/mmams/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:16.613872 amuse-mmams-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-mmams-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-mmams-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-mmams-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.442552 amuse-mmams-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-mmams-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1214 2024-04-24 16:32:36.442351 amuse-mmams-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       58 2022-11-22 11:55:14.000000 amuse-mmams-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.442080 amuse-mmams-2024.4.0/amuse_mmams.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1214 2024-04-24 16:32:35.000000 amuse-mmams-2024.4.0/amuse_mmams.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     2860 2024-04-24 16:32:36.000000 amuse-mmams-2024.4.0/amuse_mmams.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:35.000000 amuse-mmams-2024.4.0/amuse_mmams.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:35.000000 amuse-mmams-2024.4.0/amuse_mmams.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:35.000000 amuse-mmams-2024.4.0/amuse_mmams.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-mmams-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:36.442624 amuse-mmams-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1575 2024-04-24 15:35:29.000000 amuse-mmams-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.430047 amuse-mmams-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.430098 amuse-mmams-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.430149 amuse-mmams-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.432941 amuse-mmams-2024.4.0/src/amuse/community/mmams/
+-rw-r--r--   0 rieder     (501) staff       (20)     2094 2023-03-14 13:48:49.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       29 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:35.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8976 2023-03-14 13:48:49.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/interface.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    27837 2023-03-14 13:48:49.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.430267 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.433112 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/
+-rw-r--r--   0 rieder     (501) staff       (20)     1450 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/CMakeLists.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.433272 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/
+-rw-r--r--   0 rieder     (501) staff       (20)       27 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/CMakeLists.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.433728 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/eos/
+-rw-r--r--   0 rieder     (501) staff       (20)      272 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/eos/CMakeLists.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     4789 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/eos/eos.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    10896 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/eos/eos.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.434107 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/gsl/
+-rw-r--r--   0 rieder     (501) staff       (20)     1598 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/gsl/gslInterp.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1254 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/gsl/gslSpline.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.434998 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/include/
+-rw-r--r--   0 rieder     (501) staff       (20)    12882 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/include/stdinc.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2457 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/include/units.h
+-rw-r--r--   0 rieder     (501) staff       (20)     6444 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/include/vector.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.438794 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/
+-rw-r--r--   0 rieder     (501) staff       (20)     1601 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/CMakeLists.txt
+-rw-r--r--   0 rieder     (501) staff       (20)      626 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_energy.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3831 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_energy_gsl.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2879 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_extra.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      704 2023-03-14 13:48:49.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mass_loss.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)       54 2023-03-14 13:48:49.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mass_loss.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7702 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4724 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_consistently.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    14980 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_gsl.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    15187 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_gsl_adaptive.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     8692 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mixing.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2046 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mmas.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4002 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mmas2.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     8137 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/shock_heating.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      221 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/solve_hse.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      375 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/sort.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1112 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/sort_entropy.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3043 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/void.usm
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.439528 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/std/
+-rw-r--r--   0 rieder     (501) staff       (20)      211 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/std/CMakeLists.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    12934 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/std/pgetopt.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1949 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/std/trapfpe.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.440649 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/
+-rw-r--r--   0 rieder     (501) staff       (20)      499 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/CMakeLists.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     2251 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/chemical_composition.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3651 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/ez2usm.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3307 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/mass_shell.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3060 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/usm.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1389 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/usm.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4064 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/usm2col.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3900 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/usm2quad.cpp
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:36.441888 amuse-mmams-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-mmams-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-mmams-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-mmams-2024.4.0/support/version.py
```

### Comparing `amuse-mmams-2023.5.0/PKG-INFO` & `amuse-mmams-2024.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-mmams
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - MMAMS
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
 
 This package installs the MMAMS community code for AMUSE.
```

### Comparing `amuse-mmams-2023.5.0/amuse_mmams.egg-info/PKG-INFO` & `amuse-mmams-2024.4.0/amuse_mmams.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-mmams
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - MMAMS
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
 
 This package installs the MMAMS community code for AMUSE.
```

### Comparing `amuse-mmams-2023.5.0/amuse_mmams.egg-info/SOURCES.txt` & `amuse-mmams-2024.4.0/amuse_mmams.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 amuse_mmams.egg-info/PKG-INFO
 amuse_mmams.egg-info/SOURCES.txt
 amuse_mmams.egg-info/dependency_links.txt
 amuse_mmams.egg-info/requires.txt
 amuse_mmams.egg-info/top_level.txt
 src/amuse/community/mmams/Makefile
 src/amuse/community/mmams/__init__.py
+src/amuse/community/mmams/_version.py
 src/amuse/community/mmams/interface.cc
 src/amuse/community/mmams/interface.py
-src/amuse/community/mmams/version.py
 src/amuse/community/mmams/src/mmas2/CMakeLists.txt
 src/amuse/community/mmams/src/mmas2/src/CMakeLists.txt
 src/amuse/community/mmams/src/mmas2/src/eos/CMakeLists.txt
 src/amuse/community/mmams/src/mmas2/src/eos/eos.cpp
 src/amuse/community/mmams/src/mmas2/src/eos/eos.h
 src/amuse/community/mmams/src/mmas2/src/gsl/gslInterp.h
 src/amuse/community/mmams/src/mmas2/src/gsl/gslSpline.h
```

### Comparing `amuse-mmams-2023.5.0/setup.py` & `amuse-mmams-2024.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.mmams.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/mmams/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/mmams/_version.py",
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
         'amuse.community.mmams': 'src/amuse/community/mmams',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/Makefile` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/interface.cc` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/interface.cc`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/interface.py` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/CMakeLists.txt` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/eos/eos.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/eos/eos.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/eos/eos.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/eos/eos.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/gsl/gslInterp.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/gsl/gslInterp.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/gsl/gslSpline.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/gsl/gslSpline.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/include/stdinc.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/include/stdinc.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/include/units.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/include/units.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/include/vector.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/include/vector.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/CMakeLists.txt` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_energy.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_energy.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_energy_gsl.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_energy_gsl.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_extra.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/compute_extra.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mass_loss.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mass_loss.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_consistently.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_consistently.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_gsl.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_gsl.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_gsl_adaptive.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/merge_stars_gsl_adaptive.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mixing.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mixing.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mmas.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mmas.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/mmas2.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/mmas2.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/shock_heating.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/shock_heating.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/sort_entropy.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/sort_entropy.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/mmas/void.usm` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/mmas/void.usm`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/std/pgetopt.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/std/pgetopt.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/std/trapfpe.c` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/std/trapfpe.c`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/chemical_composition.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/chemical_composition.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/ez2usm.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/ez2usm.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/mass_shell.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/mass_shell.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/usm.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/usm.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/usm.h` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/usm.h`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/usm2col.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/usm2col.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/src/amuse/community/mmams/src/mmas2/src/usm/usm2quad.cpp` & `amuse-mmams-2024.4.0/src/amuse/community/mmams/src/mmas2/src/usm/usm2quad.cpp`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/support/__init__.py` & `amuse-mmams-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/support/classifiers.py` & `amuse-mmams-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/support/config.py` & `amuse-mmams-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/support/generate_main.py` & `amuse-mmams-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/support/getsp.class` & `amuse-mmams-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/support/getsp.java` & `amuse-mmams-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/support/misc.py` & `amuse-mmams-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-mmams-2023.5.0/support/setup_codes.py` & `amuse-mmams-2024.4.0/support/setup_codes.py`

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

