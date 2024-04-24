# Comparing `tmp/amuse-framework-2023.5.0.tar.gz` & `tmp/amuse_framework-2024.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-framework-2023.5.0.tar", last modified: Wed May 17 10:18:42 2023, max compression
+gzip compressed data, was "amuse_framework-2024.4.0rc1.tar", last modified: Wed Apr 24 16:07:48 2024, max compression
```

## Comparing `amuse-framework-2023.5.0.tar` & `amuse_framework-2024.4.0rc1.tar`

### file list

```diff
@@ -1,289 +1,292 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.386463 amuse-framework-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      639 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     2471 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)     1242 2023-05-17 10:18:42.386313 amuse-framework-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)      101 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.350414 amuse-framework-2023.5.0/bin/
--rwxr-xr-x   0 rieder     (501) staff       (20)      328 2022-11-22 11:55:13.000000 amuse-framework-2023.5.0/bin/amuse-tutorial
--rw-r--r--   0 rieder     (501) staff       (20)      728 2022-11-22 11:55:13.000000 amuse-framework-2023.5.0/bin/amusifier.in
--rw-r--r--   0 rieder     (501) staff       (20)    49446 2023-02-28 13:39:09.000000 amuse-framework-2023.5.0/config.guess
--rw-r--r--   0 rieder     (501) staff       (20)     2814 2022-11-22 11:55:13.000000 amuse-framework-2023.5.0/config.mk.in
--rw-r--r--   0 rieder     (501) staff       (20)    34424 2023-02-28 13:39:09.000000 amuse-framework-2023.5.0/config.sub
--rwxr-xr-x   0 rieder     (501) staff       (20)   412359 2023-03-22 19:10:26.000000 amuse-framework-2023.5.0/configure
--rwxr-xr-x   0 rieder     (501) staff       (20)    15358 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/install-sh
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.346798 amuse-framework-2023.5.0/lib/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.350821 amuse-framework-2023.5.0/lib/amuse_mpi/
--rw-r--r--   0 rieder     (501) staff       (20)      499 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/amuse_mpi/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)      335 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/amuse_mpi/amuse_mpi.c
--rw-r--r--   0 rieder     (501) staff       (20)      212 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/amuse_mpi/amuse_mpi.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.351340 amuse-framework-2023.5.0/lib/forsockets/
--rw-r--r--   0 rieder     (501) staff       (20)      494 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/forsockets/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     5068 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/forsockets/forsockets.c
--rw-r--r--   0 rieder     (501) staff       (20)      853 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/forsockets/forsockets.h
--rw-r--r--   0 rieder     (501) staff       (20)     4782 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/forsockets/forsocketsf.f90
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.351741 amuse-framework-2023.5.0/lib/g6/
--rw-r--r--   0 rieder     (501) staff       (20)      242 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/g6/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)    12542 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/g6/g6lib.c
--rw-r--r--   0 rieder     (501) staff       (20)     3957 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/g6/g6lib.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.351991 amuse-framework-2023.5.0/lib/sapporo_2/
--rw-r--r--   0 rieder     (501) staff       (20)     1469 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/sapporo_2/Makefile
--rwxr-xr-x   0 rieder     (501) staff       (20)     2548 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_2/download.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.353711 amuse-framework-2023.5.0/lib/sapporo_light/
--rw-r--r--   0 rieder     (501) staff       (20)     1339 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/sapporo_light/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)      641 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/README
--rw-r--r--   0 rieder     (501) staff       (20)    11568 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/dev_evaluate_gravity.cu
--rw-r--r--   0 rieder     (501) staff       (20)    12542 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/g6lib.c
--rw-r--r--   0 rieder     (501) staff       (20)     1461 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/g6lib.h
--rw-r--r--   0 rieder     (501) staff       (20)     5486 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/host_evaluate_gravity.cu
--rw-r--r--   0 rieder     (501) staff       (20)     7585 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporo.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4632 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporo.h
--rw-r--r--   0 rieder     (501) staff       (20)     2434 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporoG6lib.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2964 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporo_defs.h
--rw-r--r--   0 rieder     (501) staff       (20)      530 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/sapporo_multi.h
--rw-r--r--   0 rieder     (501) staff       (20)     5983 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/sapporo_light/send_fetch_data.cpp
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.354526 amuse-framework-2023.5.0/lib/simple_hash/
--rw-r--r--   0 rieder     (501) staff       (20)      619 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/simple_hash/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     8876 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/simple_hash/simple_hash.c
--rw-r--r--   0 rieder     (501) staff       (20)     1112 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/simple_hash/simple_hash.h
--rw-r--r--   0 rieder     (501) staff       (20)     1906 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/simple_hash/test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3620 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/simple_hash/test.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.355391 amuse-framework-2023.5.0/lib/stopcond/
--rw-r--r--   0 rieder     (501) staff       (20)      688 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/stopcond/Makefile
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.355524 amuse-framework-2023.5.0/lib/stopcond/mpi/
--rw-r--r--   0 rieder     (501) staff       (20)      243 2023-03-14 13:48:48.000000 amuse-framework-2023.5.0/lib/stopcond/mpi/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)    18126 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcond.c
--rw-r--r--   0 rieder     (501) staff       (20)     3591 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcond.h
--rw-r--r--   0 rieder     (501) staff       (20)     1642 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcond.inc
--rw-r--r--   0 rieder     (501) staff       (20)    21963 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcondf.F90
--rw-r--r--   0 rieder     (501) staff       (20)     9654 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/lib/stopcond/stopcondf_isoc.F90
--rw-r--r--   0 rieder     (501) staff       (20)      143 2023-05-17 09:30:35.000000 amuse-framework-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:18:42.386507 amuse-framework-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     2059 2023-05-17 09:47:47.000000 amuse-framework-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.348353 amuse-framework-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.356267 amuse-framework-2023.5.0/src/amuse/
--rw-r--r--   0 rieder     (501) staff       (20)     1903 2023-04-15 06:02:12.000000 amuse-framework-2023.5.0/src/amuse/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/src/amuse/amuserc
--rw-r--r--   0 rieder     (501) staff       (20)      915 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/src/amuse/codes.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.356414 amuse-framework-2023.5.0/src/amuse/community/
--rw-r--r--   0 rieder     (501) staff       (20)     1277 2022-11-22 11:55:14.000000 amuse-framework-2023.5.0/src/amuse/community/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.357572 amuse-framework-2023.5.0/src/amuse/community/interface/
--rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     3894 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/common.py
--rw-r--r--   0 rieder     (501) staff       (20)     3439 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/example.py
--rw-r--r--   0 rieder     (501) staff       (20)    52603 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/gd.py
--rw-r--r--   0 rieder     (501) staff       (20)    12910 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/hydro.py
--rw-r--r--   0 rieder     (501) staff       (20)     1756 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/mhd.py
--rw-r--r--   0 rieder     (501) staff       (20)    54169 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/se.py
--rw-r--r--   0 rieder     (501) staff       (20)    28066 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/community/interface/stopping_conditions.py
--rw-r--r--   0 rieder     (501) staff       (20)     2968 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/config.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.358679 amuse-framework-2023.5.0/src/amuse/couple/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    24220 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/couple/bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)     5584 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/collision_handler.py
--rw-r--r--   0 rieder     (501) staff       (20)    95615 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/encounters.py
--rw-r--r--   0 rieder     (501) staff       (20)    11720 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/fallback_stellar_evolution.py
--rw-r--r--   0 rieder     (501) staff       (20)   122275 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/multiples.py
--rw-r--r--   0 rieder     (501) staff       (20)     6255 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/couple/parallel_stellar_evolution.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.358985 amuse-framework-2023.5.0/src/amuse/data/
--rw-r--r--   0 rieder     (501) staff       (20)    60725 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/data/AMUSE.bib
--rw-r--r--   0 rieder     (501) staff       (20)       27 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/data/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.361921 amuse-framework-2023.5.0/src/amuse/datamodel/
--rw-r--r--   0 rieder     (501) staff       (20)      388 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     3473 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)    64925 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/base.py
--rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/binding.py
--rw-r--r--   0 rieder     (501) staff       (20)       42 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/code_particles.py
--rw-r--r--   0 rieder     (501) staff       (20)      150 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/console.py
--rw-r--r--   0 rieder     (501) staff       (20)     7549 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/grid_attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)    42650 2023-04-17 12:49:34.000000 amuse-framework-2023.5.0/src/amuse/datamodel/grids.py
--rw-r--r--   0 rieder     (501) staff       (20)    50773 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/incode_storage.py
--rw-r--r--   0 rieder     (501) staff       (20)    13000 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/indexing.py
--rw-r--r--   0 rieder     (501) staff       (20)    26559 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/memory_storage.py
--rw-r--r--   0 rieder     (501) staff       (20)    26325 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/datamodel/parameters.py
--rw-r--r--   0 rieder     (501) staff       (20)    47337 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/datamodel/particle_attributes.py
--rw-r--r--   0 rieder     (501) staff       (20)   155220 2023-05-11 09:04:53.000000 amuse-framework-2023.5.0/src/amuse/datamodel/particles.py
--rw-r--r--   0 rieder     (501) staff       (20)     1551 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/rotation.py
--rw-r--r--   0 rieder     (501) staff       (20)       74 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/set.py
--rw-r--r--   0 rieder     (501) staff       (20)     3904 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/simple_hash.py
--rw-r--r--   0 rieder     (501) staff       (20)    10234 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/staggeredgrid.py
--rw-r--r--   0 rieder     (501) staff       (20)    14471 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/trees.py
--rw-r--r--   0 rieder     (501) staff       (20)      188 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/datamodel/values.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.369478 amuse-framework-2023.5.0/src/amuse/ext/
--rw-r--r--   0 rieder     (501) staff       (20)     1290 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/ClusterCore.py
--rw-r--r--   0 rieder     (501) staff       (20)     2524 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/LagrangianRadii.py
--rw-r--r--   0 rieder     (501) staff       (20)     1689 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/SConstruct
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     6021 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/basicgraph.py
--rw-r--r--   0 rieder     (501) staff       (20)    69458 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/bbr_color.txt
--rw-r--r--   0 rieder     (501) staff       (20)     4018 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/bhtc_interface.pyx
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.369740 amuse-framework-2023.5.0/src/amuse/ext/blender/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/blender/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      771 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/blender/blender.py
--rw-r--r--   0 rieder     (501) staff       (20)     3386 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/boss_bodenheimer.py
--rw-r--r--   0 rieder     (501) staff       (20)    11167 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)     5473 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)     7430 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/composition_methods.py
--rw-r--r--   0 rieder     (501) staff       (20)     1932 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/comsystem.py
--rw-r--r--   0 rieder     (501) staff       (20)     6851 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/concurrent.py
--rw-r--r--   0 rieder     (501) staff       (20)     5397 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/cosmo.py
--rw-r--r--   0 rieder     (501) staff       (20)     2340 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/derived_grav_systems.py
--rw-r--r--   0 rieder     (501) staff       (20)     9939 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/evrard_test.py
--rw-r--r--   0 rieder     (501) staff       (20)     9832 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/galactic_potentials.py
--rw-r--r--   0 rieder     (501) staff       (20)     3541 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/galactics_model.py
--rw-r--r--   0 rieder     (501) staff       (20)     2446 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/gasplummer.py
--rw-r--r--   0 rieder     (501) staff       (20)    12018 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/ext/grid_remappers.py
--rw-r--r--   0 rieder     (501) staff       (20)     5851 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/grid_to_sph.py
--rw-r--r--   0 rieder     (501) staff       (20)     2247 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/halogen_model.py
--rw-r--r--   0 rieder     (501) staff       (20)    22588 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/hydro_collision.py
--rw-r--r--   0 rieder     (501) staff       (20)    12419 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/job_server.py
--rw-r--r--   0 rieder     (501) staff       (20)       33 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/kingmodel.py
--rw-r--r--   0 rieder     (501) staff       (20)    10428 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/molecular_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)    23761 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/orbital_elements.py
--rw-r--r--   0 rieder     (501) staff       (20)     6567 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/particles_with_color.py
--rw-r--r--   0 rieder     (501) staff       (20)     2982 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/plotting_hydro.py
--rw-r--r--   0 rieder     (501) staff       (20)      134 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/plummer.py
--rw-r--r--   0 rieder     (501) staff       (20)     1271 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/plummer_helper.pyx
--rw-r--r--   0 rieder     (501) staff       (20)     1917 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/polarsupport.py
--rw-r--r--   0 rieder     (501) staff       (20)     5030 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/protodisk.py
--rw-r--r--   0 rieder     (501) staff       (20)     1981 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/radial_profile.py
--rw-r--r--   0 rieder     (501) staff       (20)     4067 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/relax_sph.py
--rw-r--r--   0 rieder     (501) staff       (20)    10547 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/roche_radius.py
--rw-r--r--   0 rieder     (501) staff       (20)     6928 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/rotating_bridge.py
--rw-r--r--   0 rieder     (501) staff       (20)      137 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/salpeter.py
--rw-r--r--   0 rieder     (501) staff       (20)    12155 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sink.py
--rw-r--r--   0 rieder     (501) staff       (20)    11837 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sobol.py
--rw-r--r--   0 rieder     (501) staff       (20)    12891 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/solarsystem.py
--rw-r--r--   0 rieder     (501) staff       (20)     2200 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/speed.py
--rw-r--r--   0 rieder     (501) staff       (20)     3482 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sph_to_grid.py
--rw-r--r--   0 rieder     (501) staff       (20)     3314 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sph_to_star.py
--rw-r--r--   0 rieder     (501) staff       (20)    20811 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/spherical_model.py
--rw-r--r--   0 rieder     (501) staff       (20)    19994 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/star_to_sph.py
--rw-r--r--   0 rieder     (501) staff       (20)     8764 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/static_potentials.py
--rw-r--r--   0 rieder     (501) staff       (20)     2688 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/stellar_gyration_radius.py
--rw-r--r--   0 rieder     (501) staff       (20)    18470 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/stellar_tidal_evolution.py
--rw-r--r--   0 rieder     (501) staff       (20)    41820 2023-04-04 13:43:32.000000 amuse-framework-2023.5.0/src/amuse/ext/stellar_wind.py
--rw-r--r--   0 rieder     (501) staff       (20)     1386 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ext/sticky_spheres.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.372191 amuse-framework-2023.5.0/src/amuse/ic/
--rw-r--r--   0 rieder     (501) staff       (20)     1229 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.372608 amuse-framework-2023.5.0/src/amuse/ic/_limepy/
--rwxr-xr-x   0 rieder     (501) staff       (20)      204 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/_limepy/__init__.py
--rwxr-xr-x   0 rieder     (501) staff       (20)    43751 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/_limepy/limepy.py
--rwxr-xr-x   0 rieder     (501) staff       (20)    10121 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/_limepy/sample.py
--rw-r--r--   0 rieder     (501) staff       (20)     9096 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/brokenimf.py
--rw-r--r--   0 rieder     (501) staff       (20)     2352 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/flatimf.py
--rw-r--r--   0 rieder     (501) staff       (20)      151 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/fractalcluster.py
--rw-r--r--   0 rieder     (501) staff       (20)     3678 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/gasplummer.py
--rw-r--r--   0 rieder     (501) staff       (20)     7649 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/isotropic_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)    20594 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/kingmodel.py
--rw-r--r--   0 rieder     (501) staff       (20)      267 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/kroupa.py
--rw-r--r--   0 rieder     (501) staff       (20)     1724 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/limepy.py
--rw-r--r--   0 rieder     (501) staff       (20)    13570 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/make_planets_oligarch.py
--rw-r--r--   0 rieder     (501) staff       (20)       56 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/mameclot.py
--rw-r--r--   0 rieder     (501) staff       (20)      295 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/millerscalo.py
--rw-r--r--   0 rieder     (501) staff       (20)      468 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/molecular_cloud.py
--rw-r--r--   0 rieder     (501) staff       (20)     6918 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/plummer.py
--rw-r--r--   0 rieder     (501) staff       (20)     2981 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/salpeter.py
--rw-r--r--   0 rieder     (501) staff       (20)      263 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/scalo.py
--rw-r--r--   0 rieder     (501) staff       (20)    21531 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/solar_system_moons.py
--rw-r--r--   0 rieder     (501) staff       (20)      165 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/ic/solarsystem.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.374654 amuse-framework-2023.5.0/src/amuse/io/
--rw-r--r--   0 rieder     (501) staff       (20)     1001 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    17890 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/base.py
--rw-r--r--   0 rieder     (501) staff       (20)     6347 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/fi_io.py
--rw-r--r--   0 rieder     (501) staff       (20)    16756 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/gadget.py
--rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/horizons.py
--rw-r--r--   0 rieder     (501) staff       (20)    12272 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/nemobin.py
--rw-r--r--   0 rieder     (501) staff       (20)     5389 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/nemotsf.py
--rw-r--r--   0 rieder     (501) staff       (20)     1027 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/p10.txt
--rw-r--r--   0 rieder     (501) staff       (20)     4241 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/phigrape.py
--rw-r--r--   0 rieder     (501) staff       (20)    17938 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/starlab.py
--rw-r--r--   0 rieder     (501) staff       (20)     6419 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/store.py
--rw-r--r--   0 rieder     (501) staff       (20)    32086 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/store_v1.py
--rw-r--r--   0 rieder     (501) staff       (20)    46982 2023-05-11 09:04:53.000000 amuse-framework-2023.5.0/src/amuse/io/store_v2.py
--rw-r--r--   0 rieder     (501) staff       (20)    22593 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/text.py
--rw-r--r--   0 rieder     (501) staff       (20)    14998 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/io/vtk.py
--rw-r--r--   0 rieder     (501) staff       (20)     4808 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/lab.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.375177 amuse-framework-2023.5.0/src/amuse/plot/
--rw-r--r--   0 rieder     (501) staff       (20)       21 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/plot/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    22278 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/plot/_plot.py
--rwxr-xr-x   0 rieder     (501) staff       (20)    13863 2023-04-04 13:20:13.000000 amuse-framework-2023.5.0/src/amuse/plot/hydro.py
--rw-r--r--   0 rieder     (501) staff       (20)    12634 2023-03-16 12:23:56.000000 amuse-framework-2023.5.0/src/amuse/plot/mapper.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.376543 amuse-framework-2023.5.0/src/amuse/rfi/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    23061 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/async_request.py
--rw-r--r--   0 rieder     (501) staff       (20)    88683 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/channel.py
--rw-r--r--   0 rieder     (501) staff       (20)    52496 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/core.py
--rwxr-xr-x   0 rieder     (501) staff       (20)    15246 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/gencode.py
--rw-r--r--   0 rieder     (501) staff       (20)     4329 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/import_module.py
--rw-r--r--   0 rieder     (501) staff       (20)     5500 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/nospawn.py
--rw-r--r--   0 rieder     (501) staff       (20)    23380 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/python_code.py
--rw-r--r--   0 rieder     (501) staff       (20)     1197 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/run_command_redirected.py
--rw-r--r--   0 rieder     (501) staff       (20)     2138 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/slurm.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.378203 amuse-framework-2023.5.0/src/amuse/rfi/tools/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    45482 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_c.py
--rw-r--r--   0 rieder     (501) staff       (20)     4264 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_code.py
--rw-r--r--   0 rieder     (501) staff       (20)    10659 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_definition.py
--rw-r--r--   0 rieder     (501) staff       (20)    15062 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_dir.py
--rw-r--r--   0 rieder     (501) staff       (20)    64699 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_fortran.py
--rw-r--r--   0 rieder     (501) staff       (20)    53344 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_java.py
--rw-r--r--   0 rieder     (501) staff       (20)     2216 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/create_python_worker.py
--rw-r--r--   0 rieder     (501) staff       (20)      991 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/cython_code_script.template
--rw-r--r--   0 rieder     (501) staff       (20)    11322 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/fortran_tools.py
--rw-r--r--   0 rieder     (501) staff       (20)      980 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/java_code_script.template
--rw-r--r--   0 rieder     (501) staff       (20)     1102 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/rfi/tools/python_code_script.template
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.380099 amuse-framework-2023.5.0/src/amuse/support/
--rw-r--r--   0 rieder     (501) staff       (20)      569 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     5372 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/code.py
--rw-r--r--   0 rieder     (501) staff       (20)    11337 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/support/console.py
--rw-r--r--   0 rieder     (501) staff       (20)    15197 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/core.py
--rw-r--r--   0 rieder     (501) staff       (20)     2073 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/exceptions.py
--rw-r--r--   0 rieder     (501) staff       (20)    61635 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)    11438 2023-04-15 06:02:12.000000 amuse-framework-2023.5.0/src/amuse/support/literature.py
--rw-r--r--   0 rieder     (501) staff       (20)     8981 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/methods.py
--rw-r--r--   0 rieder     (501) staff       (20)    10236 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/support/options.py
--rw-r--r--   0 rieder     (501) staff       (20)    11751 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/parameter_tools.py
--rw-r--r--   0 rieder     (501) staff       (20)     1183 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/project.py
--rw-r--r--   0 rieder     (501) staff       (20)    19392 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/state.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.380698 amuse-framework-2023.5.0/src/amuse/support/thirdparty/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/thirdparty/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    18956 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/support/thirdparty/texttable.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.381382 amuse-framework-2023.5.0/src/amuse/test/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/test/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    12935 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/test/amusetest.py
--rw-r--r--   0 rieder     (501) staff       (20)    14500 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/test/compile_tools.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.384403 amuse-framework-2023.5.0/src/amuse/units/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    18324 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/constants.py
--rw-r--r--   0 rieder     (501) staff       (20)    33642 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/core.py
--rw-r--r--   0 rieder     (501) staff       (20)      731 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/derivedsi.py
--rw-r--r--   0 rieder     (501) staff       (20)    11358 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/generic_unit_converter.py
--rw-r--r--   0 rieder     (501) staff       (20)     2792 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/generic_unit_system.py
--rw-r--r--   0 rieder     (501) staff       (20)     4912 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/nbody_system.py
--rw-r--r--   0 rieder     (501) staff       (20)     7342 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/nist.py
--rw-r--r--   0 rieder     (501) staff       (20)    33920 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/nist.txt
--rw-r--r--   0 rieder     (501) staff       (20)    38873 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/nist2010.txt
--rw-r--r--   0 rieder     (501) staff       (20)     4718 2023-03-14 12:52:28.000000 amuse-framework-2023.5.0/src/amuse/units/optparse.py
--rw-r--r--   0 rieder     (501) staff       (20)    44745 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/quantities.py
--rw-r--r--   0 rieder     (501) staff       (20)     1853 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/scaling_converter.py
--rw-r--r--   0 rieder     (501) staff       (20)     2349 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/si.py
--rw-r--r--   0 rieder     (501) staff       (20)      190 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/translator.txt
--rw-r--r--   0 rieder     (501) staff       (20)      780 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/src/amuse/units/trigo.py
--rw-r--r--   0 rieder     (501) staff       (20)     4019 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/src/amuse/units/units.py
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.384974 amuse-framework-2023.5.0/src/amuse_framework.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1242 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     7390 2023-05-17 10:18:42.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)      130 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:18:40.000000 amuse-framework-2023.5.0/src/amuse_framework.egg-info/top_level.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:42.386097 amuse-framework-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-framework-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-framework-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-framework-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.809540 amuse_framework-2024.4.0rc1/
+-rw-r--r--   0 rieder     (501) staff       (20)      639 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     2471 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1519 2024-04-24 16:07:48.809269 amuse_framework-2024.4.0rc1/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      101 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.763983 amuse_framework-2024.4.0rc1/bin/
+-rwxr-xr-x   0 rieder     (501) staff       (20)      328 2022-11-22 11:55:13.000000 amuse_framework-2024.4.0rc1/bin/amuse-tutorial
+-rwxr-xr-x   0 rieder     (501) staff       (20)      775 2024-04-24 16:05:50.000000 amuse_framework-2024.4.0rc1/bin/amusifier
+-rw-r--r--   0 rieder     (501) staff       (20)      728 2022-11-22 11:55:13.000000 amuse_framework-2024.4.0rc1/bin/amusifier.in
+-rw-r--r--   0 rieder     (501) staff       (20)    49446 2023-02-28 13:39:09.000000 amuse_framework-2024.4.0rc1/config.guess
+-rw-r--r--   0 rieder     (501) staff       (20)     3552 2024-04-24 16:05:50.000000 amuse_framework-2024.4.0rc1/config.mk
+-rw-r--r--   0 rieder     (501) staff       (20)     2814 2022-11-22 11:55:13.000000 amuse_framework-2024.4.0rc1/config.mk.in
+-rw-r--r--   0 rieder     (501) staff       (20)    34424 2023-02-28 13:39:09.000000 amuse_framework-2024.4.0rc1/config.sub
+-rwxr-xr-x   0 rieder     (501) staff       (20)   412686 2023-07-06 10:13:12.000000 amuse_framework-2024.4.0rc1/configure
+-rwxr-xr-x   0 rieder     (501) staff       (20)    15358 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/install-sh
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.759745 amuse_framework-2024.4.0rc1/lib/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.764547 amuse_framework-2024.4.0rc1/lib/amuse_mpi/
+-rw-r--r--   0 rieder     (501) staff       (20)      499 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/lib/amuse_mpi/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      335 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/amuse_mpi/amuse_mpi.c
+-rw-r--r--   0 rieder     (501) staff       (20)      212 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/amuse_mpi/amuse_mpi.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.765141 amuse_framework-2024.4.0rc1/lib/forsockets/
+-rw-r--r--   0 rieder     (501) staff       (20)      494 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/lib/forsockets/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     5068 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/forsockets/forsockets.c
+-rw-r--r--   0 rieder     (501) staff       (20)      853 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/forsockets/forsockets.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4782 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/forsockets/forsocketsf.f90
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.765849 amuse_framework-2024.4.0rc1/lib/g6/
+-rw-r--r--   0 rieder     (501) staff       (20)      242 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/lib/g6/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)    12542 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/g6/g6lib.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3957 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/g6/g6lib.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.766110 amuse_framework-2024.4.0rc1/lib/sapporo_2/
+-rw-r--r--   0 rieder     (501) staff       (20)     1469 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/lib/sapporo_2/Makefile
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2548 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_2/download.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.768129 amuse_framework-2024.4.0rc1/lib/sapporo_light/
+-rw-r--r--   0 rieder     (501) staff       (20)     1339 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      641 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/README
+-rw-r--r--   0 rieder     (501) staff       (20)    11568 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/dev_evaluate_gravity.cu
+-rw-r--r--   0 rieder     (501) staff       (20)    12542 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/g6lib.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1461 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/g6lib.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5486 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/host_evaluate_gravity.cu
+-rw-r--r--   0 rieder     (501) staff       (20)     7585 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporo.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4632 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporo.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2434 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporoG6lib.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2964 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporo_defs.h
+-rw-r--r--   0 rieder     (501) staff       (20)      530 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporo_multi.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5983 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/sapporo_light/send_fetch_data.cpp
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.768955 amuse_framework-2024.4.0rc1/lib/simple_hash/
+-rw-r--r--   0 rieder     (501) staff       (20)      619 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/lib/simple_hash/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     8876 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/simple_hash/simple_hash.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1112 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/simple_hash/simple_hash.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1906 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/simple_hash/test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3620 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/simple_hash/test.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.770008 amuse_framework-2024.4.0rc1/lib/stopcond/
+-rw-r--r--   0 rieder     (501) staff       (20)      688 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/lib/stopcond/Makefile
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.770259 amuse_framework-2024.4.0rc1/lib/stopcond/mpi/
+-rw-r--r--   0 rieder     (501) staff       (20)      243 2023-03-14 13:48:48.000000 amuse_framework-2024.4.0rc1/lib/stopcond/mpi/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)    18126 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/stopcond/stopcond.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3591 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/stopcond/stopcond.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1642 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/stopcond/stopcond.inc
+-rw-r--r--   0 rieder     (501) staff       (20)    21963 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/stopcond/stopcondf.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     9654 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/lib/stopcond/stopcondf_isoc.F90
+-rw-r--r--   0 rieder     (501) staff       (20)      143 2023-07-06 17:43:32.000000 amuse_framework-2024.4.0rc1/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:07:48.809619 amuse_framework-2024.4.0rc1/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1880 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.761352 amuse_framework-2024.4.0rc1/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.771076 amuse_framework-2024.4.0rc1/src/amuse/
+-rw-r--r--   0 rieder     (501) staff       (20)     1902 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      420 2024-04-24 16:07:47.000000 amuse_framework-2024.4.0rc1/src/amuse/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/src/amuse/amuserc
+-rw-r--r--   0 rieder     (501) staff       (20)      915 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/src/amuse/codes.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.771225 amuse_framework-2024.4.0rc1/src/amuse/community/
+-rw-r--r--   0 rieder     (501) staff       (20)     1277 2022-11-22 11:55:14.000000 amuse_framework-2024.4.0rc1/src/amuse/community/__init__.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.772710 amuse_framework-2024.4.0rc1/src/amuse/community/interface/
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/community/interface/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3894 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/community/interface/common.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3439 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/community/interface/example.py
+-rw-r--r--   0 rieder     (501) staff       (20)    51008 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/community/interface/gd.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12910 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/community/interface/hydro.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1756 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/community/interface/mhd.py
+-rw-r--r--   0 rieder     (501) staff       (20)    54169 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/community/interface/se.py
+-rw-r--r--   0 rieder     (501) staff       (20)    28066 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/community/interface/stopping_conditions.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3036 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/config.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.774002 amuse_framework-2024.4.0rc1/src/amuse/couple/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/couple/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    25102 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/couple/bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5584 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/couple/collision_handler.py
+-rw-r--r--   0 rieder     (501) staff       (20)    95615 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/couple/encounters.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11720 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/couple/fallback_stellar_evolution.py
+-rw-r--r--   0 rieder     (501) staff       (20)   122275 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/couple/multiples.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6255 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/couple/parallel_stellar_evolution.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.774375 amuse_framework-2024.4.0rc1/src/amuse/data/
+-rw-r--r--   0 rieder     (501) staff       (20)    60725 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/data/AMUSE.bib
+-rw-r--r--   0 rieder     (501) staff       (20)       27 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/data/__init__.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.778060 amuse_framework-2024.4.0rc1/src/amuse/datamodel/
+-rw-r--r--   0 rieder     (501) staff       (20)      388 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3473 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)    64925 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/base.py
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/binding.py
+-rw-r--r--   0 rieder     (501) staff       (20)       42 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/code_particles.py
+-rw-r--r--   0 rieder     (501) staff       (20)      150 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/console.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7549 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/grid_attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)    42731 2023-07-06 13:01:40.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/grids.py
+-rw-r--r--   0 rieder     (501) staff       (20)    50770 2023-07-06 16:13:36.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/incode_storage.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13000 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/indexing.py
+-rw-r--r--   0 rieder     (501) staff       (20)    26559 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/memory_storage.py
+-rw-r--r--   0 rieder     (501) staff       (20)    26325 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/parameters.py
+-rw-r--r--   0 rieder     (501) staff       (20)    47337 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/particle_attributes.py
+-rw-r--r--   0 rieder     (501) staff       (20)   155220 2023-05-11 09:04:53.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/particles.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1701 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/rotation.py
+-rw-r--r--   0 rieder     (501) staff       (20)       74 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/set.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3904 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/simple_hash.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10234 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/staggeredgrid.py
+-rw-r--r--   0 rieder     (501) staff       (20)    14471 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/trees.py
+-rw-r--r--   0 rieder     (501) staff       (20)      188 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/datamodel/values.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.787052 amuse_framework-2024.4.0rc1/src/amuse/ext/
+-rw-r--r--   0 rieder     (501) staff       (20)     1290 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/ClusterCore.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2524 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/LagrangianRadii.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1689 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/SConstruct
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6021 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/basicgraph.py
+-rw-r--r--   0 rieder     (501) staff       (20)    69458 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/bbr_color.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     4018 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/bhtc_interface.pyx
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.787293 amuse_framework-2024.4.0rc1/src/amuse/ext/blender/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/blender/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      771 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/blender/blender.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3386 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/boss_bodenheimer.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11167 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5473 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7430 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/composition_methods.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1932 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/comsystem.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6851 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/concurrent.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5397 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/cosmo.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2340 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/derived_grav_systems.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9939 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/evrard_test.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9832 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/galactic_potentials.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3541 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/galactics_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2446 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/gasplummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13455 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/grid_remappers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5851 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/grid_to_sph.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2247 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/halogen_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22588 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/hydro_collision.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12419 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/job_server.py
+-rw-r--r--   0 rieder     (501) staff       (20)       33 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/kingmodel.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10428 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/molecular_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)    25427 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/orbital_elements.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6567 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/particles_with_color.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2982 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/plotting_hydro.py
+-rw-r--r--   0 rieder     (501) staff       (20)      134 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/plummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1271 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/plummer_helper.pyx
+-rw-r--r--   0 rieder     (501) staff       (20)     1917 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/polarsupport.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5030 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/protodisk.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1981 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/radial_profile.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4067 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/relax_sph.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10547 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/roche_radius.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6928 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/rotating_bridge.py
+-rw-r--r--   0 rieder     (501) staff       (20)      137 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/salpeter.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12155 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/sink.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11837 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/sobol.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12891 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/solarsystem.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2200 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/speed.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3482 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/sph_to_grid.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3314 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/sph_to_star.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21739 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/spherical_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19994 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/star_to_sph.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8764 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/static_potentials.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2688 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/stellar_gyration_radius.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18470 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/stellar_tidal_evolution.py
+-rw-r--r--   0 rieder     (501) staff       (20)    41820 2023-04-04 13:43:32.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/stellar_wind.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1386 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ext/sticky_spheres.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.790732 amuse_framework-2024.4.0rc1/src/amuse/ic/
+-rw-r--r--   0 rieder     (501) staff       (20)     1229 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/__init__.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.791191 amuse_framework-2024.4.0rc1/src/amuse/ic/_limepy/
+-rwxr-xr-x   0 rieder     (501) staff       (20)      204 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/_limepy/__init__.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)    43751 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/_limepy/limepy.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)    10121 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/_limepy/sample.py
+-rw-r--r--   0 rieder     (501) staff       (20)     9136 2023-07-06 17:15:18.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/brokenimf.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2352 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/flatimf.py
+-rw-r--r--   0 rieder     (501) staff       (20)      151 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/fractalcluster.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3871 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/gasplummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7680 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/isotropic_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21379 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/kingmodel.py
+-rw-r--r--   0 rieder     (501) staff       (20)      267 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/kroupa.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1724 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/limepy.py
+-rw-r--r--   0 rieder     (501) staff       (20)    13570 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/make_planets_oligarch.py
+-rw-r--r--   0 rieder     (501) staff       (20)       56 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/mameclot.py
+-rw-r--r--   0 rieder     (501) staff       (20)      295 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/millerscalo.py
+-rw-r--r--   0 rieder     (501) staff       (20)      468 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/molecular_cloud.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7521 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/plummer.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2981 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/salpeter.py
+-rw-r--r--   0 rieder     (501) staff       (20)      263 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/scalo.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21531 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/solar_system_moons.py
+-rw-r--r--   0 rieder     (501) staff       (20)      165 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/ic/solarsystem.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.794040 amuse_framework-2024.4.0rc1/src/amuse/io/
+-rw-r--r--   0 rieder     (501) staff       (20)     1001 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    17890 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/base.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6347 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/fi_io.py
+-rw-r--r--   0 rieder     (501) staff       (20)    16756 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/gadget.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/horizons.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12272 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/nemobin.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5389 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/nemotsf.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1027 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/p10.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     4241 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/phigrape.py
+-rw-r--r--   0 rieder     (501) staff       (20)    17938 2023-07-06 16:13:36.000000 amuse_framework-2024.4.0rc1/src/amuse/io/starlab.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6419 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/store.py
+-rw-r--r--   0 rieder     (501) staff       (20)    32086 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/store_v1.py
+-rw-r--r--   0 rieder     (501) staff       (20)    47030 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/io/store_v2.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22593 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/text.py
+-rw-r--r--   0 rieder     (501) staff       (20)    14998 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/io/vtk.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4808 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/lab.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.795204 amuse_framework-2024.4.0rc1/src/amuse/plot/
+-rw-r--r--   0 rieder     (501) staff       (20)       21 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/plot/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    22278 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/plot/_plot.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)    13863 2023-04-04 13:20:13.000000 amuse_framework-2024.4.0rc1/src/amuse/plot/hydro.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12634 2023-03-16 12:23:56.000000 amuse_framework-2024.4.0rc1/src/amuse/plot/mapper.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.797318 amuse_framework-2024.4.0rc1/src/amuse/rfi/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    23061 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/async_request.py
+-rw-r--r--   0 rieder     (501) staff       (20)    94834 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/channel.py
+-rw-r--r--   0 rieder     (501) staff       (20)    52766 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/core.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)    15771 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/gencode.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4329 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/import_module.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5500 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/nospawn.py
+-rw-r--r--   0 rieder     (501) staff       (20)    23380 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/python_code.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1197 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/run_command_redirected.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2138 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/slurm.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.799842 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    45482 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_c.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4264 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_code.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10659 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_definition.py
+-rw-r--r--   0 rieder     (501) staff       (20)    15062 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_dir.py
+-rw-r--r--   0 rieder     (501) staff       (20)    64699 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_fortran.py
+-rw-r--r--   0 rieder     (501) staff       (20)    53344 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_java.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2216 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_python_worker.py
+-rw-r--r--   0 rieder     (501) staff       (20)      991 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/cython_code_script.template
+-rw-r--r--   0 rieder     (501) staff       (20)    11322 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/fortran_tools.py
+-rw-r--r--   0 rieder     (501) staff       (20)      980 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/java_code_script.template
+-rw-r--r--   0 rieder     (501) staff       (20)     1102 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/python_code_script.template
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.802529 amuse_framework-2024.4.0rc1/src/amuse/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      882 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)     5372 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/code.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11337 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/support/console.py
+-rw-r--r--   0 rieder     (501) staff       (20)    15197 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/core.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2073 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/exceptions.py
+-rw-r--r--   0 rieder     (501) staff       (20)    62980 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/support/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11497 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/support/literature.py
+-rw-r--r--   0 rieder     (501) staff       (20)     8981 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/methods.py
+-rw-r--r--   0 rieder     (501) staff       (20)    10236 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/support/options.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11751 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/parameter_tools.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1183 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/project.py
+-rw-r--r--   0 rieder     (501) staff       (20)    19392 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/state.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.802827 amuse_framework-2024.4.0rc1/src/amuse/support/thirdparty/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/thirdparty/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18956 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/support/thirdparty/texttable.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.803512 amuse_framework-2024.4.0rc1/src/amuse/test/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/test/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    12939 2023-07-06 17:15:18.000000 amuse_framework-2024.4.0rc1/src/amuse/test/amusetest.py
+-rw-r--r--   0 rieder     (501) staff       (20)    14500 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/test/compile_tools.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.806522 amuse_framework-2024.4.0rc1/src/amuse/units/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/units/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)    18600 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/constants.py
+-rw-r--r--   0 rieder     (501) staff       (20)    33642 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/units/core.py
+-rw-r--r--   0 rieder     (501) staff       (20)      777 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/derivedsi.py
+-rw-r--r--   0 rieder     (501) staff       (20)    11583 2023-07-06 15:25:54.000000 amuse_framework-2024.4.0rc1/src/amuse/units/generic_unit_converter.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2792 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/src/amuse/units/generic_unit_system.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4852 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/nbody_system.py
+-rw-r--r--   0 rieder     (501) staff       (20)     7342 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/units/nist.py
+-rw-r--r--   0 rieder     (501) staff       (20)    33920 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/units/nist.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    38873 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/units/nist2010.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     4824 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/optparse.py
+-rw-r--r--   0 rieder     (501) staff       (20)    45772 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/quantities.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1764 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/scaling_converter.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2405 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/si.py
+-rw-r--r--   0 rieder     (501) staff       (20)      916 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/stellar_types.py
+-rw-r--r--   0 rieder     (501) staff       (20)      190 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/src/amuse/units/translator.txt
+-rw-r--r--   0 rieder     (501) staff       (20)      837 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/trigo.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3419 2024-04-24 15:35:29.000000 amuse_framework-2024.4.0rc1/src/amuse/units/units.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.808684 amuse_framework-2024.4.0rc1/src/amuse_framework.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1519 2024-04-24 16:07:47.000000 amuse_framework-2024.4.0rc1/src/amuse_framework.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     7450 2024-04-24 16:07:48.000000 amuse_framework-2024.4.0rc1/src/amuse_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:07:47.000000 amuse_framework-2024.4.0rc1/src/amuse_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)      130 2024-04-24 16:07:47.000000 amuse_framework-2024.4.0rc1/src/amuse_framework.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:07:47.000000 amuse_framework-2024.4.0rc1/src/amuse_framework.egg-info/top_level.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:07:48.808500 amuse_framework-2024.4.0rc1/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse_framework-2024.4.0rc1/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse_framework-2024.4.0rc1/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse_framework-2024.4.0rc1/support/version.py
```

### Comparing `amuse-framework-2023.5.0/MANIFEST.in` & `amuse_framework-2024.4.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/Makefile.in` & `amuse_framework-2024.4.0rc1/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/bin/amusifier.in` & `amuse_framework-2024.4.0rc1/bin/amusifier.in`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/config.guess` & `amuse_framework-2024.4.0rc1/config.guess`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/config.mk.in` & `amuse_framework-2024.4.0rc1/config.mk.in`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/config.sub` & `amuse_framework-2024.4.0rc1/config.sub`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/configure` & `amuse_framework-2024.4.0rc1/configure`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for amuse 2023.3.1.dev41+gaa14f8bf8.d20230322.
+# Generated by GNU Autoconf 2.71 for amuse 2023.7.0.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
 #
 # This configure script is free software; the Free Software Foundation
@@ -664,16 +664,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='amuse'
 PACKAGE_TARNAME='amuse'
-PACKAGE_VERSION='2023.3.1.dev41+gaa14f8bf8.d20230322'
-PACKAGE_STRING='amuse 2023.3.1.dev41+gaa14f8bf8.d20230322'
+PACKAGE_VERSION='2023.7.0'
+PACKAGE_STRING='amuse 2023.7.0'
 PACKAGE_BUGREPORT=''
 PACKAGE_URL=''
 
 ac_unique_file="src/amuse/__init__.py"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1501,15 +1501,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures amuse 2023.3.1.dev41+gaa14f8bf8.d20230322 to adapt to many kinds of systems.
+\`configure' configures amuse 2023.7.0 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1567,15 +1567,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of amuse 2023.3.1.dev41+gaa14f8bf8.d20230322:";;
+     short | recursive ) echo "Configuration of amuse 2023.7.0:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1721,15 +1721,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-amuse configure 2023.3.1.dev41+gaa14f8bf8.d20230322
+amuse configure 2023.7.0
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2255,15 +2255,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by amuse $as_me 2023.3.1.dev41+gaa14f8bf8.d20230322, which was
+It was created by amuse $as_me 2023.7.0, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4938,21 +4938,21 @@
 
 
 
 
 
         if test -n "$PYTHON"; then
       # If the user set $PYTHON, use it and don't search something else.
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking whether $PYTHON version is >= 3.5" >&5
-printf %s "checking whether $PYTHON version is >= 3.5... " >&6; }
+      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking whether $PYTHON version is >= 3.7" >&5
+printf %s "checking whether $PYTHON version is >= 3.7... " >&6; }
       prog="import sys
 # split strings by '.' and convert to numeric.  Append some zeros
 # because we need at least 4 digits for the hex conversion.
 # map returns an iterator in Python 3.0 and a list in 2.x
-minver = list(map(int, '3.5'.split('.'))) + [0, 0, 0]
+minver = list(map(int, '3.7'.split('.'))) + [0, 0, 0]
 minverhex = 0
 # xrange is not present in Python 3.0 and range returns an iterator
 for i in list(range(0, 4)): minverhex = (minverhex << 8) + minver[i]
 sys.exit(sys.hexversion < minverhex)"
   if { echo "$as_me:$LINENO: $PYTHON -c "$prog"" >&5
    ($PYTHON -c "$prog") >&5 2>&5
    ac_status=$?
@@ -4966,28 +4966,28 @@
 printf "%s\n" "no" >&6; }
 			       as_fn_error $? "Python interpreter is too old" "$LINENO" 5
 fi
       am_display_PYTHON=$PYTHON
     else
       # Otherwise, try each interpreter until we find one that satisfies
       # VERSION.
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for a Python interpreter with version >= 3.5" >&5
-printf %s "checking for a Python interpreter with version >= 3.5... " >&6; }
+      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for a Python interpreter with version >= 3.7" >&5
+printf %s "checking for a Python interpreter with version >= 3.7... " >&6; }
 if test ${am_cv_pathless_PYTHON+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
 
 	for am_cv_pathless_PYTHON in python python2 python3  python3.9 python3.8 python3.7 python3.6 python3.5 python3.4 python3.3  python3.2 python3.1 python3.0  python2.7 python2.6 python2.5 python2.4 python2.3 python2.2 python2.1  python2.0 none; do
 	  test "$am_cv_pathless_PYTHON" = none && break
 	  prog="import sys
 # split strings by '.' and convert to numeric.  Append some zeros
 # because we need at least 4 digits for the hex conversion.
 # map returns an iterator in Python 3.0 and a list in 2.x
-minver = list(map(int, '3.5'.split('.'))) + [0, 0, 0]
+minver = list(map(int, '3.7'.split('.'))) + [0, 0, 0]
 minverhex = 0
 # xrange is not present in Python 3.0 and range returns an iterator
 for i in list(range(0, 4)): minverhex = (minverhex << 8) + minver[i]
 sys.exit(sys.hexversion < minverhex)"
   if { echo "$as_me:$LINENO: $am_cv_pathless_PYTHON -c "$prog"" >&5
    ($am_cv_pathless_PYTHON -c "$prog") >&5 2>&5
    ac_status=$?
@@ -7772,15 +7772,21 @@
         if test "X$dir" = "X"; then
             LIBS="$LIBS -lcudart "
         else
             LIBS="$LIBS -L$dir -lcudart "
         fi
         cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
+ifelse(main, main, , # Avoid conflicting decl of main.
+    /* Override any gcc2 internal prototype to avoid an error.  */
 
+    /* We use char because int might match the return type of a gcc2
+        builtin and then its argument prototype would still apply.  */
+    char main();
+    )
 int
 main (void)
 {
 main()
   ;
   return 0;
 }
@@ -7856,15 +7862,21 @@
         if test "X$dir" = "X"; then
             LIBS="$LIBS -lcuda "
         else
             LIBS="$LIBS -L$dir -lcuda "
         fi
         cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
+ifelse(main, main, , # Avoid conflicting decl of main.
+    /* Override any gcc2 internal prototype to avoid an error.  */
 
+    /* We use char because int might match the return type of a gcc2
+        builtin and then its argument prototype would still apply.  */
+    char main();
+    )
 int
 main (void)
 {
 main()
   ;
   return 0;
 }
@@ -14318,15 +14330,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by amuse $as_me 2023.3.1.dev41+gaa14f8bf8.d20230322, which was
+This file was extended by amuse $as_me 2023.7.0, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -14373,15 +14385,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-amuse config.status 2023.3.1.dev41+gaa14f8bf8.d20230322
+amuse config.status 2023.7.0
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `amuse-framework-2023.5.0/install-sh` & `amuse_framework-2024.4.0rc1/install-sh`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/forsockets/forsockets.c` & `amuse_framework-2024.4.0rc1/lib/forsockets/forsockets.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/forsockets/forsockets.h` & `amuse_framework-2024.4.0rc1/lib/forsockets/forsockets.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/forsockets/forsocketsf.f90` & `amuse_framework-2024.4.0rc1/lib/forsockets/forsocketsf.f90`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/g6/g6lib.c` & `amuse_framework-2024.4.0rc1/lib/g6/g6lib.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/g6/g6lib.h` & `amuse_framework-2024.4.0rc1/lib/g6/g6lib.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_2/Makefile` & `amuse_framework-2024.4.0rc1/lib/sapporo_2/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_2/download.py` & `amuse_framework-2024.4.0rc1/lib/sapporo_2/download.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/Makefile` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/README` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/README`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/dev_evaluate_gravity.cu` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/dev_evaluate_gravity.cu`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/g6lib.c` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/g6lib.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/g6lib.h` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/g6lib.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/host_evaluate_gravity.cu` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/host_evaluate_gravity.cu`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/sapporo.cpp` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporo.cpp`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/sapporo.h` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporo.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/sapporoG6lib.cpp` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporoG6lib.cpp`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/sapporo_defs.h` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporo_defs.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/sapporo_multi.h` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/sapporo_multi.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/sapporo_light/send_fetch_data.cpp` & `amuse_framework-2024.4.0rc1/lib/sapporo_light/send_fetch_data.cpp`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/simple_hash/Makefile` & `amuse_framework-2024.4.0rc1/lib/simple_hash/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/simple_hash/simple_hash.c` & `amuse_framework-2024.4.0rc1/lib/simple_hash/simple_hash.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/simple_hash/simple_hash.h` & `amuse_framework-2024.4.0rc1/lib/simple_hash/simple_hash.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/simple_hash/test.cpp` & `amuse_framework-2024.4.0rc1/lib/simple_hash/test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/simple_hash/test.py` & `amuse_framework-2024.4.0rc1/lib/simple_hash/test.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/stopcond/Makefile` & `amuse_framework-2024.4.0rc1/lib/stopcond/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/stopcond/stopcond.c` & `amuse_framework-2024.4.0rc1/lib/stopcond/stopcond.c`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/stopcond/stopcond.h` & `amuse_framework-2024.4.0rc1/lib/stopcond/stopcond.h`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/stopcond/stopcond.inc` & `amuse_framework-2024.4.0rc1/lib/stopcond/stopcond.inc`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/stopcond/stopcondf.F90` & `amuse_framework-2024.4.0rc1/lib/stopcond/stopcondf.F90`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/lib/stopcond/stopcondf_isoc.F90` & `amuse_framework-2024.4.0rc1/lib/stopcond/stopcondf_isoc.F90`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/setup.py` & `amuse_framework-2024.4.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,31 +36,24 @@
     'amuse': [
         '*rc'
     ]
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/_version.py",
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
```

### Comparing `amuse-framework-2023.5.0/src/amuse/__init__.py` & `amuse_framework-2024.4.0rc1/src/amuse/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 try:
     from . import config
 except Exception as ex:
     message="Configuration not read in - or configuration invalid, exception:\n"+str(ex)
     config=NoConfig(message)
 
 
-
 # always report AMUSE reference information
 try:
     from amuse.support.literature import TrackLiteratureReferences
     TrackLiteratureReferences.default()
 except:
     pass
```

### Comparing `amuse-framework-2023.5.0/src/amuse/codes.py` & `amuse_framework-2024.4.0rc1/src/amuse/codes.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/community/__init__.py` & `amuse_framework-2024.4.0rc1/src/amuse/community/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/community/interface/common.py` & `amuse_framework-2024.4.0rc1/src/amuse/community/interface/common.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/community/interface/example.py` & `amuse_framework-2024.4.0rc1/src/amuse/community/interface/example.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/community/interface/gd.py` & `amuse_framework-2024.4.0rc1/src/amuse/community/interface/gd.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,54 +503,14 @@
             particle could not be found
         -2 - ERROR
             not yet implemented
         """
         return function
 
     @legacy_function
-    def set_acceleration():
-        """
-        Update the acceleration of a particle.
-        *Defined for symetry with the get_acceleration function.*
-        *Should be removed if physaccily unsound*
-        *Maybe moved to snapshot support functionality*
-        """
-        function = LegacyFunctionSpecification()
-        function.addParameter(
-            'index_of_the_particle', dtype='int32', direction=function.IN,
-            description=(
-                "Index of the particle for which the state is to be updated. "
-                "This index must have been returned by an earlier call to "
-                ":meth:`new_particle`"
-            )
-        )
-        function.addParameter(
-            'ax', dtype='float64', direction=function.IN,
-            description="The new acceleration vector of the particle")
-        function.addParameter(
-            'ay', dtype='float64', direction=function.IN,
-            description="The new acceleration vector of the particle")
-        function.addParameter(
-            'az', dtype='float64', direction=function.IN,
-            description="The new acceleration vector of the particle")
-        function.result_type = 'int32'
-        function.can_handle_array = True
-        function.result_doc = """
-        0 - OK
-            particle was found in the model and the information was set
-        -1 - ERROR
-            particle could not be found
-        -2 - ERROR
-            code does not support updating of a particle
-        -3 - ERROR
-            not yet implemented
-        """
-        return function
-
-    @legacy_function
     def get_potential():
         """
         Retrieve the potential at a particle position, for retrieving the
         potential anywhere in the field use get_potential_at_point.
         """
         function = LegacyFunctionSpecification()
```

### Comparing `amuse-framework-2023.5.0/src/amuse/community/interface/hydro.py` & `amuse_framework-2024.4.0rc1/src/amuse/community/interface/hydro.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/community/interface/mhd.py` & `amuse_framework-2024.4.0rc1/src/amuse/community/interface/mhd.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/community/interface/se.py` & `amuse_framework-2024.4.0rc1/src/amuse/community/interface/se.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/community/interface/stopping_conditions.py` & `amuse_framework-2024.4.0rc1/src/amuse/community/interface/stopping_conditions.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/config.py` & `amuse_framework-2024.4.0rc1/src/amuse/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 # -*- coding: utf-8 -*-
 """
 configuration from config.mk
 """
 import os
 import warnings
 
-
-def parse_configmk(filename):
-    configfile = open(filename, "r")
-    lines = configfile.readlines()
-    configfile.close()
+def parse_configmk_lines(lines,label):
     cfgvars = dict()
     if "amuse configuration" not in lines[0]:
         raise Exception(
-            "file: {0} is not an amuse configuration file".format(filename)
+            f"{label} is not an amuse configuration file"
         )
     for line in lines:
         if "=" in line:
             var, value = line.split("=", 1)
             if value.startswith("@") and value.endswith("@"):
                 warnings.warn(
-                    "possible configuration error/ unconfigured variable in"
-                    " {0}".format(filename)
+                    f"possible configuration error/ unconfigured variable in"
+                    f" {label}"
                 )
             cfgvars[var] = value.strip()
     return cfgvars
 
+def parse_configmk(filename):
+    configfile = open(filename, "r")
+    lines = configfile.readlines()
+    configfile.close()
+    return parse_configmk_lines(lines, "file " + filename)
 
 try:
     configmk = parse_configmk("config.mk")
 except IOError:
     from .support import get_amuse_root_dir
     configmk = parse_configmk(
         os.path.join(get_amuse_root_dir(), "config.mk")
```

### Comparing `amuse-framework-2023.5.0/src/amuse/couple/bridge.py` & `amuse_framework-2024.4.0rc1/src/amuse/couple/bridge.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
   bridge-like integrator for amuse
 
   the bridge class provides a bridge like coupling between different
   gravitational integrators. In this way a system composed of multiple
   components can be evolved taking account of the self gravity of the whole
-  system self consistently, while choosing the most appropiate integrator
+  system self consistently, while choosing the most appropriate integrator
   for the self-gravity of the component systems. This is mainly useful for
   systems  consist of two or more components that are either well separated
   spatially or have different scales (otherwise using a single integrator is
   more efficient)
 
   The main idea is that systems experience each others gravity through
   periodic velocty kicks with ordinary evolution in  between - the evolution
@@ -42,30 +42,30 @@
 
   bridgesys.add_system(galaxy, (cluster,), False)
 
   has three arguments: the system, a set with *interaction* partners and
   a flag to specify whether synchronization is needed . The
   interaction partners indicate which systems will kick the system. In the
   most simple case these  would be the set of other systems that are added,
-  but usually this is not  what you want to get good performace. In some
+  but usually this is not  what you want to get good performance. In some
   cases you want to ignore one  direction of interaction (eg. in a combined
   simulation of a galaxy and a  comet orbits around a star you may want the
   ignore the gravity of the comet), in other cases you want to use a
   different force calculator (eg integrating a cluster in  a galaxy where
   the galaxy is evolved with a tree code and the cluster with a direct sum
   code, one also would want to use a tree code to calculate the cluster
   gravity for the galaxy. In such a case one can derive a skeleton gravity
   interface from  the cluster system.  A module is provided with some
   examples of such *derived* systems, derived_grav_systems.py
 
   Hints for good use:
 
   The bridgesys is flexible but care should be taken in order to obtain
   valid results. For one thing, there is no restriction or check on the
-  validity of the assumption of well seperated dynamics: for example any
+  validity of the assumption of well separated dynamics: for example any
   system could be split up and put together in bridge, but if the timestep
   is chosen to be larger than the timestep criterion of the code, the
   integration will show errors.
 
   For good performance one should use derived systems to reduce the
   complexity where possible.
 
@@ -88,16 +88,15 @@
 
 from amuse.units import quantities
 from amuse.units import units, constants, generic_unit_system, nbody_system
 from amuse import datamodel
 from amuse.support.exceptions import AmuseException, CoreException
 
 
-
-class AbstractCalculateFieldForCodes(object):
+class AbstractCalculateFieldForCodes:
     """
     Calculated gravity and potential fields using the particles
     of other codes with the code provided.
     """
 
     def __init__(self, input_codes, verbose=False, required_attributes=None):
         """
@@ -108,41 +107,47 @@
         field. For example, some codes don't need the velocity. Other codes
         may (wrongly) interpret the radius of the input code as gravitational
         softening. In the latter case
             required_attributes=['mass', 'x','y','z', 'vx','vy','vz']
         should prevent the radius of the input codes from being used.
         """
         self.codes_to_calculate_field_for = input_codes
-        self.verbose=verbose
+        self.verbose = verbose
         if required_attributes is None:
             self.required_attributes = lambda p, attribute_name: True
         else:
-            self.required_attributes = lambda p, attribute_name: attribute_name in required_attributes
+            self.required_attributes = (
+                lambda p, attribute_name: attribute_name in required_attributes
+            )
 
     def evolve_model(self,tend,timestep=None):
         """
         """
 
-    def get_potential_at_point(self,radius,x,y,z):
+    def get_potential_at_point(self, radius, x, y, z):
         code = self._setup_code()
         try:
             for input_code in self.codes_to_calculate_field_for:
-                particles = input_code.particles.copy(filter_attributes = self.required_attributes)
+                particles = input_code.particles.copy(
+                    filter_attributes=self.required_attributes
+                )
                 code.particles.add_particles(particles)
-            return code.get_potential_at_point(radius,x,y,z)
+            return code.get_potential_at_point(radius, x, y, z)
         finally:
             self._cleanup_code(code)
 
-    def get_gravity_at_point(self,radius,x,y,z):
+    def get_gravity_at_point(self, radius, x, y, z):
         code = self._setup_code()
         try:
             for input_code in self.codes_to_calculate_field_for:
-                particles = input_code.particles.copy(filter_attributes = self.required_attributes)
+                particles = input_code.particles.copy(
+                    filter_attributes=self.required_attributes
+                )
                 code.particles.add_particles(particles)
-            return code.get_gravity_at_point(radius,x,y,z)
+            return code.get_gravity_at_point(radius, x, y, z)
         finally:
             self._cleanup_code(code)
 
     def _setup_code(self):
         pass
 
     def _cleanup_code(self, code):
@@ -162,14 +167,15 @@
 
     def _setup_code(self):
         return self.code_factory_function()
 
     def _cleanup_code(self, code):
         code.stop()
 
+
 class CalculateFieldForCodesUsingReinitialize(AbstractCalculateFieldForCodes):
     """
     Calculated gravity and potential fields using the particles
     of other codes with the code provided.
     The code is created for every calculation.
     """
 
@@ -179,14 +185,15 @@
 
     def _setup_code(self):
         return self.code
 
     def _cleanup_code(self, code):
         code.reset()
 
+
 class CalculateFieldForCodesUsingRemove(AbstractCalculateFieldForCodes):
     """
     Calculated gravity and potential fields using the particles
     of other codes with the code provided.
     The code is created for every calculation.
     """
 
@@ -197,210 +204,230 @@
     def _setup_code(self):
         return self.code
 
     def _cleanup_code(self, code):
         code.particles.remove_particles(code.particles)
 
 
-class CalculateFieldForParticles(object):
+class CalculateFieldForParticles:
     """
     Calculates an field for a set of particles, the set
     of particles can be from another code.
     """
 
-    def __init__(self, particles = None, gravity_constant = None,
-            softening_mode="shared", G = None):
+    def __init__(
+        self, particles=None, gravity_constant=None, softening_mode="shared", G=None
+    ):
         if particles is None:
-            self.particles=datamodel.Particles()
+            self.particles = datamodel.Particles()
         else:
             self.particles = particles
         if gravity_constant is None:
             gravity_constant = G
-        elif not G is None:
-            raise Exception("both the parameter 'gravity_constant'({0}) and the parameter 'G'({1}) are given, please specify only one!".format(gravity_constant, G))
-            
+        elif G is not None:
+            raise Exception(
+                "both the parameter 'gravity_constant'({0}) and the parameter 'G'({1}) are given, please specify only one!".format(
+                    gravity_constant, G
+                )
+            )
+
         if gravity_constant is None:
-            if len(particles) and hasattr(particles, 'mass'):
+            if len(particles) and hasattr(particles, "mass"):
                 try:
                     particles[0].mass.value_in(units.kg)
                     self.gravity_constant = constants.G
                 except:
-                    raise AmuseException("For generic units the gravity_constant must be specified")
+                    raise AmuseException(
+                        "For generic units the gravity_constant must be specified"
+                    )
             else:
-                raise AmuseException("Particle data not yet available, so the gravity_constant must be specified")
+                raise AmuseException(
+                    "Particle data not yet available, so the gravity_constant "
+                    "must be specified"
+                )
         else:
             self.gravity_constant = gravity_constant
 
         if softening_mode == "individual" or softening_mode == "radius":
             self._softening_lengths_squared = self._softening_lengths_squared_individual
         elif softening_mode == "h_smooth":
             self._softening_lengths_squared = self._softening_lengths_squared_h_smooth
         else:
             self._softening_lengths_squared = self._softening_lengths_squared_shared
         self.smoothing_length_squared = quantities.zero
 
     def _softening_lengths_squared_individual(self):
         return self.particles.radius**2
+
     def _softening_lengths_squared_h_smooth(self):
         return self.particles.h_smooth**2
+
     def _softening_lengths_squared_shared(self):
-        return self.smoothing_length_squared#.as_vector_with_length(len(self.particles))
+        return (
+            self.smoothing_length_squared
+        )
 
     def cleanup_code(self):
         self.particles = datamodel.Particles()
 
     def evolve_model(self,tend,timestep=None):
         """
         """
 
-    def get_potential_at_point(self,radius,x,y,z):
+    def get_potential_at_point(self, radius, x, y, z):
         positions = self.particles.position
         result = quantities.AdaptingVectorQuantity()
 
         for i in range(len(x)):
             dx = x[i] - positions.x
             dy = y[i] - positions.y
             dz = z[i] - positions.z
             dr_squared = (dx * dx) + (dy * dy) + (dz * dz)
             dr = (dr_squared + self._softening_lengths_squared()).sqrt()
             energy_of_this_particle = (self.particles.mass / dr).sum()
             result.append(-self.gravity_constant * energy_of_this_particle)
         return result
 
-
-    def get_gravity_at_point(self,radius,x,y,z):
+    def get_gravity_at_point(self, radius, x, y, z):
         positions = self.particles.position
         m1 = self.particles.mass
         result_ax = quantities.AdaptingVectorQuantity()
         result_ay = quantities.AdaptingVectorQuantity()
         result_az = quantities.AdaptingVectorQuantity()
         for i in range(len(x)):
             dx = x[i] - positions.x
             dy = y[i] - positions.y
             dz = z[i] - positions.z
-            dr_squared = ((dx * dx) + (dy * dy) + (dz * dz) +
-                self._softening_lengths_squared() + radius[i]**2)
+            dr_squared = (
+                (dx * dx)
+                + (dy * dy)
+                + (dz * dz)
+                + self._softening_lengths_squared()
+                + radius[i] ** 2
+            )
 
-            ax = -self.gravity_constant * (m1*dx/dr_squared**1.5).sum()
-            ay = -self.gravity_constant * (m1*dy/dr_squared**1.5).sum()
-            az = -self.gravity_constant * (m1*dz/dr_squared**1.5).sum()
+            ax = -self.gravity_constant * (m1 * dx / dr_squared**1.5).sum()
+            ay = -self.gravity_constant * (m1 * dy / dr_squared**1.5).sum()
+            az = -self.gravity_constant * (m1 * dz / dr_squared**1.5).sum()
 
             result_ax.append(ax)
             result_ay.append(ay)
             result_az.append(az)
         return result_ax, result_ay, result_az
 
 
-
-
-class GravityCodeInField(object):
-
-
-    def __init__(self, code, field_codes, do_sync=True, verbose=False, radius_is_eps=False, h_smooth_is_eps=False, zero_smoothing=False):
+class GravityCodeInField:
+    def __init__(
+        self,
+        code,
+        field_codes,
+        do_sync=True,
+        verbose=False,
+        radius_is_eps=False,
+        h_smooth_is_eps=False,
+        zero_smoothing=False,
+    ):
         """
         verbose indicates whether to output some run info
         """
         self.code = code
         self.field_codes = field_codes
 
-        if hasattr(self.code, 'model_time'):
+        if hasattr(self.code, "model_time"):
             self.time = self.code.model_time
         else:
             self.time = quantities.zero
 
-        self.do_sync=do_sync
-        self.verbose=verbose
-        self.timestep=None
+        self.do_sync = do_sync
+        self.verbose = verbose
+        self.timestep = None
         self.radius_is_eps = radius_is_eps
         self.h_smooth_is_eps = h_smooth_is_eps
 
-        required_attributes = ['mass', 'x', 'y', 'z', 'vx', 'vy', 'vz']
+        required_attributes = ["mass", "x", "y", "z", "vx", "vy", "vz"]
         if self.radius_is_eps:
-            required_attributes.append('radius')
+            required_attributes.append("radius")
         elif self.h_smooth_is_eps:
-            required_attributes.append('h_smooth')
-        self.required_attributes = lambda p, x : x in required_attributes
+            required_attributes.append("h_smooth")
+        self.required_attributes = lambda p, x: x in required_attributes
 
         try:
             hasattr(self.code.parameters, "epsilon_squared")
             self.zero_smoothing = zero_smoothing
         except AttributeError:
             self.zero_smoothing = True
         except CoreException:  # hasattr will fail with an exception
             self.zero_smoothing = True
 
-
-    def evolve_model(self,tend,timestep=None):
+    def evolve_model(self, tend, timestep=None):
         """
         evolve combined system to tend, timestep fixes timestep
         """
 
         if timestep is None:
             timestep = self.timestep
 
-        first=True
-        while self.time < (tend-timestep/2.):
+        first = True
+        while self.time < (tend - timestep / 2.0):
             if first:
-                self.kick(timestep/2.)
-                first=False
+                self.kick(timestep / 2.0)
+                first = False
             else:
                 self.kick(timestep)
 
-            self.drift(self.time+timestep)
+            self.drift(self.time + timestep)
 
-            self.time+=timestep
+            self.time += timestep
 
         if not first:
-             self.kick(timestep/2.)
-
-
+            self.kick(timestep / 2.0)
 
     def synchronize_model(self):
         """
         explicitly synchronize all components
         """
-        if hasattr(self.code,"synchronize_model"):
-            if(self.verbose):
-                print(self.code.__class__.__name__,"is synchronizing", end=' ')
+        if hasattr(self.code, "synchronize_model"):
+            if self.verbose:
+                print(self.code.__class__.__name__, "is synchronizing", end=" ")
 
             self.code.synchronize_model()
 
-            if(self.verbose):
+            if self.verbose:
                 print(".. done")
 
-    def get_potential_at_point(self,radius,x,y,z):
-        return self.code.get_potential_at_point(radius,x,y,z)
+    def get_potential_at_point(self, radius, x, y, z):
+        return self.code.get_potential_at_point(radius, x, y, z)
 
-    def get_gravity_at_point(self,radius,x,y,z):
-        return self.code.get_gravity_at_point(radius,x,y,z)
+    def get_gravity_at_point(self, radius, x, y, z):
+        return self.code.get_gravity_at_point(radius, x, y, z)
 
     @property
     def model_time(self):
-         return self.time
+        return self.time
 
     @property
     def potential_energy(self):
-        if not hasattr(self.code, 'particles'):
+        if not hasattr(self.code, "particles"):
             return quantities.zero
 
         result = self.code.potential_energy
-        particles = self.code.particles.copy(filter_attributes = self.required_attributes)
+        particles = self.code.particles.copy(filter_attributes=self.required_attributes)
 
         for y in self.field_codes:
             energy = self.get_potential_energy_in_field_code(particles, y)
             result += energy
         return result
 
     @property
     def kinetic_energy(self):
         return self.code.kinetic_energy
 
     @property
     def thermal_energy(self):
-        if hasattr(self.code,'thermal_energy'):
+        if hasattr(self.code, "thermal_energy"):
             return self.code.thermal_energy
         else:
             return quantities.zero
 
     @property
     def particles(self):
         return self.code.particles
@@ -416,298 +443,315 @@
     def dm_particles(self):
         if hasattr(self.code, "dm_particles"):
             return self.code.dm_particles
         else:
             raise AttributeError
 
     def drift(self, tend):
-        if not hasattr(self.code,"evolve_model"):
+        if not hasattr(self.code, "evolve_model"):
             return
-        if (self.verbose):
+        if self.verbose:
             print(self.code.__class__.__name__, "is evolving to", tend)
 
         self.code.evolve_model(tend)
 
-
-        if(self.verbose):
+        if self.verbose:
             print(".. done")
 
     def cannot_kick(self):
         """
-            check if the code is capable of kicking other particles,
-            please do not try to optimize this, I know it is called every kick but
-            only calculating it at the start causes an annoying bug in certain uses of the code.
-        """
-        return len(self.code.particles)==0 or not (hasattr(self, 'particles') and 'vx' in self.particles.get_attribute_names_defined_in_store())
+        check if the code is capable of kicking other particles,
+        please do not try to optimize this, I know it is called every kick but
+        only calculating it at the start causes an annoying bug in certain uses
+        of the code.
+        """
+        return len(self.code.particles) == 0 or not (
+            hasattr(self, "particles")
+            and "vx" in self.particles.get_attribute_names_defined_in_store()
+        )
 
     def kick(self, dt):
-
         if self.cannot_kick():
             return quantities.zero
 
-        particles = self.code.particles.copy(filter_attributes = self.required_attributes)
+        particles = self.code.particles.copy(filter_attributes=self.required_attributes)
         kinetic_energy_before = particles.kinetic_energy()
 
         for field_code in self.field_codes:
-            if(self.verbose):
-                print(self.code.__class__.__name__,"receives kick from",field_code.__class__.__name__, end=' ')
+            if self.verbose:
+                print(
+                    self.code.__class__.__name__,
+                    "receives kick from",
+                    field_code.__class__.__name__,
+                    end=" ",
+                )
 
-            self.kick_with_field_code(
-                particles,
-                field_code,
-                dt
-            )
+            self.kick_with_field_code(particles, field_code, dt)
 
-            if(self.verbose):
+            if self.verbose:
                 print(".. done")
 
-        channel=particles.new_channel_to(self.code.particles)
-        channel.copy_attributes(["vx","vy","vz"])
+        channel = particles.new_channel_to(self.code.particles)
+        channel.copy_attributes(["vx", "vy", "vz"])
 
         kinetic_energy_after = particles.kinetic_energy()
         return kinetic_energy_after - kinetic_energy_before
 
-
     def _softening_lengths(self, particles):
         if self.radius_is_eps:
             return particles.radius
         elif self.h_smooth_is_eps:
             return particles.h_smooth
         elif self.zero_smoothing:
-            return 0.*particles.x
+            return 0.0 * particles.x
         else:
-            return (self.code.parameters.epsilon_squared**0.5).as_vector_with_length(len(particles))
+            return (self.code.parameters.epsilon_squared**0.5).as_vector_with_length(
+                len(particles)
+            )
 
     def get_potential_energy_in_field_code(self, particles, field_code):
-        pot=field_code.get_potential_at_point(
-            self._softening_lengths(particles),
-            particles.x,
-            particles.y,
-            particles.z
+        pot = field_code.get_potential_at_point(
+            self._softening_lengths(particles), particles.x, particles.y, particles.z
         )
-        return (pot*particles.mass).sum() / 2
+        return (pot * particles.mass).sum() / 2
 
     def kick_with_field_code(self, particles, field_code, dt):
-        ax,ay,az=field_code.get_gravity_at_point(
-            self._softening_lengths(particles),
-            particles.x,
-            particles.y,
-            particles.z
+        ax, ay, az = field_code.get_gravity_at_point(
+            self._softening_lengths(particles), particles.x, particles.y, particles.z
         )
         self.update_velocities(particles, dt, ax, ay, az)
 
-    def update_velocities(self,particles, dt,  ax, ay, az):
+    def update_velocities(self, particles, dt, ax, ay, az):
         particles.vx += dt * ax
         particles.vy += dt * ay
         particles.vz += dt * az
 
     def stop(self):
         self.code.stop()
 
-class Bridge(object):
-    def __init__(self, timestep = None, verbose=False, use_threading=True,method=None):
+
+class Bridge:
+    def __init__(self, timestep=None, verbose=False, use_threading=True, method=None):
         """
         verbose indicates whether to output some run info
         """
-        self.codes=[]
-        self.time=quantities.zero
-        self.verbose=verbose
-        self.timestep=timestep
+        self.codes = []
+        self.time = quantities.zero
+        self.verbose = verbose
+        self.timestep = timestep
         self.kick_energy = quantities.zero
         self.use_threading = use_threading
-        self.time_offsets = dict()
-        self.method=method
+        self.time_offsets = {}
+        self.method = method
         self.channels = datamodel.Channels()
 
-    def add_system(self, interface, partners=set(), do_sync=True,
-            radius_is_eps=False, h_smooth_is_eps=False, zero_smoothing=False):
+    def add_system(
+        self,
+        interface,
+        partners=set(),
+        do_sync=True,
+        radius_is_eps=False,
+        h_smooth_is_eps=False,
+        zero_smoothing=False,
+    ):
         """
         add a system to bridge integrator
         """
 
         if hasattr(interface, "particles"):
-            code = GravityCodeInField(interface, partners, do_sync, self.verbose,
-                radius_is_eps, h_smooth_is_eps, zero_smoothing)
+            code = GravityCodeInField(
+                interface,
+                partners,
+                do_sync,
+                self.verbose,
+                radius_is_eps,
+                h_smooth_is_eps,
+                zero_smoothing,
+            )
             self.add_code(code)
         else:
             if len(partners):
-                raise Exception("You added a code without particles, but with partners, this is not supported!")
+                raise Exception(
+                    "You added a code without particles, but with partners, "
+                    "this is not supported!"
+                )
             self.add_code(interface)
 
     def add_code(self, code):
         self.codes.append(code)
-        if hasattr(code,"model_time"):
-            self.time_offsets[code]=(self.time-code.model_time)
+        if hasattr(code, "model_time"):
+            self.time_offsets[code] = self.time - code.model_time
         else:
-            self.time_offsets[code]=quantities.zero
-
+            self.time_offsets[code] = quantities.zero
 
     def evolve_model(self, tend, timestep=None):
         """
         evolve combined system to tend, timestep fixes timestep
         """
         if timestep is None:
             if self.timestep is None:
-                timestep=tend-self.time
+                timestep = tend - self.time
             else:
                 timestep = self.timestep
 
         if self.method is None:
-            return self.evolve_joined_leapfrog(tend,timestep)
+            return self.evolve_joined_leapfrog(tend, timestep)
         else:
-            return self.evolve_simple_steps(tend,timestep)
+            return self.evolve_simple_steps(tend, timestep)
 
-    def evolve_simple_steps(self,tend,timestep):
-        while self.time < (tend-timestep/2):
-            self._drift_time=self.time
-            self.method(self.kick_codes,self.drift_codes_dt, timestep)
+    def evolve_simple_steps(self, tend, timestep):
+        while self.time < (tend - timestep / 2):
+            self._drift_time = self.time
+            self.method(self.kick_codes, self.drift_codes_dt, timestep)
             self.channels.copy()
-            self.time=self.time+timestep
+            self.time = self.time + timestep
 
-    def evolve_joined_leapfrog(self,tend,timestep):
-        first=True
-        while self.time < (tend-timestep/2.):
+    def evolve_joined_leapfrog(self, tend, timestep):
+        first = True
+        while self.time < (tend - timestep / 2.0):
             if first:
-                self.kick_codes(timestep/2.)
-                first=False
+                self.kick_codes(timestep / 2.0)
+                first = False
             else:
                 self.kick_codes(timestep)
 
-            self.drift_codes(self.time+timestep)
+            self.drift_codes(self.time + timestep)
 
             self.channels.copy()
             self.time += timestep
 
         if not first:
-            self.kick_codes(timestep/2.)
-
+            self.kick_codes(timestep / 2.0)
 
     def synchronize_model(self):
         """
         explicitly synchronize all components
         """
         for x in self.codes:
-            if hasattr(x,"synchronize_model"):
-                if(self.verbose): print(x.__class__.__name__,"is synchronizing", end=' ')
+            if hasattr(x, "synchronize_model"):
+                if self.verbose:
+                    print(x.__class__.__name__, "is synchronizing", end=" ")
                 x.synchronize_model()
-                if(self.verbose): print(".. done")
+                if self.verbose:
+                    print(".. done")
 
     def stop(self):
         for one_code in self.codes:
             if hasattr(one_code, "stop"):
                 one_code.stop()
 
-    def get_potential_at_point(self,radius,x,y,z):
-        pot=quantities.zero
+    def get_potential_at_point(self, radius, x, y, z):
+        pot = quantities.zero
         for code in self.codes:
-            _pot=code.get_potential_at_point(radius,x,y,z)
-            pot=pot+_pot
+            _pot = code.get_potential_at_point(radius, x, y, z)
+            pot = pot + _pot
         return pot
 
-    def get_gravity_at_point(self,radius,x,y,z):
-        ax=quantities.zero
-        ay=quantities.zero
-        az=quantities.zero
+    def get_gravity_at_point(self, radius, x, y, z):
+        ax = quantities.zero
+        ay = quantities.zero
+        az = quantities.zero
         for code in self.codes:
-            _ax,_ay,_az=code.get_gravity_at_point(radius,x,y,z)
-            ax=ax+_ax
-            ay=ay+_ay
-            az=az+_az
-        return ax,ay,az
+            _ax, _ay, _az = code.get_gravity_at_point(radius, x, y, z)
+            ax = ax + _ax
+            ay = ay + _ay
+            az = az + _az
+        return ax, ay, az
 
     @property
     def model_time(self):
-         return self.time
+        return self.time
 
     @property
     def potential_energy(self):
-        result=quantities.zero
+        result = quantities.zero
         for x in self.codes:
-            result+=x.potential_energy
+            result += x.potential_energy
         return result
 
     @property
     def kinetic_energy(self):
-        result=quantities.zero
+        result = quantities.zero
         for x in self.codes:
-            result+=x.kinetic_energy
-        return result #- self.kick_energy
+            result += x.kinetic_energy
+        return result
 
     @property
     def thermal_energy(self):
-        result=quantities.zero
+        result = quantities.zero
         for x in self.codes:
-            if hasattr(x,'thermal_energy'):
-                result+=x.thermal_energy
+            if hasattr(x, "thermal_energy"):
+                result += x.thermal_energy
         return result
 
     @property
     def particles(self):
-        array=[]
+        array = []
         for x in self.codes:
-            if hasattr(x,"particles"):
+            if hasattr(x, "particles"):
                 array.append(x.particles)
         if len(array) == 0:
             raise AttributeError
         elif len(array) == 1:
             return array[0]
         return datamodel.ParticlesSuperset(array)
 
     @property
     def gas_particles(self):
-        array=[]
+        array = []
         for x in self.codes:
-            if hasattr(x,"gas_particles"):
+            if hasattr(x, "gas_particles"):
                 array.append(x.gas_particles)
         if len(array) == 0:
             raise AttributeError
         elif len(array) == 1:
             return array[0]
         return datamodel.ParticlesSuperset(array)
 
     @property
     def dm_particles(self):
-        array=[]
+        array = []
         for x in self.codes:
-            if hasattr(x,"dm_particles"):
+            if hasattr(x, "dm_particles"):
                 array.append(x.dm_particles)
-            elif hasattr(x,"particles"):
+            elif hasattr(x, "particles"):
                 array.append(x.particles)
         if len(array) == 0:
             raise AttributeError
         elif len(array) == 1:
             return array[0]
         return datamodel.ParticlesSuperset(array)
 
-# 'private' functions
-    def drift_codes_dt(self,dt):
-        self._drift_time+=dt
+    # 'private' functions
+    def drift_codes_dt(self, dt):
+        self._drift_time += dt
         self.drift_codes(self._drift_time)
 
-    def drift_codes(self,tend):
-        threads=[]
+    def drift_codes(self, tend):
+        threads = []
 
         for x in self.codes:
-            offset=self.time_offsets[x]
-            if hasattr(x,"drift"):
-                threads.append(threading.Thread(target=x.drift, args=(tend-offset,)) )
-            elif hasattr(x,"evolve_model"):
-                threads.append(threading.Thread(target=x.evolve_model, args=(tend-offset,)) )
+            offset = self.time_offsets[x]
+            if hasattr(x, "drift"):
+                threads.append(threading.Thread(target=x.drift, args=(tend - offset,)))
+            elif hasattr(x, "evolve_model"):
+                threads.append(
+                    threading.Thread(target=x.evolve_model, args=(tend - offset,))
+                )
 
         if self.use_threading:
             for x in threads:
                 x.start()
 
             for x in threads:
                 x.join()
         else:
             for x in threads:
                 x.run()
 
-    def kick_codes(self,dt):
-
+    def kick_codes(self, dt):
         de = quantities.zero
         for x in self.codes:
-            if hasattr(x,"kick"):
+            if hasattr(x, "kick"):
                 de += x.kick(dt)
 
         self.kick_energy += de
```

### Comparing `amuse-framework-2023.5.0/src/amuse/couple/collision_handler.py` & `amuse_framework-2024.4.0rc1/src/amuse/couple/collision_handler.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/couple/encounters.py` & `amuse_framework-2024.4.0rc1/src/amuse/couple/encounters.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/couple/fallback_stellar_evolution.py` & `amuse_framework-2024.4.0rc1/src/amuse/couple/fallback_stellar_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/couple/multiples.py` & `amuse_framework-2024.4.0rc1/src/amuse/couple/multiples.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/couple/parallel_stellar_evolution.py` & `amuse_framework-2024.4.0rc1/src/amuse/couple/parallel_stellar_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/data/AMUSE.bib` & `amuse_framework-2024.4.0rc1/src/amuse/data/AMUSE.bib`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/attributes.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/base.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/base.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/grid_attributes.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/grid_attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/grids.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/grids.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,21 +554,23 @@
     def shape(self):
         return indexing.shape_after_index(self._private.grid.shape, self._private.indices )
 
     def indices(self):
         return [x[self._private.indices] for x in self._original_set().indices()]
         
     def __eq__(self, other):
-        if self._private.grid!=other._private.grid:
-          return False
-        else:
-          if numpy.all(numpy.array(self.indices())==numpy.array(other.indices())):
-            return True
-          else:
+        if self._private.grid != other._private.grid:
+            return False
+        elif self.shape != other.shape:
             return False
+        else:
+            if numpy.all(numpy.array(self.indices())==numpy.array(other.indices())):
+                return True
+            else:
+                return False
         
     def __ne__(self,other):
         return not(self==other)
 
     def _factory_for_new_collection(self):
         return Grid
```

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/incode_storage.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/incode_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1130,15 +1130,15 @@
             returned_value = mapping_from_attribute_to_result[attribute]
             
             if len(array_of_indices)==0:
                 value=returned_value
             elif len(array_of_indices[0].shape) == 0:
                 value = returned_value[0]
             else:
-                if len(returned_value)!=numpy.product(array_of_indices[0].shape):
+                if len(returned_value)!=numpy.prod(array_of_indices[0].shape):
                     raise Exception("unexpected mismatch of array shapes")
                 if isinstance(returned_value,list):
                   returned_value=numpy.asarray(returned_value)
                 value = returned_value.reshape(array_of_indices[0].shape+returned_value.shape[1:])
                 
             results.append(value)
```

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/indexing.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/indexing.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/memory_storage.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/memory_storage.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/parameters.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/parameters.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/particle_attributes.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/particle_attributes.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/particles.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/particles.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/simple_hash.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/simple_hash.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/staggeredgrid.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/staggeredgrid.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/datamodel/trees.py` & `amuse_framework-2024.4.0rc1/src/amuse/datamodel/trees.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/ClusterCore.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/ClusterCore.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/LagrangianRadii.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/LagrangianRadii.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/SConstruct` & `amuse_framework-2024.4.0rc1/src/amuse/ext/SConstruct`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/basicgraph.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/basicgraph.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/bbr_color.txt` & `amuse_framework-2024.4.0rc1/src/amuse/ext/bbr_color.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/bhtc_interface.pyx` & `amuse_framework-2024.4.0rc1/src/amuse/ext/bhtc_interface.pyx`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/blender/blender.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/blender/blender.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/boss_bodenheimer.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/boss_bodenheimer.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/bridge.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/bridge.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/cloud.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/cloud.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/composition_methods.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/composition_methods.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/comsystem.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/comsystem.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/concurrent.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/concurrent.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/cosmo.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/cosmo.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/derived_grav_systems.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/derived_grav_systems.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/evrard_test.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/evrard_test.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/galactic_potentials.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/galactic_potentials.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/galactics_model.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/galactics_model.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/gasplummer.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/gasplummer.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/grid_remappers.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/grid_remappers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,326 +1,382 @@
 import numpy
 
 from amuse.units import units
 
-from amuse.units.quantities import is_quantity, value_in, to_quantity
+from amuse.units.quantities import value_in, to_quantity
 
-from amuse.datamodel import UnstructuredGrid, StructuredGrid, StructuredBaseGrid, RegularBaseGrid
+from amuse.datamodel import (
+    UnstructuredGrid,
+    StructuredBaseGrid,
+    RegularBaseGrid,
+)
 
 try:
-  import matplotlib
-  from matplotlib import tri
-  if not hasattr(tri, "LinearTriInterpolator"):
-      raise Exception("LinearTriInterpolator not in matplotlib.tri")
-  matplotlib_available=True
+    import matplotlib
+    from matplotlib import tri
+
+    if not hasattr(tri, "LinearTriInterpolator"):
+        raise Exception("LinearTriInterpolator not in matplotlib.tri")
+    matplotlib_available = True
 except:
-  matplotlib_available=False
+    matplotlib_available = False
 
 from warnings import warn
 
+
 class interpolating_2D_remapper(object):
-    def __init__(self, source, target,axes_names=None):
-        """ this class maps a source grid to a target grid using linear 
-            interpolation on a triangulation generated by adding a 
-            midpoint to every cell (source should be a structured grid) 
-            and thus generating 4 triangles for each cell. Values of the 
-            midpoints are averaged from the corners. 
+    def __init__(self, source, target, axes_names=None):
+        """this class maps a source grid to a target grid using linear
+        interpolation on a triangulation generated by adding a
+        midpoint to every cell (source should be a structured grid)
+        and thus generating 4 triangles for each cell. Values of the
+        midpoints are averaged from the corners.
         """
-        if len(source.shape) !=2:
+        if len(source.shape) != 2:
             raise Exception("source grid is not 2D")
         if not isinstance(source, StructuredBaseGrid):
             raise Exception("source grid is not instance of StructuredBaseGrid")
 
-        self.source=source
-        self.target=target
-        self._axes_names=list(axes_names or source.get_axes_names())
+        self.source = source
+        self.target = target
+        self._axes_names = list(axes_names or source.get_axes_names())
         self.generate_triangulation()
 
-    def _generate_nodes(self,grid,attributes):
+    def _generate_nodes(self, grid, attributes):
 
-        Nx,Ny=grid.shape
+        Nx, Ny = grid.shape
 
-        x,y=numpy.mgrid[0:Nx,0:Ny]
-        x1,y1=numpy.mgrid[0:Nx-1,0:Ny-1]
-                
-        x_=x.flatten()
-        y_=y.flatten()
-        x1_=x1.flatten()
-        y1_=y1.flatten()
+        x, y = numpy.mgrid[0:Nx, 0:Ny]
+        x1, y1 = numpy.mgrid[0:Nx - 1, 0:Ny - 1]
 
-        l1=Nx*Ny
+        x_ = x.flatten()
+        y_ = y.flatten()
+        x1_ = x1.flatten()
+        y1_ = y1.flatten()
 
-        i=numpy.arange(Nx*Ny).reshape((Nx,Ny))
-        i1=(numpy.arange((Nx-1)*(Ny-1))+l1).reshape((Nx-1,Ny-1))
+        l1 = Nx * Ny
 
-      
-        nodes=UnstructuredGrid(len(x_)+len(x1_))
+        nodes = UnstructuredGrid(len(x_) + len(x1_))
         for name in attributes:
-          values1=getattr(grid,name)[x_,y_]
-          values2=getattr(grid,name)[x1_,y1_]+getattr(grid,name)[x1_+1,y1_]+\
-                  getattr(grid,name)[x1_,y1_+1]+getattr(grid,name)[x1_+1,y1_+1]
-          setattr(nodes[0], name, 0.*values1[0])
-          setattr(nodes[:l1], name, 1.*values1)
-          setattr(nodes[l1:], name, values2/4)
+            values1 = getattr(grid, name)[x_, y_]
+            values2 = (
+                getattr(grid, name)[x1_, y1_]
+                + getattr(grid, name)[x1_ + 1, y1_]
+                + getattr(grid, name)[x1_, y1_ + 1]
+                + getattr(grid, name)[x1_ + 1, y1_ + 1]
+            )
+            setattr(nodes[0], name, 0.0 * values1[0])
+            setattr(nodes[:l1], name, 1.0 * values1)
+            setattr(nodes[l1:], name, values2 / 4)
         return nodes
 
-    def _generate_elements_and_boundaries(self,grid):
-        Nx,Ny=grid.shape
+    def _generate_elements_and_boundaries(self, grid):
+        Nx, Ny = grid.shape
+
+        l1 = Nx * Ny
+
+        i = numpy.arange(Nx * Ny).reshape((Nx, Ny))
+        i1 = (numpy.arange((Nx - 1) * (Ny - 1)) + l1).reshape((Nx - 1, Ny - 1))
+
+        e1 = numpy.zeros(((Nx - 1) * (Ny - 1), 3), dtype="i")
+        e2 = numpy.zeros(((Nx - 1) * (Ny - 1), 3), dtype="i")
+        e3 = numpy.zeros(((Nx - 1) * (Ny - 1), 3), dtype="i")
+        e4 = numpy.zeros(((Nx - 1) * (Ny - 1), 3), dtype="i")
+
+        e1[:, 0] = i[:-1, :-1].flatten()
+        e1[:, 1] = i[1:, :-1].flatten()
+        e1[:, 2] = i1[:, :].flatten()
 
-        l1=Nx*Ny
+        e2[:, 0] = i[1:, :-1].flatten()
+        e2[:, 1] = i[1:, 1:].flatten()
+        e2[:, 2] = i1[:, :].flatten()
 
-        i=numpy.arange(Nx*Ny).reshape((Nx,Ny))
-        i1=(numpy.arange((Nx-1)*(Ny-1))+l1).reshape((Nx-1,Ny-1))
+        e3[:, 0] = i[1:, 1:].flatten()
+        e3[:, 1] = i[:-1, 1:].flatten()
+        e3[:, 2] = i1[:, :].flatten()
 
-        e1=numpy.zeros(((Nx-1)*(Ny-1),3),dtype='i')
-        e2=numpy.zeros(((Nx-1)*(Ny-1),3),dtype='i')
-        e3=numpy.zeros(((Nx-1)*(Ny-1),3),dtype='i')
-        e4=numpy.zeros(((Nx-1)*(Ny-1),3),dtype='i')
-                
-        e1[:,0]=i[:-1,:-1].flatten()
-        e1[:,1]=i[1:,:-1].flatten()
-        e1[:,2]=i1[:,:].flatten()
-        
-        e2[:,0]=i[1:,:-1].flatten()
-        e2[:,1]=i[1:,1:].flatten()
-        e2[:,2]=i1[:,:].flatten()
-        
-        e3[:,0]=i[1:,1:].flatten()
-        e3[:,1]=i[:-1,1:].flatten()
-        e3[:,2]=i1[:,:].flatten()
-        
-        e4[:,0]=i[:-1,:-1].flatten()
-        e4[:,1]=i1[:,:].flatten()
-        e4[:,2]=i[:-1,1:].flatten()
-
-        elements=numpy.zeros((4*(Nx-1)*(Ny-1),3),dtype='i8')
-        elements[0::4,:]=e1
-        elements[1::4,:]=e2
-        elements[2::4,:]=e3
-        elements[3::4,:]=e4
-      
-        boundaries=[xx.flatten() for xx in [i[:,0],i[-1,:],i[::-1,-1],i[0,::-1]] ]
-      
-        elem=UnstructuredGrid(len(elements))
-        elem.nodes=elements
+        e4[:, 0] = i[:-1, :-1].flatten()
+        e4[:, 1] = i1[:, :].flatten()
+        e4[:, 2] = i[:-1, 1:].flatten()
 
-        return elem,boundaries
+        elements = numpy.zeros((4 * (Nx - 1) * (Ny - 1), 3), dtype="i8")
+        elements[0::4, :] = e1
+        elements[1::4, :] = e2
+        elements[2::4, :] = e3
+        elements[3::4, :] = e4
+
+        boundaries = [
+            xx.flatten() for xx in [i[:, 0], i[-1, :], i[::-1, -1], i[0, ::-1]]
+        ]
+
+        elem = UnstructuredGrid(len(elements))
+        elem.nodes = elements
+
+        return elem, boundaries
 
     def convert_grid_to_nodes_and_elements(self, grid, attributes=None):
-        
+
         if attributes is None:
-            attributes=grid.get_attribute_names_defined_in_store()
+            attributes = grid.get_attribute_names_defined_in_store()
+
+        nodes = self._generate_nodes(grid, attributes)
+        elements, boundaries = self._generate_elements_and_boundaries(grid)
 
-        nodes=self._generate_nodes(grid, attributes)
-        elements,boundaries=self._generate_elements_and_boundaries(grid)
-      
-        return nodes,elements,boundaries
+        return nodes, elements, boundaries
 
     def generate_triangulation(self):
 
-        nodes,elements,boundaries=self.convert_grid_to_nodes_and_elements(self.source, self._axes_names)
+        nodes, elements, boundaries = self.convert_grid_to_nodes_and_elements(
+            self.source, self._axes_names
+        )
+
+        xpos = to_quantity(getattr(nodes, self._axes_names[0]))
+        ypos = to_quantity(getattr(nodes, self._axes_names[1]))
+
+        self._xpos_unit = xpos.unit
+        xpos = xpos.number
+        self._ypos_unit = ypos.unit
+        ypos = ypos.number
+
+        n1 = elements.nodes[:, 0]
+        n2 = elements.nodes[:, 1]
+        n3 = elements.nodes[:, 2]
+        elem = numpy.column_stack((n1, n2, n3))
 
-        xpos=to_quantity(getattr(nodes,self._axes_names[0]))
-        ypos=to_quantity(getattr(nodes,self._axes_names[1]))
-        
-        self._xpos_unit=xpos.unit
-        xpos=xpos.number
-        self._ypos_unit=ypos.unit
-        ypos=ypos.number
-
-        n1=elements.nodes[:,0]
-        n2=elements.nodes[:,1]
-        n3=elements.nodes[:,2]
-        elem=numpy.column_stack((n1,n2,n3))
+        self._triangulation = tri.Triangulation(xpos, ypos, elem)
 
-        self._triangulation=tri.Triangulation(xpos,ypos,elem)
-        
     def sample(self, values, xpos, ypos):
-        interpolator=tri.LinearTriInterpolator(self._triangulation,values)
-        return interpolator(xpos,ypos)
+        interpolator = tri.LinearTriInterpolator(self._triangulation, values)
+        return interpolator(xpos, ypos)
 
     def forward_mapping(self, attributes, target_names=None):
         if attributes is None:
-            attributes=self.source.get_attribute_names_defined_in_store()
+            attributes = self.source.get_attribute_names_defined_in_store()
         if target_names is None:
-            target_names=attributes
-        
-        source=self.source.empty_copy()
-        channel1=self.source.new_channel_to(source)
-        target=self.target.empty_copy()
-        channel2=self.target.new_channel_to(target)
-        channel3=target.new_channel_to(self.target)
-        
+            target_names = attributes
+
+        source = self.source.empty_copy()
+        channel1 = self.source.new_channel_to(source)
+        target = self.target.empty_copy()
+        channel2 = self.target.new_channel_to(target)
+        channel3 = target.new_channel_to(self.target)
+
         channel1.copy_attributes(attributes)
         channel2.copy_attributes(self._axes_names)
-        
-        nodes=self._generate_nodes(source,attributes)
-                
-        xpos=value_in( getattr(target,self._axes_names[0]), self._xpos_unit)
-        ypos=value_in( getattr(target,self._axes_names[1]), self._ypos_unit)
-                        
+
+        nodes = self._generate_nodes(source, attributes)
+
+        xpos = value_in(getattr(target, self._axes_names[0]), self._xpos_unit)
+        ypos = value_in(getattr(target, self._axes_names[1]), self._ypos_unit)
+
         for attribute, target_name in zip(attributes, target_names):
-            values=to_quantity( getattr(nodes,attribute) ) 
-            unit=values.unit
-            values=values.number
-            samples=self.sample(values,xpos,ypos)
-            setattr(target, target_name, (samples if unit is units.none else (samples | unit)))
+            values = to_quantity(getattr(nodes, attribute))
+            unit = values.unit
+            values = values.number
+            samples = self.sample(values, xpos, ypos)
+            setattr(
+                target,
+                target_name,
+                (samples if unit is units.none else (samples | unit)),
+            )
+
+        channel3.copy_attributes(target_names)
 
-        channel3.copy_attributes(target_names)    
 
 class bilinear_2D_remapper(object):
-    def __init__(self, source, target, check_inside=True, do_slices=False):
-        """ this class maps a source grid to a target grid using bilinear 
-            interpolation. If check_inside=True, raise exception if any 
-            target point outside source grid. If the grids are 3 dimensional
-            it can be used to do a 2D interpolation of each level if shapes 
-            are the same and positions are the same in the 3rd dimension.
+    def __init__(
+        self, source, target, check_inside=True, do_slices=False, x_periodic=False
+    ):
+        """this class maps a source grid to a target grid using bilinear
+        interpolation. If check_inside=True, raise exception if any
+        target point outside source grid. If the grids are 3 dimensional
+        it can be used to do a 2D interpolation of each level if shapes
+        are the same and positions are the same in the 3rd dimension.
         """
-        if len(source.shape)!=2 and not do_slices:
-            raise Exception("source grid is not 2D, set do_slices=True remapping by slices")
-        if len(source.shape)!=len(target.shape):
+        if len(source.shape) != 2 and not do_slices:
+            raise Exception(
+                "source grid is not 2D, set do_slices=True remapping by slices"
+            )
+        if len(source.shape) != len(target.shape):
             raise Exception("incompatible shapes")
-        if len(source.shape)!=2:
-            if numpy.any(source.shape[2:]!=target.shape[2:]):
+        if len(source.shape) != 2:
+            if numpy.any(source.shape[2:] != target.shape[2:]):
                 raise Exception("source and target need same shapes (after dim 2)")
         if not isinstance(source, RegularBaseGrid):
-            raise Exception(f"source grid ({type(source)}) is not instance of RegularBaseGrid")
-
-        self.source=source
-        self.target=target
-        self._axes_names=source.get_axes_names()
-        if len(source.shape)!=2:
+            raise Exception(
+                f"source grid ({type(source)}) is not instance of RegularBaseGrid"
+            )
+
+        self.source = source
+        self.target = target
+        self._axes_names = source.get_axes_names()
+        if len(source.shape) != 2:
             for x in self._axes_names[2:]:
-                if numpy.any(getattr(source[0,0],x)!=getattr(target[0,0],x)):
-                    print(getattr(source[0,0],x))
-                    print(getattr(target[0,0],x))
+                if numpy.any(getattr(source[0, 0], x) != getattr(target[0, 0], x)):
+                    print(getattr(source[0, 0], x))
+                    print(getattr(target[0, 0], x))
                     warn(f"positions (possibly) not the same on axes {x}")
-        self.check_inside=check_inside
-        self._weights=None
-        self._indices=None
+        self.check_inside = check_inside
+        self.x_periodic = x_periodic
+        self._weights = None
+        self._indices = None
 
     def _calculate_weights(self):
-        x0=to_quantity( getattr(self.source[0,0], self._axes_names[0]) )
-        x1=to_quantity( getattr(self.source[1,1], self._axes_names[0]) )
-        y0=to_quantity( getattr(self.source[0,0], self._axes_names[1]) )
-        y1=to_quantity( getattr(self.source[1,1], self._axes_names[1]) )
+        x0 = to_quantity(getattr(self.source[0, 0], self._axes_names[0]))
+        x1 = to_quantity(getattr(self.source[1, 1], self._axes_names[0]))
+        y0 = to_quantity(getattr(self.source[0, 0], self._axes_names[1]))
+        y1 = to_quantity(getattr(self.source[1, 1], self._axes_names[1]))
 
         # guaranteed by grid being RegularBaseGrid
-        assert x0.max()==x0.min()
-        assert x1.max()==x1.min()
-        assert y0.max()==y0.min()
-        assert y1.max()==y1.min()
-
-        x0=x0.min()
-        x1=x1.min()
-        y0=y0.min()
-        y1=y1.min()
-
-        dx=x1-x0
-        dy=y1-y0
-                
-        x=getattr(self.target, self._axes_names[0])
-        y=getattr(self.target, self._axes_names[1])
+        assert x0.max() == x0.min()
+        assert x1.max() == x1.min()
+        assert y0.max() == y0.min()
+        assert y1.max() == y1.min()
+
+        x0 = x0.min()
+        x1 = x1.min()
+        y0 = y0.min()
+        y1 = y1.min()
+
+        dx = x1 - x0
+        dy = y1 - y0
+
+        x = getattr(self.target, self._axes_names[0])
+        y = getattr(self.target, self._axes_names[1])
+
+        ix = numpy.floor((x - x0) / dx).astype(int)
+        iy = numpy.floor((y - y0) / dy).astype(int)
+
+        ix2 = ix + 1
+        iy2 = iy + 1
+
+        if self.x_periodic:
+            numpy.place(ix, ix == -1, self.source.shape[0] - 1)
+            numpy.place(ix, ix == self.source.shape[0], 0)
+            numpy.place(ix2, ix2 == self.source.shape[0], 0)
 
-        ix=numpy.floor((x-x0)/dx).astype(int)
-        iy=numpy.floor((y-y0)/dy).astype(int)
         if self.check_inside:
-          if numpy.any(ix<0) or numpy.any(ix>self.source.shape[0]-2) or \
-             numpy.any(iy<0) or numpy.any(iy>self.source.shape[1]-2):
-               raise Exception("target not fully inside (restricted) source grid as required")
-        ix=numpy.clip(ix,0, self.source.shape[0]-2)
-        iy=numpy.clip(iy,0, self.source.shape[1]-2)
-
-        wx=(x0+(ix+1)*dx-x)/dx
-        wy=(y0+(iy+1)*dy-y)/dy
-        wx=numpy.clip(wx,0.,1.)
-        wy=numpy.clip(wy,0.,1.)
-
-        self._weights=[wx,wy]
-
-        while(len(ix.shape)>2):
-          ix=numpy.amax(ix,axis=-1)
-          iy=numpy.amax(iy,axis=-1)
-          
-        self._indices=[ix,iy]
-      
+            if (
+                numpy.any(ix < 0)
+                or numpy.any(ix > self.source.shape[0] - 1)
+                or numpy.any(iy < 0)
+                or numpy.any(iy > self.source.shape[1] - 1)
+                or numpy.any(ix2 < 0)
+                or numpy.any(ix2 > self.source.shape[0] - 1)
+                or numpy.any(iy2 < 0)
+                or numpy.any(iy2 > self.source.shape[1] - 1)
+            ):
+                raise Exception(
+                    "target not fully inside (restricted) source grid as required"
+                )
+
+        if not self.x_periodic:
+            ix = numpy.clip(ix, 0, self.source.shape[0] - 1)
+            ix2 = numpy.clip(ix2, 0, self.source.shape[0] - 1)
+
+        iy = numpy.clip(iy, 0, self.source.shape[1] - 1)
+        iy2 = numpy.clip(iy2, 0, self.source.shape[1] - 1)
+
+        wx = (x0 + (ix + 1) * dx - x) / dx
+        wy = (y0 + (iy + 1) * dy - y) / dy
+        wx = numpy.clip(wx, 0.0, 1.0)
+        wy = numpy.clip(wy, 0.0, 1.0)
+
+        self._weights = [wx, wy]
+
+        while len(ix.shape) > 2:
+            ix = numpy.amax(ix, axis=-1)
+            iy = numpy.amax(iy, axis=-1)
+            ix2 = numpy.amax(ix2, axis=-1)
+            iy2 = numpy.amax(iy2, axis=-1)
+
+        self._indices = [ix, ix2, iy, iy2]
+
     def _evaluate(self, values):
-        ix,iy=self._indices
-        wx,wy=self._weights
-        result=wx*wy*values[ix,iy]+(1.-wx)*wy*values[ix+1,iy]+ \
-               wx*(1.-wy)*values[ix,iy+1]+(1.-wx)*(1.-wy)*values[ix+1,iy+1]
+        ix, ix2, iy, iy2 = self._indices
+        wx, wy = self._weights
+        result = (
+            wx * wy * values[ix, iy]
+            + (1.0 - wx) * wy * values[ix2, iy]
+            + wx * (1.0 - wy) * values[ix, iy2]
+            + (1.0 - wx) * (1.0 - wy) * values[ix2, iy2]
+        )
         return result
 
     def forward_mapping(self, attributes, target_names=None):
         if attributes is None:
-            attributes=self.source.get_attribute_names_defined_in_store()
+            attributes = self.source.get_attribute_names_defined_in_store()
         if target_names is None:
-            target_names=attributes
+            target_names = attributes
         if self._weights is None:
             self._calculate_weights()
-        
-        mapped_values=[]
+
+        mapped_values = []
         for attribute, target_name in zip(attributes, target_names):
-            values=getattr(self.source,attribute)
-            samples=self._evaluate(values)
+            values = getattr(self.source, attribute)
+            samples = self._evaluate(values)
             mapped_values.append(samples)
 
         self.target.set_values_in_store(None, target_names, mapped_values)
 
 
 class nearest_2D_remapper(object):
     def __init__(self, source, target, check_inside=True):
-        """ this class maps a source grid to a target grid getting closest
-        grid value. If check_inside=True, raise exception if any 
-            target point outside source grid. 
+        """this class maps a source grid to a target grid getting closest
+        grid value. If check_inside=True, raise exception if any
+            target point outside source grid.
         """
-        if len(source.shape) !=2:
+        if len(source.shape) != 2:
             raise Exception("source grid is not 2D")
         if not isinstance(source, RegularBaseGrid):
             raise Exception("source grid is not instance of RegularBaseGrid")
 
-        self.source=source
-        self.target=target
-        self._axes_names=source.get_axes_names()
-        self.check_inside=check_inside
-        self._indices=None
-
-    def _calculate_weights(self):        
-        x=getattr(self.target, self._axes_names[0])
-        y=getattr(self.target, self._axes_names[1])
+        self.source = source
+        self.target = target
+        self._axes_names = source.get_axes_names()
+        self.check_inside = check_inside
+        self._indices = None
 
-        kwargs={self._axes_names[0]: x, self._axes_names[1]:y}
-        indices=self.source.get_index(**kwargs)
+    def _calculate_weights(self):
+        x = getattr(self.target, self._axes_names[0])
+        y = getattr(self.target, self._axes_names[1])
+
+        kwargs = {self._axes_names[0]: x, self._axes_names[1]: y}
+        indices = self.source.get_index(**kwargs)
 
-        ix=indices[...,0]
-        iy=indices[...,1]
+        ix = indices[..., 0]
+        iy = indices[..., 1]
         if self.check_inside:
-          if numpy.any(ix<0) or numpy.any(ix>self.source.shape[0]-1) or \
-             numpy.any(iy<0) or numpy.any(iy>self.source.shape[1]-1):
-               raise Exception("target not fully inside source grid as required")
-        ix=numpy.clip(ix,0, self.source.shape[0]-1)
-        iy=numpy.clip(iy,0, self.source.shape[1]-1)
-        
-        self._indices=[ix,iy]
+            if (
+                numpy.any(ix < 0)
+                or numpy.any(ix > self.source.shape[0] - 1)
+                or numpy.any(iy < 0)
+                or numpy.any(iy > self.source.shape[1] - 1)
+            ):
+                raise Exception("target not fully inside source grid as required")
+        ix = numpy.clip(ix, 0, self.source.shape[0] - 1)
+        iy = numpy.clip(iy, 0, self.source.shape[1] - 1)
+
+        self._indices = [ix, iy]
 
     def _evaluate(self, values):
         return values[self._indices[0], self._indices[1]]
 
     def forward_mapping(self, attributes, target_names=None):
         if attributes is None:
-            attributes=self.source.get_attribute_names_defined_in_store()
+            attributes = self.source.get_attribute_names_defined_in_store()
         if target_names is None:
-            target_names=attributes
+            target_names = attributes
         if self._indices is None:
             self._calculate_weights()
 
-        mapped_values=[]
+        mapped_values = []
         for attribute, target_name in zip(attributes, target_names):
-            values=getattr(self.source,attribute)
-            samples=self._evaluate(values)
+            values = getattr(self.source, attribute)
+            samples = self._evaluate(values)
             mapped_values.append(samples)
 
         self.target.set_values_in_store(None, target_names, mapped_values)
 
 
-def conservative_spherical_remapper(*args,**kwargs):
+def conservative_spherical_remapper(*args, **kwargs):
     raise Exception("conservative_spherical_remapper has moved to omuse.ext")
```

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/grid_to_sph.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/grid_to_sph.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/halogen_model.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/halogen_model.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/hydro_collision.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/hydro_collision.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/job_server.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/job_server.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/molecular_cloud.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/molecular_cloud.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/orbital_elements.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/orbital_elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
-orbital element conversion and utility functions
+Orbital element conversion and utility functions
 
-this module provides:
+This module provides the following functions:
 
-generate_binaries
-orbital_elements
-get_orbital_elements_from_binary
-get_orbital_elements_from_binaries
-get_orbital_elements_from_arrays
+- generate_binaries
+- orbital_elements
+- get_orbital_elements_from_binary
+- get_orbital_elements_from_binaries
+- get_orbital_elements_from_arrays
 
-and the following deprecated functions (assume input
+And the following deprecated functions (which assume input
 or output angle floats to be degrees):
 
-new_binary_from_orbital_elements
-orbital_elements_from_binary
-orbital_elements_for_rel_posvel_arrays
+- new_binary_from_orbital_elements
+- orbital_elements_from_binary
+- orbital_elements_for_rel_posvel_arrays
 
 """
 
-import numpy
-
 import warnings
 
+import numpy
+
+from amuse.units.quantities import as_vector_quantity
 from amuse.units import units, constants, nbody_system
 from amuse.units.trigo import cos, sin, arccos, arctan2
 from amuse.datamodel import Particles, Particle
 
 from amuse.units.quantities import to_quantity, VectorQuantity
 
 def derive_G(unit_or_quantity):
@@ -336,14 +337,17 @@
         ):
     """
     returns a two-particle Particle set, with the second particle's position
     and velocities computed from the input orbital elements.
     inclination is given between 0 and 180 deg.
     angles are assumed to be in deg if no unit is given.
     """
+    warnings.warn(
+        "new_binary_from_orbital_elements is deprecated, use generate_binaries instead"
+    )
     def angle_with_unit(angle, default_unit=units.deg):
         try:
             default_unit = angle.unit
         except:
             angle = angle | default_unit
         return angle
 
@@ -370,15 +374,15 @@
 
     result = Particles()
     result.add_particle(primary[0])
     result.add_particle(secondary[0])
     return result
 
 
-def get_orbital_elements_from_binary(binary, G=None):
+def get_orbital_elements_from_binary(binary, G=None, return_dict=False):
     """
     Function that computes orbital elements from given two-particle set.
     Elements are computed for the second particle in this set and the
     return values are: mass1, mass2, semimajor axis, eccentricity,
     cosine of true anomaly, cosine of inclination, cosine of the
     longitude of the ascending node and the cosine of the argument of
     pericenter. In case of a perfectly circular orbit the true anomaly
@@ -400,37 +404,52 @@
         primaries[0].velocity *= 0
         secondaries.add_particle(Particle())
         secondaries[0].mass = 0 * primaries[0].mass
         secondaries[0].position = binary.position
         secondaries[0].velocity = binary.velocity
 
     (
-            mass1, mass2, semimajor_axis, eccentricity, true_anomaly,
-            inclination, long_asc_node, arg_per
-            ) = get_orbital_elements_from_binaries(primaries, secondaries, G=G)
+        mass1, mass2, semimajor_axis, eccentricity, true_anomaly,
+        inclination, long_asc_node, arg_per
+    ) = get_orbital_elements_from_binaries(primaries, secondaries, G=G)
+    if return_dict:
+        return {
+            "mass_primary": mass1[0],
+            "mass_secondary": mass2[0],
+            "semi_major_axis": semimajor_axis[0],
+            "eccentricity": eccentricity[0],
+            "true_anomaly": true_anomaly[0],
+            "inclination": inclination[0],
+            "longitude_of_the_ascending_node": long_asc_node[0],
+            "argument_of_periapsis": arg_per[0],
+        }
     return (
             mass1[0], mass2[0], semimajor_axis[0], eccentricity[0],
             true_anomaly[0], inclination[0], long_asc_node[0], arg_per[0])
 
 
 def orbital_elements_from_binary(binary, G=None):
     (
-            mass1, mass2, semimajor_axis, eccentricity, true_anomaly,
-            inclination, long_asc_node, arg_per
-            ) = get_orbital_elements_from_binary(binary, G=G)
+        mass1, mass2, semimajor_axis, eccentricity, true_anomaly,
+        inclination, long_asc_node, arg_per
+    ) = get_orbital_elements_from_binary(binary, G=G)
+    warnings.warn(
+        "orbital_elements_from_binary is deprecated, use orbital_elements instead"
+    )
     return (
             mass1, mass2, semimajor_axis, eccentricity,
             true_anomaly.value_in(units.deg),
             inclination.value_in(units.deg),
             long_asc_node.value_in(units.deg),
             arg_per.value_in(units.deg))
 
 
 def get_orbital_elements_from_binaries(
-        primaries, secondaries, G=None):
+    primaries, secondaries, G=None, return_dict=False
+):
     """
     Function that computes orbital elements from given primaries and
     secondaries.
     Elements are computed for the second particle in this set and the
     return values are: mass1, mass2, semimajor axis, eccentricity,
     cosine of true anomaly, cosine of inclination, cosine of the
     longitude of the ascending node and the cosine of the argument of
@@ -443,23 +462,33 @@
     velocity = secondaries.velocity - primaries.velocity
     mass1 = primaries.mass
     mass2 = secondaries.mass
     total_mass = mass1 + mass2
     semimajor_axis, eccentricity, true_anomaly, inclination, long_asc_node, \
         arg_per = get_orbital_elements_from_arrays(
             position, velocity, total_mass, G=G)
-
+    if return_dict:
+        return {
+            "mass_primary": mass1,
+            "mass_secondary": mass2,
+            "semi_major_axis": semimajor_axis,
+            "eccentricity": eccentricity,
+            "true_anomaly": true_anomaly,
+            "inclination": inclination,
+            "longitude_of_the_ascending_node": long_asc_node,
+            "argument_of_periapsis": arg_per,
+        }
     return (
             mass1, mass2, semimajor_axis, eccentricity, true_anomaly,
             inclination, long_asc_node, arg_per)
 
 
 def get_orbital_elements_from_arrays(
-        rel_position_raw, rel_velocity_raw,
-        total_masses, G=None):
+    rel_position_raw, rel_velocity_raw, total_masses, G=None, return_dict=False
+):
     """
     Orbital elements from array of relative positions and velocities vectors,
     based on orbital_elements_from_binary and adapted to work for arrays (each
     line characterises a two body problem).
 
     For circular orbits (eccentricity=0): returns argument of pericenter = 0.,
         true anomaly = 0.
@@ -490,17 +519,19 @@
         rel_velocity = numpy.zeros([1, 3]) * rel_velocity_raw[0]
         rel_velocity[0, 0] = rel_velocity_raw[0]
         rel_velocity[0, 1] = rel_velocity_raw[1]
         rel_velocity[0, 2] = rel_velocity_raw[2]
     else:
         rel_position = rel_position_raw
         rel_velocity = rel_velocity_raw
+    rel_position = as_vector_quantity(rel_position)
+    rel_velocity = as_vector_quantity(rel_velocity)
 
     if G is None:
-        G=derive_G(total_masses[0])
+        G = derive_G(total_masses[0])
 
     separation = (rel_position**2).sum(axis=1)**0.5
     n_vec = len(rel_position)
 
     speed_squared = (rel_velocity**2).sum(axis=1)
 
     semimajor_axis = (
@@ -612,57 +643,70 @@
     # true anomaly
     cos_true_anomaly = (e_vecs_unit*pos_unit_vecs).sum(axis=-1)
     e_cross_pos = numpy.cross(e_vecs_unit, pos_unit_vecs)
     ss2 = numpy.sign((mom_unit_vecs*e_cross_pos).sum(axis=-1))
     sin_true_anomaly = ss2*(e_cross_pos**2).sum(axis=1)**0.5
     true_anomaly = arctan2(sin_true_anomaly, cos_true_anomaly)
 
+    if return_dict:
+        return {
+            "semi_major_axis": semimajor_axis,
+            "eccentricity": eccentricity,
+            "true_anomaly": true_anomaly,
+            "inclination": inc,
+            "longitude_of_the_ascending_node": long_asc_node,
+            "argument_of_periapsis": arg_per_mat,
+        }
     return (
-            semimajor_axis, eccentricity, true_anomaly,
-            inc, long_asc_node, arg_per_mat
-            )
+        semimajor_axis, eccentricity, true_anomaly,
+        inc, long_asc_node, arg_per_mat
+    )
 
 
 def orbital_elements(*args, **kwargs):
     try:
         if len(args) == 1:
             return get_orbital_elements_from_binary(*args, **kwargs)
         elif len(args) == 2:
             return get_orbital_elements_from_binaries(*args, **kwargs)
         elif len(args) == 3:
             return get_orbital_elements_from_arrays(*args, **kwargs)
         else:
             raise Exception
     except Exception as ex:
-        if not ex.args: 
-            ex.args=()
+        if not ex.args:
+            ex.args = ()
         ex.args = ex.args + ("""
-  note: orbital elements takes as input either:
+  note: orbital_elements takes as input either:
   - single two particle set,
   - two sets of primaries and secondaries
   - arrays of rel. position, rel. velocity and masses
   """,)
         raise
 
 def orbital_elements_for_rel_posvel_arrays(
-        rel_position_raw, rel_velocity_raw,
-        total_masses, G=None):
+    rel_position_raw, rel_velocity_raw, total_masses, G=None
+):
+    warnings.warn(
+        "orbital_elements_for_rel_posvel_arrays is deprecated, "
+        "use orbital_elements instead"
+    )
     (semimajor_axis, eccentricity, true_anomaly, inc, long_asc_node,
         arg_per_mat) = get_orbital_elements_from_arrays(
                 rel_position_raw, rel_velocity_raw, total_masses, G)
 
     true_anomaly = true_anomaly.value_in(units.deg)
     inc = inc.value_in(units.deg)
     long_asc_node = long_asc_node.value_in(units.deg)
     arg_per_mat = arg_per_mat.value_in(units.deg)
 
     return (
-            semimajor_axis, eccentricity, true_anomaly,
-            inc, long_asc_node, arg_per_mat
-            )
+        semimajor_axis, eccentricity, true_anomaly, inc, long_asc_node,
+        arg_per_mat
+    )
 
 
 def normalize_vector(vecs, norm, one_dim=False):
     """
     normalize array of vector quantities
     """
     if one_dim:
```

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/particles_with_color.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/particles_with_color.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/plotting_hydro.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/plotting_hydro.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/plummer_helper.pyx` & `amuse_framework-2024.4.0rc1/src/amuse/ext/plummer_helper.pyx`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/polarsupport.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/polarsupport.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/protodisk.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/protodisk.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/radial_profile.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/radial_profile.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/relax_sph.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/relax_sph.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/roche_radius.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/roche_radius.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/rotating_bridge.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/rotating_bridge.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/sink.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/sink.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/sobol.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/sobol.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/solarsystem.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/solarsystem.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/speed.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/speed.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/sph_to_grid.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/sph_to_grid.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/sph_to_star.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/sph_to_star.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/spherical_model.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/spherical_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,254 +1,311 @@
+"""
+Classes to generate a uniform spherical grid of particles, which can be used
+for other initial distribution functions.
+"""
+
 import numpy
 
-from amuse.support.exceptions import AmuseException, AmuseWarning
+from amuse.support.exceptions import AmuseException
 from amuse.units import units, nbody_system, generic_unit_system, constants
 from amuse.datamodel import Particles
 from amuse.ext.sobol import i4_sobol_generate
 
-class EnclosedMassInterpolator(object):
+
+class EnclosedMassInterpolator:
     """
-    Interpolator used in 'get_enclosed_mass_from_tabulated' and 'get_radius_for_enclosed_mass'.
-    These two functions are required for 'new_spherical_particle_distribution'.
+    Interpolator used in 'get_enclosed_mass_from_tabulated' and
+    'get_radius_for_enclosed_mass'. These two functions are required for
+    'new_spherical_particle_distribution'.
     """
-    def __init__(self, radii = None, densities = None, core_radius = None):
+
+    def __init__(self, radii=None, densities=None, core_radius=None):
         self.initialized = False
-        self.four_thirds_pi = numpy.pi * 4.0/3.0
-        if (radii and densities):
-            self.initialize(radii, densities, core_radius = core_radius)
-    
-    def initialize(self, radii, densities, core_radius = None):
-        self.sort_density_and_radius(densities*1.0, radii*1.0, core_radius = core_radius)
+        self.four_thirds_pi = numpy.pi * 4.0 / 3.0
+        if radii and densities:
+            self.initialize(radii, densities, core_radius=core_radius)
+
+    def initialize(self, radii, densities, core_radius=None):
+        self.sort_density_and_radius(
+            densities * 1.0, radii * 1.0, core_radius=core_radius
+        )
         self.calculate_enclosed_mass_table()
         self.initialized = True
-    
-    def sort_density_and_radius(self, densities, radii, core_radius = None):
+
+    def sort_density_and_radius(self, densities, radii, core_radius=None):
         self.radii, self.densities = radii.sorted_with(densities)
         self.radii.prepend(core_radius or 0 | units.m)
-    
+
     def calculate_enclosed_mass_table(self):
         self.radii_cubed = self.radii**3
         self.enclosed_mass = [0.0] | units.kg
-        for rho_shell, r3_in, r3_out in zip(self.densities, self.radii_cubed, self.radii_cubed[1:]):
-            self.enclosed_mass.append(self.enclosed_mass[-1] + rho_shell * (r3_out - r3_in))
+        for rho_shell, r3_in, r3_out in zip(
+            self.densities, self.radii_cubed, self.radii_cubed[1:]
+        ):
+            self.enclosed_mass.append(
+                self.enclosed_mass[-1] + rho_shell * (r3_out - r3_in)
+            )
         self.enclosed_mass = self.four_thirds_pi * self.enclosed_mass
-    
+
     def get_index(self, value, sorted_vector):
-        out_of_bounds = numpy.logical_or(sorted_vector[0] > value, value > sorted_vector[-1])
+        out_of_bounds = numpy.logical_or(
+            sorted_vector[0] > value, value > sorted_vector[-1]
+        )
         if out_of_bounds.any():
-            value = numpy.compress(numpy.array([out_of_bounds]).flatten(), value.number) | value.unit
-            raise AmuseException("Can't find a valid index. {0} is not in "
-                "the range [{1}, {2}].".format(value, sorted_vector[0], sorted_vector[-1]))
-        index = numpy.searchsorted(sorted_vector.number, value.value_in(sorted_vector.unit))
+            value = (
+                numpy.compress(numpy.array([out_of_bounds]).flatten(), value.number)
+                | value.unit
+            )
+            raise AmuseException(
+                "Can't find a valid index. {0} is not in "
+                "the range [{1}, {2}].".format(
+                    value, sorted_vector[0], sorted_vector[-1]
+                )
+            )
+        index = numpy.searchsorted(
+            sorted_vector.number, value.value_in(sorted_vector.unit)
+        )
         return numpy.maximum(index - 1, 0)
-    
+
     def get_enclosed_mass(self, radius):
         if not self.initialized:
-            raise AmuseException("Can't calculate enclosed mass: interpolator is not initialized")
+            raise AmuseException(
+                "Can't calculate enclosed mass: interpolator is not initialized"
+            )
         index = self.get_index(radius, self.radii)
-        return (self.enclosed_mass[index] + self.four_thirds_pi * 
-            self.densities[index] * (radius**3 - self.radii_cubed[index]))
-    
+        return self.enclosed_mass[index] + self.four_thirds_pi * self.densities[
+            index
+        ] * (radius**3 - self.radii_cubed[index])
+
     def get_radius_for_enclosed_mass(self, enclosed_mass):
         if not self.initialized:
-            raise AmuseException("Can't calculate radius for enclosed mass: interpolator is not initialized")
+            raise AmuseException(
+                "Can't calculate radius for enclosed mass: interpolator is not "
+                "initialized"
+            )
         index = self.get_index(enclosed_mass, self.enclosed_mass)
-        return (((enclosed_mass - self.enclosed_mass[index]) / (self.four_thirds_pi * self.densities[index]) 
-            + self.radii_cubed[index]))**(1.0/3.0)
-    
+        return (
+            (
+                (enclosed_mass - self.enclosed_mass[index])
+                / (self.four_thirds_pi * self.densities[index])
+                + self.radii_cubed[index]
+            )
+        ) ** (1.0 / 3.0)
 
 
-class UniformSphericalDistribution(object):
+class UniformSphericalDistribution:
     """
     Creates a uniform spherical grid of particles. Type can be:
     "cubic":  'crystal' composed of cubes with particles on each corner
     "bcc":    as cubic but with additional particles at the center of each cube
     "body_centered_cubic": same as "bcc"
     "fcc":    as cubic but with additional particles at the face of each cube
     "face_centered_cubic": same as "fcc"
     "random": particles are randomly distributed using numpy.random.uniform
     "glass":  like random, but stabilised using hydro pressure and no gravity
     "sobol":  3D sobol sequence (low discrepancy, quasi-random)
-    
-    "offset" is only used for the regular grids ("cubic", "bcc", "fcc"), and 
-    should contain three numbers in the half-open interval [0, 1). These 
-    define the offset between the origin of the grid and the corner 
+
+    "offset" is only used for the regular grids ("cubic", "bcc", "fcc"), and
+    should contain three numbers in the half-open interval [0, 1). These
+    define the offset between the origin of the grid and the corner
     of the unit cell, normalized to the unit cell size.
     "target_rms" is only used for "glass" as the density criterion for convergence
     """
-    def __init__(self, number_of_particles, type = "bcc", 
-            offset = (0.82832951,  0.27237167,  0.37096327), 
-            mass_cutoff = 1, target_rms = 0.01):
+
+    def __init__(
+        self,
+        number_of_particles,
+        type="bcc",
+        offset=(0.82832951, 0.27237167, 0.37096327),
+        mass_cutoff=1,
+        target_rms=0.01,
+    ):
         if not hasattr(self, type):
             raise TypeError("Unknown grid type option: {0}".format(type))
         self.number_of_particles = number_of_particles
         self.type = type
         self.offset = offset
         self.mass_cutoff = mass_cutoff
         self.target_rms = target_rms
-    
+
     def cubic(self):
-        n1D = numpy.ceil( 0.5*(2*self.number_of_particles)**(1./3) ) * 2 + 3 # odd number
-        x, y, z = numpy.mgrid[-1. : 1. : n1D*1j,
-                              -1. : 1. : n1D*1j,
-                              -1. : 1. : n1D*1j]
+        n1D = (
+            numpy.ceil(0.5 * (2 * self.number_of_particles) ** (1.0 / 3)) * 2 + 3
+        )  # odd number
+        x, y, z = numpy.mgrid[
+            -1.0: 1.0: n1D * 1j,
+            -1.0: 1.0: n1D * 1j,
+            -1.0: 1.0: n1D * 1j
+        ]
         x = x.flatten()
         y = y.flatten()
         z = z.flatten()
-        for delta, vec in zip(self.offset, (x,y,z)):
+        for delta, vec in zip(self.offset, (x, y, z)):
             vec += delta * 2.0 / (n1D - 1)
         return self._cutout_sphere(x, y, z)
-    
+
     def bcc(self):
-        n1D = numpy.ceil( 0.5*(self.number_of_particles)**(1./3) ) * 2 + 3 # odd number
-        x1,y1,z1 = numpy.mgrid[-1. : 1. : n1D*1j,
-                               -1. : 1. : n1D*1j,
-                               -1. : 1. : n1D*1j]
+        n1D = (
+            numpy.ceil(0.5 * (self.number_of_particles) ** (1.0 / 3)) * 2 + 3
+        )  # odd number
+        x1, y1, z1 = numpy.mgrid[
+            -1.0: 1.0: n1D * 1j,
+            -1.0: 1.0: n1D * 1j,
+            -1.0: 1.0: n1D * 1j
+        ]
         n_2 = n1D - 1
-        x2,y2,z2 = numpy.mgrid[-1.+1./n_2 : 1.-1./n_2 : n_2*1j,
-                               -1.+1./n_2 : 1.-1./n_2 : n_2*1j,
-                               -1.+1./n_2 : 1.-1./n_2 : n_2*1j]
-        x = numpy.concatenate( (x1.flatten(),x2.flatten()) )
-        y = numpy.concatenate( (y1.flatten(),y2.flatten()) )
-        z = numpy.concatenate( (z1.flatten(),z2.flatten()) )
-        for delta, vec in zip(self.offset, (x,y,z)):
+        x2, y2, z2 = numpy.mgrid[
+            -1.0 + 1.0 / n_2: 1.0 - 1.0 / n_2: n_2 * 1j,
+            -1.0 + 1.0 / n_2: 1.0 - 1.0 / n_2: n_2 * 1j,
+            -1.0 + 1.0 / n_2: 1.0 - 1.0 / n_2: n_2 * 1j,
+        ]
+        x = numpy.concatenate((x1.flatten(), x2.flatten()))
+        y = numpy.concatenate((y1.flatten(), y2.flatten()))
+        z = numpy.concatenate((z1.flatten(), z2.flatten()))
+        for delta, vec in zip(self.offset, (x, y, z)):
             vec += delta * 2.0 / n_2
         return self._cutout_sphere(x, y, z)
-    
+
     body_centered_cubic = bcc
-    
+
     def fcc(self):
-        n1D = numpy.ceil((self.number_of_particles / 2.0)**(1.0/3.0)) + 1
+        n1D = numpy.ceil((self.number_of_particles / 2.0) ** (1.0 / 3.0)) + 1
         delta = 1.0 / (n1D - 1.5)
-        x, y, z = numpy.mgrid[-1.0-2*delta : 1-delta : n1D*1j,
-                              -1.0-2*delta : 1-delta : n1D*1j,
-                              -1.0-2*delta : 1-delta : n1D*1j]
+        x, y, z = numpy.mgrid[
+            -1.0 - 2 * delta: 1 - delta: n1D * 1j,
+            -1.0 - 2 * delta: 1 - delta: n1D * 1j,
+            -1.0 - 2 * delta: 1 - delta: n1D * 1j,
+        ]
         x0 = x.flatten() + self.offset[0] * 2 * delta
         y0 = y.flatten() + self.offset[1] * 2 * delta
         z0 = z.flatten() + self.offset[2] * 2 * delta
         x1 = x0 + delta
         y1 = y0 + delta
         z1 = z0 + delta
         x = numpy.concatenate((x0, x1, x0, x1))
         y = numpy.concatenate((y0, y1, y1, y0))
         z = numpy.concatenate((z0, z0, z1, z1))
         return self._cutout_sphere(x, y, z)
-    
+
     face_centered_cubic = fcc
-    
+
     def _random_cube(self, number_of_particles):
         x = numpy.random.uniform(-1.0, 1.0, number_of_particles)
         y = numpy.random.uniform(-1.0, 1.0, number_of_particles)
         z = numpy.random.uniform(-1.0, 1.0, number_of_particles)
         return x, y, z
-    
-    def random(self, number_of_particles = None, try_number_of_particles = None):
+
+    def random(self, number_of_particles=None, try_number_of_particles=None):
         if number_of_particles is None:
             number_of_particles = self.number_of_particles
         if try_number_of_particles is None:
             try_number_of_particles = number_of_particles
         try_number_of_particles = int(try_number_of_particles)
-        x, y, z = self._random_cube(2*try_number_of_particles)
-        r_squared = x*x + y*y + z*z
-        select_sphere = numpy.where( r_squared < self.mass_cutoff**(2.0/3.0))
+        x, y, z = self._random_cube(2 * try_number_of_particles)
+        r_squared = x * x + y * y + z * z
+        select_sphere = numpy.where(r_squared < self.mass_cutoff ** (2.0 / 3.0))
         if len(select_sphere[0]) < number_of_particles:
-            return self.random(number_of_particles, numpy.ceil(try_number_of_particles*1.1) )
+            return self.random(
+                number_of_particles, numpy.ceil(try_number_of_particles * 1.1)
+            )
         else:
-            return (x[select_sphere][0:number_of_particles], 
-                y[select_sphere][0:number_of_particles], 
-                z[select_sphere][0:number_of_particles])
-    
+            return (
+                x[select_sphere][0:number_of_particles],
+                y[select_sphere][0:number_of_particles],
+                z[select_sphere][0:number_of_particles],
+            )
 
     def sobol(self):
-        x, y, z = i4_sobol_generate(3, 2*self.number_of_particles, 3) * 2.0 - 1.0
+        x, y, z = i4_sobol_generate(3, 2 * self.number_of_particles, 3) * 2.0 - 1.0
         return self._cutout_sphere(x, y, z)
-    
+
     def glass(self):
         from amuse.community.fi.interface import Fi
-        
+
         if self.target_rms < 0.0001:
             print("warning: target_rms may not succeed")
         if self.number_of_particles < 1000:
             print("warning: not enough particles")
-        
+
         N = 2 * self.number_of_particles
         L = 1 | nbody_system.length
         dt = 0.01 | nbody_system.time
-        
+
         x, y, z = self._random_cube(N)
-        vx,vy,vz= self.random(N)
-        
+        vx, vy, vz = self.random(N)
+
         p = Particles(N)
         p.x = L * x
         p.y = L * y
         p.z = L * z
         p.h_smooth = 0.0 | nbody_system.length
         p.vx = (0.1 | nbody_system.speed) * vx[:N]
         p.vy = (0.1 | nbody_system.speed) * vy[:N]
         p.vz = (0.1 | nbody_system.speed) * vz[:N]
-        p.u = (0.1*0.1) | nbody_system.speed**2
-        p.mass = (8.0/N) | nbody_system.mass
-        
-        sph = Fi(mode = 'periodic', redirection = 'none')
+        p.u = (0.1 * 0.1) | nbody_system.speed**2
+        p.mass = (8.0 / N) | nbody_system.mass
+
+        sph = Fi(mode="periodic", redirection="none")
         sph.initialize_code()
-        
+
         sph.parameters.use_hydro_flag = True
         sph.parameters.radiation_flag = False
         sph.parameters.self_gravity_flag = False
         sph.parameters.gamma = 1.0
         sph.parameters.isothermal_flag = True
         sph.parameters.integrate_entropy_flag = False
         sph.parameters.timestep = dt
         sph.parameters.verbosity = 0
         sph.parameters.periodic_box_size = 2 * L
         sph.parameters.artificial_viscosity_alpha = 1.0
         sph.parameters.beta = 2.0
         sph.commit_parameters()
         sph.gas_particles.add_particles(p)
         sph.commit_particles()
-        
+
         t = 0.0 | nbody_system.time
         rms = 1.0
         minrms = 1.0
         i = 0
         while rms > self.target_rms:
             i += 1
-            t += (0.25 | nbody_system.time)
+            t += 0.25 | nbody_system.time
             sph.evolve_model(t)
             rho = sph.particles.rho.value_in(nbody_system.density)
-            rms = rho.std()/rho.mean()
+            rms = rho.std() / rho.mean()
             minrms = min(minrms, rms)
-            if (rms > 2.0*minrms) or (i > 300):
+            if (rms > 2.0 * minrms) or (i > 300):
                 print(" RMS(rho) convergence warning:", i, rms, minrms)
             if i > 100000:
                 print("i> 100k steps - not sure about this...")
                 print(" rms:", rms)
                 break
-        
+
         x = sph.particles.x.value_in(nbody_system.length)
         y = sph.particles.y.value_in(nbody_system.length)
         z = sph.particles.z.value_in(nbody_system.length)
         sph.stop()
         del sph
         return self._cutout_sphere(x, y, z)
-    
 
     def _cutout_sphere(self, x, y, z):
-        r_squared = x*x + y*y + z*z
+        r_squared = x * x + y * y + z * z
         sorted_indices = numpy.argsort(r_squared)
-        massfrac_edge = r_squared[sorted_indices[self.number_of_particles-1]]**(1.5)
-        massfrac_next = r_squared[sorted_indices[self.number_of_particles]]**(1.5)
-        r_max = (0.5*(massfrac_edge+massfrac_next) / self.mass_cutoff)**(1.0/3.0)
-        indices = sorted_indices[:self.number_of_particles]
-        return x[indices]/r_max, y[indices]/r_max, z[indices]/r_max
-    
+        massfrac_edge = r_squared[sorted_indices[self.number_of_particles - 1]] ** (1.5)
+        massfrac_next = r_squared[sorted_indices[self.number_of_particles]] ** (1.5)
+        r_max = (0.5 * (massfrac_edge + massfrac_next) / self.mass_cutoff) ** (
+            1.0 / 3.0
+        )
+        indices = sorted_indices[: self.number_of_particles]
+        return x[indices] / r_max, y[indices] / r_max, z[indices] / r_max
+
     @property
     def result(self):
         return getattr(self, self.type)()
-    
+
 
 keyword_arguments_doc = """    :argument keyword_arguments:    Optional arguments to UniformSphericalDistribution:
         :argument type:             Type of the basegrid. Can be:
             "cubic":  'crystal' composed of cubes with particles on each corner
             "bcc":    as cubic but with additional particles at the center of each cube
             "body_centered_cubic": same as "bcc"
             "fcc":    as cubic but with additional particles at the face of each cube
@@ -259,172 +316,253 @@
         :argument offset:           only used for the regular grids ("cubic", "bcc", "fcc"), and 
             should contain three numbers in the half-open interval [0, 1). These 
             define the offset between the origin of the grid and the corner 
             of the unit cell, normalized to the unit cell size.
         :argument target_rms        only used for "glass" as the density criterion for convergence
 """
 
-def new_uniform_spherical_particle_distribution(number_of_particles, size, total_mass, **keyword_arguments):
+
+def new_uniform_spherical_particle_distribution(
+    number_of_particles, size, total_mass, **keyword_arguments
+):
     """
-    Returns a Particles set with positions following a uniform 
-    spherical distribution. Only the positions and masses 
+    Returns a Particles set with positions following a uniform
+    spherical distribution. Only the positions and masses
     (equal-mass system) are set.
-    
+
     :argument number_of_particles:  Number of particles in the resulting model
     :argument size:                 Radius of the sphere enclosing the model
     :argument total_mass:           Total mass of the Particles set
     """
     particles = Particles(number_of_particles)
     particles.mass = total_mass * 1.0 / number_of_particles
-    x, y, z = UniformSphericalDistribution(number_of_particles, **keyword_arguments).result
+    x, y, z = UniformSphericalDistribution(
+        number_of_particles, **keyword_arguments
+    ).result
     particles.x = size * x
     particles.y = size * y
     particles.z = size * z
     return particles
+
+
 new_uniform_spherical_particle_distribution.__doc__ += keyword_arguments_doc
 
-def new_spherical_particle_distribution(number_of_particles, 
-        radial_density_func = None,     # not yet supported, specify radii and densities tables:
-        radii = None, densities = None, 
-        total_mass = None, size = None, # if total_mass is not given, it will be deduced from size or max(radii)
-        **keyword_arguments):           # optional arguments for UniformSphericalDistribution
-    """
-    Returns a Particles set with positions following a spherical 
-    distribution. The radial density profile is determined from the 
-    look-up table (radii, densities). Entries in the 'radii' table 
-    are interpreted as the outer radius of the shell, with uniform 
-    density as defined by the corresponding entry in the 'densities' 
+
+def new_spherical_particle_distribution(
+    number_of_particles,
+    radial_density_func=None,  # not yet supported, specify radii and densities tables:
+    radii=None,
+    densities=None,
+    total_mass=None,
+    size=None,  # if total_mass is not given, it will be deduced from size or max(radii)
+    **keyword_arguments
+):  # optional arguments for UniformSphericalDistribution
+    """
+    Returns a Particles set with positions following a spherical
+    distribution. The radial density profile is determined from the
+    look-up table (radii, densities). Entries in the 'radii' table
+    are interpreted as the outer radius of the shell, with uniform
+    density as defined by the corresponding entry in the 'densities'
     table:
     rho(r) = densities[i],  for ( radii[i-1] <= r <= radii[i] )
-    
+
     Only the positions and masses (equal-mass system) are set.
-    
+
     :argument number_of_particles:  Number of particles in the resulting model
     :argument radii:                Table with radii for the radial density profile
     :argument densities:            Table with densities for the radial density profile
-    :argument total_mass:           Total mass of the Particles set (optional, will be 
+    :argument total_mass:           Total mass of the Particles set (optional, will be
                                     deduced from size or max(radii) otherwise)
     :argument size:                 Radius of the sphere enclosing the model (optional)
     """
     if (radii is None) or (densities is None):
-        raise AmuseException("Using an arbitrary radial density function is not yet "
-            "supported. Radius and density tables must be passed instead.")
-    
+        raise AmuseException(
+            "Using an arbitrary radial density function is not yet "
+            "supported. Radius and density tables must be passed instead."
+        )
+
     interpolator = EnclosedMassInterpolator()
     interpolator.initialize(radii, densities)
     if total_mass is None:
         total_mass = interpolator.get_enclosed_mass(size or max(radii))
     particles = Particles(number_of_particles)
     particle_mass = total_mass * 1.0 / number_of_particles
     particles.mass = particle_mass
-    x, y, z = UniformSphericalDistribution(number_of_particles, **keyword_arguments).result
-    # Now scale the uniformly distributed particle positions to match the radial density profile
-    r_old = numpy.sqrt(x*x + y*y + z*z)
+    x, y, z = UniformSphericalDistribution(
+        number_of_particles, **keyword_arguments
+    ).result
+    # Now scale the uniformly distributed particle positions to match the
+    # radial density profile
+    r_old = numpy.sqrt(x * x + y * y + z * z)
     indices = numpy.argsort(r_old)
     if r_old[indices[0]] == 0.0:
         r_old[indices[0]] = 1.0
-    f_scale = interpolator.get_radius_for_enclosed_mass(
-        (numpy.arange(0.5, number_of_particles + 0.5) | units.none) * particle_mass) / r_old[indices]
+    f_scale = (
+        interpolator.get_radius_for_enclosed_mass(
+            (numpy.arange(0.5, number_of_particles + 0.5) | units.none) * particle_mass
+        )
+        / r_old[indices]
+    )
     particles.x = (f_scale * x[indices]).as_quantity_in(radii.unit)
     particles.y = (f_scale * y[indices]).as_quantity_in(radii.unit)
     particles.z = (f_scale * z[indices]).as_quantity_in(radii.unit)
     return particles
+
+
 new_spherical_particle_distribution.__doc__ += keyword_arguments_doc
 
-plummer_arguments_doc = """
+plummer_arguments_doc = (
+    """
     :argument number_of_particles:  Number of particles in the resulting model
-    :argument total_mass:           Total mass of the Particles set 
+    :argument total_mass:           Total mass of the Particles set
     :argument virial_radius:        Virial radius of the Plummer model
-""" + keyword_arguments_doc
+"""
+    + keyword_arguments_doc
+)
 
-def new_plummer_spatial_distribution(number_of_particles, 
-        total_mass = 1.0|nbody_system.mass, 
-        virial_radius = 1.0|nbody_system.length,
-        mass_cutoff = 0.999,
-        **keyword_arguments):           # optional arguments for UniformSphericalDistribution
+
+def new_plummer_spatial_distribution(
+    number_of_particles,
+    total_mass=1.0 | nbody_system.mass,
+    virial_radius=1.0 | nbody_system.length,
+    mass_cutoff=0.999,
+    **keyword_arguments
+):  # optional arguments for UniformSphericalDistribution
     """
-    Returns a Particles set with positions following a Plummer 
-    distribution. 
+    Returns a Particles set with positions following a Plummer
+    distribution.
     Only the positions and masses (equal-mass system) are set.
     """
     particles = Particles(number_of_particles)
     particle_mass = total_mass * 1.0 / number_of_particles
     particles.mass = particle_mass
     x, y, z = UniformSphericalDistribution(
-        number_of_particles, mass_cutoff=mass_cutoff, **keyword_arguments).result
-    
-    # Now scale the uniformly distributed particle positions to match the radial density profile
-    r_old = numpy.sqrt(x*x + y*y + z*z)
-    scale_factor = (0.1875 * numpy.pi * virial_radius.number) / numpy.sqrt(1.0 - r_old**2)
+        number_of_particles, mass_cutoff=mass_cutoff, **keyword_arguments
+    ).result
+
+    # Now scale the uniformly distributed particle positions to match the
+    # radial density profile
+    r_old = numpy.sqrt(x * x + y * y + z * z)
+    scale_factor = (0.1875 * numpy.pi * virial_radius.number) / numpy.sqrt(
+        1.0 - r_old**2
+    )
     particles.x = scale_factor * x | virial_radius.unit
     particles.y = scale_factor * y | virial_radius.unit
     particles.z = scale_factor * z | virial_radius.unit
     return particles
+
+
 new_plummer_spatial_distribution.__doc__ += plummer_arguments_doc
 
-def new_gas_plummer_distribution(number_of_particles, 
-        total_mass = 1.0|nbody_system.mass, 
-        virial_radius = 1.0|nbody_system.length,
-        G = None,
-        **keyword_arguments):           # optional arguments for UniformSphericalDistribution
-    """
-    Create a plummer gas model with the given number of particles. Returns a set 
-    of SPH particles with equal masses and positions distributed to fit a plummer 
-    distribution model. Velocities are set to zero, and internal energies are set 
+
+def new_gas_plummer_distribution(
+    number_of_particles,
+    total_mass=1.0 | nbody_system.mass,
+    virial_radius=1.0 | nbody_system.length,
+    G=None,
+    **keyword_arguments
+):  # optional arguments for UniformSphericalDistribution
+    """
+    Create a plummer gas model with the given number of particles. Returns a set
+    of SPH particles with equal masses and positions distributed to fit a plummer
+    distribution model. Velocities are set to zero, and internal energies are set
     to balance the gravitational forces between the gas particles.
     """
-    particles = new_plummer_spatial_distribution(number_of_particles, total_mass=total_mass, 
-        virial_radius=virial_radius, **keyword_arguments)
-    
+    particles = new_plummer_spatial_distribution(
+        number_of_particles,
+        total_mass=total_mass,
+        virial_radius=virial_radius,
+        **keyword_arguments
+    )
+
     if G is None:
-        G = nbody_system.G if generic_unit_system.is_generic_unit(total_mass.unit) else constants.G
-    velocity_unit = (G*total_mass/virial_radius).sqrt().unit.base_unit()
+        G = (
+            nbody_system.G
+            if generic_unit_system.is_generic_unit(total_mass.unit)
+            else constants.G
+        )
+    velocity_unit = (G * total_mass / virial_radius).sqrt().unit.base_unit()
     particles.velocity = [0.0, 0.0, 0.0] | velocity_unit
-    
+
     plummer_radius = 0.1875 * numpy.pi * virial_radius
     u_unit = (velocity_unit**2).base_unit()
-    particles.u = (1 + particles.position.lengths_squared()/plummer_radius**2)**(-0.5) | u_unit
-    particles.u *= 0.25 * (G*total_mass**2/virial_radius) / particles.thermal_energy()
+    particles.u = (1 + particles.position.lengths_squared() / plummer_radius**2) ** (
+        -0.5
+    ) | u_unit
+    particles.u *= (
+        0.25 * (G * total_mass**2 / virial_radius) / particles.thermal_energy()
+    )
     return particles
+
+
 new_gas_plummer_distribution.__doc__ += plummer_arguments_doc
 
+
 def sample_from_velocity_distribution(number_of_particles):
     x = numpy.random.uniform(0.0, 1.0, number_of_particles)
     y = numpy.random.uniform(0.0, 0.1, number_of_particles)
-    selected = x[y <= (x**2) * (1.0 - x**2)**3.5]
+    selected = x[y <= (x**2) * (1.0 - x**2) ** 3.5]
     if len(selected) < number_of_particles:
-        return numpy.concatenate((selected, sample_from_velocity_distribution(number_of_particles-len(selected))))
+        return numpy.concatenate(
+            (
+                selected,
+                sample_from_velocity_distribution(number_of_particles - len(selected)),
+            )
+        )
     return selected
 
+
 def random_direction(number_of_particles):
     z = numpy.random.uniform(-1.0, 1.0, number_of_particles)
-    sine_theta = numpy.sqrt(1-z*z)
-    phi = numpy.random.uniform(0.0, 2*numpy.pi, number_of_particles)
-    return numpy.array([sine_theta * numpy.cos(phi), sine_theta * numpy.sin(phi), z]).transpose()
-
-def new_plummer_distribution(number_of_particles, 
-        total_mass = 1.0|nbody_system.mass, 
-        virial_radius = 1.0|nbody_system.length,
-        mass_cutoff = 0.999,
-        G = None,
-        **keyword_arguments):           # optional arguments for UniformSphericalDistribution
-    """
-    Create a plummer model with the given number of particles. Returns a set 
-    of particles with equal masses and positions distributed to fit a plummer 
-    distribution model. Velocities are sampled using von Neumann's rejection 
-    method (Aarseth et al. 1974), balancing the gravitational forces between 
+    sine_theta = numpy.sqrt(1 - z * z)
+    phi = numpy.random.uniform(0.0, 2 * numpy.pi, number_of_particles)
+    return numpy.array(
+        [sine_theta * numpy.cos(phi), sine_theta * numpy.sin(phi), z]
+    ).transpose()
+
+
+def new_plummer_distribution(
+    number_of_particles,
+    total_mass=1.0 | nbody_system.mass,
+    virial_radius=1.0 | nbody_system.length,
+    mass_cutoff=0.999,
+    G=None,
+    **keyword_arguments
+):  # optional arguments for UniformSphericalDistribution
+    """
+    Create a plummer model with the given number of particles. Returns a set
+    of particles with equal masses and positions distributed to fit a plummer
+    distribution model. Velocities are sampled using von Neumann's rejection
+    method (Aarseth et al. 1974), balancing the gravitational forces between
     the particles.
     """
-    particles = new_plummer_spatial_distribution(number_of_particles, total_mass=total_mass, 
-        virial_radius=virial_radius, **keyword_arguments)
-    
+    particles = new_plummer_spatial_distribution(
+        number_of_particles,
+        total_mass=total_mass,
+        virial_radius=virial_radius,
+        **keyword_arguments
+    )
+
     if G is None:
-        G = nbody_system.G if generic_unit_system.is_generic_unit(total_mass.unit) else constants.G
-    velocity_unit = (G*total_mass/virial_radius).sqrt().unit.base_unit()
+        G = (
+            nbody_system.G
+            if generic_unit_system.is_generic_unit(total_mass.unit)
+            else constants.G
+        )
+    velocity_unit = (G * total_mass / virial_radius).sqrt().unit.base_unit()
     plummer_radius = 0.1875 * numpy.pi * virial_radius
-    
-    escape_velocity = (1 + particles.position.lengths_squared()/plummer_radius**2)**(-0.25) | velocity_unit
+
+    escape_velocity = (
+        1 + particles.position.lengths_squared() / plummer_radius**2
+    ) ** (-0.25) | velocity_unit
     velocity = escape_velocity * sample_from_velocity_distribution(number_of_particles)
-    velocity *= numpy.sqrt((G*total_mass*number_of_particles) / (2*virial_radius*velocity.length_squared()))
-    particles.velocity = velocity.reshape((-1,1)) * random_direction(number_of_particles)
+    velocity *= numpy.sqrt(
+        (G * total_mass * number_of_particles)
+        / (2 * virial_radius * velocity.length_squared())
+    )
+    particles.velocity = velocity.reshape((-1, 1)) * random_direction(
+        number_of_particles
+    )
     return particles
+
+
 new_plummer_distribution.__doc__ += plummer_arguments_doc
```

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/star_to_sph.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/star_to_sph.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/static_potentials.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/static_potentials.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/stellar_gyration_radius.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/stellar_gyration_radius.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/stellar_tidal_evolution.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/stellar_tidal_evolution.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/stellar_wind.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/stellar_wind.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ext/sticky_spheres.py` & `amuse_framework-2024.4.0rc1/src/amuse/ext/sticky_spheres.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/__init__.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/_limepy/limepy.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/_limepy/limepy.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/_limepy/sample.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/_limepy/sample.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/brokenimf.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/brokenimf.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                     mass_boundaries[-j-2]**(
                         self.alphas[-j-1]-self.alphas[-j-2]
                     )
                 )
 
             result.append(factor)
         total = sum(result, 0.0)
-        return numpy.array(result)/total
+        return numpy.array(result)/total if bool(total) else numpy.array(result)
 
     def mass_mean(self):
         result = 0 | units.MSun
         for i in range(self.number_of_bins):
             a1 = self.alphas[i] + 1
             a2 = self.alphas[i] + 2
             m_low = self.mass_boundaries[i]
```

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/flatimf.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/flatimf.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/gasplummer.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/gasplummer.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,81 +12,93 @@
 from amuse.ext.evrard_test import uniform_unit_sphere
 from amuse.units import nbody_system
 from amuse.units import units
 from amuse import datamodel
 
 __all__ = ["new_plummer_gas_model"]
 
-class MakePlummerGasModel(object):
-    
-    def __init__(self, targetN, convert_nbody = None, base_grid=None, rscale=1/1.695,
-                   mass_cutoff = 0.999, do_scale = False):
+
+class MakePlummerGasModel:
+    def __init__(
+        self,
+        targetN,
+        convert_nbody=None,
+        base_grid=None,
+        rscale=1 / 1.695,
+        mass_cutoff=0.999,
+        do_scale=False,
+        **kwargs
+    ):
+        self.kwargs = kwargs
         self.targetN = targetN
         self.convert_nbody = convert_nbody
-        self.rscale=rscale
-        self.mass_frac=mass_cutoff
+        self.rscale = rscale
+        self.mass_frac = mass_cutoff
         self.do_scale = do_scale
         self.internal_energy = 0.25 / self.rscale
-        self.base_sphere=uniform_unit_sphere(targetN,base_grid)   
-           
+        self.base_sphere = uniform_unit_sphere(targetN, base_grid)
+
     def new_model(self):
-        x,y,z=self.base_sphere.make_xyz()
-        self.actualN=len(x)
-        r=numpy.sqrt(x**2+y**2+z**2)*self.mass_frac**(1/3.)
-        rtarget=self.rscale*(r**2/(1-r**2))**.5
-        mr=self.mass_frac**(1/3.)
-        maxr=self.rscale*(mr**2/(1-mr**2))**.5        
-        mass=numpy.ones_like(x)/self.actualN
-        internal_energy=self.internal_energy/(1+(rtarget/self.rscale)**2)**(1./2)
-        r=r.clip(1.e-8,maxr)
-        x=rtarget*x/r
-        y=rtarget*y/r
-        z=rtarget*z/r
-        vx=numpy.zeros_like(x)
-        vy=numpy.zeros_like(x)
-        vz=numpy.zeros_like(x)
-        return (mass,x,y,z,vx,vy,vz,internal_energy)
-    
+        x, y, z = self.base_sphere.make_xyz()
+        self.actualN = len(x)
+        r = numpy.sqrt(x**2 + y**2 + z**2) * self.mass_frac ** (1 / 3.0)
+        rtarget = self.rscale * (r**2 / (1 - r**2)) ** 0.5
+        mr = self.mass_frac ** (1 / 3.0)
+        maxr = self.rscale * (mr**2 / (1 - mr**2)) ** 0.5
+        mass = numpy.ones_like(x) / self.actualN
+        internal_energy = self.internal_energy / (1 + (rtarget / self.rscale) ** 2) ** (
+            1.0 / 2
+        )
+        r = r.clip(1.0e-8, maxr)
+        x = rtarget * x / r
+        y = rtarget * y / r
+        z = rtarget * z / r
+        vx = numpy.zeros_like(x)
+        vy = numpy.zeros_like(x)
+        vz = numpy.zeros_like(x)
+        return (mass, x, y, z, vx, vy, vz, internal_energy)
+
     @property
     def result(self):
-        mass,x,y,z,vx,vy,vz,u = self.new_model()
-        result = datamodel.Particles(self.actualN)
+        mass, x, y, z, vx, vy, vz, u = self.new_model()
+        result = datamodel.Particles(self.actualN, **self.kwargs)
         result.mass = nbody_system.mass.new_quantity(mass)
         result.x = nbody_system.length.new_quantity(x)
         result.y = nbody_system.length.new_quantity(y)
         result.z = nbody_system.length.new_quantity(z)
         result.vx = nbody_system.speed.new_quantity(vx)
         result.vy = nbody_system.speed.new_quantity(vy)
         result.vz = nbody_system.speed.new_quantity(vz)
         result.u = (nbody_system.speed**2).new_quantity(u)
 
         result.move_to_center()
         if self.do_scale:
-            potential_energy = result.potential_energy(G = nbody_system.G)
+            potential_energy = result.potential_energy(G=nbody_system.G)
             result.position *= potential_energy / (-0.5 | nbody_system.energy)
-            
+
             internal_energy = result.thermal_energy()
-            result.u *= ((0.25 | nbody_system.energy) / internal_energy)
-        
-        if not self.convert_nbody is None:
-            result = datamodel.ParticlesWithUnitsConverted(result, self.convert_nbody.as_converter_from_si_to_generic())
+            result.u *= (0.25 | nbody_system.energy) / internal_energy
+
+        if self.convert_nbody is not None:
+            result = datamodel.ParticlesWithUnitsConverted(
+                result, self.convert_nbody.as_converter_from_si_to_generic()
+            )
             result = result.copy()
-            
+
         return result
 
 
 def new_plummer_gas_model(number_of_particles, *list_arguments, **keyword_arguments):
     """
     Create a plummer gas model with the given number of particles. Returns
     a set of SPH particles with equal masses and positions distributed
     to fit a plummer distribution model. The model is centered around the
-    origin. Velocities are set to zero, and internal energies are set to 
+    origin. Velocities are set to zero, and internal energies are set to
     balance the gravitational forces between the gas particles.
 
     :argument number_of_particles: Number of particles to include in the plummer sphere
     :argument convert_nbody:  When given will convert the resulting set to SI units
     :argument mass_cutoff: Mass percentage inside radius of 1
     :argument do_scale: scale the result, similar to true nbody units (M=1, Q=0.25, U=-0.5)
     """
     uc = MakePlummerGasModel(number_of_particles, *list_arguments, **keyword_arguments)
     return uc.result
-
```

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/isotropic_cloud.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/isotropic_cloud.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,171 +19,193 @@
 
 import numpy
 
 from amuse.units import units, nbody_system
 from amuse.datamodel import Particles
 from amuse.community.kepler.interface import Kepler
 
+
 def random_power_min_max(size, x_min, x_max, exp_plus_one):
-  """
-  returns random floats in the interval [x_min,x_max] drawn from distribution
-  pdf(x) = const * x**(exp_plus_one-1), x_min <= x <= x_max; 
-  assuming: x_min < x_max, exp_plus_one != 0
-  """
-  r = numpy.random.random(size=size)
-  x_min_gamma = x_min**exp_plus_one
-  x_max_gamma = x_max**exp_plus_one
-  return (x_min_gamma + (x_max_gamma - x_min_gamma)*r)**(1./exp_plus_one)
-
-def relative_position_and_velocity_from_orbital_elements(mass1,
-                                                         mass2,
-                                                         semimajor_axis,
-                                                         eccentricity,
-                                                         mean_anomaly,
-                                                         seed=None):
-  """
-  Function that returns relative positions and velocity vectors or orbiters with masses 
-  mass2 of the central body with mass mass1 in Cartesian coordinates;
-  for vectors of orbital elements -- semi-major axes, eccentricities, mean anomalies.
-  3D orientation of orbits (inclination, longitude of ascending node and argument of periapsis) are random.
-  (cos(incl) is uniform -1--1, longitude of ascending node and argument of periapsis are uniform 0--2pi)
-  Assuming mass1 is static in the center [0,0,0] m, [0,0,0] km/s (that is mass2<<mass1)
-  """
-  position_vectors = []
-  velocity_vectors = []
-  converter = nbody_system.nbody_to_si(1|units.MSun,1|units.AU)
-  kepler = Kepler(converter)
-  kepler.initialize_code()
-  r_vec = (0.,0.,0.) | units.AU
-  v_vec = (0.,0.,0.) | units.kms
-  # to change seed for each particle
-  if seed is not None:
-    i=0
-  for m2_i, a_i, ecc_i, ma_i in zip(mass2, semimajor_axis, eccentricity, mean_anomaly):
-    #print m2_i, a_i, ecc_i, ma_i
+    """
+    returns random floats in the interval [x_min,x_max] drawn from distribution
+    pdf(x) = const * x**(exp_plus_one-1), x_min <= x <= x_max;
+    assuming: x_min < x_max, exp_plus_one != 0
+    """
+    r = numpy.random.random(size=size)
+    x_min_gamma = x_min**exp_plus_one
+    x_max_gamma = x_max**exp_plus_one
+    return (x_min_gamma + (x_max_gamma - x_min_gamma) * r) ** (1.0 / exp_plus_one)
+
+
+def relative_position_and_velocity_from_orbital_elements(
+    mass1, mass2, semimajor_axis, eccentricity, mean_anomaly, seed=None
+):
+    """
+    Function that returns relative positions and velocity vectors or orbiters
+    with masses mass2 of the central body with mass mass1 in Cartesian
+    coordinates; for vectors of orbital elements -- semi-major axes,
+    eccentricities, mean anomalies.
+    3D orientation of orbits (inclination, longitude of ascending node and
+    argument of periapsis) are random.  (cos(incl) is uniform -1--1, longitude
+    of ascending node and argument of periapsis are uniform 0--2pi)
+    Assuming mass1 is static in the center [0,0,0] m, [0,0,0] km/s (that is
+    mass2<<mass1)
+    """
+    position_vectors = []
+    velocity_vectors = []
+    converter = nbody_system.nbody_to_si(1 | units.MSun, 1 | units.AU)
+    kepler = Kepler(converter)
+    kepler.initialize_code()
+    r_vec = (0.0, 0.0, 0.0) | units.AU
+    v_vec = (0.0, 0.0, 0.0) | units.kms
+    # to change seed for each particle
     if seed is not None:
-      kepler.set_random(seed+i)
-      i=i+1
-    kepler.initialize_from_elements(mass=(mass1+m2_i),semi=a_i,ecc=ecc_i,mean_anomaly=ma_i,random_orientation=-1)
-    ri = kepler.get_separation_vector()
-    vi = kepler.get_velocity_vector()
-    # this is to get ~half of the orbits retrograde (that is with inclination
-    # of 90--180 degrees) --> velocity = -velocity
-    vel_vec_dir = numpy.random.random()
-    if (vel_vec_dir<=0.5):
-      vel_orientation = 1.
-    else:
-      vel_orientation = -1.
-    position_vectors.append([ri[0], ri[1], ri[2]])
-    velocity_vectors.append([vel_orientation*vi[0], vel_orientation*vi[1], vel_orientation*vi[2]])
-  kepler.stop()
-  return position_vectors, velocity_vectors
-
-def ecc_random_power_with_min_peri(n, semi, min_peri, power=2.):
-  """
-  random distribution in eccentricity P(e)~e
-  (power = actual_exponent + 1)
-  with minimum pericenter of min_peri
-  for given semi-major axes semi
-  """
-  x = numpy.random.power(power,size=n)
-  peri = semi*(1.-x)
-  while numpy.any(peri<min_peri):
-    filter_small_peri = (peri<min_peri)
-    n_new = sum(filter_small_peri)
-    #print "\t updating q", peri.min().in_(units.AU), n_new
-    x_random_new = numpy.random.power(power,size=n_new)
-    x_new = 1.*x
-    x_new[filter_small_peri] = x_random_new
-    x = 1.*x_new
-    peri = semi*(1.-x)
-  return x
-
-
-class SphericalIsotropicCloud(object):
-  def __init__(self,
-               targetN,
-               m_star=1.|units.MSun,
-               m_cloud=0.|units.MSun,
-               a_min=3000.|units.AU,
-               a_max=10000.|units.AU,
-               q_min=32.|units.AU,
-               gamma=-1.5,
-               seed=None):
-    self.targetN = targetN
-    self.m_star = m_star
-    self.m_cloud = m_cloud
-    self.a_min = a_min
-    self.a_max = a_max
-    self.q_min = q_min
-    self.gamma = gamma
-    self.seed = seed
-    
-    if (self.q_min is not None):
-      if (self.q_min > self.a_min):
-        self.a_min_q_corr = self.q_min
-      else:
-        self.a_min_q_corr = self.a_min
-    else:
-      self.a_min_q_corr = self.a_min
-  
-  def new_model(self):
-    if self.seed is not None:
-      numpy.random.seed(self.seed)
-    
-    a_in_au = random_power_min_max(self.targetN, 
-                                   self.a_min_q_corr.value_in(units.AU),
-                                   self.a_max.value_in(units.AU),
-                                   self.gamma+1.)
-    a = a_in_au * 1.|units.AU
-    ecc = ecc_random_power_with_min_peri(self.targetN, a, self.q_min, power=2.)
-    mean_anomaly = 2.*numpy.pi * numpy.random.random(size=self.targetN)
-    m_comets = (self.m_cloud / self.targetN) * numpy.ones_like(ecc)
-    position_vectors, velocity_vectors = \
-      relative_position_and_velocity_from_orbital_elements(self.m_star,
-                                                           m_comets,
-                                                           a,
-                                                           ecc,
-                                                           mean_anomaly,
-                                                           seed=self.seed)
-    return (m_comets, position_vectors, velocity_vectors)
-  
-  @property
-  def result(self):
-    masses, position_vectors, velocity_vectors = self.new_model()
-    result = Particles(self.targetN)
-    result.mass = masses
-    result.position = position_vectors
-    result.velocity = velocity_vectors
-    return result
-  
+        i = 0
+    for m2_i, a_i, ecc_i, ma_i in zip(
+        mass2, semimajor_axis, eccentricity, mean_anomaly
+    ):
+        # print m2_i, a_i, ecc_i, ma_i
+        if seed is not None:
+            kepler.set_random(seed + i)
+            i = i + 1
+        kepler.initialize_from_elements(
+            mass=(mass1 + m2_i),
+            semi=a_i,
+            ecc=ecc_i,
+            mean_anomaly=ma_i,
+            random_orientation=-1,
+        )
+        ri = kepler.get_separation_vector()
+        vi = kepler.get_velocity_vector()
+        # this is to get ~half of the orbits retrograde (that is with inclination
+        # of 90--180 degrees) --> velocity = -velocity
+        vel_vec_dir = numpy.random.random()
+        if vel_vec_dir <= 0.5:
+            vel_orientation = 1.0
+        else:
+            vel_orientation = -1.0
+        position_vectors.append([ri[0], ri[1], ri[2]])
+        velocity_vectors.append(
+            [vel_orientation * vi[0], vel_orientation * vi[1], vel_orientation * vi[2]]
+        )
+    kepler.stop()
+    return position_vectors, velocity_vectors
+
+
+def ecc_random_power_with_min_peri(n, semi, min_peri, power=2.0):
+    """
+    random distribution in eccentricity P(e)~e
+    (power = actual_exponent + 1)
+    with minimum pericenter of min_peri
+    for given semi-major axes semi
+    """
+    x = numpy.random.power(power, size=n)
+    peri = semi * (1.0 - x)
+    while numpy.any(peri < min_peri):
+        filter_small_peri = peri < min_peri
+        n_new = sum(filter_small_peri)
+        # print "\t updating q", peri.min().in_(units.AU), n_new
+        x_random_new = numpy.random.power(power, size=n_new)
+        x_new = 1.0 * x
+        x_new[filter_small_peri] = x_random_new
+        x = 1.0 * x_new
+        peri = semi * (1.0 - x)
+    return x
+
+
+class SphericalIsotropicCloud:
+    def __init__(
+        self,
+        targetN,
+        m_star=1.0 | units.MSun,
+        m_cloud=0.0 | units.MSun,
+        a_min=3000.0 | units.AU,
+        a_max=10000.0 | units.AU,
+        q_min=32.0 | units.AU,
+        gamma=-1.5,
+        seed=None,
+        **kwargs
+    ):
+        self.kwargs = kwargs
+        self.targetN = targetN
+        self.m_star = m_star
+        self.m_cloud = m_cloud
+        self.a_min = a_min
+        self.a_max = a_max
+        self.q_min = q_min
+        self.gamma = gamma
+        self.seed = seed
+
+        if self.q_min is not None:
+            if self.q_min > self.a_min:
+                self.a_min_q_corr = self.q_min
+            else:
+                self.a_min_q_corr = self.a_min
+        else:
+            self.a_min_q_corr = self.a_min
+
+    def new_model(self):
+        if self.seed is not None:
+            numpy.random.seed(self.seed)
+
+        a_in_au = random_power_min_max(
+            self.targetN,
+            self.a_min_q_corr.value_in(units.AU),
+            self.a_max.value_in(units.AU),
+            self.gamma + 1.0,
+        )
+        a = a_in_au * 1.0 | units.AU
+        ecc = ecc_random_power_with_min_peri(self.targetN, a, self.q_min, power=2.0)
+        mean_anomaly = 2.0 * numpy.pi * numpy.random.random(size=self.targetN)
+        m_comets = (self.m_cloud / self.targetN) * numpy.ones_like(ecc)
+        (
+            position_vectors,
+            velocity_vectors,
+        ) = relative_position_and_velocity_from_orbital_elements(
+            self.m_star, m_comets, a, ecc, mean_anomaly, seed=self.seed
+        )
+        return (m_comets, position_vectors, velocity_vectors)
+
+    @property
+    def result(self):
+        masses, position_vectors, velocity_vectors = self.new_model()
+        result = Particles(self.targetN, **self.kwargs)
+        result.mass = masses
+        result.position = position_vectors
+        result.velocity = velocity_vectors
+        return result
+
+
 def new_isotropic_cloud(number_of_particles, *list_arguments, **keyword_arguments):
-  """
-  Spherical isotropic cloud ~ Oort cloud given by distributions of orbital elements:
-    semi-major axes -- power law, default: dn/da ~ a^(-1.5),
-    eccentricities -- dn/de ~ e,
-    constrain on the minimum pericenter,
-    isotropic orbits -- distribution of orbital inclinations: cos(i) = -1--1,
-        longitude of ascending node: 0--2pi,
-        argument of periastron: 0--2pi,
-        mean anomaly: 0--2pi,
-    equal mass particles
-  
-  The default values correspond to papers:
-  * Duncan, M.; Quinn, T.; Tremaine, S. -- http://adsabs.harvard.edu/abs/1987AJ.....94.1330D
-  * Feng, F.; Bailer-Jones, C. A. L. -- http://adsabs.harvard.edu/abs/2014MNRAS.442.3653F (their DQT model)
-  
-  :argument number_of_particles: number of particles to include in the cloud
-  :argument m_star: mass of the central star
-  :argument m_cloud: total mass of the cloud (particles are equal mass)
-  :argument a_min: minimal semimajor axis
-  :argument a_max: maximal semimajor axis, a_min < a_max
-  :argument q_min: minimal pericenter
-  :argument gamma: exponent of the semimajor axis distribution, f(a) ~ a^(gamma)
-  :argument seed: random seed -- set to reproduce exactly the same IC
-  """
-  uc = SphericalIsotropicCloud(number_of_particles, *list_arguments, **keyword_arguments)
-  return uc.result
-
-if __name__ in ('__main__'):
-  cloud = new_isotropic_cloud(10)
-  print(cloud)
+    """
+    Spherical isotropic cloud ~ Oort cloud given by distributions of orbital elements:
+      semi-major axes -- power law, default: dn/da ~ a^(-1.5),
+      eccentricities -- dn/de ~ e,
+      constrain on the minimum pericenter,
+      isotropic orbits -- distribution of orbital inclinations: cos(i) = -1--1,
+          longitude of ascending node: 0--2pi,
+          argument of periastron: 0--2pi,
+          mean anomaly: 0--2pi,
+      equal mass particles
+
+    The default values correspond to papers:
+    * Duncan, M.; Quinn, T.; Tremaine, S. -- http://adsabs.harvard.edu/abs/1987AJ.....94.1330D
+    * Feng, F.; Bailer-Jones, C. A. L. -- http://adsabs.harvard.edu/abs/2014MNRAS.442.3653F (their DQT model)
+
+    :argument number_of_particles: number of particles to include in the cloud
+    :argument m_star: mass of the central star
+    :argument m_cloud: total mass of the cloud (particles are equal mass)
+    :argument a_min: minimal semimajor axis
+    :argument a_max: maximal semimajor axis, a_min < a_max
+    :argument q_min: minimal pericenter
+    :argument gamma: exponent of the semimajor axis distribution, f(a) ~ a^(gamma)
+    :argument seed: random seed -- set to reproduce exactly the same IC
+    """
+    uc = SphericalIsotropicCloud(
+        number_of_particles, *list_arguments, **keyword_arguments
+    )
+    return uc.result
+
+
+if __name__ in ("__main__"):
+    cloud = new_isotropic_cloud(10)
+    print(cloud)
```

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/kingmodel.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/kingmodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,174 +9,204 @@
 
 from amuse.support import exceptions
 from amuse.units import nbody_system
 from amuse import datamodel
 
 __all__ = ["new_king_model"]
 
-class MakeKingModel(object):
-    def __init__(self, number_of_particles, W0, convert_nbody = None, do_scale = False, 
-            beta = 0.0, verbose = False,center_model=True):
+
+class MakeKingModel:
+    """
+    Makes a distribution of particles following a King model
+    """
+
+    def __init__(
+        self,
+        number_of_particles,
+        W0,
+        convert_nbody=None,
+        do_scale=False,
+        beta=0.0,
+        verbose=False,
+        center_model=True,
+        **kwargs
+    ):
+        self.kwargs = kwargs
         self.number_of_particles = number_of_particles
         self.convert_nbody = convert_nbody
-        self.center_model=center_model
+        self.center_model = center_model
         self.do_scale = do_scale
         self.verbose = verbose
         self.beta = beta
         self.W0 = W0
-        self.beta_w0 = beta*W0
+        self.beta_w0 = beta * W0
         self.scale_fac = math.exp(self.beta_w0)
 
-        self.YMAX = 4.0 # Note: make sure YMAX is a float.
+        self.YMAX = 4.0  # Note: make sure YMAX is a float.
         self.NG = 1000
         self.g_integral = self.compute_g_integral()
         self.v33 = self.compute_v33()
-        
+
         # // profile
         self.NM = 2500
-        self.rr=[]; self.d=[]; self.v2=[]; self.psi=[]; self.zm=[]
+        self.rr = []
+        self.d = []
+        self.v2 = []
+        self.psi = []
+        self.zm = []
         self.NINDX = 100
-        self.index=[]
-    
+        self.index = []
+
     def compute_v33(self):
         v33 = []
-        for i in range(self.NG+1):
-            v33.append(self.scale_fac * math.pow(((self.YMAX/self.NG) * i), 3) / 3.0)
+        for i in range(self.NG + 1):
+            v33.append(self.scale_fac * math.pow(((self.YMAX / self.NG) * i), 3) / 3.0)
         return v33
-    
+
     def compute_g_integral(self):
-        dy = self.YMAX/self.NG
+        dy = self.YMAX / self.NG
         g = [0.0]
         for i in range(self.NG):
-            g.append(g[i]+self.trapzd_gaus2(i*dy,(i+1)*dy))
+            g.append(g[i] + self.trapzd_gaus2(i * dy, (i + 1) * dy))
         return g
-            
+
     # Trapezoid Rule for integration, after NR.
     def trapzd_gaus2(self, a, b):
-        eps = 1.e-10
+        eps = 1.0e-10
         max_steps = 50
         previous_sum = -1.0e30
         for i in range(max_steps):
             sum = self.trapint_gaus2(a, b, i, previous_sum)
-            if (abs(sum - previous_sum) < eps * abs(previous_sum)): return sum
+            if abs(sum - previous_sum) < eps * abs(previous_sum):
+                return sum
             previous_sum = sum
         return 0.0
-        
+
     # Integrate func from a to b in n steps, using the trapezoid rule.
     def trapint_gaus2(self, a, b, n, previous_sum):
-        if (n == 0):
+        if n == 0:
             return 0.5 * (b - a) * (self.gaus2(a) + self.gaus2(b))
         else:
-            base = 2**(n-1)
+            base = 2 ** (n - 1)
             dx = (b - a) / base
             x = a + 0.5 * dx
             sum = 0.0
             for i in range(base):
                 sum = sum + self.gaus2(x)
                 x = x + dx
-            return 0.5 * (previous_sum + (b - a)/base * sum)
-            
+            return 0.5 * (previous_sum + (b - a) / base * sum)
+
     def gaus2(self, x):
-        return x*x*math.exp(-x*x)
-        
+        return x * x * math.exp(-x * x)
+
     def gg_integral(self, y, g4_flag):
         # Array g contains the indefinite integral (from 0) of y^2 exp(-y^2) dy,
         # up to a maximum value of YMAX, i.e.
         #
-        #	g[i]  =  integral{0 to Y} y^2 exp(-y^2) dy,
+        # 	g[i]  =  integral{0 to Y} y^2 exp(-y^2) dy,
         #
         # where Y  =  i*YMAX/NG (i = 0,...,NG).
         #
         # Function computes  g2  =  integral{0 to y} y^2 exp(-y^2) dy
         #               and  g4  =  integral{0 to y} y^4 exp(-y^2) dy.
-        if (y >= self.YMAX):
+        if y >= self.YMAX:
             g2 = self.g_integral[self.NG]
         else:
             yindx = self.NG * y / self.YMAX
             intyindx = int(yindx)
-            g2 = self.g_integral[intyindx] + (yindx-intyindx)*(self.g_integral[intyindx+1]-self.g_integral[intyindx])
-        if (g4_flag):
-            return (g2, 1.5*g2 - 0.5*y**3*math.exp(-y*y))
+            g2 = self.g_integral[intyindx] + (yindx - intyindx) * (
+                self.g_integral[intyindx + 1] - self.g_integral[intyindx]
+            )
+        if g4_flag:
+            return (g2, 1.5 * g2 - 0.5 * y**3 * math.exp(-y * y))
         else:
             return (g2, 0.0)
-    
+
     # Return density d and local velocity dispersion v2,
     # given scaled potential psi (< 0).
     def get_dens_and_vel(self, psi, v2_flag):
-        if (psi >= -self.beta_w0): 
-            if (v2_flag): return (0.0, 1.0)
-            else: return 0.0
+        if psi >= -self.beta_w0:
+            if v2_flag:
+                return (0.0, 1.0)
+            else:
+                return 0.0
         #  // Distribution function is
         #  //
         #  //	f(r,v) = A exp(-psi) (exp(-v^2 / 2 sig^2) - exp(psi - beta*psi0)),
         #  //
         #  // where psi = phi/sig^2 and psi0 = -w0.
         #  //
         #  // Density is the integral of 4 pi v^2 f, velocity dispersion v2
         #  // is (integral of 4 pi v^4 f) / density.
-        p_max = -psi - self.beta_w0	# // v_max^2 / (2 sig^2)
+        p_max = -psi - self.beta_w0  # // v_max^2 / (2 sig^2)
         y_max = math.sqrt(p_max)
         ep = math.exp(-psi)
         (g2, g4) = self.gg_integral(y_max, v2_flag)
         dens = ep * g2 - self.scale_fac * y_max * p_max / 3
         #  // Note that this expression for dens excludes an overall factor
         #  // of 8 pi sqrt(2) sig^3 A.  Scaling to the central density
         #  // is handled elsewhere (in rhs).
-        if (v2_flag):
+        if v2_flag:
             v2 = 2 * (ep * g4 - 0.2 * self.scale_fac * y_max * p_max * p_max) / dens
             return (dens, v2)
         else:
             return dens
         #  // The unit of v2 is sig^2.
-    
+
     def rhs(self, y, x):
         # //  Define RHS of ODE, for use by rk4.
         ypr = []
         ypr.append(y[1])
-        if (x <= 0):
+        if x <= 0:
             d = 1
         else:
-            d = (self.get_dens_and_vel(y[0]/x, False)) * self.dc_inverse
+            d = (self.get_dens_and_vel(y[0] / x, False)) * self.dc_inverse
             # // d is rho/rho_0
             # // False suppresses vel
         ypr.append(9 * x * d)
         return ypr
-    
-    # //  Runge-Kutta-4 method 
+
+    # //  Runge-Kutta-4 method
     def step(self, y, x, dx, N):
         # Doesn't look very efficient...
-        dy1=[]; dy2=[]; dy3=[]; dy4=[]
-        y1=[]; y2=[]; y3=[]; y4=[]
+        dy1 = []
+        dy2 = []
+        dy3 = []
+        dy4 = []
+        y1 = []
+        y2 = []
+        y3 = []
+        y4 = []
         dydx = self.rhs(y, x)
         for i in range(N):
-            dy1.append(dx*dydx[i])
-            y1.append(y[i] + 0.5*dy1[i])
-        dydx = self.rhs(y1, x+0.5*dx)
+            dy1.append(dx * dydx[i])
+            y1.append(y[i] + 0.5 * dy1[i])
+        dydx = self.rhs(y1, x + 0.5 * dx)
         for i in range(N):
-            dy2.append(dx*dydx[i])
-            y2.append(y[i] + 0.5*dy2[i])
-        dydx = self.rhs(y2, x+0.5*dx)
+            dy2.append(dx * dydx[i])
+            y2.append(y[i] + 0.5 * dy2[i])
+        dydx = self.rhs(y2, x + 0.5 * dx)
         for i in range(N):
-            dy3.append(dx*dydx[i])
+            dy3.append(dx * dydx[i])
             y3.append(y[i] + dy3[i])
-        dydx = self.rhs(y3, x+dx)
+        dydx = self.rhs(y3, x + dx)
         for i in range(N):
-            dy4.append(dx*dydx[i])
-            y[i] = y[i] + (dy1[i] + 2*dy2[i] + 2*dy3[i] + dy4[i])/6.0
+            dy4.append(dx * dydx[i])
+            y[i] = y[i] + (dy1[i] + 2 * dy2[i] + 2 * dy3[i] + dy4[i]) / 6.0
         return y
-    
+
     def rk4(self, x, x_next, y, N, dx):
         # // Integrate the y(x) from x to x_next, using an integration step of dx.
         # // On entry y is y at the initial x.  On exit, x is replaced by x_next
         # // and y is y(x).
-        while (x < x_next - .5*dx): # // NOTE!!  Beware of rounding error!
+        while x < x_next - 0.5 * dx:  # // NOTE!!  Beware of rounding error!
             y = self.step(y, x, dx, N)
             x = x + dx
         return (x, y)
-    
+
     def poisson(self):
         # //       Self-contained 1-D (spherical) Poisson's equation solver.
         # //       Currently knows about normal and lowered King models.
         # //
         # //        Input:  nmax is the maximum number of points allowed
         # //                w0 is the dimensionless central potential
         # //                iout allows messages if nonzero
@@ -187,316 +217,347 @@
         # //                psi is scaled potential (-W0 at center)
         # //                zm  is cumulative mass (scaling from x, d scalings)
         # //                nprof is the actual number of points generated
         # //                v20 is the central 3-D velocity dispersion (unit = sig^2)
         RLIN = 0.25
         NLIN = 105
         RMAX = 1e4
-        
+
         nmax = self.NM
-        psi0 = - abs(self.W0)
+        psi0 = -abs(self.W0)
         #  // Initialize at center of cluster.
         y = [0.0, psi0]
         xn = 0.0
         self.rr.append(0.0)
         self.psi.append(psi0)
         self.zm.append(0.0)
         #  // Establish density scaling factor.
         (density, velocity_dispersion) = self.get_dens_and_vel(psi0, True)
         self.d.append(density)
         self.v2.append(velocity_dispersion)
-        self.dc_inverse = 1./density
-        fac = math.pow(10, (math.log10(RMAX/RLIN) / (nmax-NLIN)))
-        #// 	Poisson's equation is:
-        #//
-        #// 		(1/r^2) d/dr (r^2 dphi/dr)  =  4 pi G rho,
-        #//
-        #// 	where r is radius, phi is potential, and rho is density, given
-        #// 	(for equal-mass stars) by
-        #//
-        #// 		rho	=  {integral (v < ve)} 4 pi v^2 f(v) dv,
-        #//
-        #// 	where ve is the escape velocity,
-        #//
-        #// 		ve^2	=  -2 phi.
-        #//
-        #// 	The (3-D) velocity distribution is
-        #//
-        #// 		f(v)	=  A (exp(-v^2 / 2 sig^2)
-        #// 					 - exp(-ve^2 / 2 sig^2)),
-        #//
-        #// 	where sig^2 is a 1-D velocity dispersion (not quite the
-        #// 	central velocity dispersion, except in the limit of infinite
-        #// 	central potential).  In King's (1966) paper, he uses
-        #// 	j^2 = 1 / (2 sig^2).
-        #//
-        #// 	Following King, we define the core radius rc by
-        #//
-        #// 		rc^2	=  9 sig^2 / (4 pi G rho0)
-        #//
-        #// 	and the dimensionless depth as
-        #//
-        #// 		W0	=  -phi0 / sig^2,
-        #//
-        #// 	where rho0 and phi0 are the central density and potential,
-        #// 	respectively.
-        #//
-        #// 	We then scale as follows:
-        #//
-        #// 		x	=  r / rc
-        #//
-        #// 		d	=  rho / rho0
-        #//
-        #// 		psi	=  phi / sig^2,
-        #//
-        #// 	to obtain
-        #//
-        #// 		(x psi)''  =  9 x d,
-        #//
-        #// 	where ' = d/dx.
-        #//
-        #// 	We integrate this ODE from the cluster center (x = 0, d = 1,
-        #// 	psi = -W0) to the tidal radius (d = 0) by defining
-        #//
-        #//		y(0)	=  (x psi)
-        #//		y(1)	=  y(0)'
-        #//
-        #//	We cover the first RLIN core radii linearly with NLIN points;
-        #//	the remaining coverage is logarithmic, out to RMAX core radii,
-        #//	if necessary.  We stop when d <= 0.
+        self.dc_inverse = 1.0 / density
+        fac = math.pow(10, (math.log10(RMAX / RLIN) / (nmax - NLIN)))
+        # // 	Poisson's equation is:
+        # //
+        # // 		(1/r^2) d/dr (r^2 dphi/dr)  =  4 pi G rho,
+        # //
+        # // 	where r is radius, phi is potential, and rho is density, given
+        # // 	(for equal-mass stars) by
+        # //
+        # // 		rho	=  {integral (v < ve)} 4 pi v^2 f(v) dv,
+        # //
+        # // 	where ve is the escape velocity,
+        # //
+        # // 		ve^2	=  -2 phi.
+        # //
+        # // 	The (3-D) velocity distribution is
+        # //
+        # // 		f(v)	=  A (exp(-v^2 / 2 sig^2)
+        # // 					 - exp(-ve^2 / 2 sig^2)),
+        # //
+        # // 	where sig^2 is a 1-D velocity dispersion (not quite the
+        # // 	central velocity dispersion, except in the limit of infinite
+        # // 	central potential).  In King's (1966) paper, he uses
+        # // 	j^2 = 1 / (2 sig^2).
+        # //
+        # // 	Following King, we define the core radius rc by
+        # //
+        # // 		rc^2	=  9 sig^2 / (4 pi G rho0)
+        # //
+        # // 	and the dimensionless depth as
+        # //
+        # // 		W0	=  -phi0 / sig^2,
+        # //
+        # // 	where rho0 and phi0 are the central density and potential,
+        # // 	respectively.
+        # //
+        # // 	We then scale as follows:
+        # //
+        # // 		x	=  r / rc
+        # //
+        # // 		d	=  rho / rho0
+        # //
+        # // 		psi	=  phi / sig^2,
+        # //
+        # // 	to obtain
+        # //
+        # // 		(x psi)''  =  9 x d,
+        # //
+        # // 	where ' = d/dx.
+        # //
+        # // 	We integrate this ODE from the cluster center (x = 0, d = 1,
+        # // 	psi = -W0) to the tidal radius (d = 0) by defining
+        # //
+        # //		y(0)	=  (x psi)
+        # //		y(1)	=  y(0)'
+        # //
+        # //	We cover the first RLIN core radii linearly with NLIN points;
+        # //	the remaining coverage is logarithmic, out to RMAX core radii,
+        # //	if necessary.  We stop when d <= 0.
         stopped = False
-        for i in range(1,nmax+1):
+        for i in range(1, nmax + 1):
             xo = xn
-            if (i <= NLIN):
+            if i <= NLIN:
                 xn = (RLIN * i) / NLIN
             else:
                 xn = fac * xo
-            dx = 0.051*(xn-xo)
+            dx = 0.051 * (xn - xo)
             (xo, y) = self.rk4(xo, xn, y, 2, dx)
             # //  N.B. Remember that y(1) is x*psi and xo is updated by step.
             xn = xo
             self.rr.append(xn)
             self.psi.append(y[0] / xn)
             (density, velocity_dispersion) = self.get_dens_and_vel(self.psi[i], True)
             self.d.append(density)
             self.v2.append(velocity_dispersion)
-            if (density < 0):
+            if density < 0:
                 # 	// Density is negative, calculation is over.
                 # 	// Interpolate to the tidal radius.
-                self.rr[i] = self.rr[i-1] + (self.rr[i] - self.rr[i-1]) / (0.1 - self.d[i]/self.d[i-1])
+                self.rr[i] = self.rr[i - 1] + (self.rr[i] - self.rr[i - 1]) / (
+                    0.1 - self.d[i] / self.d[i - 1]
+                )
                 self.d[i] = 0
                 self.v2[i] = 0
             self.zm.append(self.rr[i] * y[1] - y[0])
-            if (density <= 0):
+            if density <= 0:
                 stopped = True
                 break
-        if not stopped: i = nmax
+        if not stopped:
+            i = nmax
         nprof = i
         #  // Scale d and v2 to their central values.  Save v2_0 (unit = sig^2).
         v2_0 = self.v2[0]
         d_0 = self.d[0]
         c_zm = 4.0 * math.pi / 9.0
-        self.d[:] = [x/d_0 for x in self.d]
-        self.v2[:] = [x/v2_0 for x in self.v2]
-        self.zm[:] = [x*c_zm for x in self.zm]
+        self.d[:] = [x / d_0 for x in self.d]
+        self.v2[:] = [x / v2_0 for x in self.v2]
+        self.zm[:] = [x * c_zm for x in self.zm]
         return nprof, v2_0
-    
+
     def coordinates_from_spherical(self, radius, theta, phi):
-        x = radius * numpy.sin( theta ) * numpy.cos( phi )
-        y = radius * numpy.sin( theta ) * numpy.sin( phi )
-        z = radius * numpy.cos( theta )
-        return [x,y,z]
-    
+        x = radius * numpy.sin(theta) * numpy.cos(phi)
+        y = radius * numpy.sin(theta) * numpy.sin(phi)
+        z = radius * numpy.cos(theta)
+        return [x, y, z]
+
     def setpos(self):
         # // Obtain a random position for body b from the King profile
         # // and return the scaled potential at that location.
-        
+
         #  //  Choose radius randomly from the mass distribution.
         rno = numpy.random.uniform()
         i = int(self.NINDX * rno)
         found_index = False
-        for i1 in range(self.index[i],self.index[i+1]+2): #(i1 = self.indx[i]; i1 <= indx[i+1]+1; i1++)
-            if (self.zm[i1] > rno):
+        for i1 in range(
+            self.index[i], self.index[i + 1] + 2
+        ):
+            if self.zm[i1] > rno:
                 found_index = True
                 break
-        if (not found_index):
+        if not found_index:
             raise exceptions.AmuseException("makeking: error in getpos")
-        rfac = (rno - self.zm[i1-1]) / (self.zm[i1] - self.zm[i1-1])
-        radius = self.rr[i1-1] + rfac * (self.rr[i1] - self.rr[i1-1])
-        potential = self.psi[i1-1] + rfac * (self.psi[i1] - self.psi[i1-1])
-        
+        rfac = (rno - self.zm[i1 - 1]) / (self.zm[i1] - self.zm[i1 - 1])
+        radius = self.rr[i1 - 1] + rfac * (self.rr[i1] - self.rr[i1 - 1])
+        potential = self.psi[i1 - 1] + rfac * (self.psi[i1] - self.psi[i1 - 1])
+
         #  //  Angular position random.
         theta = numpy.arccos(numpy.random.uniform(-1.0, 1.0))
-        phi = numpy.random.uniform(0.0, 2.0*math.pi)
+        phi = numpy.random.uniform(0.0, 2.0 * math.pi)
         return self.coordinates_from_spherical(radius, theta, phi), potential
-    
+
     def setvel(self, potential):
-        #// Obtain a random velocity for body b from the King profile
-        #// given its scaled potential.
-        
+        # // Obtain a random velocity for body b from the King profile
+        # // given its scaled potential.
+
         #    // Array v33[] contains the second term in the integral for the density,
         #    // namely exp(beta*W0) * v_esc^3 / 3 (scaling v^2 by 2 sig^2, as usual).
         #    // As with g[], the array indices run from 0 to NG, spanning a range 0 to
         #    // YMAX, i.e. the cumulative distribution function for v is
         #    //
         #    //		exp(-p) * g[i] - v33[i],
         #    //
         #    // where y = i*YMAX/NG (i = 0,...,NG) and v = sqrt(2)*sig*y (sig = 1 here).
 
         #    //  Choose speed randomly from the distribution at this radius.
         v = 0
-        if (potential < -self.beta_w0):
+        if potential < -self.beta_w0:
             pfac = math.exp(-potential)
-            ymax = math.sqrt(-potential-self.beta_w0)
-            #	// Will obtain v by bisection.  Determine maximum possible
-            #	// range in the index i.
+            ymax = math.sqrt(-potential - self.beta_w0)
+            # 	// Will obtain v by bisection.  Determine maximum possible
+            # 	// range in the index i.
             il = 0
-            iu = int(((self.NG/self.YMAX) * math.sqrt(-potential))) #	// Binning OK for W0 < 16,
+            iu = int(
+                ((self.NG / self.YMAX) * math.sqrt(-potential))
+            )  # 	// Binning OK for W0 < 16,
             #   				        		// *only* if beta >= 0.
-            if (iu > self.NG): 
+            if iu > self.NG:
                 iu = self.NG
             rl = 0
             ru = pfac * self.g_integral[iu] - self.v33[iu]
             rno = numpy.random.uniform(0.0, ru)
-            while (iu - il > 1):
+            while iu - il > 1:
                 im = (il + iu) // 2
                 rm = pfac * self.g_integral[im] - self.v33[im]
-                if (rm > rno):
+                if rm > rno:
                     iu = im
                     ru = rm
                 else:
                     il = im
                     rl = rm
-            #	// Maximum possible range of il here (for beta = 0) is
-            #	//	0 to NG*sqrt(-p)/YMAX.
-            #	// Maximum possible value of v (for beta = 0) is the local
-            #	//      escape speed, sqrt(-2*p).
-            v = (self.YMAX/self.NG) * math.sqrt(2.0) * (il + (rno - rl)/(ru - rl))
+            # 	// Maximum possible range of il here (for beta = 0) is
+            # 	//	0 to NG*sqrt(-p)/YMAX.
+            # 	// Maximum possible value of v (for beta = 0) is the local
+            # 	//      escape speed, sqrt(-2*p).
+            v = (self.YMAX / self.NG) * math.sqrt(2.0) * (il + (rno - rl) / (ru - rl))
         #    //  Direction is random.
         theta = numpy.arccos(numpy.random.uniform(-1.0, 1.0))
-        phi = numpy.random.uniform(0.0, 2.0*math.pi)
+        phi = numpy.random.uniform(0.0, 2.0 * math.pi)
         return self.coordinates_from_spherical(v, theta, phi)
-        
+
     def makeking(self):
-        #// Create a King model, and optionally initialize an N-body system
-        #// with total mass = n, core radius = 1.
-        if (self.W0 > 16): 
+        # // Create a King model, and optionally initialize an N-body system
+        # // with total mass = n, core radius = 1.
+        if self.W0 > 16:
             raise exceptions.AmuseException("makeking: must specify w0 < 16")
         #    // Compute the cluster density/velocity/potential profile
         (nprof, v20) = self.poisson()
         zm = self.zm
         d = self.d
         rr = self.rr
         v2 = self.v2
         psi = self.psi
-        if not (len(zm) == nprof+1 and len(d) == nprof+1 and 
-            len(rr) == nprof+1 and len(v2) == nprof+1 and 
-            len(psi) == nprof+1):
-            print(len(zm), len(d), len(rr), len(v2), len(psi), nprof+1)
+        if not (
+            len(zm) == nprof + 1
+            and len(d) == nprof + 1
+            and len(rr) == nprof + 1
+            and len(v2) == nprof + 1
+            and len(psi) == nprof + 1
+        ):
+            print(len(zm), len(d), len(rr), len(v2), len(psi), nprof + 1)
             raise exceptions.AmuseException("Error in result of Poisson")
         #    // Determine statistics and characteristic scales of the King model.
-        rho0 = 1 / zm[nprof]#	 // Central density for total mass = 1
+        rho0 = 1 / zm[nprof]  # 	 // Central density for total mass = 1
         #    // Unit of velocity = sig, where rc^2 = 9 sig^2 / (4 pi G rho0)
-        sig = math.sqrt(4.0 * math.pi * rho0 / 9.0)# // This 3 was v20 in the f77 version...
-        #					 // v20 is central vel. disp. / sig^2
+        sig = math.sqrt(
+            4.0 * math.pi * rho0 / 9.0
+        )  # // This 3 was v20 in the f77 version...
+        # 					 // v20 is central vel. disp. / sig^2
         #    // Scale the zm array to unit total mass.
         inv_total_mass = 1.0 / zm[nprof]
-        zm[:] = [x*inv_total_mass for x in zm]
+        zm[:] = [x * inv_total_mass for x in zm]
         #    // Index the mass distribution, and determine the core mass and
         #    // the half-mass radius.
-        
+
         #    // By construction, rr[indx[j]] and rr[indx[j+1]] bracket the
         #    // radius containing a fraction j / NINDX of the total mass.
         self.index.append(0)
-        dz = 1.0/self.NINDX
+        dz = 1.0 / self.NINDX
         z = dz
-        for j in range(1,nprof):
-            if (rr[j] < 1): jcore = j
-            if (zm[j] < 0.5): jhalf = j
-            if (zm[j] > z):
+        for j in range(1, nprof):
+            if rr[j] < 1:
+                jcore = j
+            if zm[j] < 0.5:
+                jhalf = j
+            if zm[j] > z:
                 self.index.append(j - 1)
                 z = z + dz
         self.index.append(nprof)
-        if not (len(self.index)==self.NINDX+1):
+        if not (len(self.index) == self.NINDX + 1):
             raise exceptions.AmuseException("Error in length of indx")
-        zmcore = zm[jcore] + (zm[jcore+1] - zm[jcore]) * (1 - 
-            rr[jcore]) / (rr[jcore+1] - rr[jcore])
-        rhalf = rr[jhalf] + (rr[jhalf+1] - rr[jhalf]) * (0.5 -  
-            zm[jhalf]) / (zm[jhalf+1] - zm[jhalf])
+        zmcore = zm[jcore] + (zm[jcore + 1] - zm[jcore]) * (1 - rr[jcore]) / (
+            rr[jcore + 1] - rr[jcore]
+        )
+        rhalf = rr[jhalf] + (rr[jhalf + 1] - rr[jhalf]) * (0.5 - zm[jhalf]) / (
+            zm[jhalf + 1] - zm[jhalf]
+        )
         #    // Compute the kinetic and potential energies, and determine the
         #    // virial radius and ratio.
-        kin = 0; pot =0
+        kin = 0
+        pot = 0
         for i in range(nprof):
-            kin = kin + (zm[i+1] - zm[i]) * (v2[i+1] + v2[i])
-            pot = pot - (zm[i+1] - zm[i]) * (zm[i+1] + zm[i]) / (rr[i+1] + rr[i])
-        kin *= 0.25*sig*sig*v20
-        rvirial = -0.5/pot
+            kin = kin + (zm[i + 1] - zm[i]) * (v2[i + 1] + v2[i])
+            pot = pot - (zm[i + 1] - zm[i]) * (zm[i + 1] + zm[i]) / (rr[i + 1] + rr[i])
+        kin *= 0.25 * sig * sig * v20
+        rvirial = -0.5 / pot
         #    // Initialize the N-body system.
         if self.verbose:
-            print(" King model, w0 = ",self.W0,", Rt/Rc = ",rr[nprof],", Rh/Rc = ",rhalf,", Mc/M = ", zmcore)
+            print(
+                " King model, w0 = ",
+                self.W0,
+                ", Rt/Rc = ",
+                rr[nprof],
+                ", Rh/Rc = ",
+                rhalf,
+                ", Mc/M = ",
+                zmcore,
+            )
             #    // Write essential model information
             print("initial_mass", 1.0)
-            print("initial_rtidal_over_rvirial",  rr[nprof] / (0.25/kin))
+            print("initial_rtidal_over_rvirial", rr[nprof] / (0.25 / kin))
         #    // Assign positions and velocities. Note that it may actually
         #    // be preferable to do this in layers instead.
-        masses = numpy.zeros(self.number_of_particles) + (1.0 / self.number_of_particles)
+        masses = numpy.zeros(self.number_of_particles) + (
+            1.0 / self.number_of_particles
+        )
         positions = []
         velocities = []
-        #    // Convenient to have the "unscaled" system 
+        #    // Convenient to have the "unscaled" system
         #    // be as close to standard units as possible, so rescale position
         #    // and velocity with 'xfac' and 'vfac' to force
         #    // the virial radius to 1.  (Steve, 9/04)
-        xfac = 1.0/rvirial
-        vfac = 1.0/math.sqrt(xfac)
+        xfac = 1.0 / rvirial
+        vfac = 1.0 / math.sqrt(xfac)
         for i in range(self.number_of_particles):
             (position, potential) = self.setpos()
             velocity = self.setvel(potential)
-            #	// Unit of length = rc.
-            #	// Unit of velocity = sig.
-            position[:] = [xfac*comp for comp in position]
-            velocity[:] = [vfac*comp*sig for comp in velocity]
+            # 	// Unit of length = rc.
+            # 	// Unit of velocity = sig.
+            position[:] = [xfac * comp for comp in position]
+            velocity[:] = [vfac * comp * sig for comp in velocity]
             positions.append(position)
             velocities.append(velocity)
         #    // System is in virial equilibrium in a consistent set of units
         #    // with G, core radius, and total mass = 1.
-        
+
         return (masses, positions, velocities)
-   
+
     @property
     def result(self):
         masses, positions, velocities = self.makeking()
-        result = datamodel.Particles(self.number_of_particles)
+        result = datamodel.Particles(self.number_of_particles, **self.kwargs)
         result.mass = nbody_system.mass.new_quantity(masses)
         result.position = nbody_system.length.new_quantity(positions)
         result.velocity = nbody_system.speed.new_quantity(velocities)
         result.radius = 0 | nbody_system.length
         if self.center_model:
             result.move_to_center()
         if self.do_scale:
             result.scale_to_standard()
-        
-        if not self.convert_nbody is None:
-            result = datamodel.ParticlesWithUnitsConverted(result, self.convert_nbody.as_converter_from_si_to_generic())
+
+        if self.convert_nbody is not None:
+            result = datamodel.ParticlesWithUnitsConverted(
+                result, self.convert_nbody.as_converter_from_si_to_generic()
+            )
             result = result.copy()
-        
+
         return result
-    
+
 
 def new_king_model(number_of_particles, W0, *list_arguments, **keyword_arguments):
     """
-    Create a King model with the given number of particles and King dimensionless 
-    depth W0. Returns a set of particles with equal mass and positions and velocities 
-    distributed to fit a King distribution model. The model is centered around the 
-    origin. Positions and velocities are optionally scaled such that the kinetic and 
+    Create a King model with the given number of particles and King dimensionless
+    depth W0. Returns a set of particles with equal mass and positions and velocities
+    distributed to fit a King distribution model. The model is centered around the
+    origin. Positions and velocities are optionally scaled such that the kinetic and
     potential energies are 0.25 and -0.5 in nbody-units, respectively.
 
     :argument number_of_particles: Number of particles to include in the King model
     :argument W0: King dimensionless depth, allowed range: < 0, 16 ]
     :argument convert_nbody:  When given will convert the resulting set to SI units
     :argument do_scale: scale the result to exact nbody units (M=1, K=0.25, U=-0.5)
-    :argument beta:  Steve's rescaling parameter (< 1) [0]. Models with b > 0 are just 
-        rescaled King models; models with b < 0 approach isothermal spheres as 
+    :argument beta:  Steve's rescaling parameter (< 1) [0]. Models with b > 0 are just
+        rescaled King models; models with b < 0 approach isothermal spheres as
         b --> -infinity.
     :argument verbose: Be verbose (output is suppressed by default) [False]
     """
     uc = MakeKingModel(number_of_particles, W0, *list_arguments, **keyword_arguments)
     return uc.result
```

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/limepy.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/limepy.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/make_planets_oligarch.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/make_planets_oligarch.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/plummer.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/plummer.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,133 +2,184 @@
 Plummer model generator
 
 This module contains a function used to create Plummer (1911) models, which 
 follow a spherically symmetric density profile of the form:
 rho = c * (1 + r**2)**(-5/2)
 """
 
+from math import pi, sqrt
+
 import numpy
 import numpy.random
 
-from math import pi, sqrt
-
 from amuse.units import nbody_system
 from amuse import datamodel
 
 __all__ = ["new_plummer_sphere", "new_plummer_model"]
 
-class MakePlummerModel(object):
-    def __init__(self, number_of_particles, convert_nbody = None, radius_cutoff = 22.8042468, mass_cutoff = 0.999,
-            do_scale = False, random_state = None, random = None):
+
+class MakePlummerModel:
+    def __init__(
+        self,
+        number_of_particles,
+        convert_nbody=None,
+        radius_cutoff=22.8042468,
+        mass_cutoff=0.999,
+        do_scale=False,
+        random_state=None,
+        random=None,
+        **kwargs
+    ):
+        self.kwargs = kwargs
         self.number_of_particles = number_of_particles
         self.convert_nbody = convert_nbody
-        self.mass_cutoff = min(mass_cutoff, self.calculate_mass_cuttof_from_radius_cutoff(radius_cutoff))
+        self.mass_cutoff = min(
+            mass_cutoff, self.calculate_mass_cutoff_from_radius_cutoff(radius_cutoff)
+        )
         self.do_scale = do_scale
-        if not random_state == None:
+        if random_state is not None:
             print("DO NOT USE RANDOM STATE")
-        
+
         self.random_state = None
-        
+
         if random is None:
             self.random = numpy.random
         else:
             self.random = random
 
-    def calculate_mass_cuttof_from_radius_cutoff(self, radius_cutoff):
+    def calculate_mass_cutoff_from_radius_cutoff(self, radius_cutoff):
         if radius_cutoff > 99999:
             return 1.0
         scale_factor = 16.0 / (3.0 * pi)
         rfrac = radius_cutoff * scale_factor
-        denominator = pow(1.0 + rfrac ** 2, 1.5)
-        numerator = rfrac ** 3
-        return numerator/denominator
+        denominator = pow(1.0 + rfrac**2, 1.5)
+        numerator = rfrac**3
+        return numerator / denominator
 
     def calculate_radius(self, index):
         mass_min = (index * self.mass_cutoff) / self.number_of_particles
-        mass_max = ((index+1) * self.mass_cutoff) / self.number_of_particles
+        mass_max = ((index + 1) * self.mass_cutoff) / self.number_of_particles
         random_mass_fraction = self.random.uniform(mass_min, mass_max)
-        radius = 1.0 / sqrt( pow (random_mass_fraction, -2.0/3.0) - 1.0)
+        radius = 1.0 / sqrt(pow(random_mass_fraction, -2.0 / 3.0) - 1.0)
         return radius
 
     def calculate_radius_uniform_distribution(self):
-        return 1.0 /  numpy.sqrt( numpy.power(self.random.uniform(0,self.mass_cutoff,(self.number_of_particles,1)), -2.0/3.0) - 1.0)
+        return 1.0 / numpy.sqrt(
+            numpy.power(
+                self.random.uniform(0, self.mass_cutoff, (self.number_of_particles, 1)),
+                -2.0 / 3.0,
+            )
+            - 1.0
+        )
 
     def new_positions_spherical_coordinates(self):
         pi2 = pi * 2
         radius = self.calculate_radius_uniform_distribution()
-        theta = numpy.arccos(self.random.uniform(-1.0,1.0, (self.number_of_particles,1)))
-        phi = self.random.uniform(0.0,pi2, (self.number_of_particles,1))
-        return (radius,theta,phi)
+        theta = numpy.arccos(
+            self.random.uniform(-1.0, 1.0, (self.number_of_particles, 1))
+        )
+        phi = self.random.uniform(0.0, pi2, (self.number_of_particles, 1))
+        return (radius, theta, phi)
 
     def new_velocities_spherical_coordinates(self, radius):
         pi2 = pi * 2
-        x,y = self.new_xy_for_velocity()
-        velocity = x * sqrt(2.0) * numpy.power( 1.0 + radius*radius, -0.25)
-        theta = numpy.arccos(self.random.uniform(-1.0,1.0, (self.number_of_particles,1)))
-        phi = self.random.uniform(0.0,pi2, (self.number_of_particles,1))
-        return (velocity,theta,phi)
+        x, y = self.new_xy_for_velocity()
+        velocity = x * sqrt(2.0) * numpy.power(1.0 + radius * radius, -0.25)
+        theta = numpy.arccos(
+            self.random.uniform(-1.0, 1.0, (self.number_of_particles, 1))
+        )
+        phi = self.random.uniform(0.0, pi2, (self.number_of_particles, 1))
+        return (velocity, theta, phi)
 
     def coordinates_from_spherical(self, radius, theta, phi):
-        x = radius * numpy.sin( theta ) * numpy.cos( phi )
-        y = radius * numpy.sin( theta ) * numpy.sin( phi )
-        z = radius * numpy.cos( theta )
-        return (x,y,z)
+        x = radius * numpy.sin(theta) * numpy.cos(phi)
+        y = radius * numpy.sin(theta) * numpy.sin(phi)
+        z = radius * numpy.cos(theta)
+        return (x, y, z)
 
     def new_xy_for_velocity(self):
         number_of_selected_items = 0
         selected_values_for_x = numpy.zeros(0)
         selected_values_for_y = numpy.zeros(0)
-        while (number_of_selected_items < self.number_of_particles):
-            x = self.random.uniform(0,1.0, (self.number_of_particles-number_of_selected_items))
-            y = self.random.uniform(0,0.1, (self.number_of_particles-number_of_selected_items))
+        while number_of_selected_items < self.number_of_particles:
+            x = self.random.uniform(
+                0, 1.0, (self.number_of_particles - number_of_selected_items)
+            )
+            y = self.random.uniform(
+                0, 0.1, (self.number_of_particles - number_of_selected_items)
+            )
             g = (x**2) * numpy.power(1.0 - x**2, 3.5)
             compare = y <= g
-            selected_values_for_x = numpy.concatenate((selected_values_for_x, x.compress(compare)))
-            selected_values_for_y= numpy.concatenate((selected_values_for_x, y.compress(compare)))
+            selected_values_for_x = numpy.concatenate(
+                (selected_values_for_x, x.compress(compare))
+            )
+            selected_values_for_y = numpy.concatenate(
+                (selected_values_for_x, y.compress(compare))
+            )
             number_of_selected_items = len(selected_values_for_x)
-        return numpy.atleast_2d(selected_values_for_x).transpose(), numpy.atleast_2d(selected_values_for_y).transpose()
+        return (
+            numpy.atleast_2d(selected_values_for_x).transpose(),
+            numpy.atleast_2d(selected_values_for_y).transpose(),
+        )
 
     def new_model(self):
-        m = numpy.zeros((self.number_of_particles,1)) + (1.0 / self.number_of_particles)
+        m = numpy.zeros((self.number_of_particles, 1)) + (
+            1.0 / self.number_of_particles
+        )
         radius, theta, phi = self.new_positions_spherical_coordinates()
-        position =  numpy.hstack(self.coordinates_from_spherical(radius, theta, phi))
+        position = numpy.hstack(self.coordinates_from_spherical(radius, theta, phi))
         radius, theta, phi = self.new_velocities_spherical_coordinates(radius)
         velocity = numpy.hstack(self.coordinates_from_spherical(radius, theta, phi))
         position = position / 1.695
         velocity = velocity / sqrt(1 / 1.695)
         return (m, position, velocity)
 
     @property
     def result(self):
         masses = numpy.ones(self.number_of_particles) / self.number_of_particles
         radius, theta, phi = self.new_positions_spherical_coordinates()
-        x,y,z =  self.coordinates_from_spherical(radius, theta, phi)
+        x, y, z = self.coordinates_from_spherical(radius, theta, phi)
         radius, theta, phi = self.new_velocities_spherical_coordinates(radius)
-        vx,vy,vz = self.coordinates_from_spherical(radius, theta, phi)
- 
-        result = datamodel.Particles(self.number_of_particles)
+        vx, vy, vz = self.coordinates_from_spherical(radius, theta, phi)
+
+        result = datamodel.Particles(self.number_of_particles, **self.kwargs)
         result.mass = nbody_system.mass.new_quantity(masses)
-        result.x = nbody_system.length.new_quantity(x.reshape(self.number_of_particles)/1.695)
-        result.y = nbody_system.length.new_quantity(y.reshape(self.number_of_particles)/1.695)
-        result.z = nbody_system.length.new_quantity(z.reshape(self.number_of_particles)/1.695)
-        result.vx = nbody_system.speed.new_quantity(vx.reshape(self.number_of_particles) / sqrt(1/1.695))
-        result.vy = nbody_system.speed.new_quantity(vy.reshape(self.number_of_particles) / sqrt(1/1.695))
-        result.vz = nbody_system.speed.new_quantity(vz.reshape(self.number_of_particles) / sqrt(1/1.695))
+        result.x = nbody_system.length.new_quantity(
+            x.reshape(self.number_of_particles) / 1.695
+        )
+        result.y = nbody_system.length.new_quantity(
+            y.reshape(self.number_of_particles) / 1.695
+        )
+        result.z = nbody_system.length.new_quantity(
+            z.reshape(self.number_of_particles) / 1.695
+        )
+        result.vx = nbody_system.speed.new_quantity(
+            vx.reshape(self.number_of_particles) / sqrt(1 / 1.695)
+        )
+        result.vy = nbody_system.speed.new_quantity(
+            vy.reshape(self.number_of_particles) / sqrt(1 / 1.695)
+        )
+        result.vz = nbody_system.speed.new_quantity(
+            vz.reshape(self.number_of_particles) / sqrt(1 / 1.695)
+        )
         result.radius = 0 | nbody_system.length
 
         result.move_to_center()
         if self.do_scale:
             result.scale_to_standard()
 
-        if not self.convert_nbody is None:
-            result = datamodel.ParticlesWithUnitsConverted(result, self.convert_nbody.as_converter_from_si_to_generic())
+        if self.convert_nbody is not None:
+            result = datamodel.ParticlesWithUnitsConverted(
+                result, self.convert_nbody.as_converter_from_si_to_generic()
+            )
             result = result.copy()
 
         return result
 
+
 def new_plummer_model(number_of_particles, *list_arguments, **keyword_arguments):
     """
     Create a plummer sphere with the given number of particles. Returns
     a set of stars with equal mass and positions and velocities distributed
     to fit a plummer star distribution model. The model is centered around the
     origin. Positions and velocities are optionally scaled such that the kinetic and
     potential energies are 0.25 and -0.5 in nbody-units, respectively.
@@ -138,8 +189,9 @@
     :argument radius_cutoff: Cutoff value for the radius (defaults to 22.8042468)
     :argument mass_cutoff: Mass percentage inside radius of 1
     :argument do_scale: scale the result to exact nbody units (M=1, K=0.25, U=-0.5)
     """
     uc = MakePlummerModel(number_of_particles, *list_arguments, **keyword_arguments)
     return uc.result
 
+
 new_plummer_sphere = new_plummer_model
```

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/salpeter.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/salpeter.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/ic/solar_system_moons.py` & `amuse_framework-2024.4.0rc1/src/amuse/ic/solar_system_moons.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/__init__.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/base.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/base.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/fi_io.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/fi_io.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/gadget.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/gadget.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/horizons.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/horizons.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/nemobin.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/nemobin.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/nemotsf.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/nemotsf.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/p10.txt` & `amuse_framework-2024.4.0rc1/src/amuse/io/p10.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/phigrape.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/phigrape.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/starlab.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/starlab.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         xml_string = x.convert_starlab_string_to_xml_string(string)
         xml2particles = Xml2Particles()
         xml2particles.dynamics_mass_units = self.dynamics_mass_units
         xml2particles.dynamics_time_units = self.dynamics_time_units
         xml2particles.dynamics_length_units = self.dynamics_length_units
         xml2particles.parse_xml(xml_string)
         unit_converter = None
-        if not self.nbody_to_si_converter is None:
+        if self.nbody_to_si_converter is not None:
             unit_converter = self.nbody_to_si_converter
         elif self.must_scale:
             if not self._is_valid_scaling_factor(xml2particles.mass_scale):
                 unit_converter = None
             elif not self._is_valid_scaling_factor(xml2particles.time_scale):
                 unit_converter = nbody_system.nbody_to_si(
                     (1.0 / xml2particles.mass_scale) | units.MSun,
```

### Comparing `amuse-framework-2023.5.0/src/amuse/io/store.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/store.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/store_v1.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/store_v1.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/store_v2.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/store_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -736,19 +736,19 @@
                     os.remove(filename)
                 else:
                     raise FileExistsError("Opening file for write with overwrite_file is False but file {0} exists".format(filename))
 
         if append_to_file:
             if os.access(filename, os.F_OK) and not os.access(filename, os.W_OK):
                    raise Exception("Opening file for append but file {0} is not writeable".format(filename))
-            self.hdf5file = h5py.File(filename,'a')
+            self.hdf5file = h5py.File(filename,'a',libver='latest')
         elif open_for_writing:
-            self.hdf5file = h5py.File(filename,'w')
+            self.hdf5file = h5py.File(filename,'w',libver='latest')
         else:
-            self.hdf5file = h5py.File(filename,'r')
+            self.hdf5file = h5py.File(filename,'r',libver='latest')
         
         self.copy_history = copy_history
         self.mapping_from_groupid_to_set = {}
         
         #warnings.warn("amuse hdf storage version 2.0 is still in development, do not use it for production scripts")
         
     def is_correct_version(self):
```

### Comparing `amuse-framework-2023.5.0/src/amuse/io/text.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/text.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/io/vtk.py` & `amuse_framework-2024.4.0rc1/src/amuse/io/vtk.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/lab.py` & `amuse_framework-2024.4.0rc1/src/amuse/lab.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/plot/_plot.py` & `amuse_framework-2024.4.0rc1/src/amuse/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/plot/hydro.py` & `amuse_framework-2024.4.0rc1/src/amuse/plot/hydro.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/plot/mapper.py` & `amuse_framework-2024.4.0rc1/src/amuse/plot/mapper.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/async_request.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/async_request.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/channel.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,17 @@
     from amuse import config
 except ImportError:
     config = None
     
 from amuse.support.options import OptionalAttributes, option, GlobalOptions
 from amuse.support.core import late
 from amuse.support import exceptions
-from amuse.support import get_amuse_root_dir
+from amuse.support import get_amuse_root_dir, get_amuse_package_dir
 from amuse.rfi import run_command_redirected
+from amuse.config import parse_configmk_lines
 
 from amuse.rfi import slurm
 
 from . import async_request
 
 class AbstractMessage(object):
     
@@ -505,17 +506,18 @@
         arguments.append(full_name_of_the_worker)
         
         command = 'xterm'
         return command, arguments
         
 
     @classmethod
-    def REDIRECT(cls, full_name_of_the_worker, stdoutname, stderrname, command=None, interpreter_executable=None, **options):
+    def REDIRECT(cls, full_name_of_the_worker, stdoutname, stderrname, command=None, 
+                      interpreter_executable=None, run_command_redirected_file=None  ):
         
-        fname = run_command_redirected.__file__                
+        fname = run_command_redirected_file or run_command_redirected.__file__                
         arguments = [fname , stdoutname, stderrname]
         
         if not interpreter_executable is None:
             arguments.append(interpreter_executable)
             
         arguments.append(full_name_of_the_worker)
         
@@ -802,14 +804,16 @@
                         dtype_to_result[datatype][j][ndone:ndone+self.max_message_length] = element
                 
             ndone+=self.max_message_length
         
         self._communicated_splitted_message = True
         self._merged_results_splitted_message = dtype_to_result
 
+    def makedirs(self,directory):
+        os.makedirs(directory)
 
 
 AbstractMessageChannel.DEBUGGERS = {
     "none":None,
     "gdb":AbstractMessageChannel.GDB,
     "lldb":AbstractMessageChannel.LLDB,
     "ddd":AbstractMessageChannel.DDD,
@@ -1243,25 +1247,19 @@
     def __setstate__(self, state):
         self.info = MPI.INFO_NULL
         self.cached = None
         self.intercomm = None
         self._is_inuse = False
         self._communicated_splitted_message = False
         self.inuse_semaphore = threading.Semaphore()
-        
-
-
 
     @option(sections=("channel",))
     def job_scheduler(self):
         """Name of the job scheduler to use when starting the code, if given will use job scheduler to find list of hostnames for spawning"""
         return ""
-        
-
-
 
     def get_info_from_job_scheduler(self, name, number_of_workers = 1):
         if name == "slurm":
             return self.get_info_from_slurm(number_of_workers)
         return MPI.INFO_NULL
 
     @classmethod
@@ -1273,29 +1271,29 @@
             nodelist = slurm.parse_slurm_nodelist(os.environ['SLURM_NODELIST'])
             tasks_per_node = slurm.parse_slurm_tasks_per_node(os.environ['SLURM_TASKS_PER_NODE'])
             all_nodes = []
             for node, tasks in zip(nodelist, tasks_per_node):
                 for _ in range(tasks):
                     all_nodes.append(node)
             cls._scheduler_nodes = all_nodes
-            cls._scheduler_index = 1     # start at 1 assumes that the python script is running on the first node as the first task
+            cls._scheduler_index = 1  # start at 1 assumes that the python script is running on the first node as the first task
             cls._scheduler_initialized = True
             print("NODES:", cls._scheduler_nodes)
         hostnames = []
         count = 0
         while count < number_of_workers:
                 hostnames.append(cls._scheduler_nodes[cls._scheduler_index])
                 count += 1
                 cls._scheduler_index += 1
                 if cls._scheduler_index >= len(cls._scheduler_nodes):
                     cls._scheduler_index  = 0
         host = ','.join(hostnames)
         print("HOST:", host, cls._scheduler_index, os.environ['SLURM_TASKS_PER_NODE'])
         info = MPI.Info.Create()
-        info['host'] = host                                                     #actually in mpich and openmpi, the host parameter is interpreted as a comma separated list of host names,
+        info['host'] = host   # actually in mpich and openmpi, the host parameter is interpreted as a comma separated list of host names,
         return info
 
 
 
 class MultiprocessingMPIChannel(AbstractMessageChannel):
     """
     Message channel based on JSON messages. 
@@ -1469,29 +1467,25 @@
     def _extra_path_item(self, path_of_the_module):
         result = ''
         for x in sys.path:
             if path_of_the_module.startswith(x):
                 if len(x) > len(result):
                     result = x
         return result
-        
-            
-
 
     @option(choices=AbstractMessageChannel.DEBUGGERS.keys(), sections=("channel",))
     def debugger(self):
         """Name of the debugger to use when starting the code"""
         return "none"
-    
-    
 
     @option(type="boolean")
     def check_mpi(self):
         return True
 
+
 class SocketMessage(AbstractMessage):
       
     def _receive_all(self, nbytes, thesocket):
 
         # logger.debug("receiving %d bytes", nbytes)
         
         result = []
@@ -1675,15 +1669,14 @@
         self.send_floats(socket, self.floats)
         self.send_doubles(socket, self.doubles)
         self.send_booleans(socket, self.booleans)
         self.send_strings(socket, self.strings)
         self.send_doubles(socket, self.encoded_units)
         
         # logger.debug("message send")
-    
 
     def send_doubles(self, socket, array):
         if len(array) > 0:
             data_buffer = numpy.array(array, dtype='f8')
             socket.sendall(data_buffer.tobytes())
             
     def send_ints(self, socket, array):
@@ -1713,62 +1706,66 @@
             data_buffer = numpy.array(array, dtype='b')
             socket.sendall(data_buffer.tobytes())
 
     def send_longs(self, socket, array):
         if len(array) > 0:
             data_buffer = numpy.array(array, dtype='int64')
             socket.sendall(data_buffer.tobytes())
-        
+
+
 class SocketChannel(AbstractMessageChannel):
     
-    def __init__(self, name_of_the_worker, legacy_interface_type=None, interpreter_executable=None, **options):
+    def __init__(self, name_of_the_worker, legacy_interface_type=None, interpreter_executable=None, 
+          remote_env=None, **options):
         AbstractMessageChannel.__init__(self, **options)
         
         #logging.getLogger().setLevel(logging.DEBUG)
         
         logger.debug("initializing SocketChannel with options %s", options)
         
         # self.name_of_the_worker = name_of_the_worker + "_sockets"
         self.name_of_the_worker = name_of_the_worker
 
         self.interpreter_executable = interpreter_executable
-        
-        if self.hostname != None and self.hostname not in ['localhost',socket.gethostname()]:
-            raise exceptions.CodeException("can only run codes on local machine using SocketChannel, not on %s", self.hostname)
-            
+                
+        if self.hostname == None:
+            self.hostname="localhost"
+
+        if self.hostname not in ['localhost',socket.gethostname()]:
+            self.remote=True
+            self.must_check_if_worker_is_up_to_date=False
+        else:
+            self.remote=False
+                    
         self.id = 0
         
         if not legacy_interface_type is None:
             self.full_name_of_the_worker = self.get_full_name_of_the_worker(legacy_interface_type)
         else:
             self.full_name_of_the_worker = self.name_of_the_worker
             
         logger.debug("full name of worker is %s", self.full_name_of_the_worker)
         
         self._is_inuse = False
         self._communicated_splitted_message = False
         self.socket = None
     
-    
+        self.remote_env=remote_env
 
     @option(sections=("channel",))
     def mpiexec(self):
         """mpiexec with arguments"""
         if len(config.mpi.mpiexec):
             return config.mpi.mpiexec
         return ''
 
     @option(sections=("channel",))
     def mpiexec_number_of_workers_flag(self):
         """flag to use, so that the number of workers are defined"""
         return '-n'
-    
-
-    
-
 
     @late
     def debugger_method(self):
         return self.DEBUGGERS[self.debugger]
     
     def accept_worker_connection(self, server_socket, process):
         #wait for the worker to connect. check if the process is still running once in a while
@@ -1783,36 +1780,17 @@
                 #update and read returncode
                 if process.poll() is not None:
                     raise exceptions.CodeException('could not connect to worker, worker process terminated')
                 #logger.error("worker not connecting, waiting...")
                 
         raise exceptions.CodeException('worker still not started after 60 seconds')
 
-    
-
-    def start(self):
-        server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        
-        server_socket.bind(('', 0))
-        server_socket.settimeout(1.0)
-        server_socket.listen(1)
-        
-        logger.debug("starting socket worker process, listening for worker connection on %s", server_socket.getsockname())
-
-        #this option set by CodeInterface
-        logger.debug("mpi_enabled: %s", str(self.initialize_mpi))
-        
-        # set arguments to name of the worker, and port number we listen on 
-
-
-        self.stdout = None
-        self.stderr = None
-        
+    def generate_command_and_arguments(self,server_address,port):
         arguments = []
-        
+                
         if not self.debugger_method is None:
             command, arguments = self.debugger_method(self.full_name_of_the_worker, self, interpreter_executable=self.interpreter_executable)
         else:
             if self.redirect_stdout_file == 'none' and self.redirect_stderr_file == 'none':
                 
                 if self.interpreter_executable is None:
                     command = self.full_name_of_the_worker
@@ -1831,33 +1809,160 @@
             # prepend with mpiexec and arguments back to front
             arguments.insert(0, str(self.number_of_workers))
             arguments.insert(0, self.mpiexec_number_of_workers_flag)
             arguments[:0] = mpiexec
             command = mpiexec[0]
 
             #append with port and hostname where the worker should connect            
-            arguments.append(str(server_socket.getsockname()[1]))
+            arguments.append(port)
             #hostname of this machine
-            arguments.append(str(socket.gethostname()))
-        
+            arguments.append(server_address)
+            
             #initialize MPI inside worker executable
             arguments.append('true')
         else:
             #append arguments with port and socket where the worker should connect            
-            arguments.append(str(server_socket.getsockname()[1]))
+            arguments.append(port)
             #local machine
-            arguments.append('localhost')
+            arguments.append(server_address)
         
             #do not initialize MPI inside worker executable
             arguments.append('false')
+
+        return command,arguments
+
+    def remote_env_string(self, hostname):
+        if self.remote_env is None:
+          if hostname in self.remote_envs.keys():
+            return "source "+self.remote_envs[hostname]+"\n"
+          else:
+            return ""
+        else:
+          return "source "+self.remote_env +"\n"
+
+    def generate_remote_command_and_arguments(self,hostname, server_address,port):
+        
+        # get remote config
+        args=["ssh","-T", hostname]
+
+        command=self.remote_env_string(self.hostname)+ \
+                "amusifier --get-amuse-config" +"\n"
+      
+        proc=Popen(args,stdout=PIPE, stdin=PIPE, executable="ssh")
+        out,err=proc.communicate(command.encode())
+
+        try:
+            remote_config=parse_configmk_lines(out.decode().split("\n"),"remote config at "+self.hostname )
+        except:
+            raise Exception(f"failed getting remote config from {self.hostname} - please check remote_env argument ({self.remote_env})")
+
+        # get remote amuse package dir
+        command=self.remote_env_string(self.hostname)+ \
+                "amusifier --get-amuse-package-dir" +"\n"
+      
+        proc=Popen(args,stdout=PIPE, stdin=PIPE, executable="ssh")
+        out,err=proc.communicate(command.encode())
+      
+        remote_package_dir=out.decode().strip(" \n\t")
+        local_package_dir=get_amuse_package_dir()
+                
+        mpiexec=remote_config["MPIEXEC"]
+        initialize_mpi=remote_config["MPI_ENABLED"] == 'yes'
+        run_command_redirected_file=run_command_redirected.__file__.replace(local_package_dir,remote_package_dir)
+        interpreter_executable=None if self.interpreter_executable==None else remote_config["PYTHON"]
+        # dynamic python workers? (should be send over)
+        full_name_of_the_worker=self.full_name_of_the_worker.replace(local_package_dir,remote_package_dir)
+        python_exe_for_redirection=remote_config["PYTHON"]
+
+        if not self.debugger_method is None:
+            raise Exception("remote socket channel debugging not yet supported")
+            #command, arguments = self.debugger_method(self.full_name_of_the_worker, self, interpreter_executable=self.interpreter_executable)
+        else:
+            if self.redirect_stdout_file == 'none' and self.redirect_stderr_file == 'none':
+                
+                if interpreter_executable is None:
+                    command = full_name_of_the_worker
+                    arguments = []
+                else:
+                    command = interpreter_executable
+                    arguments = [full_name_of_the_worker]
+            else:
+                command, arguments = self.REDIRECT(full_name_of_the_worker, self.redirect_stdout_file, 
+                  self.redirect_stderr_file, command=python_exe_for_redirection, 
+                  interpreter_executable=interpreter_executable, 
+                  run_command_redirected_file=run_command_redirected_file)
+
+        #start arguments with command        
+        arguments.insert(0, command)
+
+        if initialize_mpi and len(mpiexec) > 0:
+            mpiexec = shlex.split(mpiexec)
+            # prepend with mpiexec and arguments back to front
+            arguments.insert(0, str(self.number_of_workers))
+            arguments.insert(0, self.mpiexec_number_of_workers_flag)
+            arguments[:0] = mpiexec
+            command = mpiexec[0]
+
+            #append with port and hostname where the worker should connect            
+            arguments.append(port)
+            #hostname of this machine
+            arguments.append(server_address)
             
-        logger.debug("starting process with command `%s`, arguments `%s` and environment '%s'", command, arguments, os.environ)
-        self.process = Popen(arguments, executable=command, stdin=PIPE, stdout=None, stderr=None, close_fds=self.close_fds)
-        logger.debug("waiting for connection from worker")
+            #initialize MPI inside worker executable
+            arguments.append('true')
+        else:
+            #append arguments with port and socket where the worker should connect            
+            arguments.append(port)
+            #local machine
+            arguments.append(server_address)
+        
+            #do not initialize MPI inside worker executable
+            arguments.append('false')
+
+        return command,arguments
 
+    def start(self):
+        
+        server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                
+        server_address=self.get_host_ip(self.hostname)
+                
+        server_socket.bind((server_address , 0))
+        server_socket.settimeout(1.0)
+        server_socket.listen(1)
+        
+        logger.debug("starting socket worker process, listening for worker connection on %s", server_socket.getsockname())
+
+        #this option set by CodeInterface
+        logger.debug("mpi_enabled: %s", str(self.initialize_mpi))
+        
+        # set arguments to name of the worker, and port number we listen on 
+
+        self.stdout = None
+        self.stderr = None
+        
+        if self.remote:
+            command,arguments=self.generate_remote_command_and_arguments(self.hostname,server_address,str(server_socket.getsockname()[1]))
+        else:
+            command,arguments=self.generate_command_and_arguments(server_address,str(server_socket.getsockname()[1]))
+                    
+        if self.remote:
+          logger.debug("starting remote process on %s with command `%s`, arguments `%s` and environment '%s'", self.hostname, command, arguments, os.environ)
+          ssh_command=self.remote_env_string(self.hostname)+" ".join(arguments)
+          arguments=["ssh","-T", self.hostname]
+          command="ssh"
+          self.process = Popen(arguments, executable=command, stdin=PIPE, stdout=None, stderr=None, close_fds=self.close_fds)
+          self.process.stdin.write(ssh_command.encode())
+          self.process.stdin.close()
+        else:
+          logger.debug("starting process with command `%s`, arguments `%s` and environment '%s'", command, arguments, os.environ)
+          # ~ print(arguments)
+          self.process = Popen(arguments, executable=command, stdin=PIPE, stdout=None, stderr=None, close_fds=self.close_fds)
+
+        logger.debug("waiting for connection from worker")
         self.socket, address = self.accept_worker_connection(server_socket, self.process)
         
         self.socket.setblocking(1)
         
         self.socket.setsockopt(socket.SOL_TCP, socket.TCP_NODELAY, 1)
         
         server_socket.close()
@@ -1866,15 +1971,20 @@
         
         # logger.info("worker %s initialized", self.name_of_the_worker)
         
 
     @option(type="boolean", sections=("sockets_channel",))
     def close_fds(self):
         """close open file descriptors when spawning child process"""
-        return True
+        return False
+
+    @option(type="dict", sections=("sockets_channel",))
+    def remote_envs(self):
+        """ dict of remote machine - enviroment (source ..)  pairs """
+        return dict()
 
     @option(choices=AbstractMessageChannel.DEBUGGERS.keys(), sections=("channel",))
     def debugger(self):
         """Name of the debugger to use when starting the code"""
         return "none"
         
     @option(sections=("channel",))
@@ -1885,14 +1995,17 @@
         if (self.socket == None):
             return
         
         logger.debug("stopping socket worker %s", self.name_of_the_worker)
         self.socket.close()
         
         self.socket = None
+
+        if not self.process.stdin is None:
+            self.process.stdin.close()
         
         # should lookinto using poll with a timeout or some other mechanism
         # when debugger method is on, no killing
         count = 0
         while(count < 5):
             returncode = self.process.poll()
             if not returncode is None:
@@ -1948,28 +2061,25 @@
         if call_count > self.max_message_length:
             self.split_message(call_id, function_id, call_count, dtype_to_arguments, encoded_units)
         else:
             message = SocketMessage(call_id, function_id, call_count, dtype_to_arguments, encoded_units = encoded_units)
             message.send(self.socket)
 
             self._is_inuse = True
-        
-
 
     def recv_message(self, call_id, function_id, handle_as_array, has_units=False):
            
         self._is_inuse = False
         
         if self._communicated_splitted_message:
             x = self._merged_results_splitted_message
             self._communicated_splitted_message = False
             del self._merged_results_splitted_message
             return x
         
-        
         message = SocketMessage()
         
         message.receive(self.socket)
 
         if message.error:
             error_message=message.strings[0] if len(message.strings)>0 else "no error message"
             if message.call_id != call_id or message.function_id != function_id:
@@ -1984,16 +2094,14 @@
             self.stop()
             raise exceptions.CodeException('Received reply for function id {0} but expected {1}'.format(message.function_id, function_id))
         
         if has_units:
             return message.to_result(handle_as_array), message.encoded_units
         else:
             return message.to_result(handle_as_array)
-        
-
 
     def nonblocking_recv_message(self, call_id, function_id, handle_as_array, has_units=False):
         request = SocketMessage().nonblocking_receive(self.socket)
     
         def handle_result(function):
             self._is_inuse = False
     
@@ -2027,14 +2135,35 @@
     def max_message_length(self):
         """
         For calls to functions that can handle arrays, MPI messages may get too long for large N.
         The MPI channel will split long messages into blocks of size max_message_length.
         """     
         return 1000000
 
+    def sanitize_host(self,hostname):
+        if "@" in hostname:
+          return hostname.split("@")[1]
+        return hostname
+    
+    def get_host_ip(self, client):
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        s.connect((self.sanitize_host(client), 80))
+        ip=s.getsockname()[0]
+        s.close()
+        return ip
+
+    def makedirs(self,directory):
+      if self.remote:
+        args=["ssh","-T", self.hostname]
+        command=f"mkdir -p {directory}\n"
+        proc=Popen(args,stdout=PIPE, stdin=PIPE, executable="ssh")
+        out,err=proc.communicate(command.encode())
+      else:
+        os.makedirs(directory)
+
 
 class OutputHandler(threading.Thread):
     
     def __init__(self, stream, port):
         threading.Thread.__init__(self)
         self.stream = stream
 
@@ -2074,14 +2203,15 @@
                 # logger.debug("end of output", len(data))
                 return
             
             # logger.debug("got %d bytes", len(data))
             
             self.stream.write(data)
 
+
 class DistributedChannel(AbstractMessageChannel):
             
     default_distributed_instance = None
     
     @staticmethod
     def getStdoutID(instance):
         if not hasattr(instance, "_stdoutHandler") or instance._stdoutHandler is None:
@@ -2157,16 +2287,14 @@
             
         logger.debug("executable is %s", self.executable)
         logger.debug("full name of the worker is %s", self.full_name_of_the_worker)
         
         logger.debug("worker dir is %s", self.worker_dir)
             
         self._is_inuse = False
-      
-
 
     def check_if_worker_is_up_to_date(self, object):
 #         if self.hostname != 'localhost':
 #             return
 #         
 #         logger.debug("hostname = %s, checking for worker", self.hostname)
 #
```

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/core.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -956,15 +956,17 @@
         return True
     
     @late
     def channel_factory(self):
         if self.channel_type == 'mpi':
             if  MpiChannel.is_supported():
                 return MpiChannel
-            else:   
+            else:
+                warnings.warn("MPI (unexpectedly?) not available, falling back to sockets channel")
+                self.channel_type="sockets"   
                 return SocketChannel
                 
         elif self.channel_type == 'remote':
             return MultiprocessingMPIChannel
         elif self.channel_type == 'distributed':
             return DistributedChannel
         elif self.channel_type == 'sockets':
@@ -1060,23 +1062,25 @@
         function.internal_provided=True
         return function
 
 class CodeWithDataDirectories(object):
     
     
     def __init__(self):
-        if not self.channel_type == 'distributed':
+        if self.channel_type == 'distributed':
+            warnings.warn("Code with DistributedChannel wants to make output directory, check..")
+        else:
             self.ensure_data_directory_exists(self.get_output_directory())
     
     def ensure_data_directory_exists(self, directory):
         directory = os.path.expanduser(directory)
         directory = os.path.expandvars(directory)
-        
+                
         try:
-            os.makedirs(directory)
+            self.channel.makedirs(directory)
         except OSError as ex:
             if ex.errno == errno.EEXIST and os.path.isdir(directory):
                 pass
             else:
                 raise ex
 
     @property
```

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/gencode.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/gencode.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,398 +3,456 @@
 import os
 
 from optparse import OptionParser
 
 # Should probably use an absolute import here (support.config), but
 # we're not guaranteed this script will always be in a support
 # subdirectory with an __init__.py file.
-#try:  # running as a module
+# try:  # running as a module
 #    from . import config
-#except (ImportError, ValueError):  # running as a stand-alone script
+# except (ImportError, ValueError):  # running as a stand-alone script
 #    import config
 
 # setup_sys_path()
 
 # this should not be necessary?
-sys.path.insert(0,os.getcwd())
+sys.path.insert(0, os.getcwd())
 
 from amuse import config
 
 from amuse.rfi.tools import create_c
 from amuse.rfi.tools import create_fortran
 from amuse.rfi.tools import create_java
 from amuse.rfi.tools import create_dir
 from amuse.rfi.tools import create_python_worker
-    
-from amuse.support import get_amuse_root_dir    
-from amuse.support.literature import TrackLiteratureReferences    
+
+from amuse.support import get_amuse_root_dir, get_amuse_package_dir
+from amuse.support.literature import TrackLiteratureReferences
+
 
 def get_amuse_directory():
     filename_of_this_script = __file__
     directory_of_this_script = os.path.dirname(os.path.dirname(filename_of_this_script))
-    directory_of_this_script = os.path.join(directory_of_this_script, 'build', 'lib')
+    directory_of_this_script = os.path.join(directory_of_this_script, "build", "lib")
     if os.path.isabs(directory_of_this_script):
         return directory_of_this_script
     else:
         return os.path.abspath(directory_of_this_script)
 
 # in case of trouble consult old python 2:     
     #~ def get_amuse_directory():
         #~ filename_of_this_script = __file__
         #~ directory_of_this_script = os.path.dirname(os.path.dirname(filename_of_this_script))
         #~ if os.path.isabs(directory_of_this_script):
             #~ return directory_of_this_script
         #~ else:
             #~ return os.path.abspath(directory_of_this_script)
 
-def get_amuse_directory_root():
-    filename_of_this_script = __file__
-    directory_of_this_script = os.path.dirname(os.path.dirname(filename_of_this_script))
-    if os.path.isabs(directory_of_this_script):
-        return directory_of_this_script
-    else:
-        return os.path.abspath(directory_of_this_script)
-
 def setup_sys_path():
     amuse_directory = os.environ["AMUSE_DIR"]
     sys.path.insert(0, amuse_directory)
     try:
-      src_root_directory = os.environ["MUSE_PACKAGE_DIR"]
-      sys.path.insert(0, src_root_directory)
+        src_root_directory = os.environ["MUSE_PACKAGE_DIR"]
+        sys.path.insert(0, src_root_directory)
     except:
-      src_root_directory = amuse_directory
-    sys.path.insert(0, os.path.join(src_root_directory,"src"))
+        src_root_directory = amuse_directory
+    sys.path.insert(0, os.path.join(src_root_directory, "src"))
     sys.path.append(os.getcwd())
 
+
 class ParseCommandLine(object):
     usage = """usage: %prog [options] name_of_module name_of_class_in_module.
-    
+
     or: %prog --mode=dir name_of_the_code
-    
-    This script will generate code from the class with name <name_of_class_in_module>. The
-    class must be defined in the module <name_of_module>. The module name
-    can be a python file or the python module name.
-    
+
+    This script will generate code from the class with name
+    <name_of_class_in_module>. The class must be defined in the module
+    <name_of_module>. The module name can be a python file or the python module
+    name.
+
     If mode is dir the script will create a directory with all files
     needed to start creating a code interface.
-    
+
     This script handles all code generation for the AMUSE framework. It can
-    be used to create C++ or Fortran code to handle the MPI messages, 
+    be used to create C++ or Fortran code to handle the MPI messages,
     create a header file or create stub code as a start for defining
     the interface between the code and AMUSE.
-    
+
     Examples
     --------
     To generate code for interfacing with MPI do:
         %prog --type=c --mode=mpi test.py TestInterface
     or (for fortran):
         %prog --type=f90 --mode=mpi test.py TestInterface
-        
+
     To generate a header file do (for C):
         %prog --type=h test.py TestInterface
     or (for C++):
         %prog --type=H test.py TestInterface
-        
+
     To generate a stub file do:
         %prog --type=c --mode=stub test.py TestInterface
     or (for fortran):
         %prog --type=f90 --mode=stub test.py TestInterface
-        
+
     To generate create a directory and put files in it do:
         %prog --type=c --mode=dir MyCode
     or (for fortran):
         %prog --type=f90 --mode=dir MyCode
-    
+
     To see a description of all arguments do:
         %prog --help
-    
+
     """
-    
+
     def __init__(self):
         self.parser = OptionParser(self.usage)
-        #~ self.parser.prog = 'build.py' #hack to set the name, for reporting errors and help
-        
+        # self.parser.prog = 'build.py' #hack to set the name, for reporting errors and help
+
         self.parser.add_option(
             "-t",
             "--type",
-            choices=["c","h", "H", "f90", "py", "java"],
+            choices=["c", "h", "H", "f90", "py", "java"],
             default="c",
             dest="type",
-            help="TYPE of the code to generate. Can be one of c, h, H, f90, py or java. <c> will generate c code. <h/H> will generate c/c++ header. <f90> will generate fortran 90 code. <py> will generate a python worker wrapper <java> will generate java interface or class, depending on mode. (Defaults to c)")
-        
+            help=(
+                "TYPE of the code to generate. Can be one of c, h, H, f90, py or java."
+                " <c> will generate c code. <h/H> will generate c/c++ header."
+                " <f90> will generate fortran 90 code."
+                " <py> will generate a python worker wrapper."
+                " <java> will generate java interface or class, depending on mode."
+                " (Defaults to c)"
+            ),
+        )
+
         self.parser.add_option(
             "-m",
             "--mode",
-            choices=["mpi","stub", "dir", "sockets", "interface", "class", "script"],
+            choices=["mpi", "stub", "dir", "sockets", "interface", "class", "script"],
             default="mpi",
             dest="mode",
-            help="MODE of the code to generate. Can be <mpi>, <stub>, <dir>,<sockets>, <interface>, <class> or <script>. Generate the MPI handling code or STUB code for the link between mpi and the code (if needed). <dir> will create a directory ann populate it with the files needed to build a code. (Defaults to mpi)")
-        
+            help=(
+                "MODE of the code to generate. Can be <mpi>, <stub>, <dir>,<sockets>,"
+                " <interface>, <class> or <script>. Generate the MPI handling code or"
+                " STUB code for the link between mpi and the code (if needed). <dir>"
+                " will create a directory ann populate it with the files needed to"
+                " build a code. (Defaults to mpi)"
+            ),
+        )
+
         self.parser.add_option(
             "-o",
             "--output",
             default="-",
             dest="output",
-            help="Name of the OUTPUT file. Use - for standard out. ")
-        
+            help="Name of the OUTPUT file. Use - for standard out. ",
+        )
+
         self.parser.add_option(
             "-i",
             "--ignore",
             default="",
             dest="ignore",
-            help="Name of the classes to ignore, functions defined on these classes will not generate code. Comma separated list")
-    
+            help="Name of the classes to ignore, functions defined on these classes will not generate code. Comma separated list",
+        )
+
         self.parser.add_option(
             "-u",
             "--underscore",
             default="",
             dest="underscore",
-            help="Name of the classes to underscore the functions of, for XL fortran compilers")
-        
+            help="Name of the classes to underscore the functions of, for XL fortran compilers",
+        )
+
         self.parser.add_option(
             "-n",
             "--needs-mpi",
             default="true",
             dest="needs_mpi",
-            help="If this boolean flag is set, the worker will initialize mpi, even in the sockets channel is used. Defaults to true")
-        
+            help="If this boolean flag is set, the worker will initialize mpi, even in the sockets channel is used. Defaults to true",
+        )
+
         self.parser.add_option(
             "-x",
             "--executable",
-            action="store_true", 
+            action="store_true",
             default=False,
             dest="make_executable",
-            help="Set the executable bit when generating the output file")
-        
+            help="Set the executable bit when generating the output file",
+        )
+
         self.parser.add_option(
             "--get-amuse-dir",
             action="store_true",
             default=False,
             dest="get_amuse_dir",
-            help="Only output amuse directory")
+            help="Only output amuse directory",
+        )
+        self.parser.add_option(
+            "--get-amuse-package-dir",
+            action="store_true",
+            default=False,
+            dest="get_amuse_package_dir",
+            help="Only output the amuse package root directory",
+        )
         self.parser.add_option(
             "--get-amuse-configmk",
             action="store_true",
             default=False,
             dest="get_amuse_configmk",
-            help="dump amuse config.mk")
+            help="dump amuse config.mk",
+        )
 
-        
         self.options = None
         self.arguments = None
-        
+
     def parse_options(self):
         (self.options, self.arguments) = self.parser.parse_args()
         if self.options.ignore:
             self.options.ignore_classes = list(self.parse_ignore_classes())
         else:
             self.options.ignore_classes = []
-            
+
         if self.options.underscore:
             self.options.underscore_classes = list(self.parse_underscore_classes())
         else:
             self.options.underscore_classes = []
-        
-        self.options.name_of_implementation_class = None 
-        self.options.name_of_module_or_python_file = None 
-        self.options.name_of_class = None 
-        self.options.name_of_the_code = None 
-        
-        
+
+        self.options.name_of_implementation_class = None
+        self.options.name_of_module_or_python_file = None
+        self.options.name_of_class = None
+        self.options.name_of_the_code = None
+
     def parse_arguments(self):
-        if self.options.get_amuse_dir or self.options.get_amuse_configmk:
+        if (
+            self.options.get_amuse_dir
+            or self.options.get_amuse_package_dir
+            or self.options.get_amuse_configmk
+        ):
             return
-        if self.options.mode == 'dir':
+        if self.options.mode == "dir":
             if len(self.arguments) != 1:
-                self.show_error_and_exit("incorrect number of arguments, need name of the code")
-                
+                self.show_error_and_exit(
+                    "incorrect number of arguments, need name of the code"
+                )
+
             self.options.name_of_the_code = self.arguments[0]
         else:
-            if not len(self.arguments) in (2,3) :
+            if not len(self.arguments) in (2, 3):
                 self.show_error_and_exit("incorrect number of arguments")
             try:
                 self.options.name_of_module_or_python_file = self.arguments[0]
                 if len(self.arguments) > 1:
                     self.options.name_of_class = self.arguments[1]
                 if len(self.arguments) > 2:
                     self.options.name_of_implementation_class = self.arguments[2]
             except Exception as exception:
                 self.show_error_and_exit(exception)
-    
 
     def parse_ignore_classes(self):
-        names = self.options.ignore.split(',')
+        names = self.options.ignore.split(",")
         for name in names:
-            index_of_module_classname_split = name.rfind('.')
+            index_of_module_classname_split = name.rfind(".")
             modulename = name[:index_of_module_classname_split]
-            classname = name[index_of_module_classname_split+1:]
-            
+            classname = name[index_of_module_classname_split + 1 :]
+
             __import__(modulename)
             class_to_ignore = getattr(sys.modules[modulename], classname)
             yield class_to_ignore
-        
+
     def parse_underscore_classes(self):
-        names = self.options.underscore.split(',')
+        names = self.options.underscore.split(",")
         for name in names:
-            index_of_module_classname_split = name.rfind('.')
+            index_of_module_classname_split = name.rfind(".")
             modulename = name[:index_of_module_classname_split]
-            classname = name[index_of_module_classname_split+1:]
-            
+            classname = name[index_of_module_classname_split + 1 :]
+
             __import__(modulename)
             class_to_underscore = getattr(sys.modules[modulename], classname)
             yield class_to_underscore
-        
-    
+
     def start(self):
         self.parse_options()
         self.parse_arguments()
-        
+
     def show_error_and_exit(self, exception):
         self.parser.error(exception)
-        
-    
-    
-    
-    
+
+
 def module_name(string):
-    if string.endswith('.py'):
-        amuse_src_directory = os.path.join(get_amuse_directory(), 'src')
+    if string.endswith(".py"):
+        amuse_src_directory = os.path.join(get_amuse_directory(), "src")
         if not os.path.isabs(string):
             string = os.path.join(os.getcwd(), string)
         if not os.path.exists(string):
             raise Exception("Cannot find file with name {0}".format(string))
         if not string.startswith(amuse_src_directory):
-            raise Exception("File {0} must be placed under directory {1}.".format(string, amuse_src_directory))
-        
-        string = string[len(amuse_src_directory)+1:]
-        string = string[:-len('.py')]
-        string = string.replace(os.sep, '.')
+            raise Exception(
+                "File {0} must be placed under directory {1}.".format(
+                    string, amuse_src_directory
+                )
+            )
+
+        string = string[len(amuse_src_directory) + 1:]
+        string = string[: -len(".py")]
+        string = string.replace(os.sep, ".")
     return string
-    
+
+
 def make_cplusplus_header():
     result = create_c.GenerateACHeaderStringFromASpecificationClass()
     result.make_extern_c = False
     return result
 
+
 def make_a_python_worker(channel_type):
     result = create_python_worker.CreateAPythonWorker()
     result.channel_type = channel_type
     return result
 
+
 def make_a_mpi_python_worker():
-    return make_a_python_worker('mpi')
-    
+    return make_a_python_worker("mpi")
+
+
 def make_a_socket_python_worker():
-    return make_a_python_worker('sockets')
-    
+    return make_a_python_worker("sockets")
+
+
 def make_file(uc):
-    settings=uc.options
+    settings = uc.options
     implementation_class = None
     try:
-        if settings.name_of_module_or_python_file.endswith('.py'):
+        if settings.name_of_module_or_python_file.endswith(".py"):
             module = {}
             # Replace with runpy in the future?
             with open(settings.name_of_module_or_python_file) as fh:
                 text = fh.read()
-                code = compile(text, settings.name_of_module_or_python_file, 'exec')
+                code = compile(text, settings.name_of_module_or_python_file, "exec")
                 exec(code, module)
-            #execfile(settings.name_of_module_or_python_file, module)
+            # execfile(settings.name_of_module_or_python_file, module)
             specification_class = module[settings.name_of_class]
             if not settings.name_of_implementation_class is None:
                 implementation_class = module[settings.name_of_implementation_class]
         else:
-            
-            module = __import__(settings.name_of_module_or_python_file,fromlist=[settings.name_of_class])
+            module = __import__(
+                settings.name_of_module_or_python_file,
+                fromlist=[settings.name_of_class],
+            )
             specification_class = getattr(module, settings.name_of_class)
             if not settings.name_of_implementation_class is None:
-                implementation_class = getattr(module, settings.name_of_implementation_class)
+                implementation_class = getattr(
+                    module, settings.name_of_implementation_class
+                )
     except ImportError as exception:
         uc.show_error_and_exit(exception)
-    
-        
-    usecases = { 
-        ('c','mpi'): create_c.GenerateACSourcecodeStringFromASpecificationClass,
-        ('h','mpi'): create_c.GenerateACHeaderStringFromASpecificationClass,
-        ('H','mpi'): make_cplusplus_header,
-        ('f90','mpi'): create_fortran.GenerateAFortranSourcecodeStringFromASpecificationClass,      
-        ('c','stub'): create_c.GenerateACStubStringFromASpecificationClass,    
-        ('f90','stub'): create_fortran.GenerateAFortranStubStringFromASpecificationClass,
-        ('java','interface'): create_java.GenerateAJavaInterfaceStringFromASpecificationClass,
-        ('java','class'): create_java.GenerateAJavaSourcecodeStringFromASpecificationClass,
-        ('java','script'): create_java.GenerateAJavaWorkerScript,
-        ('py','sockets'): make_a_socket_python_worker,
-        ('py','mpi'): make_a_mpi_python_worker,    
+
+    usecases = {
+        ("c", "mpi"): create_c.GenerateACSourcecodeStringFromASpecificationClass,
+        ("h", "mpi"): create_c.GenerateACHeaderStringFromASpecificationClass,
+        ("H", "mpi"): make_cplusplus_header,
+        (
+            "f90",
+            "mpi",
+        ): create_fortran.GenerateAFortranSourcecodeStringFromASpecificationClass,
+        ("c", "stub"): create_c.GenerateACStubStringFromASpecificationClass,
+        (
+            "f90",
+            "stub",
+        ): create_fortran.GenerateAFortranStubStringFromASpecificationClass,
+        (
+            "java",
+            "interface",
+        ): create_java.GenerateAJavaInterfaceStringFromASpecificationClass,
+        (
+            "java",
+            "class",
+        ): create_java.GenerateAJavaSourcecodeStringFromASpecificationClass,
+        ("java", "script"): create_java.GenerateAJavaWorkerScript,
+        ("py", "sockets"): make_a_socket_python_worker,
+        ("py", "mpi"): make_a_mpi_python_worker,
     }
-    
+
     try:
         builder = usecases[(settings.type, settings.mode)]()
         builder.specification_class = specification_class
-        
+
         if not implementation_class is None:
             builder.implementation_factory = implementation_class
-            
+
         builder.ignore_functions_from_specification_classes = settings.ignore_classes
-        builder.underscore_functions_from_specification_classes = settings.underscore_classes
-        builder.needs_mpi = settings.needs_mpi.lower() == 'true'
+        builder.underscore_functions_from_specification_classes = (
+            settings.underscore_classes
+        )
+        builder.needs_mpi = settings.needs_mpi.lower() == "true"
         builder.is_mpi_enabled = config.mpi.is_enabled
         builder.name_of_outputfile = settings.output
     except:
-        uc.show_error_and_exit("'{0}' and '{1}' is not a valid combination of type and mode, cannot generate the code".format(settings.type, settings.mode))
-    
-    if settings.output == '-':
-        sys.stdout.write(str(builder.result) + '\n')
+        uc.show_error_and_exit(
+            "'{0}' and '{1}' is not a valid combination of type and mode, cannot generate the code".format(
+                settings.type, settings.mode
+            )
+        )
+
+    if settings.output == "-":
+        sys.stdout.write(str(builder.result) + "\n")
     else:
         try:
-            
             with open(settings.output, "w") as f:
                 f.write(builder.result)
-                
+
             if settings.make_executable:
                 os.chmod(settings.output, 0o755)
-                
+
         except Exception as exception:
             uc.show_error_and_exit(exception)
-            
-            
-
-
 
 
 def make_directory(uc):
-    settings=uc.options
+    settings = uc.options
 
     usecases = {
-        ('c','dir'): create_dir.CreateADirectoryAndPopulateItWithFilesForACCode,    
-        ('f90','dir'): create_dir.CreateADirectoryAndPopulateItWithFilesForAFortranCode, 
+        ("c", "dir"): create_dir.CreateADirectoryAndPopulateItWithFilesForACCode,
+        (
+            "f90",
+            "dir",
+        ): create_dir.CreateADirectoryAndPopulateItWithFilesForAFortranCode,
     }
-    
+
     try:
         builder = usecases[(settings.type, settings.mode)]()
         builder.name_of_the_code_interface_class = settings.name_of_the_code
         builder.path_of_the_root_directory = os.getcwd()
     except:
-        uc.show_error_and_exit("'{0}' and '{1}' is not a valid combination of type and mode, cannot generate the code".format(settings.type, settings.mode))
-        
+        uc.show_error_and_exit(
+            "'{0}' and '{1}' is not a valid combination of type and mode, cannot generate the code".format(
+                settings.type, settings.mode
+            )
+        )
+
     builder.start()
-    
+
+
 def amusifier():
     TrackLiteratureReferences.suppress_output()
-    
+
     uc = ParseCommandLine()
     uc.start()
-    
+
     if uc.options.get_amuse_dir:
         print(get_amuse_root_dir())
         exit(0)
+    elif uc.options.get_amuse_package_dir:
+        print(get_amuse_package_dir())
+        exit(0)
     elif uc.options.get_amuse_configmk:
         with open(os.path.join(get_amuse_root_dir(), "config.mk")) as f:
             print(f.read())
             exit(0)
-    elif uc.options.mode == 'dir':
+    elif uc.options.mode == "dir":
         make_directory(uc)
     else:
         make_file(uc)
 
-if __name__ == '__main__':
 
+if __name__ == "__main__":
     amusifier()
-
```

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/import_module.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/import_module.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/nospawn.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/nospawn.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/python_code.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/python_code.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/run_command_redirected.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/run_command_redirected.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/slurm.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/slurm.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_c.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_c.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_code.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_code.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_definition.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_definition.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_dir.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_dir.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_fortran.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_fortran.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_java.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_java.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/create_python_worker.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/create_python_worker.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/cython_code_script.template` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/cython_code_script.template`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/fortran_tools.py` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/fortran_tools.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/java_code_script.template` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/java_code_script.template`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/rfi/tools/python_code_script.template` & `amuse_framework-2024.4.0rc1/src/amuse/rfi/tools/python_code_script.template`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/code.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/code.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/console.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/console.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/core.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/core.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/exceptions.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/exceptions.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/interface.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 from amuse.units import quantities
 from amuse.units.quantities import is_quantity
 from amuse.units.core import unit
 from amuse.units import core
 from amuse.units import units
 from amuse.support.options import OptionalAttributes, option
 
-from amuse.support.methods import CodeMethodWrapper, CodeMethodWrapperDefinition, IncorrectWrappedMethodException
+from amuse.support.methods import (
+    CodeMethodWrapper,
+    CodeMethodWrapperDefinition,
+    IncorrectWrappedMethodException,
+)
 from amuse.support.methods import ProxyingMethodWrapper
 from amuse.support.core import late
 from amuse.support import exceptions
 from amuse.support import state
 
 from amuse import datamodel
 from amuse.datamodel import base
@@ -25,86 +29,87 @@
 
 
 class ConvertArgumentsException(core.IncompatibleUnitsException):
     formatstring = "{0}"
 
 
 class OldObjectsBindingMixin(object):
-
     def setup_particles(self, particles):
         self.particles.add_particles(particles)
 
     def update_particles(self, particles):
         self.particles.copy_values_of_all_attributes_to(particles)
 
+
 class MethodArgumentOrResultType(object):
     _returns_result = True
 
     def append_result_value(self, method, definition, value, result):
         result.append(self.convert_result_value(method, definition, value))
 
     def convert_result_value(self, method, definition, value):
         return value
 
     def convert_argument_value(self, method, definition, value):
         return value
 
+
 class NoUnitMethodArgumentOrResultType(MethodArgumentOrResultType):
     def __reduce__(self):
         return (_get_result_type, ("NO_UNIT",))
-        
+
+
 class UnitMethodArgumentOrResultType(MethodArgumentOrResultType):
     def __reduce__(self):
         return (_get_result_type, ("UNIT",))
 
+
 class ErrorCodeMethodArgumentOrResultType(MethodArgumentOrResultType):
     _returns_result = False
 
     def append_result_value(self, method, definition, value, result):
         self.convert_result_value(method, definition, value)
-        
+
     def convert_result_value(self, method, definition, errorcode):
-        if hasattr(errorcode, 'any'):
+        if hasattr(errorcode, "any"):
             if not errorcode.any():
                 return
-        if hasattr(errorcode, '__iter__'):
+        if hasattr(errorcode, "__iter__"):
             for x in errorcode:
                 definition.handle_errorcode(x)
         else:
             definition.handle_errorcode(errorcode)
-            
+
     def __reduce__(self):
         return (_get_result_type, ("ERROR_CODE",))
-        
 
 
 class IndexMethodArgumentOrResultType(MethodArgumentOrResultType):
-     
     def convert_result_value(self, method, definition, value):
         return value
-     
+
     def convert_argument_value(self, method, definition, value):
         return value
-        
+
     def __reduce__(self):
         return (_get_result_type, ("INDEX",))
 
+
 def _get_result_type(name):
     if name == "NO_UNIT":
         return MethodWithUnitsDefinition.NO_UNIT
     elif name == "UNIT":
         return MethodWithUnitsDefinition.UNIT
     elif name == "ERROR_CODE":
         return MethodWithUnitsDefinition.ERROR_CODE
     elif name == "INDEX":
         return MethodWithUnitsDefinition.INDEX
 
 
 class LinkMethodArgumentOrResultType(MethodArgumentOrResultType):
-
     def __init__(self, linked_set_name):
         self.linked_set_name = linked_set_name
 
     def get_linked_set(self, method, definition):
         # method might provide a shorter path to the interface object
         # and is cleaner as definition might move to interface class later
         try:
@@ -137,21 +142,21 @@
             all_keys = value.get_all_keys_in_store()
             valid_keys = all_keys[valid]
             valid_indices = numpy.asarray(storage.get_indices_of(valid_keys))
             all_indices = -1 * numpy.ones(len(value), dtype=valid_indices.dtype)
             all_indices[valid] = valid_indices
             return all_indices
 
-class CodeAttributeWrapper(object):
 
+class CodeAttributeWrapper(object):
     def __init__(self):
         pass
 
-class HandleCodeInterfaceAttributeAccess(object):
 
+class HandleCodeInterfaceAttributeAccess(object):
     def supports(self, name, was_found):
         return False
 
     def get_attribute(self, name, result):
         return result
 
     def attribute_names(self):
@@ -159,102 +164,104 @@
 
     def setup(self, object):
         pass
 
     def has_name(self, name):
         return False
 
-class LegacyInterfaceHandler(HandleCodeInterfaceAttributeAccess):
 
+class LegacyInterfaceHandler(HandleCodeInterfaceAttributeAccess):
     def __init__(self, legacy_interface):
         self.legacy_interface = legacy_interface
         self.method_instances = {}
 
     def supports(self, name, was_found):
         return name in self.method_instances or hasattr(self.legacy_interface, name)
 
     def get_attribute(self, name, result):
-
         if name not in self.method_instances:
-            attr = getattr(self.legacy_interface, name)      
-            if hasattr(attr, '__call__'):
-                self.method_instances[name] = ProxyingMethodWrapper(self.legacy_interface, name)
+            attr = getattr(self.legacy_interface, name)
+            if hasattr(attr, "__call__"):
+                self.method_instances[name] = ProxyingMethodWrapper(
+                    self.legacy_interface, name
+                )
             else:
                 return attr
 
         return self.method_instances[name]
 
     def attribute_names(self):
         return set(dir(self.legacy_interface))
 
     def has_name(self, name):
-        return name == 'LEGACY'
-
+        return name == "LEGACY"
 
-class HandleConvertUnits(HandleCodeInterfaceAttributeAccess, CodeMethodWrapperDefinition):
 
+class HandleConvertUnits(
+    HandleCodeInterfaceAttributeAccess, CodeMethodWrapperDefinition
+):
     def __init__(self, handler):
         self.handler = handler
         self.converter = None
 
     def supports(self, name, was_found):
-        return was_found and not self.converter is None
+        return was_found and self.converter is not None
 
     def get_attribute(self, name, attribute):
         if inspect.ismethod(attribute):
-            result = attribute #UnitsConvertionMethod(attribute, self.converter)
+            result = attribute  # UnitsConvertionMethod(attribute, self.converter)
         elif isinstance(attribute, datamodel.AbstractParticleSet):
-            result = attribute #datamodel.ParticlesWithUnitsConverted(attribute, self.converter)
+            result = attribute  # datamodel.ParticlesWithUnitsConverted(attribute, self.converter)
         elif isinstance(attribute, datamodel.AbstractGrid):
-            result = attribute 
+            result = attribute
         elif isinstance(attribute, quantities.Quantity):
             result = self.converter.from_target_to_source(attribute)
         elif isinstance(attribute, CodeMethodWrapper):
             result = CodeMethodWrapper(attribute, self)
         elif isinstance(attribute, parameters.Parameters):
-            result = parameters.new_parameters_with_units_converted_instance_with_docs(attribute, self.converter)
+            result = parameters.new_parameters_with_units_converted_instance_with_docs(
+                attribute, self.converter
+            )
         elif isinstance(attribute, str):
             result = attribute
         elif isinstance(attribute, bytearray):
             result = attribute
-        elif hasattr(attribute, '__iter__'):
+        elif hasattr(attribute, "__iter__"):
             result = list(self.convert_and_iterate(attribute))
         else:
             result = attribute
         return result
 
     def convert_and_iterate(self, iterable):
         for x in iterable:
             if isinstance(x, quantities.Quantity):
                 yield self.converter.from_target_to_source(x)
             else:
                 yield x
 
-
     def set_converter(self, converter):
         self.converter = converter
 
     def set_nbody_converter(self, nbody_converter):
         self.set_converter(nbody_converter.as_converter_from_si_to_generic())
 
     def has_name(self, name):
-        return name == 'UNIT'
+        return name == "UNIT"
 
     def setup(self, object):
         object.define_converter(self)
 
-    def convert_arguments(self, method,  list_arguments, keyword_arguments):
-        
+    def convert_arguments(self, method, list_arguments, keyword_arguments):
         converted_list_arguments = []
-        for x,is_nbody in zip(list_arguments, method.nbody_input_attributes):
+        for x, is_nbody in zip(list_arguments, method.nbody_input_attributes):
             if is_nbody:
                 converted_list_arguments.append(self.from_source_to_target(x))
             else:
                 converted_list_arguments.append(x)
-        
+
         converted_keyword_arguments = {}
         for key, value in keyword_arguments.items():
             converted_keyword_arguments[key] = self.from_source_to_target(value)
 
         return converted_list_arguments, converted_keyword_arguments
 
     def convert_result(self, method, result):
@@ -272,21 +279,22 @@
                 return x
             else:
                 return self.converter.from_target_to_source(x)
         elif isinstance(x, str):
             return x
         elif isinstance(x, numpy.ndarray):
             return x
-        elif hasattr(x, '__len__'):
+        elif hasattr(x, "__len__"):
             return list(self.convert_and_iterate(x))
-        elif hasattr(x, '__iter__'):
+        elif hasattr(x, "__iter__"):
             return list(self.convert_and_iterate(x))
         else:
             return x
 
+
 class StateMethodDefinition(CodeMethodWrapperDefinition):
     def __init__(self, state_machine, interface, from_state, to_state, function_name):
         self.state_machine = state_machine
         self.interface = interface
         self.transitions = []
         self.add_transition(from_state, to_state)
         self.function_name = function_name
@@ -303,15 +311,19 @@
                 index = i
         if index >= 0:
             del self.transitions[index]
 
     def new_method(self, method=None):
         if method is None:
             if self.is_determining_method:
-                raise Exception("A state is defined for a method with name '{0}', but the method is not implemented".format(self.function_name))
+                raise Exception(
+                    "A state is defined for a method with name '{0}', but the method is not implemented".format(
+                        self.function_name
+                    )
+                )
             self.is_determining_method = True
             try:
                 method = getattr(self.interface, self.function_name)
             finally:
                 self.is_determining_method = False
 
         return CodeMethodWrapper(method, self)
@@ -323,77 +335,83 @@
                 return to_state
             elif from_state.matches(self.state_machine._current_state):
                 return to_state
             else:
                 stored_transitions.append((from_state, to_state))
 
         possible_paths = []
-        for from_state, to_state  in stored_transitions:
+        for from_state, to_state in stored_transitions:
             try:
-                transition_path = self.state_machine._get_state_transition_path_to(from_state)
+                transition_path = self.state_machine._get_state_transition_path_to(
+                    from_state
+                )
                 possible_paths.append([transition_path, to_state])
             except Exception as ex:
                 pass
 
-        if len(possible_paths) == 0:            
+        if len(possible_paths) == 0:
             # do again to get an exception.
-            message = "While calling {0} of {1}: ".format(self.function_name, type(self.interface))
+            message = "While calling {0} of {1}: ".format(
+                self.function_name, type(self.interface)
+            )
             try:
-                self.state_machine._get_state_transition_path_to(stored_transitions[0][0])
+                self.state_machine._get_state_transition_path_to(
+                    stored_transitions[0][0]
+                )
             except exceptions.AmuseException as ex:
                 args = list(ex.arguments)
-                args[0] = message+str(args[0])
+                args[0] = message + str(args[0])
                 ex.arguments = tuple(args)
                 raise ex
             except Exception as ex:
                 args = list(ex.args)
-                args[0] = message+str(args[0])
+                args[0] = message + str(args[0])
                 ex.args = tuple(args)
                 raise ex
 
         for path, to_state in sorted(possible_paths, key=lambda x: len(x[0])):
             for transition in path:
                 transition.do()
             return to_state
 
-
     def postcall(self, method, to_state):
         if to_state is None:
             return
         elif to_state.matches(self.state_machine._current_state):
             return
         else:
             self.state_machine._current_state = to_state
 
     def __str__(self):
         return "<StateMethod {0}>".format(self.function_name)
 
 
 class HandleState(HandleCodeInterfaceAttributeAccess):
-
     def __init__(self, interface, **options):
         self._mapping_from_name_to_state_method = {}
         self.interface = interface
         self._state_machine = state.StateMachine(interface, **options)
 
     def supports(self, name, was_found):
-        if name == 'state_machine':
+        if name == "state_machine":
             return True
         else:
-            return self._state_machine.is_enabled and (name in self._mapping_from_name_to_state_method)
+            return self._state_machine.is_enabled and (
+                name in self._mapping_from_name_to_state_method
+            )
 
-    def get_attribute(self, name, value): 
-        if name == 'state_machine':
+    def get_attribute(self, name, value):
+        if name == "state_machine":
             return self._state_machine
         else:
             return self._mapping_from_name_to_state_method[name].new_method(value)
 
     def attribute_names(self):
         result = set(self._mapping_from_name_to_state_method.keys())
-        result.add('state_machine')
+        result.add("state_machine")
         return result
 
     def define_state(self, name):
         self._state_machine.new_state(name)
 
     def _add_state_method(self, from_state, to_state, function_name):
         if function_name not in self._mapping_from_name_to_state_method:
@@ -422,17 +440,18 @@
         self._add_state_method(
             self._state_machine.new_state(state_name),
             None,
             function_name,
         )
 
     def add_transition(self, from_name, to_name, function_name, is_auto=True):
-
         transition = self._state_machine.new_transition(
-            from_name, to_name, is_auto,
+            from_name,
+            to_name,
+            is_auto,
         )
 
         definition = StateMethodDefinition(
             self._state_machine,
             self.interface,
             transition.from_state,
             transition.to_state,
@@ -444,51 +463,54 @@
         self._add_state_method(
             transition.from_state,
             transition.to_state,
             function_name,
         )
 
     def remove_transition(self, from_name, to_name, function_name):
-
         self._state_machine.remove_transition(from_name, to_name)
 
         self._remove_state_method(from_name, to_name, function_name)
 
-
     def add_transition_to_method(self, state_name, function_name, is_auto=True):
         """
         Define a method that can run in any state and will transition the
         interface to the provided state.
         """
 
         transition = self._state_machine.new_transition(None, state_name, is_auto)
 
-        definition = StateMethodDefinition(self._state_machine, self.interface, transition.from_state, transition.to_state, function_name)
+        definition = StateMethodDefinition(
+            self._state_machine,
+            self.interface,
+            transition.from_state,
+            transition.to_state,
+            function_name,
+        )
         transition.method = definition
-    
+
         self._add_state_method(None, transition.to_state, function_name)
 
     def do_automatic_state_transitions(self, boolean):
         self._state_machine._do_automatic_state_transitions = boolean
 
     def set_initial_state(self, name):
         self._state_machine.set_initial_state(name)
 
     def setup(self, object):
         object.define_state(self)
 
     def has_name(self, name):
-        return name == 'STATE'
+        return name == "STATE"
 
     def get_name_of_current_state(self):
         return self._state_machine.get_name_of_current_state()
 
 
 class MethodWithUnits(CodeMethodWrapper):
-
     def __init__(self, original_method, definition):
         CodeMethodWrapper.__init__(self, original_method, definition)
 
     @late
     def index_input_attributes(self):
         return self.definition.index_input_attributes
 
@@ -498,42 +520,41 @@
 
     @late
     def index_output_attributes(self):
         return self.definition.index_output_attributes
 
 
 class MethodWithUnitsDefinition(CodeMethodWrapperDefinition):
-
     ERROR_CODE = ErrorCodeMethodArgumentOrResultType()
     NO_UNIT = NoUnitMethodArgumentOrResultType()
     UNIT = UnitMethodArgumentOrResultType()
     INDEX = IndexMethodArgumentOrResultType()
     LINK = LinkMethodArgumentOrResultType
 
     def __init__(self, wrapped_object, function_name, units, return_units, name):
         self.function_name = function_name
 
-        if hasattr(units, '__iter__'):
+        if hasattr(units, "__iter__"):
             self.units = units
         else:
             self.units = (units,)
 
         self.return_units = return_units
-        self.is_return_units_iterable = hasattr(self.return_units, '__iter__')
+        self.is_return_units_iterable = hasattr(self.return_units, "__iter__")
         self.wrapped_object = wrapped_object
         self.name = name
         if self.return_units is None:
             self.handle_return_value = self.handle_as_errorcode
         else:
             self.handle_return_value = self.handle_as_unit
 
     def __getstate__(self):
         result = {}
         result.update(self.__dict__)
-        del result['handle_return_value']
+        del result["handle_return_value"]
         return result
 
     def __setstate__(self, state):
         self.__dict__ = state
         if self.return_units is None:
             self.handle_return_value = self.handle_as_errorcode
         else:
@@ -555,54 +576,52 @@
     def handle_errorcode(self, errorcode):
         if errorcode in self.wrapped_object.errorcodes:
             raise exceptions.AmuseException(
                 f"Error when calling '{self.name}' of a "
                 f"'{type(self.wrapped_object)}', errorcode is "
                 f"{errorcode}, error is "
                 f"'{self.wrapped_object.errorcodes[errorcode]}'",
-                errorcode
+                errorcode,
             )
         elif errorcode < 0:
             raise exceptions.AmuseException(
                 f"Error when calling '{self.name}' of a "
                 f"'{type(self.wrapped_object)}', errorcode is "
                 f"{errorcode}",
-                errorcode
+                errorcode,
             )
         else:
             return errorcode
 
     def handle_as_errorcode(self, method, errorcode):
-        if hasattr(errorcode, 'any'):
+        if hasattr(errorcode, "any"):
             if not errorcode.any():
                 return
-        if hasattr(errorcode, '__iter__'):
+        if hasattr(errorcode, "__iter__"):
             for x in errorcode:
                 self.handle_errorcode(x)
         else:
             self.handle_errorcode(errorcode)
 
     def handle_as_unit(self, method, return_value):
         if not self.is_return_units_iterable:
-            return self.return_units.convert_result_value(
-                method, self, return_value)
+            return self.return_units.convert_result_value(method, self, return_value)
         else:
-            if not hasattr(return_value, '__iter__'):
+            if not hasattr(return_value, "__iter__"):
                 return_value = [return_value]
 
             result = []
             for value, unit in zip(return_value, self.return_units):
                 unit.append_result_value(method, self, value, result)
 
             if len(result) == 1:
                 return result[0]
             else:
                 return result
 
-
     def convert_arguments(self, method, list_arguments, keyword_arguments):
         result = {}
         input_parameters = method.method_input_argument_names
 
         for index, parameter in enumerate(input_parameters):
             if parameter in keyword_arguments:
                 if self.units[index] == self.NO_UNIT:
@@ -613,49 +632,52 @@
                         result[parameter] = arg
                 elif self.units[index] == self.INDEX:
                     result[parameter] = keyword_arguments[parameter]
                 elif self.units[index] == self.UNIT:
                     result[parameter] = keyword_arguments[parameter]
                 else:
                     result[parameter] = quantities.value_in(
-                        keyword_arguments[parameter],self.units[index])
+                        keyword_arguments[parameter], self.units[index]
+                    )
 
         for index, argument in enumerate(list_arguments):
             parameter = input_parameters[index]
             if parameter in result:
                 raise ConvertArgumentsException(
                     f"got multiple values for argument '{parameter}' "
                     f"of method {self.function_name}"
-              )
+                )
             try:
                 if self.units[index] == self.NO_UNIT:
                     if is_quantity(argument):
                         result[parameter] = argument.value_in(units.none)
                     else:
                         result[parameter] = argument
                 elif self.units[index] == self.INDEX:
                     result[parameter] = argument
                 elif self.units[index] == self.UNIT:
                     result[parameter] = argument
                 elif type(self.units[index]) == self.LINK:
-                    result[parameter] = self.units[index].convert_argument_value(method, self, argument)
+                    result[parameter] = self.units[index].convert_argument_value(
+                        method, self, argument
+                    )
                 else:
-                    if self.units[index].is_none() and not hasattr(argument,'unit'):
+                    if self.units[index].is_none() and not hasattr(argument, "unit"):
                         result[parameter] = argument
                     else:
-                        result[parameter] = quantities.value_in(argument,self.units[index])
+                        result[parameter] = quantities.value_in(
+                            argument, self.units[index]
+                        )
             except core.IncompatibleUnitsException as ex:
                 raise ConvertArgumentsException(
-                    f"error while converting parameter '{parameter}', "
-                    f"error: {ex}"
+                    f"error while converting parameter '{parameter}', " f"error: {ex}"
                 )
             except Exception as ex:
                 raise exceptions.AmuseException(
-                    f"error while converting parameter '{parameter}', "
-                    f"error: {ex}"
+                    f"error while converting parameter '{parameter}', " f"error: {ex}"
                 )
 
         return (), result
 
     def convert_result(self, method, result):
         return self.handle_return_value(method, result)
 
@@ -673,90 +695,92 @@
                 nresult = 0
                 for unit in self.return_units:
                     if not hasattr(unit, "_returns_result"):
                         nresult += 1
                     else:
                         if unit._returns_result:
                             nresult += 1
-                
+
                 return list(range(nresult))
 
     @late
     def has_same_name_as_original(self):
         return self.function_name == self.name
 
     @late
     def index_input_attributes(self):
         return [x == self.INDEX for x in self.units]
 
     @late
     def nbody_input_attributes(self):
-        return [isinstance(x, UnitMethodArgumentOrResultType) or isinstance(x, unit) and generic_unit_system.is_generic_unit(x) for x in self.units]
+        return [
+            isinstance(x, UnitMethodArgumentOrResultType)
+            or isinstance(x, unit)
+            and generic_unit_system.is_generic_unit(x)
+            for x in self.units
+        ]
 
     @late
     def index_output_attributes(self):
-        if not hasattr(self.return_units, '__iter__'):
+        if not hasattr(self.return_units, "__iter__"):
             return [self.return_units == self.INDEX]
         else:
             return [x == self.INDEX for x in self.return_units]
 
-
     def check_inputs_of_method(self, method):
-
         specification = method.legacy_specification
         if specification is None:
             return
 
         number_expected_inputs = len(specification.input_parameters)
 
         if self.units:
-            if hasattr(self.units, '__len__'):
+            if hasattr(self.units, "__len__"):
                 number_specified_inputs = len(self.units)
             else:
                 number_specified_inputs = 1
         else:
             number_specified_inputs = 0
 
         if number_expected_inputs != number_specified_inputs:
             raise IncorrectMethodDefinition(
                 self.name,
                 type(self.wrapped_object).__name__,
                 number_expected_inputs,
                 number_specified_inputs,
-                'inputs'
+                "inputs",
             )
 
     def check_outputs_of_method(self, method):
-
         specification = method.legacy_specification
         if specification is None:
             return
 
         number_expected_outputs = len(specification.output_parameters)
         if specification.result_type is not None:
             number_expected_outputs += 1
-   
+
         if self.return_units:
-            if hasattr(self.return_units, '__len__'):
+            if hasattr(self.return_units, "__len__"):
                 number_specified_outputs = len(self.return_units)
             else:
                 number_specified_outputs = 1
         else:
             number_specified_outputs = 0
 
-        if number_expected_outputs == 1 and  number_specified_outputs == 0:
+        if number_expected_outputs == 1 and number_specified_outputs == 0:
             return  # default error checks for one output
 
         if number_expected_outputs != number_specified_outputs:
             raise IncorrectMethodDefinition(
                 self.name,
                 type(self.wrapped_object).__name__,
                 number_expected_outputs,
                 number_specified_outputs,
-                'outputs'
+                "outputs",
             )
 
 
 class HandleMethodsWithUnits(object):
     ERROR_CODE = MethodWithUnitsDefinition.ERROR_CODE
     NO_UNIT = MethodWithUnitsDefinition.NO_UNIT
     INDEX = MethodWithUnitsDefinition.INDEX
@@ -776,97 +800,99 @@
 
             if not specification.result_type is None:
                 if specification.result_unit is None:
                     return_units.append(MethodWithUnitsDefinition.ERROR_CODE)
                 else:
                     return_units.append(specification.result_unit)
 
-            default_to_nounit = lambda y: MethodWithUnitsDefinition.NO_UNIT if y is None else y
+            default_to_nounit = (
+                lambda y: MethodWithUnitsDefinition.NO_UNIT if y is None else y
+            )
 
-            return_units = [ default_to_nounit(x) for x in return_units]
+            return_units = [default_to_nounit(x) for x in return_units]
             units = [default_to_nounit(x) for x in units]
             definition = MethodWithUnitsDefinition(
-                self.interface,
-                name,
-                units,
-                return_units,
-                name
+                self.interface, name, units, return_units, name
             )
             self.method_definitions[name] = definition
 
     def interface_function_specifications(self):
         interface_type = type(self.interface.legacy_interface)
         attribute_names = dir(interface_type)
         result = []
         for x in attribute_names:
-            if x.startswith('__'):
+            if x.startswith("__"):
                 continue
             value = getattr(interface_type, x)
-            if hasattr(value, 'specification') and hasattr(value.specification, 'input_parameters'):
-                result.append( [x,value.specification])
+            if hasattr(value, "specification") and hasattr(
+                value.specification, "input_parameters"
+            ):
+                result.append([x, value.specification])
         result.sort(key=lambda x: x[1].id)
         return result
-        
+
     def supports(self, name, was_found):
         return name in self.method_definitions
 
     def get_attribute(self, name, value):
         if not name in self.method_instances:
-            self.method_instances[name] = self.method_definitions[name].new_method(value)
+            self.method_instances[name] = self.method_definitions[name].new_method(
+                value
+            )
 
         return self.method_instances[name]
 
-
     def attribute_names(self):
         return set(self.method_definitions.keys())
 
-    def add_method(self, original_name, units, return_unit=None,  public_name=None):
+    def add_method(self, original_name, units, return_unit=None, public_name=None):
         if public_name is None:
             public_name = original_name
 
         definition = MethodWithUnitsDefinition(
-            self.interface,
-            original_name,
-            units,
-            return_unit,
-            public_name
+            self.interface, original_name, units, return_unit, public_name
         )
         self.method_definitions[public_name] = definition
 
     def has_name(self, name):
-        return name == 'METHOD'
+        return name == "METHOD"
 
     def setup(self, object):
         object.define_methods(self)
 
 
 class PropertyWithUnitsDefinition(object):
-
     def __init__(self, handler, function_or_attribute_name, unit, public_name):
         self.function_or_attribute_name = function_or_attribute_name
         self.unit = unit
         self.public_name = public_name
         self.handler = handler
 
     def get_value(self, original):
         if self.has_same_name_as_original:
             function_or_attribute = original
         else:
-            function_or_attribute = getattr(self.handler.interface, self.function_or_attribute_name)
-    
-        if hasattr(function_or_attribute, '__call__'):
+            function_or_attribute = getattr(
+                self.handler.interface, self.function_or_attribute_name
+            )
+
+        if hasattr(function_or_attribute, "__call__"):
             return_value = function_or_attribute()
-            if hasattr(return_value, '__iter__'):
+            if hasattr(return_value, "__iter__"):
                 if len(return_value) > 2:
                     return_value = list(return_value)
                     value, errorcode = return_value[:-1], return_value[-1]
                 else:
                     value, errorcode = return_value
                 if errorcode < 0:
-                    raise exceptions.AmuseException("calling '{0}' to get the value for property '{1}' resulted in an error (errorcode {2})".format(self.function_or_attribute_name, self.public_name, errorcode))
+                    raise exceptions.AmuseException(
+                        "calling '{0}' to get the value for property '{1}' resulted in an error (errorcode {2})".format(
+                            self.function_or_attribute_name, self.public_name, errorcode
+                        )
+                    )
                 else:
                     return self.unit.new_quantity(value)
             else:
                 return self.unit.new_quantity(return_value)
         else:
             return self.unit.new_quantity(function_or_attribute)
 
@@ -887,32 +913,29 @@
         return self.property_definitions[name].get_value(value)
 
     def attribute_names(self):
         return set(self.property_definitions.keys())
 
     def add_property(self, function_name, unit=None, public_name=None):
         if public_name is None:
-            if function_name.startswith('get_'):
+            if function_name.startswith("get_"):
                 public_name = function_name[4:]
             else:
                 public_name = function_name
 
         if unit is None:
             definition = PropertyDefinition(self, function_name, public_name)
         else:
             definition = PropertyWithUnitsDefinition(
-                self,
-                function_name,
-                unit,
-                public_name
+                self, function_name, unit, public_name
             )
         self.property_definitions[public_name] = definition
 
     def has_name(self, name):
-        return name == 'PROPERTY'
+        return name == "PROPERTY"
 
     def setup(self, object):
         object.define_properties(self)
 
 
 class HandleParameters(HandleCodeInterfaceAttributeAccess):
     def __init__(self, interface):
@@ -923,641 +946,740 @@
 
     def supports(self, name, was_found):
         return name in self.definitions.keys()
 
     def get_attribute(self, name, value):
         # note: parameters can be added after init, not yet removed
 
-        name = name or 'parameters'
+        name = name or "parameters"
 
         if name not in self.parameters:
             d = self.definitions[name]
-            self.parameters[name] = parameters.new_parameters_instance_with_docs(d, self.interface)
+            self.parameters[name] = parameters.new_parameters_instance_with_docs(
+                d, self.interface
+            )
         else:
-            self.parameters[name].update()       
+            self.parameters[name].update()
         result = self.parameters[name]
         return result
 
     def attribute_names(self):
         return set(self.definitions.keys())
 
-    def add_method_parameter(self, get_method, set_method, name, description, 
-            default_value=None, must_set_before_get=False, is_vector=False,
-            parameter_set='parameters'):
+    def add_method_parameter(
+        self,
+        get_method,
+        set_method,
+        name,
+        description,
+        default_value=None,
+        must_set_before_get=False,
+        is_vector=False,
+        parameter_set="parameters",
+    ):
         if is_vector:
             definition = parameters.ModuleVectorMethodParameterDefinition(
                 get_method,
                 set_method,
                 name,
                 description,
                 default_value,
-                must_set_before_get=must_set_before_get
+                must_set_before_get=must_set_before_get,
             )
         else:
             definition = parameters.ModuleMethodParameterDefinition(
                 get_method,
                 set_method,
                 name,
                 description,
                 default_value,
-                must_set_before_get=must_set_before_get
+                must_set_before_get=must_set_before_get,
             )
         self.definitions[parameter_set].append(definition)
 
     def add_alias_parameter(
         self,
         name,
         aliased_name,
         description,
-        parameter_set='parameters',
+        parameter_set="parameters",
         alias_set=None,
     ):
         definition = parameters.AliasParameterDefinition(
-            name,
-            aliased_name,
-            description,
-            alias_set=alias_set
+            name, aliased_name, description, alias_set=alias_set
         )
         self.definitions[parameter_set].append(definition)
 
     def add_caching_parameter(
         self,
         function_name,
         parameter_name,
         name,
         description,
         default_value=None,
-        parameter_set='parameters',
+        parameter_set="parameters",
     ):
         definition = parameters.ModuleCachingParameterDefinition(
-            function_name,
-            parameter_name,
-            name,
-            description,
-            default_value
+            function_name, parameter_name, name, description, default_value
         )
         self.definitions[parameter_set].append(definition)
 
     def add_boolean_parameter(
         self,
         get_method,
         set_method,
         name,
         description,
         default_value=None,
-        parameter_set='parameters',
+        parameter_set="parameters",
     ):
         definition = parameters.ModuleBooleanParameterDefinition(
-            get_method,
-            set_method,
-            name,
-            description,
-            default_value
+            get_method, set_method, name, description, default_value
         )
         self.definitions[parameter_set].append(definition)
 
     def add_default_form_parameter(
-        self, name, description, default, parameter_set='parameters'
+        self, name, description, default, parameter_set="parameters"
     ):
         if isinstance(default, bool):
             self.add_boolean_parameter(
-                "get_"+name,
-                "set_"+name,
+                "get_" + name,
+                "set_" + name,
                 name,
                 description,
                 default,
-                parameter_set='parameters'
+                parameter_set="parameters",
             )
         else:
             self.add_method_parameter(
-                "get_"+name,
-                "set_"+name,
+                "get_" + name,
+                "set_" + name,
                 name,
                 description,
                 default,
-                parameter_set='parameters',
+                parameter_set="parameters",
             )
 
     def add_array_parameter(
         self,
         get_method,
         set_method,
         range_method,
         name,
         description,
-        parameter_set='parameters',
+        parameter_set="parameters",
     ):
         definition = parameters.ModuleArrayParameterDefinition(
-            get_method,
-            set_method,
-            range_method,
-            name,
-            description
+            get_method, set_method, range_method, name, description
         )
         self.definitions[parameter_set].append(definition)
 
     def has_name(self, name):
-        return name == 'PARAMETER'
+        return name == "PARAMETER"
 
     def setup(self, object):
         object.define_parameters(self)
 
     def add_vector_parameter(
         self,
         name,
         description,
         parameter_names,
-        parameter_set='parameters',
+        parameter_set="parameters",
     ):
         default_value = None
         for parameter_name in parameter_names:
             for defined_parameter in self.definitions[parameter_set]:
                 if defined_parameter.name == parameter_name:
                     if default_value is None:
                         if not is_quantity(defined_parameter.default_value):
-                            default_value  = []
+                            default_value = []
                         else:
                             default_value = quantities.AdaptingVectorQuantity()
                     default_value.append(defined_parameter.default_value)
         definition = parameters.VectorParameterDefinition(
-            name,
-            description,
-            parameter_names,
-            default_value
+            name, description, parameter_names, default_value
         )
         self.definitions[parameter_set].append(definition)
 
     def add_interface_parameter(
         self,
         name,
         description,
         default_value,
         state_guard=None,
-        parameter_set='parameters',
+        parameter_set="parameters",
     ):
         definition = parameters.InterfaceParameterDefinition(
             name,
             description,
             default_value,
             state_guard=state_guard,
         )
         self.definitions[parameter_set].append(definition)
 
+
 class HandleErrorCodes(HandleCodeInterfaceAttributeAccess):
     def __init__(self, interface):
         self.error_codes = {}
         self.interface = interface
 
     def supports(self, name, was_found):
-        return name == 'errorcodes'
+        return name == "errorcodes"
 
     def get_attribute(self, name, value):
         return self.error_codes
 
     def attribute_names(self):
-        return set(['errorcodes'])
+        return set(["errorcodes"])
 
     def add_errorcode(self, number, string):
         self.error_codes[number] = string
 
     def has_name(self, name):
-        return name == 'ERRORCODE'
+        return name == "ERRORCODE"
 
     def setup(self, object):
         object.define_errorcodes(self)
 
 
 class AbstractParticleSetDefinition(object):
-
     def set_new(self, name_of_new_particle_method, names=None):
         self.new_particle_method = (name_of_new_particle_method, names)
-        
+
     def set_grid_range(self, name_of_the_get_range_method):
         self.name_of_the_get_range_method = name_of_the_get_range_method
 
     def set_delete(self, name_of_delete_particle_method):
         self.name_of_delete_particle_method = name_of_delete_particle_method
 
     def add_getter(self, name_of_the_getter, names=None):
         self.getters.append((name_of_the_getter, names))
 
     def add_setter(self, name_of_the_setter, names=None):
         self.setters.append((name_of_the_setter, names))
-    
-    def add_gridded_getter(self, name_of_the_getter, name_of_the_range_method, names=None):
-        self.gridded_getters.append((name_of_the_getter,name_of_the_range_method, names))
-        
-    def add_gridded_setter(self, name_of_the_setter, name_of_the_range_method, names=None):
-        self.gridded_setters.append((name_of_the_setter,name_of_the_range_method, names))
-        
+
+    def add_gridded_getter(
+        self, name_of_the_getter, name_of_the_range_method, names=None
+    ):
+        self.gridded_getters.append(
+            (name_of_the_getter, name_of_the_range_method, names)
+        )
+
+    def add_gridded_setter(
+        self, name_of_the_setter, name_of_the_range_method, names=None
+    ):
+        self.gridded_setters.append(
+            (name_of_the_setter, name_of_the_range_method, names)
+        )
+
     def add_attribute(self, name_of_the_attribute, name_of_the_method, names=None):
-        self.attributes.append((name_of_the_attribute,name_of_the_method, names))
+        self.attributes.append((name_of_the_attribute, name_of_the_method, names))
 
     def add_query(self, name_of_the_query, names=(), public_name=None):
         if not public_name:
             public_name = name_of_the_query
         self.queries.append((name_of_the_query, names, public_name))
 
-
     def add_method(self, name_of_the_method, public_name=None):
         if not public_name:
             public_name = name_of_the_method
         self.methods.append((name_of_the_method, public_name))
 
-
     def add_select_from_particle(self, name, names=(), public_name=None):
         if not public_name:
             public_name = name
         self.selects_form_particle.append((name, names, public_name))
-    
+
     def define_extra_keywords(self, dictionary):
         self.extra_keyword_arguments_for_getters_and_setters = dictionary
-    
-    
 
-    def add_subselect_in_set(self, name, set_query_arguments_name=None, get_number_of_particles_name=None,  public_name=None):
+    def add_subselect_in_set(
+        self,
+        name,
+        set_query_arguments_name=None,
+        get_number_of_particles_name=None,
+        public_name=None,
+    ):
         if not public_name:
             public_name = name
-        self.subselects_in_set.append((name, set_query_arguments_name, get_number_of_particles_name, public_name))
-    
+        self.subselects_in_set.append(
+            (name, set_query_arguments_name, get_number_of_particles_name, public_name)
+        )
 
-    
-    def add_subselect_from_particle(self, name, get_number_of_particles_name=None,  public_name=None):
+    def add_subselect_from_particle(
+        self, name, get_number_of_particles_name=None, public_name=None
+    ):
         if not public_name:
             public_name = name
-        self.subselects_from_particle.append((name, get_number_of_particles_name, public_name))
+        self.subselects_from_particle.append(
+            (name, get_number_of_particles_name, public_name)
+        )
 
-class ParticleSetDefinition(AbstractParticleSetDefinition):
 
+class ParticleSetDefinition(AbstractParticleSetDefinition):
     def __init__(self, handler):
         self.handler = handler
-        self.name_of_indexing_attribute = 'index_of_the_particle'
-        self.new_particle_method = ('new_particle', (), None)
-        self.name_of_delete_particle_method = 'delete_particle'
-        self.name_of_number_of_particles_method = 'get_number_of_particles'
+        self.name_of_indexing_attribute = "index_of_the_particle"
+        self.new_particle_method = ("new_particle", (), None)
+        self.name_of_delete_particle_method = "delete_particle"
+        self.name_of_number_of_particles_method = "get_number_of_particles"
         self.setters = []
         self.getters = []
         self.gridded_getters = []
         self.gridded_setters = []
         self.queries = []
         self.attributes = []
-    
+
         self.selects_form_particle = []
         self.subselects_in_set = []
         self.subselects_from_particle = []
         self.methods = []
         self.is_superset = False
         self.is_inmemory = False
         self.particles_factory = datamodel.Particles
 
     def new_storage(self, interface):
-    
         if self.is_inmemory:
             return datamodel.get_in_memory_attribute_storage_factory()()
-    
+
         setters = []
         for name, names in self.setters:
-            x = incode_storage.ParticleSetAttributesMethod(getattr(interface, name), names)
+            x = incode_storage.ParticleSetAttributesMethod(
+                getattr(interface, name), names
+            )
             setters.append(x)
-    
+
         getters = []
         for name, names in self.getters:
-            x = incode_storage.ParticleGetAttributesMethod(getattr(interface, name), names)
+            x = incode_storage.ParticleGetAttributesMethod(
+                getattr(interface, name), names
+            )
             getters.append(x)
-        
+
         for name, range_method_name, names in self.gridded_getters:
             x = incode_storage.ParticleGetGriddedAttributesMethod(
-                    getattr(interface, name), 
-                    getattr(interface, range_method_name), 
-                    names
+                getattr(interface, name), getattr(interface, range_method_name), names
             )
             getters.append(x)
-            
+
         for name, range_method_name, names in self.gridded_setters:
             x = incode_storage.ParticleSetGriddedAttributesMethod(
-                    getattr(interface, name), 
-                    getattr(interface, range_method_name), 
-                    names
+                getattr(interface, name), getattr(interface, range_method_name), names
             )
             setters.append(x)
-            
-    
+
         name, names = self.new_particle_method
-        new_particle_method = incode_storage.NewParticleMethod(getattr(interface, name), names)
-    
+        new_particle_method = incode_storage.NewParticleMethod(
+            getattr(interface, name), names
+        )
+
         delete_particle_method = getattr(interface, self.name_of_delete_particle_method)
-        number_of_particles_method = None  # getattr(interface, self.name_of_number_of_particles_method)
-    
+        number_of_particles_method = (
+            None  # getattr(interface, self.name_of_number_of_particles_method)
+        )
+
         return incode_storage.InCodeAttributeStorage(
             interface,
             new_particle_method,
             delete_particle_method,
             number_of_particles_method,
             setters,
             getters,
-            self.name_of_indexing_attribute
+            self.name_of_indexing_attribute,
         )
 
-    
     def new_set_instance(self, handler):
         storage = self.new_storage(handler.interface)
         if self.is_inmemory:
             result = self.particles_factory(handler.interface, storage=storage)
         else:
             result = self.particles_factory(storage=storage)
-            
+
         queries = self.new_queries(handler.interface)
         for x in queries:
             result.add_function_attribute(x.public_name, x.apply)
-    
+
         selects = self.new_selects_from_particle(handler.interface)
         for x in selects:
             result.add_function_attribute(x.public_name, x.apply_on_all)
             result.add_particle_function_attribute(x.public_name, x.apply_on_one)
 
         selects = self.new_subselects_from_particle(handler.interface)
         for x in selects:
-        # result.add_function_attribute(x.public_name, x.apply_on_all)
+            # result.add_function_attribute(x.public_name, x.apply_on_all)
             result.add_particle_function_attribute(x.public_name, x.apply_on_one)
-            
+
         selects = self.new_subselects_in_set(handler.interface)
         for x in selects:
             result.add_function_attribute(x.public_name, x.apply_on_all)
-    
+
         selects = self.new_particle_methods(handler.interface)
         for x in selects:
             result.add_function_attribute(x.public_name, x.apply_on_all, x.apply_on_one)
-    
+
         attributes = self.attributes
         for name_of_the_attribute, name_of_the_method, names in attributes:
-            result.add_calculated_attribute(name_of_the_attribute, getattr(handler.interface, name_of_the_method), names)
-    
+            result.add_calculated_attribute(
+                name_of_the_attribute,
+                getattr(handler.interface, name_of_the_method),
+                names,
+            )
+
         return result
 
     def new_queries(self, interface):
         queries = []
         for name, names, public_name in self.queries:
-            x = incode_storage.ParticleQueryMethod(getattr(interface, name), names, public_name)
+            x = incode_storage.ParticleQueryMethod(
+                getattr(interface, name), names, public_name
+            )
             queries.append(x)
 
         return queries
 
     def new_selects_from_particle(self, interface):
         results = []
         for name, names, public_name in self.selects_form_particle:
-            x = incode_storage.ParticleSpecificSelectMethod(getattr(interface, name), names, public_name)
+            x = incode_storage.ParticleSpecificSelectMethod(
+                getattr(interface, name), names, public_name
+            )
             results.append(x)
 
         return results
 
     def new_particle_methods(self, interface):
         results = []
         for name, public_name in self.methods:
             x = incode_storage.ParticleMethod(getattr(interface, name), public_name)
             results.append(x)
 
         return results
 
-
     def new_subselects_in_set(self, interface):
         results = []
-        for name, set_query_arguments_name, number_of_particles_name, public_name in self.subselects_in_set:
-            number_of_particles_method = None if number_of_particles_name is None else getattr(interface, number_of_particles_name)
-            set_query_arguments_method = None if set_query_arguments_name is None else getattr(interface, set_query_arguments_name)
-            x = incode_storage.ParticleSetSelectSubsetMethod(getattr(interface, name), set_query_arguments_method, number_of_particles_method, public_name)
+        for (
+            name,
+            set_query_arguments_name,
+            number_of_particles_name,
+            public_name,
+        ) in self.subselects_in_set:
+            number_of_particles_method = (
+                None
+                if number_of_particles_name is None
+                else getattr(interface, number_of_particles_name)
+            )
+            set_query_arguments_method = (
+                None
+                if set_query_arguments_name is None
+                else getattr(interface, set_query_arguments_name)
+            )
+            x = incode_storage.ParticleSetSelectSubsetMethod(
+                getattr(interface, name),
+                set_query_arguments_method,
+                number_of_particles_method,
+                public_name,
+            )
             results.append(x)
-    
+
         return results
-    
-    
+
     def new_subselects_from_particle(self, interface):
         results = []
-        for name, get_number_of_particles_name, public_name in self.subselects_from_particle:
-        
-            number_of_particles_method = None if get_number_of_particles_name is None else getattr(interface, get_number_of_particles_name)
-            x = incode_storage.ParticleSpecificSelectSubsetMethod(getattr(interface, name), number_of_particles_method, public_name)
+        for (
+            name,
+            get_number_of_particles_name,
+            public_name,
+        ) in self.subselects_from_particle:
+            number_of_particles_method = (
+                None
+                if get_number_of_particles_name is None
+                else getattr(interface, get_number_of_particles_name)
+            )
+            x = incode_storage.ParticleSpecificSelectSubsetMethod(
+                getattr(interface, name), number_of_particles_method, public_name
+            )
             results.append(x)
 
         return results
 
-class ParticleSupersetDefinition(AbstractParticleSetDefinition):
 
+class ParticleSupersetDefinition(AbstractParticleSetDefinition):
     def __init__(self, handler, particle_subset_names, index_to_default_set=None):
         self.handler = handler
         self.particle_subset_names = particle_subset_names
         self.index_to_default_set = index_to_default_set
         self.is_superset = True
         self.particles_factory = datamodel.ParticlesSuperset
         self.queries = []
-        
-    
+
     def new_set_instance(self, handler):
-        subsets = [handler.get_attribute(subset_name, None) for subset_name in self.particle_subset_names]
+        subsets = [
+            handler.get_attribute(subset_name, None)
+            for subset_name in self.particle_subset_names
+        ]
         result = self.particles_factory(
-            subsets, 
-            index_to_default_set=self.index_to_default_set
+            subsets, index_to_default_set=self.index_to_default_set
         )
         for one_query in self.new_queries(handler.interface):
             result.add_function_attribute(one_query.public_name, one_query.apply)
         return result
-    
+
     def new_queries(self, interface):
         queries = []
         for name, names, public_name in self.queries:
-            x = incode_storage.ParticleQueryMethod(getattr(interface, name), names, public_name, query_superset=True)
+            x = incode_storage.ParticleQueryMethod(
+                getattr(interface, name), names, public_name, query_superset=True
+            )
             queries.append(x)
         return queries
-    
 
-class GridDefinition(AbstractParticleSetDefinition):
 
+class GridDefinition(AbstractParticleSetDefinition):
     def __init__(self, handler, grid_class=datamodel.Grid):
         self.handler = handler
         self.axes_names = None
-        self.name_of_the_get_range_method = 'get_range'
+        self.name_of_the_get_range_method = "get_range"
         self.setters = []
         self.getters = []
         self.gridded_setters = []
         self.gridded_getters = []
         self.particles_factory = grid_class
         self.extra_keyword_arguments_for_getters_and_setters = {}
 
     def new_storage(self, interface):
-
         setters = []
         for name, names in self.setters:
-            x = incode_storage.ParticleSetAttributesMethod(getattr(interface, name), names)
+            x = incode_storage.ParticleSetAttributesMethod(
+                getattr(interface, name), names
+            )
             setters.append(x)
 
         getters = []
         for name, names in self.getters:
-            x = incode_storage.ParticleGetAttributesMethod(getattr(interface, name), names)
+            x = incode_storage.ParticleGetAttributesMethod(
+                getattr(interface, name), names
+            )
             getters.append(x)
 
         for name, range_method_name, names in self.gridded_getters:
             x = incode_storage.ParticleGetGriddedAttributesMethod(
-                    getattr(interface, name), 
-                    getattr(interface, range_method_name), 
-                    names
+                getattr(interface, name), getattr(interface, range_method_name), names
             )
             getters.append(x)
-            
+
         for name, range_method_name, names in self.gridded_setters:
             x = incode_storage.ParticleSetGriddedAttributesMethod(
-                    getattr(interface, name), 
-                    getattr(interface, range_method_name), 
-                    names
+                getattr(interface, name), getattr(interface, range_method_name), names
             )
             setters.append(x)
 
         range_method = getattr(interface, self.name_of_the_get_range_method)
 
         return incode_storage.InCodeGridAttributeStorage(
             interface,
             range_method,
             setters,
             getters,
-            self.extra_keyword_arguments_for_getters_and_setters
+            self.extra_keyword_arguments_for_getters_and_setters,
         )
 
     def new_set_instance(self, handler):
         storage = self.new_storage(handler.interface)
         result = self.particles_factory(storage=storage)
         if self.axes_names is not None:
-            result.add_vector_attribute("position",self.axes_names)
+            result.add_vector_attribute("position", self.axes_names)
         return result
 
-class CodeInMemoryParticles(datamodel.Particles):
 
+class CodeInMemoryParticles(datamodel.Particles):
     def __init__(self, code_interface=None, storage=None):
         datamodel.Particles.__init__(self, storage=storage)
         self._private.code_interface = code_interface
 
+
 class HandleParticles(HandleCodeInterfaceAttributeAccess):
     def __init__(self, interface):
         self.interface = interface
         self.mapping_from_name_to_set_definition = {}
         self.mapping_from_name_to_set_instance = {}
-        
+
     def supports(self, name, was_found):
         return name in self.mapping_from_name_to_set_definition
 
     def get_attribute(self, name, value):
         if name in self.mapping_from_name_to_set_instance:
             return self.mapping_from_name_to_set_instance[name]
-        else:          
+        else:
             set_definition = self.mapping_from_name_to_set_definition[name]
             if set_definition.state_guard:
                 getattr(self.interface, set_definition.state_guard)()
             result = set_definition.new_set_instance(self)
-                
+
             self.mapping_from_name_to_set_instance[name] = result
             return result
 
     def attribute_names(self):
         return set(self.mapping_from_name_to_set_definition.keys())
 
-
     def has_name(self, name):
-        return name == 'PARTICLES' or name == 'DATASETS' or name == 'GRIDS'
+        return name == "PARTICLES" or name == "DATASETS" or name == "GRIDS"
 
     def setup(self, object):
         object.define_particle_sets(self)
         object.define_data_sets(self)
         object.define_grids(self)
 
-    def define_set(self, name, name_of_indexing_attribute='index_of_the_particle', state_guard=None):
+    def define_set(
+        self, name, name_of_indexing_attribute="index_of_the_particle", state_guard=None
+    ):
         definition = ParticleSetDefinition(self)
         definition.name_of_indexing_attribute = name_of_indexing_attribute
         definition.state_guard = state_guard
         self.mapping_from_name_to_set_definition[name] = definition
 
-    def define_super_set(self, name, particle_subsets, index_to_default_set=None, state_guard=None):
-        definition = ParticleSupersetDefinition(self, particle_subsets, index_to_default_set)
+    def define_super_set(
+        self, name, particle_subsets, index_to_default_set=None, state_guard=None
+    ):
+        definition = ParticleSupersetDefinition(
+            self, particle_subsets, index_to_default_set
+        )
         definition.state_guard = state_guard
         self.mapping_from_name_to_set_definition[name] = definition
 
-    def define_inmemory_set(self, name, particles_factory=CodeInMemoryParticles, state_guard=None):
+    def define_inmemory_set(
+        self, name, particles_factory=CodeInMemoryParticles, state_guard=None
+    ):
         definition = ParticleSetDefinition(self)
         definition.is_inmemory = True
         definition.particles_factory = particles_factory
         definition.state_guard = state_guard
         self.mapping_from_name_to_set_definition[name] = definition
-    
-    def define_grid(self, name, name_of_indexing_attribute='index_of_the_particle', axes_names=None, grid_class=datamodel.Grid, state_guard=None):
+
+    def define_grid(
+        self,
+        name,
+        name_of_indexing_attribute="index_of_the_particle",
+        axes_names=None,
+        grid_class=datamodel.Grid,
+        state_guard=None,
+    ):
         definition = GridDefinition(self, grid_class=grid_class)
         definition.name_of_indexing_attribute = name_of_indexing_attribute
         definition.axes_names = axes_names
         definition.state_guard = state_guard
         self.mapping_from_name_to_set_definition[name] = definition
-        
+
     def set_new(self, name_of_the_set, name_of_new_particle_method, names=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].set_new(name_of_new_particle_method, names=names)
-        
+        self.mapping_from_name_to_set_definition[name_of_the_set].set_new(
+            name_of_new_particle_method, names=names
+        )
+
     def set_grid_range(self, name_of_the_set, name_of_the_get_range_method):
-        self.mapping_from_name_to_set_definition[name_of_the_set].set_grid_range(name_of_the_get_range_method)
+        self.mapping_from_name_to_set_definition[name_of_the_set].set_grid_range(
+            name_of_the_get_range_method
+        )
 
     def set_delete(self, name_of_the_set, name_of_delete_particle_method):
-        self.mapping_from_name_to_set_definition[name_of_the_set].set_delete(name_of_delete_particle_method)
+        self.mapping_from_name_to_set_definition[name_of_the_set].set_delete(
+            name_of_delete_particle_method
+        )
 
     def add_getter(self, name_of_the_set, name_of_the_getter, names=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_getter(name_of_the_getter, names=names)
-        
+        self.mapping_from_name_to_set_definition[name_of_the_set].add_getter(
+            name_of_the_getter, names=names
+        )
+
     def add_setter(self, name_of_the_set, name_of_the_setter, names=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_setter(name_of_the_setter, names=names)
+        self.mapping_from_name_to_set_definition[name_of_the_set].add_setter(
+            name_of_the_setter, names=names
+        )
 
-    def add_gridded_getter(self, name_of_the_set, name_of_the_getter, name_of_the_range_method, names=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_gridded_getter(name_of_the_getter, name_of_the_range_method, names=names)
-    
-    def add_gridded_setter(self, name_of_the_set, name_of_the_setter, name_of_the_range_method, names=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_gridded_setter(name_of_the_setter, name_of_the_range_method, names=names)
-    
-    def add_attribute(self, name_of_the_set, name_of_the_attribute, name_of_the_method, names=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_attribute(name_of_the_attribute, name_of_the_method, names=names)
+    def add_gridded_getter(
+        self, name_of_the_set, name_of_the_getter, name_of_the_range_method, names=None
+    ):
+        self.mapping_from_name_to_set_definition[name_of_the_set].add_gridded_getter(
+            name_of_the_getter, name_of_the_range_method, names=names
+        )
+
+    def add_gridded_setter(
+        self, name_of_the_set, name_of_the_setter, name_of_the_range_method, names=None
+    ):
+        self.mapping_from_name_to_set_definition[name_of_the_set].add_gridded_setter(
+            name_of_the_setter, name_of_the_range_method, names=names
+        )
+
+    def add_attribute(
+        self, name_of_the_set, name_of_the_attribute, name_of_the_method, names=None
+    ):
+        self.mapping_from_name_to_set_definition[name_of_the_set].add_attribute(
+            name_of_the_attribute, name_of_the_method, names=names
+        )
 
     def add_query(self, name_of_the_set, name_of_the_query, names=(), public_name=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_query(name_of_the_query, names=names, public_name=public_name)
+        self.mapping_from_name_to_set_definition[name_of_the_set].add_query(
+            name_of_the_query, names=names, public_name=public_name
+        )
 
     def add_method(self, name_of_the_set, name_of_the_method, public_name=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_method(name_of_the_method, public_name=public_name)
+        self.mapping_from_name_to_set_definition[name_of_the_set].add_method(
+            name_of_the_method, public_name=public_name
+        )
+
+    def add_select_from_particle(
+        self, name_of_the_set, name, names=(), public_name=None
+    ):
+        self.mapping_from_name_to_set_definition[
+            name_of_the_set
+        ].add_select_from_particle(name, names=names, public_name=public_name)
 
-    def add_select_from_particle(self, name_of_the_set, name, names=(), public_name=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_select_from_particle(name, names=names, public_name=public_name)
-        
     def define_extra_keywords(self, name_of_the_set, dictionary):
-        self.mapping_from_name_to_set_definition[name_of_the_set].define_extra_keywords(dictionary)    
-    
-    def add_subselect_in_set(self, name_of_the_set, name, set_query_arguments_name=None, get_number_of_particles_name=None,  public_name=None):
+        self.mapping_from_name_to_set_definition[name_of_the_set].define_extra_keywords(
+            dictionary
+        )
+
+    def add_subselect_in_set(
+        self,
+        name_of_the_set,
+        name,
+        set_query_arguments_name=None,
+        get_number_of_particles_name=None,
+        public_name=None,
+    ):
         self.mapping_from_name_to_set_definition[name_of_the_set].add_subselect_in_set(
-            name, 
-            set_query_arguments_name=set_query_arguments_name, 
-            get_number_of_particles_name=get_number_of_particles_name,  
-            public_name=public_name
-        )
-        
-    def add_subselect_from_particle(self, name_of_the_set, name, get_number_of_particles_name=None,  public_name=None):
-        self.mapping_from_name_to_set_definition[name_of_the_set].add_subselect_from_particle(
-            name, 
-            get_number_of_particles_name=get_number_of_particles_name,  
-            public_name=public_name
+            name,
+            set_query_arguments_name=set_query_arguments_name,
+            get_number_of_particles_name=get_number_of_particles_name,
+            public_name=public_name,
+        )
+
+    def add_subselect_from_particle(
+        self, name_of_the_set, name, get_number_of_particles_name=None, public_name=None
+    ):
+        self.mapping_from_name_to_set_definition[
+            name_of_the_set
+        ].add_subselect_from_particle(
+            name,
+            get_number_of_particles_name=get_number_of_particles_name,
+            public_name=public_name,
         )
 
     def _cleanup_instances(self):
         self.mapping_from_name_to_set_instance = {}
 
-class OverriddenCodeInterface(object):
 
+class OverriddenCodeInterface(object):
     def __init__(self, code_interface):
         self.code_interface = code_interface
 
     def __getattr__(self, name):
         return self.code_interface.__getattr__(name)
 
-class InCodeComponentImplementation(OldObjectsBindingMixin, OptionalAttributes):
 
+class InCodeComponentImplementation(OldObjectsBindingMixin, OptionalAttributes):
     def __init__(self, legacy_interface, **options):
         OptionalAttributes.__init__(self, **options)
         self.legacy_interface = legacy_interface
         self._options = options
         self._handlers = []
         self.__init_handlers__(legacy_interface, options)
 
@@ -1570,18 +1692,24 @@
         if self.must_handle_state:
             self._handlers.append(HandleState(self, **options))
         self._handlers.append(HandleConvertUnits(self))
         self._handlers.append(HandleErrorCodes(self))
 
         self.setup()
 
-    @option(type='boolean', sections=("code", "state",))
+    @option(
+        type="boolean",
+        sections=(
+            "code",
+            "state",
+        ),
+    )
     def must_handle_state(self):
         return True
-    
+
     def setup(self):
         for x in self._handlers:
             x.setup(self)
 
     def define_state(self, handler):
         pass
 
@@ -1634,54 +1762,55 @@
         return list(result)
 
     def overridden(self):
         return OverriddenCodeInterface(self)
 
     def get_name_of_current_state(self):
         return self.state_machine.get_name_of_current_state()
-        
+
     def _create_new_grid(self, builder_function, **extra_arguments):
-        handler = self.get_handler('PARTICLES')
-        definition = GridDefinition(handler, grid_class=extra_arguments.get("grid_class", datamodel.Grid))
+        handler = self.get_handler("PARTICLES")
+        definition = GridDefinition(
+            handler, grid_class=extra_arguments.get("grid_class", datamodel.Grid)
+        )
         builder_function(definition, **extra_arguments)
         return definition.new_set_instance(handler)
-        
+
     def __setstate__(self, state):
         self.__dict__ = state
 
     def data_store_names(self):
         self.before_get_data_store_names()
-        return list(self.get_handler('PARTICLES').mapping_from_name_to_set_definition.keys())
+        return list(
+            self.get_handler("PARTICLES").mapping_from_name_to_set_definition.keys()
+        )
 
     def parameter_set_names(self):
-        #~ self.before_get_data_store_names()
-        return list(self.get_handler('PARAMETER').definitions.keys())
-        
+        # ~ self.before_get_data_store_names()
+        return list(self.get_handler("PARAMETER").definitions.keys())
+
     @property
     def model_name(self):
         return type(self).__name__
 
-    
+
 class IncorrectMethodDefinition(IncorrectWrappedMethodException):
     formatstring = "Incorrect definition of method '{0}' of class '{1}', the number of {4} do not match, expected {2}, actual {3}."
 
 
 class PropertyDefinition(object):
-
     def __init__(self, handler, functionname, publicname, keyword_arguments={}):
         self.functionname = functionname
         self.publicname = publicname
         self.handler = handler
         self.keyword_arguments = {}
         self._method = None
-        
+
     def get_value(self, original):
         if self._method is None:
             self._method = getattr(self.handler.interface, self.functionname)
-         
-        result = self._method (**self.keyword_arguments)
+
+        result = self._method(**self.keyword_arguments)
         if hasattr(result, "__iter__"):
             return quantities.VectorQuantity.new_from_scalar_quantities(*result)
         else:
             return result
-
-
```

### Comparing `amuse-framework-2023.5.0/src/amuse/support/literature.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/literature.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import importlib
 from os.path import exists
 
 from collections import namedtuple
 from docutils import nodes
 from amuse.support import exceptions
 try:
-    from amuse.version import version as amuse_version
+    from amuse._version import version as amuse_version
 except ImportError:
     amuse_version = "unknown version"
 
 import amuse
 
 
 ClassWithLiteratureReferences = namedtuple(
@@ -277,22 +277,23 @@
     def __init__(self):
         self.register_use()
 
     @classmethod
     def version(cls):
         try:
             version = importlib.import_module(
-                '..version',
+                '.._version',
                 cls.__module__
             ).version
         except (ImportError, ValueError):
             try:
                 from amuse.version import version
+                version = f"framework {version}"
             except ImportError:
-                version = "unknown"
+                version = "unknown version"
         return version
 
     @classmethod
     def print_literature_references(cls):
         print("You are currently using the following codes, which contain literature references")
         print(TrackLiteratureReferences.default().all_literature_references_string())
```

### Comparing `amuse-framework-2023.5.0/src/amuse/support/methods.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/methods.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/options.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/options.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/parameter_tools.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/parameter_tools.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/project.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/project.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/state.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/state.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/support/thirdparty/texttable.py` & `amuse_framework-2024.4.0rc1/src/amuse/support/thirdparty/texttable.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/test/amusetest.py` & `amuse_framework-2024.4.0rc1/src/amuse/test/amusetest.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,42 +298,42 @@
             return True
 
 
 class TestDefaults(_Defaults):
 
     @late
     def temporarydir(self):
-        dirname=tempfile.mkdtemp()
-        print(("generating temporary dir for test results: {0}". format(dirname)))
+        dirname = tempfile.mkdtemp(dir="./")
+        print(f"generating temporary dir for test results: {dirname}")
         return dirname
 
     @options.option(sections=['test'])
     def path_to_results(self):
         name_of_testresults_directory = self.name_of_testresults_directory
         if os.path.exists(os.path.abspath(name_of_testresults_directory)):
             if os.access(os.path.abspath(name_of_testresults_directory),  os.W_OK):
                 return os.path.abspath(name_of_testresults_directory)
 
         amuse_root_dir = self.amuse_root_dir
         test_results_dir = os.path.join(amuse_root_dir, self.name_of_testresults_directory)
         if os.path.exists(test_results_dir):
             try:
-                f = open(os.path.join(test_results_dir,'test.txt'),'w')
+                f = open(os.path.join(test_results_dir, 'test.txt'), 'w')
                 f.close()
                 return test_results_dir
             except IOError as ex:
                 pass
         else:
             return self.temporarydir
 
     @options.option(sections=['test'])
     def name_of_testresults_directory(self):
-        return 'test_results'
+        return self.temporarydir
 
-    @options.option(type='boolean',sections=['test'])
+    @options.option(type='boolean', sections=['test'])
     def can_run_tests_to_compile_modules(self):
         return True
 
 _testdefaults=TestDefaults()
 
 def get_path_to_results():
     return _testdefaults.path_to_results
```

### Comparing `amuse-framework-2023.5.0/src/amuse/test/compile_tools.py` & `amuse_framework-2024.4.0rc1/src/amuse/test/compile_tools.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/units/constants.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-
-#This is an auto generated file, do not change manually. Instead if you want to add constants
-#or change them, change the nist.txt file and run nist.py
+"""
+Physical constants
+"""
+# This is an auto generated file, do not change manually. Instead if you want
+# to add constants or change them, change the nist.txt file and run nist.py
 
 import numpy
-from amuse.units.si import *
-from amuse.units.derivedsi import *
+from amuse.units.si import m, kg, s, A, K, mol, none
+from amuse.units.derivedsi import Hz, MHz, sr, N, Pa, J, W, F, C, V, T, ohm, S, Wb
 
-#BASE UNITS***********************************************
+# BASE UNITS***********************************************
 X220X_lattice_spacing_of_silicon = 1.920155762e-10 | m
 alpha_particle_mass = 6.6446562e-27 | kg
 alpha_particle_mass_energy_equivalent = 5.97191917e-10 | J
 Angstrom_star = 1.00001498e-10 | m
 u = 1.660538782e-27 | kg
 atomic_mass_constant_energy_equivalent = 1.49241783e-10 | J
-atomic_mass_unit_hyphen_hertz_relationship = 2.2523427369e+23 | Hz
+atomic_mass_unit_hyphen_hertz_relationship = 2.2523427369e23 | Hz
 atomic_mass_unit_hyphen_joule_relationship = 1.49241783e-10 | J
-atomic_mass_unit_hyphen_kelvin_relationship = 1.0809527e+13 | K
+atomic_mass_unit_hyphen_kelvin_relationship = 1.0809527e13 | K
 atomic_mass_unit_hyphen_kilogram_relationship = 1.660538782e-27 | kg
 atomic_unit_of_charge = 1.602176487e-19 | C
 atomic_unit_of_current = 0.00662361763 | A
 atomic_unit_of_electric_potential = 27.21138386 | V
 atomic_unit_of_energy = 4.35974394e-18 | J
 atomic_unit_of_force = 8.23872206e-08 | N
 atomic_unit_of_length = 5.2917720859e-11 | m
@@ -36,43 +38,43 @@
 Cu_x_unit = 1.00207699e-13 | m
 deuteron_mass = 3.3435832e-27 | kg
 deuteron_mass_energy_equivalent = 3.00506272e-10 | J
 deuteron_rms_charge_radius = 2.1402e-15 | m
 electron_mass = 9.10938215e-31 | kg
 electron_mass_energy_equivalent = 8.18710438e-14 | J
 electron_volt = 1.602176487e-19 | J
-electron_volt_hyphen_hertz_relationship = 2.417989454e+14 | Hz
+electron_volt_hyphen_hertz_relationship = 2.417989454e14 | Hz
 electron_volt_hyphen_joule_relationship = 1.602176487e-19 | J
 electron_volt_hyphen_kelvin_relationship = 11604.505 | K
 electron_volt_hyphen_kilogram_relationship = 1.782661758e-36 | kg
 elementary_charge = 1.602176487e-19 | C
 Hartree_energy = 4.35974394e-18 | J
-hartree_hyphen_hertz_relationship = 6.57968392072e+15 | Hz
+hartree_hyphen_hertz_relationship = 6.57968392072e15 | Hz
 hartree_hyphen_joule_relationship = 4.35974394e-18 | J
 hartree_hyphen_kelvin_relationship = 315774.65 | K
 hartree_hyphen_kilogram_relationship = 4.85086934e-35 | kg
 helion_mass = 5.00641192e-27 | kg
 helion_mass_energy_equivalent = 4.49953864e-10 | J
 hertz_hyphen_joule_relationship = 6.62606896e-34 | J
 hertz_hyphen_kelvin_relationship = 4.7992374e-11 | K
 hertz_hyphen_kilogram_relationship = 7.372496e-51 | kg
 inverse_meter_hyphen_hertz_relationship = 299792458.0 | Hz
 inverse_meter_hyphen_joule_relationship = 1.986445501e-25 | J
 inverse_meter_hyphen_kelvin_relationship = 0.014387752 | K
 inverse_meter_hyphen_kilogram_relationship = 2.2102187e-42 | kg
 inverse_of_conductance_quantum = 12906.4037787 | ohm
-joule_hyphen_hertz_relationship = 1.50919045e+33 | Hz
-joule_hyphen_kelvin_relationship = 7.242963e+22 | K
+joule_hyphen_hertz_relationship = 1.50919045e33 | Hz
+joule_hyphen_kelvin_relationship = 7.242963e22 | K
 joule_hyphen_kilogram_relationship = 1.112650056e-17 | kg
 kelvin_hyphen_hertz_relationship = 20836644000.0 | Hz
 kelvin_hyphen_joule_relationship = 1.3806504e-23 | J
 kelvin_hyphen_kilogram_relationship = 1.5361807e-40 | kg
-kilogram_hyphen_hertz_relationship = 1.356392733e+50 | Hz
-kilogram_hyphen_joule_relationship = 8.987551787e+16 | J
-kilogram_hyphen_kelvin_relationship = 6.509651e+39 | K
+kilogram_hyphen_hertz_relationship = 1.356392733e50 | Hz
+kilogram_hyphen_joule_relationship = 8.987551787e16 | J
+kilogram_hyphen_kelvin_relationship = 6.509651e39 | K
 lattice_parameter_of_silicon = 5.43102064e-10 | m
 mag_flux_quantum = 2.067833667e-15 | Wb
 Mo_x_unit = 1.00209955e-13 | m
 muon_Compton_wavelength = 1.173444104e-14 | m
 muon_Compton_wavelength_over_2_pi = 1.867594295e-15 | m
 muon_mass = 1.8835313e-28 | kg
 muon_mass_energy_equivalent = 1.69283351e-11 | J
@@ -82,129 +84,129 @@
 natural_unit_of_time = 1.288088657e-21 | s
 neutron_Compton_wavelength = 1.3195908951e-15 | m
 neutron_Compton_wavelength_over_2_pi = 2.1001941382e-16 | m
 neutron_mass = 1.674927211e-27 | kg
 neutron_mass_energy_equivalent = 1.505349505e-10 | J
 Planck_length = 1.616252e-35 | m
 Planck_mass = 2.17644e-08 | kg
-Planck_temperature = 1.416785e+32 | K
+Planck_temperature = 1.416785e32 | K
 Planck_time = 5.39124e-44 | s
 proton_Compton_wavelength = 1.3214098446e-15 | m
 proton_Compton_wavelength_over_2_pi = 2.1030890861e-16 | m
 proton_mass = 1.672621637e-27 | kg
 proton_mass_energy_equivalent = 1.503277359e-10 | J
 proton_rms_charge_radius = 8.768e-16 | m
-Rydberg_constant_times_c_in_Hz = 3.28984196036e+15 | Hz
+Rydberg_constant_times_c_in_Hz = 3.28984196036e15 | Hz
 Rydberg_constant_times_hc_in_J = 2.17987197e-18 | J
 standard_atmosphere = 101325.0 | Pa
 tau_Compton_wavelength = 6.9772e-16 | m
 tau_Compton_wavelength_over_2_pi = 1.11046e-16 | m
 tau_mass = 3.16777e-27 | kg
 tau_mass_energy_equivalent = 2.84705e-10 | J
 triton_mass = 5.00735588e-27 | kg
 triton_mass_energy_equivalent = 4.50038703e-10 | J
 unified_atomic_mass_unit = 1.660538782e-27 | kg
 von_Klitzing_constant = 25812.807557 | ohm
-#DERIVED UNITS***********************************************
-alpha_particle_molar_mass = 0.00400150617913 | kg*mol**-1
-atomic_mass_unit_hyphen_inverse_meter_relationship = 7.513006671e+14 | m**-1
-atomic_unit_of_1st_hyperpolarizablity = 3.206361533e-53 | C**3*m**3*J**-2
-atomic_unit_of_2nd_hyperpolarizablity = 6.23538095e-65 | C**4*m**4*J**-3
-atomic_unit_of_action = 1.054571628e-34 | J*s
-atomic_unit_of_charge_density = 1.0812023e+12 | C*m**-3
-atomic_unit_of_electric_dipole_mom = 8.47835281e-30 | C*m
-atomic_unit_of_electric_field = 5.14220632e+11 | V*m**-1
-atomic_unit_of_electric_field_gradient = 9.71736166e+21 | V*m**-2
-atomic_unit_of_electric_polarizablity = 1.6487772536e-41 | C**2*m**2*J**-1
-atomic_unit_of_electric_quadrupole_mom = 4.48655107e-40 | C*m**2
-atomic_unit_of_mag_dipole_mom = 1.85480183e-23 | J*T**-1
-atomic_unit_of_magnetizability = 7.891036433e-29 | J*T**-2
-atomic_unit_of_momentum = 1.992851565e-24 | kg*m*s**-1
-atomic_unit_of_permittivity = 1.112650056e-10 | F*m**-1
-atomic_unit_of_velocity = 2187691.2541 | m*s**-1
-Avogadro_constant = 6.02214179e+23 | mol**-1
-Bohr_magneton = 9.27400915e-24 | J*T**-1
-Bohr_magneton_in_Hz_div_T = 13996246040.0 | Hz*T**-1
-Bohr_magneton_in_inverse_meters_per_tesla = 46.6864515 | m**-1*T**-1
-Bohr_magneton_in_K_div_T = 0.6717131 | K*T**-1
-kB = 1.3806504e-23 | J*K**-1
-Boltzmann_constant_in_Hz_div_K = 20836644000.0 | Hz*K**-1
-Boltzmann_constant_in_inverse_meters_per_kelvin = 69.50356 | m**-1*K**-1
-conventional_value_of_Josephson_constant = 4.835979e+14 | Hz*V**-1
-deuteron_mag_mom = 4.33073465e-27 | J*T**-1
-deuteron_molar_mass = 0.00201355321272 | kg*mol**-1
-electric_constant = 8.854187817e-12 | F*m**-1
-electron_charge_to_mass_quotient = -1.75882015e+11 | C*kg**-1
-electron_gyromag_ratio = 1.76085977e+11 | s**-1*T**-1
-electron_gyromag_ratio_over_2_pi = 28024.95364 | MHz*T**-1
-electron_mag_mom = -9.28476377e-24 | J*T**-1
-electron_molar_mass = 5.4857990943e-07 | kg*mol**-1
+# DERIVED UNITS***********************************************
+alpha_particle_molar_mass = 0.00400150617913 | kg * mol**-1
+atomic_mass_unit_hyphen_inverse_meter_relationship = 7.513006671e14 | m**-1
+atomic_unit_of_1st_hyperpolarizablity = 3.206361533e-53 | C**3 * m**3 * J**-2
+atomic_unit_of_2nd_hyperpolarizablity = 6.23538095e-65 | C**4 * m**4 * J**-3
+atomic_unit_of_action = 1.054571628e-34 | J * s
+atomic_unit_of_charge_density = 1.0812023e12 | C * m**-3
+atomic_unit_of_electric_dipole_mom = 8.47835281e-30 | C * m
+atomic_unit_of_electric_field = 5.14220632e11 | V * m**-1
+atomic_unit_of_electric_field_gradient = 9.71736166e21 | V * m**-2
+atomic_unit_of_electric_polarizablity = 1.6487772536e-41 | C**2 * m**2 * J**-1
+atomic_unit_of_electric_quadrupole_mom = 4.48655107e-40 | C * m**2
+atomic_unit_of_mag_dipole_mom = 1.85480183e-23 | J * T**-1
+atomic_unit_of_magnetizability = 7.891036433e-29 | J * T**-2
+atomic_unit_of_momentum = 1.992851565e-24 | kg * m * s**-1
+atomic_unit_of_permittivity = 1.112650056e-10 | F * m**-1
+atomic_unit_of_velocity = 2187691.2541 | m * s**-1
+Avogadro_constant = 6.02214179e23 | mol**-1
+Bohr_magneton = 9.27400915e-24 | J * T**-1
+Bohr_magneton_in_Hz_div_T = 13996246040.0 | Hz * T**-1
+Bohr_magneton_in_inverse_meters_per_tesla = 46.6864515 | m**-1 * T**-1
+Bohr_magneton_in_K_div_T = 0.6717131 | K * T**-1
+kB = 1.3806504e-23 | J * K**-1
+Boltzmann_constant_in_Hz_div_K = 20836644000.0 | Hz * K**-1
+Boltzmann_constant_in_inverse_meters_per_kelvin = 69.50356 | m**-1 * K**-1
+conventional_value_of_Josephson_constant = 4.835979e14 | Hz * V**-1
+deuteron_mag_mom = 4.33073465e-27 | J * T**-1
+deuteron_molar_mass = 0.00201355321272 | kg * mol**-1
+electric_constant = 8.854187817e-12 | F * m**-1
+electron_charge_to_mass_quotient = -1.75882015e11 | C * kg**-1
+electron_gyromag_ratio = 1.76085977e11 | s**-1 * T**-1
+electron_gyromag_ratio_over_2_pi = 28024.95364 | MHz * T**-1
+electron_mag_mom = -9.28476377e-24 | J * T**-1
+electron_molar_mass = 5.4857990943e-07 | kg * mol**-1
 electron_volt_hyphen_inverse_meter_relationship = 806554.465 | m**-1
-elementary_charge_over_h = 2.417989454e+14 | A*J**-1
-Faraday_constant = 96485.3399 | C*mol**-1
-first_radiation_constant = 3.74177118e-16 | W*m**2
-first_radiation_constant_for_spectral_radiance = 1.191042759e-16 | W*m**2*sr**-1
+elementary_charge_over_h = 2.417989454e14 | A * J**-1
+Faraday_constant = 96485.3399 | C * mol**-1
+first_radiation_constant = 3.74177118e-16 | W * m**2
+first_radiation_constant_for_spectral_radiance = 1.191042759e-16 | W * m**2 * sr**-1
 hartree_hyphen_inverse_meter_relationship = 21947463.137 | m**-1
-helion_molar_mass = 0.0030149322473 | kg*mol**-1
+helion_molar_mass = 0.0030149322473 | kg * mol**-1
 hertz_hyphen_inverse_meter_relationship = 3.335640951e-09 | m**-1
-Josephson_constant = 4.83597891e+14 | Hz*V**-1
-joule_hyphen_inverse_meter_relationship = 5.03411747e+24 | m**-1
+Josephson_constant = 4.83597891e14 | Hz * V**-1
+joule_hyphen_inverse_meter_relationship = 5.03411747e24 | m**-1
 kelvin_hyphen_inverse_meter_relationship = 69.50356 | m**-1
-kilogram_hyphen_inverse_meter_relationship = 4.52443915e+41 | m**-1
-Loschmidt_constant_X27315_K_and__101325_kPaX = 2.6867774e+25 | m**-3
-mag_constant = 1.2566370614e-06 | N*A**-2
-molar_gas_constant = 8.314472 | J*mol**-1*K**-1
-molar_mass_constant = 0.001 | kg*mol**-1
-molar_mass_of_carbon_hyphen_12 = 0.012 | kg*mol**-1
-molar_Planck_constant = 3.9903126821e-10 | J*s*mol**-1
-molar_Planck_constant_times_c = 0.11962656472 | J*m*mol**-1
-molar_volume_of_ideal_gas_X27315_K_and__100_kPaX = 0.022710981 | m**3*mol**-1
-molar_volume_of_ideal_gas_X27315_K_and__101325_kPaX = 0.022413996 | m**3*mol**-1
-molar_volume_of_silicon = 1.20588349e-05 | m**3*mol**-1
-muon_mag_mom = -4.49044786e-26 | J*T**-1
-muon_molar_mass = 0.0001134289256 | kg*mol**-1
-natural_unit_of_action = 1.054571628e-34 | J*s
-natural_unit_of_momentum = 2.73092406e-22 | kg*m*s**-1
-natural_unit_of_velocity = 299792458.0 | m*s**-1
-neutron_gyromag_ratio = 183247185.0 | s**-1*T**-1
-neutron_gyromag_ratio_over_2_pi = 29.1646954 | MHz*T**-1
-neutron_mag_mom = -9.6623641e-27 | J*T**-1
-neutron_molar_mass = 0.00100866491597 | kg*mol**-1
-G = 6.67428e-11 | m**3*kg**-1*s**-2
-nuclear_magneton = 5.05078324e-27 | J*T**-1
-nuclear_magneton_in_inverse_meters_per_tesla = 0.02542623616 | m**-1*T**-1
-nuclear_magneton_in_K_div_T = 0.00036582637 | K*T**-1
-nuclear_magneton_in_MHz_div_T = 7.62259384 | MHz*T**-1
-h = 6.62606896e-34 | J*s
-Planck_constant_over_2_pi = 1.054571628e-34 | J*s
-proton_charge_to_mass_quotient = 95788339.2 | C*kg**-1
-proton_gyromag_ratio = 267522209.9 | s**-1*T**-1
-proton_gyromag_ratio_over_2_pi = 42.5774821 | MHz*T**-1
-proton_mag_mom = 1.410606662e-26 | J*T**-1
-proton_molar_mass = 0.00100727646677 | kg*mol**-1
-quantum_of_circulation = 0.00036369475199 | m**2*s**-1
-quantum_of_circulation_times_2 = 0.000727389504 | m**2*s**-1
+kilogram_hyphen_inverse_meter_relationship = 4.52443915e41 | m**-1
+Loschmidt_constant_X27315_K_and__101325_kPaX = 2.6867774e25 | m**-3
+mag_constant = 1.2566370614e-06 | N * A**-2
+molar_gas_constant = 8.314472 | J * mol**-1 * K**-1
+molar_mass_constant = 0.001 | kg * mol**-1
+molar_mass_of_carbon_hyphen_12 = 0.012 | kg * mol**-1
+molar_Planck_constant = 3.9903126821e-10 | J * s * mol**-1
+molar_Planck_constant_times_c = 0.11962656472 | J * m * mol**-1
+molar_volume_of_ideal_gas_X27315_K_and__100_kPaX = 0.022710981 | m**3 * mol**-1
+molar_volume_of_ideal_gas_X27315_K_and__101325_kPaX = 0.022413996 | m**3 * mol**-1
+molar_volume_of_silicon = 1.20588349e-05 | m**3 * mol**-1
+muon_mag_mom = -4.49044786e-26 | J * T**-1
+muon_molar_mass = 0.0001134289256 | kg * mol**-1
+natural_unit_of_action = 1.054571628e-34 | J * s
+natural_unit_of_momentum = 2.73092406e-22 | kg * m * s**-1
+natural_unit_of_velocity = 299792458.0 | m * s**-1
+neutron_gyromag_ratio = 183247185.0 | s**-1 * T**-1
+neutron_gyromag_ratio_over_2_pi = 29.1646954 | MHz * T**-1
+neutron_mag_mom = -9.6623641e-27 | J * T**-1
+neutron_molar_mass = 0.00100866491597 | kg * mol**-1
+G = 6.67428e-11 | m**3 * kg**-1 * s**-2
+nuclear_magneton = 5.05078324e-27 | J * T**-1
+nuclear_magneton_in_inverse_meters_per_tesla = 0.02542623616 | m**-1 * T**-1
+nuclear_magneton_in_K_div_T = 0.00036582637 | K * T**-1
+nuclear_magneton_in_MHz_div_T = 7.62259384 | MHz * T**-1
+h = 6.62606896e-34 | J * s
+Planck_constant_over_2_pi = 1.054571628e-34 | J * s
+proton_charge_to_mass_quotient = 95788339.2 | C * kg**-1
+proton_gyromag_ratio = 267522209.9 | s**-1 * T**-1
+proton_gyromag_ratio_over_2_pi = 42.5774821 | MHz * T**-1
+proton_mag_mom = 1.410606662e-26 | J * T**-1
+proton_molar_mass = 0.00100727646677 | kg * mol**-1
+quantum_of_circulation = 0.00036369475199 | m**2 * s**-1
+quantum_of_circulation_times_2 = 0.000727389504 | m**2 * s**-1
 Rydberg_constant = 10973731.5685 | m**-1
-second_radiation_constant = 0.014387752 | m*K
-shielded_helion_gyromag_ratio = 203789473.0 | s**-1*T**-1
-shielded_helion_gyromag_ratio_over_2_pi = 32.43410198 | MHz*T**-1
-shielded_helion_mag_mom = -1.074552982e-26 | J*T**-1
-shielded_proton_gyromag_ratio = 267515336.2 | s**-1*T**-1
-shielded_proton_gyromag_ratio_over_2_pi = 42.5763881 | MHz*T**-1
-shielded_proton_mag_mom = 1.410570419e-26 | J*T**-1
-c = 299792458.0 | m*s**-1
-standard_acceleration_of_gravity = 9.80665 | m*s**-2
-Stefan_hyphen_Boltzmann_constant = 5.6704e-08 | W*m**-2*K**-4
-tau_molar_mass = 0.00190768 | kg*mol**-1
+second_radiation_constant = 0.014387752 | m * K
+shielded_helion_gyromag_ratio = 203789473.0 | s**-1 * T**-1
+shielded_helion_gyromag_ratio_over_2_pi = 32.43410198 | MHz * T**-1
+shielded_helion_mag_mom = -1.074552982e-26 | J * T**-1
+shielded_proton_gyromag_ratio = 267515336.2 | s**-1 * T**-1
+shielded_proton_gyromag_ratio_over_2_pi = 42.5763881 | MHz * T**-1
+shielded_proton_mag_mom = 1.410570419e-26 | J * T**-1
+c = 299792458.0 | m * s**-1
+standard_acceleration_of_gravity = 9.80665 | m * s**-2
+Stefan_hyphen_Boltzmann_constant = 5.6704e-08 | W * m**-2 * K**-4
+tau_molar_mass = 0.00190768 | kg * mol**-1
 Thomson_cross_section = 6.652458558e-29 | m**2
-triton_mag_mom = 1.504609361e-26 | J*T**-1
-triton_molar_mass = 0.0030155007134 | kg*mol**-1
-Wien_frequency_displacement_law_constant = 58789330000.0 | Hz*K**-1
-Wien_wavelength_displacement_law_constant = 0.0028977685 | m*K
-#RATIOS ***********************************************
+triton_mag_mom = 1.504609361e-26 | J * T**-1
+triton_molar_mass = 0.0030155007134 | kg * mol**-1
+Wien_frequency_displacement_law_constant = 58789330000.0 | Hz * K**-1
+Wien_wavelength_displacement_law_constant = 0.0028977685 | m * K
+# RATIOS ***********************************************
 alpha_particle_hyphen_electron_mass_ratio = 7294.2995365 | none
 alpha_particle_hyphen_proton_mass_ratio = 3.97259968951 | none
 deuteron_hyphen_electron_mag_mom_ratio = -0.0004664345537 | none
 deuteron_hyphen_electron_mass_ratio = 3670.4829654 | none
 deuteron_g_factor = 0.8574382308 | none
 deuteron_mag_mom_to_Bohr_magneton_ratio = 0.0004669754556 | none
 deuteron_mag_mom_to_nuclear_magneton_ratio = 0.8574382308 | none
@@ -276,25 +278,25 @@
 triton_g_factor = 5.957924896 | none
 triton_mag_mom_to_Bohr_magneton_ratio = 0.001622393657 | none
 triton_mag_mom_to_nuclear_magneton_ratio = 2.978962448 | none
 triton_hyphen_neutron_mag_mom_ratio = -1.55718553 | none
 triton_hyphen_proton_mag_mom_ratio = 1.066639908 | none
 triton_hyphen_proton_mass_ratio = 2.9937170309 | none
 weak_mixing_angle = 0.22255 | none
-#DERIVED CONSTANTS***********************************************
+# DERIVED CONSTANTS***********************************************
 pi = numpy.pi
 hbar = h / (2.0 * numpy.pi)
 four_pi_stefan_boltzmann = 4.0 * numpy.pi * Stefan_hyphen_Boltzmann_constant
-mu0 = 4 * numpy.pi * 1.e-7 | N/A**2
+mu0 = 4 * numpy.pi * 1.0e-7 | N / A**2
 eps0 = mu0**-1 * c**-2
 sidereal_day = 86164.100352 | s
-#machine constants
+# machine constants
 eps = numpy.finfo(numpy.double).eps
-precision = int(numpy.log10(2/eps))
-#DROPPED UNITS***********************************************
+precision = int(numpy.log10(2 / eps))
+# DROPPED UNITS***********************************************
 """alpha_particle_mass_energy_equivalent_in_MeV = 3727.379109 | MeV
 alpha_particle_mass_in_u = 4.00150617913 | u
 atomic_mass_constant_energy_equivalent_in_MeV = 931.494028 | MeV
 atomic_mass_unit_hyphen_electron_volt_relationship = 931494028.0 | eV
 atomic_mass_unit_hyphen_hartree_relationship = 34231777.149 | E_h
 Bohr_magneton_in_eV_div_T = 5.7883817555e-05 | eV*T**-1
 kBeV = 8.617343e-05 | eV*K**-1
```

### Comparing `amuse-framework-2023.5.0/src/amuse/units/core.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/core.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/units/generic_unit_converter.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/generic_unit_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,76 +69,87 @@
         >>> from amuse.units.generic_unit_converter import ConvertBetweenGenericAndSiUnits
         >>> from amuse.units import units, constants
         >>> converter = ConvertBetweenGenericAndSiUnits(constants.c, units.m)
 
     """
 
     def __init__(self, *arguments_list):
-        
+
         self.check_arguments(arguments_list)
         
         self.values = arguments_list
         
         self.units_of_values = [x.unit for x in self.values]
         self.system_rank = len(self.values)
         
-        self.new_base = numpy.mat(numpy.zeros((self.system_rank,self.system_rank)))
-        self.new_base_inv = numpy.mat(numpy.zeros((self.system_rank,self.system_rank)))
+        self.new_base = numpy.zeros((self.system_rank,self.system_rank))
+        self.new_base_inv = numpy.zeros((self.system_rank,self.system_rank))
     
         available_units = set()
         for unit in self.units_of_values:
             for factor, base_unit in unit.base:
                 available_units.add(base_unit)
-        if not len(available_units) is self.system_rank:
+        if len(available_units) is not self.system_rank:
             raise UnitsNotOrtogonalException(self.system_rank, len(available_units))
-        self.list_of_available_units = list(available_units)
-    
+        self.list_of_available_units = numpy.array(list(available_units))
+
         self.new_base = self.determine_new_base()
         rank_of_new_base = self.matrixrank(self.new_base)
         if rank_of_new_base < self.system_rank:
             raise UnitsNotOrtogonalException(self.system_rank, rank_of_new_base)
-        self.new_base_inv = self.new_base ** -1
+        self.new_base_inv = numpy.linalg.matrix_power(self.new_base, -1)
 
     def check_arguments(self, arguments):
         
         for index, x in enumerate(arguments):
             if is_unit(x):
                 continue
             if not is_quantity(x):
                 raise NotAQuantityException(index, x)
             if not x.is_scalar():
                 raise NotAScalarException(index, x)
-        
+
     def matrixrank(self, A, tol=1e-8):
-        s = numpy.linalg.svd(A,compute_uv=0)
-        return numpy.sum(numpy.where( s>tol, 1, 0 ) )
+        s = numpy.linalg.svd(A, compute_uv=0)
+        return numpy.sum(numpy.where(s > tol, 1, 0))
 
     def determine_new_base(self):
-        matrix = numpy.asmatrix(numpy.zeros((self.system_rank,self.system_rank)))
+        matrix = numpy.zeros((self.system_rank, self.system_rank))
         for row, value in enumerate(self.values):
             for n, unit in value.unit.base:
-                matrix[row, [i for i, j in enumerate(self.list_of_available_units) if j == unit]] = n
+                matrix[
+                    row,
+                    [
+                        column for column, available_unit in enumerate(
+                            self.list_of_available_units
+                        ) if available_unit == unit
+                    ]
+                ] = n
         return matrix
 
     @late
     def conversion_factors(self):
-        factors_of_the_bases = numpy.asmatrix(numpy.zeros((self.system_rank,1)))
+        factors_of_the_bases = numpy.zeros((self.system_rank,1))
         for row, value in enumerate(self.values):
             factors_of_the_bases[row] = value.number * value.unit.factor
         log_factors_of_the_bases = numpy.log(numpy.abs(factors_of_the_bases))
-        result = numpy.array(numpy.exp(self.new_base_inv*log_factors_of_the_bases))[:,0]
+        result = numpy.array(
+            numpy.exp(
+                numpy.matmul(self.new_base_inv, log_factors_of_the_bases)
+            )
+        )[:,0]
         return result
 
     @late
     def units(self):
         conversion_factors = self.conversion_factors
         result = []
         generic_units = mass, length, time, temperature, current, luminous_intensity
 
-        for n, unit  in enumerate(self.list_of_available_units):
+        for n, unit in enumerate(self.list_of_available_units):
             conversion_factor_for_this_base_unit = conversion_factors[n]
             for generic_unit in generic_units:
                 if generic_unit.unit_in_si == unit:
                     result.append((generic_unit, conversion_factor_for_this_base_unit * unit))
 
         return result
```

### Comparing `amuse-framework-2023.5.0/src/amuse/units/generic_unit_system.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/generic_unit_system.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/units/nbody_system.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/nbody_system.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,90 +49,95 @@
 from amuse.units.quantities import new_quantity
 from amuse.support import exceptions
 
 import numpy
 
 """
 """
+
+
 class nbody_unit(core.base_unit):
     def __init__(self, unit_in_si, system):
-        core.base_unit.__init__(self, unit_in_si.quantity, unit_in_si.name, unit_in_si.symbol, system)
+        core.base_unit.__init__(
+            self, unit_in_si.quantity, unit_in_si.name, unit_in_si.symbol, system
+        )
         self.unit_in_si = unit_in_si
-        
+
     def __str__(self):
-        return 'nbody '+self.unit_in_si.quantity
-        
-  
+        return "nbody " + self.unit_in_si.quantity
 
     def is_generic(self):
         return True
-    
+
+
 length = generic_unit_system.length
-time =  generic_unit_system.time
-mass =  generic_unit_system.mass
+time = generic_unit_system.time
+mass = generic_unit_system.mass
 
-acceleration = length / (time ** 2)
-potential = (length ** 2) / (time ** 2)
+acceleration = length / (time**2)
+potential = (length**2) / (time**2)
 energy = mass * potential
 specific_energy = potential
 speed = length / time
-volume = (length ** 3)
+volume = length**3
 density = mass / volume
-pressure = mass / length / (time ** 2)
+pressure = mass / length / (time**2)
 momentum_density = density * speed
 energy_density = density * specific_energy
-G = 1. | (length**3) / (mass * (time**2))
+G = 1.0 | (length**3) / (mass * (time**2))
+
 
 def is_nbody_unit(unit):
     for factor, x in unit.base:
         if x.is_generic():
             return True
     return False
-    
+
+
 class SiToNBodyConverter(object):
     def __init__(self, nbody_to_si):
         self.nbody_to_si = nbody_to_si
-    
+
     def from_source_to_target(self, quantity):
-        if hasattr(quantity, 'unit') and not quantity.unit.is_non_numeric():
+        if hasattr(quantity, "unit") and not quantity.unit.is_non_numeric():
             return self.nbody_to_si.to_nbody(quantity)
         else:
             return quantity
-        
+
     def from_target_to_source(self, quantity):
-        if hasattr(quantity, 'unit') and not quantity.unit.is_non_numeric():
+        if hasattr(quantity, "unit") and not quantity.unit.is_non_numeric():
             return self.nbody_to_si.to_si(quantity)
         else:
             return quantity
-    
-class nbody_to_si(generic_unit_converter.ConvertBetweenGenericAndSiUnits): 
+
+
+class nbody_to_si(generic_unit_converter.ConvertBetweenGenericAndSiUnits):
     def __init__(self, value1, value2):
-        generic_unit_converter.ConvertBetweenGenericAndSiUnits.__init__(self,constants.G, value1, value2)
-        
+        generic_unit_converter.ConvertBetweenGenericAndSiUnits.__init__(
+            self, constants.G, value1, value2
+        )
+
     def to_nbody(self, value):
         return self.to_generic(value)
-        
-    
+
     def _old_unit_to_unit_in_nbody(self, unit):
         nbody_units_in_si = self.units
         base = unit.base
         factor = unit.factor
         new_unit = 1
         for n, unit in base:
             unit_in_nbody, unit_in_si = self.find_nbody_unit_for(unit)
             if not unit_in_si is None:
-                factor = factor / (unit_in_si.factor ** n)
-                new_unit *= (unit_in_nbody.base[0][1] ** n)
+                factor = factor / (unit_in_si.factor**n)
+                new_unit *= unit_in_nbody.base[0][1] ** n
             else:
-                new_unit *= (unit ** n)
+                new_unit *= unit**n
         return factor * new_unit
-        
+
     def as_converter_from_si_to_nbody(self):
         return self.as_converter_from_si_to_generic()
-        
+
     def as_converter_from_nbody_to_si(self):
         return self.as_converter_from_generic_to_si()
 
-
     def as_converter_from_si_to_generic(self):
         return SiToNBodyConverter(self)
-
```

### Comparing `amuse-framework-2023.5.0/src/amuse/units/nist.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/nist.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/units/nist.txt` & `amuse_framework-2024.4.0rc1/src/amuse/units/nist.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/units/nist2010.txt` & `amuse_framework-2024.4.0rc1/src/amuse/units/nist2010.txt`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/src/amuse/units/optparse.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/optparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-
+"""
+Overloaded option parser with unit support.
+Now deprecated, standard argparse can be used instead.
+"""
 
 import optparse
 import textwrap
 from amuse.units import quantities
 
 def check_builtin_unit(option, opt, value):
     (cvt, what) = optparse._builtin_cvt[option.type]
```

### Comparing `amuse-framework-2023.5.0/src/amuse/units/quantities.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/quantities.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from amuse.units import core
 from amuse.units.si import none
 from amuse.units.core import zero_unit
 
 try:
     import astropy.units
     import amuse.units.si
+
     HAS_ASTROPY = True
 except ImportError:
     HAS_ASTROPY = False
 
 
 class Quantity:
     """
@@ -68,15 +69,16 @@
     >>> x.value_in(units.g) # but only if the units are compatible!
     Traceback (most recent call last):
         File "<stdin>", line 1, in ?
     IncompatibleUnitsException: Cannot express m in g, the units do not have the same bases
 
 
     """
-    __slots__ = ['unit']
+
+    __slots__ = ["unit"]
 
     __array_priority__ = 101
 
     def __init__(self, unit):
         self.unit = unit
 
     def __str__(self):
@@ -97,24 +99,25 @@
     def is_vector(self):
         """
         True for vector quantities.
         """
         return False
 
     def __repr__(self):
-        return 'quantity<'+str(self)+'>'
+        return "quantity<" + str(self) + ">"
 
     def __add__(self, other):
         if self.unit.is_zero():
-            other=to_quantity(other)
+            other = to_quantity(other)
             return new_quantity(other.number, other.unit)
         else:
             other = to_quantity(other)
             factor = other.unit.conversion_factor_from(self.unit)
-            return new_quantity(self.number + factor*other.number, self.unit)
+            return new_quantity(self.number + factor * other.number, self.unit)
+
     __radd__ = __add__
 
     def __sub__(self, other):
         if self.unit.is_zero():
             return -other
         else:
             other_in_my_units = to_quantity(other).as_quantity_in(self.unit)
@@ -124,66 +127,89 @@
         if self.unit.is_zero():
             return new_quantity(other.number, other.unit)
         other_in_my_units = to_quantity(other).as_quantity_in(self.unit)
         return new_quantity(other_in_my_units.number - self.number, self.unit)
 
     def __mul__(self, other):
         other = to_quantity(other)
-        return new_quantity_nonone(self.number * other.number, (self.unit * other.unit).to_simple_form())
+        return new_quantity_nonone(
+            self.number * other.number, (self.unit * other.unit).to_simple_form()
+        )
 
     __rmul__ = __mul__
 
     def __pow__(self, other):
-        return new_quantity(self.number ** other, self.unit ** other)
+        return new_quantity(self.number**other, self.unit**other)
 
     def __truediv__(self, other):
         other = to_quantity(other)
-        return new_quantity_nonone(operator.__truediv__(self.number,other.number), (self.unit / other.unit).to_simple_form())
+        return new_quantity_nonone(
+            operator.__truediv__(self.number, other.number),
+            (self.unit / other.unit).to_simple_form(),
+        )
 
     def __rtruediv__(self, other):
-        return new_quantity_nonone(operator.__truediv__(other,self.number), (1.0 / self.unit).to_simple_form())
+        return new_quantity_nonone(
+            operator.__truediv__(other, self.number), (1.0 / self.unit).to_simple_form()
+        )
 
     def __floordiv__(self, other):
         other = to_quantity(other)
-        return new_quantity_nonone(operator.__floordiv__(self.number,other.number), (self.unit / other.unit).to_simple_form())
+        return new_quantity_nonone(
+            operator.__floordiv__(self.number, other.number),
+            (self.unit / other.unit).to_simple_form(),
+        )
 
     def __rfloordiv__(self, other):
-        return new_quantity_nonone(operator.__floordiv__(other,self.number), (1.0 / self.unit).to_simple_form())
+        return new_quantity_nonone(
+            operator.__floordiv__(other, self.number),
+            (1.0 / self.unit).to_simple_form(),
+        )
 
     def __div__(self, other):
         other = to_quantity(other)
-        return new_quantity_nonone(self.number/other.number, (self.unit / other.unit).to_simple_form())
+        return new_quantity_nonone(
+            self.number / other.number, (self.unit / other.unit).to_simple_form()
+        )
 
     def __rdiv__(self, other):
-        return new_quantity_nonone(other/self.number, (1.0 / self.unit).to_simple_form())
+        return new_quantity_nonone(
+            other / self.number, (1.0 / self.unit).to_simple_form()
+        )
 
     def __mod__(self, other):
         other_in_my_units = to_quantity(other).as_quantity_in(self.unit)
-        return new_quantity_nonone(numpy.mod(self.number , other_in_my_units.number), self.unit)
+        return new_quantity_nonone(
+            numpy.mod(self.number, other_in_my_units.number), self.unit
+        )
 
     def __rmod__(self, other):
         other_in_my_units = to_quantity(other).as_quantity_in(self.unit)
-        return new_quantity_nonone(numpy.mod(other_in_my_units.number , self.number), self.unit)
+        return new_quantity_nonone(
+            numpy.mod(other_in_my_units.number, self.number), self.unit
+        )
 
     def in_base(self):
-        unit=self.unit.base_unit()
+        unit = self.unit.base_unit()
         return self.as_quantity_in(unit)
 
     def sqrt(self):
         """Calculate the square root of each component
 
         >>> from amuse.units import units
         >>> s1 = 144.0 | units.m**2
         >>> s1.sqrt()
         quantity<12.0 m>
         >>> v1 = [16.0, 25.0, 36.0] | units.kg
         >>> v1.sqrt()
         quantity<[4.0, 5.0, 6.0] kg**0.5>
         """
-        return new_quantity(numpy.sqrt(self.number), (self.unit ** 0.5).to_simple_form())
+        return new_quantity(
+            numpy.sqrt(self.number), (self.unit**0.5).to_simple_form()
+        )
 
     def as_quantity_in(self, another_unit):
         """
         Reproduce quantity in another unit.
         The new unit must have the same basic si quantities.
 
         :argument another_unit: unit to convert quantity to
@@ -200,15 +226,17 @@
         """
         Create a string representing the quantity in another unit.
         The new unit must have the same basic si quantities.
 
         :argument another_unit: unit to convert quantity to
         :returns: string representing quantity converted to new unit
         """
-        return console.DefaultPrintingStrategy().quantity_to_string(self.as_quantity_in(another_unit))
+        return console.DefaultPrintingStrategy().quantity_to_string(
+            self.as_quantity_in(another_unit)
+        )
 
     def value_in(self, unit):
         """
         Return a numeric value (for scalars) or array (for vectors)
         in the given unit.
 
         A number is returned without any unit information. Use this
@@ -264,24 +292,26 @@
     def __le__(self, other):
         return self.value_in(self.unit) <= to_quantity(other).value_in(self.unit)
 
     def __ge__(self, other):
         return self.value_in(self.unit) >= to_quantity(other).value_in(self.unit)
 
     if HAS_ASTROPY:
+
         def as_astropy_quantity(self):
             return to_astropy(self)
 
 
 class ScalarQuantity(Quantity):
     """
     A ScalarQuantity object represents a physical scalar
     quantity.
     """
-    __slots__ = ['number']
+
+    __slots__ = ["number"]
 
     def __init__(self, number, unit):
         # Quantity.__init__(self, unit)
         # commented out super call, this speeds thing up
         self.unit = unit
         if isinstance(number, str):
             try:
@@ -292,152 +322,175 @@
             self.number = number
         else:
             if isinstance(unit.dtype, numpy.dtype):
                 self.number = unit.dtype.type(number)
             else:
                 self.number = unit.dtype(number)
 
-
     def is_scalar(self):
         return True
 
     def as_vector_with_length(self, length):
-        return VectorQuantity(numpy.ones(length, dtype=self.unit.dtype) * self.number, self.unit)
-
+        return VectorQuantity(
+            numpy.ones(length, dtype=self.unit.dtype) * self.number, self.unit
+        )
 
     def reshape(self, shape):
         if shape == -1 or (len(shape) == 1 and shape[0] == 1):
             return VectorQuantity([self.number], self.unit)
         else:
-            raise exceptions.AmuseException("Cannot reshape a scalar to vector of shape '{0}'".format(shape))
+            raise exceptions.AmuseException(
+                "Cannot reshape a scalar to vector of shape '{0}'".format(shape)
+            )
 
     def __getitem__(self, index):
         if index == 0:
             return self
         else:
             raise exceptions.AmuseException("ScalarQuantity does not support indexing")
 
     def copy(self):
         return new_quantity(self.number, self.unit)
 
     def to_unit(self):
-        in_base=self.in_base()
+        in_base = self.in_base()
         return in_base.number * in_base.unit
 
     def __getstate__(self):
         return (self.unit, self.number)
 
-    def round(self, decimals = 0):
+    def round(self, decimals=0):
         return new_quantity(numpy.round(self.number, decimals), self.unit)
 
-
     def new_zeros_array(self, length):
         array = numpy.zeros(length, dtype=self.unit.dtype)
         return new_quantity(array, self.unit)
 
     def __setstate__(self, x):
         self.unit = x[0]
         self.number = x[1]
 
     def sum(self, axis=None, dtype=None, out=None):
         return self
+
     def cumsum(self, axis=None, dtype=None, out=None):
         return self
+
     def prod(self, axis=None, dtype=None):
         return self
-    def min(self, axis = None):
+
+    def min(self, axis=None):
         return self
-    def max(self, axis = None):
+
+    def max(self, axis=None):
         return self
-    amin=min
-    amax=max
+
+    amin = min
+    amax = max
+
     def sorted(self):
         return self
 
     def as_unit(self):
         return self.number * self.unit
 
+
 class _flatiter_wrapper(object):
     def __init__(self, quantity):
-        self.flat=quantity.number.flat
-        self.quantity=quantity
+        self.flat = quantity.number.flat
+        self.quantity = quantity
+
     def __iter__(self):
         return self
+
     def __next__(self):
-        return new_quantity(next(self.flat),self.quantity.unit)
-    def __getitem__(self,x): 
+        return new_quantity(next(self.flat), self.quantity.unit)
+
+    def __getitem__(self, x):
         return new_quantity(self.flat[x], self.quantity.unit)
-    def __setitem__(self,index,x):
-        return self.flat.__setitem__(index,x.value_in(self.quantity.unit))
+
+    def __setitem__(self, index, x):
+        return self.flat.__setitem__(index, x.value_in(self.quantity.unit))
+
     @property
     def base(self):
         return self.quantity
+
     @property
     def index(self):
         return self.flat.index
+
     @property
     def coords(self):
         return self.flat.coords
+
     @property
     def unit(self):
         return self.quantity.unit
+
     @property
     def number(self):
         return self.flat
+
     def copy(self):
         return new_quantity(self.flat.copy(), self.quantity.unit)
+
     def is_quantity(self):
         return True
+
     def value_in(self, unit):
         return self.copy().value_in(unit)
+
     def as_quantity_in(self, unit):
         return self.copy().as_quantity_in(unit)
+
     # todo: add as required
 
+
 class VectorQuantity(Quantity):
     """
     A VectorQuantity object represents a physical vector
     quantity.
 
     >>> from amuse.units import units
     >>> v1 = [0.0, 1.0, 2.0] | units.kg
     >>> v2 = [2.0, 4.0, 6.0] | units.kg
     >>> v1 + v2
     quantity<[2.0, 5.0, 8.0] kg>
     >>> len(v1)
     3
     """
-    __slots__ = ['_number']
+
+    __slots__ = ["_number"]
 
     def __init__(self, array, unit):
         Quantity.__init__(self, unit)
         if unit is None:
-            self._number = numpy.array((), dtype='float64')
+            self._number = numpy.array((), dtype="float64")
         else:
             self._number = numpy.asarray(array, dtype=unit.dtype)
 
     @classmethod
     def new_from_scalar_quantities(cls, *values):
-        unit=to_quantity(values[0]).unit
+        unit = to_quantity(values[0]).unit
         try:
-            array=[value_in(x,unit) for x in values]
+            array = [value_in(x, unit) for x in values]
         except core.IncompatibleUnitsException:
             raise exceptions.AmuseException("not all values have conforming units")
         return cls(array, unit)
 
     @classmethod
     def new_from_array(cls, array):
-        shape=array.shape
-        vector=cls.new_from_scalar_quantities(*array.flat)
+        shape = array.shape
+        vector = cls.new_from_scalar_quantities(*array.flat)
         return vector.reshape(shape)
 
     def aszeros(self):
         return new_quantity(numpy.zeros(self.shape, dtype=self.number.dtype), self.unit)
 
-
     def new_zeros_array(self, length):
         array = numpy.zeros(length, dtype=self.unit.dtype)
         return type(self)(array, self.unit)
 
     @classmethod
     def zeros(cls, length, unit):
         array = numpy.zeros(length, dtype=unit.dtype)
@@ -453,56 +506,57 @@
 
     @property
     def dtype(self):
         return self.number.dtype
 
     def flatten(self):
         return new_quantity(self.number.flatten(), self.unit)
-    
+
     @property
-    def flat(self):                
+    def flat(self):
         return _flatiter_wrapper(self)
-        
+
     def is_vector(self):
         return True
 
-
     def as_vector_with_length(self, length):
-        if len(self)==length:
+        if len(self) == length:
             return self.copy()
-        if len(self)==1:
-            return self.new_from_scalar_quantities(*[self[0]]*length)
-        raise exceptions.AmuseException("as_vector_with_length only valid for same length or 1")
+        if len(self) == 1:
+            return self.new_from_scalar_quantities(*[self[0]] * length)
+        raise exceptions.AmuseException(
+            "as_vector_with_length only valid for same length or 1"
+        )
 
     def as_vector_quantity(self):
         return self
 
     def __len__(self):
         return len(self._number)
 
-    def split(self, indices_or_sections, axis = 0):
+    def split(self, indices_or_sections, axis=0):
         parts = numpy.split(self.number, indices_or_sections, axis)
         return [VectorQuantity(x, self.unit) for x in parts]
 
-    def array_split(self, indices_or_sections, axis = 0):
+    def array_split(self, indices_or_sections, axis=0):
         parts = numpy.array_split(self.number, indices_or_sections, axis)
         return [VectorQuantity(x, self.unit) for x in parts]
 
     def sum(self, axis=None, dtype=None, out=None):
         """Calculate the sum of the vector components
 
         >>> from amuse.units import units
         >>> v1 = [0.0, 1.0, 2.0] | units.kg
         >>> v1.sum()
         quantity<3.0 kg>
         """
         return new_quantity(self.number.sum(axis, dtype, out), self.unit)
 
     def cumsum(self, axis=None, dtype=None, out=None):
-        """ Calculate  the cumulative sum of the elements along a given axis. """
+        """Calculate  the cumulative sum of the elements along a given axis."""
 
         return new_quantity(numpy.cumsum(self.number, axis, dtype, out), self.unit)
 
     def prod(self, axis=None, dtype=None):
         """Calculate the product of the vector components
 
         >>> from amuse.units import units
@@ -524,31 +578,36 @@
         quantity<[[10.0, 6.0], [6.0, 16.0]] m**2>
         >>> v1.prod(1)
         quantity<[[4.0, 12.0], [15.0, 8.0]] m**2>
         >>> v1.prod(2)
         quantity<[[6.0, 8.0], [10.0, 12.0]] m**2>
         """
         if axis is None:
-            return new_quantity_nonone(self.number.prod(axis, dtype), self.unit ** numpy.prod(self.number.shape))
+            return new_quantity_nonone(
+                self.number.prod(axis, dtype),
+                self.unit ** numpy.prod(self.number.shape),
+            )
         else:
-            return new_quantity_nonone(self.number.prod(axis, dtype), self.unit ** self.number.shape[axis])
-
-
+            return new_quantity_nonone(
+                self.number.prod(axis, dtype), self.unit ** self.number.shape[axis]
+            )
 
     def inner(self, other):
         """Calculate the inner product of self with other.
 
         >>> from amuse.units import units
         >>> v1 = [1.0, 2.0, 3.0] | units.m
         >>> v1.inner(v1)
         quantity<14.0 m**2>
         """
         other = to_quantity(other)
-        return new_quantity_nonone(numpy.inner(self._number, other._number), (self.unit * other.unit).to_simple_form())
-
+        return new_quantity_nonone(
+            numpy.inner(self._number, other._number),
+            (self.unit * other.unit).to_simple_form(),
+        )
 
     def length_squared(self):
         """Calculate the squared length of the vector.
 
         >>> from amuse.units import units
         >>> v1 = [2.0, 3.0, 4.0] | units.m
         >>> v1.length_squared()
@@ -580,15 +639,17 @@
         """Calculate the length of the vectors in this vector
 
         >>> from amuse.units import units
         >>> v1 = [[0.0, 3.0, 4.0],[4.0, 2.0, 1.0]] | units.m
         >>> v1.lengths_squared()
         quantity<[25.0, 21.0] m**2>
         """
-        return (self.unit**2).new_quantity((self.number * self.number).sum(self.number.ndim - 1))
+        return (self.unit**2).new_quantity(
+            (self.number * self.number).sum(self.number.ndim - 1)
+        )
 
     def __getitem__(self, index):
         """Return the "index" component as a quantity.
 
         :argument index: index of the component, valid values
             for 3 dimensional vectors are: ``[0,1,2]``
         :returns: quantity with the same units
@@ -632,15 +693,21 @@
         >>> vector[1] = 3500 | g
         >>> print vector
         [0.0, 3.5, 2.0] kg
         """
         quantity = as_vector_quantity(quantity)
         if self.unit.is_zero():
             self.unit = quantity.unit
-        self._number[index] = quantity.value_in(self.unit)
+        if isinstance(quantity, VectorQuantity):
+            if len(quantity) == 1:
+                self._number[index] = quantity[0].value_in(self.unit)
+            else:
+                self._number[index] = quantity[:].value_in(self.unit)
+        else:
+            self._number[index] = quantity.value_in(self.unit)
 
     @property
     def number(self):
         return self._number
 
     @property
     def x(self):
@@ -693,30 +760,33 @@
 
     def norm_squared(self):
         return self.length_squared()
 
     def norm(self):
         return self.length()
 
-
     def append(self, scalar_quantity):
         """
         Append a scalar quantity to this vector.
 
         >>> from amuse.units import si
         >>> vector = [1.0, 2.0, 3.0] | si.kg
         >>> vector.append(4.0 | si.kg)
         >>> print vector
         [1.0, 2.0, 3.0, 4.0] kg
         """
-        append_number = numpy.array(scalar_quantity.value_in(self.unit)) # fix for deg, unitless
+        append_number = numpy.array(
+            scalar_quantity.value_in(self.unit)
+        )  # fix for deg, unitless
         # The following lines make sure that appending vectors works as expected,
         # e.g. ([]|units.m).append([1,2,3]|units.m) -> [[1,2,3]] | units.m
         # e.g. ([[1,2,3]]|units.m).append([4,5,6]|units.m) -> [[1,2,3],[4,5,6]] | units.m
-        if (append_number.shape and (len(self._number) == 0 or self._number.shape[1:] == append_number.shape)):
+        if append_number.shape and (
+            len(self._number) == 0 or self._number.shape[1:] == append_number.shape
+        ):
             new_shape = [1 + self._number.shape[0]] + list(append_number.shape)
         else:
             new_shape = -1
         self._number = numpy.append(self._number, append_number).reshape(new_shape)
 
     def extend(self, vector_quantity):
         """
@@ -727,29 +797,33 @@
         >>> from amuse.units import units
         >>> vector1 = [1.0, 2.0, 3.0] | units.kg
         >>> vector2 = [1500, 2500, 6000] | units.g
         >>> vector1.extend(vector2)
         >>> print vector1
         [1.0, 2.0, 3.0, 1.5, 2.5, 6.0] kg
         """
-        self._number = numpy.concatenate((self._number, vector_quantity.value_in(self.unit)))
+        self._number = numpy.concatenate(
+            (self._number, vector_quantity.value_in(self.unit))
+        )
 
     def prepend(self, scalar_quantity):
         """
         Prepend the scalar quantity before this vector.
         If the units differ, the scalar_quantity argument
         is converted to the units of this vector.
 
         >>> from amuse.units import units
         >>> vector1 = [1.0, 2.0, 3.0] | units.kg
         >>> vector1.prepend(0.0 | units.kg)
         >>> print vector1
         [0.0, 1.0, 2.0, 3.0] kg
         """
-        self._number = numpy.concatenate(([scalar_quantity.value_in(self.unit)], self._number))
+        self._number = numpy.concatenate(
+            ([scalar_quantity.value_in(self.unit)], self._number)
+        )
 
     def minimum(self, other):
         """
         Return the minimum of self and the argument.
 
         >>> from amuse.units import si
         >>> v1 = [1.0, 2.0, 3.0] | si.kg
@@ -774,62 +848,63 @@
         quantity<[1.0, 3.0, 4.0] kg>
         """
         other_in_my_units = other.as_quantity_in(self.unit)
         is_larger_than = self.number > other_in_my_units.number
         values = numpy.where(is_larger_than, self.number, other_in_my_units.number)
         return VectorQuantity(values, self.unit)
 
-    def max(self, axis = None):
+    def max(self, axis=None):
         """
         Return the maximum along an axis.
 
         >>> from amuse.units import si
         >>> v1 = [1.0, 2.0, 3.0] | si.kg
         >>> v1.amax()
         quantity<3.0 kg>
         """
 
-        return self.unit.new_quantity(numpy.amax(self.number, axis = axis))
+        return self.unit.new_quantity(numpy.amax(self.number, axis=axis))
 
-    def min(self, axis = None):
+    def min(self, axis=None):
         """
         Return the minimum value along an axis.
 
         >>> from amuse.units import si
         >>> v1 = [1.0, 2.0, 3.0] | si.kg
         >>> v1.amin()
         quantity<1.0 kg>
         """
 
-        return self.unit.new_quantity(numpy.amin(self.number, axis = axis))
-    amin=min
-    amax=max
+        return self.unit.new_quantity(numpy.amin(self.number, axis=axis))
 
-    def argmax(self, axis = None):
+    amin = min
+    amax = max
+
+    def argmax(self, axis=None):
         """
         Return the indices of the maximum values along an axis.
 
         >>> from amuse.units import si
         >>> v1 = [[1.0, 2.0, 3.0], [2.5, 2.5, 2.5]] | si.kg
         >>> v1.argmax(axis=0)
         array([1, 1, 0])
         """
-        return numpy.argmax(self.number, axis = axis)
+        return numpy.argmax(self.number, axis=axis)
 
-    def argmin(self, axis = None):
+    def argmin(self, axis=None):
         """
         Return the indices of the minimum values along an axis.
 
         >>> from amuse.units import si
         >>> v1 = [[1.0, 2.0, 3.0], [2.5, 2.5, 2.5]] | si.kg
         >>> v1.argmin(axis=0)
         array([0, 0, 1])
         """
 
-        return numpy.argmin(self.number, axis = axis)
+        return numpy.argmin(self.number, axis=axis)
 
     def sorted(self):
         """
         Return a new vector with all items sorted.
 
         >>> from amuse.units import si
         >>> v1 = [3.0, 1.0, 2.0] | si.kg
@@ -894,46 +969,53 @@
     def transpose(self, axes=None):
         return VectorQuantity(self.number.transpose(axes), self.unit)
 
     @property
     def T(self):
         return VectorQuantity(self.number.T, self.unit)
 
-    def mean(self, axis=None, dtype=None, out=None):
-        return new_quantity(self.number.mean(axis, dtype, out), self.unit)
+    def mean(self, *args, **kwargs):
+        return new_quantity(self.number.mean(*args, **kwargs), self.unit)
 
     def median(self, **kwargs):
         return new_quantity(numpy.median(self.number, **kwargs), self.unit)
 
     def std(self, axis=None, dtype=None, out=None, ddof=0):
         return new_quantity(self.number.std(axis, dtype, out, ddof), self.unit)
 
     def cross(self, other, axisa=-1, axisb=-1, axisc=-1, axis=None):
         """
         Return the cross product of this vector quantity with the supplied vector (quantity).
         """
         other = to_quantity(other)
         return new_quantity_nonone(
-            numpy.cross(self.number, other.number, axisa=axisa, axisb=axisb, axisc=axisc, axis=axis),
-            (self.unit * other.unit).to_simple_form()
+            numpy.cross(
+                self.number,
+                other.number,
+                axisa=axisa,
+                axisb=axisb,
+                axisc=axisc,
+                axis=axis,
+            ),
+            (self.unit * other.unit).to_simple_form(),
         )
 
     def dot(self, other, **kwargs):
         """
         Return the dot product of this vector quantity with the supplied vector (quantity).
 
         >>> from amuse.units import units
         >>> v1 = [1.0, 2.0, 3.0] | units.m
         >>> v1.dot(v1)
         quantity<14.0 m**2>
         """
         other = to_quantity(other)
         return new_quantity_nonone(
             numpy.dot(self.number, other.number, **kwargs),
-            (self.unit * other.unit).to_simple_form()
+            (self.unit * other.unit).to_simple_form(),
         )
 
     def __getstate__(self):
         return (self.unit, self.number)
 
     def __setstate__(self, x):
         self.unit = x[0]
@@ -949,21 +1031,20 @@
     >>> x = zero
     >>> x += 2.0 | si.kg
     >>> x
     quantity<2.0 kg>
 
     """
 
-
     def __init__(self):
         Quantity.__init__(self, zero_unit())
         self.base = ()
         self.factor = 1
         self.number = 0.0
-        self.dtype = 'float64'
+        self.dtype = "float64"
 
     def is_scalar(self):
         """
         True for scalar quantities.
         """
         return False
 
@@ -984,42 +1065,38 @@
 
     def __add__(self, other):
         return other
 
     def __sub__(self, other):
         return -other
 
-
     def __mul__(self, other):
         return self
 
-
     def __pow__(self, other):
         return self
 
     def __rmul__(self, other):
         return self
 
-
     def __truediv__(self, other):
         return self
 
     def __rtruediv__(self, other):
-        return other/self.number
+        return other / self.number
 
     def __div__(self, other):
         return self.__truediv__(other)
 
     def __rdiv__(self, other):
         return self.__rtruediv__(other)
 
     def in_base(self):
         return self
 
-
     def new_zeros_array(self, length):
         array = numpy.zeros(length, dtype=self.dtype)
         return new_quantity(array, zero_unit())
 
     def sqrt(self):
         return self
 
@@ -1038,41 +1115,41 @@
     def as_vector_with_length(self, length):
         return self.new_zeros_array(length)
 
     def __reduce__(self):
         return "zero"
 
     def __lt__(self, other):
-        other_as_q=to_quantity(other)
+        other_as_q = to_quantity(other)
         return 0 < other_as_q.value_in(other_as_q.unit)
 
     def __gt__(self, other):
-        other_as_q=to_quantity(other)
+        other_as_q = to_quantity(other)
         return 0 > other_as_q.value_in(other_as_q.unit)
 
     def __eq__(self, other):
-        other_as_q=to_quantity(other)
+        other_as_q = to_quantity(other)
         return 0 == other_as_q.value_in(other_as_q.unit)
 
     def __ne__(self, other):
-        other_as_q=to_quantity(other)
+        other_as_q = to_quantity(other)
         return 0 != other_as_q.value_in(other_as_q.unit)
 
     def __le__(self, other):
-        other_as_q=to_quantity(other)
+        other_as_q = to_quantity(other)
         return 0 <= other_as_q.value_in(other_as_q.unit)
 
     def __ge__(self, other):
-        other_as_q=to_quantity(other)
+        other_as_q = to_quantity(other)
         return 0 >= other_as_q.value_in(other_as_q.unit)
 
 
-
 zero = ZeroQuantity()
 
+
 class NonNumericQuantity(Quantity):
     """
     A Non Numeric Quantity object represents a quantity without
     a physical meaning.
 
     These Quantity objects cannot be used in
     numeric operations (like addition or multiplication). Also,
@@ -1094,34 +1171,39 @@
 
     """
 
     def __init__(self, value, unit):
         Quantity.__init__(self, unit)
         self.value = value
         if not unit.is_valid_value(value):
-            raise exceptions.AmuseException(f"<{value}> is not a valid value for {unit!r}")
+            raise exceptions.AmuseException(
+                f"<{value}> is not a valid value for {unit!r}"
+            )
 
     def as_quantity_in(self, another_unit):
         if not another_unit == self.unit:
-            raise exceptions.AmuseException("Cannot convert non-numeric quantities in to another unit")
+            raise exceptions.AmuseException(
+                "Cannot convert non-numeric quantities in to another unit"
+            )
 
         return new_quantity(self.value, another_unit)
 
     def value_in(self, unit):
         if not unit == self.unit:
-            raise exceptions.AmuseException("Cannot convert non-numeric quantities in to another unit")
+            raise exceptions.AmuseException(
+                "Cannot convert non-numeric quantities in to another unit"
+            )
 
         return self.value
 
     def __str__(self):
         return self.unit.value_to_string(self.value)
 
     def __repr__(self):
-        return f'quantity<{str(self.value)} - {str(self)}>'
-
+        return f"quantity<{str(self.value)} - {str(self)}>"
 
     def as_vector_with_length(self, length):
         return VectorQuantity(numpy.array([self.value] * length), self.unit)
 
     def as_vector_quantity(self):
         return VectorQuantity([self.value], self.unit)
 
@@ -1247,49 +1329,55 @@
 
 def is_unit(x):
     return hasattr(x, "base")
 
 
 def isNumber(x):
     try:
-        return 0 == x*0
+        return 0 == x * 0
     except:
         return False
 
 
 def as_vector_quantity(value):
-    if is_quantity(value): 
+    if is_quantity(value):
         return value
     else:
-        if isinstance(value, numpy.ndarray) and  numpy.issubdtype(value.dtype, numpy.number):
+        if isinstance(value, numpy.ndarray) and numpy.issubdtype(
+            value.dtype, numpy.number
+        ):
             return new_quantity(value, none)
-        if isinstance(value, __array_like): # its not a homogeneous numpy array, this can be slow
+        if isinstance(
+            value, __array_like
+        ):  # its not a homogeneous numpy array, this can be slow
             result = AdaptingVectorQuantity()
             for subvalue in value:
                 result.append(as_vector_quantity(subvalue))
             return result
         else:
             if isNumber(value):
                 return new_quantity(value, none)
             else:
-                raise Exception("Cannot convert '{0!r}' to a vector quantity".format(value))
+                raise Exception(
+                    "Cannot convert '{0!r}' to a vector quantity".format(value)
+                )
 
 
 def to_quantity(x):
     if is_quantity(x):
         return x
     else:
         return new_quantity(x, none)
 
 
-def as_quantity_in(x,unit):
+def as_quantity_in(x, unit):
     return to_quantity(x).as_quantity_in(unit)
 
 
-def value_in(x,unit):
+def value_in(x, unit):
     return to_quantity(x).value_in(unit)
 
 
 def concatenate(quantities):
     first = quantities[0]
     if not is_quantity(first):
         return numpy.concatenate(quantities)
@@ -1298,25 +1386,27 @@
     concatenated = numpy.concatenate(numbers)
     return VectorQuantity(concatenated, unit)
 
 
 def column_stack(args):
     args_ = [to_quantity(x) for x in args]
     units = set([x.unit for x in args_])
-    if len(units)==1:
-        return new_quantity(numpy.column_stack([x.number for x in args_]),args_[0].unit)
+    if len(units) == 1:
+        return new_quantity(
+            numpy.column_stack([x.number for x in args_]), args_[0].unit
+        )
     else:
         return numpy.column_stack(args)
 
 
 def stack(args):
     args_ = [to_quantity(x) for x in args]
     units = set([x.unit for x in args_])
     if len(units) == 1:
-        return new_quantity(numpy.stack([x.number for x in args_]),args_[0].unit)
+        return new_quantity(numpy.stack([x.number for x in args_]), args_[0].unit)
     else:
         return numpy.stack(args)
 
 
 def arange(start, stop, step):
     if not is_quantity(start):
         return numpy.arange(start, stop, step)
@@ -1325,22 +1415,22 @@
     start_value = start.value_in(unit)
     stop_value = stop.value_in(unit)
     step_value = step.value_in(unit)
     array = numpy.arange(start_value, stop_value, step_value)
     return new_quantity(array, unit)
 
 
-def linspace(start, stop, num = 50,  endpoint=True, retstep=False):
+def linspace(start, stop, num=50, endpoint=True, retstep=False):
     if not is_quantity(start):
-        return numpy.linspace(start, stop, num,  endpoint, retstep)
+        return numpy.linspace(start, stop, num, endpoint, retstep)
 
     unit = start.unit
     start_value = start.value_in(unit)
     stop_value = stop.value_in(unit)
-    array = numpy.linspace(start_value, stop_value, num,  endpoint, retstep)
+    array = numpy.linspace(start_value, stop_value, num, endpoint, retstep)
 
     if retstep:
         return new_quantity(array[0], unit), new_quantity(array[1], unit)
     else:
         return new_quantity(array, unit)
 
 
@@ -1366,26 +1456,26 @@
     return [matrix | unit for matrix, unit in zip(result, units)]
 
 
 def polyfit(x, y, deg):
     (x_number, y_number), (x_unit, y_unit) = separate_numbers_and_units([x, y])
 
     fit = numpy.polyfit(x_number, y_number, deg)
-    fit = [f | y_unit/(x_unit**(deg-i)) for i, f in enumerate(fit)]
+    fit = [f | y_unit / (x_unit ** (deg - i)) for i, f in enumerate(fit)]
 
     return fit
 
 
 def polyval(p, x):
     if len(p) == 1:
         return numpy.ones(x.shape) * p[0]
 
     p_number, p_unit = separate_numbers_and_units(p)
     y_unit = p_unit[-1].to_reduced_form()
-    x_unit = (y_unit/p_unit[-2]).to_reduced_form()
+    x_unit = (y_unit / p_unit[-2]).to_reduced_form()
 
     if x_unit != none:
         x = x.value_in(x_unit)
 
     value = numpy.polyval(p_number, x)
 
     return value | y_unit
@@ -1399,14 +1489,15 @@
 
 
 def sign(x):
     return numpy.sign(to_quantity(x).number)
 
 
 if HAS_ASTROPY:
+
     def to_astropy(quantity):
         "Convert a quantity from AMUSE to Astropy"
         # NOTE: we need to go through SI base here because AMUSE and Astropy
         # don't necessarily agree on derived unit definitions...
 
         # Find the SI bases of the unit
         unit = quantity.unit
@@ -1415,30 +1506,29 @@
         # Find the quantity's value in base units
         value = quantity.value_in(unit.base_unit())
 
         # Reconstruct the quantity in Astropy units
         ap_quantity = value
         for base_unit in unit_bases:
             if base_unit[1] == amuse.units.si.m:
-                ap_quantity = ap_quantity * astropy.units.m**base_unit[0]
+                ap_quantity = ap_quantity * astropy.units.m ** base_unit[0]
             elif base_unit[1] == amuse.units.si.kg:
-                ap_quantity = ap_quantity * astropy.units.kg**base_unit[0]
+                ap_quantity = ap_quantity * astropy.units.kg ** base_unit[0]
             elif base_unit[1] == amuse.units.si.s:
-                ap_quantity = ap_quantity * astropy.units.s**base_unit[0]
+                ap_quantity = ap_quantity * astropy.units.s ** base_unit[0]
             elif base_unit[1] == amuse.units.si.A:
-                ap_quantity = ap_quantity * astropy.units.A**base_unit[0]
+                ap_quantity = ap_quantity * astropy.units.A ** base_unit[0]
             elif base_unit[1] == amuse.units.si.K:
-                ap_quantity = ap_quantity * astropy.units.K**base_unit[0]
+                ap_quantity = ap_quantity * astropy.units.K ** base_unit[0]
             elif base_unit[1] == amuse.units.si.mol:
-                ap_quantity = ap_quantity * astropy.units.mol**base_unit[0]
+                ap_quantity = ap_quantity * astropy.units.mol ** base_unit[0]
             elif base_unit[1] == amuse.units.si.cd:
-                ap_quantity = ap_quantity * astropy.units.cd**base_unit[0]
+                ap_quantity = ap_quantity * astropy.units.cd ** base_unit[0]
         return ap_quantity
 
-
     def from_astropy(ap_quantity):
         "Convert a quantity from Astropy to AMUSE"
         # NOTE: we need to go through SI base here because AMUSE and Astropy
         # don't necessarily agree on derived unit definitions...
 
         # Find SI bases of the unit
         si_bases = ap_quantity.si.unit.bases
@@ -1448,36 +1538,28 @@
         # Find the quantity's value in base units
         si_value = ap_quantity.si.value
 
         # Reconstruct the quantity in AMUSE units
         amuse_quantity = si_value
         for base_unit in si_units:
             if base_unit[1].name == "m":
-                amuse_quantity = amuse_quantity * (
-                    1 | amuse.units.si.m**base_unit[0]
-                )
+                amuse_quantity = amuse_quantity * (1 | amuse.units.si.m ** base_unit[0])
             elif base_unit[1].name == "kg":
                 amuse_quantity = amuse_quantity * (
-                    1 | amuse.units.si.kg**base_unit[0]
+                    1 | amuse.units.si.kg ** base_unit[0]
                 )
             elif base_unit[1].name == "s":
-                amuse_quantity = amuse_quantity * (
-                    1 | amuse.units.si.s**base_unit[0]
-                )
+                amuse_quantity = amuse_quantity * (1 | amuse.units.si.s ** base_unit[0])
             elif base_unit[1].name == "A":
-                amuse_quantity = amuse_quantity * (
-                    1 | amuse.units.si.A**base_unit[0]
-                )
+                amuse_quantity = amuse_quantity * (1 | amuse.units.si.A ** base_unit[0])
             elif base_unit[1].name == "K":
-                amuse_quantity = amuse_quantity * (
-                    1 | amuse.units.si.K**base_unit[0]
-                )
+                amuse_quantity = amuse_quantity * (1 | amuse.units.si.K ** base_unit[0])
             elif base_unit[1].name == "mol":
                 amuse_quantity = amuse_quantity * (
-                    1 | amuse.units.si.mol**base_unit[0]
+                    1 | amuse.units.si.mol ** base_unit[0]
                 )
             elif base_unit[1].name == "cd":
                 amuse_quantity = amuse_quantity * (
-                    1 | amuse.units.si.cd**base_unit[0]
+                    1 | amuse.units.si.cd ** base_unit[0]
                 )
 
         return amuse_quantity
```

### Comparing `amuse-framework-2023.5.0/src/amuse/units/scaling_converter.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/scaling_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from amuse.units import generic_unit_system
 from amuse.units.quantities import new_quantity
 
-class ScalingConverter(object):
 
+class ScalingConverter(object):
     def __init__(
         self,
-        length = 1,
-        time = 1,
-        mass = 1,
-        current = 1,
-        temperature = 1,
-        amount = 1,
-        luminous_intensity = 1
+        length=1,
+        time=1,
+        mass=1,
+        current=1,
+        temperature=1,
+        amount=1,
+        luminous_intensity=1,
     ):
         self.factors = {}
-        
+
         self.factors[generic_unit_system.mass] = mass
         self.factors[generic_unit_system.length] = length
         self.factors[generic_unit_system.time] = time
         self.factors[generic_unit_system.temperature] = temperature
         self.factors[generic_unit_system.current] = current
         self.factors[generic_unit_system.luminous_intensity] = luminous_intensity
-        
+
     def reversed(self):
         return ScalingConverter(
-            length = 1 / self.factors[generic_unit_system.length],
-            time = 1 / self.factors[generic_unit_system.time],
-            mass =  1 / self.factors[generic_unit_system.mass],
-            current = 1 / self.factors[generic_unit_system.current],
-            temperature =  1 / self.factors[generic_unit_system.temperature],
-            amount = 1,
-            luminous_intensity = 1 / self.factors[generic_unit_system.luminous_intensity]
+            length=1 / self.factors[generic_unit_system.length],
+            time=1 / self.factors[generic_unit_system.time],
+            mass=1 / self.factors[generic_unit_system.mass],
+            current=1 / self.factors[generic_unit_system.current],
+            temperature=1 / self.factors[generic_unit_system.temperature],
+            amount=1,
+            luminous_intensity=1 / self.factors[generic_unit_system.luminous_intensity],
         )
-        
+
     def convert(self, quantity):
         unit = quantity.unit
         value = quantity.value_in(unit)
-        
+
         base = unit.base
         if not base:
             return quantity
-            
+
         new_unit = 1
         factor = unit.factor
-        
+
         for n, unit in base:
             if unit in self.factors:
                 factor_for_unit = self.factors[unit]
-                factor = factor * (factor_for_unit ** n)
-                new_unit *= (unit ** n)
+                factor = factor * (factor_for_unit**n)
+                new_unit *= unit**n
             else:
-                new_unit *= (unit ** n)
-        return new_quantity(value * factor, new_unit)
+                new_unit *= unit**n
+        return new_quantity(value * factor, new_unit)
```

### Comparing `amuse-framework-2023.5.0/src/amuse/units/si.py` & `amuse_framework-2024.4.0rc1/src/amuse/units/si.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,101 @@
 from amuse.units import core
 
-system = core.system('S.I.')
+system = core.system("S.I.")
 
-m = core.base_unit('length', 'meter', 'm', system)
-kg = core.base_unit('mass', 'kilogram', 'kg', system)
-s = core.base_unit('time', 'second', 's', system)
-A = core.base_unit('electric current', 'ampere', 'A', system)
-K = core.base_unit('thermodynamic temperature', 'kelvin', 'K', system)
-mol = core.base_unit('amount of substance', 'mole', 'mol', system)
-cd = core.base_unit('luminous intensity', 'candela', 'cd', system)
+m = core.base_unit("length", "meter", "m", system)
+kg = core.base_unit("mass", "kilogram", "kg", system)
+s = core.base_unit("time", "second", "s", system)
+A = core.base_unit("electric current", "ampere", "A", system)
+K = core.base_unit("thermodynamic temperature", "kelvin", "K", system)
+mol = core.base_unit("amount of substance", "mole", "mol", system)
+cd = core.base_unit("luminous intensity", "candela", "cd", system)
 
 no_system = core.no_system
-none = core.none_unit('none', 'none')
+none = core.none_unit("none", "none")
 no_unit = none
 
 named = core.named_unit
 
+
 # SI prefixes
 def deca(unit):
-    return named('deca' + unit.name, 'da' + unit.symbol, 10. * unit)
+    return named("deca" + unit.name, "da" + unit.symbol, 10.0 * unit)
+
+
 def hecto(unit):
-    return named('hecto' + unit.name, 'h' + unit.symbol, 100. * unit)
+    return named("hecto" + unit.name, "h" + unit.symbol, 100.0 * unit)
+
+
 def kilo(unit):
-    return named('kilo' + unit.name, 'k' + unit.symbol, 1000. * unit)
+    return named("kilo" + unit.name, "k" + unit.symbol, 1000.0 * unit)
+
+
 def mega(unit):
-    return named('mega' + unit.name, 'M' + unit.symbol, 1.e6 * unit)
+    return named("mega" + unit.name, "M" + unit.symbol, 1.0e6 * unit)
+
+
 def giga(unit):
-    return named('giga' + unit.name, 'G' + unit.symbol, 1.e9 * unit)
+    return named("giga" + unit.name, "G" + unit.symbol, 1.0e9 * unit)
+
+
 def tera(unit):
-    return named('tera' + unit.name, 'T' + unit.symbol, 1.e12 * unit)
+    return named("tera" + unit.name, "T" + unit.symbol, 1.0e12 * unit)
+
+
 def peta(unit):
-    return named('peta' + unit.name, 'P' + unit.symbol, 1.e15 * unit)
+    return named("peta" + unit.name, "P" + unit.symbol, 1.0e15 * unit)
+
+
 def exa(unit):
-    return named('exa' + unit.name, 'E' + unit.symbol, 1.e18 * unit)
+    return named("exa" + unit.name, "E" + unit.symbol, 1.0e18 * unit)
+
+
 def zetta(unit):
-    return named('zetta' + unit.name, 'Z' + unit.symbol, 1.e21 * unit)
+    return named("zetta" + unit.name, "Z" + unit.symbol, 1.0e21 * unit)
+
+
 def yotta(unit):
-    return named('yotta' + unit.name, 'Y' + unit.symbol, 1.e24 * unit)
+    return named("yotta" + unit.name, "Y" + unit.symbol, 1.0e24 * unit)
+
+
 def deci(unit):
-    return named('deci' + unit.name, 'd' + unit.symbol, 0.1 * unit)
+    return named("deci" + unit.name, "d" + unit.symbol, 0.1 * unit)
+
+
 def centi(unit):
-    return named('centi' + unit.name, 'c' + unit.symbol, 0.01 * unit)
+    return named("centi" + unit.name, "c" + unit.symbol, 0.01 * unit)
+
+
 def milli(unit):
-    return named('milli' + unit.name, 'm' + unit.symbol, 0.001 * unit)
+    return named("milli" + unit.name, "m" + unit.symbol, 0.001 * unit)
+
+
 def micro(unit):
-    return named('micro' + unit.name, 'mu' + unit.symbol, 1.e-6 * unit)
+    return named("micro" + unit.name, "mu" + unit.symbol, 1.0e-6 * unit)
+
+
 def nano(unit):
-    return named('nano' + unit.name, 'n' + unit.symbol, 1.e-9 * unit)
+    return named("nano" + unit.name, "n" + unit.symbol, 1.0e-9 * unit)
+
+
 def pico(unit):
-    return named('pico' + unit.name, 'p' + unit.symbol, 1.e-12 * unit)
+    return named("pico" + unit.name, "p" + unit.symbol, 1.0e-12 * unit)
+
+
 def femto(unit):
-    return named('femto' + unit.name, 'f' + unit.symbol, 1.e-15 * unit)
+    return named("femto" + unit.name, "f" + unit.symbol, 1.0e-15 * unit)
+
+
 def atto(unit):
-    return named('atto' + unit.name, 'a' + unit.symbol, 1.e-18 * unit)
+    return named("atto" + unit.name, "a" + unit.symbol, 1.0e-18 * unit)
+
+
 def zepto(unit):
-    return named('zepto' + unit.name, 'z' + unit.symbol, 1.e-21 * unit)
+    return named("zepto" + unit.name, "z" + unit.symbol, 1.0e-21 * unit)
+
+
 def yocto(unit):
-    return named('yocto' + unit.name, 'y' + unit.symbol, 1.e-24 * unit)
+    return named("yocto" + unit.name, "y" + unit.symbol, 1.0e-24 * unit)
 
 
 k = kilo
```

### Comparing `amuse-framework-2023.5.0/src/amuse_framework.egg-info/SOURCES.txt` & `amuse_framework-2024.4.0rc1/src/amuse_framework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 config.guess
 config.mk.in
 config.sub
 configure
 install-sh
 pyproject.toml
 setup.py
+./config.mk
 bin/amuse-tutorial
+bin/amusifier
 bin/amusifier.in
 lib/amuse_mpi/Makefile
 lib/amuse_mpi/amuse_mpi.c
 lib/amuse_mpi/amuse_mpi.h
 lib/forsockets/Makefile
 lib/forsockets/forsockets.c
 lib/forsockets/forsockets.h
@@ -43,19 +45,19 @@
 lib/stopcond/stopcond.c
 lib/stopcond/stopcond.h
 lib/stopcond/stopcond.inc
 lib/stopcond/stopcondf.F90
 lib/stopcond/stopcondf_isoc.F90
 lib/stopcond/mpi/Makefile
 src/amuse/__init__.py
+src/amuse/_version.py
 src/amuse/amuserc
 src/amuse/codes.py
 src/amuse/config.py
 src/amuse/lab.py
-src/amuse/version.py
 src/amuse/community/__init__.py
 src/amuse/community/interface/__init__.py
 src/amuse/community/interface/common.py
 src/amuse/community/interface/example.py
 src/amuse/community/interface/gd.py
 src/amuse/community/interface/hydro.py
 src/amuse/community/interface/mhd.py
@@ -232,14 +234,15 @@
 src/amuse/units/nist.py
 src/amuse/units/nist.txt
 src/amuse/units/nist2010.txt
 src/amuse/units/optparse.py
 src/amuse/units/quantities.py
 src/amuse/units/scaling_converter.py
 src/amuse/units/si.py
+src/amuse/units/stellar_types.py
 src/amuse/units/translator.txt
 src/amuse/units/trigo.py
 src/amuse/units/units.py
 src/amuse_framework.egg-info/PKG-INFO
 src/amuse_framework.egg-info/SOURCES.txt
 src/amuse_framework.egg-info/dependency_links.txt
 src/amuse_framework.egg-info/requires.txt
```

### Comparing `amuse-framework-2023.5.0/support/__init__.py` & `amuse_framework-2024.4.0rc1/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/support/classifiers.py` & `amuse_framework-2024.4.0rc1/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/support/config.py` & `amuse_framework-2024.4.0rc1/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/support/generate_main.py` & `amuse_framework-2024.4.0rc1/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/support/getsp.class` & `amuse_framework-2024.4.0rc1/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/support/getsp.java` & `amuse_framework-2024.4.0rc1/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/support/misc.py` & `amuse_framework-2024.4.0rc1/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-framework-2023.5.0/support/setup_codes.py` & `amuse_framework-2024.4.0rc1/support/setup_codes.py`

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

