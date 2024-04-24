# Comparing `tmp/amuse-gadget2-2023.5.0.tar.gz` & `tmp/amuse-gadget2-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-gadget2-2023.5.0.tar", last modified: Wed May 17 10:18:44 2023, max compression
+gzip compressed data, was "amuse-gadget2-2024.4.0.tar", last modified: Wed Apr 24 16:32:17 2024, max compression
```

## Comparing `amuse-gadget2-2023.5.0.tar` & `amuse-gadget2-2024.4.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:44.765818 amuse-gadget2-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-gadget2-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1189 2023-05-17 10:18:44.765663 amuse-gadget2-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       60 2022-11-22 11:55:14.000000 amuse-gadget2-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:44.756096 amuse-gadget2-2023.5.0/amuse_gadget2.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1189 2023-05-17 10:18:43.000000 amuse-gadget2-2023.5.0/amuse_gadget2.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     2479 2023-05-17 10:18:44.000000 amuse-gadget2-2023.5.0/amuse_gadget2.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:18:43.000000 amuse-gadget2-2023.5.0/amuse_gadget2.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:18:43.000000 amuse-gadget2-2023.5.0/amuse_gadget2.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:18:43.000000 amuse-gadget2-2023.5.0/amuse_gadget2.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-gadget2-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:18:44.765861 amuse-gadget2-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1784 2022-11-22 11:55:14.000000 amuse-gadget2-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:44.754734 amuse-gadget2-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:44.754787 amuse-gadget2-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:44.754837 amuse-gadget2-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:44.758368 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/
--rw-r--r--   0 rieder     (501) staff       (20)     2842 2023-03-14 13:48:49.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     1788 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/README
--rw-r--r--   0 rieder     (501) staff       (20)       31 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    88415 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/interface.cc
--rw-r--r--   0 rieder     (501) staff       (20)     1094 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/interface.h
--rw-r--r--   0 rieder     (501) staff       (20)    99817 2023-03-14 13:48:49.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)     2682 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/makefile_options_nogravity
--rw-r--r--   0 rieder     (501) staff       (20)     2683 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/makefile_options_normal
--rw-r--r--   0 rieder     (501) staff       (20)     2682 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/makefile_options_periodic
--rw-r--r--   0 rieder     (501) staff       (20)     2681 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/makefile_options_periodic_nogravity
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:44.764121 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/
--rw-r--r--   0 rieder     (501) staff       (20)     7155 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/Doxyfile
--rw-r--r--   0 rieder     (501) staff       (20)    20108 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     2901 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/accel.c
--rw-r--r--   0 rieder     (501) staff       (20)     5585 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/allocate.c
--rw-r--r--   0 rieder     (501) staff       (20)     9918 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/allvars.c
--rw-r--r--   0 rieder     (501) staff       (20)    40368 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/allvars.h
--rw-r--r--   0 rieder     (501) staff       (20)    21630 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/begrun.c
--rw-r--r--   0 rieder     (501) staff       (20)    17712 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/density.c
--rw-r--r--   0 rieder     (501) staff       (20)     6897 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/density_at_pos.c
--rw-r--r--   0 rieder     (501) staff       (20)    32138 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/domain.c
--rw-r--r--   0 rieder     (501) staff       (20)     6089 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/driftfac.c
--rw-r--r--   0 rieder     (501) staff       (20)     1350 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/endrun.c
--rw-r--r--   0 rieder     (501) staff       (20)    78328 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/forcetree.c
--rw-r--r--   0 rieder     (501) staff       (20)     7458 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/global.c
--rw-r--r--   0 rieder     (501) staff       (20)    15868 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/gravtree.c
--rw-r--r--   0 rieder     (501) staff       (20)     9598 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/gravtree_forcetest.c
--rw-r--r--   0 rieder     (501) staff       (20)    17214 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/hydra.c
--rw-r--r--   0 rieder     (501) staff       (20)     7376 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/init.c
--rw-r--r--   0 rieder     (501) staff       (20)    28792 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/io.c
--rw-r--r--   0 rieder     (501) staff       (20)     2936 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/longrange.c
--rw-r--r--   0 rieder     (501) staff       (20)    39633 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/main.c
--rw-r--r--   0 rieder     (501) staff       (20)     2683 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/makefile_options
--rw-r--r--   0 rieder     (501) staff       (20)    10879 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/ngb.c
--rw-r--r--   0 rieder     (501) staff       (20)     8534 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/peano.c
--rw-r--r--   0 rieder     (501) staff       (20)    45539 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/pm_nonperiodic.c
--rw-r--r--   0 rieder     (501) staff       (20)    35340 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/pm_periodic.c
--rw-r--r--   0 rieder     (501) staff       (20)     8672 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/potential.c
--rw-r--r--   0 rieder     (501) staff       (20)     3560 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/predict.c
--rw-r--r--   0 rieder     (501) staff       (20)     7538 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/proto.h
--rw-r--r--   0 rieder     (501) staff       (20)    20901 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/read_ic.c
--rw-r--r--   0 rieder     (501) staff       (20)     8558 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/restart.c
--rw-r--r--   0 rieder     (501) staff       (20)    11742 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/run.c
--rw-r--r--   0 rieder     (501) staff       (20)    18068 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/sigvel.c
--rw-r--r--   0 rieder     (501) staff       (20)     2738 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/system.c
--rw-r--r--   0 rieder     (501) staff       (20)      957 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/tags.h
--rw-r--r--   0 rieder     (501) staff       (20)    20165 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/timestep.c
--rw-r--r--   0 rieder     (501) staff       (20)    36542 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/timestep_limit.c
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:18:43.000000 amuse-gadget2-2023.5.0/src/amuse/community/gadget2/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:44.765453 amuse-gadget2-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-gadget2-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-gadget2-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-gadget2-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:17.599167 amuse-gadget2-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-gadget2-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1220 2024-04-24 16:32:17.598976 amuse-gadget2-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       60 2022-11-22 11:55:14.000000 amuse-gadget2-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:17.598704 amuse-gadget2-2024.4.0/amuse_gadget2.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1220 2024-04-24 16:32:16.000000 amuse-gadget2-2024.4.0/amuse_gadget2.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     2480 2024-04-24 16:32:17.000000 amuse-gadget2-2024.4.0/amuse_gadget2.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:16.000000 amuse-gadget2-2024.4.0/amuse_gadget2.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:16.000000 amuse-gadget2-2024.4.0/amuse_gadget2.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:16.000000 amuse-gadget2-2024.4.0/amuse_gadget2.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-gadget2-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:17.599221 amuse-gadget2-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1587 2024-04-24 15:35:29.000000 amuse-gadget2-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:17.587257 amuse-gadget2-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:17.587308 amuse-gadget2-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:17.587359 amuse-gadget2-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:17.590591 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/
+-rw-r--r--   0 rieder     (501) staff       (20)     2842 2023-03-14 13:48:49.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     1788 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/README
+-rw-r--r--   0 rieder     (501) staff       (20)       31 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:16.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)    88355 2024-04-24 15:35:29.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/interface.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     1094 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/interface.h
+-rw-r--r--   0 rieder     (501) staff       (20)    99817 2023-03-14 13:48:49.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2682 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/makefile_options_nogravity
+-rw-r--r--   0 rieder     (501) staff       (20)     2683 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/makefile_options_normal
+-rw-r--r--   0 rieder     (501) staff       (20)     2682 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/makefile_options_periodic
+-rw-r--r--   0 rieder     (501) staff       (20)     2681 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/makefile_options_periodic_nogravity
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:17.597242 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     7155 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/Doxyfile
+-rw-r--r--   0 rieder     (501) staff       (20)    20108 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     2901 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/accel.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5585 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/allocate.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9918 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/allvars.c
+-rw-r--r--   0 rieder     (501) staff       (20)    40368 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/allvars.h
+-rw-r--r--   0 rieder     (501) staff       (20)    21630 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/begrun.c
+-rw-r--r--   0 rieder     (501) staff       (20)    17712 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/density.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6897 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/density_at_pos.c
+-rw-r--r--   0 rieder     (501) staff       (20)    32138 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/domain.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6089 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/driftfac.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1350 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/endrun.c
+-rw-r--r--   0 rieder     (501) staff       (20)    78328 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/forcetree.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7458 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/global.c
+-rw-r--r--   0 rieder     (501) staff       (20)    15868 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/gravtree.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9598 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/gravtree_forcetest.c
+-rw-r--r--   0 rieder     (501) staff       (20)    17214 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/hydra.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7376 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/init.c
+-rw-r--r--   0 rieder     (501) staff       (20)    28792 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/io.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2936 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/longrange.c
+-rw-r--r--   0 rieder     (501) staff       (20)    39633 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/main.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2683 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/makefile_options
+-rw-r--r--   0 rieder     (501) staff       (20)    10879 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/ngb.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8534 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/peano.c
+-rw-r--r--   0 rieder     (501) staff       (20)    45539 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/pm_nonperiodic.c
+-rw-r--r--   0 rieder     (501) staff       (20)    35340 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/pm_periodic.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8672 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/potential.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3560 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/predict.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7538 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/proto.h
+-rw-r--r--   0 rieder     (501) staff       (20)    20901 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/read_ic.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8558 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/restart.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11742 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/run.c
+-rw-r--r--   0 rieder     (501) staff       (20)    18068 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/sigvel.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2738 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/system.c
+-rw-r--r--   0 rieder     (501) staff       (20)      957 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/tags.h
+-rw-r--r--   0 rieder     (501) staff       (20)    20165 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/timestep.c
+-rw-r--r--   0 rieder     (501) staff       (20)    36542 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/timestep_limit.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:17.598526 amuse-gadget2-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-gadget2-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-gadget2-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-gadget2-2024.4.0/support/version.py
```

### Comparing `amuse-gadget2-2023.5.0/PKG-INFO` & `amuse-gadget2-2024.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-gadget2
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Gadget2
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
 
 This package installs the Gadget2 community code for AMUSE.
```

### Comparing `amuse-gadget2-2023.5.0/amuse_gadget2.egg-info/PKG-INFO` & `amuse-gadget2-2024.4.0/amuse_gadget2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-gadget2
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Gadget2
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
 
 This package installs the Gadget2 community code for AMUSE.
```

### Comparing `amuse-gadget2-2023.5.0/amuse_gadget2.egg-info/SOURCES.txt` & `amuse-gadget2-2024.4.0/amuse_gadget2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 amuse_gadget2.egg-info/SOURCES.txt
 amuse_gadget2.egg-info/dependency_links.txt
 amuse_gadget2.egg-info/requires.txt
 amuse_gadget2.egg-info/top_level.txt
 src/amuse/community/gadget2/Makefile
 src/amuse/community/gadget2/README
 src/amuse/community/gadget2/__init__.py
+src/amuse/community/gadget2/_version.py
 src/amuse/community/gadget2/interface.cc
 src/amuse/community/gadget2/interface.h
 src/amuse/community/gadget2/interface.py
 src/amuse/community/gadget2/makefile_options_nogravity
 src/amuse/community/gadget2/makefile_options_normal
 src/amuse/community/gadget2/makefile_options_periodic
 src/amuse/community/gadget2/makefile_options_periodic_nogravity
-src/amuse/community/gadget2/version.py
 src/amuse/community/gadget2/src/Doxyfile
 src/amuse/community/gadget2/src/Makefile
 src/amuse/community/gadget2/src/accel.c
 src/amuse/community/gadget2/src/allocate.c
 src/amuse/community/gadget2/src/allvars.c
 src/amuse/community/gadget2/src/allvars.h
 src/amuse/community/gadget2/src/begrun.c
```

### Comparing `amuse-gadget2-2023.5.0/setup.py` & `amuse-gadget2-2024.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.gadget2.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/gadget2/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/gadget2/_version.py",
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
         'amuse.community.gadget2': 'src/amuse/community/gadget2',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/Makefile` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/README` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/README`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/interface.cc` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/interface.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1449,14 +1449,15 @@
 
 int check_counts_and_free(int *count, int length){
     int errors = 0;
     if(ThisTask) {
 #ifndef NOMPI
         MPI_Reduce(count, NULL, length, MPI_INT, MPI_SUM, 0, GADGET_WORLD);
 #endif
+        delete[] count;
         return 0;
     } else {
 #ifndef NOMPI
         MPI_Reduce(MPI_IN_PLACE, count, length, MPI_INT, MPI_SUM, 0, GADGET_WORLD);
 #endif
         for (int i = 0; i < length; i++){
             if (count[i] != 1)
@@ -2109,18 +2110,14 @@
             ay[i] *= All.Time;
             az[i] *= All.Time;
         }
     }
     return result;
 }
 
-int set_acceleration(int index, double ax, double ay, double az){
-    return -2;
-}
-
 int get_internal_energy(int *index, double *internal_energy, int length){
     int errors = 0;
     double *buffer = new double[length];
     int *count = new int[length];
     int local_index;
 #ifndef ISOTHERM_EQS
     double a3;
```

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/interface.h` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/interface.h`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/interface.py` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/makefile_options_nogravity` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/makefile_options_nogravity`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/makefile_options_normal` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/makefile_options_normal`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/makefile_options_periodic` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/makefile_options_periodic`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/makefile_options_periodic_nogravity` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/makefile_options_periodic_nogravity`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/Doxyfile` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/Doxyfile`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/Makefile` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/accel.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/accel.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/allocate.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/allocate.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/allvars.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/allvars.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/allvars.h` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/allvars.h`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/begrun.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/begrun.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/density.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/density.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/density_at_pos.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/density_at_pos.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/domain.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/domain.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/driftfac.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/driftfac.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/endrun.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/endrun.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/forcetree.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/forcetree.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/global.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/global.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/gravtree.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/gravtree.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/gravtree_forcetest.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/gravtree_forcetest.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/hydra.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/hydra.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/init.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/init.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/io.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/io.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/longrange.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/longrange.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/main.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/main.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/makefile_options` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/makefile_options`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/ngb.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/ngb.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/peano.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/peano.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/pm_nonperiodic.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/pm_nonperiodic.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/pm_periodic.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/pm_periodic.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/potential.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/potential.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/predict.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/predict.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/proto.h` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/proto.h`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/read_ic.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/read_ic.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/restart.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/restart.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/run.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/run.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/sigvel.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/sigvel.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/system.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/system.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/tags.h` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/tags.h`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/timestep.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/timestep.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/src/amuse/community/gadget2/src/timestep_limit.c` & `amuse-gadget2-2024.4.0/src/amuse/community/gadget2/src/timestep_limit.c`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/support/__init__.py` & `amuse-gadget2-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/support/classifiers.py` & `amuse-gadget2-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/support/config.py` & `amuse-gadget2-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/support/generate_main.py` & `amuse-gadget2-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/support/getsp.class` & `amuse-gadget2-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/support/getsp.java` & `amuse-gadget2-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/support/misc.py` & `amuse-gadget2-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-gadget2-2023.5.0/support/setup_codes.py` & `amuse-gadget2-2024.4.0/support/setup_codes.py`

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

