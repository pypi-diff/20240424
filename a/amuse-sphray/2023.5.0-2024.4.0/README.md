# Comparing `tmp/amuse-sphray-2023.5.0.tar.gz` & `tmp/amuse-sphray-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-sphray-2023.5.0.tar", last modified: Wed May 17 10:19:47 2023, max compression
+gzip compressed data, was "amuse-sphray-2024.4.0.tar", last modified: Wed Apr 24 16:32:57 2024, max compression
```

## Comparing `amuse-sphray-2023.5.0.tar` & `amuse-sphray-2024.4.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.837463 amuse-sphray-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-sphray-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:19:47.837281 amuse-sphray-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       59 2022-11-22 11:55:14.000000 amuse-sphray-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.803613 amuse-sphray-2023.5.0/amuse_sphray.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1186 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     6112 2023-05-17 10:19:47.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/amuse_sphray.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-sphray-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:47.837504 amuse-sphray-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1777 2022-11-22 11:55:14.000000 amuse-sphray-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.801528 amuse-sphray-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.801584 amuse-sphray-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.801639 amuse-sphray-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.805018 amuse-sphray-2023.5.0/src/amuse/community/sphray/
--rw-r--r--   0 rieder     (501) staff       (20)     1393 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.801780 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.806650 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.813588 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/
--rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt
--rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt
--rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt
--rw-r--r--   0 rieder     (501) staff       (20)   785996 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt
--rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Vor.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.815310 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/
--rw-r--r--   0 rieder     (501) staff       (20)     1288 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/latmon_b2cd_table.txt
--rw-r--r--   0 rieder     (501) staff       (20)     1288 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/tophat_b2cd_table.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.816807 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/
--rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/power2.0.cdf
--rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/power4.0.cdf
--rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/thermal1e5.cdf
--rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/thermal6e4.cdf
--rw-r--r--   0 rieder     (501) staff       (20)   370256 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/sphray_4K
--rw-r--r--   0 rieder     (501) staff       (20)       70 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/test1_sources_001.1
--rw-r--r--   0 rieder     (501) staff       (20)       69 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/test2_sources_001.1
--rw-r--r--   0 rieder     (501) staff       (20)     9907 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/interface.f90
--rw-r--r--   0 rieder     (501) staff       (20)    35232 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/interface.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.829368 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/
--rw-r--r--   0 rieder     (501) staff       (20)     9708 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     8945 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/MakefileTemplate
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.832409 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/
--rw-r--r--   0 rieder     (501) staff       (20)    71467 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GL.h
--rw-r--r--   0 rieder     (501) staff       (20)    16543 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLU.h
--rw-r--r--   0 rieder     (501) staff       (20)    19786 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLUT.h
--rw-r--r--   0 rieder     (501) staff       (20)      536 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLUT_fonts.c
--rw-r--r--   0 rieder     (501) staff       (20)    68448 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_freeglut.F90
--rw-r--r--   0 rieder     (501) staff       (20)   194062 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_gl.F90
--rw-r--r--   0 rieder     (501) staff       (20)    41410 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glu.F90
--rw-r--r--   0 rieder     (501) staff       (20)    56657 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glut.F90
--rw-r--r--   0 rieder     (501) staff       (20)    67729 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_openglut.F90
--rw-r--r--   0 rieder     (501) staff       (20)     1091 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/fthread.f
--rw-r--r--   0 rieder     (501) staff       (20)     6077 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/pt.c
--rw-r--r--   0 rieder     (501) staff       (20)     6831 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/pt.h
--rw-r--r--   0 rieder     (501) staff       (20)     1018 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/ptf77.c
--rw-r--r--   0 rieder     (501) staff       (20)    33052 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/amuse_helpers.F90
--rw-r--r--   0 rieder     (501) staff       (20)     5354 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/amuse_mainloop.F90
--rw-r--r--   0 rieder     (501) staff       (20)    25577 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)     3995 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/b2cd.F90
--rw-r--r--   0 rieder     (501) staff       (20)     8804 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/bdf.F90
--rw-r--r--   0 rieder     (501) staff       (20)    14046 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/cen_atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)    23703 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/config.F90
--rw-r--r--   0 rieder     (501) staff       (20)     2264 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/cosmology.F90
--rw-r--r--   0 rieder     (501) staff       (20)     7761 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/density_test.F90
--rw-r--r--   0 rieder     (501) staff       (20)    12191 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/euler.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13277 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_cosmoBH_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)    23569 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_general_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)     7836 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_owls_header_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)    16188 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_owls_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)     8724 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_header_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)     4112 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_header_hdf5_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13904 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13217 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_input_hdf5.F90
--rw-r--r--   0 rieder     (501) staff       (20)     7917 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_sphray_header_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)    14316 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_vbromm_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13702 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/global.F90
--rw-r--r--   0 rieder     (501) staff       (20)     2692 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/glsphray.F90
--rw-r--r--   0 rieder     (501) staff       (20)     1563 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hash.f90
--rw-r--r--   0 rieder     (501) staff       (20)     5118 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hdf5_io.F90
--rw-r--r--   0 rieder     (501) staff       (20)     4987 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/healpix_types.F90
--rw-r--r--   0 rieder     (501) staff       (20)    11601 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hui_gnedin_atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)     7028 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hummer_atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)    10043 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/iliev_comparison_project.F90
--rw-r--r--   0 rieder     (501) staff       (20)    14251 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/initialize.F90
--rw-r--r--   0 rieder     (501) staff       (20)    24603 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ion_table_class.F90
--rw-r--r--   0 rieder     (501) staff       (20)    10089 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ion_temperature_update.F90
--rw-r--r--   0 rieder     (501) staff       (20)    34740 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ionpar.F90
--rw-r--r--   0 rieder     (501) staff       (20)    12266 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/kerneldensity.F90
--rw-r--r--   0 rieder     (501) staff       (20)    17376 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/m_mrgrnk.F90
--rw-r--r--   0 rieder     (501) staff       (20)    13147 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/main_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)     6644 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/mainloop.F90
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.835771 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/
--rw-r--r--   0 rieder     (501) staff       (20)      167 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.gfortran.debug
--rw-r--r--   0 rieder     (501) staff       (20)      137 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.gfortran.opt
--rw-r--r--   0 rieder     (501) staff       (20)      201 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.intel.debug
--rw-r--r--   0 rieder     (501) staff       (20)      435 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.intel.opt
--rw-r--r--   0 rieder     (501) staff       (20)      136 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      206 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.cosma.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      195 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.cosma.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      369 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.ferrari.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      102 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.icc-graphics.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.icc-graphics.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      176 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.santabuntu.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      372 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.santabuntu.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      128 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.titania.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      177 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.titania.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)      175 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.warp.opt
--rw-r--r--   0 rieder     (501) staff       (20)      180 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.warp.opt.bck
--rw-r--r--   0 rieder     (501) staff       (20)      221 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.warp.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      194 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.xgpc.serial.debug
--rw-r--r--   0 rieder     (501) staff       (20)      447 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/makes/make.xgpc.serial.opt
--rw-r--r--   0 rieder     (501) staff       (20)    11160 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/mt19937.F90
--rw-r--r--   0 rieder     (501) staff       (20)    16660 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/myf03.f90
--rw-r--r--   0 rieder     (501) staff       (20)     6520 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/nblist.F90
--rw-r--r--   0 rieder     (501) staff       (20)    18132 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/octtree3.F90
--rw-r--r--   0 rieder     (501) staff       (20)    17069 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/octtree3p.F90
--rw-r--r--   0 rieder     (501) staff       (20)    23138 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/output.F90
--rw-r--r--   0 rieder     (501) staff       (20)    25364 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/particle_system.F90
--rw-r--r--   0 rieder     (501) staff       (20)     5612 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/physical_constants.F90
--rw-r--r--   0 rieder     (501) staff       (20)     9944 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/pix_tools.F90
--rw-r--r--   0 rieder     (501) staff       (20)    15588 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ray.F90
--rw-r--r--   0 rieder     (501) staff       (20)    12331 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/raylist.F90
--rw-r--r--   0 rieder     (501) staff       (20)    68389 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sobol.F90
--rw-r--r--   0 rieder     (501) staff       (20)    11314 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/source_input.F90
--rw-r--r--   0 rieder     (501) staff       (20)     3072 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/spectra.F90
--rw-r--r--   0 rieder     (501) staff       (20)     2903 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sphpar.F90
--rw-r--r--   0 rieder     (501) staff       (20)     3125 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sphray.F90
--rw-r--r--   0 rieder     (501) staff       (20)     5124 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/update_particles.F90
--rw-r--r--   0 rieder     (501) staff       (20)    27441 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/viewer.F90
--rw-r--r--   0 rieder     (501) staff       (20)    23330 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/src/voronov_atomic_rates.F90
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:45.000000 amuse-sphray-2023.5.0/src/amuse/community/sphray/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:47.837057 amuse-sphray-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-sphray-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-sphray-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-sphray-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.683988 amuse-sphray-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-sphray-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1217 2024-04-24 16:32:57.683770 amuse-sphray-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       59 2022-11-22 11:55:14.000000 amuse-sphray-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.683461 amuse-sphray-2024.4.0/amuse_sphray.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1217 2024-04-24 16:32:56.000000 amuse-sphray-2024.4.0/amuse_sphray.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     6113 2024-04-24 16:32:57.000000 amuse-sphray-2024.4.0/amuse_sphray.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:56.000000 amuse-sphray-2024.4.0/amuse_sphray.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:56.000000 amuse-sphray-2024.4.0/amuse_sphray.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:56.000000 amuse-sphray-2024.4.0/amuse_sphray.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-sphray-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:57.684053 amuse-sphray-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1581 2024-04-24 15:35:29.000000 amuse-sphray-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.659827 amuse-sphray-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.659878 amuse-sphray-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.659928 amuse-sphray-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.662635 amuse-sphray-2024.4.0/src/amuse/community/sphray/
+-rw-r--r--   0 rieder     (501) staff       (20)     1393 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       30 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:56.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/_version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.660046 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.663810 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.666541 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/
+-rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt
+-rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt
+-rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt
+-rw-r--r--   0 rieder     (501) staff       (20)   785996 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt
+-rw-r--r--   0 rieder     (501) staff       (20)   786348 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Vor.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.667253 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/column_depth/
+-rw-r--r--   0 rieder     (501) staff       (20)     1288 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/column_depth/latmon_b2cd_table.txt
+-rw-r--r--   0 rieder     (501) staff       (20)     1288 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/column_depth/tophat_b2cd_table.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.668032 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/
+-rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/power2.0.cdf
+-rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/power4.0.cdf
+-rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/thermal1e5.cdf
+-rw-r--r--   0 rieder     (501) staff       (20)    49123 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/thermal6e4.cdf
+-rw-r--r--   0 rieder     (501) staff       (20)   370256 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/sphray_4K
+-rw-r--r--   0 rieder     (501) staff       (20)       70 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/test1_sources_001.1
+-rw-r--r--   0 rieder     (501) staff       (20)       69 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/test2_sources_001.1
+-rw-r--r--   0 rieder     (501) staff       (20)     9907 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/interface.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    35232 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.677186 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     9708 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     8945 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/MakefileTemplate
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.679367 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/
+-rw-r--r--   0 rieder     (501) staff       (20)    71467 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/GL.h
+-rw-r--r--   0 rieder     (501) staff       (20)    16543 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/GLU.h
+-rw-r--r--   0 rieder     (501) staff       (20)    19786 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/GLUT.h
+-rw-r--r--   0 rieder     (501) staff       (20)      536 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/GLUT_fonts.c
+-rw-r--r--   0 rieder     (501) staff       (20)    68448 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_freeglut.F90
+-rw-r--r--   0 rieder     (501) staff       (20)   194062 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_gl.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    41410 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glu.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    56657 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glut.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    67729 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_openglut.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     1091 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/fthread.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6077 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/pt.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6831 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/pt.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1018 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/ptf77.c
+-rw-r--r--   0 rieder     (501) staff       (20)    33052 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/amuse_helpers.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     5354 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/amuse_mainloop.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    25577 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     3995 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/b2cd.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     8804 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/bdf.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    14046 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/cen_atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    23703 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/config.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     2264 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/cosmology.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     7761 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/density_test.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    12191 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/euler.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13277 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_cosmoBH_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    23569 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_general_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     7836 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_owls_header_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    16188 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_owls_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     8724 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_public_header_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     4112 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_public_header_hdf5_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13904 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_public_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13217 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_public_input_hdf5.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     7917 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_sphray_header_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    14316 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_vbromm_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13702 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/global.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     2692 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/glsphray.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     1563 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/hash.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     5118 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/hdf5_io.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     4987 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/healpix_types.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    11601 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/hui_gnedin_atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     7028 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/hummer_atomic_rates.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    10043 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/iliev_comparison_project.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    14251 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/initialize.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    24603 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/ion_table_class.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    10089 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/ion_temperature_update.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    34740 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/ionpar.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    12266 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/kerneldensity.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    17376 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/m_mrgrnk.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    13147 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/main_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     6644 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/mainloop.F90
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.682042 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/
+-rw-r--r--   0 rieder     (501) staff       (20)      167 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.gfortran.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      137 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.gfortran.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      201 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.intel.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      435 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.intel.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      136 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.blue-velvet.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      206 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.cosma.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      195 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.cosma.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      369 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.ferrari.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      102 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.icc-graphics.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.icc-graphics.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      176 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.santabuntu.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      372 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.santabuntu.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      128 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.titania.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      177 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.titania.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      175 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.warp.opt
+-rw-r--r--   0 rieder     (501) staff       (20)      180 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.warp.opt.bck
+-rw-r--r--   0 rieder     (501) staff       (20)      221 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.warp.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      194 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.xgpc.serial.debug
+-rw-r--r--   0 rieder     (501) staff       (20)      447 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/makes/make.xgpc.serial.opt
+-rw-r--r--   0 rieder     (501) staff       (20)    11160 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/mt19937.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    16660 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/myf03.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     6520 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/nblist.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    18132 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/octtree3.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    17069 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/octtree3p.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    23138 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/output.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    25364 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/particle_system.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     5612 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/physical_constants.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     9944 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/pix_tools.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    15588 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/ray.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    12331 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/raylist.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    68389 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/sobol.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    11314 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/source_input.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     3072 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/spectra.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     2903 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/sphpar.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     3125 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/sphray.F90
+-rw-r--r--   0 rieder     (501) staff       (20)     5124 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/update_particles.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    27441 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/viewer.F90
+-rw-r--r--   0 rieder     (501) staff       (20)    23330 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/src/amuse/community/sphray/src/voronov_atomic_rates.F90
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:57.683276 amuse-sphray-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-sphray-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-sphray-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-sphray-2024.4.0/support/version.py
```

### Comparing `amuse-sphray-2023.5.0/PKG-INFO` & `amuse-sphray-2024.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-sphray
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - SPHRay
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
 
 This package installs the SPHRay community code for AMUSE.
```

### Comparing `amuse-sphray-2023.5.0/amuse_sphray.egg-info/PKG-INFO` & `amuse-sphray-2024.4.0/amuse_sphray.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-sphray
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - SPHRay
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
 
 This package installs the SPHRay community code for AMUSE.
```

### Comparing `amuse-sphray-2023.5.0/amuse_sphray.egg-info/SOURCES.txt` & `amuse-sphray-2024.4.0/amuse_sphray.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 amuse_sphray.egg-info/PKG-INFO
 amuse_sphray.egg-info/SOURCES.txt
 amuse_sphray.egg-info/dependency_links.txt
 amuse_sphray.egg-info/requires.txt
 amuse_sphray.egg-info/top_level.txt
 src/amuse/community/sphray/Makefile
 src/amuse/community/sphray/__init__.py
+src/amuse/community/sphray/_version.py
 src/amuse/community/sphray/interface.f90
 src/amuse/community/sphray/interface.py
-src/amuse/community/sphray/version.py
 src/amuse/community/sphray/data/input/sphray_4K
 src/amuse/community/sphray/data/input/test1_sources_001.1
 src/amuse/community/sphray/data/input/test2_sources_001.1
 src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt
 src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt
 src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt
 src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt
```

### Comparing `amuse-sphray-2023.5.0/setup.py` & `amuse-sphray-2024.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.sphray.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/sphray/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/sphray/_version.py",
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
         'amuse.community.sphray': 'src/amuse/community/sphray',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/Makefile` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Cen.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hui.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Hum.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Vor.txt` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/atomic_rates/atomic_rates_Vor.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/latmon_b2cd_table.txt` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/column_depth/latmon_b2cd_table.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/column_depth/tophat_b2cd_table.txt` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/column_depth/tophat_b2cd_table.txt`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/power2.0.cdf` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/power2.0.cdf`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/power4.0.cdf` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/power4.0.cdf`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/thermal1e5.cdf` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/thermal1e5.cdf`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/spectra/thermal6e4.cdf` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/spectra/thermal6e4.cdf`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/data/input/sphray_4K` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/data/input/sphray_4K`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/interface.f90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/interface.f90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/interface.py` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/Makefile` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/MakefileTemplate` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/MakefileTemplate`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GL.h` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/GL.h`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLU.h` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/GLU.h`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLUT.h` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/GLUT.h`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/GLUT_fonts.c` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/GLUT_fonts.c`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_freeglut.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_freeglut.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_gl.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_gl.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glu.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glu.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glut.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_glut.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/OpenGL_openglut.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/OpenGL_openglut.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/fthread.f` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/fthread.f`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/pt.c` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/pt.c`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/pt.h` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/pt.h`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/OpenGL/ptf77.c` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/OpenGL/ptf77.c`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/amuse_helpers.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/amuse_helpers.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/amuse_mainloop.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/amuse_mainloop.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/atomic_rates.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/b2cd.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/b2cd.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/bdf.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/bdf.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/cen_atomic_rates.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/cen_atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/config.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/config.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/cosmology.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/cosmology.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/density_test.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/density_test.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/euler.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/euler.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_cosmoBH_input.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_cosmoBH_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_general_class.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_general_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_owls_header_class.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_owls_header_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_owls_input.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_owls_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_header_class.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_public_header_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_header_hdf5_class.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_public_header_hdf5_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_input.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_public_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_public_input_hdf5.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_public_input_hdf5.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_sphray_header_class.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_sphray_header_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/gadget_vbromm_input.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/gadget_vbromm_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/global.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/global.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/glsphray.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/glsphray.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hash.f90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/hash.f90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hdf5_io.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/hdf5_io.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/healpix_types.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/healpix_types.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hui_gnedin_atomic_rates.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/hui_gnedin_atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/hummer_atomic_rates.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/hummer_atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/iliev_comparison_project.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/iliev_comparison_project.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/initialize.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/initialize.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ion_table_class.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/ion_table_class.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ion_temperature_update.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/ion_temperature_update.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ionpar.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/ionpar.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/kerneldensity.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/kerneldensity.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/m_mrgrnk.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/m_mrgrnk.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/main_input.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/main_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/mainloop.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/mainloop.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/mt19937.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/mt19937.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/myf03.f90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/myf03.f90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/nblist.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/nblist.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/octtree3.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/octtree3.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/octtree3p.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/octtree3p.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/output.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/output.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/particle_system.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/particle_system.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/physical_constants.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/physical_constants.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/pix_tools.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/pix_tools.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/ray.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/ray.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/raylist.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/raylist.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sobol.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/sobol.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/source_input.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/source_input.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/spectra.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/spectra.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sphpar.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/sphpar.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/sphray.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/sphray.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/update_particles.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/update_particles.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/viewer.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/viewer.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/src/amuse/community/sphray/src/voronov_atomic_rates.F90` & `amuse-sphray-2024.4.0/src/amuse/community/sphray/src/voronov_atomic_rates.F90`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/support/__init__.py` & `amuse-sphray-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/support/classifiers.py` & `amuse-sphray-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/support/config.py` & `amuse-sphray-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/support/generate_main.py` & `amuse-sphray-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/support/getsp.class` & `amuse-sphray-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/support/getsp.java` & `amuse-sphray-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/support/misc.py` & `amuse-sphray-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-sphray-2023.5.0/support/setup_codes.py` & `amuse-sphray-2024.4.0/support/setup_codes.py`

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

