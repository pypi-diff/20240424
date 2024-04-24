# Comparing `tmp/amuse-ph4-2023.5.0.tar.gz` & `tmp/amuse-ph4-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-ph4-2023.5.0.tar", last modified: Wed May 17 10:19:25 2023, max compression
+gzip compressed data, was "amuse-ph4-2024.4.0.tar", last modified: Wed Apr 24 16:32:43 2024, max compression
```

## Comparing `amuse-ph4-2023.5.0.tar` & `amuse-ph4-2024.4.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.928979 amuse-ph4-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-ph4-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1177 2023-05-17 10:19:25.928794 amuse-ph4-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       56 2022-11-22 11:55:14.000000 amuse-ph4-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.905644 amuse-ph4-2023.5.0/amuse_ph4.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1177 2023-05-17 10:19:23.000000 amuse-ph4-2023.5.0/amuse_ph4.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     3060 2023-05-17 10:19:25.000000 amuse-ph4-2023.5.0/amuse_ph4.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:23.000000 amuse-ph4-2023.5.0/amuse_ph4.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:23.000000 amuse-ph4-2023.5.0/amuse_ph4.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:23.000000 amuse-ph4-2023.5.0/amuse_ph4.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-ph4-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:25.929041 amuse-ph4-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1756 2022-11-22 11:55:14.000000 amuse-ph4-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.903727 amuse-ph4-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.903782 amuse-ph4-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.903833 amuse-ph4-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.909284 amuse-ph4-2023.5.0/src/amuse/community/ph4/
--rw-r--r--   0 rieder     (501) staff       (20)     2182 2023-03-14 13:48:49.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       44 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     1007 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/binary_hist.py
--rw-r--r--   0 rieder     (501) staff       (20)    22773 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/interface.cc
--rw-r--r--   0 rieder     (501) staff       (20)    25871 2023-03-14 13:48:49.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)     3376 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/plot_energy_vs_t.py
--rw-r--r--   0 rieder     (501) staff       (20)     3250 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/plot_kT_vs_t.py
--rwxr-xr-x   0 rieder     (501) staff       (20)     7704 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/plotq.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.925919 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/
--rw-r--r--   0 rieder     (501) staff       (20)     2238 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/GPU_options.txt
--rw-r--r--   0 rieder     (501) staff       (20)     2009 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     3945 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/Makefile.ph4
--rw-r--r--   0 rieder     (501) staff       (20)     4284 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/README
--rw-r--r--   0 rieder     (501) staff       (20)      217 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/TODO
--rw-r--r--   0 rieder     (501) staff       (20)    32321 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/analyze.cc
--rw-r--r--   0 rieder     (501) staff       (20)     5738 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/close_encounter.cc
--rw-r--r--   0 rieder     (501) staff       (20)      513 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/ctest_nstab.cc
--rw-r--r--   0 rieder     (501) staff       (20)     1673 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/debug.cc
--rw-r--r--   0 rieder     (501) staff       (20)      327 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/debug.h
--rw-r--r--   0 rieder     (501) staff       (20)     4435 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/diag.cc
--rw-r--r--   0 rieder     (501) staff       (20)      417 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/f2c.c
--rw-r--r--   0 rieder     (501) staff       (20)      444 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/f2c.h
--rw-r--r--   0 rieder     (501) staff       (20)      672 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/ftest_nstab.f
--rw-r--r--   0 rieder     (501) staff       (20)    22016 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/gpu.cc
--rw-r--r--   0 rieder     (501) staff       (20)     2878 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/grape.cc
--rw-r--r--   0 rieder     (501) staff       (20)     3188 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/grape.h
--rw-r--r--   0 rieder     (501) staff       (20)     4545 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/hdyn.cc
--rw-r--r--   0 rieder     (501) staff       (20)     9879 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/hdyn.h
--rw-r--r--   0 rieder     (501) staff       (20)    24329 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/idata.cc
--rw-r--r--   0 rieder     (501) staff       (20)     1727 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/idata.h
--rw-r--r--   0 rieder     (501) staff       (20)    30657 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/jdata.cc
--rw-r--r--   0 rieder     (501) staff       (20)     7106 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/jdata.h
--rw-r--r--   0 rieder     (501) staff       (20)    54348 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/kepler.cc
--rw-r--r--   0 rieder     (501) staff       (20)     8572 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/kepler.h
--rw-r--r--   0 rieder     (501) staff       (20)    14703 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/nstab.c
--rw-r--r--   0 rieder     (501) staff       (20)     6304 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/nstab.f
--rw-r--r--   0 rieder     (501) staff       (20)      124 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/nstab.h
--rw-r--r--   0 rieder     (501) staff       (20)    19398 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/old_close_encounter.cc
--rw-r--r--   0 rieder     (501) staff       (20)     9626 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/parallel_hermite_4.cc
--rw-r--r--   0 rieder     (501) staff       (20)    15801 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer100.in
--rw-r--r--   0 rieder     (501) staff       (20)  2965542 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer16k.in
--rw-r--r--   0 rieder     (501) staff       (20)   153739 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer1k.in
--rw-r--r--   0 rieder     (501) staff       (20)   741414 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer4k.in
--rw-r--r--   0 rieder     (501) staff       (20)  1482790 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer8k.in
--rw-r--r--   0 rieder     (501) staff       (20)     1578 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer_test.in
--rw-r--r--   0 rieder     (501) staff       (20)      530 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/random_nstab.cc
--rw-r--r--   0 rieder     (501) staff       (20)     1967 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/rescale_smallN.cc
--rw-r--r--   0 rieder     (501) staff       (20)    10761 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/scheduler.cc
--rw-r--r--   0 rieder     (501) staff       (20)     2251 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/scheduler.h
--rw-r--r--   0 rieder     (501) staff       (20)    36765 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/smallN.cc
--rw-r--r--   0 rieder     (501) staff       (20)    23341 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/smallN_unpert.cc
--rw-r--r--   0 rieder     (501) staff       (20)     2105 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/stdinc.h
--rwxr-xr-x   0 rieder     (501) staff       (20)      359 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/test.sh
--rw-r--r--   0 rieder     (501) staff       (20)     3052 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/test_hosts.cc
--rwxr-xr-x   0 rieder     (501) staff       (20)      443 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/test_nstab.sh
--rw-r--r--   0 rieder     (501) staff       (20)    31606 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/two_body.cc
--rw-r--r--   0 rieder     (501) staff       (20)     5310 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/util.cc
--rw-r--r--   0 rieder     (501) staff       (20)     5535 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/src/vec.h
--rw-r--r--   0 rieder     (501) staff       (20)     8236 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/test_multiples.py
--rw-r--r--   0 rieder     (501) staff       (20)    17202 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/test_multiples2.py
--rw-r--r--   0 rieder     (501) staff       (20)    11044 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/test_ph4.py
--rw-r--r--   0 rieder     (501) staff       (20)    10277 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/test_sync.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.927113 amuse-ph4-2023.5.0/src/amuse/community/ph4/util/
--rw-r--r--   0 rieder     (501) staff       (20)     8274 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/util/initialize_system.py
--rw-r--r--   0 rieder     (501) staff       (20)      340 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/util/multiples.sh
--rw-r--r--   0 rieder     (501) staff       (20)    11443 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/util/plot_smalln_data.py
--rwxr-xr-x   0 rieder     (501) staff       (20)     7704 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/util/plotq.py
--rw-r--r--   0 rieder     (501) staff       (20)     9744 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/util/run_ph4.py
--rw-r--r--   0 rieder     (501) staff       (20)    10630 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/util/utils.py
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:23.000000 amuse-ph4-2023.5.0/src/amuse/community/ph4/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:25.928518 amuse-ph4-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-ph4-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-ph4-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-ph4-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.022589 amuse-ph4-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-ph4-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1208 2024-04-24 16:32:43.022375 amuse-ph4-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       56 2022-11-22 11:55:14.000000 amuse-ph4-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.022057 amuse-ph4-2024.4.0/amuse_ph4.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1208 2024-04-24 16:32:42.000000 amuse-ph4-2024.4.0/amuse_ph4.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     3061 2024-04-24 16:32:42.000000 amuse-ph4-2024.4.0/amuse_ph4.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:42.000000 amuse-ph4-2024.4.0/amuse_ph4.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:42.000000 amuse-ph4-2024.4.0/amuse_ph4.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:42.000000 amuse-ph4-2024.4.0/amuse_ph4.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-ph4-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:43.022645 amuse-ph4-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1563 2024-04-24 15:35:29.000000 amuse-ph4-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.004031 amuse-ph4-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.004081 amuse-ph4-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.004131 amuse-ph4-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.007594 amuse-ph4-2024.4.0/src/amuse/community/ph4/
+-rw-r--r--   0 rieder     (501) staff       (20)     2182 2023-03-14 13:48:49.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       44 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:42.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1007 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/binary_hist.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22513 2024-04-24 15:35:29.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/interface.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    25871 2023-03-14 13:48:49.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3376 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/plot_energy_vs_t.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3250 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/plot_kT_vs_t.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)     7704 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/plotq.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.019562 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     2238 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/GPU_options.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     2009 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     3945 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/Makefile.ph4
+-rw-r--r--   0 rieder     (501) staff       (20)     4284 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/README
+-rw-r--r--   0 rieder     (501) staff       (20)      217 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/TODO
+-rw-r--r--   0 rieder     (501) staff       (20)    32321 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/analyze.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     5738 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/close_encounter.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      513 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/ctest_nstab.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     1673 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/debug.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      327 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/debug.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4435 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/diag.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/f2c.c
+-rw-r--r--   0 rieder     (501) staff       (20)      444 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/f2c.h
+-rw-r--r--   0 rieder     (501) staff       (20)      672 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/ftest_nstab.f
+-rw-r--r--   0 rieder     (501) staff       (20)    22016 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/gpu.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     2878 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/grape.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     3188 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/grape.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4545 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/hdyn.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     9879 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/hdyn.h
+-rw-r--r--   0 rieder     (501) staff       (20)    24329 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/idata.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     1727 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/idata.h
+-rw-r--r--   0 rieder     (501) staff       (20)    30657 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/jdata.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     7106 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/jdata.h
+-rw-r--r--   0 rieder     (501) staff       (20)    54348 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/kepler.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     8572 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/kepler.h
+-rw-r--r--   0 rieder     (501) staff       (20)    14703 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/nstab.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6304 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/nstab.f
+-rw-r--r--   0 rieder     (501) staff       (20)      124 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/nstab.h
+-rw-r--r--   0 rieder     (501) staff       (20)    19398 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/old_close_encounter.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     9626 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/parallel_hermite_4.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    15801 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer100.in
+-rw-r--r--   0 rieder     (501) staff       (20)  2965542 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer16k.in
+-rw-r--r--   0 rieder     (501) staff       (20)   153739 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer1k.in
+-rw-r--r--   0 rieder     (501) staff       (20)   741414 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer4k.in
+-rw-r--r--   0 rieder     (501) staff       (20)  1482790 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer8k.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1578 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer_test.in
+-rw-r--r--   0 rieder     (501) staff       (20)      530 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/random_nstab.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     1967 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/rescale_smallN.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    10761 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/scheduler.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     2251 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/scheduler.h
+-rw-r--r--   0 rieder     (501) staff       (20)    36765 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/smallN.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    23341 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/smallN_unpert.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     2105 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/stdinc.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)      359 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/test.sh
+-rw-r--r--   0 rieder     (501) staff       (20)     3052 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/test_hosts.cc
+-rwxr-xr-x   0 rieder     (501) staff       (20)      443 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/test_nstab.sh
+-rw-r--r--   0 rieder     (501) staff       (20)    31606 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/two_body.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     5310 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/util.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     5535 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/src/vec.h
+-rw-r--r--   0 rieder     (501) staff       (20)     8236 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/test_multiples.py
+-rw-r--r--   0 rieder     (501) staff       (20)    17202 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/test_multiples2.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11044 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/test_ph4.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10277 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/test_sync.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.020528 amuse-ph4-2024.4.0/src/amuse/community/ph4/util/
+-rw-r--r--   0 rieder     (501) staff       (20)     8274 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/util/initialize_system.py
+-rw-r--r--   0 rieder     (501) staff       (20)      340 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/util/multiples.sh
+-rw-r--r--   0 rieder     (501) staff       (20)    11443 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/util/plot_smalln_data.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)     7704 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/util/plotq.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9744 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/util/run_ph4.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10630 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/src/amuse/community/ph4/util/utils.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:43.021856 amuse-ph4-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-ph4-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-ph4-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-ph4-2024.4.0/support/version.py
```

### Comparing `amuse-ph4-2023.5.0/PKG-INFO` & `amuse-ph4-2024.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-ph4
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - ph4
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
 
 This package installs the ph4 community code for AMUSE.
```

### Comparing `amuse-ph4-2023.5.0/amuse_ph4.egg-info/PKG-INFO` & `amuse-ph4-2024.4.0/amuse_ph4.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-ph4
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - ph4
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
 
 This package installs the ph4 community code for AMUSE.
```

### Comparing `amuse-ph4-2023.5.0/amuse_ph4.egg-info/SOURCES.txt` & `amuse-ph4-2024.4.0/amuse_ph4.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 amuse_ph4.egg-info/PKG-INFO
 amuse_ph4.egg-info/SOURCES.txt
 amuse_ph4.egg-info/dependency_links.txt
 amuse_ph4.egg-info/requires.txt
 amuse_ph4.egg-info/top_level.txt
 src/amuse/community/ph4/Makefile
 src/amuse/community/ph4/__init__.py
+src/amuse/community/ph4/_version.py
 src/amuse/community/ph4/binary_hist.py
 src/amuse/community/ph4/interface.cc
 src/amuse/community/ph4/interface.py
 src/amuse/community/ph4/plot_energy_vs_t.py
 src/amuse/community/ph4/plot_kT_vs_t.py
 src/amuse/community/ph4/plotq.py
 src/amuse/community/ph4/test_multiples.py
 src/amuse/community/ph4/test_multiples2.py
 src/amuse/community/ph4/test_ph4.py
 src/amuse/community/ph4/test_sync.py
-src/amuse/community/ph4/version.py
 src/amuse/community/ph4/src/GPU_options.txt
 src/amuse/community/ph4/src/Makefile
 src/amuse/community/ph4/src/Makefile.ph4
 src/amuse/community/ph4/src/README
 src/amuse/community/ph4/src/TODO
 src/amuse/community/ph4/src/analyze.cc
 src/amuse/community/ph4/src/close_encounter.cc
```

### Comparing `amuse-ph4-2023.5.0/setup.py` & `amuse-ph4-2024.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.ph4.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/ph4/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/ph4/_version.py",
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
         'amuse.community.ph4': 'src/amuse/community/ph4',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/Makefile` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/binary_hist.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/binary_hist.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/interface.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/interface.cc`

 * *Files 2% similar despite different names*

```diff
@@ -575,25 +575,14 @@
     if (j < 0) return -1;
     *vx = jd->vel[j][0];
     *vy = jd->vel[j][1];
     *vz = jd->vel[j][2];
     return 0;
 }
 
-int set_acceleration(int index_of_the_particle,
-		     double ax, double ay, double az)
-{
-    int j = jd->get_inverse_id(index_of_the_particle);
-    if (j < 0) return -1;
-    jd->acc[j][0] = ax;
-    jd->acc[j][1] = ay;
-    jd->acc[j][2] = az;
-    return 0;
-}
-
 int get_acceleration(int index_of_the_particle,
 		     double * ax, double * ay, double * az)
 {
     int j = jd->get_inverse_id(index_of_the_particle);
     if (j < 0) return -1;
     *ax = jd->acc[j][0];
     *ay = jd->acc[j][1];
```

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/interface.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/plot_energy_vs_t.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/plot_energy_vs_t.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/plot_kT_vs_t.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/plot_kT_vs_t.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/plotq.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/plotq.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/GPU_options.txt` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/GPU_options.txt`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/Makefile` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/Makefile.ph4` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/Makefile.ph4`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/README` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/README`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/analyze.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/analyze.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/close_encounter.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/close_encounter.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/ctest_nstab.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/ctest_nstab.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/debug.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/debug.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/diag.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/diag.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/ftest_nstab.f` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/ftest_nstab.f`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/gpu.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/gpu.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/grape.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/grape.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/grape.h` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/grape.h`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/hdyn.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/hdyn.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/hdyn.h` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/hdyn.h`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/idata.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/idata.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/idata.h` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/idata.h`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/jdata.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/jdata.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/jdata.h` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/jdata.h`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/kepler.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/kepler.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/kepler.h` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/kepler.h`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/nstab.c` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/nstab.c`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/nstab.f` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/nstab.f`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/old_close_encounter.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/old_close_encounter.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/parallel_hermite_4.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/parallel_hermite_4.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer100.in` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer100.in`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer16k.in` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer16k.in`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer1k.in` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer1k.in`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer4k.in` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer4k.in`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer8k.in` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer8k.in`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/plummer_test.in` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/plummer_test.in`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/random_nstab.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/random_nstab.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/rescale_smallN.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/rescale_smallN.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/scheduler.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/scheduler.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/scheduler.h` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/scheduler.h`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/smallN.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/smallN.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/smallN_unpert.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/smallN_unpert.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/stdinc.h` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/stdinc.h`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/test_hosts.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/test_hosts.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/two_body.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/two_body.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/util.cc` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/util.cc`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/src/vec.h` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/src/vec.h`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/test_multiples.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/test_multiples.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/test_multiples2.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/test_multiples2.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/test_ph4.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/test_ph4.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/test_sync.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/test_sync.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/util/initialize_system.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/util/initialize_system.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/util/plot_smalln_data.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/util/plot_smalln_data.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/util/plotq.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/util/plotq.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/util/run_ph4.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/util/run_ph4.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/src/amuse/community/ph4/util/utils.py` & `amuse-ph4-2024.4.0/src/amuse/community/ph4/util/utils.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/support/__init__.py` & `amuse-ph4-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/support/classifiers.py` & `amuse-ph4-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/support/config.py` & `amuse-ph4-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/support/generate_main.py` & `amuse-ph4-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/support/getsp.class` & `amuse-ph4-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/support/getsp.java` & `amuse-ph4-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/support/misc.py` & `amuse-ph4-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-ph4-2023.5.0/support/setup_codes.py` & `amuse-ph4-2024.4.0/support/setup_codes.py`

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

