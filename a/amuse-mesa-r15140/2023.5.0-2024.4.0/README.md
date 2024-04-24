# Comparing `tmp/amuse-mesa-r15140-2023.5.0.tar.gz` & `tmp/amuse-mesa-r15140-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-mesa-r15140-2023.5.0.tar", last modified: Wed May 17 10:19:10 2023, max compression
+gzip compressed data, was "amuse-mesa-r15140-2024.4.0.tar", last modified: Wed Apr 24 16:32:32 2024, max compression
```

## Comparing `amuse-mesa-r15140-2023.5.0.tar` & `amuse-mesa-r15140-2024.4.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.482635 amuse-mesa-r15140-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2023-03-14 13:48:48.000000 amuse-mesa-r15140-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1205 2023-05-17 10:19:10.482445 amuse-mesa-r15140-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       66 2023-03-14 13:48:48.000000 amuse-mesa-r15140-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.473948 amuse-mesa-r15140-2023.5.0/amuse_mesa_r15140.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1205 2023-05-17 10:19:08.000000 amuse-mesa-r15140-2023.5.0/amuse_mesa_r15140.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     2767 2023-05-17 10:19:10.000000 amuse-mesa-r15140-2023.5.0/amuse_mesa_r15140.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:08.000000 amuse-mesa-r15140-2023.5.0/amuse_mesa_r15140.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:08.000000 amuse-mesa-r15140-2023.5.0/amuse_mesa_r15140.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:08.000000 amuse-mesa-r15140-2023.5.0/amuse_mesa_r15140.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-mesa-r15140-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:10.482699 amuse-mesa-r15140-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1814 2023-03-14 13:48:48.000000 amuse-mesa-r15140-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.472196 amuse-mesa-r15140-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.472250 amuse-mesa-r15140-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.472299 amuse-mesa-r15140-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.475352 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/
--rw-r--r--   0 rieder     (501) staff       (20)       23 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/.gitignore
--rw-r--r--   0 rieder     (501) staff       (20)     4302 2023-03-14 13:48:49.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/Makefile
--rwxr-xr-x   0 rieder     (501) staff       (20)     4221 2023-05-15 07:12:42.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/download.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.477737 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/
--rw-r--r--   0 rieder     (501) staff       (20)      285 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      552 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/basic.py
--rw-r--r--   0 rieder     (501) staff       (20)      584 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/basic2.py
--rw-r--r--   0 rieder     (501) staff       (20)     2531 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/controls.py
--rw-r--r--   0 rieder     (501) staff       (20)      347 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/gyre.in
--rw-r--r--   0 rieder     (501) staff       (20)      507 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/gyre.py
--rw-r--r--   0 rieder     (501) staff       (20)       50 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/inlist
--rw-r--r--   0 rieder     (501) staff       (20)      581 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/inlist.py
--rw-r--r--   0 rieder     (501) staff       (20)      829 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/multi.py
--rw-r--r--   0 rieder     (501) staff       (20)     1182 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/new_model.py
--rw-r--r--   0 rieder     (501) staff       (20)     1277 2023-05-16 07:06:02.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/photo_load.py
--rw-r--r--   0 rieder     (501) staff       (20)     2118 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/plot.py
--rw-r--r--   0 rieder     (501) staff       (20)      682 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/prems.py
--rw-r--r--   0 rieder     (501) staff       (20)      662 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/purehe.py
--rw-r--r--   0 rieder     (501) staff       (20)     1026 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/rotation.py
--rw-r--r--   0 rieder     (501) staff       (20)     1277 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/save_and_load.py
--rw-r--r--   0 rieder     (501) staff       (20)      824 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/sun.py
--rw-r--r--   0 rieder     (501) staff       (20)    40997 2023-05-16 07:06:02.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/interface.f90
--rw-r--r--   0 rieder     (501) staff       (20)    88033 2023-05-16 07:06:02.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)    38783 2023-05-16 07:06:02.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/mesa_interface.f90
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.477870 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/mesa_reqs/
--rw-r--r--   0 rieder     (501) staff       (20)       83 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/mesa_reqs/README
--rwxr-xr-x   0 rieder     (501) staff       (20)     3233 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patch_files.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.480282 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/
--rw-r--r--   0 rieder     (501) staff       (20)    24474 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Add-support-for-namelist-setting-from-a-string.patch
--rw-r--r--   0 rieder     (501) staff       (20)     1109 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Dont-make-empty-output-directories.patch
--rw-r--r--   0 rieder     (501) staff       (20)      730 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Fix-astero-builds-when-disabled.patch
--rw-r--r--   0 rieder     (501) staff       (20)      996 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Get-photo-loading-working.patch
--rw-r--r--   0 rieder     (501) staff       (20)     5220 2023-03-14 13:48:49.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Patch-error-messages.patch
--rw-r--r--   0 rieder     (501) staff       (20)     2550 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Stop-crashes-when-profile-column-name-is-bad.patch
--rw-r--r--   0 rieder     (501) staff       (20)      649 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-declare-i.patch
--rw-r--r--   0 rieder     (501) staff       (20)     1541 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0003-Add-mpi-to-utils.patch
--rw-r--r--   0 rieder     (501) staff       (20)      751 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0004-Fix-adipls-and-gyre-builds.patch
--rw-r--r--   0 rieder     (501) staff       (20)      824 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/fpx3_deps.patch
--rw-r--r--   0 rieder     (501) staff       (20)      744 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/lapack95.patch
--rw-r--r--   0 rieder     (501) staff       (20)    16108 2023-03-14 13:48:49.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/makefile_header_non_mesasdk
--rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/series_deps
--rw-r--r--   0 rieder     (501) staff       (20)      358 2023-03-14 13:48:49.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/series_mesa
--rw-r--r--   0 rieder     (501) staff       (20)     1296 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/run_star_extras.f90
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:08.000000 amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:10.482175 amuse-mesa-r15140-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-mesa-r15140-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-mesa-r15140-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.542150 amuse-mesa-r15140-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2023-03-14 13:48:48.000000 amuse-mesa-r15140-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1236 2024-04-24 16:32:32.541882 amuse-mesa-r15140-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       66 2023-03-14 13:48:48.000000 amuse-mesa-r15140-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.541582 amuse-mesa-r15140-2024.4.0/amuse_mesa_r15140.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1236 2024-04-24 16:32:31.000000 amuse-mesa-r15140-2024.4.0/amuse_mesa_r15140.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     2768 2024-04-24 16:32:32.000000 amuse-mesa-r15140-2024.4.0/amuse_mesa_r15140.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:31.000000 amuse-mesa-r15140-2024.4.0/amuse_mesa_r15140.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:31.000000 amuse-mesa-r15140-2024.4.0/amuse_mesa_r15140.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:31.000000 amuse-mesa-r15140-2024.4.0/amuse_mesa_r15140.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-mesa-r15140-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:32.542215 amuse-mesa-r15140-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1613 2024-04-24 15:35:29.000000 amuse-mesa-r15140-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.531230 amuse-mesa-r15140-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.531281 amuse-mesa-r15140-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.531331 amuse-mesa-r15140-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.534479 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/
+-rw-r--r--   0 rieder     (501) staff       (20)       23 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/.gitignore
+-rw-r--r--   0 rieder     (501) staff       (20)     4318 2024-04-24 15:35:29.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:31.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/_version.py
+-rwxr-xr-x   0 rieder     (501) staff       (20)     4224 2024-04-24 15:35:29.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/download.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.537232 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/
+-rw-r--r--   0 rieder     (501) staff       (20)      285 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      552 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/basic.py
+-rw-r--r--   0 rieder     (501) staff       (20)      584 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/basic2.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2531 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/controls.py
+-rw-r--r--   0 rieder     (501) staff       (20)      347 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/gyre.in
+-rw-r--r--   0 rieder     (501) staff       (20)      507 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/gyre.py
+-rw-r--r--   0 rieder     (501) staff       (20)       50 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/inlist
+-rw-r--r--   0 rieder     (501) staff       (20)      581 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/inlist.py
+-rw-r--r--   0 rieder     (501) staff       (20)      829 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/multi.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1182 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/new_model.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1277 2023-05-16 07:06:02.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/photo_load.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2118 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/plot.py
+-rw-r--r--   0 rieder     (501) staff       (20)      682 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/prems.py
+-rw-r--r--   0 rieder     (501) staff       (20)      662 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/purehe.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1026 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/rotation.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1277 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/save_and_load.py
+-rw-r--r--   0 rieder     (501) staff       (20)      824 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/sun.py
+-rw-r--r--   0 rieder     (501) staff       (20)    41108 2024-04-24 15:35:29.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/interface.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    88033 2023-05-16 07:06:02.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)    38783 2023-05-16 07:06:02.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/mesa_interface.f90
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.537398 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/mesa_reqs/
+-rw-r--r--   0 rieder     (501) staff       (20)       83 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/mesa_reqs/README
+-rwxr-xr-x   0 rieder     (501) staff       (20)     3233 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patch_files.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.540070 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/
+-rw-r--r--   0 rieder     (501) staff       (20)    24474 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Add-support-for-namelist-setting-from-a-string.patch
+-rw-r--r--   0 rieder     (501) staff       (20)     1109 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Dont-make-empty-output-directories.patch
+-rw-r--r--   0 rieder     (501) staff       (20)      730 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Fix-astero-builds-when-disabled.patch
+-rw-r--r--   0 rieder     (501) staff       (20)      996 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Get-photo-loading-working.patch
+-rw-r--r--   0 rieder     (501) staff       (20)     5220 2023-03-14 13:48:49.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Patch-error-messages.patch
+-rw-r--r--   0 rieder     (501) staff       (20)     2550 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Stop-crashes-when-profile-column-name-is-bad.patch
+-rw-r--r--   0 rieder     (501) staff       (20)      649 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-declare-i.patch
+-rw-r--r--   0 rieder     (501) staff       (20)     1541 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0003-Add-mpi-to-utils.patch
+-rw-r--r--   0 rieder     (501) staff       (20)      751 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0004-Fix-adipls-and-gyre-builds.patch
+-rw-r--r--   0 rieder     (501) staff       (20)      824 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/fpx3_deps.patch
+-rw-r--r--   0 rieder     (501) staff       (20)      744 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/lapack95.patch
+-rw-r--r--   0 rieder     (501) staff       (20)    16112 2024-04-24 15:35:29.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/makefile_header_non_mesasdk
+-rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/series_deps
+-rw-r--r--   0 rieder     (501) staff       (20)      358 2023-03-14 13:48:49.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/series_mesa
+-rw-r--r--   0 rieder     (501) staff       (20)     1296 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/run_star_extras.f90
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:32.541373 amuse-mesa-r15140-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-mesa-r15140-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-mesa-r15140-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-mesa-r15140-2024.4.0/support/version.py
```

### Comparing `amuse-mesa-r15140-2023.5.0/PKG-INFO` & `amuse-mesa-r15140-2024.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-mesa-r15140
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - MESA (r15140)
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,9 +21,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the MESA community code (r15140) for AMUSE.
```

### Comparing `amuse-mesa-r15140-2023.5.0/amuse_mesa_r15140.egg-info/PKG-INFO` & `amuse-mesa-r15140-2024.4.0/amuse_mesa_r15140.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-mesa-r15140
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - MESA (r15140)
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,9 +21,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the MESA community code (r15140) for AMUSE.
```

### Comparing `amuse-mesa-r15140-2023.5.0/amuse_mesa_r15140.egg-info/SOURCES.txt` & `amuse-mesa-r15140-2024.4.0/amuse_mesa_r15140.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 amuse_mesa_r15140.egg-info/PKG-INFO
 amuse_mesa_r15140.egg-info/SOURCES.txt
 amuse_mesa_r15140.egg-info/dependency_links.txt
 amuse_mesa_r15140.egg-info/requires.txt
 amuse_mesa_r15140.egg-info/top_level.txt
 src/amuse/community/mesa_r15140/.gitignore
 src/amuse/community/mesa_r15140/Makefile
+src/amuse/community/mesa_r15140/_version.py
 src/amuse/community/mesa_r15140/download.py
 src/amuse/community/mesa_r15140/interface.f90
 src/amuse/community/mesa_r15140/interface.py
 src/amuse/community/mesa_r15140/mesa_interface.f90
 src/amuse/community/mesa_r15140/patch_files.py
 src/amuse/community/mesa_r15140/run_star_extras.f90
-src/amuse/community/mesa_r15140/version.py
 src/amuse/community/mesa_r15140/examples/__init__.py
 src/amuse/community/mesa_r15140/examples/basic.py
 src/amuse/community/mesa_r15140/examples/basic2.py
 src/amuse/community/mesa_r15140/examples/controls.py
 src/amuse/community/mesa_r15140/examples/gyre.in
 src/amuse/community/mesa_r15140/examples/gyre.py
 src/amuse/community/mesa_r15140/examples/inlist
```

### Comparing `amuse-mesa-r15140-2023.5.0/setup.py` & `amuse-mesa-r15140-2024.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,32 +29,25 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.mesa_r15140.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/mesa_r15140/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/mesa_r15140/_version.py",
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

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/Makefile` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 -include ${AMUSE_DIR}/config.mk
 
 
 GFORTRAN_VERSION?=$(shell $(FC) -v 2>&1 | grep gcc\ version | cut -d\  -f3)
 GFORTRAN_MAJOR_MINOR=$(shell echo $(GFORTRAN_VERSION) | cut -s -d'.' -f1,2)
 #IFORT_VERSION?=$(shell $(FC) -v 2>&1 | cut -d\  -f2)
 #IFORT_MAJOR_MINOR=$(shell echo $(IFORT_VERSION) | cut -s -d'.' -f1,2)
+MPIFC ?= mpif90
 MPIF90 ?= mpif90
 MPICC ?= mpicc
 FORTRAN ?= gfortran
 PYTHON ?= python
 FC      ?= $(FORTRAN)
 export CC		?= gcc
 MPIFC+= $(FCFLAGS)
```

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/download.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     instance.filename_template='{version}.zip'
     instance.version = 'v1.2'
     instance.start()  
 
 
 def get_crlibm():
     instance = GetCodeFromHttp()
-    instance.url_template = 'http://www.astro.wisc.edu/~townsend/resource/download/sdk2/src/crlibm-{version}.tar.gz'
+    instance.url_template = 'http://user.astro.wisc.edu/~townsend/resource/download/sdk2/src/crlibm-{version}.tar.gz'
     instance.filename_template='crlibm-{version}.tar.gz'
     instance.version = '1.0beta4'
     instance.zip = False
     instance.start()  
 
 def get_fpx3deps():
     instance = GetCodeFromHttp()
@@ -90,23 +90,23 @@
     instance.version = ''
     instance.zip = False
     instance.unpack = False
     instance.start()  
 
 def get_fpx3():
     instance = GetCodeFromHttp()
-    instance.url_template = 'http://www.astro.wisc.edu/~townsend/resource/download/sdk2/src/fpx3.tar.gz'
+    instance.url_template = 'http://user.astro.wisc.edu/~townsend/resource/download/sdk2/src/fpx3.tar.gz'
     instance.filename_template='fpx3.tar.gz'
     instance.version = ''
     instance.zip = False
     instance.start()  
 
 def get_lapack95():
     instance = GetCodeFromHttp()
-    instance.url_template = 'http://www.astro.wisc.edu/~townsend/resource/download/sdk2/src/lapack95.tgz'
+    instance.url_template = 'http://user.astro.wisc.edu/~townsend/resource/download/sdk2/src/lapack95.tgz'
     instance.filename_template='lapack95.tgz'
     instance.version = ''
     instance.zip = False
     instance.start()      
 
 def get_mesa():
     instance = GetCodeFromHttp()
```

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/basic.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/basic.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/basic2.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/basic2.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/controls.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/controls.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/inlist.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/inlist.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/multi.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/multi.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/new_model.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/new_model.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/photo_load.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/photo_load.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/plot.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/plot.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/prems.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/prems.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/purehe.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/purehe.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/rotation.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/rotation.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/save_and_load.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/save_and_load.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/examples/sun.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/examples/sun.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/interface.f90` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/interface.f90`

 * *Files 0% similar despite different names*

```diff
@@ -580,15 +580,15 @@
 
 ! Return the current stellar type of the star
    integer function get_stellar_type(AMUSE_id, AMUSE_value)
       integer, intent(in) :: AMUSE_id
       integer, intent(out) :: AMUSE_value
       integer :: ierr
       double precision :: lgR, mass, ch1, che3, che4, cc12, cne20
-      double precision :: lgL, lgLH, ah1, ahe3, ahe4, lgLHe
+      double precision :: lgL, lgLH, ah1, ahe3, ahe4, lgLHe, logg
       AMUSE_value = -99
       get_stellar_type = -1
 
       call get_history_value(AMUSE_id, 'log_R', lgR, ierr)
       if(ierr/=MESA_SUCESS) return
       call get_history_value(AMUSE_id,'star_mass',mass, ierr)
       if(ierr/=MESA_SUCESS) return
@@ -614,17 +614,20 @@
       call get_history_value(AMUSE_id,'average h1',ah1, ierr)
       if(ierr/=MESA_SUCESS) return
       call get_history_value(AMUSE_id,'average he3',ahe3, ierr)
       if(ierr/=MESA_SUCESS) return
       call get_history_value(AMUSE_id,'average he4',ahe4, ierr)
       if(ierr/=MESA_SUCESS) return
 
+      call get_history_value(AMUSE_id,'photosphere_logg',logg, ierr)
+      if(ierr/=MESA_SUCESS) return
+
 
 
-      if (lgR > -1.0) then
+      if (logg < 6.0) then
          if(ch1 > 1d-4) then ! MS
             if(lgLH-lgL < -1 ) then ! Pre-main-sequence star
                AMUSE_value = 17
             else if(mass < 0.75) then
                AMUSE_value = 0 ! Convective low mass star
             else
                AMUSE_value = 1 ! Main sequence star
```

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/interface.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/mesa_interface.f90` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/mesa_interface.f90`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patch_files.py` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patch_files.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Add-support-for-namelist-setting-from-a-string.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Add-support-for-namelist-setting-from-a-string.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Dont-make-empty-output-directories.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Dont-make-empty-output-directories.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Fix-astero-builds-when-disabled.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Fix-astero-builds-when-disabled.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Get-photo-loading-working.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Get-photo-loading-working.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Patch-error-messages.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Patch-error-messages.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-Stop-crashes-when-profile-column-name-is-bad.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-Stop-crashes-when-profile-column-name-is-bad.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0001-declare-i.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0001-declare-i.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0003-Add-mpi-to-utils.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0003-Add-mpi-to-utils.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/0004-Fix-adipls-and-gyre-builds.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/0004-Fix-adipls-and-gyre-builds.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/fpx3_deps.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/fpx3_deps.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/lapack95.patch` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/lapack95.patch`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/patches/makefile_header_non_mesasdk` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/patches/makefile_header_non_mesasdk`

 * *Files 0% similar despite different names*

```diff
@@ -413,14 +413,14 @@
 .PHONY: all clean install install_lib install_mod
 
 # Path to cp_if_newer script
 CP_IF_NEWER = $(MESA_DIR)/utils/cp_if_newer
 
 # makedepf90 invocation (depends on whether we have the SDK2-patched version that
 # supports the -X flag)
-ifneq ($(shell makedepf90 -V | grep sdk2),)
+ifneq ($(shell src/makedepf90 -V | grep sdk2),)
     MAKEDEPF90_IGNORE_MODS = intrinsic omp_lib iso_c_binding iso_fortran_env ieee_arithmetic crmath hdf5
     MAKEDEPF90 := $(MESA_DIR)/utils/makedepf90-2.8.8/makedepf90 -m %m.mod -X $(addprefix -u,$(MAKEDEPF90_IGNORE_MODS))
 else
     MAKEDEPF90 := $(MESA_DIR)/utils/makedepf90-2.8.8/makedepf90 -m %m.mod
 endif
```

### Comparing `amuse-mesa-r15140-2023.5.0/src/amuse/community/mesa_r15140/run_star_extras.f90` & `amuse-mesa-r15140-2024.4.0/src/amuse/community/mesa_r15140/run_star_extras.f90`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/support/__init__.py` & `amuse-mesa-r15140-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/support/classifiers.py` & `amuse-mesa-r15140-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/support/config.py` & `amuse-mesa-r15140-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/support/generate_main.py` & `amuse-mesa-r15140-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/support/getsp.class` & `amuse-mesa-r15140-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/support/getsp.java` & `amuse-mesa-r15140-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/support/misc.py` & `amuse-mesa-r15140-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-mesa-r15140-2023.5.0/support/setup_codes.py` & `amuse-mesa-r15140-2024.4.0/support/setup_codes.py`

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

