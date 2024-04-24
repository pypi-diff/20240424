# Comparing `tmp/amuse-secularmultiple-2023.5.0.tar.gz` & `tmp/amuse-secularmultiple-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-secularmultiple-2023.5.0.tar", last modified: Wed May 17 10:19:34 2023, max compression
+gzip compressed data, was "amuse-secularmultiple-2024.4.0.tar", last modified: Wed Apr 24 16:32:48 2024, max compression
```

## Comparing `amuse-secularmultiple-2023.5.0.tar` & `amuse-secularmultiple-2024.4.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.858979 amuse-secularmultiple-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-secularmultiple-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1213 2023-05-17 10:19:34.858823 amuse-secularmultiple-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       68 2022-11-22 11:55:14.000000 amuse-secularmultiple-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.845065 amuse-secularmultiple-2023.5.0/amuse_secularmultiple.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1213 2023-05-17 10:19:33.000000 amuse-secularmultiple-2023.5.0/amuse_secularmultiple.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     3025 2023-05-17 10:19:34.000000 amuse-secularmultiple-2023.5.0/amuse_secularmultiple.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:33.000000 amuse-secularmultiple-2023.5.0/amuse_secularmultiple.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:33.000000 amuse-secularmultiple-2023.5.0/amuse_secularmultiple.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:33.000000 amuse-secularmultiple-2023.5.0/amuse_secularmultiple.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-secularmultiple-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:34.859022 amuse-secularmultiple-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1840 2022-11-22 11:55:14.000000 amuse-secularmultiple-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.843618 amuse-secularmultiple-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.843669 amuse-secularmultiple-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.843720 amuse-secularmultiple-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.846988 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/
--rw-r--r--   0 rieder     (501) staff       (20)     1110 2023-03-14 13:48:49.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       39 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    56053 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/interface.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    15575 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/interface.h
--rw-r--r--   0 rieder     (501) staff       (20)    84722 2023-03-14 13:48:49.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)     2893 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/readme.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.850716 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/
--rw-r--r--   0 rieder     (501) staff       (20)    12028 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/ODE_system.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      529 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/ODE_system.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.857171 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/
--rwxr-xr-x   0 rieder     (501) staff       (20)   116925 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode.c
--rwxr-xr-x   0 rieder     (501) staff       (20)    34616 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode.h
--rwxr-xr-x   0 rieder     (501) staff       (20)    10120 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_dense.c
--rwxr-xr-x   0 rieder     (501) staff       (20)     1741 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_dense.h
--rwxr-xr-x   0 rieder     (501) staff       (20)    12822 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct.c
--rwxr-xr-x   0 rieder     (501) staff       (20)    11044 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct.h
--rwxr-xr-x   0 rieder     (501) staff       (20)     4009 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct_impl.h
--rwxr-xr-x   0 rieder     (501) staff       (20)    24337 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_impl.h
--rwxr-xr-x   0 rieder     (501) staff       (20)    22926 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_io.c
--rwxr-xr-x   0 rieder     (501) staff       (20)    20761 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/nvector_serial.c
--rwxr-xr-x   0 rieder     (501) staff       (20)    10045 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/nvector_serial.h
--rwxr-xr-x   0 rieder     (501) staff       (20)     2779 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_config.h
--rwxr-xr-x   0 rieder     (501) staff       (20)     8335 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_dense.c
--rwxr-xr-x   0 rieder     (501) staff       (20)     7746 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_dense.h
--rwxr-xr-x   0 rieder     (501) staff       (20)     5779 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_direct.c
--rwxr-xr-x   0 rieder     (501) staff       (20)    12547 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_direct.h
--rwxr-xr-x   0 rieder     (501) staff       (20)     2465 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_math.c
--rwxr-xr-x   0 rieder     (501) staff       (20)     4285 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_math.h
--rwxr-xr-x   0 rieder     (501) staff       (20)     4693 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_nvector.c
--rwxr-xr-x   0 rieder     (501) staff       (20)    15955 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_nvector.h
--rwxr-xr-x   0 rieder     (501) staff       (20)     3717 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_types.h
--rw-r--r--   0 rieder     (501) staff       (20)     7068 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/evolve.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      885 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/evolve.h
--rw-r--r--   0 rieder     (501) staff       (20)    43884 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/external.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     1944 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/external.h
--rw-r--r--   0 rieder     (501) staff       (20)    37765 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/newtonian.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      497 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/newtonian.h
--rw-r--r--   0 rieder     (501) staff       (20)     2084 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/postnewtonian.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      241 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/postnewtonian.h
--rw-r--r--   0 rieder     (501) staff       (20)    19982 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/root_finding.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      497 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/root_finding.h
--rw-r--r--   0 rieder     (501) staff       (20)     6767 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/structure.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      212 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/structure.h
--rw-r--r--   0 rieder     (501) staff       (20)    22971 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/tides.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2619 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/tides.h
--rw-r--r--   0 rieder     (501) staff       (20)     2286 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/types.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    25374 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/types.h
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:33.000000 amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:34.858609 amuse-secularmultiple-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-secularmultiple-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-secularmultiple-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-secularmultiple-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.637368 amuse-secularmultiple-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-secularmultiple-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1244 2024-04-24 16:32:48.637157 amuse-secularmultiple-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       68 2022-11-22 11:55:14.000000 amuse-secularmultiple-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.636870 amuse-secularmultiple-2024.4.0/amuse_secularmultiple.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1244 2024-04-24 16:32:47.000000 amuse-secularmultiple-2024.4.0/amuse_secularmultiple.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     3026 2024-04-24 16:32:48.000000 amuse-secularmultiple-2024.4.0/amuse_secularmultiple.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:47.000000 amuse-secularmultiple-2024.4.0/amuse_secularmultiple.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:47.000000 amuse-secularmultiple-2024.4.0/amuse_secularmultiple.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:47.000000 amuse-secularmultiple-2024.4.0/amuse_secularmultiple.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-secularmultiple-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:48.637422 amuse-secularmultiple-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1635 2024-04-24 15:35:29.000000 amuse-secularmultiple-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.624714 amuse-secularmultiple-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.624767 amuse-secularmultiple-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.624819 amuse-secularmultiple-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.627589 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/
+-rw-r--r--   0 rieder     (501) staff       (20)     1110 2023-03-14 13:48:49.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       39 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:47.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)    56053 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/interface.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    15575 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/interface.h
+-rw-r--r--   0 rieder     (501) staff       (20)    84722 2023-03-14 13:48:49.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2893 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/readme.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.631040 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/
+-rw-r--r--   0 rieder     (501) staff       (20)    12028 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/ODE_system.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      529 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/ODE_system.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.635380 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/
+-rwxr-xr-x   0 rieder     (501) staff       (20)   116925 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)    34616 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)    10120 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_dense.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1741 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_dense.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)    12822 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)    11044 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)     4009 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct_impl.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)    24337 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_impl.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)    22926 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_io.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)    20761 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/nvector_serial.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)    10045 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/nvector_serial.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2779 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_config.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)     8335 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_dense.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)     7746 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_dense.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)     5779 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_direct.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)    12547 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_direct.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2465 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_math.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)     4285 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_math.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)     4693 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_nvector.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)    15955 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_nvector.h
+-rwxr-xr-x   0 rieder     (501) staff       (20)     3717 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_types.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7068 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/evolve.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      885 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/evolve.h
+-rw-r--r--   0 rieder     (501) staff       (20)    43884 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/external.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1944 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/external.h
+-rw-r--r--   0 rieder     (501) staff       (20)    37765 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/newtonian.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      497 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/newtonian.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2084 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/postnewtonian.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      241 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/postnewtonian.h
+-rw-r--r--   0 rieder     (501) staff       (20)    19982 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/root_finding.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      497 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/root_finding.h
+-rw-r--r--   0 rieder     (501) staff       (20)     6767 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/structure.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      212 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/structure.h
+-rw-r--r--   0 rieder     (501) staff       (20)    22971 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/tides.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2619 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/tides.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2286 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/types.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    25374 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/types.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:48.636683 amuse-secularmultiple-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-secularmultiple-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-secularmultiple-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-secularmultiple-2024.4.0/support/version.py
```

### Comparing `amuse-secularmultiple-2023.5.0/PKG-INFO` & `amuse-secularmultiple-2024.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-secularmultiple
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - SecularMultiple
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
 
 This package installs the SecularMultiple community code for AMUSE.
```

### Comparing `amuse-secularmultiple-2023.5.0/amuse_secularmultiple.egg-info/PKG-INFO` & `amuse-secularmultiple-2024.4.0/amuse_secularmultiple.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-secularmultiple
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - SecularMultiple
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
 
 This package installs the SecularMultiple community code for AMUSE.
```

### Comparing `amuse-secularmultiple-2023.5.0/amuse_secularmultiple.egg-info/SOURCES.txt` & `amuse-secularmultiple-2024.4.0/amuse_secularmultiple.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 amuse_secularmultiple.egg-info/PKG-INFO
 amuse_secularmultiple.egg-info/SOURCES.txt
 amuse_secularmultiple.egg-info/dependency_links.txt
 amuse_secularmultiple.egg-info/requires.txt
 amuse_secularmultiple.egg-info/top_level.txt
 src/amuse/community/secularmultiple/Makefile
 src/amuse/community/secularmultiple/__init__.py
+src/amuse/community/secularmultiple/_version.py
 src/amuse/community/secularmultiple/interface.cpp
 src/amuse/community/secularmultiple/interface.h
 src/amuse/community/secularmultiple/interface.py
 src/amuse/community/secularmultiple/readme.txt
-src/amuse/community/secularmultiple/version.py
 src/amuse/community/secularmultiple/src/ODE_system.cpp
 src/amuse/community/secularmultiple/src/ODE_system.h
 src/amuse/community/secularmultiple/src/evolve.cpp
 src/amuse/community/secularmultiple/src/evolve.h
 src/amuse/community/secularmultiple/src/external.cpp
 src/amuse/community/secularmultiple/src/external.h
 src/amuse/community/secularmultiple/src/newtonian.cpp
```

### Comparing `amuse-secularmultiple-2023.5.0/setup.py` & `amuse-secularmultiple-2024.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.secularmultiple.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/secularmultiple/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/secularmultiple/_version.py",
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
         'amuse.community.secularmultiple': 'src/amuse/community/secularmultiple',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/Makefile` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/interface.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/interface.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/interface.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/interface.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/interface.py` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/readme.txt` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/readme.txt`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/ODE_system.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/ODE_system.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/ODE_system.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/ODE_system.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_dense.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_dense.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_dense.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_dense.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct_impl.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_direct_impl.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_impl.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_impl.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/cvode_io.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/cvode_io.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/nvector_serial.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/nvector_serial.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_config.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_config.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_dense.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_dense.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_direct.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_direct.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_math.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_math.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_math.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_math.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_nvector.c` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_nvector.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/cvode/sundials_types.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/cvode/sundials_types.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/evolve.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/evolve.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/evolve.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/evolve.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/external.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/external.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/external.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/external.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/newtonian.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/newtonian.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/postnewtonian.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/postnewtonian.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/root_finding.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/root_finding.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/structure.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/structure.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/tides.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/tides.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/tides.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/tides.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/types.cpp` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/types.cpp`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/src/amuse/community/secularmultiple/src/types.h` & `amuse-secularmultiple-2024.4.0/src/amuse/community/secularmultiple/src/types.h`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/support/__init__.py` & `amuse-secularmultiple-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/support/classifiers.py` & `amuse-secularmultiple-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/support/config.py` & `amuse-secularmultiple-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/support/generate_main.py` & `amuse-secularmultiple-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/support/getsp.class` & `amuse-secularmultiple-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/support/getsp.java` & `amuse-secularmultiple-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/support/misc.py` & `amuse-secularmultiple-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-secularmultiple-2023.5.0/support/setup_codes.py` & `amuse-secularmultiple-2024.4.0/support/setup_codes.py`

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

