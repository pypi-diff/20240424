# Comparing `tmp/amuse-simplex-2023.5.0.tar.gz` & `tmp/amuse-simplex-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-simplex-2023.5.0.tar", last modified: Wed May 17 10:19:37 2023, max compression
+gzip compressed data, was "amuse-simplex-2024.4.0.tar", last modified: Wed Apr 24 16:32:50 2024, max compression
```

## Comparing `amuse-simplex-2023.5.0.tar` & `amuse-simplex-2024.4.0.tar`

### file list

```diff
@@ -1,428 +1,428 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.416102 amuse-simplex-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-simplex-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1189 2023-05-17 10:19:37.415935 amuse-simplex-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       60 2022-11-22 11:55:14.000000 amuse-simplex-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.315498 amuse-simplex-2023.5.0/amuse_simplex.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1189 2023-05-17 10:19:35.000000 amuse-simplex-2023.5.0/amuse_simplex.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)    26107 2023-05-17 10:19:37.000000 amuse-simplex-2023.5.0/amuse_simplex.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:35.000000 amuse-simplex-2023.5.0/amuse_simplex.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       30 2023-05-17 10:19:35.000000 amuse-simplex-2023.5.0/amuse_simplex.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:35.000000 amuse-simplex-2023.5.0/amuse_simplex.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-simplex-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:37.416154 amuse-simplex-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1839 2022-11-22 11:55:14.000000 amuse-simplex-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.310967 amuse-simplex-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.311020 amuse-simplex-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.311075 amuse-simplex-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.316591 amuse-simplex-2023.5.0/src/amuse/community/simplex/
--rw-r--r--   0 rieder     (501) staff       (20)     2577 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       31 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.311208 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.322093 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/
--rw-r--r--   0 rieder     (501) staff       (20)     3248 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/C.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6504 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/C.cool
--rw-r--r--   0 rieder     (501) staff       (20)     3245 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Fe.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     3603 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Fe.cool
--rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/H.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/H.cool
--rw-r--r--   0 rieder     (501) staff       (20)    23681 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/H2.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/He.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/He.cool
--rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/N.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/N.cool
--rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Ne.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Ne.cool
--rw-r--r--   0 rieder     (501) staff       (20)     3253 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/O.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/O.cool
--rw-r--r--   0 rieder     (501) staff       (20)     3252 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Si.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     2703 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Si.cool
--rw-r--r--   0 rieder     (501) staff       (20)    41934 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/vertices_10.txt
--rw-r--r--   0 rieder     (501) staff       (20)    38547 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/vertices_test.txt
--rw-r--r--   0 rieder     (501) staff       (20)    38798 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/vertices_test2.txt
--rw-r--r--   0 rieder     (501) staff       (20)    50786 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/vertices_test3.txt
--rw-r--r--   0 rieder     (501) staff       (20)    48398 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/interface.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.322537 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/
--rw-r--r--   0 rieder     (501) staff       (20)     4300 2023-04-15 06:03:30.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/Makefile
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.322892 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/bin/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/bin/empty_dir.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.323038 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/obj/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/obj/empty_dir.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.313978 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.311761 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.330397 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/
--rw-r--r--   0 rieder     (501) staff       (20)     4818 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm.h
--rw-r--r--   0 rieder     (501) staff       (20)     3763 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_fitsio.h
--rw-r--r--   0 rieder     (501) staff       (20)     7249 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_healpix_tools.h
--rw-r--r--   0 rieder     (501) staff       (20)     4067 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_map_tools.h
--rw-r--r--   0 rieder     (501) staff       (20)     4773 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_powspec_tools.h
--rw-r--r--   0 rieder     (501) staff       (20)    14819 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/arr.h
--rw-r--r--   0 rieder     (501) staff       (20)     9531 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/cxxutils.h
--rw-r--r--   0 rieder     (501) staff       (20)     7291 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/datatypes.h
--rw-r--r--   0 rieder     (501) staff       (20)     2937 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fftpack_support.h
--rw-r--r--   0 rieder     (501) staff       (20)    16598 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fitshandle.h
--rw-r--r--   0 rieder     (501) staff       (20)   102034 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fitsio.h
--rw-r--r--   0 rieder     (501) staff       (20)     2186 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/geom_utils.h
--rw-r--r--   0 rieder     (501) staff       (20)    11109 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_base.h
--rw-r--r--   0 rieder     (501) staff       (20)    10973 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_base2.h
--rw-r--r--   0 rieder     (501) staff       (20)     1817 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_data_io.h
--rw-r--r--   0 rieder     (501) staff       (20)    10627 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_map.h
--rw-r--r--   0 rieder     (501) staff       (20)     2833 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_map_fitsio.h
--rw-r--r--   0 rieder     (501) staff       (20)    20229 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/longnam.h
--rw-r--r--   0 rieder     (501) staff       (20)     6068 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/ls_fft.h
--rw-r--r--   0 rieder     (501) staff       (20)     3385 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/lsconstants.h
--rw-r--r--   0 rieder     (501) staff       (20)     2567 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/message_error.h
--rw-r--r--   0 rieder     (501) staff       (20)     2165 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/openmp_support.h
--rw-r--r--   0 rieder     (501) staff       (20)     3825 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/paramfile.h
--rw-r--r--   0 rieder     (501) staff       (20)     4246 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/planck_rng.h
--rw-r--r--   0 rieder     (501) staff       (20)     3366 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/pointing.h
--rw-r--r--   0 rieder     (501) staff       (20)     4210 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/powspec.h
--rw-r--r--   0 rieder     (501) staff       (20)     1801 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/powspec_fitsio.h
--rw-r--r--   0 rieder     (501) staff       (20)     5621 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/rotmatrix.h
--rw-r--r--   0 rieder     (501) staff       (20)     2574 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/simparams.h
--rw-r--r--   0 rieder     (501) staff       (20)     5824 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/tga_image.h
--rw-r--r--   0 rieder     (501) staff       (20)     3619 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/trafos.h
--rw-r--r--   0 rieder     (501) staff       (20)     3964 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/vec3.h
--rw-r--r--   0 rieder     (501) staff       (20)     5681 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/xcomplex.h
--rw-r--r--   0 rieder     (501) staff       (20)     5687 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/ylmgen.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.330573 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/lib/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/lib/empty_dir.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.339376 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/
--rw-r--r--   0 rieder     (501) staff       (20)     5433 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/Healpix_cxx.dox
--rw-r--r--   0 rieder     (501) staff       (20)     1979 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     4818 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm.h
--rw-r--r--   0 rieder     (501) staff       (20)     4649 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm2map_cxx.cc
--rw-r--r--   0 rieder     (501) staff       (20)      903 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm2map_cxx.par.txt
--rw-r--r--   0 rieder     (501) staff       (20)     7220 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_fitsio.cc
--rw-r--r--   0 rieder     (501) staff       (20)     3763 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_fitsio.h
--rw-r--r--   0 rieder     (501) staff       (20)    11358 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_healpix_tools.cc
--rw-r--r--   0 rieder     (501) staff       (20)     7249 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_healpix_tools.h
--rw-r--r--   0 rieder     (501) staff       (20)    22943 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_map_tools.cc
--rw-r--r--   0 rieder     (501) staff       (20)     4067 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_map_tools.h
--rw-r--r--   0 rieder     (501) staff       (20)    16281 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_powspec_tools.cc
--rw-r--r--   0 rieder     (501) staff       (20)     4773 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_powspec_tools.h
--rw-r--r--   0 rieder     (501) staff       (20)     4408 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/anafast_cxx.cc
--rw-r--r--   0 rieder     (501) staff       (20)      945 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/anafast_cxx.par.txt
--rw-r--r--   0 rieder     (501) staff       (20)     2409 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/calc_powspec.cc
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.344561 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/
--rw-r--r--   0 rieder     (501) staff       (20)     1662 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)    14819 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/arr.h
--rw-r--r--   0 rieder     (501) staff       (20)      170 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxsupport.dox
--rw-r--r--   0 rieder     (501) staff       (20)     8750 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxutils.cc
--rw-r--r--   0 rieder     (501) staff       (20)     9531 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxutils.h
--rw-r--r--   0 rieder     (501) staff       (20)     7291 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/datatypes.h
--rw-r--r--   0 rieder     (501) staff       (20)     2937 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fftpack_support.h
--rw-r--r--   0 rieder     (501) staff       (20)    26850 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fitshandle.cc
--rw-r--r--   0 rieder     (501) staff       (20)    16598 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fitshandle.h
--rw-r--r--   0 rieder     (501) staff       (20)    61838 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/font_data.inc
--rw-r--r--   0 rieder     (501) staff       (20)     2186 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/geom_utils.h
--rw-r--r--   0 rieder     (501) staff       (20)     3385 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/lsconstants.h
--rw-r--r--   0 rieder     (501) staff       (20)     2567 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/message_error.h
--rw-r--r--   0 rieder     (501) staff       (20)     2165 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/openmp_support.h
--rw-r--r--   0 rieder     (501) staff       (20)     3825 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/paramfile.h
--rw-r--r--   0 rieder     (501) staff       (20)     4246 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/planck_rng.h
--rw-r--r--   0 rieder     (501) staff       (20)     3366 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/pointing.h
--rw-r--r--   0 rieder     (501) staff       (20)     4910 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/rotmatrix.cc
--rw-r--r--   0 rieder     (501) staff       (20)     5621 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/rotmatrix.h
--rw-r--r--   0 rieder     (501) staff       (20)     2344 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/simparams.cc
--rw-r--r--   0 rieder     (501) staff       (20)     2574 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/simparams.h
--rw-r--r--   0 rieder     (501) staff       (20)     3680 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/tga_image.cc
--rw-r--r--   0 rieder     (501) staff       (20)     5824 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/tga_image.h
--rw-r--r--   0 rieder     (501) staff       (20)     5203 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/trafos.cc
--rw-r--r--   0 rieder     (501) staff       (20)     3619 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/trafos.h
--rw-r--r--   0 rieder     (501) staff       (20)     3964 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/vec3.h
--rw-r--r--   0 rieder     (501) staff       (20)     5681 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/xcomplex.h
--rw-r--r--   0 rieder     (501) staff       (20)    21724 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base.cc
--rw-r--r--   0 rieder     (501) staff       (20)    11109 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base.h
--rw-r--r--   0 rieder     (501) staff       (20)    16091 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base2.cc
--rw-r--r--   0 rieder     (501) staff       (20)    10973 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base2.h
--rw-r--r--   0 rieder     (501) staff       (20)     3484 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_data_io.cc
--rw-r--r--   0 rieder     (501) staff       (20)     1817 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_data_io.h
--rw-r--r--   0 rieder     (501) staff       (20)     2885 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map.cc
--rw-r--r--   0 rieder     (501) staff       (20)    10627 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map.h
--rw-r--r--   0 rieder     (501) staff       (20)     4624 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map_fitsio.cc
--rw-r--r--   0 rieder     (501) staff       (20)     2833 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map_fitsio.h
--rw-r--r--   0 rieder     (501) staff       (20)     3134 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/hotspots_cxx.cc
--rw-r--r--   0 rieder     (501) staff       (20)    22202 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/hpxtest.cc
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.346187 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/
--rw-r--r--   0 rieder     (501) staff       (20)      451 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     1758 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/README
--rw-r--r--   0 rieder     (501) staff       (20)     4532 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/bluestein.c
--rw-r--r--   0 rieder     (501) staff       (20)     1297 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/bluestein.h
--rw-r--r--   0 rieder     (501) staff       (20)    46443 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/fftpack.c
--rw-r--r--   0 rieder     (501) staff       (20)     1569 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/fftpack.h
--rw-r--r--   0 rieder     (501) staff       (20)      102 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/libfftpack.dox
--rw-r--r--   0 rieder     (501) staff       (20)     6098 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/ls_fft.c
--rw-r--r--   0 rieder     (501) staff       (20)     6068 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/ls_fft.h
--rw-r--r--   0 rieder     (501) staff       (20)    11372 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/map2tga.cc
--rw-r--r--   0 rieder     (501) staff       (20)     2044 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/map2tga.par.txt
--rw-r--r--   0 rieder     (501) staff       (20)     2280 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/median_filter.cc
--rw-r--r--   0 rieder     (501) staff       (20)     4790 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/mult_alm.cc
--rw-r--r--   0 rieder     (501) staff       (20)      943 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/mult_alm.par.txt
--rw-r--r--   0 rieder     (501) staff       (20)     2803 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec.cc
--rw-r--r--   0 rieder     (501) staff       (20)     4210 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec.h
--rw-r--r--   0 rieder     (501) staff       (20)     4652 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec_fitsio.cc
--rw-r--r--   0 rieder     (501) staff       (20)     1801 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec_fitsio.h
--rw-r--r--   0 rieder     (501) staff       (20)     4201 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/rotalm_cxx.cc
--rw-r--r--   0 rieder     (501) staff       (20)     3717 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/smoothing_cxx.cc
--rw-r--r--   0 rieder     (501) staff       (20)      780 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/smoothing_cxx.par.txt
--rw-r--r--   0 rieder     (501) staff       (20)     3912 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/syn_alm_cxx.cc
--rw-r--r--   0 rieder     (501) staff       (20)      690 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/syn_alm_cxx.par.txt
--rw-r--r--   0 rieder     (501) staff       (20)     3103 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/udgrade_cxx.cc
--rw-r--r--   0 rieder     (501) staff       (20)     5687 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/ylmgen.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.347872 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/
--rw-r--r--   0 rieder     (501) staff       (20)     4870 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/array_class.h
--rw-r--r--   0 rieder     (501) staff       (20)    19775 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    19571 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w.h
--rw-r--r--   0 rieder     (501) staff       (20)    19717 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_parallel.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    18351 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_parallel.h
--rw-r--r--   0 rieder     (501) staff       (20)    21649 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_serial.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    19637 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_serial.h
--rw-r--r--   0 rieder     (501) staff       (20)    10515 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/hdf5_routines.cpp
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.348317 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hilbert/
--rw-r--r--   0 rieder     (501) staff       (20)    46290 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hilbert/hilbert.c
--rw-r--r--   0 rieder     (501) staff       (20)     5769 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hilbert/hilbert.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.348741 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/keyValue/
--rw-r--r--   0 rieder     (501) staff       (20)     4896 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/keyValue/configfile.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     7253 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/keyValue/configfile.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.351007 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/
--rw-r--r--   0 rieder     (501) staff       (20)     2816 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/array.h
--rw-r--r--   0 rieder     (501) staff       (20)     2434 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/array2d.h
--rw-r--r--   0 rieder     (501) staff       (20)      340 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/demo.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     1043 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/numtraits.h
--rw-r--r--   0 rieder     (501) staff       (20)     4367 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/octree.h
--rw-r--r--   0 rieder     (501) staff       (20)    24927 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/octree.tcc
--rw-r--r--   0 rieder     (501) staff       (20)     4283 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/octree.vcproj
--rw-r--r--   0 rieder     (501) staff       (20)     1309 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/point3d.h
--rw-r--r--   0 rieder     (501) staff       (20)     2268 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/shareddata.h
--rw-r--r--   0 rieder     (501) staff       (20)     5394 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/tinyvector.h
--rw-r--r--   0 rieder     (501) staff       (20)     6424 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/tree_structures.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2346 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/tree_structures.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.353300 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/
--rw-r--r--   0 rieder     (501) staff       (20)     2458 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/Announce.txt
--rw-r--r--   0 rieder     (501) staff       (20)    14404 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/CMakeLists.txt
--rw-r--r--   0 rieder     (501) staff       (20)     1635 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/COPYING.txt
--rw-r--r--   0 rieder     (501) staff       (20)      421 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/File_id.diz
--rw-r--r--   0 rieder     (501) staff       (20)    23167 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     1463 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/QHULL-GO.lnk
--rw-r--r--   0 rieder     (501) staff       (20)    17514 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/README.txt
--rw-r--r--   0 rieder     (501) staff       (20)      958 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/REGISTER.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.355431 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/
--rw-r--r--   0 rieder     (501) staff       (20)      562 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-eg
--rw-r--r--   0 rieder     (501) staff       (20)     1141 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-html
--rw-r--r--   0 rieder     (501) staff       (20)     1986 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-libqhull
--rw-r--r--   0 rieder     (501) staff       (20)      544 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-main
--rw-r--r--   0 rieder     (501) staff       (20)      333 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile.am
--rw-r--r--   0 rieder     (501) staff       (20)      883 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/README
--rwxr-xr-x   0 rieder     (501) staff       (20)      869 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/bootstrap.sh
--rw-r--r--   0 rieder     (501) staff       (20)     4835 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/changelog
--rw-r--r--   0 rieder     (501) staff       (20)      464 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/configure.ac
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.356040 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/
--rw-r--r--   0 rieder     (501) staff       (20)       37 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/00list
--rwxr-xr-x   0 rieder     (501) staff       (20)      932 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/QHpointer.dpatch
--rwxr-xr-x   0 rieder     (501) staff       (20)     1456 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/make-new-msg.dpatch
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.358723 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/
--rwxr-xr-x   0 rieder     (501) staff       (20)      485 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/Qhull-go.bat
--rwxr-xr-x   0 rieder     (501) staff       (20)     3179 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/make-vcproj.sh
--rwxr-xr-x   0 rieder     (501) staff       (20)     3384 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_eg
--rwxr-xr-x   0 rieder     (501) staff       (20)     2106 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_egtest
--rwxr-xr-x   0 rieder     (501) staff       (20)    12186 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test
--rw-r--r--   0 rieder     (501) staff       (20)   405961 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test-ok.txt
--rwxr-xr-x   0 rieder     (501) staff       (20)    30923 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test.bat
--rwxr-xr-x   0 rieder     (501) staff       (20)     9647 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/qhull-zip.sh
--rw-r--r--   0 rieder     (501) staff       (20)    36996 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/qhulltest-ok.txt
--rw-r--r--   0 rieder     (501) staff       (20)    14000 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/index.htm
--rw-r--r--   0 rieder     (501) staff       (20)    13134 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/qhull-2012.1-src-tgz.md5sum
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.361275 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/
--rw-r--r--   0 rieder     (501) staff       (20)    82851 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/Changes.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.371292 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/
--rw-r--r--   0 rieder     (501) staff       (20)     6701 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     6071 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/Mborland
--rw-r--r--   0 rieder     (501) staff       (20)    42431 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom.c
--rw-r--r--   0 rieder     (501) staff       (20)     7193 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom.h
--rw-r--r--   0 rieder     (501) staff       (20)    65555 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom2.c
--rw-r--r--   0 rieder     (501) staff       (20)    70589 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/global.c
--rw-r--r--   0 rieder     (501) staff       (20)    10771 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/index.htm
--rw-r--r--   0 rieder     (501) staff       (20)   133486 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/io.c
--rw-r--r--   0 rieder     (501) staff       (20)     7926 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/io.h
--rw-r--r--   0 rieder     (501) staff       (20)    51817 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.c
--rw-r--r--   0 rieder     (501) staff       (20)    50146 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.h
--rw-r--r--   0 rieder     (501) staff       (20)     1515 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.pro
--rw-r--r--   0 rieder     (501) staff       (20)    19024 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/mem.c
--rw-r--r--   0 rieder     (501) staff       (20)     8537 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/mem.h
--rw-r--r--   0 rieder     (501) staff       (20)   121690 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/merge.c
--rw-r--r--   0 rieder     (501) staff       (20)     7301 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/merge.h
--rw-r--r--   0 rieder     (501) staff       (20)    39828 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly.c
--rw-r--r--   0 rieder     (501) staff       (20)    10935 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly.h
--rw-r--r--   0 rieder     (501) staff       (20)   110261 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly2.c
--rw-r--r--   0 rieder     (501) staff       (20)    13066 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-geom.htm
--rw-r--r--   0 rieder     (501) staff       (20)     7348 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-globa.htm
--rw-r--r--   0 rieder     (501) staff       (20)    14430 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-io.htm
--rw-r--r--   0 rieder     (501) staff       (20)     6145 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-mem.htm
--rw-r--r--   0 rieder     (501) staff       (20)    15144 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-merge.htm
--rw-r--r--   0 rieder     (501) staff       (20)    20940 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-poly.htm
--rw-r--r--   0 rieder     (501) staff       (20)    12695 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-qhull.htm
--rw-r--r--   0 rieder     (501) staff       (20)    13092 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-set.htm
--rw-r--r--   0 rieder     (501) staff       (20)     7078 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-stat.htm
--rw-r--r--   0 rieder     (501) staff       (20)    11351 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-user.htm
--rw-r--r--   0 rieder     (501) staff       (20)     7543 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qhull-exports.def
--rw-r--r--   0 rieder     (501) staff       (20)     4926 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qhull_a.h
--rw-r--r--   0 rieder     (501) staff       (20)    33590 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qset.c
--rw-r--r--   0 rieder     (501) staff       (20)    14830 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qset.h
--rw-r--r--   0 rieder     (501) staff       (20)     6357 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/random.c
--rw-r--r--   0 rieder     (501) staff       (20)      935 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/random.h
--rw-r--r--   0 rieder     (501) staff       (20)    22239 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/rboxlib.c
--rw-r--r--   0 rieder     (501) staff       (20)    30502 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/stat.c
--rw-r--r--   0 rieder     (501) staff       (20)    12877 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/stat.h
--rw-r--r--   0 rieder     (501) staff       (20)    19708 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/user.c
--rw-r--r--   0 rieder     (501) staff       (20)    28181 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/user.h
--rw-r--r--   0 rieder     (501) staff       (20)     1495 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/usermem.c
--rw-r--r--   0 rieder     (501) staff       (20)     1790 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/userprintf.c
--rw-r--r--   0 rieder     (501) staff       (20)     1620 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/userprintf_rbox.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.379453 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/
--rw-r--r--   0 rieder     (501) staff       (20)     3769 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Coordinates.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    15543 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Coordinates.h
--rw-r--r--   0 rieder     (501) staff       (20)     8182 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/PointCoordinates.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     6806 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/PointCoordinates.h
--rw-r--r--   0 rieder     (501) staff       (20)    15907 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Qhull.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     6391 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Qhull.h
--rw-r--r--   0 rieder     (501) staff       (20)     2361 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullError.h
--rw-r--r--   0 rieder     (501) staff       (20)    15691 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacet.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     6857 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacet.h
--rw-r--r--   0 rieder     (501) staff       (20)     4285 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetList.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4082 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetList.h
--rw-r--r--   0 rieder     (501) staff       (20)     3639 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetSet.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3614 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetSet.h
--rw-r--r--   0 rieder     (501) staff       (20)     4357 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullHyperplane.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     6025 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullHyperplane.h
--rw-r--r--   0 rieder     (501) staff       (20)     7882 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullIterator.h
--rw-r--r--   0 rieder     (501) staff       (20)    11956 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullLinkedList.h
--rw-r--r--   0 rieder     (501) staff       (20)     4945 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoint.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     6159 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoint.h
--rw-r--r--   0 rieder     (501) staff       (20)     4691 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPointSet.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    12576 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPointSet.h
--rw-r--r--   0 rieder     (501) staff       (20)     5026 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoints.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    16146 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoints.h
--rw-r--r--   0 rieder     (501) staff       (20)     3376 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullQh.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     1314 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullQh.h
--rw-r--r--   0 rieder     (501) staff       (20)     2979 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullRidge.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4117 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullRidge.h
--rw-r--r--   0 rieder     (501) staff       (20)     1255 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSet.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    11623 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSet.h
--rw-r--r--   0 rieder     (501) staff       (20)      783 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSets.h
--rw-r--r--   0 rieder     (501) staff       (20)      881 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullStat.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     1308 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullStat.h
--rw-r--r--   0 rieder     (501) staff       (20)     2773 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertex.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3862 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertex.h
--rw-r--r--   0 rieder     (501) staff       (20)     3310 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertexSet.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3269 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertexSet.h
--rw-r--r--   0 rieder     (501) staff       (20)     5787 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RboxPoints.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2109 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RboxPoints.h
--rw-r--r--   0 rieder     (501) staff       (20)     3350 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadError.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3135 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadError.h
--rw-r--r--   0 rieder     (501) staff       (20)     3133 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadLogEvent.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3536 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadLogEvent.h
--rw-r--r--   0 rieder     (501) staff       (20)    11749 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/UsingLibQhull.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     6172 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/UsingLibQhull.h
--rw-r--r--   0 rieder     (501) staff       (20)     1516 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/functionObjects.h
--rw-r--r--   0 rieder     (501) staff       (20)     1778 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/libqhullcpp.pro
--rw-r--r--   0 rieder     (501) staff       (20)     3565 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/qhull_interface.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2700 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/qt-qhull.cpp
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.379768 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/
--rw-r--r--   0 rieder     (501) staff       (20)      709 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/libqhullp.pro
--rw-r--r--   0 rieder     (501) staff       (20)     7488 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/qhull_p-exports.def
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.379941 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstatic/
--rw-r--r--   0 rieder     (501) staff       (20)      550 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstatic/libqhullstatic.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.380151 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstaticp/
--rw-r--r--   0 rieder     (501) staff       (20)      551 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstaticp/libqhullstaticp.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.380509 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qconvex/
--rw-r--r--   0 rieder     (501) staff       (20)    12363 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qconvex/qconvex.c
--rw-r--r--   0 rieder     (501) staff       (20)      222 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qconvex/qconvex.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.380829 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qdelaunay/
--rw-r--r--   0 rieder     (501) staff       (20)    12032 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qdelaunay/qdelaun.c
--rw-r--r--   0 rieder     (501) staff       (20)      227 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qdelaunay/qdelaunay.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.381320 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhalf/
--rw-r--r--   0 rieder     (501) staff       (20)    12005 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhalf/qhalf.c
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhalf/qhalf.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.381781 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull/
--rw-r--r--   0 rieder     (501) staff       (20)      213 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull/qhull.pro
--rw-r--r--   0 rieder     (501) staff       (20)    15724 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull/unix.c
--rw-r--r--   0 rieder     (501) staff       (20)     2803 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-all.pro
--rw-r--r--   0 rieder     (501) staff       (20)      608 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-c.pri
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-cpp.pri
--rw-r--r--   0 rieder     (501) staff       (20)      678 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-shared.pri
--rw-r--r--   0 rieder     (501) staff       (20)      759 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-sharedp.pri
--rw-r--r--   0 rieder     (501) staff       (20)     1253 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-libqhull-src.pri
--rw-r--r--   0 rieder     (501) staff       (20)     3164 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-warn.pri
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.386392 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/
--rw-r--r--   0 rieder     (501) staff       (20)    13536 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Coordinates_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    11090 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/PointCoordinates_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     5742 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Point_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4869 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacetList_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4010 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacetSet_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     8632 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacet_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    11248 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullHyperplane_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     8965 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullLinkedList_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    10055 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPointSet_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    10363 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPoint_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    13003 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPoints_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4456 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullRidge_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    12138 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullSet_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     4777 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullVertexSet_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     5314 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullVertex_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    11775 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Qhull_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     6052 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RboxPoints_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     1852 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RoadTest.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2084 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RoadTest.h
--rw-r--r--   0 rieder     (501) staff       (20)     7814 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/UsingLibQhull_test.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2510 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/qhulltest.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      946 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/qhulltest.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.386759 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qvoronoi/
--rw-r--r--   0 rieder     (501) staff       (20)    11433 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qvoronoi/qvoronoi.c
--rw-r--r--   0 rieder     (501) staff       (20)      226 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qvoronoi/qvoronoi.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.387092 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/rbox/
--rw-r--r--   0 rieder     (501) staff       (20)     3547 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/rbox/rbox.c
--rw-r--r--   0 rieder     (501) staff       (20)      205 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/rbox/rbox.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.387481 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/
--rw-r--r--   0 rieder     (501) staff       (20)    32472 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/testqset.c
--rw-r--r--   0 rieder     (501) staff       (20)      621 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/testqset.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.387846 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg/
--rw-r--r--   0 rieder     (501) staff       (20)    11089 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg/user_eg.c
--rw-r--r--   0 rieder     (501) staff       (20)      231 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg/user_eg.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.388240 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg2/
--rw-r--r--   0 rieder     (501) staff       (20)    26662 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg2/user_eg2.c
--rw-r--r--   0 rieder     (501) staff       (20)      256 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg2/user_eg2.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.388577 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg3/
--rw-r--r--   0 rieder     (501) staff       (20)     4564 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg3/user_eg3.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      256 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg3/user_eg3.pro
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.314037 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.403837 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/
--rw-r--r--   0 rieder     (501) staff       (20)   753132 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map16.h
--rw-r--r--   0 rieder     (501) staff       (20)   993818 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map21.h
--rw-r--r--   0 rieder     (501) staff       (20)  1523503 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map32.h
--rw-r--r--   0 rieder     (501) staff       (20)  2004913 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map42.h
--rw-r--r--   0 rieder     (501) staff       (20)  3064038 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map64.h
--rw-r--r--   0 rieder     (501) staff       (20)  4027038 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map84.h
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.414282 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/
--rw-r--r--   0 rieder     (501) staff       (20)    12117 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Common.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     5730 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Common.h
--rw-r--r--   0 rieder     (501) staff       (20)     5224 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Main.cpp
--rw-r--r--   0 rieder     (501) staff       (20)      732 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Main.h
--rw-r--r--   0 rieder     (501) staff       (20)   289150 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/SimpleX.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    21034 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/SimpleX.h
--rw-r--r--   0 rieder     (501) staff       (20)     7124 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Structs.cpp
--rw-r--r--   0 rieder     (501) staff       (20)    21893 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Structs.h
--rw-r--r--   0 rieder     (501) staff       (20)    35337 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/amuse_interface.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3234 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/amuse_interface.h
--rw-r--r--   0 rieder     (501) staff       (20)     4502 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/rates.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     3026 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/rates.h
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:35.000000 amuse-simplex-2023.5.0/src/amuse/community/simplex/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:37.415686 amuse-simplex-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-simplex-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-simplex-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-simplex-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.035500 amuse-simplex-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-simplex-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1249 2024-04-24 16:32:50.035269 amuse-simplex-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       60 2022-11-22 11:55:14.000000 amuse-simplex-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.034921 amuse-simplex-2024.4.0/amuse_simplex.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1249 2024-04-24 16:32:48.000000 amuse-simplex-2024.4.0/amuse_simplex.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)    26108 2024-04-24 16:32:49.000000 amuse-simplex-2024.4.0/amuse_simplex.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:48.000000 amuse-simplex-2024.4.0/amuse_simplex.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       30 2024-04-24 16:32:48.000000 amuse-simplex-2024.4.0/amuse_simplex.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:48.000000 amuse-simplex-2024.4.0/amuse_simplex.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-simplex-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:50.035559 amuse-simplex-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1642 2024-04-24 15:35:29.000000 amuse-simplex-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.952791 amuse-simplex-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.952843 amuse-simplex-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.952893 amuse-simplex-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.957821 amuse-simplex-2024.4.0/src/amuse/community/simplex/
+-rw-r--r--   0 rieder     (501) staff       (20)     2577 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       31 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:48.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/_version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.953005 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.961552 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/
+-rw-r--r--   0 rieder     (501) staff       (20)     3248 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/C.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6504 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/C.cool
+-rw-r--r--   0 rieder     (501) staff       (20)     3245 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Fe.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     3603 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Fe.cool
+-rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/H.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/H.cool
+-rw-r--r--   0 rieder     (501) staff       (20)    23681 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/H2.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/He.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/He.cool
+-rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/N.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/N.cool
+-rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Ne.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Ne.cool
+-rw-r--r--   0 rieder     (501) staff       (20)     3253 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/O.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/O.cool
+-rw-r--r--   0 rieder     (501) staff       (20)     3252 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Si.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     2703 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Si.cool
+-rw-r--r--   0 rieder     (501) staff       (20)    41934 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/vertices_10.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    38547 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/vertices_test.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    38798 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/vertices_test2.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    50786 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/vertices_test3.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    48398 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.961743 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     4300 2023-04-15 06:03:30.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/Makefile
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.961906 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/bin/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/bin/empty_dir.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.962023 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/obj/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/obj/empty_dir.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.955467 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.953466 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.968238 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/
+-rw-r--r--   0 rieder     (501) staff       (20)     4818 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3763 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_fitsio.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7249 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_healpix_tools.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4067 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_map_tools.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4773 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_powspec_tools.h
+-rw-r--r--   0 rieder     (501) staff       (20)    14819 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/arr.h
+-rw-r--r--   0 rieder     (501) staff       (20)     9531 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/cxxutils.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7291 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/datatypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2937 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fftpack_support.h
+-rw-r--r--   0 rieder     (501) staff       (20)    16598 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fitshandle.h
+-rw-r--r--   0 rieder     (501) staff       (20)   102034 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fitsio.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2186 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/geom_utils.h
+-rw-r--r--   0 rieder     (501) staff       (20)    11109 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_base.h
+-rw-r--r--   0 rieder     (501) staff       (20)    10973 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_base2.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1817 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_data_io.h
+-rw-r--r--   0 rieder     (501) staff       (20)    10627 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_map.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2833 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_map_fitsio.h
+-rw-r--r--   0 rieder     (501) staff       (20)    20229 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/longnam.h
+-rw-r--r--   0 rieder     (501) staff       (20)     6068 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/ls_fft.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3385 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/lsconstants.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2567 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/message_error.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2165 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/openmp_support.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3825 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/paramfile.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4246 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/planck_rng.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3366 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/pointing.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4210 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/powspec.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1801 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/powspec_fitsio.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5621 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/rotmatrix.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2574 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/simparams.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5824 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/tga_image.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3619 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/trafos.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3964 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/vec3.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5681 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/xcomplex.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5687 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/ylmgen.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.968399 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/lib/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/lib/empty_dir.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.976946 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     5433 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/Healpix_cxx.dox
+-rw-r--r--   0 rieder     (501) staff       (20)     1979 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     4818 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4649 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm2map_cxx.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      903 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm2map_cxx.par.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     7220 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_fitsio.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     3763 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_fitsio.h
+-rw-r--r--   0 rieder     (501) staff       (20)    11358 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_healpix_tools.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     7249 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_healpix_tools.h
+-rw-r--r--   0 rieder     (501) staff       (20)    22943 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_map_tools.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     4067 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_map_tools.h
+-rw-r--r--   0 rieder     (501) staff       (20)    16281 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_powspec_tools.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     4773 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_powspec_tools.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4408 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/anafast_cxx.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      945 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/anafast_cxx.par.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     2409 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/calc_powspec.cc
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.981781 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/
+-rw-r--r--   0 rieder     (501) staff       (20)     1662 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)    14819 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/arr.h
+-rw-r--r--   0 rieder     (501) staff       (20)      170 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxsupport.dox
+-rw-r--r--   0 rieder     (501) staff       (20)     8750 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxutils.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     9531 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxutils.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7291 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/datatypes.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2937 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fftpack_support.h
+-rw-r--r--   0 rieder     (501) staff       (20)    26850 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fitshandle.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    16598 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fitshandle.h
+-rw-r--r--   0 rieder     (501) staff       (20)    61838 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/font_data.inc
+-rw-r--r--   0 rieder     (501) staff       (20)     2186 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/geom_utils.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3385 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/lsconstants.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2567 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/message_error.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2165 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/openmp_support.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3825 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/paramfile.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4246 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/planck_rng.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3366 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/pointing.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4910 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/rotmatrix.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     5621 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/rotmatrix.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2344 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/simparams.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     2574 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/simparams.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3680 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/tga_image.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     5824 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/tga_image.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5203 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/trafos.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     3619 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/trafos.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3964 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/vec3.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5681 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/xcomplex.h
+-rw-r--r--   0 rieder     (501) staff       (20)    21724 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    11109 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base.h
+-rw-r--r--   0 rieder     (501) staff       (20)    16091 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base2.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    10973 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base2.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3484 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_data_io.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     1817 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_data_io.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2885 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    10627 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4624 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map_fitsio.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     2833 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map_fitsio.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3134 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/hotspots_cxx.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    22202 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/hpxtest.cc
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.983259 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/
+-rw-r--r--   0 rieder     (501) staff       (20)      451 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     1758 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/README
+-rw-r--r--   0 rieder     (501) staff       (20)     4532 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/bluestein.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1297 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/bluestein.h
+-rw-r--r--   0 rieder     (501) staff       (20)    46443 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/fftpack.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1569 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/fftpack.h
+-rw-r--r--   0 rieder     (501) staff       (20)      102 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/libfftpack.dox
+-rw-r--r--   0 rieder     (501) staff       (20)     6098 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/ls_fft.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6068 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/ls_fft.h
+-rw-r--r--   0 rieder     (501) staff       (20)    11372 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/map2tga.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     2044 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/map2tga.par.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     2280 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/median_filter.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     4790 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/mult_alm.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      943 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/mult_alm.par.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     2803 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     4210 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4652 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec_fitsio.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     1801 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec_fitsio.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4201 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/rotalm_cxx.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     3717 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/smoothing_cxx.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      780 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/smoothing_cxx.par.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     3912 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/syn_alm_cxx.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      690 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/syn_alm_cxx.par.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     3103 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/udgrade_cxx.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     5687 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/ylmgen.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.984693 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/
+-rw-r--r--   0 rieder     (501) staff       (20)     4870 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/array_class.h
+-rw-r--r--   0 rieder     (501) staff       (20)    19775 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    19571 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w.h
+-rw-r--r--   0 rieder     (501) staff       (20)    19717 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_parallel.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    18351 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_parallel.h
+-rw-r--r--   0 rieder     (501) staff       (20)    21649 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_serial.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    19637 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_serial.h
+-rw-r--r--   0 rieder     (501) staff       (20)    10515 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/hdf5_routines.cpp
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.985083 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hilbert/
+-rw-r--r--   0 rieder     (501) staff       (20)    46290 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hilbert/hilbert.c
+-rw-r--r--   0 rieder     (501) staff       (20)     5769 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hilbert/hilbert.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.985455 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/keyValue/
+-rw-r--r--   0 rieder     (501) staff       (20)     4896 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/keyValue/configfile.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     7253 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/keyValue/configfile.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.987300 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/
+-rw-r--r--   0 rieder     (501) staff       (20)     2816 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/array.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2434 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/array2d.h
+-rw-r--r--   0 rieder     (501) staff       (20)      340 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/demo.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1043 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/numtraits.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4367 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/octree.h
+-rw-r--r--   0 rieder     (501) staff       (20)    24927 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/octree.tcc
+-rw-r--r--   0 rieder     (501) staff       (20)     4283 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/octree.vcproj
+-rw-r--r--   0 rieder     (501) staff       (20)     1309 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/point3d.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2268 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/shareddata.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5394 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/tinyvector.h
+-rw-r--r--   0 rieder     (501) staff       (20)     6424 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/tree_structures.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2346 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/tree_structures.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.989408 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/
+-rw-r--r--   0 rieder     (501) staff       (20)     2458 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/Announce.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    14404 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/CMakeLists.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     1635 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/COPYING.txt
+-rw-r--r--   0 rieder     (501) staff       (20)      421 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/File_id.diz
+-rw-r--r--   0 rieder     (501) staff       (20)    23167 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     1463 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/QHULL-GO.lnk
+-rw-r--r--   0 rieder     (501) staff       (20)    17514 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/README.txt
+-rw-r--r--   0 rieder     (501) staff       (20)      958 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/REGISTER.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.991203 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/
+-rw-r--r--   0 rieder     (501) staff       (20)      562 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-eg
+-rw-r--r--   0 rieder     (501) staff       (20)     1141 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-html
+-rw-r--r--   0 rieder     (501) staff       (20)     1986 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-libqhull
+-rw-r--r--   0 rieder     (501) staff       (20)      544 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-main
+-rw-r--r--   0 rieder     (501) staff       (20)      333 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile.am
+-rw-r--r--   0 rieder     (501) staff       (20)      883 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/README
+-rwxr-xr-x   0 rieder     (501) staff       (20)      869 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/bootstrap.sh
+-rw-r--r--   0 rieder     (501) staff       (20)     4835 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/changelog
+-rw-r--r--   0 rieder     (501) staff       (20)      464 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/configure.ac
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.991702 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/
+-rw-r--r--   0 rieder     (501) staff       (20)       37 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/00list
+-rwxr-xr-x   0 rieder     (501) staff       (20)      932 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/QHpointer.dpatch
+-rwxr-xr-x   0 rieder     (501) staff       (20)     1456 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/make-new-msg.dpatch
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.993629 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/
+-rwxr-xr-x   0 rieder     (501) staff       (20)      485 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/Qhull-go.bat
+-rwxr-xr-x   0 rieder     (501) staff       (20)     3179 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/make-vcproj.sh
+-rwxr-xr-x   0 rieder     (501) staff       (20)     3384 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_eg
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2106 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_egtest
+-rwxr-xr-x   0 rieder     (501) staff       (20)    12186 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test
+-rw-r--r--   0 rieder     (501) staff       (20)   405961 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test-ok.txt
+-rwxr-xr-x   0 rieder     (501) staff       (20)    30923 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test.bat
+-rwxr-xr-x   0 rieder     (501) staff       (20)     9647 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/qhull-zip.sh
+-rw-r--r--   0 rieder     (501) staff       (20)    36996 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/qhulltest-ok.txt
+-rw-r--r--   0 rieder     (501) staff       (20)    14000 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/index.htm
+-rw-r--r--   0 rieder     (501) staff       (20)    13134 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/qhull-2012.1-src-tgz.md5sum
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.995024 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/
+-rw-r--r--   0 rieder     (501) staff       (20)    82851 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/Changes.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.004652 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/
+-rw-r--r--   0 rieder     (501) staff       (20)     6701 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     6071 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/Mborland
+-rw-r--r--   0 rieder     (501) staff       (20)    42431 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7193 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom.h
+-rw-r--r--   0 rieder     (501) staff       (20)    65555 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom2.c
+-rw-r--r--   0 rieder     (501) staff       (20)    70589 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/global.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10771 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/index.htm
+-rw-r--r--   0 rieder     (501) staff       (20)   133486 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/io.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7926 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/io.h
+-rw-r--r--   0 rieder     (501) staff       (20)    51817 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.c
+-rw-r--r--   0 rieder     (501) staff       (20)    50146 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1515 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.pro
+-rw-r--r--   0 rieder     (501) staff       (20)    19024 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/mem.c
+-rw-r--r--   0 rieder     (501) staff       (20)     8537 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/mem.h
+-rw-r--r--   0 rieder     (501) staff       (20)   121690 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/merge.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7301 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/merge.h
+-rw-r--r--   0 rieder     (501) staff       (20)    39828 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10935 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly.h
+-rw-r--r--   0 rieder     (501) staff       (20)   110261 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly2.c
+-rw-r--r--   0 rieder     (501) staff       (20)    13066 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-geom.htm
+-rw-r--r--   0 rieder     (501) staff       (20)     7348 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-globa.htm
+-rw-r--r--   0 rieder     (501) staff       (20)    14430 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-io.htm
+-rw-r--r--   0 rieder     (501) staff       (20)     6145 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-mem.htm
+-rw-r--r--   0 rieder     (501) staff       (20)    15144 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-merge.htm
+-rw-r--r--   0 rieder     (501) staff       (20)    20940 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-poly.htm
+-rw-r--r--   0 rieder     (501) staff       (20)    12695 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-qhull.htm
+-rw-r--r--   0 rieder     (501) staff       (20)    13092 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-set.htm
+-rw-r--r--   0 rieder     (501) staff       (20)     7078 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-stat.htm
+-rw-r--r--   0 rieder     (501) staff       (20)    11351 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-user.htm
+-rw-r--r--   0 rieder     (501) staff       (20)     7543 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qhull-exports.def
+-rw-r--r--   0 rieder     (501) staff       (20)     4926 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qhull_a.h
+-rw-r--r--   0 rieder     (501) staff       (20)    33590 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qset.c
+-rw-r--r--   0 rieder     (501) staff       (20)    14830 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qset.h
+-rw-r--r--   0 rieder     (501) staff       (20)     6357 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/random.c
+-rw-r--r--   0 rieder     (501) staff       (20)      935 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/random.h
+-rw-r--r--   0 rieder     (501) staff       (20)    22239 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/rboxlib.c
+-rw-r--r--   0 rieder     (501) staff       (20)    30502 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/stat.c
+-rw-r--r--   0 rieder     (501) staff       (20)    12877 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/stat.h
+-rw-r--r--   0 rieder     (501) staff       (20)    19708 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/user.c
+-rw-r--r--   0 rieder     (501) staff       (20)    28181 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/user.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1495 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/usermem.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1790 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/userprintf.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1620 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/userprintf_rbox.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.013544 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/
+-rw-r--r--   0 rieder     (501) staff       (20)     3769 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Coordinates.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    15543 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Coordinates.h
+-rw-r--r--   0 rieder     (501) staff       (20)     8182 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/PointCoordinates.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     6806 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/PointCoordinates.h
+-rw-r--r--   0 rieder     (501) staff       (20)    15907 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Qhull.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     6391 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Qhull.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2361 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullError.h
+-rw-r--r--   0 rieder     (501) staff       (20)    15691 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacet.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     6857 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacet.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4285 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetList.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4082 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetList.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3639 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetSet.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3614 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetSet.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4357 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullHyperplane.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     6025 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullHyperplane.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7882 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullIterator.h
+-rw-r--r--   0 rieder     (501) staff       (20)    11956 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullLinkedList.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4945 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoint.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     6159 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoint.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4691 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPointSet.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    12576 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPointSet.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5026 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoints.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    16146 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoints.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3376 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullQh.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1314 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullQh.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2979 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullRidge.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4117 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullRidge.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1255 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSet.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    11623 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSet.h
+-rw-r--r--   0 rieder     (501) staff       (20)      783 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSets.h
+-rw-r--r--   0 rieder     (501) staff       (20)      881 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullStat.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1308 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullStat.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2773 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertex.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3862 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertex.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3310 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertexSet.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3269 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertexSet.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5787 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RboxPoints.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2109 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RboxPoints.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3350 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadError.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3135 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadError.h
+-rw-r--r--   0 rieder     (501) staff       (20)     3133 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadLogEvent.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3536 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadLogEvent.h
+-rw-r--r--   0 rieder     (501) staff       (20)    11749 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/UsingLibQhull.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     6172 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/UsingLibQhull.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1516 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/functionObjects.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1778 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/libqhullcpp.pro
+-rw-r--r--   0 rieder     (501) staff       (20)     3565 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/qhull_interface.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2700 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/qt-qhull.cpp
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.013870 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/
+-rw-r--r--   0 rieder     (501) staff       (20)      709 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/libqhullp.pro
+-rw-r--r--   0 rieder     (501) staff       (20)     7488 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/qhull_p-exports.def
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.014032 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstatic/
+-rw-r--r--   0 rieder     (501) staff       (20)      550 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstatic/libqhullstatic.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.014183 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstaticp/
+-rw-r--r--   0 rieder     (501) staff       (20)      551 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstaticp/libqhullstaticp.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.014802 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qconvex/
+-rw-r--r--   0 rieder     (501) staff       (20)    12363 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qconvex/qconvex.c
+-rw-r--r--   0 rieder     (501) staff       (20)      222 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qconvex/qconvex.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.015196 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qdelaunay/
+-rw-r--r--   0 rieder     (501) staff       (20)    12032 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qdelaunay/qdelaun.c
+-rw-r--r--   0 rieder     (501) staff       (20)      227 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qdelaunay/qdelaunay.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.015604 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhalf/
+-rw-r--r--   0 rieder     (501) staff       (20)    12005 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhalf/qhalf.c
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhalf/qhalf.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.015893 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull/
+-rw-r--r--   0 rieder     (501) staff       (20)      213 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull/qhull.pro
+-rw-r--r--   0 rieder     (501) staff       (20)    15724 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull/unix.c
+-rw-r--r--   0 rieder     (501) staff       (20)     2803 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-all.pro
+-rw-r--r--   0 rieder     (501) staff       (20)      608 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-c.pri
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-cpp.pri
+-rw-r--r--   0 rieder     (501) staff       (20)      678 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-shared.pri
+-rw-r--r--   0 rieder     (501) staff       (20)      759 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-sharedp.pri
+-rw-r--r--   0 rieder     (501) staff       (20)     1253 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-libqhull-src.pri
+-rw-r--r--   0 rieder     (501) staff       (20)     3164 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-warn.pri
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.021010 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/
+-rw-r--r--   0 rieder     (501) staff       (20)    13536 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Coordinates_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    11090 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/PointCoordinates_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     5742 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Point_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4869 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacetList_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4010 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacetSet_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     8632 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacet_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    11248 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullHyperplane_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     8965 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullLinkedList_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    10055 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPointSet_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    10363 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPoint_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    13003 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPoints_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4456 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullRidge_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    12138 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullSet_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     4777 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullVertexSet_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     5314 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullVertex_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    11775 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Qhull_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     6052 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RboxPoints_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1852 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RoadTest.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2084 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RoadTest.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7814 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/UsingLibQhull_test.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2510 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/qhulltest.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      946 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/qhulltest.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.021384 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qvoronoi/
+-rw-r--r--   0 rieder     (501) staff       (20)    11433 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qvoronoi/qvoronoi.c
+-rw-r--r--   0 rieder     (501) staff       (20)      226 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qvoronoi/qvoronoi.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.021682 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/rbox/
+-rw-r--r--   0 rieder     (501) staff       (20)     3547 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/rbox/rbox.c
+-rw-r--r--   0 rieder     (501) staff       (20)      205 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/rbox/rbox.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.021995 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/
+-rw-r--r--   0 rieder     (501) staff       (20)    32472 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/testqset.c
+-rw-r--r--   0 rieder     (501) staff       (20)      621 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/testqset.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.022334 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg/
+-rw-r--r--   0 rieder     (501) staff       (20)    11089 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg/user_eg.c
+-rw-r--r--   0 rieder     (501) staff       (20)      231 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg/user_eg.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.022629 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg2/
+-rw-r--r--   0 rieder     (501) staff       (20)    26662 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg2/user_eg2.c
+-rw-r--r--   0 rieder     (501) staff       (20)      256 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg2/user_eg2.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.022919 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg3/
+-rw-r--r--   0 rieder     (501) staff       (20)     4564 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg3/user_eg3.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      256 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg3/user_eg3.pro
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:49.955518 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.028947 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/
+-rw-r--r--   0 rieder     (501) staff       (20)   753132 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map16.h
+-rw-r--r--   0 rieder     (501) staff       (20)   993818 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map21.h
+-rw-r--r--   0 rieder     (501) staff       (20)  1523503 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map32.h
+-rw-r--r--   0 rieder     (501) staff       (20)  2004913 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map42.h
+-rw-r--r--   0 rieder     (501) staff       (20)  3064038 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map64.h
+-rw-r--r--   0 rieder     (501) staff       (20)  4027038 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map84.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.033374 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/
+-rw-r--r--   0 rieder     (501) staff       (20)    12117 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Common.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     5730 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Common.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5224 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Main.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)      732 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Main.h
+-rw-r--r--   0 rieder     (501) staff       (20)   289150 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/SimpleX.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    21034 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/SimpleX.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7124 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Structs.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)    21893 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Structs.h
+-rw-r--r--   0 rieder     (501) staff       (20)    35337 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/amuse_interface.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3234 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/amuse_interface.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4502 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/rates.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     3026 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/rates.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:50.034680 amuse-simplex-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-simplex-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-simplex-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-simplex-2024.4.0/support/version.py
```

### Comparing `amuse-simplex-2023.5.0/PKG-INFO` & `amuse-simplex-2024.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-simplex
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Simplex
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,13 @@
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
+Requires-Dist: mpi4py>=1.1.0
+Requires-Dist: amuse-framework
 
 This package installs the Simplex community code for AMUSE.
```

### Comparing `amuse-simplex-2023.5.0/amuse_simplex.egg-info/PKG-INFO` & `amuse-simplex-2024.4.0/amuse_simplex.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-simplex
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Simplex
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,13 @@
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
+Requires-Dist: mpi4py>=1.1.0
+Requires-Dist: amuse-framework
 
 This package installs the Simplex community code for AMUSE.
```

### Comparing `amuse-simplex-2023.5.0/amuse_simplex.egg-info/SOURCES.txt` & `amuse-simplex-2024.4.0/amuse_simplex.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 amuse_simplex.egg-info/PKG-INFO
 amuse_simplex.egg-info/SOURCES.txt
 amuse_simplex.egg-info/dependency_links.txt
 amuse_simplex.egg-info/requires.txt
 amuse_simplex.egg-info/top_level.txt
 src/amuse/community/simplex/Makefile
 src/amuse/community/simplex/__init__.py
+src/amuse/community/simplex/_version.py
 src/amuse/community/simplex/interface.py
-src/amuse/community/simplex/version.py
 src/amuse/community/simplex/data/input/C.Hcool
 src/amuse/community/simplex/data/input/C.cool
 src/amuse/community/simplex/data/input/Fe.Hcool
 src/amuse/community/simplex/data/input/Fe.cool
 src/amuse/community/simplex/data/input/H.Hcool
 src/amuse/community/simplex/data/input/H.cool
 src/amuse/community/simplex/data/input/H2.Hcool
```

### Comparing `amuse-simplex-2023.5.0/setup.py` & `amuse-simplex-2024.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,42 +30,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.simplex.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/simplex/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/simplex/_version.py",
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
         'amuse.community.simplex': 'src/amuse/community/simplex',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/Makefile` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/C.Hcool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/C.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/C.cool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/C.cool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Fe.Hcool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Fe.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Fe.cool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Fe.cool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/H.cool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/H.cool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/H2.Hcool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/H2.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/He.cool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/He.cool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/N.cool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/N.cool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Ne.cool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Ne.cool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/O.Hcool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/O.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/O.cool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/O.cool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Si.Hcool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Si.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/Si.cool` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/Si.cool`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/vertices_10.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/vertices_10.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/vertices_test.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/vertices_test.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/vertices_test2.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/vertices_test2.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/data/input/vertices_test3.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/data/input/vertices_test3.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/interface.py` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/Makefile` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_fitsio.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_fitsio.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_healpix_tools.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_healpix_tools.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_map_tools.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_map_tools.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_powspec_tools.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/alm_powspec_tools.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/arr.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/arr.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/cxxutils.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/cxxutils.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/datatypes.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/datatypes.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fftpack_support.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fftpack_support.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fitshandle.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fitshandle.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fitsio.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/fitsio.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/geom_utils.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/geom_utils.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_base.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_base.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_base2.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_base2.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_data_io.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_data_io.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_map.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_map.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_map_fitsio.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/healpix_map_fitsio.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/longnam.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/longnam.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/ls_fft.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/ls_fft.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/lsconstants.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/lsconstants.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/message_error.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/message_error.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/openmp_support.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/openmp_support.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/paramfile.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/paramfile.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/planck_rng.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/planck_rng.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/pointing.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/pointing.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/powspec.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/powspec.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/powspec_fitsio.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/powspec_fitsio.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/rotmatrix.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/rotmatrix.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/simparams.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/simparams.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/tga_image.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/tga_image.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/trafos.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/trafos.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/vec3.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/vec3.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/xcomplex.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/xcomplex.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/include/ylmgen.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/include/ylmgen.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/Healpix_cxx.dox` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/Healpix_cxx.dox`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/Makefile` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm2map_cxx.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm2map_cxx.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm2map_cxx.par.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm2map_cxx.par.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_fitsio.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_fitsio.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_fitsio.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_fitsio.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_healpix_tools.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_healpix_tools.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_healpix_tools.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_healpix_tools.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_map_tools.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_map_tools.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_map_tools.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_map_tools.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_powspec_tools.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_powspec_tools.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_powspec_tools.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/alm_powspec_tools.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/anafast_cxx.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/anafast_cxx.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/anafast_cxx.par.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/anafast_cxx.par.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/calc_powspec.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/calc_powspec.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/Makefile` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/arr.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/arr.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxutils.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxutils.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxutils.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/cxxutils.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/datatypes.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/datatypes.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fftpack_support.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fftpack_support.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fitshandle.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fitshandle.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fitshandle.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/fitshandle.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/font_data.inc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/font_data.inc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/geom_utils.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/geom_utils.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/lsconstants.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/lsconstants.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/message_error.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/message_error.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/openmp_support.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/openmp_support.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/paramfile.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/paramfile.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/planck_rng.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/planck_rng.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/pointing.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/pointing.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/rotmatrix.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/rotmatrix.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/rotmatrix.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/rotmatrix.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/simparams.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/simparams.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/simparams.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/simparams.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/tga_image.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/tga_image.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/tga_image.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/tga_image.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/trafos.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/trafos.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/trafos.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/trafos.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/vec3.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/vec3.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/xcomplex.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/cxxsupport/xcomplex.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base2.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base2.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base2.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_base2.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_data_io.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_data_io.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_data_io.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_data_io.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map_fitsio.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map_fitsio.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map_fitsio.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/healpix_map_fitsio.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/hotspots_cxx.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/hotspots_cxx.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/hpxtest.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/hpxtest.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/README` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/README`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/bluestein.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/bluestein.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/bluestein.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/bluestein.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/fftpack.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/fftpack.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/fftpack.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/fftpack.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/ls_fft.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/ls_fft.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/ls_fft.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/libfftpack/ls_fft.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/map2tga.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/map2tga.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/map2tga.par.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/map2tga.par.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/median_filter.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/median_filter.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/mult_alm.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/mult_alm.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/mult_alm.par.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/mult_alm.par.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec_fitsio.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec_fitsio.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec_fitsio.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/powspec_fitsio.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/rotalm_cxx.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/rotalm_cxx.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/smoothing_cxx.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/smoothing_cxx.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/smoothing_cxx.par.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/smoothing_cxx.par.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/syn_alm_cxx.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/syn_alm_cxx.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/syn_alm_cxx.par.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/syn_alm_cxx.par.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/udgrade_cxx.cc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/udgrade_cxx.cc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/HEALPix/src/ylmgen.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/HEALPix/src/ylmgen.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/array_class.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/array_class.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_parallel.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_parallel.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_parallel.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_parallel.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_serial.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_serial.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_serial.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/h5w_serial.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hdf5/hdf5_routines.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hdf5/hdf5_routines.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hilbert/hilbert.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hilbert/hilbert.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/hilbert/hilbert.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/hilbert/hilbert.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/keyValue/configfile.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/keyValue/configfile.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/keyValue/configfile.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/keyValue/configfile.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/array.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/array.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/array2d.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/array2d.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/numtraits.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/numtraits.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/octree.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/octree.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/octree.tcc` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/octree.tcc`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/octree.vcproj` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/octree.vcproj`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/point3d.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/point3d.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/shareddata.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/shareddata.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/tinyvector.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/tinyvector.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/tree_structures.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/tree_structures.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/octree/tree_structures.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/octree/tree_structures.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/Announce.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/Announce.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/CMakeLists.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/COPYING.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/Makefile` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/QHULL-GO.lnk` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/QHULL-GO.lnk`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/README.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/README.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/REGISTER.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/REGISTER.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-eg` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-eg`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-html` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-html`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-libqhull` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-libqhull`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-main` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/Makefile-am-main`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/README` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/README`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/bootstrap.sh` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/changelog` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/changelog`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/QHpointer.dpatch` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/QHpointer.dpatch`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/make-new-msg.dpatch` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/config/patches/make-new-msg.dpatch`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/make-vcproj.sh` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/make-vcproj.sh`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_eg` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_eg`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_egtest` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_egtest`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test-ok.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test-ok.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test.bat` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/q_test.bat`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/qhull-zip.sh` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/qhull-zip.sh`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/qhulltest-ok.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/eg/qhulltest-ok.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/index.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/index.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/qhull-2012.1-src-tgz.md5sum` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/qhull-2012.1-src-tgz.md5sum`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/Changes.txt` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/Changes.txt`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/Makefile` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/Mborland` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/Mborland`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom2.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/geom2.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/global.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/global.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/index.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/index.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/io.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/io.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/io.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/io.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.pro` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/libqhull.pro`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/mem.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/mem.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/mem.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/mem.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/merge.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/merge.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/merge.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/merge.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly2.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/poly2.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-geom.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-geom.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-globa.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-globa.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-io.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-io.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-mem.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-mem.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-merge.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-merge.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-poly.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-poly.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-qhull.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-qhull.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-set.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-set.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-stat.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-stat.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-user.htm` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qh-user.htm`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qhull-exports.def` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qhull-exports.def`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qhull_a.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qhull_a.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qset.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qset.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qset.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/qset.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/random.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/random.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/random.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/random.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/rboxlib.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/rboxlib.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/stat.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/stat.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/stat.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/stat.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/user.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/user.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/user.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/user.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/usermem.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/usermem.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/userprintf.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/userprintf.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/userprintf_rbox.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhull/userprintf_rbox.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Coordinates.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Coordinates.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Coordinates.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Coordinates.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/PointCoordinates.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/PointCoordinates.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/PointCoordinates.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/PointCoordinates.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Qhull.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Qhull.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Qhull.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/Qhull.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullError.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullError.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacet.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacet.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacet.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacet.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetList.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetList.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetList.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetList.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetSet.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetSet.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetSet.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullFacetSet.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullHyperplane.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullHyperplane.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullHyperplane.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullHyperplane.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullIterator.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullIterator.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullLinkedList.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullLinkedList.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoint.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoint.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoint.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoint.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPointSet.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPointSet.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPointSet.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPointSet.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoints.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoints.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoints.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullPoints.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullQh.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullQh.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullQh.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullQh.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullRidge.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullRidge.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullRidge.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullRidge.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSet.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSet.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSet.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSet.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSets.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullSets.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullStat.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullStat.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullStat.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullStat.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertex.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertex.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertex.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertex.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertexSet.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertexSet.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertexSet.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/QhullVertexSet.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RboxPoints.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RboxPoints.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RboxPoints.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RboxPoints.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadError.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadError.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadError.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadError.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadLogEvent.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadLogEvent.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadLogEvent.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/RoadLogEvent.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/UsingLibQhull.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/UsingLibQhull.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/UsingLibQhull.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/UsingLibQhull.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/functionObjects.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/functionObjects.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/libqhullcpp.pro` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/libqhullcpp.pro`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/qhull_interface.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/qhull_interface.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/qt-qhull.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullcpp/qt-qhull.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/libqhullp.pro` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/libqhullp.pro`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/qhull_p-exports.def` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullp/qhull_p-exports.def`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstatic/libqhullstatic.pro` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstatic/libqhullstatic.pro`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstaticp/libqhullstaticp.pro` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/libqhullstaticp/libqhullstaticp.pro`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qconvex/qconvex.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qconvex/qconvex.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qdelaunay/qdelaun.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qdelaunay/qdelaun.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhalf/qhalf.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhalf/qhalf.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull/unix.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull/unix.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-all.pro` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-all.pro`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-c.pri` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-c.pri`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-cpp.pri` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-cpp.pri`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-shared.pri` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-shared.pri`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-sharedp.pri` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-app-sharedp.pri`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-libqhull-src.pri` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-libqhull-src.pri`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-warn.pri` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhull-warn.pri`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Coordinates_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Coordinates_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/PointCoordinates_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/PointCoordinates_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Point_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Point_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacetList_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacetList_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacetSet_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacetSet_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacet_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullFacet_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullHyperplane_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullHyperplane_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullLinkedList_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullLinkedList_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPointSet_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPointSet_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPoint_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPoint_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPoints_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullPoints_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullRidge_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullRidge_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullSet_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullSet_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullVertexSet_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullVertexSet_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullVertex_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/QhullVertex_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Qhull_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/Qhull_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RboxPoints_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RboxPoints_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RoadTest.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RoadTest.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RoadTest.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/RoadTest.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/UsingLibQhull_test.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/UsingLibQhull_test.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/qhulltest.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/qhulltest.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/qhulltest.pro` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qhulltest/qhulltest.pro`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qvoronoi/qvoronoi.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/qvoronoi/qvoronoi.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/rbox/rbox.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/rbox/rbox.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/testqset.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/testqset.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/testqset.pro` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/testqset/testqset.pro`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg/user_eg.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg/user_eg.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg2/user_eg2.c` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg2/user_eg2.c`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg3/user_eg3.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/qhull-2012.1/src/user_eg3/user_eg3.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map16.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map16.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map21.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map21.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map32.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map32.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map42.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map42.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map64.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map64.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map84.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/plugins/unit_sphere_tess/include/Map84.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Common.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Common.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Common.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Common.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Main.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Main.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Main.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Main.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/SimpleX.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/SimpleX.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/SimpleX.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/SimpleX.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Structs.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Structs.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/Structs.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/Structs.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/amuse_interface.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/amuse_interface.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/amuse_interface.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/amuse_interface.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/rates.cpp` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/rates.cpp`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/src/amuse/community/simplex/src/src/rates.h` & `amuse-simplex-2024.4.0/src/amuse/community/simplex/src/src/rates.h`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/support/__init__.py` & `amuse-simplex-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/support/classifiers.py` & `amuse-simplex-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/support/config.py` & `amuse-simplex-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/support/generate_main.py` & `amuse-simplex-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/support/getsp.class` & `amuse-simplex-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/support/getsp.java` & `amuse-simplex-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/support/misc.py` & `amuse-simplex-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-simplex-2023.5.0/support/setup_codes.py` & `amuse-simplex-2024.4.0/support/setup_codes.py`

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

