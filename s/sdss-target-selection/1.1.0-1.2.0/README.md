# Comparing `tmp/sdss-target-selection-1.1.0.tar.gz` & `tmp/sdss_target_selection-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-target-selection-1.1.0.tar", last modified: Thu Sep 28 21:45:02 2023, max compression
+gzip compressed data, was "sdss_target_selection-1.2.0.tar", last modified: Wed Apr 24 00:03:19 2024, max compression
```

## Comparing `sdss-target-selection-1.1.0.tar` & `sdss_target_selection-1.2.0.tar`

### file list

```diff
@@ -1,152 +1,81 @@
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.213499 sdss-target-selection-1.1.0/
--rw-r--r--   0 gallegoj   (501) staff       (20)      213 2023-04-19 16:37:23.000000 sdss-target-selection-1.1.0/.flake8
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.094212 sdss-target-selection-1.1.0/.github/
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.104417 sdss-target-selection-1.1.0/.github/workflows/
--rw-r--r--   0 gallegoj   (501) staff       (20)     1153 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/.github/workflows/pythonapp.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     1281 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/.gitignore
--rw-r--r--   0 gallegoj   (501) staff       (20)    14452 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/.pylintrc
--rw-r--r--   0 gallegoj   (501) staff       (20)      149 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/.rstcheck.cfg
--rw-r--r--   0 gallegoj   (501) staff       (20)    11723 2023-09-28 21:43:52.000000 sdss-target-selection-1.1.0/CHANGELOG.md
--rw-r--r--   0 gallegoj   (501) staff       (20)     1288 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/CODEOWNERS
--rw-r--r--   0 gallegoj   (501) staff       (20)     1504 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/LICENSE.md
--rw-r--r--   0 gallegoj   (501) staff       (20)       79 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/MANIFEST.in
--rw-r--r--   0 gallegoj   (501) staff       (20)     3962 2023-09-28 21:45:02.213251 sdss-target-selection-1.1.0/PKG-INFO
--rw-r--r--   0 gallegoj   (501) staff       (20)     1484 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/README.md
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.107863 sdss-target-selection-1.1.0/bin/
--rwxr-xr-x   0 gallegoj   (501) staff       (20)     3854 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/bin/build_sdssv_plateholes
--rwxr-xr-x   0 gallegoj   (501) staff       (20)     3667 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/bin/list_missing_cadences
--rwxr-xr-x   0 gallegoj   (501) staff       (20)     2914 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/bin/recreate_indexes
--rw-r--r--   0 gallegoj   (501) staff       (20)      302 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/bin/target_selection
--rwxr-xr-x   0 gallegoj   (501) staff       (20)     6590 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/bin/yanny_scraper
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.096014 sdss-target-selection-1.1.0/docs/
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.115072 sdss-target-selection-1.1.0/docs/sphinx/
--rw-r--r--   0 gallegoj   (501) staff       (20)      604 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/Makefile
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.122299 sdss-target-selection-1.1.0/docs/sphinx/_static/
--rw-r--r--   0 gallegoj   (501) staff       (20)   121256 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/Catalogdb_Crossmatch.graffle
--rw-r--r--   0 gallegoj   (501) staff       (20)   106177 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/Catalogdb_Crossmatch.png
--rw-r--r--   0 gallegoj   (501) staff       (20)      544 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/custom.css
--rw-r--r--   0 gallegoj   (501) staff       (20)     1690 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/custom_bootstrap.css
--rw-r--r--   0 gallegoj   (501) staff       (20)     1150 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/favicon_sdssv.ico
--rw-r--r--   0 gallegoj   (501) staff       (20)     5010 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/pygments.css
--rw-r--r--   0 gallegoj   (501) staff       (20)   121846 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/sample_graph.graffle
--rw-r--r--   0 gallegoj   (501) staff       (20)    21927 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/sample_graph.png
--rw-r--r--   0 gallegoj   (501) staff       (20)    42239 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/sdssv_logo.png
--rw-r--r--   0 gallegoj   (501) staff       (20)     7404 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_static/sdssv_logo_small.png
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.123993 sdss-target-selection-1.1.0/docs/sphinx/_templates/
--rw-r--r--   0 gallegoj   (501) staff       (20)       32 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_templates/fulltoc.html
--rw-r--r--   0 gallegoj   (501) staff       (20)      162 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/_templates/layout.html
--rw-r--r--   0 gallegoj   (501) staff       (20)      607 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/docs/sphinx/api.rst
--rw-r--r--   0 gallegoj   (501) staff       (20)       67 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/docs/sphinx/changelog.md
--rw-r--r--   0 gallegoj   (501) staff       (20)     1787 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/cli.rst
--rw-r--r--   0 gallegoj   (501) staff       (20)     6813 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/docs/sphinx/conf.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    21684 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/cross-match.rst
--rw-r--r--   0 gallegoj   (501) staff       (20)    15661 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/database.rst
--rw-r--r--   0 gallegoj   (501) staff       (20)      852 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/docs/sphinx/index.rst
--rw-r--r--   0 gallegoj   (501) staff       (20)      800 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/docs/sphinx/skies.rst
--rw-r--r--   0 gallegoj   (501) staff       (20)     5515 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/docs/sphinx/tagging.rst
--rw-r--r--   0 gallegoj   (501) staff       (20)    18966 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/docs/sphinx/target-selection.rst
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.095787 sdss-target-selection-1.1.0/docs/v1_documentation/
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.138368 sdss-target-selection-1.1.0/docs/v1_documentation/catalog_to_catalog/
--rw-r--r--   0 gallegoj   (501) staff       (20)      276 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/catalog_to_catalog/cat_to_cat.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)    18948 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/catalog_to_catalog/catalog_to_catalog.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     3005 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/catalog_to_catalog/catalog_to_catalog_description.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)     1849 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/catalog_to_catalog/catalog_to_catalog_statistics.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)  4732555 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/catalog_to_catalog/catalog_ver25_to_ver31_non_matched.csv
--rw-r--r--   0 gallegoj   (501) staff       (20)     1558 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/catalog_to_catalog/individual_crossmatches.yml
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.140045 sdss-target-selection-1.1.0/docs/v1_documentation/duplicates/
--rw-r--r--   0 gallegoj   (501) staff       (20)   185547 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/duplicates/duplicates_info_statistics.pages
--rw-r--r--   0 gallegoj   (501) staff       (20)    17591 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/duplicates/v1_duplicates_table_creation.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.147749 sdss-target-selection-1.1.0/docs/v1_documentation/v1_crossmatch/
--rw-r--r--   0 gallegoj   (501) staff       (20)   618458 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/v1_crossmatch/catalogdb-v1.drawio.png
--rw-r--r--   0 gallegoj   (501) staff       (20)     1394 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/v1_crossmatch/caveats.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)   387832 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/v1_crossmatch/changes_to_codes_from_v0p5_to_v1.pages
--rw-r--r--   0 gallegoj   (501) staff       (20)   220535 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/v1_crossmatch/crossmatch_statistics_v1.0.numbers
--rw-r--r--   0 gallegoj   (501) staff       (20)   797382 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/v1_crossmatch/duplicates.key
--rw-r--r--   0 gallegoj   (501) staff       (20)     6063 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/v1_documentation/v1_crossmatch/how_to_link_non_crossmatched_tables_to_catalog.txt
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.096150 sdss-target-selection-1.1.0/docs/website/
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.150632 sdss-target-selection-1.1.0/docs/website/bhm_cartons/
--rw-r--r--   0 gallegoj   (501) staff       (20)     7621 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/website/bhm_cartons/README_build_tables.sh
--rw-r--r--   0 gallegoj   (501) staff       (20)    73346 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/website/bhm_cartons/bhm_target_cartons.html
--rw-r--r--   0 gallegoj   (501) staff       (20)    60502 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/website/bhm_cartons/bhm_target_cartons.tex
--rw-r--r--   0 gallegoj   (501) staff       (20)    53201 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/website/bhm_cartons/carton_descriptions.json
--rw-r--r--   0 gallegoj   (501) staff       (20)     2335 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/docs/website/bhm_cartons/proc_carton_desc.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.151747 sdss-target-selection-1.1.0/etc/
--rw-r--r--   0 gallegoj   (501) staff       (20)      146 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/etc/config.ini
--rw-r--r--   0 gallegoj   (501) staff       (20)     2501 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/etc/target_selection.module
--rw-r--r--   0 gallegoj   (501) staff       (20)     1061 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/noxfile.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.096898 sdss-target-selection-1.1.0/python/
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.154718 sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/
--rw-r--r--   0 gallegoj   (501) staff       (20)     3962 2023-09-28 21:45:02.000000 sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/PKG-INFO
--rw-r--r--   0 gallegoj   (501) staff       (20)     5440 2023-09-28 21:45:02.000000 sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/SOURCES.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)        1 2023-09-28 21:45:02.000000 sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/dependency_links.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)        1 2023-01-06 19:32:19.000000 sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/not-zip-safe
--rw-r--r--   0 gallegoj   (501) staff       (20)      618 2023-09-28 21:45:02.000000 sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/requires.txt
--rw-r--r--   0 gallegoj   (501) staff       (20)       17 2023-09-28 21:45:02.000000 sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/top_level.txt
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.158168 sdss-target-selection-1.1.0/python/target_selection/
--rw-r--r--   0 gallegoj   (501) staff       (20)      718 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/__init__.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    11216 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/__main__.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.184529 sdss-target-selection-1.1.0/python/target_selection/cartons/
--rw-r--r--   0 gallegoj   (501) staff       (20)     1079 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/__init__.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    49750 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/base.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    11674 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_aqmes.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    13826 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_csc.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    11105 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_galaxies.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    10763 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_gua.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    14152 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_rm.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    52812 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_spiders_agn.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    16838 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_spiders_clusters.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     2654 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/guide.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    12336 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_bin_gaia.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     5621 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_bin_vis.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    45489 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_cb.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     3361 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_cb_cvcandidates.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    13869 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_dust.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    13013 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_erosita.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    10863 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_galactic.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     8713 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_halo.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    50754 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_halo_gaia_dr3.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     5476 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_legacy_ir2opt.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     7694 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_magcloud_agb.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     7060 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_magcloud_rgb.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    14468 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_monitor_apogee.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     9872 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_ob.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     4055 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_planet.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    26484 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_rv.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    17466 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_snc.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     4079 2023-04-19 16:37:23.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_tess_ob.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     6738 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_tess_rgb.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     4882 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_wd.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    71200 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_yso.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     7568 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/ops_apogee_stds.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    59366 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/ops_boss_stds.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    12519 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/ops_bright_stars.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    15848 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/ops_skies.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     5789 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/skymask.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    21933 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/cartons/tools.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.190463 sdss-target-selection-1.1.0/python/target_selection/config/
--rw-r--r--   0 gallegoj   (501) staff       (20)   145936 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/config/target_selection.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     9866 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/config/target_selection_v0.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     8761 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/config/xmatch_v0.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     6480 2023-04-19 16:37:23.000000 sdss-target-selection-1.1.0/python/target_selection/config/xmatch_v0p5.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)    32525 2023-09-28 21:43:52.000000 sdss-target-selection-1.1.0/python/target_selection/config/xmatch_v1.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     1383 2023-09-25 17:14:33.000000 sdss-target-selection-1.1.0/python/target_selection/exceptions.py
--rw-r--r--   0 gallegoj   (501) staff       (20)     3148 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/mag_flux.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.206541 sdss-target-selection-1.1.0/python/target_selection/masks/
--rw-r--r--   0 gallegoj   (501) staff       (20)     4171 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply
--rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)     8640 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)   348269 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply
--rw-r--r--   0 gallegoj   (501) staff       (20)   135360 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/masks/rsFields_boss_survey.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)    40320 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/masks/rsFields_boss_survey_sgc.fits
--rw-r--r--   0 gallegoj   (501) staff       (20)    37638 2023-02-07 16:26:59.000000 sdss-target-selection-1.1.0/python/target_selection/skies.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    10703 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/python/target_selection/utils.py
--rw-r--r--   0 gallegoj   (501) staff       (20)    88957 2023-09-28 21:44:18.000000 sdss-target-selection-1.1.0/python/target_selection/xmatch.py
--rw-r--r--   0 gallegoj   (501) staff       (20)      282 2023-04-19 16:37:23.000000 sdss-target-selection-1.1.0/readthedocs.yml
--rw-r--r--   0 gallegoj   (501) staff       (20)     2535 2023-09-28 21:45:02.214818 sdss-target-selection-1.1.0/setup.cfg
--rw-r--r--   0 gallegoj   (501) staff       (20)       73 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/setup.py
-drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2023-09-28 21:45:02.208582 sdss-target-selection-1.1.0/tests/
--rw-r--r--   0 gallegoj   (501) staff       (20)        0 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/tests/__init__.py
--rw-r--r--   0 gallegoj   (501) staff       (20)      475 2022-11-28 16:42:41.000000 sdss-target-selection-1.1.0/tests/conftest.py
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.799222 sdss_target_selection-1.2.0/
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     1504 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/LICENSE.md
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)       79 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/MANIFEST.in
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     3968 2024-04-24 00:03:19.799222 sdss_target_selection-1.2.0/PKG-INFO
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1484 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/README.md
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.787222 sdss_target_selection-1.2.0/bin/
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)      302 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/bin/target_selection
+-rwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)     6590 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/bin/yanny_scraper
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.787222 sdss_target_selection-1.2.0/python/
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.795222 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     3968 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/PKG-INFO
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     3296 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/SOURCES.txt
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)        1 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/dependency_links.txt
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)        1 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/not-zip-safe
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)      624 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/requires.txt
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)       17 2024-04-24 00:03:19.000000 sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/top_level.txt
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.787222 sdss_target_selection-1.2.0/python/target_selection/
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)      718 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/__init__.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11216 2023-05-17 22:25:33.000000 sdss_target_selection-1.2.0/python/target_selection/__main__.py
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.791222 sdss_target_selection-1.2.0/python/target_selection/cartons/
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1079 2023-06-01 13:48:09.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/__init__.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    50847 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/base.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11674 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_aqmes.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13826 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_csc.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    11105 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_galaxies.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    10763 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_gua.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    14152 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_rm.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    52812 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_spiders_agn.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    16838 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_spiders_clusters.py
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     2654 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/guide.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    12336 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_bin_gaia.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     5621 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_bin_vis.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    45489 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_cb.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     3361 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_cb_cvcandidates.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13869 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_dust.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    13013 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_erosita.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    10863 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_galactic.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8713 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_halo.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    50754 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_halo_gaia_dr3.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     5476 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_legacy_ir2opt.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7694 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_magcloud_agb.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7060 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_magcloud_rgb.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    14468 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_monitor_apogee.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     9872 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_ob.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4055 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_planet.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    25410 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_rv.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    17466 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_snc.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4079 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_tess_ob.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     6738 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_tess_rgb.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     4882 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_wd.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    71200 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_yso.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     7568 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/ops_apogee_stds.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    59366 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/ops_boss_stds.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    12519 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/ops_bright_stars.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    15848 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/ops_skies.py
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     5789 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/skymask.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     2161 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/too.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    21933 2023-05-18 08:21:33.000000 sdss_target_selection-1.2.0/python/target_selection/cartons/tools.py
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.795222 sdss_target_selection-1.2.0/python/target_selection/config/
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)   147249 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.0/python/target_selection/config/target_selection.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     9866 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/config/target_selection_v0.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8761 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v0.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     6480 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v0p5.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    32525 2024-04-13 21:50:23.000000 sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v1.yml
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     1383 2023-06-01 20:51:59.000000 sdss_target_selection-1.2.0/python/target_selection/exceptions.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     3148 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/mag_flux.py
+drwxrwxr-x   0 gallegoj  (1004) gallegoj  (1005)        0 2024-04-24 00:03:19.795222 sdss_target_selection-1.2.0/python/target_selection/masks/
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     4171 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)     8640 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)   348269 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)   135360 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/rsFields_boss_survey.fits
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    40320 2021-05-24 23:45:27.000000 sdss_target_selection-1.2.0/python/target_selection/masks/rsFields_boss_survey_sgc.fits
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    37638 2023-05-11 16:17:06.000000 sdss_target_selection-1.2.0/python/target_selection/skies.py
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)    10703 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/python/target_selection/utils.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)    86433 2024-04-23 23:42:23.000000 sdss_target_selection-1.2.0/python/target_selection/xmatch.py
+-rw-rw-r--   0 gallegoj  (1004) gallegoj  (1005)     2541 2024-04-24 00:03:19.799222 sdss_target_selection-1.2.0/setup.cfg
+-rw-r--r--   0 gallegoj  (1004) gallegoj  (1005)       73 2021-05-24 23:45:26.000000 sdss_target_selection-1.2.0/setup.py
```

### Comparing `sdss-target-selection-1.1.0/LICENSE.md` & `sdss_target_selection-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/PKG-INFO` & `sdss_target_selection-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-target-selection
-Version: 1.1.0
+Version: 1.2.0
 Summary: Code to perform target selection for BHM/MWM using catalogdb
 Home-page: https://github.com/sdss/target_selection
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/target_selection
 Project-URL: Documentation, https://sdss-target-selection.readthedocs.org
@@ -19,23 +19,23 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: pydl>=1.0.0rc1
-Requires-Dist: sdssdb>=0.6.2
+Requires-Dist: sdssdb>=0.10.0
 Requires-Dist: click>=7.0
 Requires-Dist: astropy>=5.0.0
 Requires-Dist: networkx>=2.4
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: healpy>=1.13.0
-Requires-Dist: pymangle>=0.9.1
+Requires-Dist: sdss-pymangle>=0.9.3
 Requires-Dist: tables>=3.6.1
-Requires-Dist: sdsstools>=1.0.0
+Requires-Dist: sdsstools>=1.6.0
 Requires-Dist: enlighten>=1.4.0
 Requires-Dist: mocpy>=0.8.5
 Requires-Dist: pymoc>=0.5.0
 Requires-Dist: gala>=1.6.1
 Requires-Dist: matplotlib>=3.1.1
 Requires-Dist: dustmaps==1.0.10
 Provides-Extra: dev
```

### Comparing `sdss-target-selection-1.1.0/README.md` & `sdss_target_selection-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/bin/yanny_scraper` & `sdss_target_selection-1.2.0/bin/yanny_scraper`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/PKG-INFO` & `sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-target-selection
-Version: 1.1.0
+Version: 1.2.0
 Summary: Code to perform target selection for BHM/MWM using catalogdb
 Home-page: https://github.com/sdss/target_selection
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/target_selection
 Project-URL: Documentation, https://sdss-target-selection.readthedocs.org
@@ -19,23 +19,23 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: pydl>=1.0.0rc1
-Requires-Dist: sdssdb>=0.6.2
+Requires-Dist: sdssdb>=0.10.0
 Requires-Dist: click>=7.0
 Requires-Dist: astropy>=5.0.0
 Requires-Dist: networkx>=2.4
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: healpy>=1.13.0
-Requires-Dist: pymangle>=0.9.1
+Requires-Dist: sdss-pymangle>=0.9.3
 Requires-Dist: tables>=3.6.1
-Requires-Dist: sdsstools>=1.0.0
+Requires-Dist: sdsstools>=1.6.0
 Requires-Dist: enlighten>=1.4.0
 Requires-Dist: mocpy>=0.8.5
 Requires-Dist: pymoc>=0.5.0
 Requires-Dist: gala>=1.6.1
 Requires-Dist: matplotlib>=3.1.1
 Requires-Dist: dustmaps==1.0.10
 Provides-Extra: dev
```

### Comparing `sdss-target-selection-1.1.0/python/sdss_target_selection.egg-info/requires.txt` & `sdss_target_selection-1.2.0/python/sdss_target_selection.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 numpy>=1.18.1
 pydl>=1.0.0rc1
-sdssdb>=0.6.2
+sdssdb>=0.10.0
 click>=7.0
 astropy>=5.0.0
 networkx>=2.4
 pandas>=1.0.0
 healpy>=1.13.0
-pymangle>=0.9.1
+sdss-pymangle>=0.9.3
 tables>=3.6.1
-sdsstools>=1.0.0
+sdsstools>=1.6.0
 enlighten>=1.4.0
 mocpy>=0.8.5
 pymoc>=0.5.0
 gala>=1.6.1
 matplotlib>=3.1.1
 dustmaps==1.0.10
```

### Comparing `sdss-target-selection-1.1.0/python/target_selection/__init__.py` & `sdss_target_selection-1.2.0/python/target_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/__main__.py` & `sdss_target_selection-1.2.0/python/target_selection/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/__init__.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/base.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,20 +251,20 @@
         query_region = query_region or self.query_region
 
         path = self.path
         execute_sql = self.database.execute_sql
 
         if self.database.table_exists(self.table_name, schema=self.schema):
             if overwrite:
-                log.info(f'Dropping table {path!r}.')
+                self.log.info(f'Dropping table {path!r}.')
                 self.drop_table()
             else:
                 raise RuntimeError(f'Temporary table {path!r} already exists.')
 
-        log.info('Running query ...')
+        self.log.info('Running query ...')
         version_id = self.get_version_id()
 
         with Timer() as timer:
             # If build_query accepts a query_region parameter, call with the query region.
             # Otherwise will add the radial query condition later.
             if 'query_region' in self._build_query_signature.parameters:
                 query = self.build_query(version_id, query_region=query_region)
@@ -300,29 +300,32 @@
                 query = query.limit(limit)
 
             query_sql, params = self.database.get_sql_context().sql(query).query()
             cursor = self.database.cursor()
             query_str = cursor.mogrify(query_sql, params).decode()
 
             if not self._disable_query_log:
-                log.debug(color_text(f'CREATE TABLE IF NOT EXISTS {path} AS ' + query_str,
-                                     'darkgrey'))
+                log_message = f'CREATE TABLE IF NOT EXISTS {path} AS ' + query_str
+                if self.log.rich_console:
+                    self.log.debug(log_message, extra={"highlighter": None})
+                else:
+                    self.log.debug(color_text(log_message, 'darkgrey'))
             else:
-                log.debug('Not printing VERY long query.')
+                self.log.debug('Not printing VERY long query.')
 
             with self.database.atomic():
                 self.setup_transaction()
                 execute_sql(f'CREATE TABLE IF NOT EXISTS {path} AS ' + query_sql,
                             params)
 
-        log.info(f'Created table {path!r} in {timer.interval:.3f} s.')
+        self.log.info(f'Created table {path!r} in {timer.interval:.3f} s.')
 
         self.RModel = self.get_model()
 
-        log.debug('Adding columns and indexes.')
+        self.log.debug('Adding columns and indexes.')
 
         columns = [
             col.name for col in self.database.get_columns(self.table_name, self.schema)
         ]
 
         if 'selected' not in columns:
             execute_sql(f'ALTER TABLE {path} ADD COLUMN selected BOOL DEFAULT TRUE;')
@@ -341,26 +344,26 @@
             self.RModel._meta.add_field('instrument', peewee.TextField())
 
         execute_sql(f'ALTER TABLE {path} ADD PRIMARY KEY (catalogid);')
         execute_sql(f'CREATE INDEX ON {path} (selected);')
         execute_sql(f'ANALYZE {path};')
 
         n_rows = self.RModel.select().count()
-        log.debug(f'Table {path!r} contains {n_rows:,} rows.')
+        self.log.debug(f'Table {path!r} contains {n_rows:,} rows.')
 
-        log.debug('Running post-process.')
+        self.log.debug('Running post-process.')
         with self.database.atomic():
             self.setup_transaction()
             self.post_process(self.RModel, **post_process_kawrgs)
 
         n_selected = self.RModel.select().where(self.RModel.selected >> True).count()
-        log.debug(f'Selected {n_selected:,} rows after post-processing.')
+        self.log.debug(f'Selected {n_selected:,} rows after post-processing.')
 
         if add_optical_magnitudes:
-            log.debug('Adding optical magnitude columns.')
+            self.log.debug('Adding optical magnitude columns.')
             self.add_optical_magnitudes()
 
         self.has_run = True
 
         return self.RModel
 
     def get_version_id(self):
@@ -376,20 +379,18 @@
         magnitudes = ['g', 'r', 'i', 'z']
 
         # Check if ALL the columns have already been created in the query.
         # If so, just return.
         if any([mag in Model._meta.columns for mag in magnitudes]):
             if not all([mag in Model._meta.columns for mag in magnitudes]):
                 raise TargetSelectionError(
-                    'Some optical magnitudes are defined in the query '
-                    'but not all of them.')
+                    'Some optical magnitudes are defined in the query but not all of them.')
             if 'optical_prov' not in Model._meta.columns:
                 raise TargetSelectionError('optical_prov column does not exist.')
-            warnings.warn('All optical magnitude columns are defined in the query.',
-                          TargetSelectionUserWarning)
+            self.log.warning('All optical magnitude columns are defined in the query.')
             return
 
         # First create the columns. Also create z to speed things up. We won't
         # use transformations for z but we can use the initial query to populate
         # it and avoid doing the same query later when loading the magnitudes.
         for mag in magnitudes:
             self.database.execute_sql(f'ALTER TABLE {self.path} ADD COLUMN {mag} REAL;')
@@ -712,15 +713,15 @@
 
         if not filename:
             if mode == 'results':
                 filename = f'{self.name}_{self.plan}.fits.gz'
             else:
                 filename = f'{self.name}_{self.plan}_targetdb.fits.gz'
 
-        log.debug(f'Writing table to {filename}.')
+        self.log.debug(f'Writing table to {filename}.')
 
         if not self.RModel:
             self.RModel = self.get_model()
 
         if mode == 'results':
 
             results_model = self.RModel
@@ -789,32 +790,55 @@
         carton_table = table.Table(rows=results, names=colnames, masked=True)
 
         if write:
             carton_table.write(filename, overwrite=True)
 
         return carton_table
 
-    def load(self, overwrite=False):
-        """Loads the output of the intermediate table into targetdb."""
+    def load(self, mode='fail', overwrite=False):
+        """Loads the output of the intermediate table into targetdb.
+
+        Parameters
+        ----------
+        mode : str
+            The mode to use when loading the targets. If ``'fail'``, raises an
+            error if the carton already exist. If ``'overwrite'``, overwrites
+            the targets. If ``'append'``, appends the targets.
+        overwrite : bool
+            Equivalent to setting ``mode='overwrite'``. This option is deprecated and
+            will raise a warning.
+
+        """
+
+        if overwrite:
+            mode = 'overwrite'
+            warnings.warn(
+                'The `overwrite` option is deprecated and will be removed in a future version. '
+                'Use `mode="overwrite"` instead.',
+                TargetSelectionUserWarning)
 
         if self.check_targets():
-            if overwrite:
+            if mode == 'overwrite':
                 warnings.warn(
                     f'Carton {self.name!r} with plan {self.plan!r} '
                     f'already has targets loaded. '
                     'Dropping carton-to-target entries.',
                     TargetSelectionUserWarning,
                 )
                 self.drop_carton()
-            else:
+            elif mode == 'append':
+                pass
+            elif mode == 'fail':
                 raise TargetSelectionError(
                     f'Found existing targets for '
                     f'carton {self.name!r} with plan '
                     f'{self.plan!r}.'
                 )
+            else:
+                raise ValueError(f'Invalid mode {mode!r}. Use "fail", "overwrite", or "append".')
 
         if self.RModel is None:
             RModel = self.get_model()
         else:
             RModel = self.RModel
 
         if not RModel.table_exists():
@@ -868,15 +892,15 @@
             tag=self.tag,
             target_selection=True,
             robostrategy=False
         )
         version_pk = version.pk
 
         if created:
-            log.info(
+            self.log.info(
                 f'Created record in targetdb.version for '
                 f'{self.plan!r} with tag {self.tag!r}.'
             )
 
         if (
             tdb.Carton.select()
             .where(tdb.Carton.carton == self.name, tdb.Carton.version_pk == version_pk)
@@ -885,37 +909,37 @@
             return
 
         # Create carton and associated values.
         if self.mapper:
             mapper, created_pk = tdb.Mapper.get_or_create(label=self.mapper)
             mapper_pk = mapper.pk
             if created:
-                log.debug(f'Created mapper {self.mapper!r}')
+                self.log.debug(f'Created mapper {self.mapper!r}')
 
         if self.category:
             category, created = tdb.Category.get_or_create(label=self.category)
             category_pk = category.pk
             if created:
-                log.debug(f'Created category {self.category!r}')
+                self.log.debug(f'Created category {self.category!r}')
 
         tdb.Carton.create(
             carton=self.name,
             category_pk=category_pk,
             program=self.program,
             mapper_pk=mapper_pk,
             version_pk=version_pk,
             run_on=datetime.datetime.now().isoformat().split('T')[0]
         ).save()
 
-        log.debug(f'Created carton {self.name!r}')
+        self.log.debug(f'Created carton {self.name!r}')
 
     def _load_targets(self, RModel):
         """Load data from the intermediate table tp targetdb.target."""
 
-        log.debug('loading data into targetdb.target.')
+        self.log.debug('loading data into targetdb.target.')
 
         n_inserted = (  # noqa: 841
             tdb.Target.insert_from(
                 cdb.Catalog.select(
                     cdb.Catalog.catalogid,
                     cdb.Catalog.ra,
                     cdb.Catalog.dec,
@@ -943,22 +967,22 @@
                     tdb.Target.epoch,
                 ],
             )
             .returning()
             .execute()
         )
 
-        log.info('Inserted new rows into targetdb.target.')
+        self.log.info('Inserted new rows into targetdb.target.')
 
         return
 
     def _load_magnitudes(self, RModel):
         """Load magnitudes into targetdb.magnitude."""
 
-        log.debug('Loading data into targetdb.magnitude.')
+        self.log.debug('Loading data into targetdb.magnitude.')
 
         Magnitude = tdb.Magnitude
 
         magnitude_paths = self.config['magnitudes']
         fields = [Magnitude.carton_to_target_pk]
 
         select_from = (
@@ -1031,20 +1055,20 @@
             raise TargetSelectionError('optical_prov column not found in temporary table.')
 
         select_from = select_from.select_extend(RModel._meta.columns['optical_prov'])
         fields.append(Magnitude.optical_prov)
 
         n_inserted = Magnitude.insert_from(select_from, fields).returning().execute()  # noqa: 841
 
-        log.info('Inserted new rows into targetdb.magnitude.')
+        self.log.info('Inserted new rows into targetdb.magnitude.')
 
     def _load_carton_to_target(self, RModel):
         """Populate targetdb.carton_to_target."""
 
-        log.debug('Loading data into targetdb.carton_to_target.')
+        self.log.debug('Loading data into targetdb.carton_to_target.')
 
         version_pk = tdb.Version.get(
             plan=self.plan,
             tag=self.tag,
             target_selection=True,
         )
         carton_pk = tdb.Carton.get(carton=self.name, version_pk=version_pk).pk
@@ -1224,15 +1248,15 @@
                     CartonToTarget.lambda_eff
                 ],
             )
             .returning()
             .execute()
         )
 
-        log.info('Inserted rows into targetdb.carton_to_target.')
+        self.log.info('Inserted rows into targetdb.carton_to_target.')
 
     def drop_carton(self):
         """Drops the entry in ``targetdb.carton``."""
 
         version = tdb.Version.select().where(
             tdb.Version.plan == self.plan,
             tdb.Version.tag == self.tag,
```

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_aqmes.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_aqmes.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_csc.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_csc.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_galaxies.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_galaxies.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_gua.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_gua.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_rm.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_rm.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_spiders_agn.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_spiders_agn.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/bhm_spiders_clusters.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/bhm_spiders_clusters.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/guide.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/guide.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_bin_gaia.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_bin_gaia.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_bin_vis.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_bin_vis.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_cb.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_cb.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_cb_cvcandidates.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_cb_cvcandidates.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_dust.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_dust.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_erosita.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_erosita.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_galactic.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_galactic.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_halo.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_halo.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_halo_gaia_dr3.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_halo_gaia_dr3.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_legacy_ir2opt.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_legacy_ir2opt.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_magcloud_agb.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_magcloud_agb.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_magcloud_rgb.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_magcloud_rgb.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_monitor_apogee.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_monitor_apogee.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_ob.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_ob.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_planet.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_planet.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_rv.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_rv.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 #
 # @Author: Pramod Gupta (psgupta@uw.edu)
 # @Date: 2020-06-10
 # @Filename: mwm_rv.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 import math
-import random
 
 import peewee
 
 from sdssdb.peewee.sdss5db.catalogdb import (Catalog, CatalogToGaia_DR3,
                                              CatalogToTIC_v8,
                                              CatalogToTwoMassPSC, Gaia_DR3,
                                              SDSS_DR17_APOGEE_Allstarmerge,
@@ -661,35 +660,7 @@
                             TwoMassPSC.h_m < 10.8,
                             Gaia_DR3.logg_gspphot > 1.2,
                             Gaia_DR3.logg_gspphot <= 3.0,
                             Gaia_DR3.teff_gspphot < 5500,
                             Gaia_DR3.parallax_error / Gaia_DR3.parallax < 0.2,
                             *mwm_rv_short_condition)
         return query
-
-    def post_process(self, model):
-        """
-        a set random seed, select 1/2 of the targets
-        """
-
-        cursor = self.database.execute_sql(
-            "update sandbox.temp_mwm_bin_rv_short_rgb_apogee " +
-            "set selected = false;")
-
-        # The below "order by catalogid" ensures that the random selection
-        # further below gives the same result every time we run this carton.
-        cursor = self.database.execute_sql(
-            "select catalogid from " +
-            " sandbox.temp_mwm_bin_rv_short_rgb_apogee " +
-            " order by catalogid;")
-
-        output = cursor.fetchall()
-
-        random.seed(9123)
-        for i in range(len(output)):
-            current_catalogid = output[i][0]
-            current_random = random.randrange(2)
-            if (current_random == 0):
-                self.database.execute_sql(
-                    " update sandbox.temp_mwm_bin_rv_short_rgb_apogee " +
-                    " set selected = true " +
-                    " where catalogid = " + str(current_catalogid) + ";")
```

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_snc.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_snc.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_tess_ob.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_tess_ob.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_tess_rgb.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_tess_rgb.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_wd.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_wd.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/mwm_yso.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/mwm_yso.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/ops_apogee_stds.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/ops_apogee_stds.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/ops_boss_stds.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/ops_boss_stds.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/ops_bright_stars.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/ops_bright_stars.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/ops_skies.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/ops_skies.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/skymask.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/skymask.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/cartons/tools.py` & `sdss_target_selection-1.2.0/python/target_selection/cartons/tools.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/config/target_selection.yml` & `sdss_target_selection-1.2.0/python/target_selection/config/target_selection.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+'1.1.0': # This is a dedicated plan for ToO
+  xmatch_plan: 1.0.0
+  cartons:
+    - too
+  schema: sandbox
+  magnitudes:
+    h: [catalog_to_twomass_psc, twomass_psc, twomass_psc.h_m]
+    j: [catalog_to_twomass_psc, twomass_psc, twomass_psc.j_m]
+    k: [catalog_to_twomass_psc, twomass_psc, twomass_psc.k_m]
+    bp: [catalog_to_gaia_dr3_source, gaia_dr3_source, gaia_dr3_source.phot_bp_mean_mag]
+    rp: [catalog_to_gaia_dr3_source, gaia_dr3_source, gaia_dr3_source.phot_rp_mean_mag]
+    gaia_g: [catalog_to_gaia_dr3_source, gaia_dr3_source, gaia_dr3_source.phot_g_mean_mag]
+  database_options:
+    work_mem: '5GB'
+
+'1.0.51':
+  xmatch_plan: 1.0.0
+  cartons:
+    - mwm_bin_rv_short_rgb_apogee
+  open_fiber_path: /uufs/chpc.utah.edu/common/home/sdss50/sdsswork/target/open_fiber/1.0.0/draft2/
+  schema: sandbox
+  magnitudes:
+    h: [catalog_to_twomass_psc, twomass_psc, twomass_psc.h_m]
+    j: [catalog_to_twomass_psc, twomass_psc, twomass_psc.j_m]
+    k: [catalog_to_twomass_psc, twomass_psc, twomass_psc.k_m]
+    bp: [catalog_to_gaia_dr3_source, gaia_dr3_source, gaia_dr3_source.phot_bp_mean_mag]
+    rp: [catalog_to_gaia_dr3_source, gaia_dr3_source, gaia_dr3_source.phot_rp_mean_mag]
+    gaia_g: [catalog_to_gaia_dr3_source, gaia_dr3_source, gaia_dr3_source.phot_g_mean_mag]
+  database_options:
+    work_mem: '5GB'
+
 '1.0.50':
   xmatch_plan: 1.0.0
   cartons:
     - mwm_magcloud_agb_apogee
     - mwm_magcloud_rgb_boss
   open_fiber_path: /uufs/chpc.utah.edu/common/home/sdss50/sdsswork/target/open_fiber/1.0.0/draft2/
   schema: sandbox
```

### Comparing `sdss-target-selection-1.1.0/python/target_selection/config/target_selection_v0.yml` & `sdss_target_selection-1.2.0/python/target_selection/config/target_selection_v0.yml`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/config/xmatch_v0.yml` & `sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v0.yml`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/config/xmatch_v0p5.yml` & `sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v0p5.yml`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/config/xmatch_v1.yml` & `sdss_target_selection-1.2.0/python/target_selection/config/xmatch_v1.yml`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/exceptions.py` & `sdss_target_selection-1.2.0/python/target_selection/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/mag_flux.py` & `sdss_target_selection-1.2.0/python/target_selection/mag_flux.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply` & `sdss_target_selection-1.2.0/python/target_selection/masks/AQMES_wboss_imaging_NGC_proc.ply`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits` & `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits` & `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_med_v0.3.1.fits`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits` & `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits` & `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_aqmes_wide_v0.3.1.fits`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits` & `sdss_target_selection-1.2.0/python/target_selection/masks/candidate_target_fields_bhm_rm_v0.2.1.fits`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply` & `sdss_target_selection-1.2.0/python/target_selection/masks/rsFields-annotated-lco-deep_proc.ply`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/rsFields_boss_survey.fits` & `sdss_target_selection-1.2.0/python/target_selection/masks/rsFields_boss_survey.fits`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/masks/rsFields_boss_survey_sgc.fits` & `sdss_target_selection-1.2.0/python/target_selection/masks/rsFields_boss_survey_sgc.fits`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/skies.py` & `sdss_target_selection-1.2.0/python/target_selection/skies.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/utils.py` & `sdss_target_selection-1.2.0/python/target_selection/utils.py`

 * *Files identical despite different names*

### Comparing `sdss-target-selection-1.1.0/python/target_selection/xmatch.py` & `sdss_target_selection-1.2.0/python/target_selection/xmatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,48 +2,44 @@
 # -*- coding: utf-8 -*-
 #
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
 # @Date: 2020-04-06
 # @Filename: xmatch.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
+import copy
 import hashlib
 import inspect
 import os
 import re
 import types
 import uuid
 import warnings
 
 import networkx
 import numpy
 import peewee
+import rich.markup
 import yaml
 from networkx.algorithms import shortest_path
 from peewee import SQL, Case, Model, fn
+
 from sdssdb.connection import PeeweeDatabaseConnection
 from sdssdb.utils.internals import get_row_count
 from sdsstools import merge_config
 from sdsstools._vendor.color_print import color_text
 
 import target_selection
-from target_selection.exceptions import (
-    TargetSelectionNotImplemented,
-    TargetSelectionUserWarning,
-    XMatchError,
-)
-from target_selection.utils import (
-    Timer,
-    get_configuration_values,
-    get_epoch,
-    is_view,
-    sql_apply_pm,
-    vacuum_outputs,
-    vacuum_table,
-)
+from target_selection.exceptions import (TargetSelectionNotImplemented,
+                                         TargetSelectionUserWarning,
+                                         XMatchError)
+from target_selection.utils import (Timer, get_configuration_values,
+                                    get_epoch, is_view, sql_apply_pm,
+                                    vacuum_outputs, vacuum_table)
+
 
 EPOCH = 2016.0
 QUERY_RADIUS = 1.
 
 #: Reserve last 11 bits for the run id.
 RUN_ID_BIT_SHIFT = 64 - 11
 
@@ -362,18 +358,23 @@
         If specified, the name of the table that will be inserted first
         regarding of the above sorting process.
     query_radius : float
         The radius, in arcsec, for cross-matching between existing targets.
         Used in phase 2. Defaults to 1 arcsec.
     schema : str
         The schema in which all the tables to cross-match live (multiple
-        schemas are not supported), and the schema in which the output table
+        schemas are not supported), and the schema in which the output tables
         will be created.
     output_table : str
         The name of the output table. Defaults to ``catalog``.
+    temp_schema
+        The schema where the temporary ``catalog`` table will be initially created.
+    log
+        A logger to which to log messages. If not provided the ``target_selection``
+        logger is used.
     log_path : str
         The path to which to log or `False` to disable file logging.
     debug : bool or int
         Controls the level to which to log to the screen. If `False` no logging
         is done to ``stdout``. If `True` the logging level is set to ``debug``
         (all messages). It's also possible specify a numerical value for the
         `logging level <logging>`.
@@ -391,19 +392,14 @@
         starts again until no shortest paths are available. ``full`` mode
         retrieves all the paths that are not a subsample of another path.
         ``config_list`` mode takes the list of paths from ``join_paths``
         parameter in the .yml configuration file.
     join_paths : list
         When using path_mode=``config_list`` is the list of paths to link
         tables to output catalog table in phase_1.
-    phase1_range : list
-        List to indicate which tables will be ingested in phase_1 with multiple
-        queries split by pk range instead of using a single query.
-        Each element of this list is a list with the name of the table the
-        minimum pk value, the maximum pk value and the bin width.
     database_options : dict
         A dictionary of database configuration parameters to be set locally
         during each phase transaction, temporarily overriding the default
         database configuration. Keys must be the database parameter to modify.
         The value can be a simple string with the value to set, or a dictionary
         that more accurately defines when the parameter will be applied. For
         example ::
@@ -417,20 +413,20 @@
         be set up when defining the `.XMatchModel`.
 
     """
 
     def __init__(self, database, models, plan, run_id, version_id=None,
                  extra_nodes=[], order='hierarchical', key='row_count',
                  epoch=EPOCH, start_node=None, query_radius=None,
-                 schema='catalogdb', output_table='catalog',
-                 log_path='./xmatch_{plan}.log', debug=False, show_sql=False,
+                 schema='catalogdb', temp_schema=TEMP_SCHEMA, output_table='catalog',
+                 log=None, log_path='./xmatch_{plan}.log', debug=False, show_sql=False,
                  sample_region=None, database_options=None, path_mode='full',
-                 join_paths=None, phase1_range=[]):
+                 join_paths=None):
 
-        self.log = target_selection.log
+        self.log = log or target_selection.log
         self.log.header = ''
 
         if log_path:
             log_path = os.path.realpath(log_path)
             if self.log.fh:
                 self.log.removeHandler(self.log.fh)
                 self.log.fh = None
@@ -441,14 +437,15 @@
             self.log.sh.setLevel(0)
         elif debug is False:
             self.log.sh.setLevel(100)
         else:
             self.log.sh.setLevel(debug)
 
         self.schema = schema
+        self.temp_schema = temp_schema
 
         self.output_table = output_table
         self.md5 = hashlib.md5(plan.encode()).hexdigest()[0:16]
         self._temp_table = self.output_table + '_' + self.md5
 
         self.database = database
         assert self.database.connected, 'database is not connected.'
@@ -488,15 +485,14 @@
         self.update_model_graph()
 
         self.process_order = []
         self.set_process_order(order=order, key=key, start_node=start_node)
 
         self._max_cid = self.run_id << RUN_ID_BIT_SHIFT
         self.path_mode = path_mode
-        self.phase1_range = phase1_range
 
         if path_mode == 'config_list':
             join_paths_warning = 'join_paths needed for path_mode=config_list'
             assert join_paths is not None, join_paths_warning
             self.join_paths = join_paths
 
     @classmethod
@@ -564,15 +560,15 @@
             models to use subclass, or a
             `~sdssdb.connection.PeeweeDatabaseConnection` to the database
             containing the models. In the latter case, the models must have
             been imported so that they are available via the ``models``
             attribute.
         plan : str
             The cross-matching plan.
-        config_file : str
+        config_file : str or dict
             The path to the configuration file to use. Defaults to
             ``config/xmatch.yml``. The file must contain a hash with the
             cross-match plan.
         kwargs : dict
             User arguments that will override the configuration file values.
 
         """
@@ -643,15 +639,18 @@
         return cls(database, xmatch_models.values(), plan,
                    extra_nodes=extra_nodes, **valid_kw)
 
     @staticmethod
     def _read_config(file_, plan):
         """Reads the configuration file, recursively."""
 
-        config = yaml.load(open(file_, 'r'), Loader=yaml.SafeLoader)
+        if isinstance(file_, dict):
+            config = copy.deepcopy(file_)
+        else:
+            config = yaml.load(open(file_, 'r'), Loader=yaml.SafeLoader)
 
         assert plan in config, f'plan {plan!r} not found in configuration.'
 
         base_plan = config[plan].pop('base_plan', None)
         if base_plan:
             config = merge_config(config[plan],
                                   XMatchPlanner._read_config(file_, base_plan))
@@ -723,15 +722,15 @@
         values = get_configuration_values(self.database, parameters)
 
         self.log.debug('Current database configuration parameters.')
         for parameter in values:
             log_str = f'{parameter} = {values[parameter]}'
             self.log.debug(log_str)
 
-    def update_model_graph(self, silent=False):
+    def update_model_graph(self):
         """Updates the model graph using models as nodes and fks as edges."""
 
         self.model_graph = networkx.Graph()
         self.model_graph.add_node(self._temp_table, model=TempCatalog)
 
         all_models = (list(self.models.values()) +
                       list(self.extra_nodes.values()))
@@ -761,15 +760,15 @@
 
                 join_weight = 0.5 * (model_weight + fk_model_weight)
 
                 self.model_graph.add_edge(table_name, ref_table_name,
                                           join_weight=join_weight)
 
             if model in self.models.values():
-                rel_model = self._get_relational_model(model)
+                rel_model = self.get_relational_model(model, sandboxed=False)
                 rel_model._meta.schema = self.schema
                 rel_model_tname = rel_model._meta.table_name
                 self.model_graph.add_node(rel_model_tname, model=rel_model)
                 self.model_graph.add_edge(self._temp_table, rel_model_tname)
                 self.model_graph.add_edge(table_name, rel_model_tname)
 
         return self.model_graph
@@ -970,15 +969,15 @@
 
         # Sets the metadata of the Catalog, TempCatalog, and Version tables.
 
         Catalog._meta.schema = self.schema
         Catalog._meta.table_name = self.output_table
         Catalog._meta.set_database(self.database)
 
-        TempCatalog._meta.schema = TEMP_SCHEMA
+        TempCatalog._meta.schema = self.temp_schema
         TempCatalog._meta.table_name = self._temp_table
         TempCatalog._meta.set_database(self.database)
 
         Version._meta.schema = self.schema
         Version._meta.set_database(self.database)
 
     def _check_version(self, model, force=False):
@@ -1049,34 +1048,38 @@
             if force:
                 self.log.warning(msg)
             else:
                 raise XMatchError(msg)
 
             self._check_version(TempCatalog, force)
 
-            self._temp_count = int(get_row_count(self.database,
-                                                 self._temp_table,
-                                                 schema=self.schema,
-                                                 approximate=True))
+            try:
+                self._temp_count = int(get_row_count(self.database,
+                                                     self._temp_table,
+                                                     schema=self.schema,
+                                                     approximate=True))
+            except ValueError:
+                self._temp_count = 0
+
         else:
 
             # Add Q3C index for TempCatalog
-            TempCatalog.add_index(SQL(f'CREATE INDEX '
+            TempCatalog.add_index(SQL(f'CREATE INDEX IF NOT EXISTS '
                                       f'{self._temp_table}_q3c_idx ON '
-                                      f'{TEMP_SCHEMA}.{self._temp_table} '
+                                      f'{self.temp_schema}.{self._temp_table} '
                                       f'(q3c_ang2ipix(ra, dec))'))
 
             self.database.create_tables([TempCatalog])
 
             self.log.info(f'Created table {self._temp_table}.')
 
             self._temp_count = 0
 
     def run(self, vacuum=False, analyze=False, from_=None,
-            force=False, load_catalog=True, keep_temp=False):
+            force=False, dry_run=False, keep_temp=False):
         """Runs the cross-matching process.
 
         Parameters
         ----------
         vacuum : bool
             Vacuum all output tables before processing new catalogues.
         analyze : bool
@@ -1084,23 +1087,32 @@
         from_ : str
             Table from which to start running the process. Useful in reruns
             to skip tables already processed.
         force : bool
             Allows to continue even if the temporary table exists or the
             output table contains records for this version. ``force=True`` is
             assumed if ``from_`` is defined.
-        load_catalog : bool
-            If `True`, loads the temporary table into ``Catalog``. `False` implies
-            ``keep_temp=True``.
+        dry_run : bool
+            If `False`, loads the temporary tables into ``Catalog`` and ``CatalogToXXX``.
+            `True` implies ``keep_temp=True``; all the cross-matching steps will be run
+            but the original tables won't be modified. A dry run can only be executed for
+            a plan with a single catalogue since processing multiple catalogue requires the
+            final tables to have been updated for successive catalogues.
         keep_temp : bool
             Whether to keep the temporary table or to drop it after the cross
             matching is done.
 
         """
 
+        if len(self.process_order) > 1 and dry_run is True:
+            raise RuntimeError('Cannot dry run with a plan that includes more than one catalogue.')
+
+        if dry_run:
+            keep_temp = True
+
         if vacuum or analyze:
             cmd = ' '.join(('VACUUM' if vacuum else '',
                             'ANALYZE' if analyze else '')).strip()
             self.log.info(f'Running {cmd} on output tables.')
             vacuum_outputs(self.database, vacuum=vacuum, analyze=analyze,
                            schema=Catalog._meta.schema,
                            table=Catalog._meta.table_name)
@@ -1126,40 +1138,52 @@
             max_cid = (TempCatalog
                        .select(fn.MAX(TempCatalog.catalogid))
                        .scalar())
             self._max_cid = max_cid + 1  # just to be sure numbers dont overlap
 
         with Timer() as timer:
             p_order = self.process_order
-            for table_name in p_order:
-                if (from_ and
-                        p_order.index(table_name) < p_order.index(from_)):
+            for norder, table_name in enumerate(p_order):
+                if dry_run and norder > 0:
+                    raise RuntimeError('Cannot dry run more than one catalogue.')
+
+                if (from_ and p_order.index(table_name) < p_order.index(from_)):
                     self.log.warning(f'Skipping table {table_name}.')
                     continue
                 model = self.models[table_name]
-                self.process_model(model)
+                self.process_model(model, force=force)
 
-            if load_catalog:
-                self._load_output_table(keep_temp=keep_temp)
+                if not dry_run:
+                    self.load_output_tables(model, keep_temp=keep_temp)
 
         self.log.info(f'Cross-matching completed in {timer.interval:.3f} s.')
 
-    def process_model(self, model):
+    def process_model(self, model, force=False):
         """Processes a model, loading it into the output table."""
 
         table_name = model._meta.table_name
         self.log.header = f'[{table_name.upper()}] '
 
         self.log.info(f'Processing table {table_name}.')
         self._log_table_configuration(model)
 
         if model._meta.xmatch.has_duplicates:
             raise TargetSelectionNotImplemented(
                 'handling of tables with duplicates is not implemented.')
 
+        rel_model = self.get_relational_model(model, sandboxed=True, create=False)
+        rel_model_table_name = rel_model._meta.table_name
+        if rel_model.table_exists():
+            if force is False:
+                raise RuntimeError(
+                    f'Sandboxed relational table {rel_model_table_name} exists. '
+                    'Delete it manually before continuing.')
+            else:
+                self.log.warning(f'Sandboxed relational table {rel_model_table_name} exists.')
+
         # Check if there are already records in catalog for this version.
         if self.process_order.index(model._meta.table_name) == 0 and not self.is_addendum:
             is_first_model = True
         else:
             is_first_model = False
 
         self._phases_run = set()
@@ -1168,16 +1192,15 @@
             if is_first_model:
                 self._run_phase_3(model)
             else:
                 self._run_phase_1(model)
                 self._run_phase_2(model)
                 self._run_phase_3(model)
 
-        self.log.info(f'Fully processed {table_name} '
-                      f'in {timer.elapsed:.0f} s.')
+        self.log.info(f'Fully processed {table_name} in {timer.elapsed:.0f} s.')
 
         self.update_model_graph()
 
         self.log.header = ''
 
     def _get_model_fields(self, model):
         """Returns the model fields needed to populate Catalog."""
@@ -1265,19 +1288,27 @@
         # Parallax
         if xmatch.parallax_column:
             model_fields.append(fields[xmatch.parallax_column]
                                 .alias('parallax'))
 
         return model_fields
 
-    def _get_relational_model(self, model, temp=False, create=False):
+    def get_output_model(self, temporary=False):
+        """Returns the temporary or final output model (``catalog``)."""
+
+        if temporary:
+            return TempCatalog
+
+        return Catalog
+
+    def get_relational_model(self, model, sandboxed=False, temp=False, create=False):
         """Gets or creates a relational table for a given model.
 
-        Returns the relational model and `True` if the table was created or
-        `False` if it already existed.
+        When the relational model is ``sandboxed``, the table is created in the
+        temporary schema and suffixed with the same MD5 used for the run.
 
         """
 
         cat_table = Catalog._meta.table_name
         prefix = cat_table + '_to_'
 
         meta = model._meta
@@ -1300,36 +1331,37 @@
 
             catalogid = peewee.BigIntegerField(null=False, index=True)
             target_id = model_pk_class(null=False, index=True)
             version_id = peewee.SmallIntegerField(null=False, index=True)
             distance = peewee.DoubleField(null=True)
             best = peewee.BooleanField(null=False)
             plan_id = peewee.TextField(null=True)
+            added_by_phase = peewee.SmallIntegerField(null=True)
 
             class Meta:
                 database = meta.database
-                schema = meta.schema
+                schema = self.temp_schema if sandboxed else meta.schema
                 primary_key = False
 
         model_prefix = ''.join(x.capitalize() or '_'
                                for x in prefix.rstrip().split('_'))
 
         RelationalModel = type(model_prefix + model.__name__, (BaseModel,), {})
 
         if temp:
             RelationalModel._meta.primary_key = False
             RelationalModel._meta.composite_key = False
             RelationalModel._meta.set_table_name(uuid.uuid4().hex[0:8])
             RelationalModel._meta.schema = None
             return RelationalModel
 
-        if meta.xmatch.relational_table is not None:
-            RelationalModel._meta.table_name = meta.xmatch.relational_table
-        else:
-            RelationalModel._meta.table_name = prefix + meta.table_name
+        table_name = prefix + meta.table_name
+        if sandboxed:
+            table_name += f'_{self.md5}'
+        RelationalModel._meta.table_name = table_name
 
         if create and not RelationalModel.table_exists():
             RelationalModel.create_table()
 
         # Add foreign key field here. We want to avoid Peewee creating it
         # as a constraint and index if the table is created because that would
         # slow down inserts. We'll created them manually with add_fks.
@@ -1364,15 +1396,17 @@
 
         return query
 
     def _run_phase_1(self, model):
         """Runs the linking against matched catalogids stage."""
 
         table_name = model._meta.table_name
-        rel_model = self._get_relational_model(model, create=True)
+        rel_model_sb = self.get_relational_model(model, create=True, sandboxed=True)
+
+        rel_model = self.get_relational_model(model, create=False, sandboxed=False)
 
         model_pk = model._meta.primary_key
 
         self.log.info('Phase 1: linking existing targets.')
 
         if 1 in model._meta.xmatch.skip_phases:
             self.log.warning('Skipping due to configuration.')
@@ -1399,191 +1433,112 @@
                            in path]
 
             # Get the relational model that leads to the temporary catalog
             # table in the join. We'll want to filter on version_id to avoid
             # a sequential scan.
             join_rel_model = join_models[-1]
 
-            # We can have join catalogues that produce more than
-            # one result for each target or different targets that
-            # are joined to the same catalogid. In the future we may
-            # want to order by something that selects the best
-            # candidate.
-
-            partition = (fn.first_value(model_pk)
-                         .over(partition_by=[join_rel_model.catalogid],
-                               order_by=[model_pk.asc()]))
-            best = peewee.Value(partition == model_pk)
-
             query = (self._build_join(join_models)
                      .select(model_pk.alias('target_id'),
                              join_rel_model.catalogid,
-                             best.alias('best'))
+                             peewee.Value(True).alias('best'))
                      .where(join_rel_model.version_id == self.version_id,
                             join_rel_model.best >> True)
                      .where(~fn.EXISTS(
-                         rel_model
+                         rel_model_sb
                          .select(SQL('1'))
-                         .where(rel_model.version_id == self.version_id,
-                                ((rel_model.target_id == model_pk) |
-                                 (rel_model.catalogid ==
-                                  join_rel_model.catalogid)))))
-                     # To avoid breaking the unique constraint in rel tables
-                     .distinct(model_pk, join_rel_model.catalogid))
+                         .where(rel_model_sb.version_id == self.version_id,
+                                ((rel_model_sb.target_id == model_pk) |
+                                 (rel_model_sb.catalogid == join_rel_model.catalogid)))))
+                     # Select only one match per target in the catalogue with are cross-matching.
+                     .distinct(model_pk))
 
             # Deal with duplicates in LS8
             if table_name == 'legacy_survey_dr8':
                 query = query.where(self._get_ls8_where(model))
 
             # Remove Duplicates and non-primary entries from LS10
             if table_name == 'legacy_survey_dr10':
                 query = query.where(model.survey_primary >> True,
                                     fn.coalesce(model.ref_cat, '') != 'T2')
 
+            # If the real relational model exists, exclude any matches that already exist there.
+            if rel_model.table_exists():
+                query = query.where(
+                    ~fn.EXISTS(rel_model
+                               .select(SQL('1'))
+                               .where(rel_model.version_id == self.version_id,
+                                      rel_model.target_id == model_pk)))
+
             # In query we do not include a Q3C where for the sample region because
             # TempCatalog for this plan should already be sample region limited.
 
             with Timer() as timer:
 
                 with self.database.atomic():
 
-                    self._setup_transaction(model, phase=1)
-                    inter_name1 = 'phase1_content'
-                    model_pk_class = model_pk.__class__
+                    temp_model = self.get_relational_model(model, temp=True, sandboxed=True)
+                    temp_table = temp_model._meta.table_name
 
-                    class Intermediate1(peewee.Model):
-                        """Model for the intermediate results of phase_1."""
-                        target_id = model_pk_class(null=False, index=True)
-                        catalogid = peewee.BigIntegerField(index=True, null=False)
-                        best = peewee.BooleanField(null=False)
-                        distance = peewee.DoubleField(null=True)
-                        version_id = peewee.SmallIntegerField(null=False, index=True)
-
-                        class Meta:
-                            database = self.database
-                            schema = TEMP_SCHEMA
-                            table_name = inter_name1
-                            primary_key = False
-
-                    query_str = self._get_sql(query, return_string=True)
-
-                    range_info = self.phase1_range
-                    range_tables = [el[0] for el in range_info]
-
-                    if table_name not in range_tables:
-                        self.log.debug(f'Selecting linked targets into '
-                                       f'table {self.schema}.{inter_name1} IN PSQL '
-                                       f'with join path {path}{self._get_sql(query)}')
-
-                        sql_file = open('phase1_query.sql', 'w')
-
-                        if self._options['database_options']:
-                            options = self._options['database_options'].copy()
-                            for param in options:
-                                if param == 'maintenance_work_mem':
-                                    continue
-                                value = options[param]
-                                sql_file.write(f'SET {param}={value!r};\n')
-
-                        sql_file.write(f'DROP TABLE IF EXISTS {TEMP_SCHEMA}.{inter_name1};')
-                        sql_file.write(f'CREATE TABLE {TEMP_SCHEMA}.{inter_name1} AS (')
-                        sql_file.write(query_str + ');')
-                        sql_file.close()
-
-                        os.system('psql -U sdss -d sdss5db -f '
-                                  'phase1_query.sql -o phase1_output.log')
-
-                    # If the config file indicates that we want to ingest phase_1 by PK range
-                    # Then instead of doing a simple query to create the intermediate result table
-                    # We first create the table and then do multiple queries each with a PK range
-                    # each time inserting the result to the intermediate result table
-
-                    else:
-                        range_info_table = range_info[range_tables.index(table_name)]
-                        low_limit = range_info_table[1]
-                        high_limit = range_info_table[2]
-                        bin_range = range_info_table[3]
-                        first_query = query.where(model_pk < low_limit)
-                        first_query_str = self._get_sql(first_query, return_string=True)
-                        self.log.debug(f'Selecting linked targets into '
-                                       f'table {TEMP_SCHEMA}.{inter_name1} IN PSQL BY PK RANGE '
-                                       f'with join path {path} and base (before splitting) query'
-                                       f'{self._get_sql(query)}')
-
-                        sql_file = open('phase1_query.sql', 'w')
-                        sql_file.write(f'DROP TABLE IF EXISTS {TEMP_SCHEMA}.{inter_name1};')
-                        sql_file.write(f'CREATE TABLE {TEMP_SCHEMA}.{inter_name1} AS (')
-                        sql_file.write(first_query_str + ');')
-                        sql_file.close()
-
-                        os.system('psql -U sdss -d sdss5db -f phase1_query.sql '
-                                  '-o phase1_output.log')
-
-                        min_id, max_id = low_limit, low_limit + bin_range
-
-                        while max_id <= high_limit:
-                            range_query = query.where(model_pk >= min_id, model_pk < max_id)
-                            range_query_str = self._get_sql(range_query)
-                            sql_file = open('phase1_query.sql', 'w')
-
-                            if self._options['database_options']:
-                                options = self._options['database_options'].copy()
-                                for param in options:
-                                    if param == 'maintenance_work_mem':
-                                        continue
-                                    value = options[param]
-                                    sql_file.write(f'SET {param}={value!r};\n')
-
-                            sql_file.write(f'INSERT INTO {TEMP_SCHEMA}.{inter_name1} ')
-                            sql_file.write(range_query_str + ';')
-                            sql_file.close()
-                            os.system('psql -U sdss -d sdss5db -f phase1_query.sql '
-                                      '-o phase1_output.log')
-                            min_id += bin_range
-                            max_id += bin_range
+                    self._setup_transaction(model, phase=1)
+                    self.log.debug(f'Selecting linked targets into temporary '
+                                   f'table {temp_table!r} with join path '
+                                   f'{path}{self._get_sql(query)}')
+                    query.create_table(temp_table, temporary=True)
 
                     self.log.debug(f'Copying data into relational model '
-                                   f'{rel_model._meta.table_name!r}.')
+                                   f'{rel_model_sb._meta.table_name!r}.')
 
-                    fields = [Intermediate1.target_id, Intermediate1.catalogid,
-                              Intermediate1.version_id, Intermediate1.best,
-                              rel_model.plan_id]
-
-                    cursor = rel_model.insert_from(
-                        Intermediate1.select(Intermediate1.target_id,
-                                             Intermediate1.catalogid,
-                                             peewee.Value(self.version_id),
-                                             Intermediate1.best,
-                                             self.plan if self.is_addendum else None),
+                    fields = [temp_model.target_id, temp_model.catalogid,
+                              temp_model.version_id, temp_model.best,
+                              temp_model.plan_id, temp_model.added_by_phase]
+
+                    nids = rel_model_sb.insert_from(
+                        temp_model.select(temp_model.target_id,
+                                          temp_model.catalogid,
+                                          peewee.Value(self.version_id),
+                                          temp_model.best,
+                                          peewee.Value(self.plan) if self.is_addendum else None,
+                                          peewee.Value(1)),
                         fields).returning().execute()
-                    nids = cursor.rowcount
 
-            self.log.debug(f'Linked {nids:,} records in'
-                           f' {timer.interval:.3f} s.')
+            self.log.debug(f'Linked {nids.rowcount:,} records in {timer.interval:.3f} s.')
             self._phases_run.add(1)
 
-            if nids > 0:
-                self._analyze(rel_model)
+            if nids.rowcount > 0:
+                self._analyze(rel_model_sb)
+
+    def _run_phase_2(self, model, source=TempCatalog):
+        """Associates existing targets in Catalog with entries in the model.
 
-    def _run_phase_2(self, model):
-        """Associates existing targets in Catalog with entries in the model."""
+        Here ``source`` is the catalogue with which we are spatially cross-matching.
+        Normally this is the temporary catalog table which we are building for this
+        cross-match run. But when we are doing an addendum, that table is going to be
+        empty (at least of the first table in the addeundum), so we need to also have
+        the option of using the real ``catalog`` table as the source. This method will
+        call itself recursively with ``source=Catalog`` if this is an addendum run.
+
+        """
 
         meta = model._meta
         xmatch = meta.xmatch
 
         table_name = meta.table_name
 
-        self.log.info('Phase 2: cross-matching against existing targets.')
+        self.log.info('Phase 2: cross-matching against existing targets '
+                      f'({source._meta.table_name}).')
 
         if 2 in xmatch.skip_phases:
             self.log.warning('Skipping due to configuration.')
             return
 
-        rel_model = self._get_relational_model(model, create=True)
-        rel_table_name = rel_model._meta.table_name
+        rel_model_sb = self.get_relational_model(model, create=True, sandboxed=True)
+        rel_sb_table_name = rel_model_sb._meta.table_name
+
+        rel_model = self.get_relational_model(model, create=False, sandboxed=False)
 
         model_pk = meta.primary_key
         model_ra = meta.fields[xmatch.ra_column]
         model_dec = meta.fields[xmatch.dec_column]
 
         catalog_epoch = self._options['epoch']
 
@@ -1610,50 +1565,48 @@
                     .select(fn.MAX(fn.ABS(model_epoch - catalog_epoch)))
                     .where(self._get_sample_where(model_ra, model_dec))
                     .scalar()
                 )
 
             max_delta_epoch += .1  # Add .1 yr to be sure it's an upper bound
 
-            self.log.debug(f'Maximum epoch delta: '
-                           f'{max_delta_epoch:.3f} (+ 0.1 year).')
-
-        self.log.debug('Cross-matching model against temporary table.')
+            self.log.debug(f'Maximum epoch delta: {max_delta_epoch:.3f} (+ 0.1 year).')
 
         if use_pm:
 
             model_pmra = meta.fields[xmatch.pmra_column]
             model_pmdec = meta.fields[xmatch.pmdec_column]
             model_is_pmra_cos = int(xmatch.is_pmra_cos)
 
             q3c_dist = fn.q3c_dist_pm(model_ra, model_dec,
                                       model_pmra, model_pmdec,
                                       model_is_pmra_cos, model_epoch,
-                                      TempCatalog.ra, TempCatalog.dec,
+                                      source.ra, source.dec,
                                       catalog_epoch)
             q3c_join = fn.q3c_join_pm(model_ra, model_dec,
                                       model_pmra, model_pmdec,
                                       model_is_pmra_cos, model_epoch,
-                                      TempCatalog.ra, TempCatalog.dec,
+                                      source.ra, source.dec,
                                       catalog_epoch, max_delta_epoch,
                                       query_radius / 3600.)
         else:
 
             q3c_dist = fn.q3c_dist(model_ra, model_dec,
-                                   TempCatalog.ra, TempCatalog.dec)
+                                   source.ra, source.dec)
             q3c_join = fn.q3c_join(model_ra, model_dec,
-                                   TempCatalog.ra, TempCatalog.dec,
+                                   source.ra, source.dec,
                                    query_radius / 3600.)
 
         # Get the cross-matched catalogid and model target pk (target_id),
         # and their distance.
-        xmatched = (TempCatalog
-                    .select(TempCatalog.catalogid,
+        xmatched = (source
+                    .select(source.catalogid,
                             model_pk.alias('target_id'),
-                            q3c_dist.alias('distance'))
+                            q3c_dist.alias('distance'),
+                            source.version_id)
                     .join(model, peewee.JOIN.CROSS)
                     .where(q3c_join)
                     .where(self._get_sample_where(model_ra, model_dec)))
 
         if table_name == 'legacy_survey_dr8':
             xmatched = xmatched.where(self._get_ls8_where(model))
         if table_name == 'legacy_survey_dr10':
@@ -1684,93 +1637,90 @@
         # because that's the order in which we defined the index.
         in_query = (xmatched
                     .select(xmatched.c.target_id,
                             xmatched.c.catalogid,
                             peewee.Value(self.version_id).alias('version_id'),
                             xmatched.c.distance.alias('distance'),
                             best.alias('best'),
-                            self.plan if self.is_addendum else None))
+                            self.plan if self.is_addendum else None,
+                            peewee.Value(2).alias('added_by_phase')))
 
         # We only need to care about already linked targets if phase 1 run.
         if 1 in self._phases_run:
             in_query = (
-                in_query .where(
-                    ~fn.EXISTS(
-                        rel_model .select(
-                            SQL('1')) .where(
-                            (rel_model.version_id == self.version_id) & (
-                                (rel_model.catalogid ==
-                                 xmatched.c.catalogid) | (
-                                    (rel_model.target_id ==
-                                     xmatched.c.target_id)))))))
+                in_query.where(
+                    xmatched.c.version_id == self.version_id,
+                    ~fn.EXISTS(rel_model_sb.select(SQL('1'))
+                               .where((rel_model_sb.version_id == self.version_id) &
+                                      ((rel_model_sb.catalogid == xmatched.c.catalogid) |
+                                       ((rel_model_sb.target_id == xmatched.c.target_id))))
+                               )))
+
+        if rel_model.table_exists():
+            in_query = (
+                in_query.where(
+                    ~fn.EXISTS(rel_model.select(SQL('1'))
+                               .where((rel_model.version_id == self.version_id) &
+                                      ((rel_model.catalogid == xmatched.c.catalogid) |
+                                       ((rel_model.target_id == xmatched.c.target_id))))
+                               )))
 
         with Timer() as timer:
 
             with self.database.atomic():
 
                 # 1. Tweak database configuration for this transaction to
                 #    ensure Q3C index is used.
 
                 # May need to increase work_mem during this transaction to
                 # make sure the Q3C index is used.
                 self._setup_transaction(model, phase=2)
 
                 # 2. Run cross-match and insert data into relational model.
 
-                fields = [rel_model.target_id, rel_model.catalogid,
-                          rel_model.version_id, rel_model.distance,
-                          rel_model.best, rel_model.plan_id]
-
-                in_query = (rel_model
-                            .insert_from(in_query.with_cte(xmatched),
-                                         fields).returning())
-
-                self.log.debug(f'Inserting cross-matched data into '
-                               f'relational model {rel_table_name!r} in PSQL: '
-                               f'{self._get_sql(in_query)}')
+                fields = [rel_model_sb.target_id, rel_model_sb.catalogid,
+                          rel_model_sb.version_id, rel_model_sb.distance,
+                          rel_model_sb.best, rel_model_sb.plan_id, rel_model_sb.added_by_phase]
 
-                in_query_str = self._get_sql(in_query, return_string=True)
+                in_query = rel_model_sb.insert_from(in_query.with_cte(xmatched),
+                                                    fields).returning()
 
-                sql_file = open('phase2_query.sql', 'w')
+                self.log.debug(f'Running Q3C query and inserting cross-matched data into '
+                               f'relational table {rel_sb_table_name!r}: '
+                               f'{self._get_sql(in_query)}')
 
-                if self._options['database_options']:
-                    options = self._options['database_options'].copy()
-                    for param in options:
-                        if param == 'maintenance_work_mem':
-                            continue
-                        value = options[param]
-                        sql_file.write(f'SET {param}={value!r};\n')
-
-                sql_file.write(in_query_str + ';')
-                sql_file.close()
-
-                os.system('psql -U sdss -d sdss5db -f phase2_query.sql -o phase2_output.log')
-                out_file = open('phase2_output.log', 'r')
-                lines = out_file.readlines()
-                out_file.close()
-                n_catalogid = int(lines[-1].split()[-1])
+                n_catalogid = in_query.execute().rowcount
 
-        self.log.debug(f'Cross-matched {TempCatalog._meta.table_name} with '
+        self.log.debug(f'Cross-matched {source._meta.table_name} with '
                        f'{n_catalogid:,} targets in {table_name}. '
                        f'Run in {timer.interval:.3f} s.')
 
         if n_catalogid > 0:
             self._phases_run.add(2)
-            self._analyze(rel_model)
+            self._analyze(rel_model_sb)
+
+        # For addenda it's not sufficient to cross-match with the temporary table, because that
+        # does not contain all the cumulated targets from this cross-match version. We need to
+        # also spatially cross-match with the real catalog table (but only for the targets with
+        # version_id=<this-version-id>).
+        if self.is_addendum and source != Catalog:
+            self._run_phase_2(model, source=Catalog)
 
     def _run_phase_3(self, model):
         """Add non-matched targets to Catalog and the relational table."""
 
         meta = model._meta
         xmatch = meta.xmatch
 
         self.log.info('Phase 3: adding non cross-matched targets.')
 
-        rel_model = self._get_relational_model(model, create=True)
-        rel_table_name = rel_model._meta.table_name
+        rel_model_sb = self.get_relational_model(model, create=True, sandboxed=True)
+        rel_sb_table_name = rel_model_sb._meta.table_name
+
+        rel_model = self.get_relational_model(model, create=False, sandboxed=False)
 
         if 3 in xmatch.skip_phases:
             self.log.warning('Skipping due to configuration.')
             return
 
         table_name = meta.table_name
 
@@ -1787,18 +1737,27 @@
                              *model_fields)
                      .where(self._get_sample_where(model_ra, model_dec)))
 
         if 1 in self._phases_run or 2 in self._phases_run:
             unmatched = (
                 unmatched.where(
                     ~fn.EXISTS(
-                        rel_model .select(
-                            SQL('1')) .where(
-                            rel_model.version_id == self.version_id,
-                            rel_model.target_id == model_pk))))
+                        rel_model_sb.select(SQL('1')).where(
+                            rel_model_sb.version_id == self.version_id,
+                            rel_model_sb.target_id == model_pk,
+                            rel_model_sb.best >> True))))
+
+        if rel_model.table_exists():
+            print('Im here', rel_model)
+            unmatched = unmatched.where(
+                ~fn.EXISTS(
+                    rel_model.select(SQL('1')).where(
+                        rel_model.version_id == self.version_id,
+                        rel_model.target_id == model_pk,
+                        rel_model.best >> True)))
 
         if xmatch.has_missing_coordinates:
             unmatched = unmatched.where(model_ra.is_null(False),
                                         model_dec.is_null(False))
 
         # TODO: this is horrible and should be moved to the configuration.
         if model._meta.table_name == 'tic_v8':
@@ -1818,90 +1777,59 @@
             with self.database.atomic():
 
                 # TODO: Not sure it's worth using a temporary table here.
 
                 # 1. Run link query and create temporary table with results.
 
                 self._setup_transaction(model, phase=3)
-                inter_name3 = 'phase3_content'
-                model_pk_class = model_pk.__class__
-
-                class Intermediate3(peewee.Model):
-                    """Model for the intermediate results of phase_3."""
 
-                    catalogid = peewee.BigIntegerField(index=True, null=False)
-                    target_id = model_pk_class(null=False, index=True)
-                    version_id = peewee.SmallIntegerField(null=False, index=True)
-                    best = peewee.BooleanField(null=False)
-                    distance = peewee.DoubleField(null=True)
-
-                    class Meta:
-                        database = self.database
-                        schema = TEMP_SCHEMA
-                        table_name = inter_name3
-                        primary_key = False
-
-                unmatched_query_str = self._get_sql(unmatched, return_string=True)
+                temp_model = self.get_relational_model(model, temp=True, sandboxed=True)
+                temp_model_name = temp_model._meta.table_name
 
                 self.log.debug(f'Selecting unique targets '
-                               f'into table '
-                               f'{self.schema}.{inter_name3!r}'
-                               f' in PSLQ: {self._get_sql(unmatched)}')
-
-                sql_file = open('phase3_query.sql', 'w')
-
-                if self._options['database_options']:
-                    options = self._options['database_options'].copy()
-                    for param in options:
-                        if param == 'maintenance_work_mem':
-                            continue
-                        value = options[param]
-                        sql_file.write(f'SET {param}={value!r};\n')
-
-                sql_file.write(f'DROP TABLE IF EXISTS {TEMP_SCHEMA}.{inter_name3};')
-                sql_file.write(f'CREATE TABLE {TEMP_SCHEMA}.{inter_name3} AS (')
-                sql_file.write(unmatched_query_str + ');')
-                sql_file.close()
+                               f'into temporary table '
+                               f'{temp_model_name!r}{self._get_sql(unmatched)}')
 
-                os.system('psql -U sdss -d sdss5db -f phase3_query.sql -o phase3_output.log')
+                unmatched.create_table(temp_model_name, temporary=True)
 
                 # Analyze the temporary table to gather stats.
                 # self.log.debug('Running ANALYZE on temporary table.')
-                # self.database.execute_sql(f'ANALYZE "{temp_table}";')
+                # self.database.execute_sql(f'ANALYZE "{temp_model_name}";')
 
                 # 2. Copy data from temporary table to relational table. Add
                 #    catalogid at this point.
 
-                fields = [Intermediate3.catalogid, Intermediate3.target_id,
-                          Intermediate3.version_id, Intermediate3.best,
-                          rel_model.plan_id]
-
-                rel_insert_query = rel_model.insert_from(
-                    Intermediate3.select(Intermediate3.catalogid,
-                                         Intermediate3.target_id,
-                                         self.version_id,
-                                         peewee.SQL('true'),
-                                         self.plan if self.is_addendum else None),
+                fields = [temp_model.catalogid, temp_model.target_id,
+                          temp_model.version_id, temp_model.best,
+                          rel_model_sb.plan_id, rel_model_sb.added_by_phase]
+
+                rel_insert_query = rel_model_sb.insert_from(
+                    temp_model.select(temp_model.catalogid,
+                                      temp_model.target_id,
+                                      self.version_id,
+                                      peewee.SQL('true'),
+                                      self.plan if self.is_addendum else None,
+                                      peewee.Value(3).alias('added_by_phase')),
                     fields).returning()
 
                 self.log.debug(f'Copying data into relational model '
-                               f'{rel_table_name!r}'
+                               f'{rel_sb_table_name!r}'
                                f'{self._get_sql(rel_insert_query)}')
 
                 cursor = rel_insert_query.execute()
                 n_rows = cursor.rowcount
 
-                self.log.debug(f'Insertion into {rel_table_name} completed '
+                self.log.debug(f'Insertion into {rel_sb_table_name} completed '
                                f'with {n_rows:,} rows in '
                                f'{timer.elapsed:.3f} s.')
 
                 # 3. Fill out the temporary catalog table with the information
                 #    from the unique targets.
 
-                temp_table = peewee.Table(inter_name3, schema=TEMP_SCHEMA)
+                temp_table = peewee.Table(temp_model_name)
 
                 fields = [TempCatalog.catalogid,
                           TempCatalog.lead,
                           TempCatalog.version_id]
                 select_columns = [temp_table.c.catalogid,
                                   peewee.Value(table_name),
                                   self.version_id]
@@ -1939,66 +1867,79 @@
                        f'Total time: {timer.elapsed:.3f} s.')
 
         self._phases_run.add(3)
 
         if n_rows > 0.5 * self._temp_count:  # Cluster if > 50% of rows are new
             self.log.debug(f'Running CLUSTER on {self._temp_table} '
                            f'with q3c index.')
-            self.database.execute_sql(f'CLUSTER {TEMP_SCHEMA}.{self._temp_table} '
+            self.database.execute_sql(f'CLUSTER {self.temp_schema}.{self._temp_table} '
                                       f'using {self._temp_table}_q3c_idx;')
             self.log.debug(f'Running ANALYZE on {self._temp_table}.')
-            self.database.execute_sql(f'ANALYZE {TEMP_SCHEMA}.{self._temp_table};')
+            self.database.execute_sql(f'ANALYZE {self.temp_schema}.{self._temp_table};')
+
+        self._analyze(rel_model_sb, catalog=False)
+
+    def load_output_tables(self, model, keep_temp=False):
+        """Loads the temporary tables into the output tables."""
 
-        self._analyze(rel_model, catalog=False)
+        self._load_output_table(TempCatalog, Catalog, keep_temp=keep_temp)
 
-    def _load_output_table(self, keep_temp=False):
+        rel_model_sb = self.get_relational_model(model, sandboxed=True, create=False)
+        rel_model = self.get_relational_model(model, sandboxed=False, create=True)
+        self._load_output_table(rel_model_sb, rel_model, keep_temp=keep_temp)
+
+    def _load_output_table(self, from_model, to_model, keep_temp=False):
         """Copies the temporary table to the real output table."""
 
-        self.log.info('Copying temporary table to output table.')
+        to_table = f'{to_model._meta.schema}.{to_model._meta.table_name}'
+        from_table = f'{from_model._meta.schema}.{from_model._meta.table_name}'
+
+        self.log.info(f'Copying {from_table} to {to_table}.')
 
         with Timer() as timer:
             with self.database.atomic():
 
                 self._setup_transaction()
 
-                insert_query = Catalog.insert_from(
-                    TempCatalog.select(),
-                    TempCatalog.select()._returning).returning()
+                insert_query = to_model.insert_from(
+                    from_model.select(),
+                    from_model.select()._returning).returning()
 
-                self.log.debug(f'Running INSERT query into {self.output_table}'
+                self.log.debug(f'Running INSERT query into {to_table}'
                                f'{self._get_sql(insert_query)}')
 
                 cursor = insert_query.execute()
                 n_rows = cursor.rowcount
 
         self.log.debug(f'Inserted {n_rows:,} rows in {timer.elapsed:.3f} s.')
 
         if not keep_temp:
-            self.database.drop_tables([TempCatalog])
-            self.log.info(f'Dropped temporary table {self._temp_table}')
+            self.database.drop_tables([from_model])
+            self.log.info(f'Dropped temporary table {from_table}.')
 
-        self.log.debug(f'Running VACUUM ANALYZE on {self.output_table}.')
-        vacuum_table(self.database, f'{self.schema}.{self.output_table}',
-                     vacuum=True, analyze=True)
+        self.log.debug(f'Running VACUUM ANALYZE on {to_table}.')
+        vacuum_table(self.database, to_table, vacuum=True, analyze=True)
 
     def _get_sql(self, query, return_string=False):
-        """Returns coulourised SQL text for logging."""
+        """Returns colourised SQL text for logging."""
 
         query_str, query_params = query.sql()
 
         if query_params:
             for ind in range(len(query_params)):
                 if isinstance(query_params[ind], str):
                     query_params[ind] = '\'' + query_params[ind] + '\''
 
             query_str = query_str % tuple(query_params)
 
         query_str = query_str.replace('None', 'Null')
         if return_string:
             return query_str
+        elif self.log.rich_console:
+            return f': {rich.markup.escape(query_str)}'
         elif self._options['show_sql']:
             return f': {color_text(query_str, "blue")}'
         else:
             return '.'
 
     def _setup_transaction(self, model=None, phase=None):
         """Sets database parameters for the transaction."""
@@ -2080,16 +2021,15 @@
         schema = rel_model._meta.schema
         table_name = rel_model._meta.table_name
 
         db_opts = self._options['database_options']
         if db_opts:
             work_mem = db_opts.get('maintenance_work_mem', None)
             if work_mem:
-                self.database.execute_sql(f'SET maintenance_work_mem'
-                                          f' = {work_mem!r}')
+                self.database.execute_sql(f'SET maintenance_work_mem = {work_mem!r}')
 
         self.log.debug(f'Running ANALYZE on {table_name}.')
         vacuum_table(self.database, f'{schema}.{table_name}',
                      vacuum=vacuum, analyze=True)
 
         if catalog:
             self.log.debug(f'Running ANALYZE on {self._temp_table}.')
```

### Comparing `sdss-target-selection-1.1.0/setup.cfg` & `sdss_target_selection-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-target-selection
-version = 1.1.0
+version = 1.2.0
 author = José Sánchez-Gallego
 author_email = gallegoj@uw.edu
 description = Code to perform target selection for BHM/MWM using catalogdb
 url = https://github.com/sdss/target_selection
 project_urls = 
 	Repository = https://github.com/sdss/target_selection
 	Documentation = https://sdss-target-selection.readthedocs.org
@@ -31,23 +31,23 @@
 package_dir = 
 	= python
 setup_requires = 
 	numpy>=1.20.0
 install_requires = 
 	numpy>=1.18.1
 	pydl>=1.0.0rc1
-	sdssdb>=0.6.2
+	sdssdb>=0.10.0
 	click>=7.0
 	astropy>=5.0.0
 	networkx>=2.4
 	pandas>=1.0.0
 	healpy>=1.13.0
-	pymangle>=0.9.1
+	sdss-pymangle>=0.9.3
 	tables>=3.6.1
-	sdsstools>=1.0.0
+	sdsstools>=1.6.0
 	enlighten>=1.4.0
 	mocpy>=0.8.5
 	pymoc>=0.5.0
 	gala>=1.6.1
 	matplotlib>=3.1.1
 	dustmaps==1.0.10
 scripts =
```

