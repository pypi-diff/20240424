# Comparing `tmp/invenio-campusonline-0.4.3.tar.gz` & `tmp/invenio-campusonline-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-campusonline-0.4.3.tar", last modified: Thu Mar 14 19:36:39 2024, max compression
+gzip compressed data, was "invenio-campusonline-0.4.4.tar", last modified: Wed Apr 24 21:07:56 2024, max compression
```

## Comparing `invenio-campusonline-0.4.3.tar` & `invenio-campusonline-0.4.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.008172 invenio-campusonline-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.000172 invenio-campusonline-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.004172 invenio-campusonline-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.004172 invenio-campusonline-0.4.3/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-14 19:36:39.008172 invenio-campusonline-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.004172 invenio-campusonline-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.008172 invenio-campusonline-0.4.3/invenio_campusonline/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.008172 invenio-campusonline-0.4.3/invenio_campusonline/records/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/records/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.008172 invenio-campusonline-0.4.3/invenio_campusonline/services/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/services/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/services/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/services/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/invenio_campusonline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.008172 invenio-campusonline-0.4.3/invenio_campusonline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-14 19:36:38.000000 invenio-campusonline-0.4.3/invenio_campusonline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-14 19:36:38.000000 invenio-campusonline-0.4.3/invenio_campusonline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:36:38.000000 invenio-campusonline-0.4.3/invenio_campusonline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-14 19:36:38.000000 invenio-campusonline-0.4.3/invenio_campusonline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:36:38.000000 invenio-campusonline-0.4.3/invenio_campusonline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-14 19:36:38.000000 invenio-campusonline-0.4.3/invenio_campusonline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-14 19:36:38.000000 invenio-campusonline-0.4.3/invenio_campusonline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-14 19:36:39.008172 invenio-campusonline-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:36:39.008172 invenio-campusonline-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/tests/minimal_record.xml
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/tests/test_invenio_campusonline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-14 19:36:34.000000 invenio-campusonline-0.4.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.077405 invenio-campusonline-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.069405 invenio-campusonline-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.073405 invenio-campusonline-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.073405 invenio-campusonline-0.4.4/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 21:07:56.077405 invenio-campusonline-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.073405 invenio-campusonline-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.077405 invenio-campusonline-0.4.4/invenio_campusonline/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.077405 invenio-campusonline-0.4.4/invenio_campusonline/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.077405 invenio-campusonline-0.4.4/invenio_campusonline/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/services/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/invenio_campusonline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.077405 invenio-campusonline-0.4.4/invenio_campusonline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 21:07:56.000000 invenio-campusonline-0.4.4/invenio_campusonline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-24 21:07:56.000000 invenio-campusonline-0.4.4/invenio_campusonline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:07:56.000000 invenio-campusonline-0.4.4/invenio_campusonline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 21:07:56.000000 invenio-campusonline-0.4.4/invenio_campusonline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:07:56.000000 invenio-campusonline-0.4.4/invenio_campusonline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 21:07:56.000000 invenio-campusonline-0.4.4/invenio_campusonline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 21:07:56.000000 invenio-campusonline-0.4.4/invenio_campusonline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-24 21:07:56.081405 invenio-campusonline-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:07:56.077405 invenio-campusonline-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/tests/minimal_record.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/tests/test_invenio_campusonline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-24 21:07:48.000000 invenio-campusonline-0.4.4/tests/test_utils.py
```

### Comparing `invenio-campusonline-0.4.3/.editorconfig` & `invenio-campusonline-0.4.4/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/.github/workflows/tests.yml` & `invenio-campusonline-0.4.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/.tx/config` & `invenio-campusonline-0.4.4/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/CHANGES.rst` & `invenio-campusonline-0.4.4/CHANGES.rst`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     invenio-campusonline is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.4.4 (release 2024-04-24)
+
+- fix: change not applied to all places
+
+
 Version v0.4.3 (release 2024-03-14)
 
 - fix: cli used wrong cms api words
 
 
 Version v0.4.2 (release 2024-03-12)
```

### Comparing `invenio-campusonline-0.4.3/CONTRIBUTING.rst` & `invenio-campusonline-0.4.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/LICENSE` & `invenio-campusonline-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/MANIFEST.in` & `invenio-campusonline-0.4.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/PKG-INFO` & `invenio-campusonline-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-campusonline
-Version: 0.4.3
+Version: 0.4.4
 Summary: "The module is used to import/export from/to the CampusOnline System."
 Home-page: https://github.com/tu-graz-library/invenio-campusonline
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio TODO
 Platform: any
@@ -53,14 +53,19 @@
     invenio-campusonline is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.4.4 (release 2024-04-24)
+
+- fix: change not applied to all places
+
+
 Version v0.4.3 (release 2024-03-14)
 
 - fix: cli used wrong cms api words
 
 
 Version v0.4.2 (release 2024-03-12)
```

### Comparing `invenio-campusonline-0.4.3/README.rst` & `invenio-campusonline-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/babel.ini` & `invenio-campusonline-0.4.4/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/docs/Makefile` & `invenio-campusonline-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/docs/conf.py` & `invenio-campusonline-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/docs/index.rst` & `invenio-campusonline-0.4.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/docs/make.bat` & `invenio-campusonline-0.4.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/__init__.py` & `invenio-campusonline-0.4.4/invenio_campusonline/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 from .ext import InvenioCampusonline
 from .proxies import current_campusonline
 from .services import CampusOnlineRESTService
 from .types import CampusOnlineID, ThesesFilter
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 __all__ = (
     "__version__",
     "InvenioCampusonline",
     "CampusOnlineID",
     "CampusOnlineRESTService",
     "ThesesFilter",
```

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/cli.py` & `invenio-campusonline-0.4.4/invenio_campusonline/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,18 @@
 @option("--endpoint", type=UrlParamType(may_have_port=True), required=True)
 @option("--token", type=STRING, required=True)
 @option("--campusonline-id", type=STRING, default="")
 @build_services
 def duplicate_check(cms_service: CampusOnlineRESTService, campusonline_id: str) -> None:
     """Duplicate check."""
     duplicate_func = current_app.config["CAMPUSONLINE_DUPLICATE_FUNC"]
-    theses_filters = current_app.config["CAMPUSONLINE_THESES_FILTERS"]
+    theses_filter = current_app.config["CAMPUSONLINE_THESES_FILTER"]
 
     if campusonline_id == "":
-        ids = cms_service.fetch_all_ids(theses_filters)
+        ids = cms_service.fetch_all_ids(theses_filter)
     else:
         ids = [campusonline_id]
 
     duplicates = [cms_id for cms_id in ids if duplicate_func(cms_id)]
 
     for duplicate in duplicates:
         secho(duplicate, fg=Color.neutral)
```

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/config.py` & `invenio-campusonline-0.4.4/invenio_campusonline/config.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/ext.py` & `invenio-campusonline-0.4.4/invenio_campusonline/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/records/api.py` & `invenio-campusonline-0.4.4/invenio_campusonline/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/records/models.py` & `invenio-campusonline-0.4.4/invenio_campusonline/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/services/config.py` & `invenio-campusonline-0.4.4/invenio_campusonline/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/services/decorators.py` & `invenio-campusonline-0.4.4/invenio_campusonline/services/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/services/services.py` & `invenio-campusonline-0.4.4/invenio_campusonline/services/services.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/tasks.py` & `invenio-campusonline-0.4.4/invenio_campusonline/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/types.py` & `invenio-campusonline-0.4.4/invenio_campusonline/types.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline/utils.py` & `invenio-campusonline-0.4.4/invenio_campusonline/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline.egg-info/PKG-INFO` & `invenio-campusonline-0.4.4/invenio_campusonline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-campusonline
-Version: 0.4.3
+Version: 0.4.4
 Summary: "The module is used to import/export from/to the CampusOnline System."
 Home-page: https://github.com/tu-graz-library/invenio-campusonline
 Author: Graz University of Technology
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio TODO
 Platform: any
@@ -53,14 +53,19 @@
     invenio-campusonline is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.4.4 (release 2024-04-24)
+
+- fix: change not applied to all places
+
+
 Version v0.4.3 (release 2024-03-14)
 
 - fix: cli used wrong cms api words
 
 
 Version v0.4.2 (release 2024-03-12)
```

### Comparing `invenio-campusonline-0.4.3/invenio_campusonline.egg-info/SOURCES.txt` & `invenio-campusonline-0.4.4/invenio_campusonline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/setup.cfg` & `invenio-campusonline-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/tests/conftest.py` & `invenio-campusonline-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/tests/minimal_record.xml` & `invenio-campusonline-0.4.4/tests/minimal_record.xml`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/tests/test_invenio_campusonline.py` & `invenio-campusonline-0.4.4/tests/test_invenio_campusonline.py`

 * *Files identical despite different names*

### Comparing `invenio-campusonline-0.4.3/tests/test_utils.py` & `invenio-campusonline-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

