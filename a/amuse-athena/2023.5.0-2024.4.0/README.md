# Comparing `tmp/amuse-athena-2023.5.0.tar.gz` & `tmp/amuse-athena-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-athena-2023.5.0.tar", last modified: Wed May 17 10:17:29 2023, max compression
+gzip compressed data, was "amuse-athena-2024.4.0.tar", last modified: Wed Apr 24 16:31:12 2024, max compression
```

## Comparing `amuse-athena-2023.5.0.tar` & `amuse-athena-2024.4.0.tar`

### file list

```diff
@@ -1,461 +1,461 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.859997 amuse-athena-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:17:29.859819 amuse-athena-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       59 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.770409 amuse-athena-2023.5.0/amuse_athena.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)    26055 2023-05-17 10:17:29.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/amuse_athena.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-athena-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:17:29.860043 amuse-athena-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1777 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.766105 amuse-athena-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.766156 amuse-athena-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.766209 amuse-athena-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.772483 amuse-athena-2023.5.0/src/amuse/community/athena/
--rw-r--r--   0 rieder     (501) staff       (20)     6368 2023-03-14 13:48:48.000000 amuse-athena-2023.5.0/src/amuse/community/athena/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     1456 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_3.1.c
--rw-r--r--   0 rieder     (501) staff       (20)     1438 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_4.0.c
--rw-r--r--   0 rieder     (501) staff       (20)     1438 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_4.1.c
--rwxr-xr-x   0 rieder     (501) staff       (20)     2212 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/download.py
--rw-r--r--   0 rieder     (501) staff       (20)    53617 2023-03-14 13:48:48.000000 amuse-athena-2023.5.0/src/amuse/community/athena/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)    21626 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/interface_3.1.c
--rw-r--r--   0 rieder     (501) staff       (20)    43174 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/interface_4.0.c
--rw-r--r--   0 rieder     (501) staff       (20)    94883 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/interface_4.1.c
--rw-r--r--   0 rieder     (501) staff       (20)      908 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/makefile.patch
--rwxr-xr-x   0 rieder     (501) staff       (20)     2859 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/patch_files.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.766335 amuse-athena-2023.5.0/src/amuse/community/athena/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.773715 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/
--rw-r--r--   0 rieder     (501) staff       (20)     2428 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)     2720 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/Makeoptions.in
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.774531 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/
--rw-r--r--   0 rieder     (501) staff       (20)   146872 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/output.0
--rw-r--r--   0 rieder     (501) staff       (20)     5106 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/requests
--rw-r--r--   0 rieder     (501) staff       (20)     7765 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/traces.0
--rwxr-xr-x   0 rieder     (501) staff       (20)   146471 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/configure
--rw-r--r--   0 rieder     (501) staff       (20)    21424 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/configure.ac
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.774714 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/doc/
--rw-r--r--   0 rieder     (501) staff       (20)      552 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/doc/pbs-script
--rwxr-xr-x   0 rieder     (501) staff       (20)     5598 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/install-sh
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.780698 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/
--rw-r--r--   0 rieder     (501) staff       (20)     4367 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)     4632 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_array.c
--rw-r--r--   0 rieder     (501) staff       (20)     4098 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_files.c
--rw-r--r--   0 rieder     (501) staff       (20)     9753 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_log.c
--rw-r--r--   0 rieder     (501) staff       (20)     2475 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_signal.c
--rw-r--r--   0 rieder     (501) staff       (20)    22054 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/athena.h
--rw-r--r--   0 rieder     (501) staff       (20)     3459 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/baton.c
--rw-r--r--   0 rieder     (501) staff       (20)    96563 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/bvals_mhd.c
--rw-r--r--   0 rieder     (501) staff       (20)    84875 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/bvals_shear.c
--rw-r--r--   0 rieder     (501) staff       (20)     5317 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/cc_pos.c
--rw-r--r--   0 rieder     (501) staff       (20)      433 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/config.h.in
--rw-r--r--   0 rieder     (501) staff       (20)    35952 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/convert_var.c
--rw-r--r--   0 rieder     (501) staff       (20)      876 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/copyright.h
--rw-r--r--   0 rieder     (501) staff       (20)     5237 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/defs.h.in
--rw-r--r--   0 rieder     (501) staff       (20)     8144 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_binary.c
--rw-r--r--   0 rieder     (501) staff       (20)    14784 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_history.c
--rw-r--r--   0 rieder     (501) staff       (20)    15062 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_tab.c
--rw-r--r--   0 rieder     (501) staff       (20)    10697 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_vtk.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.783120 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/
--rw-r--r--   0 rieder     (501) staff       (20)    17771 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/LICENSE
--rw-r--r--   0 rieder     (501) staff       (20)     1545 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    11355 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/ath_fft.c
--rw-r--r--   0 rieder     (501) staff       (20)     1662 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/factor.c
--rw-r--r--   0 rieder     (501) staff       (20)    11433 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.c
--rw-r--r--   0 rieder     (501) staff       (20)     2348 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.h
--rw-r--r--   0 rieder     (501) staff       (20)    15253 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     2572 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.h
--rw-r--r--   0 rieder     (501) staff       (20)    10480 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.c
--rw-r--r--   0 rieder     (501) staff       (20)     1203 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.h
--rw-r--r--   0 rieder     (501) staff       (20)    20644 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     1552 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.h
--rw-r--r--   0 rieder     (501) staff       (20)     3814 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    13200 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.c
--rw-r--r--   0 rieder     (501) staff       (20)     2598 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.h
--rw-r--r--   0 rieder     (501) staff       (20)    15313 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     2640 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.h
--rw-r--r--   0 rieder     (501) staff       (20)     3524 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/globals.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.784176 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/
--rw-r--r--   0 rieder     (501) staff       (20)     1287 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    40334 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/bvals_grav.c
--rw-r--r--   0 rieder     (501) staff       (20)     1539 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    20655 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg.c
--rw-r--r--   0 rieder     (501) staff       (20)    10585 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft.c
--rw-r--r--   0 rieder     (501) staff       (20)    17807 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft_obc.c
--rw-r--r--   0 rieder     (501) staff       (20)    35053 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_multigrid.c
--rw-r--r--   0 rieder     (501) staff       (20)    48007 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/init_grid.c
--rw-r--r--   0 rieder     (501) staff       (20)    37805 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/init_mesh.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.786162 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/
--rw-r--r--   0 rieder     (501) staff       (20)     1466 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)     3239 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate.c
--rw-r--r--   0 rieder     (501) staff       (20)    22956 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_ctu.c
--rw-r--r--   0 rieder     (501) staff       (20)    15882 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl.c
--rw-r--r--   0 rieder     (501) staff       (20)    22889 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)    73042 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_ctu.c
--rw-r--r--   0 rieder     (501) staff       (20)    48617 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl.c
--rw-r--r--   0 rieder     (501) staff       (20)    54176 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)   138756 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_ctu.c
--rw-r--r--   0 rieder     (501) staff       (20)    79851 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl.c
--rw-r--r--   0 rieder     (501) staff       (20)    84225 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)     1151 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    28050 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/main.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.787490 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/
--rw-r--r--   0 rieder     (501) staff       (20)     1355 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    13039 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/conduction.c
--rw-r--r--   0 rieder     (501) staff       (20)     2773 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/cool.c
--rw-r--r--   0 rieder     (501) staff       (20)     3252 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/diff_dt.c
--rw-r--r--   0 rieder     (501) staff       (20)     4491 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/get_eta.c
--rw-r--r--   0 rieder     (501) staff       (20)     3299 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/integrate_diffusion.c
--rw-r--r--   0 rieder     (501) staff       (20)     1606 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    45134 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/resistivity.c
--rw-r--r--   0 rieder     (501) staff       (20)    26948 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/viscosity.c
--rw-r--r--   0 rieder     (501) staff       (20)     5855 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/new_dt.c
--rw-r--r--   0 rieder     (501) staff       (20)    45790 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output.c
--rw-r--r--   0 rieder     (501) staff       (20)    11218 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_pdf.c
--rw-r--r--   0 rieder     (501) staff       (20)     4214 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_pgm.c
--rw-r--r--   0 rieder     (501) staff       (20)     5464 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_ppm.c
--rw-r--r--   0 rieder     (501) staff       (20)     8395 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_tab.c
--rw-r--r--   0 rieder     (501) staff       (20)     8403 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_vtk.c
--rw-r--r--   0 rieder     (501) staff       (20)    65505 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/palette.h
--rw-r--r--   0 rieder     (501) staff       (20)    31102 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/par.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.789009 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/
--rw-r--r--   0 rieder     (501) staff       (20)     1326 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    87780 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/bvals_particle.c
--rw-r--r--   0 rieder     (501) staff       (20)    13665 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/dump_particle_history.c
--rw-r--r--   0 rieder     (501) staff       (20)    41179 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/feedback.c
--rw-r--r--   0 rieder     (501) staff       (20)     9078 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/init_particle.c
--rw-r--r--   0 rieder     (501) staff       (20)    29582 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/integrators_particle.c
--rw-r--r--   0 rieder     (501) staff       (20)    11513 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/output_particle.c
--rw-r--r--   0 rieder     (501) staff       (20)     1491 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/particle.h
--rw-r--r--   0 rieder     (501) staff       (20)     3799 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    23052 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/utils_particle.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.822698 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/
--rw-r--r--   0 rieder     (501) staff       (20)     4565 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/README
--rw-r--r--   0 rieder     (501) staff       (20)     3503 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/blast.c
--rw-r--r--   0 rieder     (501) staff       (20)    15849 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/bubble.c
--rw-r--r--   0 rieder     (501) staff       (20)     6022 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/carbuncle.c
--rw-r--r--   0 rieder     (501) staff       (20)     7857 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/collapse3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     9095 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    12810 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    17446 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     8063 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cshock1d.c
--rw-r--r--   0 rieder     (501) staff       (20)     3295 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/current_sheet.c
--rw-r--r--   0 rieder     (501) staff       (20)     9456 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cyladvect.c
--rw-r--r--   0 rieder     (501) staff       (20)     6663 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylblast.c
--rw-r--r--   0 rieder     (501) staff       (20)     6283 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylbphi.c
--rw-r--r--   0 rieder     (501) staff       (20)     9325 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylbr.c
--rw-r--r--   0 rieder     (501) staff       (20)     7401 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylfieldloop.c
--rw-r--r--   0 rieder     (501) staff       (20)    25462 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylnewtmri.c
--rw-r--r--   0 rieder     (501) staff       (20)     5379 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylrayleigh.c
--rw-r--r--   0 rieder     (501) staff       (20)     6349 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylunif.c
--rw-r--r--   0 rieder     (501) staff       (20)     6362 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwind.c
--rw-r--r--   0 rieder     (501) staff       (20)     6841 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwindrot.c
--rw-r--r--   0 rieder     (501) staff       (20)     8182 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwindrotb.c
--rw-r--r--   0 rieder     (501) staff       (20)     7564 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/dmr.c
--rw-r--r--   0 rieder     (501) staff       (20)    13562 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/field_loop.c
--rw-r--r--   0 rieder     (501) staff       (20)    12054 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/firehose.c
--rw-r--r--   0 rieder     (501) staff       (20)     4867 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hall_drift.c
--rw-r--r--   0 rieder     (501) staff       (20)    16086 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hb3.c
--rw-r--r--   0 rieder     (501) staff       (20)    25056 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hgb.c
--rw-r--r--   0 rieder     (501) staff       (20)    12816 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hkdisk.c
--rw-r--r--   0 rieder     (501) staff       (20)     6137 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/jeans.c
--rw-r--r--   0 rieder     (501) staff       (20)     7058 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/jet.c
--rw-r--r--   0 rieder     (501) staff       (20)     8274 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/kh.c
--rw-r--r--   0 rieder     (501) staff       (20)    17209 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    18726 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    21769 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     3693 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/lw_implode.c
--rw-r--r--   0 rieder     (501) staff       (20)     7336 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/noh.c
--rw-r--r--   0 rieder     (501) staff       (20)     4220 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/orszag-tang.c
--rw-r--r--   0 rieder     (501) staff       (20)    14369 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_circ.c
--rw-r--r--   0 rieder     (501) staff       (20)    10895 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_collision.c
--rw-r--r--   0 rieder     (501) staff       (20)     9861 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_epicycle.c
--rw-r--r--   0 rieder     (501) staff       (20)     8447 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_friction.c
--rw-r--r--   0 rieder     (501) staff       (20)    12838 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    11854 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    14766 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_shwave1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    12434 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_shwave2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    27638 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_strat2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    27921 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_strat3d.c
--rw-r--r--   0 rieder     (501) staff       (20)    10544 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/pgflow.c
--rw-r--r--   0 rieder     (501) staff       (20)    12411 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/planet-disk.c
--rw-r--r--   0 rieder     (501) staff       (20)     4045 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/rotor.c
--rw-r--r--   0 rieder     (501) staff       (20)    20876 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/rt.c
--rw-r--r--   0 rieder     (501) staff       (20)     8808 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shk_cloud.c
--rw-r--r--   0 rieder     (501) staff       (20)     7338 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset1d.c
--rw-r--r--   0 rieder     (501) staff       (20)    14921 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset2d.c
--rw-r--r--   0 rieder     (501) staff       (20)    30745 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset3d.c
--rw-r--r--   0 rieder     (501) staff       (20)     3250 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shu-osher.c
--rw-r--r--   0 rieder     (501) staff       (20)    41891 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/strat.c
--rw-r--r--   0 rieder     (501) staff       (20)    19916 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_multi.c
--rw-r--r--   0 rieder     (501) staff       (20)    25339 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_single.c
--rw-r--r--   0 rieder     (501) staff       (20)    20516 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_multi.c
--rw-r--r--   0 rieder     (501) staff       (20)    25902 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_single.c
--rw-r--r--   0 rieder     (501) staff       (20)    20966 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/ti.c
--rw-r--r--   0 rieder     (501) staff       (20)    24287 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/turb.c
--rw-r--r--   0 rieder     (501) staff       (20)     4145 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/twoibw.c
--rw-r--r--   0 rieder     (501) staff       (20)    10180 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prototypes.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.823952 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/
--rw-r--r--   0 rieder     (501) staff       (20)     1343 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    18745 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/esystem_prim.c
--rw-r--r--   0 rieder     (501) staff       (20)     2581 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_dc.c
--rw-r--r--   0 rieder     (501) staff       (20)    12889 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_plm.c
--rw-r--r--   0 rieder     (501) staff       (20)    22476 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_ppm.c
--rw-r--r--   0 rieder     (501) staff       (20)    11888 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim2.c
--rw-r--r--   0 rieder     (501) staff       (20)    14242 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim3.c
--rw-r--r--   0 rieder     (501) staff       (20)     1755 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)    27483 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/restart.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.826355 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/
--rw-r--r--   0 rieder     (501) staff       (20)     1343 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/Makefile.in
--rw-r--r--   0 rieder     (501) staff       (20)    22384 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/esystem_roe.c
--rw-r--r--   0 rieder     (501) staff       (20)    20557 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/exact.c
--rw-r--r--   0 rieder     (501) staff       (20)    28427 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/exact_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)     8082 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/force.c
--rw-r--r--   0 rieder     (501) staff       (20)     6545 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc.c
--rw-r--r--   0 rieder     (501) staff       (20)    30910 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)    21397 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld.c
--rw-r--r--   0 rieder     (501) staff       (20)    33705 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)     7683 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle.c
--rw-r--r--   0 rieder     (501) staff       (20)    19191 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle_sr.c
--rw-r--r--   0 rieder     (501) staff       (20)     1706 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/prototypes.h
--rw-r--r--   0 rieder     (501) staff       (20)     9544 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/roe.c
--rw-r--r--   0 rieder     (501) staff       (20)     3816 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/two_shock.c
--rw-r--r--   0 rieder     (501) staff       (20)    10463 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/show_config.c
--rw-r--r--   0 rieder     (501) staff       (20)    85682 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/smr.c
--rw-r--r--   0 rieder     (501) staff       (20)    32081 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/utils.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.768186 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.829004 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     3986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1125
--rw-r--r--   0 rieder     (501) staff       (20)     3985 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1203
--rw-r--r--   0 rieder     (501) staff       (20)     3994 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.leveque
--rw-r--r--   0 rieder     (501) staff       (20)     3587 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d
--rw-r--r--   0 rieder     (501) staff       (20)     3621 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     3919 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.noh
--rw-r--r--   0 rieder     (501) staff       (20)     2206 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.pgflow
--rw-r--r--   0 rieder     (501) staff       (20)     3263 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.shu-osher
--rw-r--r--   0 rieder     (501) staff       (20)     3947 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.slow-moving-shock
--rw-r--r--   0 rieder     (501) staff       (20)     4004 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod
--rw-r--r--   0 rieder     (501) staff       (20)     3927 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-lw
--rw-r--r--   0 rieder     (501) staff       (20)     3989 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-toro
--rw-r--r--   0 rieder     (501) staff       (20)     4333 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.twoibw
--rwxr-xr-x   0 rieder     (501) staff       (20)     1116 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/run.linear_wave1d
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.831982 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     4222 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.brio-wu
--rw-r--r--   0 rieder     (501) staff       (20)     3728 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cpaw1d
--rw-r--r--   0 rieder     (501) staff       (20)     2195 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cshock1d
--rw-r--r--   0 rieder     (501) staff       (20)     3801 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d
--rw-r--r--   0 rieder     (501) staff       (20)     3604 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2627 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1a
--rw-r--r--   0 rieder     (501) staff       (20)     2636 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1b
--rw-r--r--   0 rieder     (501) staff       (20)     2650 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2a
--rw-r--r--   0 rieder     (501) staff       (20)     2636 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2b
--rw-r--r--   0 rieder     (501) staff       (20)     2640 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3a
--rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3b
--rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4a
--rw-r--r--   0 rieder     (501) staff       (20)     2606 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4b
--rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4c
--rw-r--r--   0 rieder     (501) staff       (20)     2604 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4d
--rw-r--r--   0 rieder     (501) staff       (20)     4106 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.torrilhon
--rwxr-xr-x   0 rieder     (501) staff       (20)      857 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.cpaw1d
--rwxr-xr-x   0 rieder     (501) staff       (20)     1177 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.linear_wave1d
--rwxr-xr-x   0 rieder     (501) staff       (20)      684 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.test
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.832581 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     2737 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb1
--rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb2
--rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb3
--rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb4
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.834906 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk1
--rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk2
--rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk3
--rw-r--r--   0 rieder     (501) staff       (20)     3005 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod1
--rw-r--r--   0 rieder     (501) staff       (20)     3006 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod2
--rw-r--r--   0 rieder     (501) staff       (20)     4231 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWoffFRF
--rw-r--r--   0 rieder     (501) staff       (20)     4229 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWonSRF
--rw-r--r--   0 rieder     (501) staff       (20)     4214 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SlowShock
--rw-r--r--   0 rieder     (501) staff       (20)     4230 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.brio-wu
--rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub1
--rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub2
--rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub3
--rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub4
--rw-r--r--   0 rieder     (501) staff       (20)     2996 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubcontact
--rw-r--r--   0 rieder     (501) staff       (20)     2999 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubrot
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.836683 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     3200 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     2218 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.carbuncle
--rw-r--r--   0 rieder     (501) staff       (20)     3713 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.dmr
--rw-r--r--   0 rieder     (501) staff       (20)     2220 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.jeans
--rw-r--r--   0 rieder     (501) staff       (20)     3968 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.kh
--rw-r--r--   0 rieder     (501) staff       (20)     3894 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d
--rw-r--r--   0 rieder     (501) staff       (20)     3901 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2824 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.lw_implode
--rw-r--r--   0 rieder     (501) staff       (20)     2582 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.noh
--rw-r--r--   0 rieder     (501) staff       (20)     2519 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.pgflow
--rw-r--r--   0 rieder     (501) staff       (20)     2446 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.rt
--rw-r--r--   0 rieder     (501) staff       (20)     3465 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.shk_cloud
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.838905 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     2742 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.Tconduct
--rw-r--r--   0 rieder     (501) staff       (20)     3498 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B1
--rw-r--r--   0 rieder     (501) staff       (20)     3403 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B10
--rw-r--r--   0 rieder     (501) staff       (20)     4435 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.cpaw2d
--rw-r--r--   0 rieder     (501) staff       (20)     4173 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.field_loop
--rw-r--r--   0 rieder     (501) staff       (20)     2003 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hall_drift
--rw-r--r--   0 rieder     (501) staff       (20)     3498 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hb3
--rw-r--r--   0 rieder     (501) staff       (20)     2848 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.kh
--rw-r--r--   0 rieder     (501) staff       (20)     5173 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d
--rw-r--r--   0 rieder     (501) staff       (20)     3931 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2598 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.orszag-tang
--rw-r--r--   0 rieder     (501) staff       (20)     2842 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rj2a
--rw-r--r--   0 rieder     (501) staff       (20)     2686 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rotor
--rw-r--r--   0 rieder     (501) staff       (20)     2737 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rt
--rwxr-xr-x   0 rieder     (501) staff       (20)      907 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.cpaw2d
--rwxr-xr-x   0 rieder     (501) staff       (20)     1230 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.linear_wave2d
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.839181 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     2052 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     2828 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.jet
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.839736 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     2183 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     3405 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.brio-wu
--rw-r--r--   0 rieder     (501) staff       (20)     2019 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.current-sheet
--rw-r--r--   0 rieder     (501) staff       (20)     2889 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.jet
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.841681 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)    16800 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-160-FPwave.dat
--rw-r--r--   0 rieder     (501) staff       (20)     4200 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-40-FPwave.dat
--rw-r--r--   0 rieder     (501) staff       (20)     3192 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     2217 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.carbuncle
--rw-r--r--   0 rieder     (501) staff       (20)     1904 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.fp-wave
--rw-r--r--   0 rieder     (501) staff       (20)     4064 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d
--rw-r--r--   0 rieder     (501) staff       (20)     4056 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2216 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.nl-shwave
--rw-r--r--   0 rieder     (501) staff       (20)     3078 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.noh
--rw-r--r--   0 rieder     (501) staff       (20)     2364 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.pgflow
--rw-r--r--   0 rieder     (501) staff       (20)     3540 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shk_cloud
--rw-r--r--   0 rieder     (501) staff       (20)     2816 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shwave
--rw-r--r--   0 rieder     (501) staff       (20)     2437 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.turb
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.844266 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     3148 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.Tconduct
--rw-r--r--   0 rieder     (501) staff       (20)     3314 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B1
--rw-r--r--   0 rieder     (501) staff       (20)     3414 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B10
--rw-r--r--   0 rieder     (501) staff       (20)     4527 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.cpaw3d
--rw-r--r--   0 rieder     (501) staff       (20)     4160 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop
--rw-r--r--   0 rieder     (501) staff       (20)     3591 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop4
--rw-r--r--   0 rieder     (501) staff       (20)     2960 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.hgb
--rw-r--r--   0 rieder     (501) staff       (20)     5410 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d
--rw-r--r--   0 rieder     (501) staff       (20)     3999 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d-3lev1
--rw-r--r--   0 rieder     (501) staff       (20)     2877 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rj2a_3d
--rw-r--r--   0 rieder     (501) staff       (20)     2200 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rt
--rw-r--r--   0 rieder     (501) staff       (20)     5397 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.strat
--rwxr-xr-x   0 rieder     (501) staff       (20)      964 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.cpaw3d
--rwxr-xr-x   0 rieder     (501) staff       (20)     1317 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.linear_wave3d
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.844407 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/
--rw-r--r--   0 rieder     (501) staff       (20)     2913 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/athinput.jet
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.844690 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/
--rw-r--r--   0 rieder     (501) staff       (20)     2232 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.blast
--rw-r--r--   0 rieder     (501) staff       (20)     2944 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.jet
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.851225 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/
--rw-r--r--   0 rieder     (501) staff       (20)     2952 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2754 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2603 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B0-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2690 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2859 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2820 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2860 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2186 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2304 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2422 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2386 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2504 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-3D
--rw-r--r--   0 rieder     (501) staff       (20)     3831 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2677 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-3D
--rw-r--r--   0 rieder     (501) staff       (20)     3249 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylnewtmri
--rw-r--r--   0 rieder     (501) staff       (20)     2390 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylrayleigh-2D
--rw-r--r--   0 rieder     (501) staff       (20)     1803 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylunif-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2112 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2245 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2395 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2235 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2404 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2486 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2142 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-1D
--rw-r--r--   0 rieder     (501) staff       (20)     2302 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-2D
--rw-r--r--   0 rieder     (501) staff       (20)     2396 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-3D
--rw-r--r--   0 rieder     (501) staff       (20)     2499 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.hkdisk-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      838 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cyladvect-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      717 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      690 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      819 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast.mpi-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      792 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylfieldloop-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      682 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylunif-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      723 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      748 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      731 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      771 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      751 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-3D
--rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-1D
--rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-2D
--rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-3D
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.853635 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/
--rw-r--r--   0 rieder     (501) staff       (20)     2762 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_circ
--rw-r--r--   0 rieder     (501) staff       (20)     3007 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_collision
--rw-r--r--   0 rieder     (501) staff       (20)     2663 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_epicycle
--rw-r--r--   0 rieder     (501) staff       (20)     2535 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_friction
--rw-r--r--   0 rieder     (501) staff       (20)     2894 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave1d
--rw-r--r--   0 rieder     (501) staff       (20)     3079 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave2d
--rw-r--r--   0 rieder     (501) staff       (20)     3184 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave1d
--rw-r--r--   0 rieder     (501) staff       (20)     3148 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave2d
--rw-r--r--   0 rieder     (501) staff       (20)     4321 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat2d
--rw-r--r--   0 rieder     (501) staff       (20)     4348 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat3d
--rw-r--r--   0 rieder     (501) staff       (20)     4057 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_multi
--rw-r--r--   0 rieder     (501) staff       (20)     5158 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_single
--rw-r--r--   0 rieder     (501) staff       (20)     4114 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_multi
--rw-r--r--   0 rieder     (501) staff       (20)     5373 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_single
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.768885 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.854202 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/
--rw-r--r--   0 rieder     (501) staff       (20)      748 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/noh.pro
--rw-r--r--   0 rieder     (501) staff       (20)     1874 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/plotdecay.pro
--rw-r--r--   0 rieder     (501) staff       (20)    13414 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/pltath.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.857278 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/
--rw-r--r--   0 rieder     (501) staff       (20)      334 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/animateppm.m
--rw-r--r--   0 rieder     (501) staff       (20)      508 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_construct_filename.m
--rw-r--r--   0 rieder     (501) staff       (20)     6756 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_getvar.m
--rw-r--r--   0 rieder     (501) staff       (20)      487 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_ijk_to_xyz.m
--rw-r--r--   0 rieder     (501) staff       (20)     5020 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_init_grid.m
--rw-r--r--   0 rieder     (501) staff       (20)     1851 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_ijk.m
--rw-r--r--   0 rieder     (501) staff       (20)     2081 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_xyz.m
--rw-r--r--   0 rieder     (501) staff       (20)     1354 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_palette.m
--rw-r--r--   0 rieder     (501) staff       (20)      723 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_parse_filename.m
--rw-r--r--   0 rieder     (501) staff       (20)      960 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_pcolor.m
--rw-r--r--   0 rieder     (501) staff       (20)      403 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_plotbdry.m
--rw-r--r--   0 rieder     (501) staff       (20)     4338 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_readbin.m
--rw-r--r--   0 rieder     (501) staff       (20)      326 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_sizeof.m
--rw-r--r--   0 rieder     (501) staff       (20)      642 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_ijk.m
--rw-r--r--   0 rieder     (501) staff       (20)     2011 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_xyz.m
--rw-r--r--   0 rieder     (501) staff       (20)     1169 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_text.m
--rw-r--r--   0 rieder     (501) staff       (20)     1196 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_xyz_to_ijk.m
--rw-r--r--   0 rieder     (501) staff       (20)       94 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/displayppm.m
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.857955 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/
--rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/Read_par_standard.m
--rw-r--r--   0 rieder     (501) staff       (20)     7217 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/join_lis.c
--rw-r--r--   0 rieder     (501) staff       (20)     1361 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/par_motion_movie.m
--rw-r--r--   0 rieder     (501) staff       (20)     7804 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/sort_lis.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.858121 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/sm/
--rw-r--r--   0 rieder     (501) staff       (20)     7015 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/sm/plot-smr-tab.sm
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.858285 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/vtk/
--rw-r--r--   0 rieder     (501) staff       (20)    19489 2022-11-22 11:55:14.000000 amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/vtk/join_vtk.c
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:17:28.000000 amuse-athena-2023.5.0/src/amuse/community/athena/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:17:29.859584 amuse-athena-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-athena-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-athena-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-athena-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.680333 amuse-athena-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1217 2024-04-24 16:31:12.680128 amuse-athena-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       59 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.679811 amuse-athena-2024.4.0/amuse_athena.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1217 2024-04-24 16:31:11.000000 amuse-athena-2024.4.0/amuse_athena.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)    26056 2024-04-24 16:31:12.000000 amuse-athena-2024.4.0/amuse_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:31:11.000000 amuse-athena-2024.4.0/amuse_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:31:11.000000 amuse-athena-2024.4.0/amuse_athena.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:31:11.000000 amuse-athena-2024.4.0/amuse_athena.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-athena-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:31:12.680388 amuse-athena-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1581 2024-04-24 15:35:29.000000 amuse-athena-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.611240 amuse-athena-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.611292 amuse-athena-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.611343 amuse-athena-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.617020 amuse-athena-2024.4.0/src/amuse/community/athena/
+-rw-r--r--   0 rieder     (501) staff       (20)     6368 2023-03-14 13:48:48.000000 amuse-athena-2024.4.0/src/amuse/community/athena/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:31:11.000000 amuse-athena-2024.4.0/src/amuse/community/athena/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1456 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/amuse_problem_3.1.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1438 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/amuse_problem_4.0.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1438 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/amuse_problem_4.1.c
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2212 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/download.py
+-rw-r--r--   0 rieder     (501) staff       (20)    53617 2023-03-14 13:48:48.000000 amuse-athena-2024.4.0/src/amuse/community/athena/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21626 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/interface_3.1.c
+-rw-r--r--   0 rieder     (501) staff       (20)    43174 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/interface_4.0.c
+-rw-r--r--   0 rieder     (501) staff       (20)    94883 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/interface_4.1.c
+-rw-r--r--   0 rieder     (501) staff       (20)      908 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/makefile.patch
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2859 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/patch_files.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.611463 amuse-athena-2024.4.0/src/amuse/community/athena/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.617857 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/
+-rw-r--r--   0 rieder     (501) staff       (20)     2428 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)     2720 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/Makeoptions.in
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.618461 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/autom4te.cache/
+-rw-r--r--   0 rieder     (501) staff       (20)   146872 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/autom4te.cache/output.0
+-rw-r--r--   0 rieder     (501) staff       (20)     5106 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/autom4te.cache/requests
+-rw-r--r--   0 rieder     (501) staff       (20)     7765 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/autom4te.cache/traces.0
+-rwxr-xr-x   0 rieder     (501) staff       (20)   146471 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/configure
+-rw-r--r--   0 rieder     (501) staff       (20)    21424 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/configure.ac
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.618616 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/doc/
+-rw-r--r--   0 rieder     (501) staff       (20)      552 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/doc/pbs-script
+-rwxr-xr-x   0 rieder     (501) staff       (20)     5598 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/install-sh
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.625090 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     4367 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)     4632 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/ath_array.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4098 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/ath_files.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9753 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/ath_log.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2475 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/ath_signal.c
+-rw-r--r--   0 rieder     (501) staff       (20)    22054 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/athena.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3459 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/baton.c
+-rw-r--r--   0 rieder     (501) staff       (20)    96563 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/bvals_mhd.c
+-rw-r--r--   0 rieder     (501) staff       (20)    84875 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/bvals_shear.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5317 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/cc_pos.c
+-rw-r--r--   0 rieder     (501) staff       (20)      433 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/config.h.in
+-rw-r--r--   0 rieder     (501) staff       (20)    35952 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/convert_var.c
+-rw-r--r--   0 rieder     (501) staff       (20)      876 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/copyright.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5237 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/defs.h.in
+-rw-r--r--   0 rieder     (501) staff       (20)     8144 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/dump_binary.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14784 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/dump_history.c
+-rw-r--r--   0 rieder     (501) staff       (20)    15062 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/dump_tab.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10697 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/dump_vtk.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.627626 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/
+-rw-r--r--   0 rieder     (501) staff       (20)    17771 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/LICENSE
+-rw-r--r--   0 rieder     (501) staff       (20)     1545 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    11355 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/ath_fft.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1662 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/factor.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11433 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2348 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.h
+-rw-r--r--   0 rieder     (501) staff       (20)    15253 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2572 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.h
+-rw-r--r--   0 rieder     (501) staff       (20)    10480 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1203 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.h
+-rw-r--r--   0 rieder     (501) staff       (20)    20644 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1552 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3814 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    13200 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2598 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.h
+-rw-r--r--   0 rieder     (501) staff       (20)    15313 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2640 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3524 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/globals.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.628667 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/
+-rw-r--r--   0 rieder     (501) staff       (20)     1287 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    40334 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/bvals_grav.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1539 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    20655 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10585 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft.c
+-rw-r--r--   0 rieder     (501) staff       (20)    17807 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft_obc.c
+-rw-r--r--   0 rieder     (501) staff       (20)    35053 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_multigrid.c
+-rw-r--r--   0 rieder     (501) staff       (20)    48007 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/init_grid.c
+-rw-r--r--   0 rieder     (501) staff       (20)    37805 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/init_mesh.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.631202 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/
+-rw-r--r--   0 rieder     (501) staff       (20)     1466 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)     3239 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate.c
+-rw-r--r--   0 rieder     (501) staff       (20)    22956 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_ctu.c
+-rw-r--r--   0 rieder     (501) staff       (20)    15882 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl.c
+-rw-r--r--   0 rieder     (501) staff       (20)    22889 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)    73042 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_ctu.c
+-rw-r--r--   0 rieder     (501) staff       (20)    48617 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl.c
+-rw-r--r--   0 rieder     (501) staff       (20)    54176 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)   138756 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_ctu.c
+-rw-r--r--   0 rieder     (501) staff       (20)    79851 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl.c
+-rw-r--r--   0 rieder     (501) staff       (20)    84225 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1151 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    28050 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/main.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.632589 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/
+-rw-r--r--   0 rieder     (501) staff       (20)     1355 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    13039 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/conduction.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2773 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/cool.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3252 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/diff_dt.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4491 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/get_eta.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3299 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/integrate_diffusion.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1606 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    45134 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/resistivity.c
+-rw-r--r--   0 rieder     (501) staff       (20)    26948 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/viscosity.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5855 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/new_dt.c
+-rw-r--r--   0 rieder     (501) staff       (20)    45790 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11218 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_pdf.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4214 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_pgm.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5464 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_ppm.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8395 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_tab.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8403 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_vtk.c
+-rw-r--r--   0 rieder     (501) staff       (20)    65505 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/palette.h
+-rw-r--r--   0 rieder     (501) staff       (20)    31102 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/par.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.634238 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/
+-rw-r--r--   0 rieder     (501) staff       (20)     1326 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    87780 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/bvals_particle.c
+-rw-r--r--   0 rieder     (501) staff       (20)    13665 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/dump_particle_history.c
+-rw-r--r--   0 rieder     (501) staff       (20)    41179 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/feedback.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9078 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/init_particle.c
+-rw-r--r--   0 rieder     (501) staff       (20)    29582 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/integrators_particle.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11513 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/output_particle.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1491 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/particle.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3799 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    23052 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/utils_particle.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.644915 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/
+-rw-r--r--   0 rieder     (501) staff       (20)     4565 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/README
+-rw-r--r--   0 rieder     (501) staff       (20)     3503 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/blast.c
+-rw-r--r--   0 rieder     (501) staff       (20)    15849 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/bubble.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6022 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/carbuncle.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7857 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/collapse3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9095 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12810 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    17446 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8063 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cshock1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3295 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/current_sheet.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9456 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cyladvect.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6663 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylblast.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6283 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylbphi.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9325 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylbr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7401 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylfieldloop.c
+-rw-r--r--   0 rieder     (501) staff       (20)    25462 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylnewtmri.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5379 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylrayleigh.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6349 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylunif.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6362 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylwind.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6841 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylwindrot.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8182 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylwindrotb.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7564 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/dmr.c
+-rw-r--r--   0 rieder     (501) staff       (20)    13562 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/field_loop.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12054 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/firehose.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4867 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/hall_drift.c
+-rw-r--r--   0 rieder     (501) staff       (20)    16086 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/hb3.c
+-rw-r--r--   0 rieder     (501) staff       (20)    25056 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/hgb.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12816 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/hkdisk.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6137 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/jeans.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7058 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/jet.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8274 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/kh.c
+-rw-r--r--   0 rieder     (501) staff       (20)    17209 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    18726 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    21769 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3693 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/lw_implode.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7336 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/noh.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4220 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/orszag-tang.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14369 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_circ.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10895 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_collision.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9861 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_epicycle.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8447 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_friction.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12838 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11854 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14766 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_shwave1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12434 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_shwave2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    27638 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_strat2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    27921 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_strat3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10544 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/pgflow.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12411 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/planet-disk.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4045 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/rotor.c
+-rw-r--r--   0 rieder     (501) staff       (20)    20876 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/rt.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8808 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shk_cloud.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7338 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shkset1d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14921 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shkset2d.c
+-rw-r--r--   0 rieder     (501) staff       (20)    30745 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shkset3d.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3250 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shu-osher.c
+-rw-r--r--   0 rieder     (501) staff       (20)    41891 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/strat.c
+-rw-r--r--   0 rieder     (501) staff       (20)    19916 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_multi.c
+-rw-r--r--   0 rieder     (501) staff       (20)    25339 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_single.c
+-rw-r--r--   0 rieder     (501) staff       (20)    20516 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_multi.c
+-rw-r--r--   0 rieder     (501) staff       (20)    25902 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_single.c
+-rw-r--r--   0 rieder     (501) staff       (20)    20966 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/ti.c
+-rw-r--r--   0 rieder     (501) staff       (20)    24287 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/turb.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4145 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/twoibw.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10180 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prototypes.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.646349 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/
+-rw-r--r--   0 rieder     (501) staff       (20)     1343 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    18745 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/esystem_prim.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2581 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_dc.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12889 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_plm.c
+-rw-r--r--   0 rieder     (501) staff       (20)    22476 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_ppm.c
+-rw-r--r--   0 rieder     (501) staff       (20)    11888 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim2.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14242 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim3.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1755 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)    27483 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/restart.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.648838 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/
+-rw-r--r--   0 rieder     (501) staff       (20)     1343 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/Makefile.in
+-rw-r--r--   0 rieder     (501) staff       (20)    22384 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/esystem_roe.c
+-rw-r--r--   0 rieder     (501) staff       (20)    20557 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/exact.c
+-rw-r--r--   0 rieder     (501) staff       (20)    28427 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/exact_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8082 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/force.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6545 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc.c
+-rw-r--r--   0 rieder     (501) staff       (20)    30910 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)    21397 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld.c
+-rw-r--r--   0 rieder     (501) staff       (20)    33705 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7683 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle.c
+-rw-r--r--   0 rieder     (501) staff       (20)    19191 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle_sr.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1706 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/prototypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)     9544 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/roe.c
+-rw-r--r--   0 rieder     (501) staff       (20)     3816 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/two_shock.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10463 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/show_config.c
+-rw-r--r--   0 rieder     (501) staff       (20)    85682 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/smr.c
+-rw-r--r--   0 rieder     (501) staff       (20)    32081 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/utils.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.613152 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.651098 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     3986 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1125
+-rw-r--r--   0 rieder     (501) staff       (20)     3985 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1203
+-rw-r--r--   0 rieder     (501) staff       (20)     3994 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.leveque
+-rw-r--r--   0 rieder     (501) staff       (20)     3587 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3621 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     3919 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.noh
+-rw-r--r--   0 rieder     (501) staff       (20)     2206 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.pgflow
+-rw-r--r--   0 rieder     (501) staff       (20)     3263 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.shu-osher
+-rw-r--r--   0 rieder     (501) staff       (20)     3947 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.slow-moving-shock
+-rw-r--r--   0 rieder     (501) staff       (20)     4004 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod
+-rw-r--r--   0 rieder     (501) staff       (20)     3927 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-lw
+-rw-r--r--   0 rieder     (501) staff       (20)     3989 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-toro
+-rw-r--r--   0 rieder     (501) staff       (20)     4333 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.twoibw
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1116 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/run.linear_wave1d
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.654095 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     4222 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.brio-wu
+-rw-r--r--   0 rieder     (501) staff       (20)     3728 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cpaw1d
+-rw-r--r--   0 rieder     (501) staff       (20)     2195 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cshock1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3801 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3604 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2627 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1a
+-rw-r--r--   0 rieder     (501) staff       (20)     2636 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1b
+-rw-r--r--   0 rieder     (501) staff       (20)     2650 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2a
+-rw-r--r--   0 rieder     (501) staff       (20)     2636 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2b
+-rw-r--r--   0 rieder     (501) staff       (20)     2640 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3a
+-rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3b
+-rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4a
+-rw-r--r--   0 rieder     (501) staff       (20)     2606 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4b
+-rw-r--r--   0 rieder     (501) staff       (20)     2608 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4c
+-rw-r--r--   0 rieder     (501) staff       (20)     2604 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4d
+-rw-r--r--   0 rieder     (501) staff       (20)     4106 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.torrilhon
+-rwxr-xr-x   0 rieder     (501) staff       (20)      857 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.cpaw1d
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1177 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.linear_wave1d
+-rwxr-xr-x   0 rieder     (501) staff       (20)      684 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.test
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.654641 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     2737 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb1
+-rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb2
+-rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb3
+-rw-r--r--   0 rieder     (501) staff       (20)     2684 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb4
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.656783 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk1
+-rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk2
+-rw-r--r--   0 rieder     (501) staff       (20)     4215 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk3
+-rw-r--r--   0 rieder     (501) staff       (20)     3005 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod1
+-rw-r--r--   0 rieder     (501) staff       (20)     3006 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod2
+-rw-r--r--   0 rieder     (501) staff       (20)     4231 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWoffFRF
+-rw-r--r--   0 rieder     (501) staff       (20)     4229 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWonSRF
+-rw-r--r--   0 rieder     (501) staff       (20)     4214 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SlowShock
+-rw-r--r--   0 rieder     (501) staff       (20)     4230 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.brio-wu
+-rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub1
+-rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub2
+-rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub3
+-rw-r--r--   0 rieder     (501) staff       (20)     2986 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub4
+-rw-r--r--   0 rieder     (501) staff       (20)     2996 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubcontact
+-rw-r--r--   0 rieder     (501) staff       (20)     2999 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubrot
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.658638 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     3200 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     2218 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.carbuncle
+-rw-r--r--   0 rieder     (501) staff       (20)     3713 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.dmr
+-rw-r--r--   0 rieder     (501) staff       (20)     2220 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.jeans
+-rw-r--r--   0 rieder     (501) staff       (20)     3968 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.kh
+-rw-r--r--   0 rieder     (501) staff       (20)     3894 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d
+-rw-r--r--   0 rieder     (501) staff       (20)     3901 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2824 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.lw_implode
+-rw-r--r--   0 rieder     (501) staff       (20)     2582 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.noh
+-rw-r--r--   0 rieder     (501) staff       (20)     2519 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.pgflow
+-rw-r--r--   0 rieder     (501) staff       (20)     2446 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.rt
+-rw-r--r--   0 rieder     (501) staff       (20)     3465 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.shk_cloud
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.660914 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     2742 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.Tconduct
+-rw-r--r--   0 rieder     (501) staff       (20)     3498 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B1
+-rw-r--r--   0 rieder     (501) staff       (20)     3403 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B10
+-rw-r--r--   0 rieder     (501) staff       (20)     4435 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.cpaw2d
+-rw-r--r--   0 rieder     (501) staff       (20)     4173 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.field_loop
+-rw-r--r--   0 rieder     (501) staff       (20)     2003 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hall_drift
+-rw-r--r--   0 rieder     (501) staff       (20)     3498 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hb3
+-rw-r--r--   0 rieder     (501) staff       (20)     2848 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.kh
+-rw-r--r--   0 rieder     (501) staff       (20)     5173 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d
+-rw-r--r--   0 rieder     (501) staff       (20)     3931 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2598 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.orszag-tang
+-rw-r--r--   0 rieder     (501) staff       (20)     2842 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rj2a
+-rw-r--r--   0 rieder     (501) staff       (20)     2686 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rotor
+-rw-r--r--   0 rieder     (501) staff       (20)     2737 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rt
+-rwxr-xr-x   0 rieder     (501) staff       (20)      907 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.cpaw2d
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1230 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.linear_wave2d
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.661200 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     2052 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     2828 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.jet
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.661751 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     2183 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     3405 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.brio-wu
+-rw-r--r--   0 rieder     (501) staff       (20)     2019 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.current-sheet
+-rw-r--r--   0 rieder     (501) staff       (20)     2889 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.jet
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.663557 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)    16800 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-160-FPwave.dat
+-rw-r--r--   0 rieder     (501) staff       (20)     4200 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-40-FPwave.dat
+-rw-r--r--   0 rieder     (501) staff       (20)     3192 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     2217 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.carbuncle
+-rw-r--r--   0 rieder     (501) staff       (20)     1904 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.fp-wave
+-rw-r--r--   0 rieder     (501) staff       (20)     4064 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d
+-rw-r--r--   0 rieder     (501) staff       (20)     4056 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2216 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.nl-shwave
+-rw-r--r--   0 rieder     (501) staff       (20)     3078 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.noh
+-rw-r--r--   0 rieder     (501) staff       (20)     2364 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.pgflow
+-rw-r--r--   0 rieder     (501) staff       (20)     3540 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shk_cloud
+-rw-r--r--   0 rieder     (501) staff       (20)     2816 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shwave
+-rw-r--r--   0 rieder     (501) staff       (20)     2437 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.turb
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.665527 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     3148 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.Tconduct
+-rw-r--r--   0 rieder     (501) staff       (20)     3314 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B1
+-rw-r--r--   0 rieder     (501) staff       (20)     3414 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B10
+-rw-r--r--   0 rieder     (501) staff       (20)     4527 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.cpaw3d
+-rw-r--r--   0 rieder     (501) staff       (20)     4160 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop
+-rw-r--r--   0 rieder     (501) staff       (20)     3591 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop4
+-rw-r--r--   0 rieder     (501) staff       (20)     2960 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.hgb
+-rw-r--r--   0 rieder     (501) staff       (20)     5410 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d
+-rw-r--r--   0 rieder     (501) staff       (20)     3999 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d-3lev1
+-rw-r--r--   0 rieder     (501) staff       (20)     2877 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rj2a_3d
+-rw-r--r--   0 rieder     (501) staff       (20)     2200 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rt
+-rw-r--r--   0 rieder     (501) staff       (20)     5397 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.strat
+-rwxr-xr-x   0 rieder     (501) staff       (20)      964 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.cpaw3d
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1317 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.linear_wave3d
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.665670 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/
+-rw-r--r--   0 rieder     (501) staff       (20)     2913 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/athinput.jet
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.665946 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/
+-rw-r--r--   0 rieder     (501) staff       (20)     2232 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.blast
+-rw-r--r--   0 rieder     (501) staff       (20)     2944 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.jet
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.672190 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/
+-rw-r--r--   0 rieder     (501) staff       (20)     2952 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2754 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2603 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B0-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2690 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2859 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2820 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2860 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2186 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2304 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2422 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2386 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2504 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     3831 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2677 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     3249 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylnewtmri
+-rw-r--r--   0 rieder     (501) staff       (20)     2390 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylrayleigh-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     1803 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylunif-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2112 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2245 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2395 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2235 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2404 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2486 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2142 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-1D
+-rw-r--r--   0 rieder     (501) staff       (20)     2302 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-2D
+-rw-r--r--   0 rieder     (501) staff       (20)     2396 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-3D
+-rw-r--r--   0 rieder     (501) staff       (20)     2499 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.hkdisk-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      838 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cyladvect-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      717 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      690 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      819 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast.mpi-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      792 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylfieldloop-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      682 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylunif-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      723 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      748 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      849 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      731 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      771 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      751 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-3D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-1D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-2D
+-rwxr-xr-x   0 rieder     (501) staff       (20)      852 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-3D
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.674167 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/
+-rw-r--r--   0 rieder     (501) staff       (20)     2762 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_circ
+-rw-r--r--   0 rieder     (501) staff       (20)     3007 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_collision
+-rw-r--r--   0 rieder     (501) staff       (20)     2663 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_epicycle
+-rw-r--r--   0 rieder     (501) staff       (20)     2535 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_friction
+-rw-r--r--   0 rieder     (501) staff       (20)     2894 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3079 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave2d
+-rw-r--r--   0 rieder     (501) staff       (20)     3184 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave1d
+-rw-r--r--   0 rieder     (501) staff       (20)     3148 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave2d
+-rw-r--r--   0 rieder     (501) staff       (20)     4321 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat2d
+-rw-r--r--   0 rieder     (501) staff       (20)     4348 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat3d
+-rw-r--r--   0 rieder     (501) staff       (20)     4057 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_multi
+-rw-r--r--   0 rieder     (501) staff       (20)     5158 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_single
+-rw-r--r--   0 rieder     (501) staff       (20)     4114 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_multi
+-rw-r--r--   0 rieder     (501) staff       (20)     5373 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_single
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.613518 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.674610 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/idl/
+-rw-r--r--   0 rieder     (501) staff       (20)      748 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/idl/noh.pro
+-rw-r--r--   0 rieder     (501) staff       (20)     1874 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/idl/plotdecay.pro
+-rw-r--r--   0 rieder     (501) staff       (20)    13414 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/idl/pltath.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.677424 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/
+-rw-r--r--   0 rieder     (501) staff       (20)      334 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/animateppm.m
+-rw-r--r--   0 rieder     (501) staff       (20)      508 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_construct_filename.m
+-rw-r--r--   0 rieder     (501) staff       (20)     6756 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_getvar.m
+-rw-r--r--   0 rieder     (501) staff       (20)      487 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_ijk_to_xyz.m
+-rw-r--r--   0 rieder     (501) staff       (20)     5020 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_init_grid.m
+-rw-r--r--   0 rieder     (501) staff       (20)     1851 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_ijk.m
+-rw-r--r--   0 rieder     (501) staff       (20)     2081 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_xyz.m
+-rw-r--r--   0 rieder     (501) staff       (20)     1354 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_palette.m
+-rw-r--r--   0 rieder     (501) staff       (20)      723 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_parse_filename.m
+-rw-r--r--   0 rieder     (501) staff       (20)      960 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_pcolor.m
+-rw-r--r--   0 rieder     (501) staff       (20)      403 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_plotbdry.m
+-rw-r--r--   0 rieder     (501) staff       (20)     4338 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_readbin.m
+-rw-r--r--   0 rieder     (501) staff       (20)      326 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_sizeof.m
+-rw-r--r--   0 rieder     (501) staff       (20)      642 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_ijk.m
+-rw-r--r--   0 rieder     (501) staff       (20)     2011 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_xyz.m
+-rw-r--r--   0 rieder     (501) staff       (20)     1169 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_text.m
+-rw-r--r--   0 rieder     (501) staff       (20)     1196 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_xyz_to_ijk.m
+-rw-r--r--   0 rieder     (501) staff       (20)       94 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/displayppm.m
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.678031 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/
+-rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/Read_par_standard.m
+-rw-r--r--   0 rieder     (501) staff       (20)     7217 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/join_lis.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1361 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/par_motion_movie.m
+-rw-r--r--   0 rieder     (501) staff       (20)     7804 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/sort_lis.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.678196 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/sm/
+-rw-r--r--   0 rieder     (501) staff       (20)     7015 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/sm/plot-smr-tab.sm
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.678347 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/vtk/
+-rw-r--r--   0 rieder     (501) staff       (20)    19489 2022-11-22 11:55:14.000000 amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/vtk/join_vtk.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:31:12.679596 amuse-athena-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-athena-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-athena-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-athena-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-athena-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-athena-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-athena-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-athena-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-athena-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-athena-2024.4.0/support/version.py
```

### Comparing `amuse-athena-2023.5.0/PKG-INFO` & `amuse-athena-2024.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-athena
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Athena
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
 
 This package installs the Athena community code for AMUSE.
```

### Comparing `amuse-athena-2023.5.0/amuse_athena.egg-info/PKG-INFO` & `amuse-athena-2024.4.0/amuse_athena.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-athena
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Athena
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
 
 This package installs the Athena community code for AMUSE.
```

### Comparing `amuse-athena-2023.5.0/amuse_athena.egg-info/SOURCES.txt` & `amuse-athena-2024.4.0/amuse_athena.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 amuse_athena.egg-info/PKG-INFO
 amuse_athena.egg-info/SOURCES.txt
 amuse_athena.egg-info/dependency_links.txt
 amuse_athena.egg-info/requires.txt
 amuse_athena.egg-info/top_level.txt
 src/amuse/community/athena/Makefile
 src/amuse/community/athena/__init__.py
+src/amuse/community/athena/_version.py
 src/amuse/community/athena/amuse_problem_3.1.c
 src/amuse/community/athena/amuse_problem_4.0.c
 src/amuse/community/athena/amuse_problem_4.1.c
 src/amuse/community/athena/download.py
 src/amuse/community/athena/interface.py
 src/amuse/community/athena/interface_3.1.c
 src/amuse/community/athena/interface_4.0.c
 src/amuse/community/athena/interface_4.1.c
 src/amuse/community/athena/makefile.patch
 src/amuse/community/athena/patch_files.py
-src/amuse/community/athena/version.py
 src/amuse/community/athena/src/athena/Makefile.in
 src/amuse/community/athena/src/athena/Makeoptions.in
 src/amuse/community/athena/src/athena/configure
 src/amuse/community/athena/src/athena/configure.ac
 src/amuse/community/athena/src/athena/install-sh
 src/amuse/community/athena/src/athena/autom4te.cache/output.0
 src/amuse/community/athena/src/athena/autom4te.cache/requests
```

### Comparing `amuse-athena-2023.5.0/setup.py` & `amuse-athena-2024.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.athena.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/athena/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/athena/_version.py",
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
         'amuse.community.athena': 'src/amuse/community/athena',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/Makefile` & `amuse-athena-2024.4.0/src/amuse/community/athena/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_3.1.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/amuse_problem_3.1.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_4.0.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/amuse_problem_4.0.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/amuse_problem_4.1.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/amuse_problem_4.1.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/download.py` & `amuse-athena-2024.4.0/src/amuse/community/athena/download.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/interface.py` & `amuse-athena-2024.4.0/src/amuse/community/athena/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/interface_3.1.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/interface_3.1.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/interface_4.0.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/interface_4.0.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/interface_4.1.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/interface_4.1.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/makefile.patch` & `amuse-athena-2024.4.0/src/amuse/community/athena/makefile.patch`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/patch_files.py` & `amuse-athena-2024.4.0/src/amuse/community/athena/patch_files.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/Makeoptions.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/Makeoptions.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/output.0` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/autom4te.cache/output.0`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/requests` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/autom4te.cache/requests`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/autom4te.cache/traces.0` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/autom4te.cache/traces.0`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/configure` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/configure`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/configure.ac` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/configure.ac`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/doc/pbs-script` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/doc/pbs-script`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/install-sh` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/install-sh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_array.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/ath_array.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_files.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/ath_files.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_log.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/ath_log.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/ath_signal.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/ath_signal.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/athena.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/athena.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/baton.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/baton.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/bvals_mhd.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/bvals_mhd.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/bvals_shear.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/bvals_shear.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/cc_pos.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/cc_pos.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/convert_var.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/convert_var.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/copyright.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/copyright.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/defs.h.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/defs.h.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_binary.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/dump_binary.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_history.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/dump_history.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_tab.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/dump_tab.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/dump_vtk.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/dump_vtk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/LICENSE` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/LICENSE`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/ath_fft.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/ath_fft.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/factor.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/factor.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_2d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/fft_3d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_2d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/pack_3d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/prototypes.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_2d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/fftsrc/remap_3d.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/globals.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/globals.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/bvals_grav.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/bvals_grav.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/prototypes.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft_obc.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_fft_obc.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/gravity/selfg_multigrid.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/gravity/selfg_multigrid.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/init_grid.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/init_grid.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/init_mesh.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/init_mesh.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_ctu.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_ctu.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl_sr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_1d_vl_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_ctu.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_ctu.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl_sr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_2d_vl_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_ctu.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_ctu.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl_sr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/integrate_3d_vl_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/integrators/prototypes.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/integrators/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/main.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/main.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/conduction.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/conduction.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/cool.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/cool.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/diff_dt.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/diff_dt.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/get_eta.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/get_eta.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/integrate_diffusion.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/integrate_diffusion.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/prototypes.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/resistivity.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/resistivity.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/microphysics/viscosity.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/microphysics/viscosity.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/new_dt.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/new_dt.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_pdf.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_pdf.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_pgm.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_pgm.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_ppm.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_ppm.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_tab.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_tab.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/output_vtk.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/output_vtk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/palette.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/palette.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/par.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/par.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/bvals_particle.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/bvals_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/dump_particle_history.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/dump_particle_history.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/feedback.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/feedback.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/init_particle.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/init_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/integrators_particle.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/integrators_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/output_particle.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/output_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/particle.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/particle.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/prototypes.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/particles/utils_particle.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/particles/utils_particle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/README` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/README`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/blast.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/blast.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/bubble.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/bubble.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/carbuncle.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/carbuncle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/collapse3d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/collapse3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw1d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cpaw3d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cpaw3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cshock1d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cshock1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/current_sheet.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/current_sheet.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cyladvect.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cyladvect.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylblast.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylblast.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylbphi.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylbphi.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylbr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylbr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylfieldloop.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylfieldloop.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylnewtmri.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylnewtmri.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylrayleigh.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylrayleigh.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylunif.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylunif.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwind.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylwind.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwindrot.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylwindrot.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/cylwindrotb.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/cylwindrotb.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/dmr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/dmr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/field_loop.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/field_loop.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/firehose.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/firehose.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hall_drift.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/hall_drift.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hb3.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/hb3.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hgb.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/hgb.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/hkdisk.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/hkdisk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/jeans.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/jeans.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/jet.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/jet.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/kh.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/kh.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave1d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/linear_wave3d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/linear_wave3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/lw_implode.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/lw_implode.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/noh.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/noh.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/orszag-tang.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/orszag-tang.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_circ.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_circ.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_collision.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_collision.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_epicycle.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_epicycle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_friction.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_friction.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave1d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_linearwave2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_shwave1d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_shwave1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_shwave2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_shwave2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_strat2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_strat2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/par_strat3d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/par_strat3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/pgflow.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/pgflow.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/planet-disk.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/planet-disk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/rotor.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/rotor.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/rt.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/rt.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shk_cloud.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shk_cloud.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset1d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shkset1d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset2d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shkset2d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shkset3d.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shkset3d.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/shu-osher.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/shu-osher.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/strat.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/strat.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_multi.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_multi.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_single.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/streaming2d_single.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_multi.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_multi.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_single.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/streaming3d_single.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/ti.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/ti.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/turb.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/turb.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prob/twoibw.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prob/twoibw.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/prototypes.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/esystem_prim.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/esystem_prim.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_dc.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_dc.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_plm.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_plm.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_ppm.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_ppm.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim2.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim2.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim3.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/lr_states_prim3.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/reconstruction/prototypes.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/reconstruction/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/restart.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/restart.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/Makefile.in` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/Makefile.in`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/esystem_roe.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/esystem_roe.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/exact.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/exact.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/exact_sr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/exact_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/force.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/force.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc_sr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hllc_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld_sr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlld_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle_sr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/hlle_sr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/prototypes.h` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/prototypes.h`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/roe.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/roe.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/rsolvers/two_shock.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/rsolvers/two_shock.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/show_config.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/show_config.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/smr.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/smr.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/src/utils.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/src/utils.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1125` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1125`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1203` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.einfeldt1203`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.leveque` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.leveque`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d-3lev1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.linear_wave1d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.noh` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.noh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.pgflow` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.pgflow`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.shu-osher` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.shu-osher`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.slow-moving-shock` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.slow-moving-shock`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-lw` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-lw`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-toro` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.sod-toro`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.twoibw` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/athinput.twoibw`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-hydro/run.linear_wave1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-hydro/run.linear_wave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.brio-wu` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.brio-wu`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cpaw1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cpaw1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cshock1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.cshock1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d-3lev1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.linear_wave1d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1a` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1b` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj1b`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2a` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2b` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj2b`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3a` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3b` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj3b`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4a` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4b` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4b`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.rj4d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.torrilhon` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/athinput.torrilhon`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.cpaw1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.cpaw1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.linear_wave1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.linear_wave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.test` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-mhd/run.test`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb2` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb2`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb3` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb3`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb4` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-hydro/athinput.mb4`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk2` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk2`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk3` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.FastShk3`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod2` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.K99sod2`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWoffFRF` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWoffFRF`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWonSRF` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SWonSRF`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SlowShock` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.SlowShock`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.brio-wu` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.brio-wu`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub2` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub2`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub3` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub3`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub4` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mub4`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubcontact` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubcontact`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubrot` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/1D-sr-mhd/athinput.mubrot`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.blast` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.carbuncle` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.carbuncle`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.dmr` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.dmr`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.jeans` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.jeans`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.kh` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.kh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d-3lev1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.linear_wave2d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.lw_implode` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.lw_implode`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.noh` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.noh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.pgflow` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.pgflow`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.rt` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.rt`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.shk_cloud` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-hydro/athinput.shk_cloud`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.Tconduct` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.Tconduct`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B10` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.blast_B10`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.cpaw2d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.cpaw2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.field_loop` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.field_loop`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hall_drift` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hall_drift`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hb3` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.hb3`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.kh` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.kh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d-3lev1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.linear_wave2d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.orszag-tang` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.orszag-tang`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rj2a` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rj2a`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rotor` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rotor`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rt` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/athinput.rt`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.cpaw2d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.cpaw2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.linear_wave2d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-mhd/run.linear_wave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.blast` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.jet` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-hydro/athinput.jet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.blast` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.brio-wu` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.brio-wu`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.current-sheet` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.current-sheet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.jet` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/2D-sr-mhd/athinput.jet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-160-FPwave.dat` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-160-FPwave.dat`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-40-FPwave.dat` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/Data-40-FPwave.dat`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.blast` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.carbuncle` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.carbuncle`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.fp-wave` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.fp-wave`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d-3lev1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.linear_wave3d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.nl-shwave` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.nl-shwave`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.noh` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.noh`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.pgflow` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.pgflow`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shk_cloud` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shk_cloud`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shwave` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.shwave`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.turb` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-hydro/athinput.turb`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.Tconduct` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.Tconduct`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B10` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.blast_B10`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.cpaw3d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.cpaw3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop4` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.field_loop4`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.hgb` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.hgb`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d-3lev1` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.linear_wave3d-3lev1`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rj2a_3d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rj2a_3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rt` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.rt`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.strat` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/athinput.strat`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.cpaw3d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.cpaw3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.linear_wave3d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-mhd/run.linear_wave3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/athinput.jet` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-hydro/athinput.jet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.blast` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.blast`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.jet` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/3D-sr-mhd/athinput.jet`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cyladvect-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B0-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B0-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B1-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylblast_B10-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbphi-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylbr-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylfieldloop-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylnewtmri` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylnewtmri`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylrayleigh-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylrayleigh-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylunif-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylunif-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwind-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrot-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.cylwindrotb-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.hkdisk-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/athinput.hkdisk-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cyladvect-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cyladvect-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast.mpi-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylblast.mpi-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylfieldloop-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylfieldloop-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylunif-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylunif-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrot.mpi-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-1D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-1D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-2D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-2D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-3D` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/cylindrical/run.cylwindrotb.mpi-3D`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_circ` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_circ`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_collision` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_collision`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_epicycle` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_epicycle`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_friction` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_friction`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave2d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_linearwave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave1d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave1d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave2d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_shwave2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat2d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat2d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat3d` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.par_strat3d`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_multi` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_multi`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_single` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming2d_single`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_multi` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_multi`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_single` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/tst/particle/athinput.streaming3d_single`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/noh.pro` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/idl/noh.pro`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/plotdecay.pro` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/idl/plotdecay.pro`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/idl/pltath.pro` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/idl/pltath.pro`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_getvar.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_getvar.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_init_grid.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_init_grid.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_ijk.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_ijk.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_xyz.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_lineout_xyz.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_palette.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_palette.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_parse_filename.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_parse_filename.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_pcolor.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_pcolor.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_readbin.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_readbin.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_ijk.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_ijk.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_xyz.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_slice_xyz.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_text.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_text.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/matlab/ath_xyz_to_ijk.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/matlab/ath_xyz_to_ijk.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/Read_par_standard.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/Read_par_standard.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/join_lis.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/join_lis.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/par_motion_movie.m` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/par_motion_movie.m`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/particle/sort_lis.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/particle/sort_lis.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/sm/plot-smr-tab.sm` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/sm/plot-smr-tab.sm`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/src/amuse/community/athena/src/athena/vis/vtk/join_vtk.c` & `amuse-athena-2024.4.0/src/amuse/community/athena/src/athena/vis/vtk/join_vtk.c`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/support/__init__.py` & `amuse-athena-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/support/classifiers.py` & `amuse-athena-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/support/config.py` & `amuse-athena-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/support/generate_main.py` & `amuse-athena-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/support/getsp.class` & `amuse-athena-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/support/getsp.java` & `amuse-athena-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/support/misc.py` & `amuse-athena-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-athena-2023.5.0/support/setup_codes.py` & `amuse-athena-2024.4.0/support/setup_codes.py`

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

