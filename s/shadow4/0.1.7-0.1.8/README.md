# Comparing `tmp/shadow4-0.1.7.tar.gz` & `tmp/shadow4-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shadow4-0.1.7.tar", last modified: Thu Jan 12 11:20:43 2023, max compression
+gzip compressed data, was "dist/shadow4-0.1.8.tar", last modified: Wed Jan 18 19:21:53 2023, max compression
```

## Comparing `shadow4-0.1.7.tar` & `shadow4-0.1.8.tar`

### file list

```diff
@@ -1,108 +1,123 @@
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/
--rw-r--r--   0 srio      (4230) soft      (3401)     1079 2020-10-16 10:04:46.000000 shadow4-0.1.7/LICENSE
--rw-r--r--   0 srio      (4230) soft      (3401)      263 2023-01-12 11:20:43.000000 shadow4-0.1.7/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)      121 2020-10-16 10:04:46.000000 shadow4-0.1.7/README.md
--rw-r--r--   0 srio      (4230) soft      (3401)       38 2023-01-12 11:20:43.000000 shadow4-0.1.7/setup.cfg
--rw-r--r--   0 srio      (4230) soft      (3401)     3137 2023-01-12 11:19:24.000000 shadow4-0.1.7/setup.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/
--rw-r--r--   0 srio      (4230) soft      (3401)       21 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/beam/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beam/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    50423 2022-06-16 10:21:55.000000 shadow4-0.1.7/shadow4/beam/beam.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/beamline/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/absorbers/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/absorbers/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     5763 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/absorbers/s4_screen.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/crystals/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/crystals/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    18528 2022-06-14 10:23:47.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/crystals/s4_crystal.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4823 2022-06-14 10:23:38.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/crystals/s4_plane_crystal.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/gratings/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/gratings/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     9887 2022-06-16 10:12:57.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/gratings/s4_grating.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4746 2022-06-16 10:06:38.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/gratings/s4_plane_grating.py
--rw-r--r--   0 srio      (4230) soft      (3401)     5520 2022-06-16 10:08:20.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/gratings/s4_sphere_grating.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/ideal_elements/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/ideal_elements/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1575 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/ideal_elements/s4_empty.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3693 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/ideal_elements/s4_ideal_lens.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     5880 2022-06-14 10:12:44.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_additive_surface_data_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1966 2022-06-14 10:12:44.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_conic_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2607 2022-06-14 10:12:44.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_ellipsoid_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3737 2022-06-14 10:12:44.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_hyperboloid_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)    11070 2022-06-14 09:55:18.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2706 2022-06-14 10:13:57.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_paraboloid_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1968 2022-06-14 10:13:57.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_plane_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2526 2022-06-14 10:15:45.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_sphere_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2134 2022-06-14 10:15:45.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_surface_data_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2257 2022-06-14 10:15:45.000000 shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_toroidal_mirror.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2670 2023-01-12 10:48:31.000000 shadow4-0.1.7/shadow4/beamline/s4_beamline.py
--rw-r--r--   0 srio      (4230) soft      (3401)      515 2022-05-17 10:44:42.000000 shadow4-0.1.7/shadow4/beamline/s4_beamline_element.py
--rw-r--r--   0 srio      (4230) soft      (3401)    15917 2022-06-16 09:57:28.000000 shadow4-0.1.7/shadow4/beamline/s4_optical_element.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/devel/
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/devel/wolter/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2022-10-07 09:57:51.000000 shadow4-0.1.7/shadow4/devel/wolter/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)      695 2022-09-20 10:26:23.000000 shadow4-0.1.7/shadow4/devel/wolter/conic_confocal.py
--rw-r--r--   0 srio      (4230) soft      (3401)    32996 2022-12-12 08:31:43.000000 shadow4-0.1.7/shadow4/devel/wolter/conic_penelope.py
--rw-r--r--   0 srio      (4230) soft      (3401)    14381 2022-09-14 15:18:19.000000 shadow4-0.1.7/shadow4/devel/wolter/conic_viewer.py
--rw-r--r--   0 srio      (4230) soft      (3401)    13958 2022-12-12 12:41:04.000000 shadow4-0.1.7/shadow4/devel/wolter/conics_from_factory_parameters.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3245 2022-09-20 10:27:38.000000 shadow4-0.1.7/shadow4/devel/wolter/elliptic_coordinates.py
--rw-r--r--   0 srio      (4230) soft      (3401)    10571 2022-12-13 13:44:27.000000 shadow4-0.1.7/shadow4/devel/wolter/wolter1.py
--rw-r--r--   0 srio      (4230) soft      (3401)     6527 2022-12-13 11:39:48.000000 shadow4-0.1.7/shadow4/devel/wolter/wolter_underwood.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/optical_surfaces/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/optical_surfaces/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    41721 2022-10-07 10:03:00.000000 shadow4-0.1.7/shadow4/optical_surfaces/s4_conic.py
--rw-r--r--   0 srio      (4230) soft      (3401)    15175 2022-06-07 15:09:00.000000 shadow4-0.1.7/shadow4/optical_surfaces/s4_mesh.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4312 2022-05-25 08:13:30.000000 shadow4-0.1.7/shadow4/optical_surfaces/s4_optical_surface.py
--rw-r--r--   0 srio      (4230) soft      (3401)    15547 2022-05-24 10:31:14.000000 shadow4-0.1.7/shadow4/optical_surfaces/s4_toroid.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/physical_models/
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/physical_models/bragg/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/physical_models/bragg/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    12017 2022-01-28 08:38:12.000000 shadow4-0.1.7/shadow4/physical_models/bragg/bragg.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/physical_models/mlayer/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/physical_models/mlayer/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    42070 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/physical_models/mlayer/mlayer.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/physical_models/prerefl/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/physical_models/prerefl/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21883 2021-12-16 15:03:11.000000 shadow4-0.1.7/shadow4/physical_models/prerefl/prerefl.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/sources/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/sources/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/sources/bending_magnet/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/sources/bending_magnet/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     6001 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/sources/bending_magnet/s4_bending_magnet.py
--rw-r--r--   0 srio      (4230) soft      (3401)    23917 2022-05-19 06:31:41.000000 shadow4-0.1.7/shadow4/sources/bending_magnet/s4_bending_magnet_light_source.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2222 2022-05-19 06:31:41.000000 shadow4-0.1.7/shadow4/sources/s4_electron_beam.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1232 2022-05-19 06:31:41.000000 shadow4-0.1.7/shadow4/sources/s4_light_source.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/sources/source_geometrical/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/sources/source_geometrical/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    11878 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/sources/source_geometrical/probability_distributions.py
--rw-r--r--   0 srio      (4230) soft      (3401)     7276 2022-06-14 12:42:57.000000 shadow4-0.1.7/shadow4/sources/source_geometrical/source_gaussian.py
--rw-r--r--   0 srio      (4230) soft      (3401)    19852 2022-06-14 12:44:52.000000 shadow4-0.1.7/shadow4/sources/source_geometrical/source_geometrical.py
--rw-r--r--   0 srio      (4230) soft      (3401)    12027 2022-10-10 14:22:16.000000 shadow4-0.1.7/shadow4/sources/source_geometrical/source_grid_cartesian.py
--rw-r--r--   0 srio      (4230) soft      (3401)    11821 2022-10-11 08:49:35.000000 shadow4-0.1.7/shadow4/sources/source_geometrical/source_grid_polar.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/sources/undulator/
--rw-r--r--   0 srio      (4230) soft      (3401)     8710 2022-05-19 06:31:41.000000 shadow4-0.1.7/shadow4/sources/undulator/s4_undulator.py
--rw-r--r--   0 srio      (4230) soft      (3401)    40967 2022-05-19 06:31:41.000000 shadow4-0.1.7/shadow4/sources/undulator/s4_undulator_light_source.py
--rw-r--r--   0 srio      (4230) soft      (3401)    10607 2022-05-13 08:23:59.000000 shadow4-0.1.7/shadow4/sources/undulator/source_undulator_factory.py
--rw-r--r--   0 srio      (4230) soft      (3401)     5050 2022-05-13 08:31:45.000000 shadow4-0.1.7/shadow4/sources/undulator/source_undulator_factory_pysru.py
--rw-r--r--   0 srio      (4230) soft      (3401)    12318 2022-05-13 08:31:45.000000 shadow4-0.1.7/shadow4/sources/undulator/source_undulator_factory_srw.py
--rw-r--r--   0 srio      (4230) soft      (3401)    13416 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/sources/undulator/source_undulator_input_output.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/sources/wiggler/
--rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/sources/wiggler/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    12459 2022-05-19 06:31:41.000000 shadow4-0.1.7/shadow4/sources/wiggler/s4_wiggler.py
--rw-r--r--   0 srio      (4230) soft      (3401)    36805 2022-05-19 06:31:41.000000 shadow4-0.1.7/shadow4/sources/wiggler/s4_wiggler_light_source.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4/tools/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/tools/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3117 2022-06-14 11:48:36.000000 shadow4-0.1.7/shadow4/tools/arrayofvectors.py
--rw-r--r--   0 srio      (4230) soft      (3401)    18250 2020-10-16 10:04:46.000000 shadow4-0.1.7/shadow4/tools/graphics.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4.egg-info/
--rw-r--r--   0 srio      (4230) soft      (3401)      263 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4.egg-info/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)     3749 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4.egg-info/SOURCES.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4.egg-info/dependency_links.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       57 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4.egg-info/requires.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        8 2023-01-12 11:20:43.000000 shadow4-0.1.7/shadow4.egg-info/top_level.txt
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/
+-rw-r--r--   0 srio      (4230) soft      (3401)     1079 2020-10-16 10:04:46.000000 shadow4-0.1.8/LICENSE
+-rw-r--r--   0 srio      (4230) soft      (3401)      263 2023-01-18 19:21:53.000000 shadow4-0.1.8/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)      125 2023-01-18 11:56:55.000000 shadow4-0.1.8/README.md
+-rw-r--r--   0 srio      (4230) soft      (3401)       38 2023-01-18 19:21:53.000000 shadow4-0.1.8/setup.cfg
+-rw-r--r--   0 srio      (4230) soft      (3401)     3221 2023-01-18 19:21:16.000000 shadow4-0.1.8/setup.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/
+-rw-r--r--   0 srio      (4230) soft      (3401)       21 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/beam/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beam/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    50423 2022-06-16 10:21:55.000000 shadow4-0.1.8/shadow4/beam/beam.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/beamline/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/absorbers/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/absorbers/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5763 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/absorbers/s4_screen.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/crystals/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/crystals/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    18528 2022-06-14 10:23:47.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/crystals/s4_crystal.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4823 2022-06-14 10:23:38.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/crystals/s4_plane_crystal.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/gratings/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/gratings/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     9887 2022-06-16 10:12:57.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/gratings/s4_grating.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4746 2022-06-16 10:06:38.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/gratings/s4_plane_grating.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5520 2022-06-16 10:08:20.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/gratings/s4_sphere_grating.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/ideal_elements/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/ideal_elements/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1575 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/ideal_elements/s4_empty.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3693 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/ideal_elements/s4_ideal_lens.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5880 2022-06-14 10:12:44.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_additive_surface_data_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1966 2022-06-14 10:12:44.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_conic_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2607 2022-06-14 10:12:44.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_ellipsoid_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3737 2022-06-14 10:12:44.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_hyperboloid_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    11070 2022-06-14 09:55:18.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2706 2022-06-14 10:13:57.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_paraboloid_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1968 2022-06-14 10:13:57.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_plane_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2526 2022-06-14 10:15:45.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_sphere_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2134 2022-06-14 10:15:45.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_surface_data_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2257 2022-06-14 10:15:45.000000 shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_toroidal_mirror.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2670 2023-01-12 10:48:31.000000 shadow4-0.1.8/shadow4/beamline/s4_beamline.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      515 2022-05-17 10:44:42.000000 shadow4-0.1.8/shadow4/beamline/s4_beamline_element.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    15917 2022-06-16 09:57:28.000000 shadow4-0.1.8/shadow4/beamline/s4_optical_element.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/devel/
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/devel/wolter/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2022-10-07 09:57:51.000000 shadow4-0.1.8/shadow4/devel/wolter/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      695 2022-09-20 10:26:23.000000 shadow4-0.1.8/shadow4/devel/wolter/conic_confocal.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    32996 2022-12-12 08:31:43.000000 shadow4-0.1.8/shadow4/devel/wolter/conic_penelope.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    14381 2022-09-14 15:18:19.000000 shadow4-0.1.8/shadow4/devel/wolter/conic_viewer.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    13958 2022-12-12 12:41:04.000000 shadow4-0.1.8/shadow4/devel/wolter/conics_from_factory_parameters.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3245 2022-09-20 10:27:38.000000 shadow4-0.1.8/shadow4/devel/wolter/elliptic_coordinates.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    10568 2023-01-13 15:52:46.000000 shadow4-0.1.8/shadow4/devel/wolter/wolter1.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     6527 2022-12-13 11:39:48.000000 shadow4-0.1.8/shadow4/devel/wolter/wolter_underwood.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/optical_surfaces/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/optical_surfaces/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    41721 2022-10-07 10:03:00.000000 shadow4-0.1.8/shadow4/optical_surfaces/s4_conic.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    15175 2022-06-07 15:09:00.000000 shadow4-0.1.8/shadow4/optical_surfaces/s4_mesh.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4312 2022-05-25 08:13:30.000000 shadow4-0.1.8/shadow4/optical_surfaces/s4_optical_surface.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    15547 2022-05-24 10:31:14.000000 shadow4-0.1.8/shadow4/optical_surfaces/s4_toroid.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/physical_models/
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/physical_models/bragg/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/physical_models/bragg/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    12017 2022-01-28 08:38:12.000000 shadow4-0.1.8/shadow4/physical_models/bragg/bragg.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/physical_models/mlayer/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/physical_models/mlayer/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    42070 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/physical_models/mlayer/mlayer.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/physical_models/prerefl/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/physical_models/prerefl/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21883 2021-12-16 15:03:11.000000 shadow4-0.1.8/shadow4/physical_models/prerefl/prerefl.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/sources/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/sources/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/sources/bending_magnet/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/sources/bending_magnet/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     6001 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/sources/bending_magnet/s4_bending_magnet.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    23917 2022-05-19 06:31:41.000000 shadow4-0.1.8/shadow4/sources/bending_magnet/s4_bending_magnet_light_source.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2222 2022-05-19 06:31:41.000000 shadow4-0.1.8/shadow4/sources/s4_electron_beam.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1232 2022-05-19 06:31:41.000000 shadow4-0.1.8/shadow4/sources/s4_light_source.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/sources/source_geometrical/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/sources/source_geometrical/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    11878 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/sources/source_geometrical/probability_distributions.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     7276 2022-06-14 12:42:57.000000 shadow4-0.1.8/shadow4/sources/source_geometrical/source_gaussian.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    19852 2022-06-14 12:44:52.000000 shadow4-0.1.8/shadow4/sources/source_geometrical/source_geometrical.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    12027 2022-10-10 14:22:16.000000 shadow4-0.1.8/shadow4/sources/source_geometrical/source_grid_cartesian.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    11821 2022-10-11 08:49:35.000000 shadow4-0.1.8/shadow4/sources/source_geometrical/source_grid_polar.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/sources/undulator/
+-rw-r--r--   0 srio      (4230) soft      (3401)     8710 2022-05-19 06:31:41.000000 shadow4-0.1.8/shadow4/sources/undulator/s4_undulator.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    40967 2022-05-19 06:31:41.000000 shadow4-0.1.8/shadow4/sources/undulator/s4_undulator_light_source.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    10607 2022-05-13 08:23:59.000000 shadow4-0.1.8/shadow4/sources/undulator/source_undulator_factory.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5050 2022-05-13 08:31:45.000000 shadow4-0.1.8/shadow4/sources/undulator/source_undulator_factory_pysru.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    12318 2022-05-13 08:31:45.000000 shadow4-0.1.8/shadow4/sources/undulator/source_undulator_factory_srw.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    13416 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/sources/undulator/source_undulator_input_output.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/sources/wiggler/
+-rw-r--r--   0 srio      (4230) soft      (3401)       20 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/sources/wiggler/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    12459 2022-05-19 06:31:41.000000 shadow4-0.1.8/shadow4/sources/wiggler/s4_wiggler.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    36805 2022-05-19 06:31:41.000000 shadow4-0.1.8/shadow4/sources/wiggler/s4_wiggler_light_source.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/syned/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/syned/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/syned/absorbers/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/syned/absorbers/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      361 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/syned/absorbers/absorber.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      662 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/syned/absorbers/beam_stopper.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      860 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/syned/absorbers/filter.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1148 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/syned/absorbers/holed_filter.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      941 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/syned/absorbers/slit.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1491 2022-05-17 10:48:15.000000 shadow4-0.1.8/shadow4/syned/beamline_element.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2736 2022-01-17 08:33:48.000000 shadow4-0.1.8/shadow4/syned/element_coordinates.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/syned/refractors/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2022-01-10 09:44:04.000000 shadow4-0.1.8/shadow4/syned/refractors/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1385 2022-01-10 15:45:14.000000 shadow4-0.1.8/shadow4/syned/refractors/interface.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    36205 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/syned/shape.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4/tools/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/tools/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3117 2022-06-14 11:48:36.000000 shadow4-0.1.8/shadow4/tools/arrayofvectors.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    18250 2020-10-16 10:04:46.000000 shadow4-0.1.8/shadow4/tools/graphics.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4.egg-info/
+-rw-r--r--   0 srio      (4230) soft      (3401)      263 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4.egg-info/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)     4162 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4.egg-info/SOURCES.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4.egg-info/dependency_links.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       57 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4.egg-info/requires.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        8 2023-01-18 19:21:53.000000 shadow4-0.1.8/shadow4.egg-info/top_level.txt
```

### Comparing `shadow4-0.1.7/LICENSE` & `shadow4-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/setup.py` & `shadow4-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,17 @@
     "shadow4.beamline",
     "shadow4.beamline.optical_elements",
     "shadow4.beamline.optical_elements.ideal_elements",
     "shadow4.beamline.optical_elements.absorbers",
     "shadow4.beamline.optical_elements.mirrors",
     "shadow4.beamline.optical_elements.crystals",
     "shadow4.beamline.optical_elements.gratings",
+    "shadow4.syned",
+    "shadow4.syned.absorbers",
+    "shadow4.syned.refractors",
     "shadow4.tools",
     "shadow4.devel.wolter",  # TODO: relocate
 ]
 
 INSTALL_REQUIRES = (
     'setuptools',
     'numpy',
@@ -78,15 +81,15 @@
     'syned>=1.0.19',
     'srxraylib',
     'wofryimpl',
 )
 
 
 setup(name='shadow4',
-      version='0.1.7',
+      version='0.1.8',
       description='shadow implementation in python',
       author='Manuel Sanchez del Rio',
       author_email='srio@esrf.eu, ',
       url='https://github.com/srio/shadow4/',
       packages=PACKAGES,
       install_requires=INSTALL_REQUIRES,
      )
```

### Comparing `shadow4-0.1.7/shadow4/beam/beam.py` & `shadow4-0.1.8/shadow4/beam/beam.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/absorbers/s4_screen.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/absorbers/s4_screen.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/crystals/s4_crystal.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/crystals/s4_crystal.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/crystals/s4_plane_crystal.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/crystals/s4_plane_crystal.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/gratings/s4_grating.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/gratings/s4_grating.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/gratings/s4_plane_grating.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/gratings/s4_plane_grating.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/gratings/s4_sphere_grating.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/gratings/s4_sphere_grating.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/ideal_elements/s4_empty.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/ideal_elements/s4_empty.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/ideal_elements/s4_ideal_lens.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/ideal_elements/s4_ideal_lens.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_additive_surface_data_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_additive_surface_data_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_conic_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_conic_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_ellipsoid_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_ellipsoid_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_hyperboloid_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_hyperboloid_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_paraboloid_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_paraboloid_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_plane_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_plane_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_sphere_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_sphere_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_surface_data_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_surface_data_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/optical_elements/mirrors/s4_toroidal_mirror.py` & `shadow4-0.1.8/shadow4/beamline/optical_elements/mirrors/s4_toroidal_mirror.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/s4_beamline.py` & `shadow4-0.1.8/shadow4/beamline/s4_beamline.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/s4_beamline_element.py` & `shadow4-0.1.8/shadow4/beamline/s4_beamline_element.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/beamline/s4_optical_element.py` & `shadow4-0.1.8/shadow4/beamline/s4_optical_element.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/devel/wolter/conic_confocal.py` & `shadow4-0.1.8/shadow4/devel/wolter/conic_confocal.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/devel/wolter/conic_penelope.py` & `shadow4-0.1.8/shadow4/devel/wolter/conic_penelope.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/devel/wolter/conic_viewer.py` & `shadow4-0.1.8/shadow4/devel/wolter/conic_viewer.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/devel/wolter/conics_from_factory_parameters.py` & `shadow4-0.1.8/shadow4/devel/wolter/conics_from_factory_parameters.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/devel/wolter/elliptic_coordinates.py` & `shadow4-0.1.8/shadow4/devel/wolter/elliptic_coordinates.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/devel/wolter/wolter1.py` & `shadow4-0.1.8/shadow4/devel/wolter/wolter1.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,10 +357,7 @@
         ccc_hyp = tkt_hyp['ccc']
 
         # print("\n\nNormalized Parabola: ",  ccc_ell/ccc_ell[0])
         # print("Normalized Hyperbola: ", ccc_hyp/ccc_hyp[0])
         #
         # print("\n\nParabola: ",  ccc_ell)
         # print("Hyperbola: ", ccc_hyp)
-
-
-
```

### Comparing `shadow4-0.1.7/shadow4/devel/wolter/wolter_underwood.py` & `shadow4-0.1.8/shadow4/devel/wolter/wolter_underwood.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/optical_surfaces/s4_conic.py` & `shadow4-0.1.8/shadow4/optical_surfaces/s4_conic.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/optical_surfaces/s4_mesh.py` & `shadow4-0.1.8/shadow4/optical_surfaces/s4_mesh.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/optical_surfaces/s4_optical_surface.py` & `shadow4-0.1.8/shadow4/optical_surfaces/s4_optical_surface.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/optical_surfaces/s4_toroid.py` & `shadow4-0.1.8/shadow4/optical_surfaces/s4_toroid.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/physical_models/bragg/bragg.py` & `shadow4-0.1.8/shadow4/physical_models/bragg/bragg.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/physical_models/mlayer/mlayer.py` & `shadow4-0.1.8/shadow4/physical_models/mlayer/mlayer.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/physical_models/prerefl/prerefl.py` & `shadow4-0.1.8/shadow4/physical_models/prerefl/prerefl.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/bending_magnet/s4_bending_magnet.py` & `shadow4-0.1.8/shadow4/sources/bending_magnet/s4_bending_magnet.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/bending_magnet/s4_bending_magnet_light_source.py` & `shadow4-0.1.8/shadow4/sources/bending_magnet/s4_bending_magnet_light_source.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/s4_electron_beam.py` & `shadow4-0.1.8/shadow4/sources/s4_electron_beam.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/s4_light_source.py` & `shadow4-0.1.8/shadow4/sources/s4_light_source.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/source_geometrical/probability_distributions.py` & `shadow4-0.1.8/shadow4/sources/source_geometrical/probability_distributions.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/source_geometrical/source_gaussian.py` & `shadow4-0.1.8/shadow4/sources/source_geometrical/source_gaussian.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/source_geometrical/source_geometrical.py` & `shadow4-0.1.8/shadow4/sources/source_geometrical/source_geometrical.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/source_geometrical/source_grid_cartesian.py` & `shadow4-0.1.8/shadow4/sources/source_geometrical/source_grid_cartesian.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/source_geometrical/source_grid_polar.py` & `shadow4-0.1.8/shadow4/sources/source_geometrical/source_grid_polar.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/undulator/s4_undulator.py` & `shadow4-0.1.8/shadow4/sources/undulator/s4_undulator.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/undulator/s4_undulator_light_source.py` & `shadow4-0.1.8/shadow4/sources/undulator/s4_undulator_light_source.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/undulator/source_undulator_factory.py` & `shadow4-0.1.8/shadow4/sources/undulator/source_undulator_factory.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/undulator/source_undulator_factory_pysru.py` & `shadow4-0.1.8/shadow4/sources/undulator/source_undulator_factory_pysru.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/undulator/source_undulator_factory_srw.py` & `shadow4-0.1.8/shadow4/sources/undulator/source_undulator_factory_srw.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/undulator/source_undulator_input_output.py` & `shadow4-0.1.8/shadow4/sources/undulator/source_undulator_input_output.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/wiggler/s4_wiggler.py` & `shadow4-0.1.8/shadow4/sources/wiggler/s4_wiggler.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/sources/wiggler/s4_wiggler_light_source.py` & `shadow4-0.1.8/shadow4/sources/wiggler/s4_wiggler_light_source.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/tools/arrayofvectors.py` & `shadow4-0.1.8/shadow4/tools/arrayofvectors.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4/tools/graphics.py` & `shadow4-0.1.8/shadow4/tools/graphics.py`

 * *Files identical despite different names*

### Comparing `shadow4-0.1.7/shadow4.egg-info/SOURCES.txt` & `shadow4-0.1.8/shadow4.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -73,10 +73,22 @@
 shadow4/sources/undulator/source_undulator_factory.py
 shadow4/sources/undulator/source_undulator_factory_pysru.py
 shadow4/sources/undulator/source_undulator_factory_srw.py
 shadow4/sources/undulator/source_undulator_input_output.py
 shadow4/sources/wiggler/__init__.py
 shadow4/sources/wiggler/s4_wiggler.py
 shadow4/sources/wiggler/s4_wiggler_light_source.py
+shadow4/syned/__init__.py
+shadow4/syned/beamline_element.py
+shadow4/syned/element_coordinates.py
+shadow4/syned/shape.py
+shadow4/syned/absorbers/__init__.py
+shadow4/syned/absorbers/absorber.py
+shadow4/syned/absorbers/beam_stopper.py
+shadow4/syned/absorbers/filter.py
+shadow4/syned/absorbers/holed_filter.py
+shadow4/syned/absorbers/slit.py
+shadow4/syned/refractors/__init__.py
+shadow4/syned/refractors/interface.py
 shadow4/tools/__init__.py
 shadow4/tools/arrayofvectors.py
 shadow4/tools/graphics.py
```

