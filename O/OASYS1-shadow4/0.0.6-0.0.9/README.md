# Comparing `tmp/OASYS1-shadow4-0.0.6.tar.gz` & `tmp/OASYS1-shadow4-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OASYS1-shadow4-0.0.6.tar", last modified: Fri Feb 24 21:11:24 2023, max compression
+gzip compressed data, was "OASYS1-shadow4-0.0.9.tar", last modified: Tue Feb 28 21:13:57 2023, max compression
```

## Comparing `OASYS1-shadow4-0.0.6.tar` & `OASYS1-shadow4-0.0.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.861129 OASYS1-shadow4-0.0.6/
--rw-------   0 rook       (505) staff       (20)     1079 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/LICENSE
--rw-------   0 rook       (505) staff       (20)      350 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/MANIFEST.in
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.848506 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/
--rw-r--r--   0 rook       (505) staff       (20)      663 2023-02-24 21:11:24.000000 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/PKG-INFO
--rw-r--r--   0 rook       (505) staff       (20)     2933 2023-02-24 21:11:24.000000 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/SOURCES.txt
--rw-r--r--   0 rook       (505) staff       (20)        1 2023-02-24 21:11:24.000000 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/dependency_links.txt
--rw-r--r--   0 rook       (505) staff       (20)      226 2023-02-24 21:11:24.000000 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/entry_points.txt
--rw-r--r--   0 rook       (505) staff       (20)       66 2023-02-24 21:11:24.000000 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/namespace_packages.txt
--rw-r--r--   0 rook       (505) staff       (20)        1 2023-01-12 17:00:24.000000 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/not-zip-safe
--rw-r--r--   0 rook       (505) staff       (20)       24 2023-02-24 21:11:24.000000 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/requires.txt
--rw-r--r--   0 rook       (505) staff       (20)       14 2023-02-24 21:11:24.000000 OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/top_level.txt
--rw-r--r--   0 rook       (505) staff       (20)      663 2023-02-24 21:11:24.860902 OASYS1-shadow4-0.0.6/PKG-INFO
--rw-------   0 rook       (505) staff       (20)       90 2023-01-12 17:05:46.000000 OASYS1-shadow4-0.0.6/README.md
--rw-------   0 rook       (505) staff       (20)       16 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/README.txt
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.848673 OASYS1-shadow4-0.0.6/orangecontrib/
--rw-------   0 rook       (505) staff       (20)       83 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.848840 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/
--rw-------   0 rook       (505) staff       (20)       81 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.849474 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/util/
--rw-------   0 rook       (505) staff       (20)     8261 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/util/python_script.py
--rw-------   0 rook       (505) staff       (20)    15577 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/util/shadow_objects.py
--rwx--x--x   0 rook       (505) staff       (20)    74481 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/util/shadow_util.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.850185 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/
--rw-------   0 rook       (505) staff       (20)       81 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.851631 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/
--rw-------   0 rook       (505) staff       (20)        0 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/__init__.py
--rw-r--r--   0 rook       (505) staff       (20)     3022 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/ow_automatic_element.py
--rw-r--r--   0 rook       (505) staff       (20)    17820 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/ow_electron_beam.py
--rwx--x--x   0 rook       (505) staff       (20)    13180 2023-02-24 19:10:23.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/ow_generic_element.py
--rw-------   0 rook       (505) staff       (20)     2541 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/plots.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.852108 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/
--rw-------   0 rook       (505) staff       (20)      133 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.854615 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/
--rw-r--r--   0 rook       (505) staff       (20)    35020 2022-06-23 16:14:55.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/conic_coefficients_mirror.png
--rw-r--r--   0 rook       (505) staff       (20)    31753 2022-06-23 16:14:55.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/ellipsoid_mirror.png
--rw-r--r--   0 rook       (505) staff       (20)    31628 2022-06-23 16:14:55.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/hyperboloid_mirror.png
--rwx--x--x   0 rook       (505) staff       (20)    14391 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/opticalElements.png
--rw-r--r--   0 rook       (505) staff       (20)    32312 2022-06-23 16:14:55.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/paraboloid_mirror.png
--rw-r--r--   0 rook       (505) staff       (20)    17594 2022-06-23 16:14:55.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/plane_mirror.png
--rw-r--r--   0 rook       (505) staff       (20)    34296 2022-06-23 16:14:55.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/spherical_mirror.png
--rw-r--r--   0 rook       (505) staff       (20)    31480 2022-06-23 16:14:55.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/toroidal_mirror.png
--rwxr-xr-x   0 rook       (505) staff       (20)    51550 2023-02-24 21:04:11.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/ow_mirror.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.855947 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/
--rw-------   0 rook       (505) staff       (20)      128 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.857187 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/
--rw-------   0 rook       (505) staff       (20)    14771 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/bending_magnet.png
--rw-------   0 rook       (505) staff       (20)    19767 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/geometrical.png
--rw-------   0 rook       (505) staff       (20)     7895 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/source.png
--rw-------   0 rook       (505) staff       (20)    52413 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/ugaussian.png
--rw-------   0 rook       (505) staff       (20)    21621 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/undulator.png
--rw-------   0 rook       (505) staff       (20)    24422 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/wiggler.png
--rwxr-xr-x   0 rook       (505) staff       (20)     9104 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_bending_magnet.py
--rwxr-xr-x   0 rook       (505) staff       (20)    38957 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_geometrical.py
--rw-r--r--   0 rook       (505) staff       (20)    16810 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_undulator.py
--rwxr-xr-x   0 rook       (505) staff       (20)     7724 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_undulator_gaussian.py
--rw-r--r--   0 rook       (505) staff       (20)    18803 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_wiggler.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.858239 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/
--rw-------   0 rook       (505) staff       (20)      124 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/__init__.py
-drwxr-xr-x   0 rook       (505) staff       (20)        0 2023-02-24 21:11:24.860592 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/
--rw-------   0 rook       (505) staff       (20)     3831 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam3to4.png
--rw-------   0 rook       (505) staff       (20)     3927 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam4to3.png
--rw-------   0 rook       (505) staff       (20)     2611 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam_file_reader.png
--rw-------   0 rook       (505) staff       (20)     2013 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam_file_writer.png
--rw-r--r--   0 rook       (505) staff       (20)    26761 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam_movement.png
--rw-------   0 rook       (505) staff       (20)    11929 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/image_converter.png
--rw-------   0 rook       (505) staff       (20)    12949 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/merge.png
--rw-------   0 rook       (505) staff       (20)    30587 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/to_wofry_wavefront_2d.png
--rwx--x--x   0 rook       (505) staff       (20)    29342 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/utility.png
--rwxr-xr-x   0 rook       (505) staff       (20)     9159 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/ow_beam_movements.py
--rw-r--r--   0 rook       (505) staff       (20)     3258 2023-02-24 15:43:50.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/ow_shadow3_beam_to_shadow4_beam.py
--rw-------   0 rook       (505) staff       (20)     3268 2023-01-12 16:57:03.000000 OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/ow_shadow4_beam_to_shadow3_beam.py
--rw-r--r--   0 rook       (505) staff       (20)       38 2023-02-24 21:11:24.861319 OASYS1-shadow4-0.0.6/setup.cfg
--rwx--x--x   0 rook       (505) staff       (20)     4511 2023-02-24 21:11:21.000000 OASYS1-shadow4-0.0.6/setup.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.190103 OASYS1-shadow4-0.0.9/
+-rw-rw-rw-   0 bishop    (1601)      907     1079 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/LICENSE
+-rw-rw-rw-   0 bishop    (1601)      907      350 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/MANIFEST.in
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.144569 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/
+-rw-rw-rw-   0 bishop    (1601)      907      696 2023-02-28 21:13:57.000000 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907     2933 2023-02-28 21:13:57.000000 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/SOURCES.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2023-02-28 21:13:57.000000 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/dependency_links.txt
+-rw-rw-rw-   0 bishop    (1601)      907      227 2023-02-28 21:13:57.000000 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/entry_points.txt
+-rw-rw-rw-   0 bishop    (1601)      907       66 2023-02-28 21:13:57.000000 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/namespace_packages.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2023-02-22 23:09:36.000000 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/not-zip-safe
+-rw-rw-rw-   0 bishop    (1601)      907       32 2023-02-28 21:13:57.000000 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/requires.txt
+-rw-rw-rw-   0 bishop    (1601)      907       14 2023-02-28 21:13:57.000000 OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/top_level.txt
+-rw-r--r--   0 bishop    (1601)      907      696 2023-02-28 21:13:57.189400 OASYS1-shadow4-0.0.9/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907       90 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/README.md
+-rw-rw-rw-   0 bishop    (1601)      907       16 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/README.txt
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.144946 OASYS1-shadow4-0.0.9/orangecontrib/
+-rw-rw-rw-   0 bishop    (1601)      907       83 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.145573 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/
+-rw-rw-rw-   0 bishop    (1601)      907       81 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.147160 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/util/
+-rw-rw-rw-   0 bishop    (1601)      907     8261 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/util/python_script.py
+-rw-rw-rw-   0 bishop    (1601)      907    15577 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/util/shadow_objects.py
+-rwxrwxrwx   0 bishop    (1601)      907    74481 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/util/shadow_util.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.148164 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/
+-rw-rw-rw-   0 bishop    (1601)      907       81 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.151449 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     3022 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/ow_automatic_element.py
+-rw-rw-rw-   0 bishop    (1601)      907    17820 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/ow_electron_beam.py
+-rwxrwxrwx   0 bishop    (1601)      907    13180 2023-02-27 15:50:20.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/ow_generic_element.py
+-rw-rw-rw-   0 bishop    (1601)      907     2541 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/plots.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.153078 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/
+-rw-rw-rw-   0 bishop    (1601)      907      133 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.161847 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/
+-rw-rw-rw-   0 bishop    (1601)      907    35020 2023-02-27 15:50:20.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/conic_coefficients_mirror.png
+-rw-rw-rw-   0 bishop    (1601)      907    31753 2023-02-27 15:50:20.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/ellipsoid_mirror.png
+-rw-rw-rw-   0 bishop    (1601)      907    31628 2023-02-27 15:50:20.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/hyperboloid_mirror.png
+-rwxrwxrwx   0 bishop    (1601)      907    14391 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/opticalElements.png
+-rw-rw-rw-   0 bishop    (1601)      907    32312 2023-02-27 15:50:20.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/paraboloid_mirror.png
+-rw-rw-rw-   0 bishop    (1601)      907    17594 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/plane_mirror.png
+-rw-rw-rw-   0 bishop    (1601)      907    34296 2023-02-27 15:50:20.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/spherical_mirror.png
+-rw-rw-rw-   0 bishop    (1601)      907    31480 2023-02-27 15:50:20.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/toroidal_mirror.png
+-rwxrwxrwx   0 bishop    (1601)      907    51965 2023-02-28 20:53:21.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/ow_mirror.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.167375 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/
+-rw-rw-rw-   0 bishop    (1601)      907      128 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.173665 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/
+-rw-rw-rw-   0 bishop    (1601)      907    14771 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/bending_magnet.png
+-rw-rw-rw-   0 bishop    (1601)      907    19767 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/geometrical.png
+-rw-rw-rw-   0 bishop    (1601)      907     7895 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/source.png
+-rw-rw-rw-   0 bishop    (1601)      907    52413 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/ugaussian.png
+-rw-rw-rw-   0 bishop    (1601)      907    21621 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/undulator.png
+-rw-rw-rw-   0 bishop    (1601)      907    24422 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/wiggler.png
+-rwxrwxrwx   0 bishop    (1601)      907     9104 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_bending_magnet.py
+-rwxrwxrwx   0 bishop    (1601)      907    38957 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_geometrical.py
+-rw-rw-rw-   0 bishop    (1601)      907    16810 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_undulator.py
+-rwxrwxrwx   0 bishop    (1601)      907     7724 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_undulator_gaussian.py
+-rw-rw-rw-   0 bishop    (1601)      907    18803 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_wiggler.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.177986 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/
+-rw-rw-rw-   0 bishop    (1601)      907      124 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-02-28 21:13:57.187792 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/
+-rw-rw-rw-   0 bishop    (1601)      907     3831 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam3to4.png
+-rw-rw-rw-   0 bishop    (1601)      907     3927 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam4to3.png
+-rw-rw-rw-   0 bishop    (1601)      907     2611 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam_file_reader.png
+-rw-rw-rw-   0 bishop    (1601)      907     2013 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam_file_writer.png
+-rw-rw-rw-   0 bishop    (1601)      907    26761 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam_movement.png
+-rw-rw-rw-   0 bishop    (1601)      907    11929 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/image_converter.png
+-rw-rw-rw-   0 bishop    (1601)      907    12949 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/merge.png
+-rw-rw-rw-   0 bishop    (1601)      907    30587 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/to_wofry_wavefront_2d.png
+-rwxrwxrwx   0 bishop    (1601)      907    29342 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/utility.png
+-rwxrwxrwx   0 bishop    (1601)      907     9159 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/ow_beam_movements.py
+-rw-rw-rw-   0 bishop    (1601)      907     3258 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/ow_shadow3_beam_to_shadow4_beam.py
+-rw-rw-rw-   0 bishop    (1601)      907     3268 2023-02-22 23:06:31.000000 OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/ow_shadow4_beam_to_shadow3_beam.py
+-rw-r--r--   0 bishop    (1601)      907       38 2023-02-28 21:13:57.190341 OASYS1-shadow4-0.0.9/setup.cfg
+-rwxrwxrwx   0 bishop    (1601)      907     4519 2023-02-28 21:13:52.000000 OASYS1-shadow4-0.0.9/setup.py
```

### Comparing `OASYS1-shadow4-0.0.6/LICENSE` & `OASYS1-shadow4-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/OASYS1_shadow4.egg-info/SOURCES.txt` & `OASYS1-shadow4-0.0.9/OASYS1_shadow4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/util/python_script.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/util/python_script.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/util/shadow_objects.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/util/shadow_objects.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/util/shadow_util.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/util/shadow_util.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/ow_automatic_element.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/ow_automatic_element.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/ow_electron_beam.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/ow_electron_beam.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/ow_generic_element.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/ow_generic_element.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/gui/plots.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/gui/plots.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/conic_coefficients_mirror.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/conic_coefficients_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/ellipsoid_mirror.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/ellipsoid_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/hyperboloid_mirror.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/hyperboloid_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/opticalElements.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/opticalElements.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/paraboloid_mirror.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/paraboloid_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/plane_mirror.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/plane_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/spherical_mirror.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/spherical_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/icons/toroidal_mirror.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/icons/toroidal_mirror.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/optics/ow_mirror.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/optics/ow_mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,19 @@
 from orangecontrib.shadow4.util.shadow_objects import ShadowBeam
 
 from syned.beamline.beamline import Beamline
 from shadow4.beamline.s4_beamline import S4Beamline
 
 from syned.widget.widget_decorator import WidgetDecorator
 
-from shadow4.syned.element_coordinates import ElementCoordinates
-
-from shadow4.syned.shape import Rectangle  # TODO from syned.beamline.shape
-from shadow4.syned.shape import Convexity  #  Convexity: NONE = -1  UPWARD = 0  DOWNWARD = 1
-from shadow4.syned.shape import Direction  #  Direction:  TANGENTIAL = 0  SAGITTAL = 1
-from shadow4.syned.shape import Side       #  Side:  SOURCE = 0  IMAGE = 1
+from syned.beamline.element_coordinates import ElementCoordinates
+from syned.beamline.shape import Rectangle
+from syned.beamline.shape import Convexity  #  Convexity: NONE = -1  UPWARD = 0  DOWNWARD = 1
+from syned.beamline.shape import Direction  #  Direction:  TANGENTIAL = 0  SAGITTAL = 1
+from syned.beamline.shape import Side       #  Side:  SOURCE = 0  IMAGE = 1
 
 from shadow4.beamline.s4_optical_element import SurfaceCalculation # INTERNAL = 0  EXTERNAL = 1
 
 from shadow4.beamline.optical_elements.mirrors.s4_conic_mirror import S4ConicMirror, S4ConicMirrorElement
 from shadow4.beamline.optical_elements.mirrors.s4_toroidal_mirror import S4ToroidalMirror, S4ToroidalMirrorElement
 from shadow4.beamline.optical_elements.mirrors.s4_surface_data_mirror import S4SurfaceDataMirror, S4SurfaceDataMirrorElement
 from shadow4.beamline.optical_elements.mirrors.s4_plane_mirror import S4PlaneMirror, S4PlaneMirrorElement
@@ -52,20 +51,28 @@
     icons_for_type = {0 : "icons/plane_mirror.png",
                       1 : "icons/spherical_mirror.png",
                       2 : "icons/ellipsoid_mirror.png",
                       3 : "icons/hyperboloid_mirror.png",
                       4 : "icons/paraboloid_mirror.png",
                       5 : "icons/toroidal_mirror.png",}
 
-    titles_for_type = {0 : "Plane",
-                       1 : "Spherical",
-                       2 : "Elliptical",
-                       3 : "Hyperbolical",
-                       4 : "Parabolical",
-                       5 : "Toroidal",}
+    mirror_names = ["Generic Mirror",
+                    "Plane Mirror",
+                    "Spherical Mirror",
+                    "Elliptical Mirror",
+                    "Hyperbolical Mirror",
+                    "Parabolical Mirror",
+                    "Toroidal Mirror"]
+
+    titles_for_type = {0 : mirror_names[1],
+                       1 : mirror_names[2],
+                       2 : mirror_names[3],
+                       3 : mirror_names[4],
+                       4 : mirror_names[5],
+                       5 : mirror_names[6]}
 
     name = "Generic Mirror"
     description = "Shadow Mirror"
     icon = "icons/plane_mirror.png"
 
     priority = 5
 
@@ -134,23 +141,25 @@
     dim_x_minus  = Setting(1.0)
     dim_y_plus   = Setting(1.0)
     dim_y_minus  = Setting(1.0)
 
     input_beam = None
     beamline   = None
 
-    def createdFromNode(self, node : SchemeNode):
-        super(GenericElement, self).createdFromNode(node)
+    def widgetNodeAdded(self, node_item : SchemeNode):
+        super(GenericElement, self).widgetNodeAdded(node_item)
 
         self.__change_icon_from_surface_type(is_init=False)
 
     def __change_icon_from_surface_type(self, is_init):
         if not is_init:
-            self._node.description.icon = self.icons_for_type[self.surface_shape_type]
-            self.changeNodeIcon(icon_loader.from_description(self._node.description).get(self._node.description.icon))
+            node = self.getNode()
+            node.description.icon = self.icons_for_type[self.surface_shape_type]
+            self.changeNodeIcon(icon_loader.from_description(node.description).get(node.description.icon))
+            if node.title in self.mirror_names: self.changeNodeTitle(self.titles_for_type[self.surface_shape_type])
 
     def __init__(self):
         super().__init__()
 
         #
         # main buttons
         #
@@ -969,8 +978,8 @@
 
     from PyQt5.QtWidgets import QApplication
     a = QApplication(sys.argv)
     ow = OWMirror()
     ow.setBeam(get_test_beam())
     ow.show()
     a.exec_()
-    ow.saveSettings()
+    ow.saveSettings()
```

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/bending_magnet.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/bending_magnet.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/geometrical.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/geometrical.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/source.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/source.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/ugaussian.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/ugaussian.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/undulator.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/undulator.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/icons/wiggler.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/icons/wiggler.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_bending_magnet.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_bending_magnet.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_geometrical.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_geometrical.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_undulator.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_undulator.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_undulator_gaussian.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_undulator_gaussian.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/sources/ow_wiggler.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/sources/ow_wiggler.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam3to4.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam3to4.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam4to3.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam4to3.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam_file_reader.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam_file_reader.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam_file_writer.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam_file_writer.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/beam_movement.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/beam_movement.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/image_converter.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/image_converter.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/merge.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/merge.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/to_wofry_wavefront_2d.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/to_wofry_wavefront_2d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/icons/utility.png` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/icons/utility.png`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/ow_beam_movements.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/ow_beam_movements.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/ow_shadow3_beam_to_shadow4_beam.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/ow_shadow3_beam_to_shadow4_beam.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/orangecontrib/shadow4/widgets/tools/ow_shadow4_beam_to_shadow3_beam.py` & `OASYS1-shadow4-0.0.9/orangecontrib/shadow4/widgets/tools/ow_shadow4_beam_to_shadow3_beam.py`

 * *Files identical despite different names*

### Comparing `OASYS1-shadow4-0.0.6/setup.py` & `OASYS1-shadow4-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 import imp
 import os
 import sys
 from setuptools import find_packages, setup
 import subprocess
 
 NAME = 'OASYS1-shadow4'
-VERSION = '0.0.6'
+VERSION = '0.0.9'
 ISRELEASED = False
 
 DESCRIPTION = 'oasys-shadow4: Oasys widgets for shadow4'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.txt')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'M. Sanchez del Rio'
 AUTHOR_EMAIL = 'srio@esrf.eu'
@@ -85,16 +85,16 @@
 
 
 SETUP_REQUIRES = (
                   'setuptools',
                   )
 
 INSTALL_REQUIRES = (
-                    'oasys1>=1.2.102',
-                    'shadow4'
+                    'oasys1>=1.2.123',
+                    'shadow4>=0.1.10'
                     )
 
 PACKAGES = find_packages(exclude=('*.tests', '*.tests.*', 'tests.*', 'tests'))
 
 
 
 PACKAGE_DATA = {
```

