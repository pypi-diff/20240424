# Comparing `tmp/xsar-2024.2.1.tar.gz` & `tmp/xsar-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsar-2024.2.1.tar", last modified: Wed Feb  7 08:49:17 2024, max compression
+gzip compressed data, was "xsar-2024.4.24.tar", last modified: Wed Apr 24 18:35:35 2024, max compression
```

## Comparing `xsar-2024.2.1.tar` & `xsar-2024.4.24.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.505353 xsar-2024.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-07 08:48:59.000000 xsar-2024.2.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-07 08:48:59.000000 xsar-2024.2.1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-07 08:48:59.000000 xsar-2024.2.1/.gitconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.493353 xsar-2024.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.493353 xsar-2024.2.1/.github/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-07 08:48:59.000000 xsar-2024.2.1/.github/actions/dynamic_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-07 08:48:59.000000 xsar-2024.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.493353 xsar-2024.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-07 08:48:59.000000 xsar-2024.2.1/.github/workflows/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-07 08:48:59.000000 xsar-2024.2.1/.github/workflows/conda-feedstock-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-02-07 08:48:59.000000 xsar-2024.2.1/.github/workflows/install-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-07 08:48:59.000000 xsar-2024.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-07 08:48:59.000000 xsar-2024.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-07 08:48:59.000000 xsar-2024.2.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-07 08:48:59.000000 xsar-2024.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-02-07 08:48:59.000000 xsar-2024.2.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-07 08:48:59.000000 xsar-2024.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-07 08:48:59.000000 xsar-2024.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-07 08:49:17.505353 xsar-2024.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-02-07 08:48:59.000000 xsar-2024.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-07 08:48:59.000000 xsar-2024.2.1/README_dev.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-07 08:48:59.000000 xsar-2024.2.1/condarc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.497353 xsar-2024.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.489353 xsar-2024.2.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.497353 xsar-2024.2.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/_static/css/xsar.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.497353 xsar-2024.2.1/docs/_static/uml/
--rw-r--r--   0 runner    (1001) docker     (127)   856119 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/_static/uml/classes_all_attributes.png
--rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/_static/uml/packages_all_attributes.png
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.501353 xsar-2024.2.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/mask.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/projections.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/radarsat2.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/rcm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/xsar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/xsar_advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   664426 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/xsar_batch_datarmor.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/xsar_multiple.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/examples/xsar_tops_slc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-07 08:48:59.000000 xsar-2024.2.1/docs/uml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-07 08:48:59.000000 xsar-2024.2.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.501353 xsar-2024.2.1/highlevel-checks/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-02-07 08:48:59.000000 xsar-2024.2.1/highlevel-checks/check_s1_xsar_opendataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-07 08:48:59.000000 xsar-2024.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-07 08:48:59.000000 xsar-2024.2.1/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 08:49:17.505353 xsar-2024.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-02-07 08:48:59.000000 xsar-2024.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.489353 xsar-2024.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.501353 xsar-2024.2.1/src/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4082 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/scripts/compress_safe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.501353 xsar-2024.2.1/src/xsar/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37154 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/base_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/ipython_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)    32278 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/radarsat2_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/radarsat2_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/raster_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    34783 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/rcm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/rcm_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    68497 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/sentinel1_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15634 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/sentinel1_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/xarray_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-02-07 08:48:59.000000 xsar-2024.2.1/src/xsar/xsar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.505353 xsar-2024.2.1/src/xsar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-07 08:49:17.000000 xsar-2024.2.1/src/xsar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-07 08:49:17.000000 xsar-2024.2.1/src/xsar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 08:49:17.000000 xsar-2024.2.1/src/xsar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-07 08:49:17.000000 xsar-2024.2.1/src/xsar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-07 08:49:17.000000 xsar-2024.2.1/src/xsar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-07 08:49:17.000000 xsar-2024.2.1/src/xsar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:17.505353 xsar-2024.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-07 08:48:59.000000 xsar-2024.2.1/test/test_raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.562019 xsar-2024.4.24/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 18:35:25.000000 xsar-2024.4.24/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-24 18:35:25.000000 xsar-2024.4.24/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 18:35:25.000000 xsar-2024.4.24/.gitconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/.github/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/actions/dynamic_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/workflows/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/workflows/conda-feedstock-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/workflows/install-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 18:35:25.000000 xsar-2024.4.24/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-24 18:35:25.000000 xsar-2024.4.24/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-24 18:35:25.000000 xsar-2024.4.24/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 18:35:25.000000 xsar-2024.4.24/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 18:35:25.000000 xsar-2024.4.24/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 18:35:25.000000 xsar-2024.4.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 18:35:25.000000 xsar-2024.4.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 18:35:35.562019 xsar-2024.4.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-24 18:35:25.000000 xsar-2024.4.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-24 18:35:25.000000 xsar-2024.4.24/README_dev.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 18:35:25.000000 xsar-2024.4.24/condarc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.546019 xsar-2024.4.24/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.550019 xsar-2024.4.24/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/_static/css/xsar.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.554019 xsar-2024.4.24/docs/_static/uml/
+-rw-r--r--   0 runner    (1001) docker     (127)   856119 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/_static/uml/classes_all_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (127)   126927 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/_static/uml/packages_all_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.554019 xsar-2024.4.24/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/mask.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/projections.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18449 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/radarsat2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/rcm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar_advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   664426 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar_batch_datarmor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar_multiple.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/examples/xsar_tops_slc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 18:35:25.000000 xsar-2024.4.24/docs/uml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-24 18:35:25.000000 xsar-2024.4.24/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.554019 xsar-2024.4.24/highlevel-checks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-24 18:35:25.000000 xsar-2024.4.24/highlevel-checks/check_s1_xsar_opendataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 18:35:25.000000 xsar-2024.4.24/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 18:35:25.000000 xsar-2024.4.24/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:35:35.562019 xsar-2024.4.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-24 18:35:25.000000 xsar-2024.4.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.546019 xsar-2024.4.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.554019 xsar-2024.4.24/src/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4082 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/scripts/compress_safe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.558019 xsar-2024.4.24/src/xsar/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37154 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/base_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/ipython_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32278 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/radarsat2_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12462 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/radarsat2_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/raster_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34783 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/rcm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15175 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/rcm_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68497 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/sentinel1_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/sentinel1_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/xarray_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-24 18:35:25.000000 xsar-2024.4.24/src/xsar/xsar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.558019 xsar-2024.4.24/src/xsar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 18:35:35.000000 xsar-2024.4.24/src/xsar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:35:35.558019 xsar-2024.4.24/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-24 18:35:25.000000 xsar-2024.4.24/test/test_raster_readers.py
```

### Comparing `xsar-2024.2.1/.github/actions/dynamic_matrix.py` & `xsar-2024.4.24/.github/actions/dynamic_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # minimal python script that returns a strategy matrix, for given github.event_name
 
 
 with urllib.request.urlopen('https://endoflife.date/api/python.json') as f:
     python_versions = json.loads(f.read().decode('utf-8'))
 
 now = datetime.datetime.now().strftime('%Y-%m-%d')
-python_supported_versions = [ v['cycle'] for v in python_versions if v['eol'] > now and v['cycle'] not in ['3.7','3.8'] ]
+python_supported_versions = [ v['cycle'] for v in python_versions if v['eol'] > now and v['cycle'] not in ['3.7','3.8','3.12'] ]
 
 python_default_version = python_supported_versions[1]
 
 matrix = {
     'default': {
         'os': ['ubuntu-latest'],
         'python_version': [python_default_version],
```

### Comparing `xsar-2024.2.1/.github/workflows/README.md` & `xsar-2024.4.24/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/.github/workflows/conda-feedstock-check.yml` & `xsar-2024.4.24/.github/workflows/conda-feedstock-check.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/.github/workflows/install-test.yml` & `xsar-2024.4.24/.github/workflows/install-test.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/.github/workflows/publish.yml` & `xsar-2024.4.24/.github/workflows/publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -47,8 +47,8 @@
       - name: Download build artifacts
         uses: actions/download-artifact@v4
         with:
           name: packages
           path: dist/
 
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@2f6f737ca5f74c637829c0f5c3acd0e29ea5e8bf
+        uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
```

### Comparing `xsar-2024.2.1/.gitignore` & `xsar-2024.4.24/.gitignore`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/.gitlab-ci.yml` & `xsar-2024.4.24/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/Dockerfile` & `xsar-2024.4.24/Dockerfile`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/LICENSE` & `xsar-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/PKG-INFO` & `xsar-2024.4.24/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsar
-Version: 2024.2.1
+Version: 2024.4.24
 Summary: xarray L1 SAR mapper
 Home-page: https://github.com/umr-lops/xsar
 Author: Olivier Archer, Alexandre Levieux, Antoine Grouazel
 Author-email: Olivier.Archer@ifremer.fr, Alexandre.Levieux@gmail.com, Antoine.Grouazel@ifremer.fr
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `xsar-2024.2.1/README.md` & `xsar-2024.4.24/README.md`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/README_dev.md` & `xsar-2024.4.24/README_dev.md`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/Makefile` & `xsar-2024.4.24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/_static/uml/classes_all_attributes.png` & `xsar-2024.4.24/docs/_static/uml/classes_all_attributes.png`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/_static/uml/packages_all_attributes.png` & `xsar-2024.4.24/docs/_static/uml/packages_all_attributes.png`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/basic_api.rst` & `xsar-2024.4.24/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/conf.py` & `xsar-2024.4.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/mask.ipynb` & `xsar-2024.4.24/docs/examples/mask.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/projections.ipynb` & `xsar-2024.4.24/docs/examples/projections.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/radarsat2.ipynb` & `xsar-2024.4.24/docs/examples/radarsat2.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/rcm.ipynb` & `xsar-2024.4.24/docs/examples/rcm.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/xsar.ipynb` & `xsar-2024.4.24/docs/examples/xsar.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/xsar_advanced.ipynb` & `xsar-2024.4.24/docs/examples/xsar_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/xsar_batch_datarmor.ipynb` & `xsar-2024.4.24/docs/examples/xsar_batch_datarmor.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/xsar_multiple.ipynb` & `xsar-2024.4.24/docs/examples/xsar_multiple.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/examples/xsar_tops_slc.ipynb` & `xsar-2024.4.24/docs/examples/xsar_tops_slc.ipynb`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/index.rst` & `xsar-2024.4.24/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/docs/installing.rst` & `xsar-2024.4.24/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/highlevel-checks/check_s1_xsar_opendataset.py` & `xsar-2024.4.24/highlevel-checks/check_s1_xsar_opendataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/setup.py` & `xsar-2024.4.24/setup.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/scripts/compress_safe.py` & `xsar-2024.4.24/src/scripts/compress_safe.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/base_dataset.py` & `xsar-2024.4.24/src/xsar/base_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/base_meta.py` & `xsar-2024.4.24/src/xsar/base_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/config.yml` & `xsar-2024.4.24/src/xsar/config.yml`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/ipython_backends.py` & `xsar-2024.4.24/src/xsar/ipython_backends.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/radarsat2_dataset.py` & `xsar-2024.4.24/src/xsar/radarsat2_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/radarsat2_meta.py` & `xsar-2024.4.24/src/xsar/radarsat2_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/raster_readers.py` & `xsar-2024.4.24/src/xsar/raster_readers.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/rcm_dataset.py` & `xsar-2024.4.24/src/xsar/rcm_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/rcm_meta.py` & `xsar-2024.4.24/src/xsar/rcm_meta.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/sentinel1_dataset.py` & `xsar-2024.4.24/src/xsar/sentinel1_dataset.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/sentinel1_meta.py` & `xsar-2024.4.24/src/xsar/sentinel1_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,18 @@
     # class attributes are needed to fetch instance attribute (ie self.name) with dask actors
     # ref http://distributed.dask.org/en/stable/actors.html#access-attributes
     # FIXME: not needed if @property, so it might be a good thing to have getter for those attributes
     xsd_definitions = None
 
     @timing
     def __init__(self, name):
-        from safe_s1.metadata import Sentinel1Reader
+        try:
+            from safe_s1.metadata import Sentinel1Reader
+        except:
+            from safe_s1.reader import Sentinel1Reader
         self.reader = Sentinel1Reader(name)
 
         if not name.startswith('SENTINEL1_DS:'):
             name = name.rstrip('/') # remove trailing space
             name = 'SENTINEL1_DS:%s:' % name
         else:
             name = name.replace('/:',':')
```

### Comparing `xsar-2024.2.1/src/xsar/utils.py` & `xsar-2024.4.24/src/xsar/utils.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/xarray_backends.py` & `xsar-2024.4.24/src/xsar/xarray_backends.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar/xsar.py` & `xsar-2024.4.24/src/xsar/xsar.py`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/src/xsar.egg-info/PKG-INFO` & `xsar-2024.4.24/src/xsar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsar
-Version: 2024.2.1
+Version: 2024.4.24
 Summary: xarray L1 SAR mapper
 Home-page: https://github.com/umr-lops/xsar
 Author: Olivier Archer, Alexandre Levieux, Antoine Grouazel
 Author-email: Olivier.Archer@ifremer.fr, Alexandre.Levieux@gmail.com, Antoine.Grouazel@ifremer.fr
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `xsar-2024.2.1/src/xsar.egg-info/SOURCES.txt` & `xsar-2024.4.24/src/xsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xsar-2024.2.1/test/test_raster_readers.py` & `xsar-2024.4.24/test/test_raster_readers.py`

 * *Files identical despite different names*

