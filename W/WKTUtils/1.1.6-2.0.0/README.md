# Comparing `tmp/WKTUtils-1.1.6.tar.gz` & `tmp/wktutils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WKTUtils-1.1.6.tar", last modified: Wed Aug 31 23:11:03 2022, max compression
+gzip compressed data, was "wktutils-2.0.0.tar", last modified: Wed Apr 24 18:41:20 2024, max compression
```

## Comparing `WKTUtils-1.1.6.tar` & `wktutils-2.0.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.685394 WKTUtils-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.665394 WKTUtils-1.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.665394 WKTUtils-1.1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.665394 WKTUtils-1.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/workflows/auto-merge-nonprod.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4369 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/workflows/auto-merge-prod.yml
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/workflows/label-prod-pr.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/workflows/prod-request-merged.yml
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-08-31 23:11:03.685394 WKTUtils-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.669394 WKTUtils-1.1.6/WKTUtils/
--rw-r--r--   0 runner    (1001) docker     (121)     9435 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/WKTUtils/FilesToWKT.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/WKTUtils/Input.py
--rw-r--r--   0 runner    (1001) docker     (121)    27682 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/WKTUtils/RepairWKT.py
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/WKTUtils/ValidateWKT.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/WKTUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4129 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/WKTUtils/asf_env.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.669394 WKTUtils-1.1.6/WKTUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-08-31 23:11:03.000000 WKTUtils-1.1.6/WKTUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-08-31 23:11:03.000000 WKTUtils-1.1.6/WKTUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-31 23:11:03.000000 WKTUtils-1.1.6/WKTUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-08-31 23:11:03.000000 WKTUtils-1.1.6/WKTUtils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-31 23:11:03.000000 WKTUtils-1.1.6/WKTUtils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-31 23:11:03.685394 WKTUtils-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.677394 WKTUtils-1.1.6/yml_tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.661394 WKTUtils-1.1.6/yml_tests/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.677394 WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/
--rw-r--r--   0 runner    (1001) docker     (121)    18716 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/AoI.geojson
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/Basic_FC_GC_1.geojson
--rw-r--r--   0 runner    (1001) docker     (121)    28126 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/ManyCoords_ShovelCreek.geojson
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/Multi-FC_Multi-GC_1.geojson
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/SmallestJson_1.geojson
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.681394 WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/BillionLaughs.kml
--rw-r--r--   0 runner    (1001) docker     (121)   292712 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/Blowup.kml
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/LocalEntityExpansion.kml
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/RemoteEntityExpansion.kml
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/RetrieveDTD.kml
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/XSLTransformation.kml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/emptyfile.kml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.681394 WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/3D_coords.kml
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/Iceland1.kml
--rw-r--r--   0 runner    (1001) docker     (121)     5099 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/Polygon_point_line.kml
--rw-r--r--   0 runner    (1001) docker     (121)   403351 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/asf-datapool-results-2019-10-01_10-29-15.kml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.681394 WKTUtils-1.1.6/yml_tests/Resources/shps_valid/
--rw-r--r--   0 runner    (1001) docker     (121)   550344 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/shps_valid/Fires-all_region_region.zip
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/shps_valid/NED1_F.shp
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/shps_valid/NED2_M.shp
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/shps_valid/PIGSearch.shp
--rw-r--r--   0 runner    (1001) docker     (121)   600436 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/shps_valid/ShorelineMask26.shp
--rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/shps_valid/UTM_7N.zip
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/shps_valid/Unknown_CRS_shapeset.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.681394 WKTUtils-1.1.6/yml_tests/Resources/zips_invalid/
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/zips_invalid/DoubleCompressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-31 23:11:03.685394 WKTUtils-1.1.6/yml_tests/Resources/zips_valid/
--rw-r--r--   0 runner    (1001) docker     (121)   486234 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/zips_valid/MultiShp_SingleGeo_WithDir.zip
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/zips_valid/NED1_F.zip
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/Resources/zips_valid/OneBad_TwoGood.zip
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/pytest-config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/pytest-managers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3860 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/test_filesToWKT.py
--rw-r--r--   0 runner    (1001) docker     (121) 10810065 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/test_filesToWKT.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4666 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/test_repairWKT.py
--rw-r--r--   0 runner    (1001) docker     (121)   100187 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/test_repairWKT.yml
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/test_validateWKT.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-31 23:10:48.000000 WKTUtils-1.1.6/yml_tests/test_validateWKT.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.652731 wktutils-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.624731 wktutils-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.628731 wktutils-2.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.628731 wktutils-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/workflows/auto-merge-nonprod.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/workflows/auto-merge-prod.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/workflows/label-prod-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/workflows/prod-request-merged.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-24 18:41:12.000000 wktutils-2.0.0/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-24 18:41:12.000000 wktutils-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-24 18:41:12.000000 wktutils-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-24 18:41:12.000000 wktutils-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 18:41:20.652731 wktutils-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-24 18:41:12.000000 wktutils-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.628731 wktutils-2.0.0/WKTUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-04-24 18:41:12.000000 wktutils-2.0.0/WKTUtils/FilesToWKT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-24 18:41:12.000000 wktutils-2.0.0/WKTUtils/Input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28163 2024-04-24 18:41:12.000000 wktutils-2.0.0/WKTUtils/RepairWKT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-24 18:41:12.000000 wktutils-2.0.0/WKTUtils/ValidateWKT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 18:41:12.000000 wktutils-2.0.0/WKTUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-24 18:41:12.000000 wktutils-2.0.0/WKTUtils/asf_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.648731 wktutils-2.0.0/WKTUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 18:41:20.000000 wktutils-2.0.0/WKTUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-24 18:41:20.000000 wktutils-2.0.0/WKTUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:41:20.000000 wktutils-2.0.0/WKTUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 18:41:20.000000 wktutils-2.0.0/WKTUtils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 18:41:20.000000 wktutils-2.0.0/WKTUtils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-24 18:41:12.000000 wktutils-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-24 18:41:12.000000 wktutils-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:41:20.652731 wktutils-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-24 18:41:12.000000 wktutils-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.644731 wktutils-2.0.0/yml_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.624731 wktutils-2.0.0/yml_tests/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.644731 wktutils-2.0.0/yml_tests/Resources/geojsons_valid/
+-rw-r--r--   0 runner    (1001) docker     (127)    18716 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/geojsons_valid/AoI.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/geojsons_valid/Basic_FC_GC_1.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    28126 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/geojsons_valid/ManyCoords_ShovelCreek.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/geojsons_valid/Multi-FC_Multi-GC_1.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/geojsons_valid/SmallestJson_1.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.644731 wktutils-2.0.0/yml_tests/Resources/kmls_invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_invalid/BillionLaughs.kml
+-rw-r--r--   0 runner    (1001) docker     (127)   292712 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_invalid/Blowup.kml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_invalid/LocalEntityExpansion.kml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_invalid/RemoteEntityExpansion.kml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_invalid/RetrieveDTD.kml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_invalid/XSLTransformation.kml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_invalid/emptyfile.kml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.644731 wktutils-2.0.0/yml_tests/Resources/kmls_valid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_valid/3D_coords.kml
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_valid/Iceland1.kml
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_valid/Polygon_point_line.kml
+-rw-r--r--   0 runner    (1001) docker     (127)   403351 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/kmls_valid/asf-datapool-results-2019-10-01_10-29-15.kml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.648731 wktutils-2.0.0/yml_tests/Resources/shps_valid/
+-rw-r--r--   0 runner    (1001) docker     (127)   550344 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/shps_valid/Fires-all_region_region.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/shps_valid/NED1_F.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/shps_valid/NED2_M.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/shps_valid/PIGSearch.shp
+-rw-r--r--   0 runner    (1001) docker     (127)   600436 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/shps_valid/ShorelineMask26.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/shps_valid/UTM_7N.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/shps_valid/Unknown_CRS_shapeset.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.648731 wktutils-2.0.0/yml_tests/Resources/zips_invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/zips_invalid/DoubleCompressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:20.648731 wktutils-2.0.0/yml_tests/Resources/zips_valid/
+-rw-r--r--   0 runner    (1001) docker     (127)   486234 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/zips_valid/MultiShp_SingleGeo_WithDir.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/zips_valid/NED1_F.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/Resources/zips_valid/OneBad_TwoGood.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/pytest-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/pytest-managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/test_filesToWKT.py
+-rw-r--r--   0 runner    (1001) docker     (127) 10810065 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/test_filesToWKT.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/test_repairWKT.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100186 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/test_repairWKT.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/test_validateWKT.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:41:12.000000 wktutils-2.0.0/yml_tests/test_validateWKT.yml
```

### Comparing `WKTUtils-1.1.6/.github/ISSUE_TEMPLATE/bug_report.md` & `wktutils-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `wktutils-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/.github/workflows/auto-merge-nonprod.yml` & `wktutils-2.0.0/.github/workflows/auto-merge-nonprod.yml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/.github/workflows/auto-merge-prod.yml` & `wktutils-2.0.0/.github/workflows/auto-merge-prod.yml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/.github/workflows/changelog.yml` & `wktutils-2.0.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/.github/workflows/label-prod-pr.yml` & `wktutils-2.0.0/.github/workflows/label-prod-pr.yml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/.github/workflows/prod-request-merged.yml` & `wktutils-2.0.0/.github/workflows/prod-request-merged.yml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/.github/workflows/pypi-publish.yml` & `wktutils-2.0.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/.gitignore` & `wktutils-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/CHANGELOG.md` & `wktutils-2.0.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,28 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [PEP 440](https://www.python.org/dev/peps/pep-0440/) 
 and uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ------
 
+## [2.0.0](https://github.com/asfadmin/Discovery-WKTUtils/compare/v1.1.6...v2.0.0)
+
+### Changed
+- Makes `sklearn` and `requests` optional dependency (required for `RepairWKT.py` functionality). Installable via `python3 -m pip install WKTUtils[extras]`
+
+------
+
+## [1.1.6](https://github.com/asfadmin/Discovery-WKTUtils/compare/v1.1.5...v1.1.6)
+
+### Fixed
+- Fixes clockwise polygon repair failing due to updated CMR error message
+
+------
+
 ## [1.1.5](https://github.com/asfadmin/Discovery-WKTUtils/compare/v1.1.4...v1.1.5)
 
 ### Removed
 - Removed warning, when the 'MATURITY' env var isn't set. Still defaults to 'prod'.
 
 ------
```

### Comparing `WKTUtils-1.1.6/LICENSE` & `wktutils-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/PKG-INFO` & `wktutils-2.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: WKTUtils
-Version: 1.1.6
-Summary: A few WKT utilities for use elsewhere
-Home-page: https://github.com/asfadmin/Discovery-WKTUtils.git
-Author: ASF Discovery Team
-Author-email: uaf-asf-discovery@alaska.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Discovery-WKTUtils
 
 [![image](https://img.shields.io/pypi/v/wktutils.svg)](https://pypi.python.org/pypi/WKTUtils)
 
 ### To Install as Package, add the following line to requirements.txt:
 
 ```bash
@@ -34,8 +20,8 @@
 You must open shapefiles in read binary mode, before passing them into the function.
 
 ```python
 from WKTUtils.FilesToWKT import filesToWKT
 f = open("path/to/file.shp", "rb")
 # NOTE: f can be a list of files too. filesToWKT([f1, f2, ...]).getWKT()
 wkt = filesToWKT(f).getWKT()
-```
+```
```

### Comparing `WKTUtils-1.1.6/WKTUtils/FilesToWKT.py` & `wktutils-2.0.0/WKTUtils/FilesToWKT.py`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/WKTUtils/Input.py` & `wktutils-2.0.0/WKTUtils/Input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import dateparser
-import re
 from geomet import wkt, InvalidGeoJSONException
 
 
 # Parse and validate a date: "1991-10-01T00:00:00Z"
 def parse_date_util(v):
     d = dateparser.parse(v)
     if d is None:
```

### Comparing `WKTUtils-1.1.6/WKTUtils/RepairWKT.py` & `wktutils-2.0.0/WKTUtils/RepairWKT.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,39 @@
+import re
 from .asf_env import get_config
 from .Input import parse_wkt_util
-
 import logging
-import requests
-import shapely.wkt
-import shapely.ops
-import re
 import json
 import pyproj
 import geopandas
 import numpy as np
 import pyproj
 import geopandas
-from geomet import wkt, InvalidGeoJSONException
-from sklearn.neighbors import NearestNeighbors
+from geomet import wkt as geomet_wkt, InvalidGeoJSONException
 from shapely.geometry import Polygon, LineString, Point
+import shapely.wkt
+import shapely.ops
+
+try:
+    import requests
+    from sklearn.neighbors import NearestNeighbors
+except ImportError:
+    requests = None
+    NearestNeighbors = None
+
 
 # Accepts a single wkt string, or a tuple with crs projection
 # (Or a list of the above, mixed)
 # Accepted: wkt_str, (wkt_str,), (wkt_str, crs), [wkt_str, (wkt_str,crs)]
 
 class simplifyWKT():
     def __init__(self, wkt_obj, default_crs="EPSG:4326"):
+        if requests is None or NearestNeighbors is None:
+               raise ImportError(f'Could not find required packages for class "simplifyWKT". Install additional dependencies via pip.\nEx: `python3 -m pip install WKTUtils[extras]`')
+
         self.shapes = []
         self.errors = None
         self.repairs = []
 
         # Make sure you can load the default_crs:
         try:
             default_crs = pyproj.CRS.from_user_input(default_crs)
@@ -77,15 +85,15 @@
         self.regex_digit = r"(-?(((\d+\.\d+|\d+)(e-?\d+)?)|(\d+\.|\.\d+)))"
 
         try:
             # wkt.loads doesn't like 3D/4D tags, BUT it loads the coords just fine:
             # (Needed until https://github.com/geomet/geomet/issues/58 is fixed)
             wkt_str = wkt_str.upper()
             wkt_str = wkt_str.replace(" Z ", " ").replace(" M ", " ").replace(" ZM ", " ")
-            wkt_json = wkt.loads(wkt_str)
+            wkt_json = geomet_wkt.loads(wkt_str)
         except AttributeError as e:
             self.errors = { 'errors': [{'type': 'ATTRIBUTE', 'report': 'Could not parse WKT: {0}.'.format(str(e))}] }
             return
         except (ValueError, InvalidGeoJSONException) as e:
             self.errors = { 'errors': [{'type': 'VALUE', 'report': 'Could not parse WKT: {0}.'.format(str(e))}] }
             return
         except TypeError as e:
@@ -310,44 +318,44 @@
         wkt_shapely = []
         # If you passed it a single geomet.wkt or shapely.wkt:
         if not isinstance(wkt_obj, type([])):
             wkt_obj = [wkt_obj]
         for item in wkt_obj:
             # If a json / geojson:
             if isinstance(item, type({})):
-                wkt_shapely.append(shapely.wkt.loads(wkt.dumps(item)))
+                wkt_shapely.append(shapely.wkt.loads(geomet_wkt.dumps(item)))
             # Else you got it from shapely:
             elif getattr(item, "geom_type", None) != None:
                 converted_from_shapely = True
                 wkt_shapely.append(item)
         # Check for simple case:
         if len(wkt_shapely) == 1 and wkt_shapely[0].geom_type.upper() in ["POINT","MULTIPOINT","LINESTRING","POLYGON"]:
             hulled_shape = wkt_shapely[0].convex_hull
-            return hulled_shape if converted_from_shapely else wkt.loads(shapely.wkt.dumps(hulled_shape))
+            return hulled_shape if converted_from_shapely else geomet_wkt.loads(shapely.wkt.dumps(hulled_shape))
         # Have to merge the coords:
-        wkt_json = [wkt.loads(shapely.wkt.dumps(shape)) for shape in wkt_shapely]
+        wkt_json = [geomet_wkt.loads(shapely.wkt.dumps(shape)) for shape in wkt_shapely]
         all_coords = self.__getAllCoords(wkt_json)
         if len(all_coords) == 0:
             return None
 
         # Convex_hull and add the new shape:
         MultiPoint = {'type': 'MultiPoint', 'coordinates': all_coords }
         # Quicky convert to shapely obj for the convex hull:
-        shape = shapely.wkt.loads(wkt.dumps(MultiPoint)).convex_hull
+        shape = shapely.wkt.loads(geomet_wkt.dumps(MultiPoint)).convex_hull
         # If they passed in a shapely object, return one. Else return a geojson
         if converted_from_shapely:
             return shape
         else:
             # else convert back to geojson:
-            return wkt.loads(shapely.wkt.dumps(shape))
+            return geomet_wkt.loads(shapely.wkt.dumps(shape))
 
     def __jsonToShapely(self, list_of_shapes):
         shapely_shapes = []
         for shape in list_of_shapes:
-            shape = shapely.wkt.loads(wkt.dumps(shape))
+            shape = shapely.wkt.loads(geomet_wkt.dumps(shape))
             shapely_shapes.append(shape)
         return shapely_shapes
 
     # Returns the merge of the shapes IF it could get it down to one,
     # else None otherwise
     def __mergeShapelyList(self, shapely_list):
         # Merge the shape, then apply some repairs:
@@ -373,21 +381,21 @@
         else:
             print("--- UNCHECKED FIX IN MERGE ---")
             print(union)
             return None
 
     # Takes either a list, or single geomet/shapely wkt, and returns a unique list of points:
     def __getAllCoords(self, wkt_obj):
-        if not isinstance(wkt, type([])):
+        if not isinstance(wkt_obj, type([])):
             wkt_obj = [wkt_obj]
 
         for i, single_shape in enumerate(wkt_obj):
             # If the shape is from shapely:
             if getattr(single_shape, "geom_type", None) != None:
-                wkt_obj[i] = wkt.loads(shapely.wkt.dumps(single_shape))
+                wkt_obj[i] = geomet_wkt.loads(shapely.wkt.dumps(single_shape))
 
         match_coords = r'(\[\s*' +self.regex_digit+ r'\s*,\s*' +self.regex_digit+ r'\s*\])'
         coords = re.findall(match_coords, str(wkt_obj))
 
         all_coords = []
         for i in range(len(coords)):
             # Group 0 = "[ 1.0, 1.0 ]" as a literall string. Convert to list of floats:
@@ -415,15 +423,15 @@
         def getJsonWKT(str_type, coords):
             if str_type.upper() == "POLYGON":
                 new_shape = shapely.wkt.dumps(Polygon( coords ))
             elif str_type.upper() == "LINESTRING":
                 new_shape = shapely.wkt.dumps(LineString( coords ))
             elif str_type.upper() == "POINT":
                 new_shape = shapely.wkt.dumps(Point( coords[0] ))
-            return wkt.loads(new_shape)
+            return geomet_wkt.loads(new_shape)
 
         def getClampedCoords(wkt_json):
             # num_coords out of lat +/- 90
             clamped = 0
             new_coords = []
             old_coords = getCoords(wkt_json)
             for i in range(len(old_coords)):
@@ -502,68 +510,68 @@
 
             ## simplifyPoints START
             tolerance = 0.00001
             attempts = 0
             org_num_points = len(getCoords(wkt_json))
             current_num_points = org_num_points
             closest_distance = getClosestPointDist(wkt_json)
-            wkt_shapely = shapely.wkt.loads(wkt.dumps(wkt_json))
+            wkt_shapely = shapely.wkt.loads(geomet_wkt.dumps(wkt_json))
             while (current_num_points > 300 or closest_distance < 0.004) and attempts < 10:
                 # Set the tolerance/closest_distance for the next loop around:
                 logging.debug('The shape\'s length is {0}, simplifying further with tolerance {1}'.format(current_num_points, tolerance ))
                 attempts += 1
                 wkt_shapely = wkt_shapely.simplify(tolerance, preserve_topology=True)
                 tolerance *= 5
-                wkt_json = wkt.loads(shapely.wkt.dumps(wkt_shapely))
+                wkt_json = geomet_wkt.loads(shapely.wkt.dumps(wkt_shapely))
                 current_num_points = len(getCoords(wkt_json))
                 closest_distance = getClosestPointDist(wkt_json)
             # If it couldn't simplify enough:
             # Would add closest_dist check here, but it's unclear *exactly* what that distance is. Just hope CMR accept's it at this point:
             if current_num_points > 300:
                 self.errors = { 'errors': [{'type': 'SIMPLIFY', 'report': 'Could not simplify {0} past 300 points. (Got from {1}, to {2})'.format(wkt_shapely.geom_type, org_num_points, current_num_points)}] }
                 return
             if attempts > 0:
                 self.repairs.append({
                     'type': 'SIMPLIFY',
                     'report': 'Simplified shape from {0} points to {1} points, after {2} iterations.'.format(org_num_points, current_num_points, attempts)
                 })
                 logging.debug(self.repairs[-1])
-            return wkt.loads(shapely.wkt.dumps(wkt_shapely))
+            return geomet_wkt.loads(shapely.wkt.dumps(wkt_shapely))
 
         ## REPAIR MERGED WKT START:
         # Quick sanity check. No clue if it's actually possible to hit this:
         if single_wkt.geom_type.upper() not in ["POLYGON", "LINESTRING", "POINT"]:
             self.errors = {'errors': [{'type': 'VALUE', 'report': 'Could not simplify WKT down to single shape.'}] }
             return
         # You can't edit coords in shapely. You have to create a new shape w/ the new coords:
-        wkt_json = wkt.loads(shapely.wkt.dumps(single_wkt))
+        wkt_json = geomet_wkt.loads(shapely.wkt.dumps(single_wkt))
         wkt_json = getClampedCoords(wkt_json)
         wkt_json = simplifyPoints(wkt_json)
         # Clamp, simplify, *then* wrap, to help simplify be more accuate w/ points outside of poles
         if self.errors != None:
             return
         wrapped_coords = getWrappedCoords(wkt_json)
-        wkt_wrapped = wkt.dumps(wrapped_coords)
-        wkt_unwrapped = wkt.dumps(getUnwrappedCoords(wrapped_coords))
+        wkt_wrapped = geomet_wkt.dumps(wrapped_coords)
+        wkt_unwrapped = geomet_wkt.dumps(getUnwrappedCoords(wrapped_coords))
         return wkt_unwrapped, wkt_wrapped
 
     def __runWKTsAgainstCMR(self):
 
         def CMRSendRequest(cmr_coords):
             cfg = get_config()
             # logging.debug({'polygon': ','.join(cmr_coords), 'provider': 'ASF', 'page_size': 1})
             logging.debug({'polygon': ','.join(cmr_coords), 'provider': 'ASF', 'page_size': 1, 'attribute[]': 'string,ASF_PLATFORM,FAKEPLATFORM'})
             r = requests.post(cfg['cmr_base'] + cfg['cmr_api'], headers=cfg['cmr_headers'], data={'polygon': ','.join(cmr_coords), 'provider': 'ASF', 'page_size': 1, 'attribute[]': 'string,ASF_PLATFORM,FAKEPLATFORM'})
             return r.status_code, r.text
 
         # NOTE: Only polygons get sent here. Linestring and point wkt's have already returned.
-        wkt_obj_wrapped = wkt.loads(self.wkt_wrapped)
-        wkt_obj_unwrapped = wkt.loads(self.wkt_unwrapped)
+        wkt_obj_wrapped = geomet_wkt.loads(self.wkt_wrapped)
+        wkt_obj_unwrapped = geomet_wkt.loads(self.wkt_unwrapped)
 
-        cmr_coords = parse_wkt_util(wkt.dumps(wkt_obj_wrapped)).split(':')[1].split(',')
+        cmr_coords = parse_wkt_util(geomet_wkt.dumps(wkt_obj_wrapped)).split(':')[1].split(',')
         status_code, text = CMRSendRequest(cmr_coords)
         if status_code != 200:
             if 'Points must be provided in counter-clockwise order.' in text:
                 it = iter(cmr_coords)
                 rev = reversed(list(zip(it, it)))
                 reversed_coords = [i for sub in rev for i in sub]
                 status_code, text = CMRSendRequest(reversed_coords)
@@ -588,16 +596,16 @@
                 match_brackets = r'\[(.*?)\]'
                 bad_points = re.findall(match_brackets, text)
                 self.errors = { 'errors': [{'type': 'DUPLICATE_POINTS', 'report': 'Duplicated or too-close points: [{0}]'.format("], [".join(bad_points))}]}
             else:
                 self.errors = { 'errors': [{'type': 'UNKNOWN', 'report': 'Unknown CMR error: {0}'.format(text)}]}
                 return
 
-        self.wkt_wrapped = wkt.dumps(wkt_obj_wrapped)
-        self.wkt_unwrapped = wkt.dumps(wkt_obj_unwrapped)
+        self.wkt_wrapped = geomet_wkt.dumps(wkt_obj_wrapped)
+        self.wkt_unwrapped = geomet_wkt.dumps(wkt_obj_unwrapped)
 
 def repairWKT(wkt_str, default_crs="EPSG:4326"):
     return simplifyWKT(wkt_str, default_crs=default_crs).get_simplified_json()
 
 
 
 def unwrap_wkt(v):
```

### Comparing `WKTUtils-1.1.6/WKTUtils/ValidateWKT.py` & `wktutils-2.0.0/WKTUtils/ValidateWKT.py`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/WKTUtils/asf_env.py` & `wktutils-2.0.0/WKTUtils/asf_env.py`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/WKTUtils.egg-info/PKG-INFO` & `wktutils-2.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 Metadata-Version: 2.1
 Name: WKTUtils
-Version: 1.1.6
+Version: 2.0.0
 Summary: A few WKT utilities for use elsewhere
 Home-page: https://github.com/asfadmin/Discovery-WKTUtils.git
 Author: ASF Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dateparser
+Requires-Dist: defusedxml
+Requires-Dist: geomet
+Requires-Dist: geopandas
+Requires-Dist: kml2geojson
+Requires-Dist: pyshp
+Requires-Dist: PyYAML
+Requires-Dist: Shapely
+Provides-Extra: extras
+Requires-Dist: requests; extra == "extras"
+Requires-Dist: scikit-learn; extra == "extras"
+Provides-Extra: test
+Requires-Dist: pytest==6.2.5; extra == "test"
+Requires-Dist: pytest-automation==1.1.2; extra == "test"
+Requires-Dist: pytest-xdist==2.4.0; extra == "test"
 
 # Discovery-WKTUtils
 
 [![image](https://img.shields.io/pypi/v/wktutils.svg)](https://pypi.python.org/pypi/WKTUtils)
 
 ### To Install as Package, add the following line to requirements.txt:
```

### Comparing `WKTUtils-1.1.6/WKTUtils.egg-info/SOURCES.txt` & `wktutils-2.0.0/WKTUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/requirements.txt` & `wktutils-2.0.0/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -48,13 +48,12 @@
 regex==2021.9.30
 requests==2.26.0
 retrying==1.3.3
 scikit-learn==0.24.2
 scipy==1.7.1
 Shapely==1.7.1
 six==1.16.0
-sklearn==0.0
 threadpoolctl==2.2.0
 toml==0.10.2
 tzlocal==3.0
 urllib3==1.26.6
 webencodings==0.5.1
```

### Comparing `WKTUtils-1.1.6/setup.py` & `wktutils-2.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import setuptools
 
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+extra_requirements = [
+    'requests',
+    'scikit-learn', 
+]
+
+test_requirements = [
+    "pytest==6.2.5",
+    "pytest-automation==1.1.2",
+    'pytest-xdist==2.4.0',
+]
+
 setuptools.setup(
     name="WKTUtils",
     # version= Moved to pyproject.toml,
     author="ASF Discovery Team",
     author_email="uaf-asf-discovery@alaska.edu",
     description="A few WKT utilities for use elsewhere",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/asfadmin/Discovery-WKTUtils.git",
+    extras_require={"extras": extra_requirements, "test": test_requirements},
     packages=setuptools.find_packages(),
     # package_data= {'WKTUtils': ['VERSION']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=[
         'dateparser',
         'defusedxml',
-        'Fiona',
         'geomet',
         'geopandas',
         'kml2geojson',
         'pyshp',
         'PyYAML',
-        'regex',
-        'requests',
-        'Shapely',
-        'sklearn',
-    ]
+        'Shapely'
+    ],
 )
```

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/AoI.geojson` & `wktutils-2.0.0/yml_tests/Resources/geojsons_valid/AoI.geojson`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/Basic_FC_GC_1.geojson` & `wktutils-2.0.0/yml_tests/Resources/geojsons_valid/Basic_FC_GC_1.geojson`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/ManyCoords_ShovelCreek.geojson` & `wktutils-2.0.0/yml_tests/Resources/geojsons_valid/ManyCoords_ShovelCreek.geojson`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/geojsons_valid/Multi-FC_Multi-GC_1.geojson` & `wktutils-2.0.0/yml_tests/Resources/geojsons_valid/Multi-FC_Multi-GC_1.geojson`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/Blowup.kml` & `wktutils-2.0.0/yml_tests/Resources/kmls_invalid/Blowup.kml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/kmls_invalid/XSLTransformation.kml` & `wktutils-2.0.0/yml_tests/Resources/kmls_invalid/XSLTransformation.kml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/3D_coords.kml` & `wktutils-2.0.0/yml_tests/Resources/kmls_valid/3D_coords.kml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/Iceland1.kml` & `wktutils-2.0.0/yml_tests/Resources/kmls_valid/Iceland1.kml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/Polygon_point_line.kml` & `wktutils-2.0.0/yml_tests/Resources/kmls_valid/Polygon_point_line.kml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/kmls_valid/asf-datapool-results-2019-10-01_10-29-15.kml` & `wktutils-2.0.0/yml_tests/Resources/kmls_valid/asf-datapool-results-2019-10-01_10-29-15.kml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/shps_valid/Fires-all_region_region.zip` & `wktutils-2.0.0/yml_tests/Resources/shps_valid/Fires-all_region_region.zip`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/shps_valid/ShorelineMask26.shp` & `wktutils-2.0.0/yml_tests/Resources/shps_valid/ShorelineMask26.shp`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/shps_valid/UTM_7N.zip` & `wktutils-2.0.0/yml_tests/Resources/shps_valid/UTM_7N.zip`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/shps_valid/Unknown_CRS_shapeset.zip` & `wktutils-2.0.0/yml_tests/Resources/shps_valid/Unknown_CRS_shapeset.zip`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/zips_invalid/DoubleCompressed.zip` & `wktutils-2.0.0/yml_tests/Resources/zips_invalid/DoubleCompressed.zip`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/zips_valid/MultiShp_SingleGeo_WithDir.zip` & `wktutils-2.0.0/yml_tests/Resources/zips_valid/MultiShp_SingleGeo_WithDir.zip`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/zips_valid/NED1_F.zip` & `wktutils-2.0.0/yml_tests/Resources/zips_valid/NED1_F.zip`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/Resources/zips_valid/OneBad_TwoGood.zip` & `wktutils-2.0.0/yml_tests/Resources/zips_valid/OneBad_TwoGood.zip`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/pytest-managers.py` & `wktutils-2.0.0/yml_tests/pytest-managers.py`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/test_filesToWKT.py` & `wktutils-2.0.0/yml_tests/test_filesToWKT.py`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/test_filesToWKT.yml` & `wktutils-2.0.0/yml_tests/test_filesToWKT.yml`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/test_repairWKT.py` & `wktutils-2.0.0/yml_tests/test_repairWKT.py`

 * *Files identical despite different names*

### Comparing `WKTUtils-1.1.6/yml_tests/test_repairWKT.yml` & `wktutils-2.0.0/yml_tests/test_repairWKT.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 - REPAIR wrap longitude:
     test wkt: POLYGON((28 25,12 4,-222 22,28 25))
     repair: 'Wrapped 1 value(s) to +/-180 longitude'
 
 - REPAIR simplify multidimentional coords:
     # Those points are inside the final polygon, so they never make it to the final repair step
     test wkt: GEOMETRYCOLLECTION (POINT (-122.6819440000000014 45.5200000000000031 0.0000000000000000),POINT (-43.1963890000000035 -22.9083329999999989 0.0000000000000000),POINT (28.9760179999999998 41.0122399999999985 0.0000000000000000),POINT (-21.9333330000000011 64.1333329999999933 0.0000000000000000),POLYGON ((-122.6819440000000014 45.5200000000000031 0.0000000000000000, -43.1963890000000035 -22.9083329999999989 0.0000000000000000, 28.9760179999999998 41.0122399999999985 0.0000000000000000, -21.9333330000000011 64.1333329999999933 0.0000000000000000, -122.6819440000000014 45.5200000000000031 0.0000000000000000)))
-    repaired wkt: POLYGON ((-43.1963890000000000 -22.9083330000000000, 28.9760180000000000 41.0122400000000000, -21.9333330000000000 64.1333330000000000, -122.6819440000000000 45.5200000000000000, -43.1963890000000000 -22.9083330000000000))
+    repaired wkt: POLYGON ((-122.6819440000000000 45.5200000000000000, -43.1963890000000000 -22.9083330000000000, 28.9760180000000000 41.0122400000000000, -21.9333330000000000 64.1333330000000000, -122.6819440000000000 45.5200000000000000))
     repair:
       - "Shape(s) that used multidimentional coords: 5. Truncated to 2D"
       - "Multiple points found: 4. Grouping them and using their convex hull instead"
       - "Reversed polygon winding order"
 
 - REPAIR simplify points and reverse polygon order:
     test wkt: GEOMETRYCOLLECTION (POLYGON ((-76.9002014084999956 43.5831678113000009, -80.0249249999999961 43.1852990000000005, -80.0598828581999982 43.3130937289000002, -80.0593369429000035 43.3131630924999982, -80.4371509534999944 44.6942759988000020, -77.2287060000000025 45.0922740000000033, -76.8994176375999956 43.5833930601000006, -76.9002276007999939 43.5832899310000030, -76.9002014084999956 43.5831678113000009)),POLYGON ((-76.9002014084999956 43.5831678113000009, -80.0249249999999961 43.1852990000000005, -80.0598828581999982 43.3130937289000002, -80.0593369429000035 43.3131630924999982, -80.4371509534999944 44.6942759988000020, -77.2287060000000025 45.0922740000000033, -76.8994176375999956 43.5833930601000006, -76.9002276007999939 43.5832899310000030, -76.9002014084999956 43.5831678113000009)),POLYGON ((-76.9002014084999956 43.5831678113000009, -80.0249249999999961 43.1852990000000005, -80.0598828581999982 43.3130937289000002, -80.0593369429000035 43.3131630924999982, -80.4371509534999944 44.6942759988000020, -77.2287060000000025 45.0922740000000033, -76.8994176375999956 43.5833930601000006, -76.9002276007999939 43.5832899310000030, -76.9002014084999956 43.5831678113000009)),POLYGON ((-76.9002014084999956 43.5831678113000009, -80.0249249999999961 43.1852990000000005, -80.0598828581999982 43.3130937289000002, -80.0593369429000035 43.3131630924999982, -80.4371509534999944 44.6942759988000020, -77.2287060000000025 45.0922740000000033, -76.8994176375999956 43.5833930601000006, -76.9002276007999939 43.5832899310000030, -76.9002014084999956 43.5831678113000009)),POLYGON ((-76.9002014084999956 43.5831678113000009, -80.0249249999999961 43.1852990000000005, -80.0598828581999982 43.3130937289000002, -80.0593369429000035 43.3131630924999982, -80.4371509534999944 44.6942759988000020, -77.2287060000000025 45.0922740000000033, -76.8994176375999956 43.5833930601000006, -76.9002276007999939 43.5832899310000030, -76.9002014084999956 43.5831678113000009)),POLYGON ((-76.9000037682999960 43.5831929766000030, -80.0249249999999961 43.1852990000000005, -80.4376515447000031 44.6940950095000034, -77.2293240000000054 45.0921099999999981, -76.9000037682999960 43.5831929766000030)),POLYGON ((-76.9000037682999960 43.5831929766000030, -80.0249249999999961 43.1852990000000005, -80.4376515447000031 44.6940950095000034, -77.2293240000000054 45.0921099999999981, -76.9000037682999960 43.5831929766000030)),POLYGON ((-76.9000037682999960 43.5831929766000030, -80.0249249999999961 43.1852990000000005, -80.4376515447000031 44.6940950095000034, -77.2293240000000054 45.0921099999999981, -76.9000037682999960 43.5831929766000030)),POLYGON ((-76.9000037682999960 43.5831929766000030, -80.0249249999999961 43.1852990000000005, -80.4376515447000031 44.6940950095000034, -77.2293240000000054 45.0921099999999981, -76.9000037682999960 43.5831929766000030)),POLYGON ((-76.9000037682999960 43.5831929766000030, -80.0249249999999961 43.1852990000000005, -80.4376515447000031 44.6940950095000034, -77.2293240000000054 45.0921099999999981, -76.9000037682999960 43.5831929766000030)),POLYGON ((-80.0604362668999983 43.3128883254999977, -76.9280239999999935 43.7108989999999977, -76.5688169999999957 42.0361100000000008, -79.6128780845999984 41.6381159640000007, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0604362668999983 43.3128883254999977)),POLYGON ((-80.0604362668999983 43.3128883254999977, -76.9280239999999935 43.7108989999999977, -76.5688169999999957 42.0361100000000008, -79.6128780845999984 41.6381159640000007, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0604362668999983 43.3128883254999977)),POLYGON ((-80.0604362668999983 43.3128883254999977, -76.9280239999999935 43.7108989999999977, -76.5688169999999957 42.0361100000000008, -79.6128780845999984 41.6381159640000007, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0604362668999983 43.3128883254999977)),POLYGON ((-80.0604362668999983 43.3128883254999977, -76.9280239999999935 43.7108989999999977, -76.5688169999999957 42.0361100000000008, -79.6128780845999984 41.6381159640000007, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0604362668999983 43.3128883254999977)),POLYGON ((-80.0604362668999983 43.3128883254999977, -76.9280239999999935 43.7108989999999977, -76.5688169999999957 42.0361100000000008, -79.6128780845999984 41.6381159640000007, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0604362668999983 43.3128883254999977)),POLYGON ((-76.5961686036999936 42.1636358137999991, -76.5688169999999957 42.0361100000000008, -79.6139673673999937 41.6379735463000031, -79.6140005734000056 41.6381020038000003, -79.6157801078999938 41.6378693237999968, -80.0606161664999973 43.3114737249999990, -80.0600324969000070 43.3115478933000020, -80.0604004400999969 43.3128928777000013, -76.9280239999999935 43.7108989999999977, -76.9004127224000058 43.5821624663999998, -76.9010153688000031 43.5820857252000025, -76.5967474148000065 42.1635603073999974, -76.5961686036999936 42.1636358137999991)),POLYGON ((-76.5961686036999936 42.1636358137999991, -76.5688169999999957 42.0361100000000008, -79.6139673673999937 41.6379735463000031, -79.6140005734000056 41.6381020038000003, -79.6157801078999938 41.6378693237999968, -80.0606161664999973 43.3114737249999990, -80.0600324969000070 43.3115478933000020, -80.0604004400999969 43.3128928777000013, -76.9280239999999935 43.7108989999999977, -76.9004127224000058 43.5821624663999998, -76.9010153688000031 43.5820857252000025, -76.5967474148000065 42.1635603073999974, -76.5961686036999936 42.1636358137999991)),POLYGON ((-76.5961686036999936 42.1636358137999991, -76.5688169999999957 42.0361100000000008, -79.6139673673999937 41.6379735463000031, -79.6140005734000056 41.6381020038000003, -79.6157801078999938 41.6378693237999968, -80.0606161664999973 43.3114737249999990, -80.0600324969000070 43.3115478933000020, -80.0604004400999969 43.3128928777000013, -76.9280239999999935 43.7108989999999977, -76.9004127224000058 43.5821624663999998, -76.9010153688000031 43.5820857252000025, -76.5967474148000065 42.1635603073999974, -76.5961686036999936 42.1636358137999991)),POLYGON ((-76.5961686036999936 42.1636358137999991, -76.5688169999999957 42.0361100000000008, -79.6139673673999937 41.6379735463000031, -79.6140005734000056 41.6381020038000003, -79.6157801078999938 41.6378693237999968, -80.0606161664999973 43.3114737249999990, -80.0600324969000070 43.3115478933000020, -80.0604004400999969 43.3128928777000013, -76.9280239999999935 43.7108989999999977, -76.9004127224000058 43.5821624663999998, -76.9010153688000031 43.5820857252000025, -76.5967474148000065 42.1635603073999974, -76.5961686036999936 42.1636358137999991)),POLYGON ((-76.5961686036999936 42.1636358137999991, -76.5688169999999957 42.0361100000000008, -79.6139673673999937 41.6379735463000031, -79.6140005734000056 41.6381020038000003, -79.6157801078999938 41.6378693237999968, -80.0606161664999973 43.3114737249999990, -80.0600324969000070 43.3115478933000020, -80.0604004400999969 43.3128928777000013, -76.9280239999999935 43.7108989999999977, -76.9004127224000058 43.5821624663999998, -76.9010153688000031 43.5820857252000025, -76.5967474148000065 42.1635603073999974, -76.5961686036999936 42.1636358137999991)),POLYGON ((-76.2548994580999988 40.5458131060999989, -79.2281190000000066 40.1472970000000018, -79.2611847290999947 40.2752228454000019, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6135673407000013 41.6385329773999970, -79.6463779999999986 41.7654720000000026, -76.5942459999999983 42.1636009999999999, -76.2530284871999982 40.5464317644999994, -76.2549739180000046 40.5461710133999986, -76.2548994580999988 40.5458131060999989)),POLYGON ((-76.2548994580999988 40.5458131060999989, -79.2281190000000066 40.1472970000000018, -79.2611847290999947 40.2752228454000019, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6135673407000013 41.6385329773999970, -79.6463779999999986 41.7654720000000026, -76.5942459999999983 42.1636009999999999, -76.2530284871999982 40.5464317644999994, -76.2549739180000046 40.5461710133999986, -76.2548994580999988 40.5458131060999989)),POLYGON ((-76.2548994580999988 40.5458131060999989, -79.2281190000000066 40.1472970000000018, -79.2611847290999947 40.2752228454000019, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6135673407000013 41.6385329773999970, -79.6463779999999986 41.7654720000000026, -76.5942459999999983 42.1636009999999999, -76.2530284871999982 40.5464317644999994, -76.2549739180000046 40.5461710133999986, -76.2548994580999988 40.5458131060999989)),POLYGON ((-76.2548994580999988 40.5458131060999989, -79.2281190000000066 40.1472970000000018, -79.2611847290999947 40.2752228454000019, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6135673407000013 41.6385329773999970, -79.6463779999999986 41.7654720000000026, -76.5942459999999983 42.1636009999999999, -76.2530284871999982 40.5464317644999994, -76.2549739180000046 40.5461710133999986, -76.2548994580999988 40.5458131060999989)),POLYGON ((-76.2548994580999988 40.5458131060999989, -79.2281190000000066 40.1472970000000018, -79.2611847290999947 40.2752228454000019, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6135673407000013 41.6385329773999970, -79.6463779999999986 41.7654720000000026, -76.5942459999999983 42.1636009999999999, -76.2530284871999982 40.5464317644999994, -76.2549739180000046 40.5461710133999986, -76.2548994580999988 40.5458131060999989)),POLYGON ((-76.2559556714000024 40.5456715362999986, -79.2281190000000066 40.1472970000000018, -79.6463779999999986 41.7654720000000026, -76.5948283463000053 42.1635250369999994, -76.2535170000000022 40.5460319999999967, -76.2559624670000034 40.5457041981999993, -76.2559556714000024 40.5456715362999986)),POLYGON ((-76.2559556714000024 40.5456715362999986, -79.2281190000000066 40.1472970000000018, -79.6463779999999986 41.7654720000000026, -76.5948283463000053 42.1635250369999994, -76.2535170000000022 40.5460319999999967, -76.2559624670000034 40.5457041981999993, -76.2559556714000024 40.5456715362999986)),POLYGON ((-76.2559556714000024 40.5456715362999986, -79.2281190000000066 40.1472970000000018, -79.6463779999999986 41.7654720000000026, -76.5948283463000053 42.1635250369999994, -76.2535170000000022 40.5460319999999967, -76.2559624670000034 40.5457041981999993, -76.2559556714000024 40.5456715362999986)),POLYGON ((-76.2559556714000024 40.5456715362999986, -79.2281190000000066 40.1472970000000018, -79.6463779999999986 41.7654720000000026, -76.5948283463000053 42.1635250369999994, -76.2535170000000022 40.5460319999999967, -76.2559624670000034 40.5457041981999993, -76.2559556714000024 40.5456715362999986)),POLYGON ((-76.2559556714000024 40.5456715362999986, -79.2281190000000066 40.1472970000000018, -79.6463779999999986 41.7654720000000026, -76.5948283463000053 42.1635250369999994, -76.2535170000000022 40.5460319999999967, -76.2559624670000034 40.5457041981999993, -76.2559556714000024 40.5456715362999986)),POLYGON ((-75.9470724066000002 39.0548425578000007, -78.8562770000000057 38.6551210000000012, -78.8885483993000065 38.7831225286999981, -78.8880009078999933 38.7831976097999984, -79.2639780619000049 40.2744763022000001, -76.2818829999999934 40.6734160000000031, -75.9453042850000060 39.0555714301000023, -75.9471694998999993 39.0553151570000026, -75.9470724066000002 39.0548425578000007)),POLYGON ((-75.9470724066000002 39.0548425578000007, -78.8562770000000057 38.6551210000000012, -78.8885483993000065 38.7831225286999981, -78.8880009078999933 38.7831976097999984, -79.2639780619000049 40.2744763022000001, -76.2818829999999934 40.6734160000000031, -75.9453042850000060 39.0555714301000023, -75.9471694998999993 39.0553151570000026, -75.9470724066000002 39.0548425578000007)),POLYGON ((-75.9470724066000002 39.0548425578000007, -78.8562770000000057 38.6551210000000012, -78.8885483993000065 38.7831225286999981, -78.8880009078999933 38.7831976097999984, -79.2639780619000049 40.2744763022000001, -76.2818829999999934 40.6734160000000031, -75.9453042850000060 39.0555714301000023, -75.9471694998999993 39.0553151570000026, -75.9470724066000002 39.0548425578000007)),POLYGON ((-75.9470724066000002 39.0548425578000007, -78.8562770000000057 38.6551210000000012, -78.8885483993000065 38.7831225286999981, -78.8880009078999933 38.7831976097999984, -79.2639780619000049 40.2744763022000001, -76.2818829999999934 40.6734160000000031, -75.9453042850000060 39.0555714301000023, -75.9471694998999993 39.0553151570000026, -75.9470724066000002 39.0548425578000007)),POLYGON ((-75.9470724066000002 39.0548425578000007, -78.8562770000000057 38.6551210000000012, -78.8885483993000065 38.7831225286999981, -78.8880009078999933 38.7831976097999984, -79.2639780619000049 40.2744763022000001, -76.2818829999999934 40.6734160000000031, -75.9453042850000060 39.0555714301000023, -75.9471694998999993 39.0553151570000026, -75.9470724066000002 39.0548425578000007)),POLYGON ((-75.9480241899999982 39.0547117837000002, -78.8562770000000057 38.6551210000000012, -79.2645260000000036 40.2744029999999995, -76.2818829999999934 40.6734160000000031, -76.2553312553000069 40.5457888087999976, -76.2559624670000034 40.5457041981999993, -75.9458159999999936 39.0550459999999973, -75.9480303429999992 39.0547417312999983, -75.9480241899999982 39.0547117837000002)),POLYGON ((-75.9480241899999982 39.0547117837000002, -78.8562770000000057 38.6551210000000012, -79.2645260000000036 40.2744029999999995, -76.2818829999999934 40.6734160000000031, -76.2553312553000069 40.5457888087999976, -76.2559624670000034 40.5457041981999993, -75.9458159999999936 39.0550459999999973, -75.9480303429999992 39.0547417312999983, -75.9480241899999982 39.0547117837000002)),POLYGON ((-75.9480241899999982 39.0547117837000002, -78.8562770000000057 38.6551210000000012, -79.2645260000000036 40.2744029999999995, -76.2818829999999934 40.6734160000000031, -76.2553312553000069 40.5457888087999976, -76.2559624670000034 40.5457041981999993, -75.9458159999999936 39.0550459999999973, -75.9480303429999992 39.0547417312999983, -75.9480241899999982 39.0547117837000002)),POLYGON ((-75.9480241899999982 39.0547117837000002, -78.8562770000000057 38.6551210000000012, -79.2645260000000036 40.2744029999999995, -76.2818829999999934 40.6734160000000031, -76.2553312553000069 40.5457888087999976, -76.2559624670000034 40.5457041981999993, -75.9458159999999936 39.0550459999999973, -75.9480303429999992 39.0547417312999983, -75.9480241899999982 39.0547117837000002)),POLYGON ((-75.9480241899999982 39.0547117837000002, -78.8562770000000057 38.6551210000000012, -79.2645260000000036 40.2744029999999995, -76.2818829999999934 40.6734160000000031, -76.2553312553000069 40.5457888087999976, -76.2559624670000034 40.5457041981999993, -75.9458159999999936 39.0550459999999973, -75.9480303429999992 39.0547417312999983, -75.9480241899999982 39.0547117837000002)),POLYGON ((-78.8911251651999947 38.7822747179000018, -75.9737089999999995 39.1823649999999972, -75.6411509999999936 37.5636439999999965, -78.4924145597999967 37.1622436303999990, -78.5116875310999944 37.2421673051999989, -78.8911251651999947 38.7822747179000018)),POLYGON ((-78.8911251651999947 38.7822747179000018, -75.9737089999999995 39.1823649999999972, -75.6411509999999936 37.5636439999999965, -78.4924145597999967 37.1622436303999990, -78.5116875310999944 37.2421673051999989, -78.8911251651999947 38.7822747179000018)),POLYGON ((-78.8911251651999947 38.7822747179000018, -75.9737089999999995 39.1823649999999972, -75.6411509999999936 37.5636439999999965, -78.4924145597999967 37.1622436303999990, -78.5116875310999944 37.2421673051999989, -78.8911251651999947 38.7822747179000018)),POLYGON ((-78.8911251651999947 38.7822747179000018, -75.9737089999999995 39.1823649999999972, -75.6411509999999936 37.5636439999999965, -78.4924145597999967 37.1622436303999990, -78.5116875310999944 37.2421673051999989, -78.8911251651999947 38.7822747179000018)),POLYGON ((-78.8911251651999947 38.7822747179000018, -75.9737089999999995 39.1823649999999972, -75.6411509999999936 37.5636439999999965, -78.4924145597999967 37.1622436303999990, -78.5116875310999944 37.2421673051999989, -78.8911251651999947 38.7822747179000018)),POLYGON ((-75.6418404204000012 37.5635469435000005, -78.4925539999999984 37.1622240000000019, -78.8916700000000048 38.7822000000000031, -75.9737089999999995 39.1823649999999972, -75.9475042984000055 39.0548140141000033, -75.9480303429999992 39.0547417312999983, -75.6678714406999973 37.6911627473999999, -75.6677700000000044 37.6911770000000033, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.6418404204000012 37.5635469435000005)),POLYGON ((-75.6418404204000012 37.5635469435000005, -78.4925539999999984 37.1622240000000019, -78.8916700000000048 38.7822000000000031, -75.9737089999999995 39.1823649999999972, -75.9475042984000055 39.0548140141000033, -75.9480303429999992 39.0547417312999983, -75.6678714406999973 37.6911627473999999, -75.6677700000000044 37.6911770000000033, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.6418404204000012 37.5635469435000005)),POLYGON ((-75.6418404204000012 37.5635469435000005, -78.4925539999999984 37.1622240000000019, -78.8916700000000048 38.7822000000000031, -75.9737089999999995 39.1823649999999972, -75.9475042984000055 39.0548140141000033, -75.9480303429999992 39.0547417312999983, -75.6678714406999973 37.6911627473999999, -75.6677700000000044 37.6911770000000033, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.6418404204000012 37.5635469435000005)),POLYGON ((-75.6418404204000012 37.5635469435000005, -78.4925539999999984 37.1622240000000019, -78.8916700000000048 38.7822000000000031, -75.9737089999999995 39.1823649999999972, -75.9475042984000055 39.0548140141000033, -75.9480303429999992 39.0547417312999983, -75.6678714406999973 37.6911627473999999, -75.6677700000000044 37.6911770000000033, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.6418404204000012 37.5635469435000005)),POLYGON ((-75.6418404204000012 37.5635469435000005, -78.4925539999999984 37.1622240000000019, -78.8916700000000048 38.7822000000000031, -75.9737089999999995 39.1823649999999972, -75.9475042984000055 39.0548140141000033, -75.9480303429999992 39.0547417312999983, -75.6678714406999973 37.6911627473999999, -75.6677700000000044 37.6911770000000033, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.6418404204000012 37.5635469435000005)),POLYGON ((-78.5234583425000068 37.2899440997000013, -75.6672590000000014 37.6912189999999967, -75.3382720000000035 36.0717509999999990, -78.1326534138000000 35.6689347980000022, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234583425000068 37.2899440997000013)),POLYGON ((-78.5234583425000068 37.2899440997000013, -75.6672590000000014 37.6912189999999967, -75.3382720000000035 36.0717509999999990, -78.1326534138000000 35.6689347980000022, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234583425000068 37.2899440997000013)),POLYGON ((-78.5234583425000068 37.2899440997000013, -75.6672590000000014 37.6912189999999967, -75.3382720000000035 36.0717509999999990, -78.1326534138000000 35.6689347980000022, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234583425000068 37.2899440997000013)),POLYGON ((-78.5234583425000068 37.2899440997000013, -75.6672590000000014 37.6912189999999967, -75.3382720000000035 36.0717509999999990, -78.1326534138000000 35.6689347980000022, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234583425000068 37.2899440997000013)),POLYGON ((-78.5234583425000068 37.2899440997000013, -75.6672590000000014 37.6912189999999967, -75.3382720000000035 36.0717509999999990, -78.1326534138000000 35.6689347980000022, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234583425000068 37.2899440997000013)),POLYGON ((-75.3388903207000027 36.0716618677000014, -78.1328740000000010 35.6689030000000002, -78.5237580000000008 37.2899019999999979, -75.6677641154000042 37.6911480349999977, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.3647062815000055 36.1994428458000002, -75.3645939999999968 36.1994589999999974, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.3388903207000027 36.0716618677000014)),POLYGON ((-75.3388903207000027 36.0716618677000014, -78.1328740000000010 35.6689030000000002, -78.5237580000000008 37.2899019999999979, -75.6677641154000042 37.6911480349999977, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.3647062815000055 36.1994428458000002, -75.3645939999999968 36.1994589999999974, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.3388903207000027 36.0716618677000014)),POLYGON ((-75.3388903207000027 36.0716618677000014, -78.1328740000000010 35.6689030000000002, -78.5237580000000008 37.2899019999999979, -75.6677641154000042 37.6911480349999977, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.3647062815000055 36.1994428458000002, -75.3645939999999968 36.1994589999999974, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.3388903207000027 36.0716618677000014)),POLYGON ((-75.3388903207000027 36.0716618677000014, -78.1328740000000010 35.6689030000000002, -78.5237580000000008 37.2899019999999979, -75.6677641154000042 37.6911480349999977, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.3647062815000055 36.1994428458000002, -75.3645939999999968 36.1994589999999974, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.3388903207000027 36.0716618677000014)),POLYGON ((-75.3388903207000027 36.0716618677000014, -78.1328740000000010 35.6689030000000002, -78.5237580000000008 37.2899019999999979, -75.6677641154000042 37.6911480349999977, -75.6585368586000016 37.6457298165000012, -75.6416629999999941 37.5636020000000030, -75.6418463610999936 37.5635761846999969, -75.3647062815000055 36.1994428458000002, -75.3645939999999968 36.1994589999999974, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.3388903207000027 36.0716618677000014)),POLYGON ((-78.1631240095999971 35.7966985682000001, -75.3640819999999962 36.1993790000000004, -75.0268480000000011 34.5225719999999967, -77.7664134764000039 34.1180470596000021, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631240095999971 35.7966985682000001)),POLYGON ((-78.1631240095999971 35.7966985682000001, -75.3640819999999962 36.1993790000000004, -75.0268480000000011 34.5225719999999967, -77.7664134764000039 34.1180470596000021, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631240095999971 35.7966985682000001)),POLYGON ((-78.1631240095999971 35.7966985682000001, -75.3640819999999962 36.1993790000000004, -75.0268480000000011 34.5225719999999967, -77.7664134764000039 34.1180470596000021, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631240095999971 35.7966985682000001)),POLYGON ((-78.1631240095999971 35.7966985682000001, -75.3640819999999962 36.1993790000000004, -75.0268480000000011 34.5225719999999967, -77.7664134764000039 34.1180470596000021, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631240095999971 35.7966985682000001)),POLYGON ((-78.1631240095999971 35.7966985682000001, -75.3640819999999962 36.1993790000000004, -75.0268480000000011 34.5225719999999967, -77.7664134764000039 34.1180470596000021, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631240095999971 35.7966985682000001)),POLYGON ((-75.0273100667999984 34.5225037710999985, -77.7666779999999989 34.1180080000000032, -78.1634059999999948 35.7966580000000008, -75.3645639639999985 36.1993096628999993, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.0542092546999982 34.6562448995000025, -75.0541000000000054 34.6562610000000006, -75.0412326924000013 34.5917262199000035, -75.0273100667999984 34.5225037710999985)),POLYGON ((-75.0273100667999984 34.5225037710999985, -77.7666779999999989 34.1180080000000032, -78.1634059999999948 35.7966580000000008, -75.3645639639999985 36.1993096628999993, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.0542092546999982 34.6562448995000025, -75.0541000000000054 34.6562610000000006, -75.0412326924000013 34.5917262199000035, -75.0273100667999984 34.5225037710999985)),POLYGON ((-75.0273100667999984 34.5225037710999985, -77.7666779999999989 34.1180080000000032, -78.1634059999999948 35.7966580000000008, -75.3645639639999985 36.1993096628999993, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.0542092546999982 34.6562448995000025, -75.0541000000000054 34.6562610000000006, -75.0412326924000013 34.5917262199000035, -75.0273100667999984 34.5225037710999985)),POLYGON ((-75.0273100667999984 34.5225037710999985, -77.7666779999999989 34.1180080000000032, -78.1634059999999948 35.7966580000000008, -75.3645639639999985 36.1993096628999993, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.0542092546999982 34.6562448995000025, -75.0541000000000054 34.6562610000000006, -75.0412326924000013 34.5917262199000035, -75.0273100667999984 34.5225037710999985)),POLYGON ((-75.0273100667999984 34.5225037710999985, -77.7666779999999989 34.1180080000000032, -78.1634059999999948 35.7966580000000008, -75.3645639639999985 36.1993096628999993, -75.3531624974999943 36.1426222640000034, -75.3388060000000053 36.0719569999999976, -75.3389456315999979 36.0719368704999965, -75.0542092546999982 34.6562448995000025, -75.0541000000000054 34.6562610000000006, -75.0412326924000013 34.5917262199000035, -75.0273100667999984 34.5225037710999985)),POLYGON ((-79.0919202831999968 44.1930897386000012, -78.7430569999999932 42.5763469999999984, -81.8085024035000004 42.1791449636999971, -81.8086182617000048 42.1795890514000007, -81.8176650000000052 42.1784170000000032, -82.2516250000000042 43.7949219999999997, -79.0919202831999968 44.1930897386000012)),POLYGON ((-79.0919202831999968 44.1930897386000012, -78.7430569999999932 42.5763469999999984, -81.8085024035000004 42.1791449636999971, -81.8086182617000048 42.1795890514000007, -81.8176650000000052 42.1784170000000032, -82.2516250000000042 43.7949219999999997, -79.0919202831999968 44.1930897386000012)),POLYGON ((-79.0919202831999968 44.1930897386000012, -78.7430569999999932 42.5763469999999984, -81.8085024035000004 42.1791449636999971, -81.8086182617000048 42.1795890514000007, -81.8176650000000052 42.1784170000000032, -82.2516250000000042 43.7949219999999997, -79.0919202831999968 44.1930897386000012)),POLYGON ((-79.0919202831999968 44.1930897386000012, -78.7430569999999932 42.5763469999999984, -81.8085024035000004 42.1791449636999971, -81.8086182617000048 42.1795890514000007, -81.8176650000000052 42.1784170000000032, -82.2516250000000042 43.7949219999999997, -79.0919202831999968 44.1930897386000012)),POLYGON ((-79.0919202831999968 44.1930897386000012, -78.7430569999999932 42.5763469999999984, -81.8085024035000004 42.1791449636999971, -81.8086182617000048 42.1795890514000007, -81.8176650000000052 42.1784170000000032, -82.2516250000000042 43.7949219999999997, -79.0919202831999968 44.1930897386000012)),POLYGON ((-82.2518702643999973 43.7951874892999982, -79.0919949999999972 44.1934359999999984, -78.7430569999999932 42.5763469999999984, -81.8086447075999956 42.1791265247999974, -81.8087988561999992 42.1797173603999980, -81.8178630000000027 42.1785429999999977, -82.2518702643999973 43.7951874892999982)),POLYGON ((-82.2518702643999973 43.7951874892999982, -79.0919949999999972 44.1934359999999984, -78.7430569999999932 42.5763469999999984, -81.8086447075999956 42.1791265247999974, -81.8087988561999992 42.1797173603999980, -81.8178630000000027 42.1785429999999977, -82.2518702643999973 43.7951874892999982)),POLYGON ((-82.2518702643999973 43.7951874892999982, -79.0919949999999972 44.1934359999999984, -78.7430569999999932 42.5763469999999984, -81.8086447075999956 42.1791265247999974, -81.8087988561999992 42.1797173603999980, -81.8178630000000027 42.1785429999999977, -82.2518702643999973 43.7951874892999982)),POLYGON ((-82.2518702643999973 43.7951874892999982, -79.0919949999999972 44.1934359999999984, -78.7430569999999932 42.5763469999999984, -81.8086447075999956 42.1791265247999974, -81.8087988561999992 42.1797173603999980, -81.8178630000000027 42.1785429999999977, -82.2518702643999973 43.7951874892999982)),POLYGON ((-82.2518702643999973 43.7951874892999982, -79.0919949999999972 44.1934359999999984, -78.7430569999999932 42.5763469999999984, -81.8086447075999956 42.1791265247999974, -81.8087988561999992 42.1797173603999980, -81.8178630000000027 42.1785429999999977, -82.2518702643999973 43.7951874892999982)),POLYGON ((-81.8096068983000038 42.1794609684000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4201400457999966 40.6892724662000020, -81.4327742228999938 40.7389688853999985, -81.8086182617000048 42.1795890514000007, -81.8096068983000038 42.1794609684000008)),POLYGON ((-81.8096068983000038 42.1794609684000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4201400457999966 40.6892724662000020, -81.4327742228999938 40.7389688853999985, -81.8086182617000048 42.1795890514000007, -81.8096068983000038 42.1794609684000008)),POLYGON ((-81.8096068983000038 42.1794609684000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4201400457999966 40.6892724662000020, -81.4327742228999938 40.7389688853999985, -81.8086182617000048 42.1795890514000007, -81.8096068983000038 42.1794609684000008)),POLYGON ((-81.8096068983000038 42.1794609684000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4201400457999966 40.6892724662000020, -81.4327742228999938 40.7389688853999985, -81.8086182617000048 42.1795890514000007, -81.8096068983000038 42.1794609684000008)),POLYGON ((-81.8096068983000038 42.1794609684000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4201400457999966 40.6892724662000020, -81.4327742228999938 40.7389688853999985, -81.8086182617000048 42.1795890514000007, -81.8096068983000038 42.1794609684000008)),POLYGON ((-81.8096451862000009 42.1796077089000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4202777448000035 40.6892541790000024, -81.4332364444999968 40.7402257361000011, -81.8087988561999992 42.1797173603999980, -81.8096451862000009 42.1796077089000008)),POLYGON ((-81.8096451862000009 42.1796077089000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4202777448000035 40.6892541790000024, -81.4332364444999968 40.7402257361000011, -81.8087988561999992 42.1797173603999980, -81.8096451862000009 42.1796077089000008)),POLYGON ((-81.8096451862000009 42.1796077089000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4202777448000035 40.6892541790000024, -81.4332364444999968 40.7402257361000011, -81.8087988561999992 42.1797173603999980, -81.8096451862000009 42.1796077089000008)),POLYGON ((-81.8096451862000009 42.1796077089000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4202777448000035 40.6892541790000024, -81.4332364444999968 40.7402257361000011, -81.8087988561999992 42.1797173603999980, -81.8096451862000009 42.1796077089000008)),POLYGON ((-81.8096451862000009 42.1796077089000008, -81.8427889999999962 42.3066329999999979, -78.7648619999999937 42.7043760000000034, -78.4218439999999930 41.0874629999999996, -81.4202777448000035 40.6892541790000024, -81.4332364444999968 40.7402257361000011, -81.8087988561999992 42.1797173603999980, -81.8096451862000009 42.1796077089000008)),POLYGON ((-81.4531057422999965 40.8169001384000012, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743870181999995 39.3255841443999969, -81.0734846669000007 39.3257067313999968, -81.4327742228999938 40.7389688853999985, -81.4531057422999965 40.8169001384000012)),POLYGON ((-81.4531057422999965 40.8169001384000012, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743870181999995 39.3255841443999969, -81.0734846669000007 39.3257067313999968, -81.4327742228999938 40.7389688853999985, -81.4531057422999965 40.8169001384000012)),POLYGON ((-81.4531057422999965 40.8169001384000012, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743870181999995 39.3255841443999969, -81.0734846669000007 39.3257067313999968, -81.4327742228999938 40.7389688853999985, -81.4531057422999965 40.8169001384000012)),POLYGON ((-81.4531057422999965 40.8169001384000012, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743870181999995 39.3255841443999969, -81.0734846669000007 39.3257067313999968, -81.4327742228999938 40.7389688853999985, -81.4531057422999965 40.8169001384000012)),POLYGON ((-81.4531057422999965 40.8169001384000012, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743870181999995 39.3255841443999969, -81.0734846669000007 39.3257067313999968, -81.4327742228999938 40.7389688853999985, -81.4531057422999965 40.8169001384000012)),POLYGON ((-81.4532362335999949 40.8168828455999986, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743650450999951 39.3254977241999981, -81.0735912958000000 39.3256028436999969, -81.4332364444999968 40.7402257361000011, -81.4532362335999949 40.8168828455999986)),POLYGON ((-81.4532362335999949 40.8168828455999986, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743650450999951 39.3254977241999981, -81.0735912958000000 39.3256028436999969, -81.4332364444999968 40.7402257361000011, -81.4532362335999949 40.8168828455999986)),POLYGON ((-81.4532362335999949 40.8168828455999986, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743650450999951 39.3254977241999981, -81.0735912958000000 39.3256028436999969, -81.4332364444999968 40.7402257361000011, -81.4532362335999949 40.8168828455999986)),POLYGON ((-81.4532362335999949 40.8168828455999986, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743650450999951 39.3254977241999981, -81.0735912958000000 39.3256028436999969, -81.4332364444999968 40.7402257361000011, -81.4532362335999949 40.8168828455999986)),POLYGON ((-81.4532362335999949 40.8168828455999986, -78.4485860000000059 41.2150609999999986, -78.1104050000000001 39.5971029999999971, -81.0419540000000040 39.1980250000000012, -81.0743650450999951 39.3254977241999981, -81.0735912958000000 39.3256028436999969, -81.4332364444999968 40.7402257361000011, -81.4532362335999949 40.8168828455999986)),POLYGON ((-77.8069852093999970 38.1054755198000024, -80.6750260000000026 37.7053640000000030, -80.7067746208000045 37.8332276942999997, -80.7059106984000039 37.8333479834000030, -81.0763239999999996 39.3253210000000024, -81.0734846669000007 39.3257067313999968, -81.0735015218999990 39.3257730302999988, -78.1387560000000008 39.7245139999999992, -77.8048432060000010 38.1059050308999971, -77.8070111221999952 38.1056026320000001, -77.8069852093999970 38.1054755198000024)),POLYGON ((-77.8069852093999970 38.1054755198000024, -80.6750260000000026 37.7053640000000030, -80.7067746208000045 37.8332276942999997, -80.7059106984000039 37.8333479834000030, -81.0763239999999996 39.3253210000000024, -81.0734846669000007 39.3257067313999968, -81.0735015218999990 39.3257730302999988, -78.1387560000000008 39.7245139999999992, -77.8048432060000010 38.1059050308999971, -77.8070111221999952 38.1056026320000001, -77.8069852093999970 38.1054755198000024)),POLYGON ((-77.8069852093999970 38.1054755198000024, -80.6750260000000026 37.7053640000000030, -80.7067746208000045 37.8332276942999997, -80.7059106984000039 37.8333479834000030, -81.0763239999999996 39.3253210000000024, -81.0734846669000007 39.3257067313999968, -81.0735015218999990 39.3257730302999988, -78.1387560000000008 39.7245139999999992, -77.8048432060000010 38.1059050308999971, -77.8070111221999952 38.1056026320000001, -77.8069852093999970 38.1054755198000024)),POLYGON ((-77.8069852093999970 38.1054755198000024, -80.6750260000000026 37.7053640000000030, -80.7067746208000045 37.8332276942999997, -80.7059106984000039 37.8333479834000030, -81.0763239999999996 39.3253210000000024, -81.0734846669000007 39.3257067313999968, -81.0735015218999990 39.3257730302999988, -78.1387560000000008 39.7245139999999992, -77.8048432060000010 38.1059050308999971, -77.8070111221999952 38.1056026320000001, -77.8069852093999970 38.1054755198000024)),POLYGON ((-77.8069852093999970 38.1054755198000024, -80.6750260000000026 37.7053640000000030, -80.7067746208000045 37.8332276942999997, -80.7059106984000039 37.8333479834000030, -81.0763239999999996 39.3253210000000024, -81.0734846669000007 39.3257067313999968, -81.0735015218999990 39.3257730302999988, -78.1387560000000008 39.7245139999999992, -77.8048432060000010 38.1059050308999971, -77.8070111221999952 38.1056026320000001, -77.8069852093999970 38.1054755198000024)),POLYGON ((-81.0736301209000061 39.3257555576999991, -78.1387560000000008 39.7245139999999992, -77.8048169999999999 38.1057780000000008, -80.6750260000000026 37.7053640000000030, -80.7067226970000036 37.8330185777000025, -80.7059715174000019 37.8331231730999988, -81.0764240000000029 39.3252179999999996, -81.0735912958000000 39.3256028436999969, -81.0736301209000061 39.3257555576999991)),POLYGON ((-81.0736301209000061 39.3257555576999991, -78.1387560000000008 39.7245139999999992, -77.8048169999999999 38.1057780000000008, -80.6750260000000026 37.7053640000000030, -80.7067226970000036 37.8330185777000025, -80.7059715174000019 37.8331231730999988, -81.0764240000000029 39.3252179999999996, -81.0735912958000000 39.3256028436999969, -81.0736301209000061 39.3257555576999991)),POLYGON ((-81.0736301209000061 39.3257555576999991, -78.1387560000000008 39.7245139999999992, -77.8048169999999999 38.1057780000000008, -80.6750260000000026 37.7053640000000030, -80.7067226970000036 37.8330185777000025, -80.7059715174000019 37.8331231730999988, -81.0764240000000029 39.3252179999999996, -81.0735912958000000 39.3256028436999969, -81.0736301209000061 39.3257555576999991)),POLYGON ((-81.0736301209000061 39.3257555576999991, -78.1387560000000008 39.7245139999999992, -77.8048169999999999 38.1057780000000008, -80.6750260000000026 37.7053640000000030, -80.7067226970000036 37.8330185777000025, -80.7059715174000019 37.8331231730999988, -81.0764240000000029 39.3252179999999996, -81.0735912958000000 39.3256028436999969, -81.0736301209000061 39.3257555576999991)),POLYGON ((-81.0736301209000061 39.3257555576999991, -78.1387560000000008 39.7245139999999992, -77.8048169999999999 38.1057780000000008, -80.6750260000000026 37.7053640000000030, -80.7067226970000036 37.8330185777000025, -80.7059715174000019 37.8331231730999988, -81.0764240000000029 39.3252179999999996, -81.0735912958000000 39.3256028436999969, -81.0736301209000061 39.3257555576999991)),POLYGON ((-80.7104505995000068 37.8326588141000002, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365869704000062 36.2894989918999968, -80.3357630956000008 36.2896165769999968, -80.7104505995000068 37.8326588141000002)),POLYGON ((-80.7104505995000068 37.8326588141000002, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365869704000062 36.2894989918999968, -80.3357630956000008 36.2896165769999968, -80.7104505995000068 37.8326588141000002)),POLYGON ((-80.7104505995000068 37.8326588141000002, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365869704000062 36.2894989918999968, -80.3357630956000008 36.2896165769999968, -80.7104505995000068 37.8326588141000002)),POLYGON ((-80.7104505995000068 37.8326588141000002, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365869704000062 36.2894989918999968, -80.3357630956000008 36.2896165769999968, -80.7104505995000068 37.8326588141000002)),POLYGON ((-80.7104505995000068 37.8326588141000002, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365869704000062 36.2894989918999968, -80.3357630956000008 36.2896165769999968, -80.7104505995000068 37.8326588141000002)),POLYGON ((-80.7060097630999991 37.8332772175999992, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365978309000042 36.2895437132999987, -80.3358773165000031 36.2896465505999970, -80.7105260000000015 37.8324890000000025, -80.7059715174000019 37.8331231730999988, -80.7060097630999991 37.8332772175999992)),POLYGON ((-80.7060097630999991 37.8332772175999992, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365978309000042 36.2895437132999987, -80.3358773165000031 36.2896465505999970, -80.7105260000000015 37.8324890000000025, -80.7059715174000019 37.8331231730999988, -80.7060097630999991 37.8332772175999992)),POLYGON ((-80.7060097630999991 37.8332772175999992, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365978309000042 36.2895437132999987, -80.3358773165000031 36.2896465505999970, -80.7105260000000015 37.8324890000000025, -80.7059715174000019 37.8331231730999988, -80.7060097630999991 37.8332772175999992)),POLYGON ((-80.7060097630999991 37.8332772175999992, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365978309000042 36.2895437132999987, -80.3358773165000031 36.2896465505999970, -80.7105260000000015 37.8324890000000025, -80.7059715174000019 37.8331231730999988, -80.7060097630999991 37.8332772175999992)),POLYGON ((-80.7060097630999991 37.8332772175999992, -77.8338389999999976 38.2332380000000001, -77.4921420000000012 36.5572810000000032, -80.3039469999999937 36.1550939999999983, -80.3365978309000042 36.2895437132999987, -80.3358773165000031 36.2896465505999970, -80.7105260000000015 37.8324890000000025, -80.7059715174000019 37.8331231730999988, -80.7060097630999991 37.8332772175999992)),POLYGON ((-80.3358109856000056 36.2898137983999973, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9584599940999965 34.6960639469999990, -79.9817280000000039 34.7957230000000024, -79.9813702383000020 34.7957752701000018, -80.3366780000000063 36.2894859999999966, -80.3357630956000008 36.2896165769999968, -80.3358109856000056 36.2898137983999973)),POLYGON ((-80.3358109856000056 36.2898137983999973, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9584599940999965 34.6960639469999990, -79.9817280000000039 34.7957230000000024, -79.9813702383000020 34.7957752701000018, -80.3366780000000063 36.2894859999999966, -80.3357630956000008 36.2896165769999968, -80.3358109856000056 36.2898137983999973)),POLYGON ((-80.3358109856000056 36.2898137983999973, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9584599940999965 34.6960639469999990, -79.9817280000000039 34.7957230000000024, -79.9813702383000020 34.7957752701000018, -80.3366780000000063 36.2894859999999966, -80.3357630956000008 36.2896165769999968, -80.3358109856000056 36.2898137983999973)),POLYGON ((-80.3358109856000056 36.2898137983999973, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9584599940999965 34.6960639469999990, -79.9817280000000039 34.7957230000000024, -79.9813702383000020 34.7957752701000018, -80.3366780000000063 36.2894859999999966, -80.3357630956000008 36.2896165769999968, -80.3358109856000056 36.2898137983999973)),POLYGON ((-80.3358109856000056 36.2898137983999973, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9584599940999965 34.6960639469999990, -79.9817280000000039 34.7957230000000024, -79.9813702383000020 34.7957752701000018, -80.3366780000000063 36.2894859999999966, -80.3357630956000008 36.2896165769999968, -80.3358109856000056 36.2898137983999973)),POLYGON ((-80.3359143466000063 36.2897990446000023, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9639599499000013 34.7191831535999995, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -80.3367920000000026 36.2895159999999990, -80.3358773165000031 36.2896465505999970, -80.3359143466000063 36.2897990446000023)),POLYGON ((-80.3359143466000063 36.2897990446000023, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9639599499000013 34.7191831535999995, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -80.3367920000000026 36.2895159999999990, -80.3358773165000031 36.2896465505999970, -80.3359143466000063 36.2897990446000023)),POLYGON ((-80.3359143466000063 36.2897990446000023, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9639599499000013 34.7191831535999995, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -80.3367920000000026 36.2895159999999990, -80.3358773165000031 36.2896465505999970, -80.3359143466000063 36.2897990446000023)),POLYGON ((-80.3359143466000063 36.2897990446000023, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9639599499000013 34.7191831535999995, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -80.3367920000000026 36.2895159999999990, -80.3358773165000031 36.2896465505999970, -80.3359143466000063 36.2897990446000023)),POLYGON ((-80.3359143466000063 36.2897990446000023, -77.5201339999999988 36.6917230000000032, -77.1918639999999954 35.0646709999999970, -79.9500730000000033 34.6608090000000004, -79.9639599499000013 34.7191831535999995, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -80.3367920000000026 36.2895159999999990, -80.3358773165000031 36.2896465505999970, -80.3359143466000063 36.2897990446000023)),POLYGON ((-79.9816889755000062 34.7955558542000034, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6015660239999931 33.1661722077000007, -79.6188636165999952 33.2415407912999967, -79.9816889755000062 34.7955558542000034)),POLYGON ((-79.9816889755000062 34.7955558542000034, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6015660239999931 33.1661722077000007, -79.6188636165999952 33.2415407912999967, -79.9816889755000062 34.7955558542000034)),POLYGON ((-79.9816889755000062 34.7955558542000034, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6015660239999931 33.1661722077000007, -79.6188636165999952 33.2415407912999967, -79.9816889755000062 34.7955558542000034)),POLYGON ((-79.9816889755000062 34.7955558542000034, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6015660239999931 33.1661722077000007, -79.6188636165999952 33.2415407912999967, -79.9816889755000062 34.7955558542000034)),POLYGON ((-79.9816889755000062 34.7955558542000034, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6015660239999931 33.1661722077000007, -79.6188636165999952 33.2415407912999967, -79.9816889755000062 34.7955558542000034)),POLYGON ((-79.9814241071999987 34.7955945568999994, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6016510439999934 33.1661594710000003, -79.6190240111999969 33.2418556523999982, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -79.9814241071999987 34.7955945568999994)),POLYGON ((-79.9814241071999987 34.7955945568999994, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6016510439999934 33.1661594710000003, -79.6190240111999969 33.2418556523999982, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -79.9814241071999987 34.7955945568999994)),POLYGON ((-79.9814241071999987 34.7955945568999994, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6016510439999934 33.1661594710000003, -79.6190240111999969 33.2418556523999982, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -79.9814241071999987 34.7955945568999994)),POLYGON ((-79.9814241071999987 34.7955945568999994, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6016510439999934 33.1661594710000003, -79.6190240111999969 33.2418556523999982, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -79.9814241071999987 34.7955945568999994)),POLYGON ((-79.9814241071999987 34.7955945568999994, -77.2192610000000030 35.1992029999999971, -76.8938600000000037 33.5718079999999972, -79.6016510439999934 33.1661594710000003, -79.6190240111999969 33.2418556523999982, -79.9817809999999980 34.7955090000000027, -79.9814164265000045 34.7955622679000030, -79.9814241071999987 34.7955945568999994)),POLYGON ((-79.6327398977999934 33.3009742058000029, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584155642000070 31.6710066782000013, -79.6188636165999952 33.2415407912999967, -79.6327398977999934 33.3009742058000029)),POLYGON ((-79.6327398977999934 33.3009742058000029, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584155642000070 31.6710066782000013, -79.6188636165999952 33.2415407912999967, -79.6327398977999934 33.3009742058000029)),POLYGON ((-79.6327398977999934 33.3009742058000029, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584155642000070 31.6710066782000013, -79.6188636165999952 33.2415407912999967, -79.6327398977999934 33.3009742058000029)),POLYGON ((-79.6327398977999934 33.3009742058000029, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584155642000070 31.6710066782000013, -79.6188636165999952 33.2415407912999967, -79.6327398977999934 33.3009742058000029)),POLYGON ((-79.6327398977999934 33.3009742058000029, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584155642000070 31.6710066782000013, -79.6188636165999952 33.2415407912999967, -79.6327398977999934 33.3009742058000029)),POLYGON ((-79.6328244406000039 33.3009615663000034, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584969193000006 31.6709942154000004, -79.6190240111999969 33.2418556523999982, -79.6328244406000039 33.3009615663000034)),POLYGON ((-79.6328244406000039 33.3009615663000034, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584969193000006 31.6709942154000004, -79.6190240111999969 33.2418556523999982, -79.6328244406000039 33.3009615663000034)),POLYGON ((-79.6328244406000039 33.3009615663000034, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584969193000006 31.6709942154000004, -79.6190240111999969 33.2418556523999982, -79.6328244406000039 33.3009615663000034)),POLYGON ((-79.6328244406000039 33.3009615663000034, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584969193000006 31.6709942154000004, -79.6190240111999969 33.2418556523999982, -79.6328244406000039 33.3009615663000034)),POLYGON ((-79.6328244406000039 33.3009615663000034, -76.9206920000000025 33.7064359999999965, -76.5977170000000029 32.0785979999999995, -79.2584969193000006 31.6709942154000004, -79.6190240111999969 33.2418556523999982, -79.6328244406000039 33.3009615663000034)),POLYGON ((-76.8999971323000011 43.5822153877999980, -80.0252080000000063 43.1842499999999987, -80.0604361542000049 43.3130234274999992, -80.0593369429000035 43.3131630924999982, -80.4371194983999942 44.6941610133999987, -77.2293240000000054 45.0921099999999981, -76.9000304082999975 43.5833150387000003, -76.9002276007999939 43.5832899310000030, -76.8999971323000011 43.5822153877999980)),POLYGON ((-76.8999971323000011 43.5822153877999980, -80.0252080000000063 43.1842499999999987, -80.0604361542000049 43.3130234274999992, -80.0593369429000035 43.3131630924999982, -80.4371194983999942 44.6941610133999987, -77.2293240000000054 45.0921099999999981, -76.9000304082999975 43.5833150387000003, -76.9002276007999939 43.5832899310000030, -76.8999971323000011 43.5822153877999980)),POLYGON ((-76.8999971323000011 43.5822153877999980, -80.0252080000000063 43.1842499999999987, -80.0604361542000049 43.3130234274999992, -80.0593369429000035 43.3131630924999982, -80.4371194983999942 44.6941610133999987, -77.2293240000000054 45.0921099999999981, -76.9000304082999975 43.5833150387000003, -76.9002276007999939 43.5832899310000030, -76.8999971323000011 43.5822153877999980)),POLYGON ((-76.8999971323000011 43.5822153877999980, -80.0252080000000063 43.1842499999999987, -80.0604361542000049 43.3130234274999992, -80.0593369429000035 43.3131630924999982, -80.4371194983999942 44.6941610133999987, -77.2293240000000054 45.0921099999999981, -76.9000304082999975 43.5833150387000003, -76.9002276007999939 43.5832899310000030, -76.8999971323000011 43.5822153877999980)),POLYGON ((-76.8999971323000011 43.5822153877999980, -80.0252080000000063 43.1842499999999987, -80.0604361542000049 43.3130234274999992, -80.0593369429000035 43.3131630924999982, -80.4371194983999942 44.6941610133999987, -77.2293240000000054 45.0921099999999981, -76.9000304082999975 43.5833150387000003, -76.9002276007999939 43.5832899310000030, -76.8999971323000011 43.5822153877999980)),POLYGON ((-80.0600784308000044 43.3115420564000004, -76.9283449999999931 43.7094990000000010, -76.5694270000000046 42.0361899999999977, -79.6129112906999978 41.6382444310999986, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0600784308000044 43.3115420564000004)),POLYGON ((-80.0600784308000044 43.3115420564000004, -76.9283449999999931 43.7094990000000010, -76.5694270000000046 42.0361899999999977, -79.6129112906999978 41.6382444310999986, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0600784308000044 43.3115420564000004)),POLYGON ((-80.0600784308000044 43.3115420564000004, -76.9283449999999931 43.7094990000000010, -76.5694270000000046 42.0361899999999977, -79.6129112906999978 41.6382444310999986, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0600784308000044 43.3115420564000004)),POLYGON ((-80.0600784308000044 43.3115420564000004, -76.9283449999999931 43.7094990000000010, -76.5694270000000046 42.0361899999999977, -79.6129112906999978 41.6382444310999986, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0600784308000044 43.3115420564000004)),POLYGON ((-80.0600784308000044 43.3115420564000004, -76.9283449999999931 43.7094990000000010, -76.5694270000000046 42.0361899999999977, -79.6129112906999978 41.6382444310999986, -79.6130048816999931 41.6386065145999993, -79.6153340000000043 41.6383020000000030, -80.0600784308000044 43.3115420564000004)),POLYGON ((-76.2549062551999981 40.5458457777999968, -79.2286150000000049 40.1472359999999995, -79.2616821171999959 40.2751563069000014, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6140941738999999 41.6384640978999983, -79.6469730000000027 41.7656559999999999, -76.5948869999999999 42.1638030000000015, -76.2535855988000009 40.5463570933999975, -76.2549739180000046 40.5461710133999986, -76.2549062551999981 40.5458457777999968)),POLYGON ((-76.2549062551999981 40.5458457777999968, -79.2286150000000049 40.1472359999999995, -79.2616821171999959 40.2751563069000014, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6140941738999999 41.6384640978999983, -79.6469730000000027 41.7656559999999999, -76.5948869999999999 42.1638030000000015, -76.2535855988000009 40.5463570933999975, -76.2549739180000046 40.5461710133999986, -76.2549062551999981 40.5458457777999968)),POLYGON ((-76.2549062551999981 40.5458457777999968, -79.2286150000000049 40.1472359999999995, -79.2616821171999959 40.2751563069000014, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6140941738999999 41.6384640978999983, -79.6469730000000027 41.7656559999999999, -76.5948869999999999 42.1638030000000015, -76.2535855988000009 40.5463570933999975, -76.2549739180000046 40.5461710133999986, -76.2549062551999981 40.5458457777999968)),POLYGON ((-76.2549062551999981 40.5458457777999968, -79.2286150000000049 40.1472359999999995, -79.2616821171999959 40.2751563069000014, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6140941738999999 41.6384640978999983, -79.6469730000000027 41.7656559999999999, -76.5948869999999999 42.1638030000000015, -76.2535855988000009 40.5463570933999975, -76.2549739180000046 40.5461710133999986, -76.2549062551999981 40.5458457777999968)),POLYGON ((-76.2549062551999981 40.5458457777999968, -79.2286150000000049 40.1472359999999995, -79.2616821171999959 40.2751563069000014, -79.2606182731999951 40.2752986233999977, -79.6130048816999931 41.6386065145999993, -79.6140941738999999 41.6384640978999983, -79.6469730000000027 41.7656559999999999, -76.5948869999999999 42.1638030000000015, -76.2535855988000009 40.5463570933999975, -76.2549739180000046 40.5461710133999986, -76.2549062551999981 40.5458457777999968)),POLYGON ((-75.9470785608999961 39.0548725139000013, -78.8567500000000052 38.6550599999999989, -78.8890222146000042 38.7830575512000024, -78.8880009078999933 38.7831976097999984, -79.2639793703000066 40.2744814922000032, -76.2825239999999951 40.6733669999999989, -75.9459080610999990 39.0554884737000023, -75.9471694998999993 39.0553151570000026, -75.9470785608999961 39.0548725139000013)),POLYGON ((-75.9470785608999961 39.0548725139000013, -78.8567500000000052 38.6550599999999989, -78.8890222146000042 38.7830575512000024, -78.8880009078999933 38.7831976097999984, -79.2639793703000066 40.2744814922000032, -76.2825239999999951 40.6733669999999989, -75.9459080610999990 39.0554884737000023, -75.9471694998999993 39.0553151570000026, -75.9470785608999961 39.0548725139000013)),POLYGON ((-75.9470785608999961 39.0548725139000013, -78.8567500000000052 38.6550599999999989, -78.8890222146000042 38.7830575512000024, -78.8880009078999933 38.7831976097999984, -79.2639793703000066 40.2744814922000032, -76.2825239999999951 40.6733669999999989, -75.9459080610999990 39.0554884737000023, -75.9471694998999993 39.0553151570000026, -75.9470785608999961 39.0548725139000013)),POLYGON ((-75.9470785608999961 39.0548725139000013, -78.8567500000000052 38.6550599999999989, -78.8890222146000042 38.7830575512000024, -78.8880009078999933 38.7831976097999984, -79.2639793703000066 40.2744814922000032, -76.2825239999999951 40.6733669999999989, -75.9459080610999990 39.0554884737000023, -75.9471694998999993 39.0553151570000026, -75.9470785608999961 39.0548725139000013)),POLYGON ((-75.9470785608999961 39.0548725139000013, -78.8567500000000052 38.6550599999999989, -78.8890222146000042 38.7830575512000024, -78.8880009078999933 38.7831976097999984, -79.2639793703000066 40.2744814922000032, -76.2825239999999951 40.6733669999999989, -75.9459080610999990 39.0554884737000023, -75.9471694998999993 39.0553151570000026, -75.9470785608999961 39.0548725139000013)),POLYGON ((-78.8911260888999948 38.7822784673000029, -75.9742430000000013 39.1823229999999967, -75.6416629999999941 37.5636020000000030, -78.4924151093999996 37.1622459096000028, -78.5116875310999944 37.2421673051999989, -78.8911260888999948 38.7822784673000029)),POLYGON ((-78.8911260888999948 38.7822784673000029, -75.9742430000000013 39.1823229999999967, -75.6416629999999941 37.5636020000000030, -78.4924151093999996 37.1622459096000028, -78.5116875310999944 37.2421673051999989, -78.8911260888999948 38.7822784673000029)),POLYGON ((-78.8911260888999948 38.7822784673000029, -75.9742430000000013 39.1823229999999967, -75.6416629999999941 37.5636020000000030, -78.4924151093999996 37.1622459096000028, -78.5116875310999944 37.2421673051999989, -78.8911260888999948 38.7822784673000029)),POLYGON ((-78.8911260888999948 38.7822784673000029, -75.9742430000000013 39.1823229999999967, -75.6416629999999941 37.5636020000000030, -78.4924151093999996 37.1622459096000028, -78.5116875310999944 37.2421673051999989, -78.8911260888999948 38.7822784673000029)),POLYGON ((-78.8911260888999948 38.7822784673000029, -75.9742430000000013 39.1823229999999967, -75.6416629999999941 37.5636020000000030, -78.4924151093999996 37.1622459096000028, -78.5116875310999944 37.2421673051999989, -78.8911260888999948 38.7822784673000029)),POLYGON ((-78.5234588731999992 37.2899462540000002, -75.6677700000000044 37.6911770000000033, -75.3388060000000053 36.0719569999999976, -78.1327119692000025 35.6691825563000009, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234588731999992 37.2899462540000002)),POLYGON ((-78.5234588731999992 37.2899462540000002, -75.6677700000000044 37.6911770000000033, -75.3388060000000053 36.0719569999999976, -78.1327119692000025 35.6691825563000009, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234588731999992 37.2899462540000002)),POLYGON ((-78.5234588731999992 37.2899462540000002, -75.6677700000000044 37.6911770000000033, -75.3388060000000053 36.0719569999999976, -78.1327119692000025 35.6691825563000009, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234588731999992 37.2899462540000002)),POLYGON ((-78.5234588731999992 37.2899462540000002, -75.6677700000000044 37.6911770000000033, -75.3388060000000053 36.0719569999999976, -78.1327119692000025 35.6691825563000009, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234588731999992 37.2899462540000002)),POLYGON ((-78.5234588731999992 37.2899462540000002, -75.6677700000000044 37.6911770000000033, -75.3388060000000053 36.0719569999999976, -78.1327119692000025 35.6691825563000009, -78.1493215771999985 35.7394608387999995, -78.5116875310999944 37.2421673051999989, -78.5234588731999992 37.2899462540000002)),POLYGON ((-78.1631540479999956 35.7968231354999986, -75.3645939999999968 36.1994589999999974, -75.0272899999999936 34.5224040000000016, -77.7663852214000002 34.1179252809999980, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631540479999956 35.7968231354999986)),POLYGON ((-78.1631540479999956 35.7968231354999986, -75.3645939999999968 36.1994589999999974, -75.0272899999999936 34.5224040000000016, -77.7663852214000002 34.1179252809999980, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631540479999956 35.7968231354999986)),POLYGON ((-78.1631540479999956 35.7968231354999986, -75.3645939999999968 36.1994589999999974, -75.0272899999999936 34.5224040000000016, -77.7663852214000002 34.1179252809999980, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631540479999956 35.7968231354999986)),POLYGON ((-78.1631540479999956 35.7968231354999986, -75.3645939999999968 36.1994589999999974, -75.0272899999999936 34.5224040000000016, -77.7663852214000002 34.1179252809999980, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631540479999956 35.7968231354999986)),POLYGON ((-78.1631540479999956 35.7968231354999986, -75.3645939999999968 36.1994589999999974, -75.0272899999999936 34.5224040000000016, -77.7663852214000002 34.1179252809999980, -77.7823993234000000 34.1869458258000023, -78.1493215771999985 35.7394608387999995, -78.1631540479999956 35.7968231354999986)),POLYGON ((-77.7977595960999935 34.2519379423000032, -75.0541000000000054 34.6562610000000006, -74.7296300000000002 33.0289119999999983, -77.4194422650000007 32.6226062313999989, -77.7823993234000000 34.1869458258000023, -77.7977595960999935 34.2519379423000032)),POLYGON ((-77.7977595960999935 34.2519379423000032, -75.0541000000000054 34.6562610000000006, -74.7296300000000002 33.0289119999999983, -77.4194422650000007 32.6226062313999989, -77.7823993234000000 34.1869458258000023, -77.7977595960999935 34.2519379423000032)),POLYGON ((-77.7977595960999935 34.2519379423000032, -75.0541000000000054 34.6562610000000006, -74.7296300000000002 33.0289119999999983, -77.4194422650000007 32.6226062313999989, -77.7823993234000000 34.1869458258000023, -77.7977595960999935 34.2519379423000032)),POLYGON ((-77.7977595960999935 34.2519379423000032, -75.0541000000000054 34.6562610000000006, -74.7296300000000002 33.0289119999999983, -77.4194422650000007 32.6226062313999989, -77.7823993234000000 34.1869458258000023, -77.7977595960999935 34.2519379423000032)),POLYGON ((-77.7977595960999935 34.2519379423000032, -75.0541000000000054 34.6562610000000006, -74.7296300000000002 33.0289119999999983, -77.4194422650000007 32.6226062313999989, -77.7823993234000000 34.1869458258000023, -77.7977595960999935 34.2519379423000032)),POLYGON ((-79.0910218158000049 44.1932547526999997, -78.7423100000000034 42.5770150000000029, -81.8141524374999989 42.1790237445000002, -82.2480240000000009 43.7954560000000015, -79.0910218158000049 44.1932547526999997)),POLYGON ((-79.0910218158000049 44.1932547526999997, -78.7423100000000034 42.5770150000000029, -81.8141524374999989 42.1790237445000002, -82.2480240000000009 43.7954560000000015, -79.0910218158000049 44.1932547526999997)),POLYGON ((-79.0910218158000049 44.1932547526999997, -78.7423100000000034 42.5770150000000029, -81.8141524374999989 42.1790237445000002, -82.2480240000000009 43.7954560000000015, -79.0910218158000049 44.1932547526999997)),POLYGON ((-79.0910218158000049 44.1932547526999997, -78.7423100000000034 42.5770150000000029, -81.8141524374999989 42.1790237445000002, -82.2480240000000009 43.7954560000000015, -79.0910218158000049 44.1932547526999997)),POLYGON ((-79.0910218158000049 44.1932547526999997, -78.7423100000000034 42.5770150000000029, -81.8141524374999989 42.1790237445000002, -82.2480240000000009 43.7954560000000015, -79.0910218158000049 44.1932547526999997)),POLYGON ((-79.0910717634999969 44.1934862549000016, -78.7423100000000034 42.5770150000000029, -81.8139477827999997 42.1790502598000003, -82.2478870000000057 43.7957230000000024, -79.0910717634999969 44.1934862549000016)),POLYGON ((-79.0910717634999969 44.1934862549000016, -78.7423100000000034 42.5770150000000029, -81.8139477827999997 42.1790502598000003, -82.2478870000000057 43.7957230000000024, -79.0910717634999969 44.1934862549000016)),POLYGON ((-79.0910717634999969 44.1934862549000016, -78.7423100000000034 42.5770150000000029, -81.8139477827999997 42.1790502598000003, -82.2478870000000057 43.7957230000000024, -79.0910717634999969 44.1934862549000016)),POLYGON ((-79.0910717634999969 44.1934862549000016, -78.7423100000000034 42.5770150000000029, -81.8139477827999997 42.1790502598000003, -82.2478870000000057 43.7957230000000024, -79.0910717634999969 44.1934862549000016)),POLYGON ((-79.0910717634999969 44.1934862549000016, -78.7423100000000034 42.5770150000000029, -81.8139477827999997 42.1790502598000003, -82.2478870000000057 43.7957230000000024, -79.0910717634999969 44.1934862549000016)),POLYGON ((-78.4234766261999994 41.0873057590000030, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678069096999991 42.7046870511000023, -78.7676947491000021 42.7041671747999985, -78.7669070000000033 42.7042689999999965, -78.4508817699999952 41.2149099195000019, -78.4501719999999949 41.2150040000000004, -78.4234766261999994 41.0873057590000030)),POLYGON ((-78.4234766261999994 41.0873057590000030, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678069096999991 42.7046870511000023, -78.7676947491000021 42.7041671747999985, -78.7669070000000033 42.7042689999999965, -78.4508817699999952 41.2149099195000019, -78.4501719999999949 41.2150040000000004, -78.4234766261999994 41.0873057590000030)),POLYGON ((-78.4234766261999994 41.0873057590000030, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678069096999991 42.7046870511000023, -78.7676947491000021 42.7041671747999985, -78.7669070000000033 42.7042689999999965, -78.4508817699999952 41.2149099195000019, -78.4501719999999949 41.2150040000000004, -78.4234766261999994 41.0873057590000030)),POLYGON ((-78.4234766261999994 41.0873057590000030, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678069096999991 42.7046870511000023, -78.7676947491000021 42.7041671747999985, -78.7669070000000033 42.7042689999999965, -78.4508817699999952 41.2149099195000019, -78.4501719999999949 41.2150040000000004, -78.4234766261999994 41.0873057590000030)),POLYGON ((-78.4234766261999994 41.0873057590000030, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678069096999991 42.7046870511000023, -78.7676947491000021 42.7041671747999985, -78.7669070000000033 42.7042689999999965, -78.4508817699999952 41.2149099195000019, -78.4501719999999949 41.2150040000000004, -78.4234766261999994 41.0873057590000030)),POLYGON ((-78.4234726458000040 41.0873062876000006, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678008484000003 42.7046878343000031, -78.7677096296999935 42.7042650173999974, -78.7669980000000010 42.7043570000000017, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.4234726458000040 41.0873062876000006)),POLYGON ((-78.4234726458000040 41.0873062876000006, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678008484000003 42.7046878343000031, -78.7677096296999935 42.7042650173999974, -78.7669980000000010 42.7043570000000017, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.4234726458000040 41.0873062876000006)),POLYGON ((-78.4234726458000040 41.0873062876000006, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678008484000003 42.7046878343000031, -78.7677096296999935 42.7042650173999974, -78.7669980000000010 42.7043570000000017, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.4234726458000040 41.0873062876000006)),POLYGON ((-78.4234726458000040 41.0873062876000006, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678008484000003 42.7046878343000031, -78.7677096296999935 42.7042650173999974, -78.7669980000000010 42.7043570000000017, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.4234726458000040 41.0873062876000006)),POLYGON ((-78.4234726458000040 41.0873062876000006, -81.4199749999999938 40.6893960000000021, -81.8421249999999958 42.3074530000000024, -78.7678008484000003 42.7046878343000031, -78.7677096296999935 42.7042650173999974, -78.7669980000000010 42.7043570000000017, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.4234726458000040 41.0873062876000006)),POLYGON ((-78.1362907255000039 39.7249136354000001, -78.1095889999999997 39.5971490000000017, -81.0378462033999938 39.1985542522999992, -81.0378696972999961 39.1986489108000029, -81.0412000119000027 39.1981954479999999, -81.4527659999999969 40.8170429999999982, -78.4501525935999950 41.2149111689000023, -78.1386023148999982 39.7245996696999981, -78.1362907255000039 39.7249136354000001)),POLYGON ((-78.1362907255000039 39.7249136354000001, -78.1095889999999997 39.5971490000000017, -81.0378462033999938 39.1985542522999992, -81.0378696972999961 39.1986489108000029, -81.0412000119000027 39.1981954479999999, -81.4527659999999969 40.8170429999999982, -78.4501525935999950 41.2149111689000023, -78.1386023148999982 39.7245996696999981, -78.1362907255000039 39.7249136354000001)),POLYGON ((-78.1362907255000039 39.7249136354000001, -78.1095889999999997 39.5971490000000017, -81.0378462033999938 39.1985542522999992, -81.0378696972999961 39.1986489108000029, -81.0412000119000027 39.1981954479999999, -81.4527659999999969 40.8170429999999982, -78.4501525935999950 41.2149111689000023, -78.1386023148999982 39.7245996696999981, -78.1362907255000039 39.7249136354000001)),POLYGON ((-78.1362907255000039 39.7249136354000001, -78.1095889999999997 39.5971490000000017, -81.0378462033999938 39.1985542522999992, -81.0378696972999961 39.1986489108000029, -81.0412000119000027 39.1981954479999999, -81.4527659999999969 40.8170429999999982, -78.4501525935999950 41.2149111689000023, -78.1386023148999982 39.7245996696999981, -78.1362907255000039 39.7249136354000001)),POLYGON ((-78.1362907255000039 39.7249136354000001, -78.1095889999999997 39.5971490000000017, -81.0378462033999938 39.1985542522999992, -81.0378696972999961 39.1986489108000029, -81.0412000119000027 39.1981954479999999, -81.4527659999999969 40.8170429999999982, -78.4501525935999950 41.2149111689000023, -78.1386023148999982 39.7245996696999981, -78.1362907255000039 39.7249136354000001)),POLYGON ((-78.1362286619000059 39.7246166687000013, -78.1095889999999997 39.5971490000000017, -81.0411759999999930 39.1981010000000012, -81.4527659999999969 40.8170429999999982, -78.4509305043000040 41.2148080899999982, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.1385410500000006 39.7243026079000003, -78.1362286619000059 39.7246166687000013)),POLYGON ((-78.1362286619000059 39.7246166687000013, -78.1095889999999997 39.5971490000000017, -81.0411759999999930 39.1981010000000012, -81.4527659999999969 40.8170429999999982, -78.4509305043000040 41.2148080899999982, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.1385410500000006 39.7243026079000003, -78.1362286619000059 39.7246166687000013)),POLYGON ((-78.1362286619000059 39.7246166687000013, -78.1095889999999997 39.5971490000000017, -81.0411759999999930 39.1981010000000012, -81.4527659999999969 40.8170429999999982, -78.4509305043000040 41.2148080899999982, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.1385410500000006 39.7243026079000003, -78.1362286619000059 39.7246166687000013)),POLYGON ((-78.1362286619000059 39.7246166687000013, -78.1095889999999997 39.5971490000000017, -81.0411759999999930 39.1981010000000012, -81.4527659999999969 40.8170429999999982, -78.4509305043000040 41.2148080899999982, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.1385410500000006 39.7243026079000003, -78.1362286619000059 39.7246166687000013)),POLYGON ((-78.1362286619000059 39.7246166687000013, -78.1095889999999997 39.5971490000000017, -81.0411759999999930 39.1981010000000012, -81.4527659999999969 40.8170429999999982, -78.4509305043000040 41.2148080899999982, -78.4509161266999939 41.2147403315999981, -78.4501340000000056 41.2148439999999994, -78.1385410500000006 39.7243026079000003, -78.1362286619000059 39.7246166687000013)),POLYGON ((-81.0447666768999966 39.1977098033000004, -81.0764240000000029 39.3252179999999996, -78.1379009999999994 39.7244379999999992, -77.8040239999999983 38.1058239999999984, -80.6725018546000001 37.7056877855999986, -80.7035750000000007 37.8336910000000017, -80.6992404334999947 37.8342943963000025, -81.0378696972999961 39.1986489108000029, -81.0447666768999966 39.1977098033000004)),POLYGON ((-81.0447666768999966 39.1977098033000004, -81.0764240000000029 39.3252179999999996, -78.1379009999999994 39.7244379999999992, -77.8040239999999983 38.1058239999999984, -80.6725018546000001 37.7056877855999986, -80.7035750000000007 37.8336910000000017, -80.6992404334999947 37.8342943963000025, -81.0378696972999961 39.1986489108000029, -81.0447666768999966 39.1977098033000004)),POLYGON ((-81.0447666768999966 39.1977098033000004, -81.0764240000000029 39.3252179999999996, -78.1379009999999994 39.7244379999999992, -77.8040239999999983 38.1058239999999984, -80.6725018546000001 37.7056877855999986, -80.7035750000000007 37.8336910000000017, -80.6992404334999947 37.8342943963000025, -81.0378696972999961 39.1986489108000029, -81.0447666768999966 39.1977098033000004)),POLYGON ((-81.0447666768999966 39.1977098033000004, -81.0764240000000029 39.3252179999999996, -78.1379009999999994 39.7244379999999992, -77.8040239999999983 38.1058239999999984, -80.6725018546000001 37.7056877855999986, -80.7035750000000007 37.8336910000000017, -80.6992404334999947 37.8342943963000025, -81.0378696972999961 39.1986489108000029, -81.0447666768999966 39.1977098033000004)),POLYGON ((-81.0447666768999966 39.1977098033000004, -81.0764240000000029 39.3252179999999996, -78.1379009999999994 39.7244379999999992, -77.8040239999999983 38.1058239999999984, -80.6725018546000001 37.7056877855999986, -80.7035750000000007 37.8336910000000017, -80.6992404334999947 37.8342943963000025, -81.0378696972999961 39.1986489108000029, -81.0447666768999966 39.1977098033000004)),POLYGON ((-78.1378912759000031 39.7243908579999996, -77.8040239999999983 38.1058239999999984, -80.6723144531000003 37.7057139270999997, -80.7033459999999963 37.8335489999999979, -80.6989734577999940 37.8341576685999996, -81.0375710641999945 39.1983971836000009, -81.0446964653000066 39.1974270077000000, -81.0764240000000029 39.3252179999999996, -78.1385508958999964 39.7243497069000000, -78.1385410500000006 39.7243026079000003, -78.1378912759000031 39.7243908579999996)),POLYGON ((-78.1378912759000031 39.7243908579999996, -77.8040239999999983 38.1058239999999984, -80.6723144531000003 37.7057139270999997, -80.7033459999999963 37.8335489999999979, -80.6989734577999940 37.8341576685999996, -81.0375710641999945 39.1983971836000009, -81.0446964653000066 39.1974270077000000, -81.0764240000000029 39.3252179999999996, -78.1385508958999964 39.7243497069000000, -78.1385410500000006 39.7243026079000003, -78.1378912759000031 39.7243908579999996)),POLYGON ((-78.1378912759000031 39.7243908579999996, -77.8040239999999983 38.1058239999999984, -80.6723144531000003 37.7057139270999997, -80.7033459999999963 37.8335489999999979, -80.6989734577999940 37.8341576685999996, -81.0375710641999945 39.1983971836000009, -81.0446964653000066 39.1974270077000000, -81.0764240000000029 39.3252179999999996, -78.1385508958999964 39.7243497069000000, -78.1385410500000006 39.7243026079000003, -78.1378912759000031 39.7243908579999996)),POLYGON ((-78.1378912759000031 39.7243908579999996, -77.8040239999999983 38.1058239999999984, -80.6723144531000003 37.7057139270999997, -80.7033459999999963 37.8335489999999979, -80.6989734577999940 37.8341576685999996, -81.0375710641999945 39.1983971836000009, -81.0446964653000066 39.1974270077000000, -81.0764240000000029 39.3252179999999996, -78.1385508958999964 39.7243497069000000, -78.1385410500000006 39.7243026079000003, -78.1378912759000031 39.7243908579999996)),POLYGON ((-78.1378912759000031 39.7243908579999996, -77.8040239999999983 38.1058239999999984, -80.6723144531000003 37.7057139270999997, -80.7033459999999963 37.8335489999999979, -80.6989734577999940 37.8341576685999996, -81.0375710641999945 39.1983971836000009, -81.0446964653000066 39.1974270077000000, -81.0764240000000029 39.3252179999999996, -78.1385508958999964 39.7243497069000000, -78.1385410500000006 39.7243026079000003, -78.1378912759000031 39.7243908579999996)),POLYGON ((-80.7035200220999940 37.8334645230000035, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3029056574000037 36.1550859533999969, -80.3350449999999938 36.2901949999999971, -80.3290931612999941 36.2910444952999995, -80.7035200220999940 37.8334645230000035)),POLYGON ((-80.7035200220999940 37.8334645230000035, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3029056574000037 36.1550859533999969, -80.3350449999999938 36.2901949999999971, -80.3290931612999941 36.2910444952999995, -80.7035200220999940 37.8334645230000035)),POLYGON ((-80.7035200220999940 37.8334645230000035, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3029056574000037 36.1550859533999969, -80.3350449999999938 36.2901949999999971, -80.3290931612999941 36.2910444952999995, -80.7035200220999940 37.8334645230000035)),POLYGON ((-80.7035200220999940 37.8334645230000035, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3029056574000037 36.1550859533999969, -80.3350449999999938 36.2901949999999971, -80.3290931612999941 36.2910444952999995, -80.7035200220999940 37.8334645230000035)),POLYGON ((-80.7035200220999940 37.8334645230000035, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3029056574000037 36.1550859533999969, -80.3350449999999938 36.2901949999999971, -80.3290931612999941 36.2910444952999995, -80.7035200220999940 37.8334645230000035)),POLYGON ((-80.7033318537000071 37.8334907238999989, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3027267466000012 36.1551115417000020, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.7033318537000071 37.8334907238999989)),POLYGON ((-80.7033318537000071 37.8334907238999989, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3027267466000012 36.1551115417000020, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.7033318537000071 37.8334907238999989)),POLYGON ((-80.7033318537000071 37.8334907238999989, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3027267466000012 36.1551115417000020, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.7033318537000071 37.8334907238999989)),POLYGON ((-80.7033318537000071 37.8334907238999989, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3027267466000012 36.1551115417000020, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.7033318537000071 37.8334907238999989)),POLYGON ((-80.7033318537000071 37.8334907238999989, -77.8330150000000032 38.2331580000000031, -77.4913559999999961 36.5572009999999992, -80.3027267466000012 36.1551115417000020, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.7033318537000071 37.8334907238999989)),POLYGON ((-77.1916992873999988 35.0646299440999982, -79.9493789999999933 34.6608810000000034, -79.9815402769999935 34.7960829197999999, -79.9796941827000012 34.7963526776999998, -80.3349461509999969 36.2897794535999978, -77.5193479999999937 36.6916429999999991, -77.1912175753000014 35.0651371870999995, -77.1917841294000056 35.0650542373999983, -77.1916992873999988 35.0646299440999982)),POLYGON ((-77.1916992873999988 35.0646299440999982, -79.9493789999999933 34.6608810000000034, -79.9815402769999935 34.7960829197999999, -79.9796941827000012 34.7963526776999998, -80.3349461509999969 36.2897794535999978, -77.5193479999999937 36.6916429999999991, -77.1912175753000014 35.0651371870999995, -77.1917841294000056 35.0650542373999983, -77.1916992873999988 35.0646299440999982)),POLYGON ((-77.1916992873999988 35.0646299440999982, -79.9493789999999933 34.6608810000000034, -79.9815402769999935 34.7960829197999999, -79.9796941827000012 34.7963526776999998, -80.3349461509999969 36.2897794535999978, -77.5193479999999937 36.6916429999999991, -77.1912175753000014 35.0651371870999995, -77.1917841294000056 35.0650542373999983, -77.1916992873999988 35.0646299440999982)),POLYGON ((-77.1916992873999988 35.0646299440999982, -79.9493789999999933 34.6608810000000034, -79.9815402769999935 34.7960829197999999, -79.9796941827000012 34.7963526776999998, -80.3349461509999969 36.2897794535999978, -77.5193479999999937 36.6916429999999991, -77.1912175753000014 35.0651371870999995, -77.1917841294000056 35.0650542373999983, -77.1916992873999988 35.0646299440999982)),POLYGON ((-77.1916992873999988 35.0646299440999982, -79.9493789999999933 34.6608810000000034, -79.9815402769999935 34.7960829197999999, -79.9796941827000012 34.7963526776999998, -80.3349461509999969 36.2897794535999978, -77.5193479999999937 36.6916429999999991, -77.1912175753000014 35.0651371870999995, -77.1917841294000056 35.0650542373999983, -77.1916992873999988 35.0646299440999982)),POLYGON ((-77.1917043239999998 35.0646292066999976, -79.9493789999999933 34.6608810000000034, -79.9814658683000062 34.7957701150999981, -79.9794497644000018 34.7960647056999974, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.3288134568000061 36.2906547583000005, -77.5193479999999937 36.6916429999999991, -77.1911517833000005 35.0648110636999988, -77.1917239376000026 35.0647272961000027, -77.1917043239999998 35.0646292066999976)),POLYGON ((-77.1917043239999998 35.0646292066999976, -79.9493789999999933 34.6608810000000034, -79.9814658683000062 34.7957701150999981, -79.9794497644000018 34.7960647056999974, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.3288134568000061 36.2906547583000005, -77.5193479999999937 36.6916429999999991, -77.1911517833000005 35.0648110636999988, -77.1917239376000026 35.0647272961000027, -77.1917043239999998 35.0646292066999976)),POLYGON ((-77.1917043239999998 35.0646292066999976, -79.9493789999999933 34.6608810000000034, -79.9814658683000062 34.7957701150999981, -79.9794497644000018 34.7960647056999974, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.3288134568000061 36.2906547583000005, -77.5193479999999937 36.6916429999999991, -77.1911517833000005 35.0648110636999988, -77.1917239376000026 35.0647272961000027, -77.1917043239999998 35.0646292066999976)),POLYGON ((-77.1917043239999998 35.0646292066999976, -79.9493789999999933 34.6608810000000034, -79.9814658683000062 34.7957701150999981, -79.9794497644000018 34.7960647056999974, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.3288134568000061 36.2906547583000005, -77.5193479999999937 36.6916429999999991, -77.1911517833000005 35.0648110636999988, -77.1917239376000026 35.0647272961000027, -77.1917043239999998 35.0646292066999976)),POLYGON ((-77.1917043239999998 35.0646292066999976, -79.9493789999999933 34.6608810000000034, -79.9814658683000062 34.7957701150999981, -79.9794497644000018 34.7960647056999974, -80.3347629999999953 36.2897910000000010, -80.3288100302000032 36.2906406425000014, -80.3288134568000061 36.2906547583000005, -77.5193479999999937 36.6916429999999991, -77.1911517833000005 35.0648110636999988, -77.1917239376000026 35.0647272961000027, -77.1917043239999998 35.0646292066999976)))
-    repaired wkt: POLYGON ((-76.7264221326474001 32.7272894024876990, -74.7296300000000002 33.0289119999999983, -75.0274073821014156 34.5223866663338868, -75.0272899999999936 34.5224040000000016, -75.0273100668365487 34.5225037710924809, -75.0268480000000011 34.5225719999999967, -75.3384098723529689 36.0717311253983013, -75.3382720000000035 36.0717509999999990, -75.3524806960481897 36.1416945800556491, -75.3640819999999962 36.1993790000000004, -75.3641956813450093 36.1993626453854773, -75.6413374312874112 37.5636177542369865, -75.6411509999999936 37.5636439999999965, -75.6582814345933627 37.6470261294793858, -75.6672590000000014 37.6912189999999967, -75.6673577839198259 37.6912051215892774, -75.9474981448632036 39.0547840618241011, -75.9458159999999936 39.0550459999999973, -75.9459080611074597 39.0554884736670687, -75.9453042850000060 39.0555714301000023, -76.2553244590283157 40.5457561410112604, -76.2535170000000022 40.5460319999999967, -76.2535855987902949 40.5463570933988748, -76.2530284871999982 40.5464317644999994, -76.5942459999999983 42.1636009999999999, -76.5948283463256985 42.1635250370467887, -76.5948869999999999 42.1638030000000015, -76.5961686036928029 42.1636358137983436, -76.9004127223897456 43.5821624664202147, -76.8999971323000011 43.5822153877999980, -76.9002014084947803 43.5831678112159153, -76.9000037682999960 43.5831929766000030, -76.9000304082730253 43.5833150386688857, -76.8994176375999956 43.5833930601000006, -77.2287060000000025 45.0922740000000033, -80.4371509534999944 44.6942759988000020, -80.4371194983870765 44.6941610134865783, -80.4376515447000031 44.6940950095000034, -80.2604154102009346 44.0461764883741935, -82.2518702643999973 43.7951874892999982, -81.8178630000000027 42.1785429999999977, -81.8177043437100906 42.1785635556827145, -81.8176650000000052 42.1784170000000032, -81.8087605703170198 42.1795706145804488, -81.4332364444999968 40.7402257361000011, -81.0736132660060349 39.3256892608491810, -81.0763239999999996 39.3253210000000024, -81.0763025253777414 39.3252345032224397, -81.0764240000000029 39.3252179999999996, -80.7060234353635622 37.8333322863560539, -80.7104505995000068 37.8326588141000002, -80.7104131791847266 37.8325047093423024, -80.7105260000000015 37.8324890000000025, -80.3358773165000031 36.2896465505999970, -80.3367920000000026 36.2895159999999990, -79.9814638414651711 34.7957615943856808, -79.9817280000000039 34.7957230000000024, -79.9816814327263046 34.7955235477923637, -79.9817809999999980 34.7955090000000027, -79.6190240111999969 33.2418556523999982, -79.2584969193000006 31.6709942154000004, -76.5977170000000029 32.0785979999999995, -76.7264221326474001 32.7272894024876990))
+    repaired wkt: POLYGON ((-80.7105260000000000 37.8324890000000000, -80.3358773165000000 36.2896465506000000, -80.3367920000000000 36.2895160000000000, -79.9814638414651700 34.7957615943856800, -79.9817280000000000 34.7957230000000000, -79.9816814327263000 34.7955235477923640, -79.9817810000000000 34.7955090000000000, -79.6190240112000000 33.2418556524000000, -79.2584969193000000 31.6709942154000000, -76.5977170000000000 32.0785980000000000, -76.7264221326473900 32.7272894024877060, -74.7296300000000000 33.0289120000000000, -75.0274073821014200 34.5223866663338900, -75.0272900000000000 34.5224040000000000, -75.0273100668365500 34.5225037710924800, -75.0268480000000000 34.5225720000000000, -75.3384098723529700 36.0717311253983100, -75.3382720000000000 36.0717510000000000, -75.3524806960481800 36.1416945800555640, -75.3640820000000000 36.1993790000000000, -75.3641956813450100 36.1993626453854800, -75.6413374312874100 37.5636177542369900, -75.6411510000000000 37.5636440000000000, -75.6582814345933300 37.6470261294792400, -75.6672590000000000 37.6912190000000000, -75.6673577839198300 37.6912051215892800, -75.9474981448632000 39.0547840618241000, -75.9458160000000000 39.0550460000000000, -75.9459080611074600 39.0554884736670700, -75.9453042850000000 39.0555714301000000, -76.2553244590283200 40.5457561410112600, -76.2535170000000000 40.5460320000000000, -76.2535855987903000 40.5463570933988750, -76.2530284872000000 40.5464317645000000, -76.5942460000000000 42.1636010000000000, -76.5948283463257000 42.1635250370467900, -76.5948870000000000 42.1638030000000000, -76.5961686036928000 42.1636358137983440, -76.9004127223897500 43.5821624664202150, -76.8999971323000000 43.5822153878000000, -76.9002014084947800 43.5831678112159150, -76.9000037683000000 43.5831929766000000, -76.9000304082730300 43.5833150386688860, -76.8994176376000000 43.5833930601000000, -77.2287060000000000 45.0922740000000000, -80.4371509535000000 44.6942759988000000, -80.4371194983870800 44.6941610134865800, -80.4376515447000000 44.6940950095000000, -80.2604154102009300 44.0461764883741900, -82.2518702644000000 43.7951874893000000, -81.8178630000000000 42.1785430000000000, -81.8177043437100900 42.1785635556827150, -81.8176650000000000 42.1784170000000000, -81.8087605703170200 42.1795706145804500, -81.4332364445000000 40.7402257361000000, -81.0736132660060300 39.3256892608491800, -81.0763240000000000 39.3253210000000000, -81.0763025253777300 39.3252345032224400, -81.0764240000000000 39.3252180000000000, -80.7060234353635600 37.8333322863560540, -80.7104505995000000 37.8326588141000000, -80.7104131791847300 37.8325047093423000, -80.7105260000000000 37.8324890000000000))
     repair:
         - "Simplified shape from 84 points to 63 points, after 2 iterations."
         - "Reversed polygon winding order"
 
 - REPAIR Merge individual shapes together and reverse polygon order:
     test wkt: GEOMETRYCOLLECTION(POLYGON((46 -19,30 26,-3 41,22 39,49 16,46 -19)), POLYGON((27 24,12 4,18 31,27 24)))
-    repaired wkt: POLYGON ((46.0000000000000000 -19.0000000000000000, 49.0000000000000000 16.0000000000000000, 22.0000000000000000 39.0000000000000000, -3.0000000000000000 41.0000000000000000, 15.2549019607843128 18.6470588235294130, 12.0000000000000000 4.0000000000000000, 19.2845744680851077 13.7127659574468090, 46.0000000000000000 -19.0000000000000000))
+    repaired wkt: POLYGON ((19.2845744680851080 13.7127659574468090, 46.0000000000000000 -19.0000000000000000, 49.0000000000000000 16.0000000000000000, 22.0000000000000000 39.0000000000000000, -3.0000000000000000 41.0000000000000000, 15.2549019607843130 18.6470588235294130, 12.0000000000000000 4.0000000000000000, 19.2845744680851080 13.7127659574468090))
     repair:
       - 'Unconnected shapes: Convex-halled each INDIVIDUAL shape to merge them together.'
       - 'Reversed polygon winding order'
 
 - REPAIR Merge ALL shapes together and reverse polygon order:
     test wkt: GEOMETRYCOLLECTION (POINT (102.0000000000000000 -90.0000000000000000),POLYGON ((100.0000000000000000 0.0000000000000000, 101.0000000000000000 0.0000000000000000, 101.0000000000000000 1.0000000000000000, 100.0000000000000000 1.0000000000000000, 100.0000000000000000 0.0000000000000000)),LINESTRING (102.0000000000000000 0.0000000000000000, 103.0000000000000000 1.0000000000000000, 104.0000000000000000 0.0000000000000000, 105.0000000000000000 1.0000000000000000),POLYGON ((30.0000000000000000 10.0000000000000000, 40.0000000000000000 40.0000000000000000, 20.0000000000000000 40.0000000000000000, 10.0000000000000000 20.0000000000000000, 30.0000000000000000 10.0000000000000000)))
     repaired wkt: POLYGON ((102.0000000000000000 -90.0000000000000000, 105.0000000000000000 1.0000000000000000, 40.0000000000000000 40.0000000000000000, 20.0000000000000000 40.0000000000000000, 10.0000000000000000 20.0000000000000000, 102.0000000000000000 -90.0000000000000000))
```

