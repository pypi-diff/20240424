# Comparing `tmp/intake-2.0.3.tar.gz` & `tmp/intake-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-2.0.3.tar", last modified: Mon Feb 26 21:16:29 2024, max compression
+gzip compressed data, was "intake-2.0.4.tar", last modified: Tue Mar 19 18:16:09 2024, max compression
```

## Comparing `intake-2.0.3.tar` & `intake-2.0.4.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.575656 intake-2.0.3/
--rw-r--r--   0 mdurant    (502) staff       (20)       37 2022-09-18 01:28:48.000000 intake-2.0.3/.ci-coveragerc
--rw-r--r--   0 mdurant    (502) staff       (20)      109 2022-09-18 01:28:48.000000 intake-2.0.3/.coveragerc
--rw-r--r--   0 mdurant    (502) staff       (20)       32 2022-09-18 01:28:48.000000 intake-2.0.3/.gitattributes
--rw-r--r--   0 mdurant    (502) staff       (20)     1250 2024-02-08 15:07:13.000000 intake-2.0.3/.gitignore
--rw-r--r--   0 mdurant    (502) staff       (20)     1286 2022-09-18 01:28:48.000000 intake-2.0.3/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      119 2024-02-12 18:20:48.000000 intake-2.0.3/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     2376 2024-02-26 21:16:29.575324 intake-2.0.3/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1864 2024-02-05 18:55:18.000000 intake-2.0.3/README.md
--rw-r--r--   0 mdurant    (502) staff       (20)     6671 2024-02-05 18:55:18.000000 intake-2.0.3/README_refactor.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.561041 intake-2.0.3/intake/
--rw-r--r--   0 mdurant    (502) staff       (20)     6664 2024-02-26 21:01:11.000000 intake-2.0.3/intake/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      411 2024-02-26 21:16:29.000000 intake-2.0.3/intake/_version.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.563313 intake-2.0.3/intake/catalog/
--rw-r--r--   0 mdurant    (502) staff       (20)      875 2024-02-05 18:55:18.000000 intake-2.0.3/intake/catalog/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    17743 2024-02-05 18:55:18.000000 intake-2.0.3/intake/catalog/base.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3132 2023-11-23 21:31:02.000000 intake-2.0.3/intake/catalog/default.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4009 2024-02-05 18:55:18.000000 intake-2.0.3/intake/catalog/entry.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2514 2023-11-23 21:31:02.000000 intake-2.0.3/intake/catalog/exceptions.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1076 2024-02-05 18:55:18.000000 intake-2.0.3/intake/catalog/gui.py
--rw-r--r--   0 mdurant    (502) staff       (20)    34086 2024-02-22 22:00:49.000000 intake-2.0.3/intake/catalog/local.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.564260 intake-2.0.3/intake/catalog/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-23 21:31:02.000000 intake-2.0.3/intake/catalog/tests/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.556581 intake-2.0.3/intake/catalog/tests/catalog_search/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.556745 intake-2.0.3/intake/catalog/tests/catalog_search/example_packages/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.564437 intake-2.0.3/intake/catalog/tests/catalog_search/example_packages/ep/
--rw-r--r--   0 mdurant    (502) staff       (20)       27 2023-11-06 15:45:12.000000 intake-2.0.3/intake/catalog/tests/catalog_search/example_packages/ep/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.564620 intake-2.0.3/intake/catalog/tests/catalog_search/example_packages/ep-0.1.dist-info/
--rw-r--r--   0 mdurant    (502) staff       (20)       39 2022-09-18 01:28:48.000000 intake-2.0.3/intake/catalog/tests/catalog_search/example_packages/ep-0.1.dist-info/entry_points.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      194 2023-11-06 15:45:12.000000 intake-2.0.3/intake/catalog/tests/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)      614 2023-11-23 21:31:02.000000 intake-2.0.3/intake/catalog/tests/example1_source.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.564783 intake-2.0.3/intake/catalog/tests/example_plugin_dir/
--rw-r--r--   0 mdurant    (502) staff       (20)      567 2023-11-23 21:31:02.000000 intake-2.0.3/intake/catalog/tests/example_plugin_dir/example2_source.py
--rw-r--r--   0 mdurant    (502) staff       (20)      928 2022-09-18 01:28:48.000000 intake-2.0.3/intake/catalog/tests/small.npy
--rw-r--r--   0 mdurant    (502) staff       (20)     1015 2023-11-23 21:31:03.000000 intake-2.0.3/intake/catalog/tests/util.py
--rw-r--r--   0 mdurant    (502) staff       (20)    11393 2024-02-05 18:55:18.000000 intake-2.0.3/intake/catalog/utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3307 2024-02-05 18:55:18.000000 intake-2.0.3/intake/catalog/zarr.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5062 2024-02-05 18:55:18.000000 intake-2.0.3/intake/config.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2541 2024-02-05 18:55:18.000000 intake-2.0.3/intake/conftest.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.565072 intake-2.0.3/intake/container/
--rw-r--r--   0 mdurant    (502) staff       (20)       42 2024-02-05 18:55:18.000000 intake-2.0.3/intake/container/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)       68 2024-02-05 18:55:18.000000 intake-2.0.3/intake/container/base.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.566421 intake-2.0.3/intake/interface/
--rw-r--r--   0 mdurant    (502) staff       (20)     1304 2024-02-05 18:55:18.000000 intake-2.0.3/intake/interface/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9051 2024-02-05 18:55:18.000000 intake-2.0.3/intake/interface/base.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.566977 intake-2.0.3/intake/interface/catalog/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-06 15:45:12.000000 intake-2.0.3/intake/interface/catalog/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9406 2024-02-05 18:55:18.000000 intake-2.0.3/intake/interface/catalog/add.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1023 2024-02-05 18:55:18.000000 intake-2.0.3/intake/interface/catalog/search.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7942 2024-02-05 18:55:18.000000 intake-2.0.3/intake/interface/gui.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.567324 intake-2.0.3/intake/interface/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-06 15:45:12.000000 intake-2.0.3/intake/interface/source/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    14604 2024-02-05 18:55:18.000000 intake-2.0.3/intake/interface/source/defined_plots.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.570287 intake-2.0.3/intake/readers/
--rw-r--r--   0 mdurant    (502) staff       (20)     1085 2024-02-26 21:01:11.000000 intake-2.0.3/intake/readers/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    23014 2024-02-26 21:01:11.000000 intake-2.0.3/intake/readers/catalogs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    21959 2024-02-26 21:01:11.000000 intake-2.0.3/intake/readers/convert.py
--rw-r--r--   0 mdurant    (502) staff       (20)    23237 2024-02-26 21:01:11.000000 intake-2.0.3/intake/readers/datatypes.py
--rw-r--r--   0 mdurant    (502) staff       (20)    23761 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/entry.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2600 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/examples.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1964 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/importlist.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1377 2024-02-05 20:05:25.000000 intake-2.0.3/intake/readers/metadata.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6085 2024-02-26 21:01:11.000000 intake-2.0.3/intake/readers/mixins.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2673 2024-02-05 20:05:25.000000 intake-2.0.3/intake/readers/namespaces.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6112 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/output.py
--rw-r--r--   0 mdurant    (502) staff       (20)    43023 2024-02-26 21:01:11.000000 intake-2.0.3/intake/readers/readers.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4099 2024-02-05 20:05:25.000000 intake-2.0.3/intake/readers/search.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.570463 intake-2.0.3/intake/readers/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/tests/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.570608 intake-2.0.3/intake/readers/tests/cats/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/tests/cats/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.557724 intake-2.0.3/intake/readers/tests/cats/stac_data/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.557793 intake-2.0.3/intake/readers/tests/cats/stac_data/1.0.0beta2/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.570752 intake-2.0.3/intake/readers/tests/cats/stac_data/1.0.0beta2/earthsearch/
--rw-r--r--   0 mdurant    (502) staff       (20)      788 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/tests/cats/stac_data/1.0.0beta2/earthsearch/readme.md
--rw-r--r--   0 mdurant    (502) staff       (20)     3356 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/transform.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9114 2024-02-05 18:55:18.000000 intake-2.0.3/intake/readers/user_parameters.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13979 2024-02-26 21:01:11.000000 intake-2.0.3/intake/readers/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.572625 intake-2.0.3/intake/source/
--rw-r--r--   0 mdurant    (502) staff       (20)     2506 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8275 2024-02-07 21:09:13.000000 intake-2.0.3/intake/source/base.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1254 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/csv.py
--rw-r--r--   0 mdurant    (502) staff       (20)    16318 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/derived.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6429 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/discovery.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5489 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/jsonfiles.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1551 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/npy.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.572955 intake-2.0.3/intake/source/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-23 21:31:02.000000 intake-2.0.3/intake/source/tests/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.573296 intake-2.0.3/intake/source/tests/data.zarr/
--rw-r--r--   0 mdurant    (502) staff       (20)      312 2023-02-23 03:44:29.000000 intake-2.0.3/intake/source/tests/data.zarr/.zarray
--rw-r--r--   0 mdurant    (502) staff       (20)       96 2022-09-18 01:28:48.000000 intake-2.0.3/intake/source/tests/data.zarr/0
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.558746 intake-2.0.3/intake/source/tests/plugin_searchpath/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.573466 intake-2.0.3/intake/source/tests/plugin_searchpath/collision_foo/
--rw-r--r--   0 mdurant    (502) staff       (20)      496 2023-11-23 21:31:03.000000 intake-2.0.3/intake/source/tests/plugin_searchpath/collision_foo/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.573638 intake-2.0.3/intake/source/tests/plugin_searchpath/collision_foo2/
--rw-r--r--   0 mdurant    (502) staff       (20)      496 2023-11-23 21:31:02.000000 intake-2.0.3/intake/source/tests/plugin_searchpath/collision_foo2/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.573806 intake-2.0.3/intake/source/tests/plugin_searchpath/driver_with_entrypoints/
--rw-r--r--   0 mdurant    (502) staff       (20)       30 2023-11-06 15:45:12.000000 intake-2.0.3/intake/source/tests/plugin_searchpath/driver_with_entrypoints/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.573994 intake-2.0.3/intake/source/tests/plugin_searchpath/driver_with_entrypoints-0.1.dist-info/
--rw-r--r--   0 mdurant    (502) staff       (20)       75 2022-09-18 01:28:48.000000 intake-2.0.3/intake/source/tests/plugin_searchpath/driver_with_entrypoints-0.1.dist-info/entry_points.txt
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.574189 intake-2.0.3/intake/source/tests/plugin_searchpath/intake_foo/
--rw-r--r--   0 mdurant    (502) staff       (20)      544 2023-11-23 21:31:02.000000 intake-2.0.3/intake/source/tests/plugin_searchpath/intake_foo/__init__.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.574360 intake-2.0.3/intake/source/tests/plugin_searchpath/not_intake_foo/
--rw-r--r--   0 mdurant    (502) staff       (20)      549 2023-11-23 21:31:02.000000 intake-2.0.3/intake/source/tests/plugin_searchpath/not_intake_foo/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1019 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/tests/util.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3026 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/textfiles.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4495 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/tiled.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7698 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1800 2024-02-05 18:55:18.000000 intake-2.0.3/intake/source/zarr.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.574530 intake-2.0.3/intake/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-23 21:31:02.000000 intake-2.0.3/intake/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      763 2024-02-05 18:55:18.000000 intake-2.0.3/intake/util_tests.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9999 2024-02-05 18:55:18.000000 intake-2.0.3/intake/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-02-26 21:16:29.574892 intake-2.0.3/intake.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     2376 2024-02-26 21:16:29.000000 intake-2.0.3/intake.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     2732 2024-02-26 21:16:29.000000 intake-2.0.3/intake.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-02-26 21:16:29.000000 intake-2.0.3/intake.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-02-08 21:13:17.000000 intake-2.0.3/intake.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)       32 2024-02-26 21:16:29.000000 intake-2.0.3/intake.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        7 2024-02-26 21:16:29.000000 intake-2.0.3/intake.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)     1246 2024-02-12 18:20:48.000000 intake-2.0.3/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)       38 2024-02-26 21:16:29.575735 intake-2.0.3/setup.cfg
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.455016 intake-2.0.4/
+-rw-r--r--   0 mdurant    (502) staff       (20)       37 2022-09-18 01:28:48.000000 intake-2.0.4/.ci-coveragerc
+-rw-r--r--   0 mdurant    (502) staff       (20)      109 2022-09-18 01:28:48.000000 intake-2.0.4/.coveragerc
+-rw-r--r--   0 mdurant    (502) staff       (20)       32 2022-09-18 01:28:48.000000 intake-2.0.4/.gitattributes
+-rw-r--r--   0 mdurant    (502) staff       (20)     1250 2024-03-06 15:49:20.000000 intake-2.0.4/.gitignore
+-rw-r--r--   0 mdurant    (502) staff       (20)     1286 2022-09-18 01:28:48.000000 intake-2.0.4/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      119 2024-03-06 15:49:20.000000 intake-2.0.4/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     2376 2024-03-19 18:16:09.454748 intake-2.0.4/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1864 2024-03-06 15:49:20.000000 intake-2.0.4/README.md
+-rw-r--r--   0 mdurant    (502) staff       (20)     6671 2024-03-06 15:49:20.000000 intake-2.0.4/README_refactor.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.435085 intake-2.0.4/intake/
+-rw-r--r--   0 mdurant    (502) staff       (20)     6664 2024-03-06 15:49:20.000000 intake-2.0.4/intake/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      411 2024-03-19 18:16:09.000000 intake-2.0.4/intake/_version.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.438854 intake-2.0.4/intake/catalog/
+-rw-r--r--   0 mdurant    (502) staff       (20)      875 2024-03-06 15:49:20.000000 intake-2.0.4/intake/catalog/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    17743 2024-03-06 15:49:20.000000 intake-2.0.4/intake/catalog/base.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3132 2023-11-23 21:31:02.000000 intake-2.0.4/intake/catalog/default.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4009 2024-03-06 15:49:20.000000 intake-2.0.4/intake/catalog/entry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2514 2023-11-23 21:31:02.000000 intake-2.0.4/intake/catalog/exceptions.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1076 2024-03-06 15:49:20.000000 intake-2.0.4/intake/catalog/gui.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    34219 2024-03-06 15:56:47.000000 intake-2.0.4/intake/catalog/local.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.440298 intake-2.0.4/intake/catalog/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-23 21:31:02.000000 intake-2.0.4/intake/catalog/tests/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.428325 intake-2.0.4/intake/catalog/tests/catalog_search/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.428511 intake-2.0.4/intake/catalog/tests/catalog_search/example_packages/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.440635 intake-2.0.4/intake/catalog/tests/catalog_search/example_packages/ep/
+-rw-r--r--   0 mdurant    (502) staff       (20)       27 2023-11-06 15:45:12.000000 intake-2.0.4/intake/catalog/tests/catalog_search/example_packages/ep/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.440945 intake-2.0.4/intake/catalog/tests/catalog_search/example_packages/ep-0.1.dist-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)       39 2022-09-18 01:28:48.000000 intake-2.0.4/intake/catalog/tests/catalog_search/example_packages/ep-0.1.dist-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      194 2023-11-06 15:45:12.000000 intake-2.0.4/intake/catalog/tests/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      614 2023-11-23 21:31:02.000000 intake-2.0.4/intake/catalog/tests/example1_source.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.441264 intake-2.0.4/intake/catalog/tests/example_plugin_dir/
+-rw-r--r--   0 mdurant    (502) staff       (20)      567 2023-11-23 21:31:02.000000 intake-2.0.4/intake/catalog/tests/example_plugin_dir/example2_source.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      928 2022-09-18 01:28:48.000000 intake-2.0.4/intake/catalog/tests/small.npy
+-rw-r--r--   0 mdurant    (502) staff       (20)     1015 2023-11-23 21:31:03.000000 intake-2.0.4/intake/catalog/tests/util.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    11393 2024-03-06 15:49:20.000000 intake-2.0.4/intake/catalog/utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3307 2024-03-06 15:49:20.000000 intake-2.0.4/intake/catalog/zarr.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5062 2024-03-06 15:49:20.000000 intake-2.0.4/intake/config.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2541 2024-03-06 15:49:20.000000 intake-2.0.4/intake/conftest.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.441671 intake-2.0.4/intake/container/
+-rw-r--r--   0 mdurant    (502) staff       (20)       42 2024-03-06 15:49:20.000000 intake-2.0.4/intake/container/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)       68 2024-03-06 15:49:20.000000 intake-2.0.4/intake/container/base.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.442455 intake-2.0.4/intake/interface/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1304 2024-03-06 15:49:20.000000 intake-2.0.4/intake/interface/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9051 2024-03-06 15:49:20.000000 intake-2.0.4/intake/interface/base.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.443119 intake-2.0.4/intake/interface/catalog/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-06 15:45:12.000000 intake-2.0.4/intake/interface/catalog/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9406 2024-03-06 15:49:20.000000 intake-2.0.4/intake/interface/catalog/add.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1023 2024-03-06 15:49:20.000000 intake-2.0.4/intake/interface/catalog/search.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7942 2024-03-06 15:49:20.000000 intake-2.0.4/intake/interface/gui.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.443687 intake-2.0.4/intake/interface/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-06 15:45:12.000000 intake-2.0.4/intake/interface/source/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    14604 2024-03-06 15:49:20.000000 intake-2.0.4/intake/interface/source/defined_plots.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.447821 intake-2.0.4/intake/readers/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1085 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    23391 2024-03-06 15:56:47.000000 intake-2.0.4/intake/readers/catalogs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    21995 2024-03-06 15:56:47.000000 intake-2.0.4/intake/readers/convert.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    23303 2024-03-06 15:56:47.000000 intake-2.0.4/intake/readers/datatypes.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    23761 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/entry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2600 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/examples.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1964 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/importlist.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1377 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/metadata.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6085 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/mixins.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2673 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/namespaces.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6112 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/output.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    43043 2024-03-06 15:56:47.000000 intake-2.0.4/intake/readers/readers.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4099 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/search.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.448061 intake-2.0.4/intake/readers/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/tests/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.448206 intake-2.0.4/intake/readers/tests/cats/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/tests/cats/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.429595 intake-2.0.4/intake/readers/tests/cats/stac_data/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.429669 intake-2.0.4/intake/readers/tests/cats/stac_data/1.0.0beta2/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.448352 intake-2.0.4/intake/readers/tests/cats/stac_data/1.0.0beta2/earthsearch/
+-rw-r--r--   0 mdurant    (502) staff       (20)      788 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/tests/cats/stac_data/1.0.0beta2/earthsearch/readme.md
+-rw-r--r--   0 mdurant    (502) staff       (20)     3356 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/transform.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9114 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/user_parameters.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13979 2024-03-06 15:49:20.000000 intake-2.0.4/intake/readers/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.450938 intake-2.0.4/intake/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2506 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8275 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/base.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1254 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/csv.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    16318 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/derived.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6429 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/discovery.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5489 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/jsonfiles.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1551 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/npy.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.451522 intake-2.0.4/intake/source/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-23 21:31:02.000000 intake-2.0.4/intake/source/tests/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.452027 intake-2.0.4/intake/source/tests/data.zarr/
+-rw-r--r--   0 mdurant    (502) staff       (20)      312 2023-02-23 03:44:29.000000 intake-2.0.4/intake/source/tests/data.zarr/.zarray
+-rw-r--r--   0 mdurant    (502) staff       (20)       96 2022-09-18 01:28:48.000000 intake-2.0.4/intake/source/tests/data.zarr/0
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.430705 intake-2.0.4/intake/source/tests/plugin_searchpath/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.452325 intake-2.0.4/intake/source/tests/plugin_searchpath/collision_foo/
+-rw-r--r--   0 mdurant    (502) staff       (20)      496 2023-11-23 21:31:03.000000 intake-2.0.4/intake/source/tests/plugin_searchpath/collision_foo/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.452643 intake-2.0.4/intake/source/tests/plugin_searchpath/collision_foo2/
+-rw-r--r--   0 mdurant    (502) staff       (20)      496 2023-11-23 21:31:02.000000 intake-2.0.4/intake/source/tests/plugin_searchpath/collision_foo2/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.452936 intake-2.0.4/intake/source/tests/plugin_searchpath/driver_with_entrypoints/
+-rw-r--r--   0 mdurant    (502) staff       (20)       30 2023-11-06 15:45:12.000000 intake-2.0.4/intake/source/tests/plugin_searchpath/driver_with_entrypoints/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.453198 intake-2.0.4/intake/source/tests/plugin_searchpath/driver_with_entrypoints-0.1.dist-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)       75 2022-09-18 01:28:48.000000 intake-2.0.4/intake/source/tests/plugin_searchpath/driver_with_entrypoints-0.1.dist-info/entry_points.txt
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.453469 intake-2.0.4/intake/source/tests/plugin_searchpath/intake_foo/
+-rw-r--r--   0 mdurant    (502) staff       (20)      544 2023-11-23 21:31:02.000000 intake-2.0.4/intake/source/tests/plugin_searchpath/intake_foo/__init__.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.453679 intake-2.0.4/intake/source/tests/plugin_searchpath/not_intake_foo/
+-rw-r--r--   0 mdurant    (502) staff       (20)      549 2023-11-23 21:31:02.000000 intake-2.0.4/intake/source/tests/plugin_searchpath/not_intake_foo/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1019 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/tests/util.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3026 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/textfiles.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4495 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/tiled.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7698 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1800 2024-03-06 15:49:20.000000 intake-2.0.4/intake/source/zarr.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.453894 intake-2.0.4/intake/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)      328 2023-11-23 21:31:02.000000 intake-2.0.4/intake/tests/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      763 2024-03-06 15:49:20.000000 intake-2.0.4/intake/util_tests.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9999 2024-03-06 15:49:20.000000 intake-2.0.4/intake/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-19 18:16:09.454307 intake-2.0.4/intake.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2376 2024-03-19 18:16:09.000000 intake-2.0.4/intake.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     2765 2024-03-19 18:16:09.000000 intake-2.0.4/intake.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-03-19 18:16:09.000000 intake-2.0.4/intake.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      277 2024-03-19 18:16:09.000000 intake-2.0.4/intake.egg-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-02-08 21:13:17.000000 intake-2.0.4/intake.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)       32 2024-03-19 18:16:09.000000 intake-2.0.4/intake.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        7 2024-03-19 18:16:09.000000 intake-2.0.4/intake.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)     1559 2024-03-06 15:56:47.000000 intake-2.0.4/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)       38 2024-03-19 18:16:09.455926 intake-2.0.4/setup.cfg
```

### Comparing `intake-2.0.3/.gitignore` & `intake-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/LICENSE` & `intake-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/PKG-INFO` & `intake-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake
-Version: 2.0.3
+Version: 2.0.4
 Summary: Data catalog, search and load
 Author-email: Martin Durant <martin.durant@alumni.utoronto.ca>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `intake-2.0.3/README.md` & `intake-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/README_refactor.md` & `intake-2.0.4/README_refactor.md`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/__init__.py` & `intake-2.0.4/intake/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/__init__.py` & `intake-2.0.4/intake/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/base.py` & `intake-2.0.4/intake/catalog/base.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/default.py` & `intake-2.0.4/intake/catalog/default.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/entry.py` & `intake-2.0.4/intake/catalog/entry.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/exceptions.py` & `intake-2.0.4/intake/catalog/exceptions.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/gui.py` & `intake-2.0.4/intake/catalog/gui.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/local.py` & `intake-2.0.4/intake/catalog/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,14 +390,18 @@
                 self.error(
                     "value in list of plugins sources must be a " "dictionary",
                     data["plugins"],
                     "source",
                 )
                 continue
 
+            elif "module" in plugin_source:
+                import intake
+
+                intake.import_name(plugin_source["module"])
             elif "dir" in plugin_source:
                 self.error(
                     "The key 'dir', and in general the feature of registering "
                     "plugins from a directory of Python scripts outside of "
                     "sys.path, is no longer supported. Use 'module'.",
                     plugin_source,
                 )
@@ -551,15 +555,15 @@
         return sources
 
     def _parse(self, data):
         if not isinstance(data, dict):
             self.error("catalog must be a dictionary", data)
             return
         if (data.get("version", None) or data.get("metadata", {}).get("version", None) or 1) > 1:
-            raise VersionError("Not a V1 Catalog; perhaps use intake.from_yaml_file")
+            raise VersionError("Not a V1 Catalog; perhaps use intake.open_catalog")
 
         return dict(
             plugin_sources=self._parse_plugins(data),
             data_sources=self._parse_data_sources(data),
             metadata=data.get("metadata", {}),
             name=data.get("name"),
             description=data.get("description"),
```

### Comparing `intake-2.0.3/intake/catalog/tests/example1_source.py` & `intake-2.0.4/intake/catalog/tests/example1_source.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/tests/example_plugin_dir/example2_source.py` & `intake-2.0.4/intake/catalog/tests/example_plugin_dir/example2_source.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/tests/small.npy` & `intake-2.0.4/intake/catalog/tests/small.npy`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/tests/util.py` & `intake-2.0.4/intake/catalog/tests/util.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/utils.py` & `intake-2.0.4/intake/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/catalog/zarr.py` & `intake-2.0.4/intake/catalog/zarr.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/config.py` & `intake-2.0.4/intake/config.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/conftest.py` & `intake-2.0.4/intake/conftest.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/interface/__init__.py` & `intake-2.0.4/intake/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/interface/base.py` & `intake-2.0.4/intake/interface/base.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/interface/catalog/add.py` & `intake-2.0.4/intake/interface/catalog/add.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/interface/catalog/search.py` & `intake-2.0.4/intake/interface/catalog/search.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/interface/gui.py` & `intake-2.0.4/intake/interface/gui.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/interface/source/defined_plots.py` & `intake-2.0.4/intake/interface/source/defined_plots.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/__init__.py` & `intake-2.0.4/intake/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/catalogs.py` & `intake-2.0.4/intake/readers/catalogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,31 +138,31 @@
         if isinstance(data, datatypes.JSONFile):
             self._stac = cls.from_file(data.url)
         else:
             self._stac = cls.from_dict(data.data)
         metadata = self._stac.to_dict()
         metadata.pop("links", None)
         self.metadata.update(metadata)
-        import pystac
-
         cat = Catalog(metadata=self.metadata)
         items = []
 
         # the following can be slow and could be deferred to lazy entries, if we can get
         # the names without details cheaply
         if isinstance(self._stac, pystac.Catalog):
             items = itertools.chain(self._stac.get_children(), self._stac.get_items())
         elif isinstance(self._stac, pystac.ItemCollection):
             items = self._stac.items
         if hasattr(self._stac, "assets"):
             for key, value in self._stac.assets.items():
                 if signer:
                     signer(value)
                 try:
-                    reader = self._get_reader(value, signer=signer, prefer=prefer).to_entry()
+                    reader = self._get_reader(
+                        value, signer=signer, prefer=prefer, metadata=self.metadata
+                    ).to_entry()
                     cat[key] = reader
                 except (ValueError, TypeError, StopIteration):
                     pass
 
         for subcatalog in items:
             subcls = type(subcatalog).__name__
 
@@ -173,19 +173,20 @@
                         "cls": subcls,
                         "data": datatypes.Literal(subcatalog.to_dict()),
                         "signer": signer,
                         "prefer": prefer,
                     },
                     **kwargs,
                 ),
+                metadata=self.metadata,
             )
         return cat
 
     @staticmethod
-    def _get_reader(asset, signer=None, prefer=None):
+    def _get_reader(asset, signer=None, prefer=None, metadata=None):
         """
         Assign intake driver for data I/O
 
         prefer: str | list[str]
             passed to .to_reader to inform what class of reader would be preferable, if any
         """
         url = asset.href
@@ -209,29 +210,29 @@
             from intake.readers.readers import DaskGeoParquet
 
             data.metadata["signer"] = signer
             data.metadata["prefer"] = prefer
             return DaskGeoParquet(data)
         else:
             rr = None
-        return data.to_reader(reader=rr, outtype=prefer)
+        return data.to_reader(reader=rr, outtype=prefer, metadata=metadata)
 
 
 class StackBands(BaseReader):
     """Reimplementation of "StackBandsSource" from intake-stac
 
     Takes the subitems of a given collection and concatenates them using xarray
     on the given dimension.
     """
 
     implements = {datatypes.STACJSON, datatypes.Literal}
     imports = {"pystac", "xarray"}
-    output_instance = "intake.readers.readers:XarrayReader"
+    output_instance = "xarray:Dataset"
 
-    def _read(self, data, bands: list[str], concat_dim: str = "band", **kw):
+    def _read(self, data, bands: list[str], concat_dim: str = "band", signer=None, **kw):
         """
         Parameters
         ----------
         data:
             STAC endpoint, file, or dict literal
         bands:
             band_id, name or common_name to select from contained items
@@ -248,30 +249,39 @@
         from pystac.extensions.eo import EOExtension
 
         cls = pystac.Item
         if isinstance(data, datatypes.JSONFile):
             self._stac = cls.from_file(data.url)
         else:
             self._stac = cls.from_dict(data.data)
+        if signer:
+            signer(self._stac)
 
         band_info = [band.to_dict() for band in EOExtension.ext(self._stac).bands]
         metadatas = {}
         titles = []
         hrefs = []
         types = []
         assets = self._stac.assets
         for band in bands:
             # band can be band id, name or common_name
             if band in assets:
                 info = next(
-                    (b for b in band_info if b.get("id", b.get("name")) == band),
+                    (
+                        b
+                        for b in band_info
+                        if band in [b.get(_) for _ in ["common_name", "name", "id"]]
+                    ),
                     None,
                 )
             else:
-                info = next((b for b in band_info if b.get("common_name") == band), None)
+                info = next(
+                    (b for b in band_info if band in [b.get(_) for _ in ["common_name", "name"]]),
+                    None,
+                )
                 if info is not None:
                     band = info.get("id", info.get("name"))
 
             if band not in assets or info is None:
                 valid_band_names = []
                 for b in band_info:
                     valid_band_names.append(b.get("id", b.get("name")))
@@ -287,19 +297,19 @@
             hrefs.append(asset.href)
 
         unique_types = set(types)
         if len(unique_types) != 1:
             raise ValueError(
                 f"Stacking failed: bands must have same type, multiple found: {unique_types}"
             )
-        reader = StacCatalogReader._get_reader(asset)
-        reader.kwargs["concat_dim"] = concat_dim
+        reader = StacCatalogReader._get_reader(asset, signer=signer)
+        reader.kwargs["dim"] = concat_dim
         reader.kwargs["data"].url = hrefs
         reader.kwargs.update(kw)
-        return reader
+        return reader.read()
 
 
 class StacSearch(BaseReader):
     """
     Get stac objects matching a search spec from a STAC endpoint
     """
```

### Comparing `intake-2.0.3/intake/readers/convert.py` & `intake-2.0.4/intake/readers/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,14 +297,15 @@
         stac = stac_geoparquet.stac_geoparquet.to_item_collection(data)
         lit = Literal(stac.to_dict())
         return StacCatalogReader(
             lit,
             signer=self.metadata.get("signer"),
             prefer=self.metadata.get("prefer"),
             cls="ItemCollection",
+            metadata=self.metadata,
         ).read()
 
 
 class PandasToMetagraph(BaseConverter):
     instances = {"pd:DataFrame": "metagraph.wrappers.EdgeSet:PandasEdgeSet"}
     func = "metagraph.wrappers.EdgeSet:PandasEdgeSet"
```

### Comparing `intake-2.0.3/intake/readers/datatypes.py` & `intake-2.0.4/intake/readers/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,14 +673,15 @@
 
 
 comp_magic = {
     # These are a bit like datatypes making raw bytes/file object output
     (0, b"\x1f\x8b"): "gzip",
     (0, b"BZh"): "bzip2",
     (0, b"(\xc2\xb5/\xc3\xbd"): "zstd",
+    (0, b"\xff\x06\x00\x00sNaPpY"): "sz",  # stream framed format
 }
 container_magic = {
     # these are like datatypes making filesystems
     (257, b"ustar"): "tar",
     (0, b"PK"): "zip",
 }
```

### Comparing `intake-2.0.3/intake/readers/entry.py` & `intake-2.0.4/intake/readers/entry.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/examples.py` & `intake-2.0.4/intake/readers/examples.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/importlist.py` & `intake-2.0.4/intake/readers/importlist.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/metadata.py` & `intake-2.0.4/intake/readers/metadata.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/mixins.py` & `intake-2.0.4/intake/readers/mixins.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/namespaces.py` & `intake-2.0.4/intake/readers/namespaces.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/output.py` & `intake-2.0.4/intake/readers/output.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/readers.py` & `intake-2.0.4/intake/readers/readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             data = args[0]
         if not isinstance(data, datatypes.BaseData):
             raise ValueError("Data argument isn't a BaseData")
         return data
 
     def to_reader(self, outtype: tuple[str] | str | None = None, reader: str | None = None, **kw):
         """Make a different reader for the data used by this reader"""
-        return self.data.to_reader(outtype=outtype, reader=reader, **kw)
+        return self.data.to_reader(outtype=outtype, reader=reader, metadata=self.metadata, **kw)
 
     def auto_pipeline(self, outtype: str | tuple[str], avoid: list[str] | None = None):
         from intake import auto_pipeline
 
         return auto_pipeline(self, outtype=outtype, avoid=avoid)
 
 
@@ -1010,16 +1010,16 @@
 
         concat_kwargs = concat_kwargs or {
             k: kwargs.pop(k)
             for k in {"dim", "data_vars", "coords", "compat", "position", "join"}
             if k in kwargs
         }
 
-        with fsspec.open_files(data.url, **(data.storage_options or {})) as ofs:
-            bits = [open_rasterio(of, **kwargs) for of in ofs]
+        ofs = fsspec.open_files(data.url, **(data.storage_options or {}))
+        bits = [open_rasterio(of.open(), **kwargs) for of in ofs]
         if len(bits) == 1:
             return bits
         else:
             # requires dim= in kwargs
             return xr.concat(bits, **concat_kwargs)
```

### Comparing `intake-2.0.3/intake/readers/search.py` & `intake-2.0.4/intake/readers/search.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/tests/cats/stac_data/1.0.0beta2/earthsearch/readme.md` & `intake-2.0.4/intake/readers/tests/cats/stac_data/1.0.0beta2/earthsearch/readme.md`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/transform.py` & `intake-2.0.4/intake/readers/transform.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/user_parameters.py` & `intake-2.0.4/intake/readers/user_parameters.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/readers/utils.py` & `intake-2.0.4/intake/readers/utils.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/__init__.py` & `intake-2.0.4/intake/source/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/base.py` & `intake-2.0.4/intake/source/base.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/csv.py` & `intake-2.0.4/intake/source/csv.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/derived.py` & `intake-2.0.4/intake/source/derived.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/discovery.py` & `intake-2.0.4/intake/source/discovery.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/jsonfiles.py` & `intake-2.0.4/intake/source/jsonfiles.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/npy.py` & `intake-2.0.4/intake/source/npy.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/tests/plugin_searchpath/intake_foo/__init__.py` & `intake-2.0.4/intake/source/tests/plugin_searchpath/intake_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/tests/plugin_searchpath/not_intake_foo/__init__.py` & `intake-2.0.4/intake/source/tests/plugin_searchpath/not_intake_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/tests/util.py` & `intake-2.0.4/intake/source/tests/util.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/textfiles.py` & `intake-2.0.4/intake/source/textfiles.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/tiled.py` & `intake-2.0.4/intake/source/tiled.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/utils.py` & `intake-2.0.4/intake/source/utils.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/source/zarr.py` & `intake-2.0.4/intake/source/zarr.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/util_tests.py` & `intake-2.0.4/intake/util_tests.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake/utils.py` & `intake-2.0.4/intake/utils.py`

 * *Files identical despite different names*

### Comparing `intake-2.0.3/intake.egg-info/PKG-INFO` & `intake-2.0.4/intake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake
-Version: 2.0.3
+Version: 2.0.4
 Summary: Data catalog, search and load
 Author-email: Martin Durant <martin.durant@alumni.utoronto.ca>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `intake-2.0.3/intake.egg-info/SOURCES.txt` & `intake-2.0.4/intake.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 intake/config.py
 intake/conftest.py
 intake/util_tests.py
 intake/utils.py
 intake.egg-info/PKG-INFO
 intake.egg-info/SOURCES.txt
 intake.egg-info/dependency_links.txt
+intake.egg-info/entry_points.txt
 intake.egg-info/not-zip-safe
 intake.egg-info/requires.txt
 intake.egg-info/top_level.txt
 intake/catalog/__init__.py
 intake/catalog/base.py
 intake/catalog/default.py
 intake/catalog/entry.py
```

