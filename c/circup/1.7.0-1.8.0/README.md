# Comparing `tmp/circup-1.7.0.tar.gz` & `tmp/circup-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circup-1.7.0.tar", last modified: Tue Apr  9 22:59:22 2024, max compression
+gzip compressed data, was "circup-1.8.0.tar", last modified: Wed Apr 24 20:54:54 2024, max compression
```

## Comparing `circup-1.7.0.tar` & `circup-1.8.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.586066 circup-1.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.570066 circup-1.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-09 22:59:11.000000 circup-1.7.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-09 22:59:11.000000 circup-1.7.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.574066 circup-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-09 22:59:11.000000 circup-1.7.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-09 22:59:11.000000 circup-1.7.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 22:59:11.000000 circup-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 22:59:11.000000 circup-1.7.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-09 22:59:11.000000 circup-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-09 22:59:11.000000 circup-1.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-09 22:59:11.000000 circup-1.7.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/CODE_OF_CONDUCT.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-09 22:59:11.000000 circup-1.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/CONTRIBUTING.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-09 22:59:11.000000 circup-1.7.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.574066 circup-1.7.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-09 22:59:11.000000 circup-1.7.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 22:59:11.000000 circup-1.7.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 22:59:11.000000 circup-1.7.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-04-09 22:59:22.582066 circup-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-09 22:59:11.000000 circup-1.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.574066 circup-1.7.0/circup/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 22:59:11.000000 circup-1.7.0/circup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31649 2024-04-09 22:59:11.000000 circup-1.7.0/circup/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-09 22:59:11.000000 circup-1.7.0/circup/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    19934 2024-04-09 22:59:11.000000 circup-1.7.0/circup/command_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-04-09 22:59:11.000000 circup-1.7.0/circup/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.574066 circup-1.7.0/circup/config/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 22:59:11.000000 circup-1.7.0/circup/config/bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 22:59:11.000000 circup-1.7.0/circup/config/bundle_config.json.license
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 22:59:11.000000 circup-1.7.0/circup/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-09 22:59:11.000000 circup-1.7.0/circup/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-09 22:59:11.000000 circup-1.7.0/circup/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.582066 circup-1.7.0/circup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13382 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 22:59:22.000000 circup-1.7.0/circup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.578066 circup-1.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.578066 circup-1.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-09 22:59:11.000000 circup-1.7.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 22:59:11.000000 circup-1.7.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-09 22:59:11.000000 circup-1.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 22:59:11.000000 circup-1.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)    36437 2024-04-09 22:59:11.000000 circup-1.7.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/docs/logo.png.license
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 22:59:11.000000 circup-1.7.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 22:59:11.000000 circup-1.7.0/optional_requirements.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 22:59:11.000000 circup-1.7.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 22:59:11.000000 circup-1.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 22:59:11.000000 circup-1.7.0/requirements.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:59:22.586066 circup-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-09 22:59:11.000000 circup-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.578066 circup-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:11.000000 circup-1.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.578066 circup-1.7.0/tests/bad_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bad_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bad_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bad_python.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bundle.json
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/bundle.json.license
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 22:59:11.000000 circup-1.7.0/tests/device.json
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/device.json.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.582066 circup-1.7.0/tests/dir_module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:11.000000 circup-1.7.0/tests/dir_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-09 22:59:11.000000 circup-1.7.0/tests/dir_module/my_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 22:59:11.000000 circup-1.7.0/tests/import_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 22:59:11.000000 circup-1.7.0/tests/local_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 22:59:11.000000 circup-1.7.0/tests/local_module_cp7.mpy
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/local_module_cp7.mpy.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.582066 circup-1.7.0/tests/mock_device/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mock_device/boot_out.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mock_device/boot_out.txt.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.570066 circup-1.7.0/tests/mock_device/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:22.582066 circup-1.7.0/tests/mock_device/lib/adafruit_waveform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mock_device/lib/adafruit_waveform/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mount_exists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mount_exists.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mount_missing.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/mount_missing.txt.license
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 22:59:11.000000 circup-1.7.0/tests/remote_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_bundle_config.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_bundle_config.json.license
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_bundle_config_local.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_bundle_config_local.json.license
--rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_circup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_module.mpy
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 22:59:11.000000 circup-1.7.0/tests/test_module.mpy.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.824052 circup-1.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-24 20:54:44.000000 circup-1.8.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-24 20:54:44.000000 circup-1.8.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.824052 circup-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-24 20:54:44.000000 circup-1.8.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-24 20:54:44.000000 circup-1.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-24 20:54:44.000000 circup-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 20:54:44.000000 circup-1.8.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-24 20:54:44.000000 circup-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-24 20:54:44.000000 circup-1.8.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-24 20:54:44.000000 circup-1.8.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/CODE_OF_CONDUCT.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-24 20:54:44.000000 circup-1.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/CONTRIBUTING.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-24 20:54:44.000000 circup-1.8.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.824052 circup-1.8.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-24 20:54:44.000000 circup-1.8.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-24 20:54:44.000000 circup-1.8.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 20:54:44.000000 circup-1.8.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-24 20:54:54.836052 circup-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-24 20:54:44.000000 circup-1.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.828052 circup-1.8.0/circup/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 20:54:44.000000 circup-1.8.0/circup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33883 2024-04-24 20:54:44.000000 circup-1.8.0/circup/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-24 20:54:44.000000 circup-1.8.0/circup/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22083 2024-04-24 20:54:44.000000 circup-1.8.0/circup/command_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-04-24 20:54:44.000000 circup-1.8.0/circup/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.828052 circup-1.8.0/circup/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-24 20:54:44.000000 circup-1.8.0/circup/config/bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 20:54:44.000000 circup-1.8.0/circup/config/bundle_config.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 20:54:44.000000 circup-1.8.0/circup/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-24 20:54:44.000000 circup-1.8.0/circup/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-24 20:54:44.000000 circup-1.8.0/circup/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/circup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 20:54:54.000000 circup-1.8.0/circup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.828052 circup-1.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.828052 circup-1.8.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-24 20:54:44.000000 circup-1.8.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 20:54:44.000000 circup-1.8.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-24 20:54:44.000000 circup-1.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 20:54:44.000000 circup-1.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)    36437 2024-04-24 20:54:44.000000 circup-1.8.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/docs/logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 20:54:44.000000 circup-1.8.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 20:54:44.000000 circup-1.8.0/optional_requirements.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 20:54:44.000000 circup-1.8.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 20:54:44.000000 circup-1.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 20:54:44.000000 circup-1.8.0/requirements.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:54:54.836052 circup-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-24 20:54:44.000000 circup-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.832052 circup-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:44.000000 circup-1.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.832052 circup-1.8.0/tests/bad_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bad_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bad_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bad_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bundle.json
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/bundle.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 20:54:44.000000 circup-1.8.0/tests/device.json
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/device.json.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/tests/dir_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:44.000000 circup-1.8.0/tests/dir_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 20:54:44.000000 circup-1.8.0/tests/dir_module/my_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 20:54:44.000000 circup-1.8.0/tests/import_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 20:54:44.000000 circup-1.8.0/tests/local_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 20:54:44.000000 circup-1.8.0/tests/local_module_cp7.mpy
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/local_module_cp7.mpy.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/tests/mock_device/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mock_device/boot_out.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mock_device/boot_out.txt.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.820052 circup-1.8.0/tests/mock_device/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:54.836052 circup-1.8.0/tests/mock_device/lib/adafruit_waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mock_device/lib/adafruit_waveform/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mount_exists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mount_exists.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mount_missing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/mount_missing.txt.license
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 20:54:44.000000 circup-1.8.0/tests/remote_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_bundle_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_bundle_config.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_bundle_config_local.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_bundle_config_local.json.license
+-rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_circup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_module.mpy
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 20:54:44.000000 circup-1.8.0/tests/test_module.mpy.license
```

### Comparing `circup-1.7.0/.github/ISSUE_TEMPLATE.md` & `circup-1.8.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/.github/PULL_REQUEST_TEMPLATE.md` & `circup-1.8.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/.github/workflows/build.yml` & `circup-1.8.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/.github/workflows/release.yml` & `circup-1.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/.gitignore` & `circup-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/.pre-commit-config.yaml` & `circup-1.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/.pylintrc` & `circup-1.8.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/CODE_OF_CONDUCT.rst` & `circup-1.8.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/CONTRIBUTING.rst` & `circup-1.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/LICENSE` & `circup-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/LICENSES/CC-BY-4.0.txt` & `circup-1.8.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/LICENSES/MIT.txt` & `circup-1.8.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/LICENSES/Unlicense.txt` & `circup-1.8.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/PKG-INFO` & `circup-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.7.0
+Version: 1.8.0
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
@@ -55,22 +55,22 @@
 Requires-Dist: black; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: all
 Requires-Dist: wheel; extra == "all"
 Requires-Dist: pytest-faulthandler; extra == "all"
-Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
+Requires-Dist: coverage; extra == "all"
 Requires-Dist: pylint; extra == "all"
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: coverage; extra == "all"
-Requires-Dist: black; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: twine; extra == "all"
 Requires-Dist: sphinx; extra == "all"
+Requires-Dist: black; extra == "all"
+Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
 
 
 CircUp
 ======
 
 .. image:: https://readthedocs.org/projects/circup/badge/?version=latest
     :target: https://circuitpython.readthedocs.io/projects/circup/en/latest/
@@ -161,26 +161,29 @@
     Options:
       --verbose           Comprehensive logging is sent to stdout.
       --path DIRECTORY    Path to CircuitPython directory. Overrides automatic
                           path detection.
       --host TEXT         Hostname or IP address of a device. Overrides automatic
                           path detection.
       --password TEXT     Password to use for authentication when --host is used.
+      --timeout INTEGER   Specify the timeout in seconds for any network
+                          operations.
       --board-id TEXT     Manual Board ID of the CircuitPython device. If provided
                           in combination with --cpy-version, it overrides the
                           detected board ID.
       --cpy-version TEXT  Manual CircuitPython version. If provided in combination
                           with --board-id, it overrides the detected CPy version.
       --version           Show the version and exit.
       --help              Show this message and exit.
 
     Commands:
       bundle-add     Add bundles to the local bundles list, by "user/repo"...
       bundle-remove  Remove one or more bundles from the local bundles list.
       bundle-show    Show the list of bundles, default and local, with URL,...
+      example        Copy named example(s) from a bundle onto the device.
       freeze         Output details of all the modules found on the connected...
       install        Install a named module(s) onto the device.
       list           Lists all out of date modules found on the connected...
       show           Show a list of available modules in the bundle.
       uninstall      Uninstall a named module(s) from the connected device.
       update         Update modules on the device. Use --all to automatically
                      update all modules without Major Version warnings.
```

### Comparing `circup-1.7.0/README.rst` & `circup-1.8.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -91,26 +91,29 @@
     Options:
       --verbose           Comprehensive logging is sent to stdout.
       --path DIRECTORY    Path to CircuitPython directory. Overrides automatic
                           path detection.
       --host TEXT         Hostname or IP address of a device. Overrides automatic
                           path detection.
       --password TEXT     Password to use for authentication when --host is used.
+      --timeout INTEGER   Specify the timeout in seconds for any network
+                          operations.
       --board-id TEXT     Manual Board ID of the CircuitPython device. If provided
                           in combination with --cpy-version, it overrides the
                           detected board ID.
       --cpy-version TEXT  Manual CircuitPython version. If provided in combination
                           with --board-id, it overrides the detected CPy version.
       --version           Show the version and exit.
       --help              Show this message and exit.
 
     Commands:
       bundle-add     Add bundles to the local bundles list, by "user/repo"...
       bundle-remove  Remove one or more bundles from the local bundles list.
       bundle-show    Show the list of bundles, default and local, with URL,...
+      example        Copy named example(s) from a bundle onto the device.
       freeze         Output details of all the modules found on the connected...
       install        Install a named module(s) onto the device.
       list           Lists all out of date modules found on the connected...
       show           Show a list of available modules in the bundle.
       uninstall      Uninstall a named module(s) from the connected device.
       update         Update modules on the device. Use --all to automatically
                      update all modules without Major Version warnings.
```

### Comparing `circup-1.7.0/circup/__init__.py` & `circup-1.8.0/circup/__init__.py`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/circup/backends.py` & `circup-1.8.0/circup/backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import tempfile
 from urllib.parse import urlparse, urljoin
 import click
 import requests
 from requests.adapters import HTTPAdapter
 from requests.auth import HTTPBasicAuth
 
-
 from circup.shared import DATA_DIR, BAD_FILE_FORMAT, extract_metadata, _get_modules_file
 
 #: The location to store a local copy of code.py for use with --auto and
 #  web workflow
 LOCAL_CODE_PY_COPY = os.path.join(DATA_DIR, "code.tmp.py")
 
 
@@ -75,51 +74,64 @@
 
     def _create_library_directory(self, device_path, library_path):
         """
         To be overridden by subclass
         """
         raise NotImplementedError
 
-    def _install_module_py(self, metadata):
+    def install_module_py(self, metadata, location=None):
         """
         To be overridden by subclass
         """
         raise NotImplementedError
 
-    def _install_module_mpy(self, bundle, metadata):
+    def install_module_mpy(self, bundle, metadata):
         """
         To be overridden by subclass
         """
         raise NotImplementedError
 
     # pylint: disable=too-many-locals,too-many-branches,too-many-arguments,too-many-nested-blocks
     def install_module(
-        self, device_path, device_modules, name, pyext, mod_names
+        self, device_path, device_modules, name, pyext, mod_names, upgrade=False
     ):  # pragma: no cover
         """
         Finds a connected device and installs a given module name if it
         is available in the current module bundle and is not already
         installed on the device.
         TODO: There is currently no check for the version.
 
         :param str device_path: The path to the connected board.
         :param list(dict) device_modules: List of module metadata from the device.
         :param str name: Name of module to install
         :param bool pyext: Boolean to specify if the module should be installed from
                         source or from a pre-compiled module
         :param mod_names: Dictionary of metadata from modules that can be generated
                            with get_bundle_versions()
+        :param bool upgrade: Upgrade the specified modules if they're already installed.
         """
         if not name:
             click.echo("No module name(s) provided.")
         elif name in mod_names:
             # Grab device modules to check if module already installed
             if name in device_modules:
-                click.echo("'{}' is already installed.".format(name))
-                return
+                if not upgrade:
+                    # skip already installed modules if no -upgrade flag
+                    click.echo("'{}' is already installed.".format(name))
+                    return
+
+                # uninstall the module before installing
+                name = name.lower()
+                _mod_names = {}
+                for module_item, _metadata in device_modules.items():
+                    _mod_names[module_item.replace(".py", "").lower()] = _metadata
+                if name in _mod_names:
+                    _metadata = _mod_names[name]
+                    module_path = _metadata["path"]
+                    self.uninstall(device_path, module_path)
 
             library_path = (
                 os.path.join(device_path, self.LIB_DIR_PATH)
                 if not isinstance(self, WebBackend)
                 else urljoin(device_path, self.LIB_DIR_PATH)
             )
             metadata = mod_names[name]
@@ -155,18 +167,18 @@
                 return
 
             # Create the library directory first.
             self._create_library_directory(device_path, library_path)
 
             if pyext:
                 # Use Python source for module.
-                self._install_module_py(metadata)
+                self.install_module_py(metadata)
             else:
                 # Use pre-compiled mpy modules.
-                self._install_module_mpy(bundle, metadata)
+                self.install_module_mpy(bundle, metadata)
             click.echo("Installed '{}'.".format(name))
         else:
             click.echo("Unknown module named, '{}'.".format(name))
 
     # def libraries_from_imports(self, code_py, mod_names):
     #     """
     #     To be overridden by subclass
@@ -215,14 +227,20 @@
         board_line = lines[1]
         if board_line.startswith("Board ID:"):
             board_id = board_line[9:].strip()
         else:
             board_id = ""
         return circuit_python, board_id
 
+    def file_exists(self, filepath):
+        """
+        To be overriden by subclass
+        """
+        raise NotImplementedError
+
 
 def _writeable_error():
     click.secho(
         "CircuitPython Web Workflow Device not writable\n - "
         "Remount storage as writable to device (not PC)",
         fg="red",
     )
@@ -246,49 +264,61 @@
         except socket.gaierror as exc:
             raise RuntimeError(
                 "Invalid host: {}.".format(host) + " You should remove the 'http://'"
                 if "http://" in host or "https://" in host
                 else "Could not find or connect to specified device"
             ) from exc
 
-        self.LIB_DIR_PATH = "fs/lib/"
+        self.FS_PATH = "fs/"
+        self.LIB_DIR_PATH = f"{self.FS_PATH}lib/"
         self.host = host
         self.password = password
         self.device_location = f"http://:{self.password}@{self.host}"
 
         self.session = requests.Session()
         self.session.mount(self.device_location, HTTPAdapter(max_retries=5))
         self.library_path = self.device_location + "/" + self.LIB_DIR_PATH
         self.timeout = timeout
 
-    def install_file_http(self, source):
+    def install_file_http(self, source, location=None):
         """
         Install file to device using web workflow.
         :param source source file.
+        :param location the location on the device to copy the source
+          directory in to. If omitted is CIRCUITPY/lib/ used.
         """
         file_name = source.split(os.path.sep)
         file_name = file_name[-2] if file_name[-1] == "" else file_name[-1]
-        target = self.device_location + "/" + self.LIB_DIR_PATH + file_name
+
+        if location is None:
+            target = self.device_location + "/" + self.LIB_DIR_PATH + file_name
+        else:
+            target = self.device_location + "/" + self.FS_PATH + location + file_name
 
         auth = HTTPBasicAuth("", self.password)
 
         with open(source, "rb") as fp:
             r = self.session.put(target, fp.read(), auth=auth, timeout=self.timeout)
             if r.status_code == 409:
                 _writeable_error()
             r.raise_for_status()
 
-    def install_dir_http(self, source):
+    def install_dir_http(self, source, location=None):
         """
         Install directory to device using web workflow.
         :param source source directory.
+        :param location the location on the device to copy the source
+          directory in to. If omitted is CIRCUITPY/lib/ used.
         """
         mod_name = source.split(os.path.sep)
         mod_name = mod_name[-2] if mod_name[-1] == "" else mod_name[-1]
-        target = self.device_location + "/" + self.LIB_DIR_PATH + mod_name
+        if location is None:
+            target = self.device_location + "/" + self.LIB_DIR_PATH + mod_name
+        else:
+            target = self.device_location + "/" + self.FS_PATH + location + mod_name
         target = target + "/" if target[:-1] != "/" else target
         url = urlparse(target)
         auth = HTTPBasicAuth("", url.password)
 
         # Create the top level directory.
         with self.session.put(target, auth=auth, timeout=self.timeout) as r:
             if r.status_code == 409:
@@ -486,15 +516,15 @@
         url = urlparse(device_path)
         auth = HTTPBasicAuth("", url.password)
         with self.session.put(library_path, auth=auth, timeout=self.timeout) as r:
             if r.status_code == 409:
                 _writeable_error()
             r.raise_for_status()
 
-    def _install_module_mpy(self, bundle, metadata):
+    def install_module_mpy(self, bundle, metadata):
         """
         :param bundle library bundle.
         :param library_path library path
         :param metadata dictionary.
         """
         module_name = os.path.basename(metadata["path"]).replace(".py", ".mpy")
         if not module_name:
@@ -510,26 +540,26 @@
         elif os.path.isfile(bundle_path):
             self.install_file_http(bundle_path)
 
         else:
             raise IOError("Cannot find compiled version of module.")
 
     # pylint: enable=too-many-locals,too-many-branches
-    def _install_module_py(self, metadata):
+    def install_module_py(self, metadata, location=None):
         """
         :param library_path library path
         :param metadata dictionary.
         """
 
         source_path = metadata["path"]  # Path to Python source version.
         if os.path.isdir(source_path):
-            self.install_dir_http(source_path)
+            self.install_dir_http(source_path, location=location)
 
         else:
-            self.install_file_http(source_path)
+            self.install_file_http(source_path, location=location)
 
     def get_auto_file_path(self, auto_file_path):
         """
         Make a local temp copy of the --auto file from the device.
         Returns the path to the local copy.
         """
         url = auto_file_path
@@ -556,14 +586,26 @@
         Delete the module on the device, then copy the module from the bundle
         back onto the device.
 
         The caller is expected to handle any exceptions raised.
         """
         self._update_http(module)
 
+    def file_exists(self, filepath):
+        """
+        return True if the file exists, otherwise False.
+        """
+        auth = HTTPBasicAuth("", self.password)
+        resp = requests.get(
+            self.get_file_path(filepath), auth=auth, timeout=self.timeout
+        )
+        if resp.status_code == 200:
+            return True
+        return False
+
     def _update_http(self, module):
         """
         Update the module using web workflow.
         """
         if module.file:
             # Copy the file (will overwrite).
             self.install_file_http(module.bundle_path)
@@ -729,18 +771,17 @@
         """
         return _get_modules_file(device_lib_path, self.logger)
 
     def _create_library_directory(self, device_path, library_path):
         if not os.path.exists(library_path):  # pragma: no cover
             os.makedirs(library_path)
 
-    def _install_module_mpy(self, bundle, metadata):
+    def install_module_mpy(self, bundle, metadata):
         """
         :param bundle library bundle.
-        :param library_path library path
         :param metadata dictionary.
         """
         module_name = os.path.basename(metadata["path"]).replace(".py", ".mpy")
         if not module_name:
             # Must be a directory based module.
             module_name = os.path.basename(os.path.dirname(metadata["path"]))
 
@@ -759,29 +800,34 @@
 
             # Copy file.
             shutil.copyfile(bundle_path, target_path)
         else:
             raise IOError("Cannot find compiled version of module.")
 
     # pylint: enable=too-many-locals,too-many-branches
-    def _install_module_py(self, metadata):
+    def install_module_py(self, metadata, location=None):
         """
-        :param library_path library path
         :param metadata dictionary.
+        :param location the location on the device to copy the py module to.
+          If omitted is CIRCUITPY/lib/ used.
         """
+        if location is None:
+            location = self.library_path
+        else:
+            location = os.path.join(self.device_location, location)
 
         source_path = metadata["path"]  # Path to Python source version.
         if os.path.isdir(source_path):
             target = os.path.basename(os.path.dirname(source_path))
-            target_path = os.path.join(self.library_path, target)
+            target_path = os.path.join(location, target)
             # Copy the directory.
             shutil.copytree(source_path, target_path)
         else:
             target = os.path.basename(source_path)
-            target_path = os.path.join(self.library_path, target)
+            target_path = os.path.join(location, target)
             # Copy file.
             shutil.copyfile(source_path, target_path)
 
     def get_auto_file_path(self, auto_file_path):
         """
         Returns the path on the device to the file to be read for --auto.
         """
@@ -821,14 +867,20 @@
             shutil.rmtree(module.path, ignore_errors=True)
             shutil.copytree(module.bundle_path, module.path)
         else:
             # Delete and copy file.
             os.remove(module.path)
             shutil.copyfile(module.bundle_path, module.path)
 
+    def file_exists(self, filepath):
+        """
+        return True if the file exists, otherwise False.
+        """
+        return os.path.exists(os.path.join(self.device_location, filepath))
+
     def get_file_path(self, filename):
         """
         returns the full path on the device to a given file name.
         """
         return os.path.join(self.device_location, filename)
 
     def is_device_present(self):
```

### Comparing `circup-1.7.0/circup/bundle.py` & `circup-1.8.0/circup/bundle.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,28 @@
         tag = self.current_tag
         return os.path.join(
             self.dir.format(platform=platform),
             self.basename.format(platform=PLATFORMS[platform], tag=tag),
             "lib",
         )
 
+    def examples_dir(self, platform):
+        """
+        This bundle's examples directory for the platform.
+
+        :param str platform: The platform identifier (py/6mpy/...).
+        :return: The path to the examples directory for the platform.
+        """
+        tag = self.current_tag
+        return os.path.join(
+            self.dir.format(platform=platform),
+            self.basename.format(platform=PLATFORMS[platform], tag=tag),
+            "examples",
+        )
+
     def requirements_for(self, library_name, toml_file=False):
         """
         The requirements file for this library.
 
         :param str library_name: The name of the library.
         :return: The path to the requirements.txt file.
         """
```

### Comparing `circup-1.7.0/circup/command_utils.py` & `circup-1.8.0/circup/command_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,31 @@
     available_modules = get_bundle_versions(get_bundles_list(), avoid_download=True)
     module_names = {m.replace(".py", "") for m in available_modules}
     if incomplete:
         module_names = [name for name in module_names if name.startswith(incomplete)]
     return sorted(module_names)
 
 
+def completion_for_example(ctx, param, incomplete):
+    """
+    Returns the list of available modules for the command line tab-completion
+    with the ``circup example`` command.
+    """
+    # pylint: disable=unused-argument, consider-iterating-dictionary
+    available_examples = get_bundle_examples(get_bundles_list(), avoid_download=True)
+
+    matching_examples = [
+        example_path
+        for example_path in available_examples.keys()
+        if example_path.startswith(incomplete)
+    ]
+
+    return sorted(matching_examples)
+
+
 def ensure_latest_bundle(bundle):
     """
     Ensure that there's a copy of the latest library bundle available so circup
     can check the metadata contained therein.
 
     :param Bundle bundle: the target Bundle object.
     """
@@ -286,14 +303,51 @@
             shutil.rmtree(temp_dir)
         with zipfile.ZipFile(temp_zip, "r") as zfile:
             zfile.extractall(temp_dir)
     bundle.current_tag = tag
     click.echo("\nOK\n")
 
 
+def get_bundle_examples(bundles_list, avoid_download=False):
+    """
+    Return a dictionary of metadata from examples in the all of the bundles
+    specified by bundles_list argument.
+
+    :param List[Bundle] bundles_list: List of supported bundles as Bundle objects.
+    :param bool avoid_download: if True, download the bundle only if missing.
+    :return: A dictionary of metadata about the examples available in the
+             library bundle.
+    """
+    # pylint: disable=too-many-nested-blocks
+    all_the_examples = dict()
+
+    try:
+        for bundle in bundles_list:
+            if not avoid_download or not os.path.isdir(bundle.lib_dir("py")):
+                ensure_latest_bundle(bundle)
+            path = bundle.examples_dir("py")
+            path_examples = _get_modules_file(path, logger)
+            for lib_name, lib_metadata in path_examples.items():
+                for _dir_level in os.walk(lib_metadata["path"]):
+                    for _file in _dir_level[2]:
+                        _parts = _dir_level[0].split(os.path.sep)
+                        _lib_name_index = _parts.index(lib_name)
+                        _dirs = _parts[_lib_name_index:]
+                        if _dirs[-1] == "":
+                            _dirs.pop(-1)
+                        slug = f"{os.path.sep}".join(_dirs + [_file.replace(".py", "")])
+                        all_the_examples[slug] = os.path.join(_dir_level[0], _file)
+
+    except NotADirectoryError:
+        # Bundle does not have new style examples directory
+        # so we cannot include its examples.
+        pass
+    return all_the_examples
+
+
 def get_bundle_versions(bundles_list, avoid_download=False):
     """
     Returns a dictionary of metadata from modules in the latest known release
     of the library bundle. Uses the Python version (rather than the compiled
     version) of the library modules.
 
     :param List[Bundle] bundles_list: List of supported bundles as Bundle objects.
```

### Comparing `circup-1.7.0/circup/commands.py` & `circup-1.8.0/circup/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     get_bundle_versions,
     libraries_from_requirements,
     libraries_from_code_py,
     get_dependencies,
     get_bundles_local_dict,
     save_local_bundles,
     get_bundles_dict,
+    completion_for_example,
+    get_bundle_examples,
 )
 
 
 @click.group()
 @click.option(
     "--verbose", is_flag=True, help="Comprehensive logging is sent to stdout."
 )
@@ -281,21 +283,26 @@
     help="specify a text file to install all modules listed in the text file."
     " Typically requirements.txt.",
 )
 @click.option(
     "--auto", "-a", is_flag=True, help="Install the modules imported in code.py."
 )
 @click.option(
+    "--upgrade", "-U", is_flag=True, help="Upgrade modules that are already installed."
+)
+@click.option(
     "--auto-file",
     default=None,
     help="Specify the name of a file on the board to read for auto install."
     " Also accepts an absolute path or a local ./ path.",
 )
 @click.pass_context
-def install(ctx, modules, pyext, requirement, auto, auto_file):  # pragma: no cover
+def install(
+    ctx, modules, pyext, requirement, auto, auto_file, upgrade=False
+):  # pragma: no cover
     """
     Install a named module(s) onto the device. Multiple modules
     can be installed at once by providing more than one module name, each
     separated by a space.
     """
 
     # TODO: Ensure there's enough space on the device
@@ -339,15 +346,59 @@
     to_install = get_dependencies(requested_installs, mod_names=mod_names)
     device_modules = ctx.obj["backend"].get_device_versions()
     if to_install is not None:
         to_install = sorted(to_install)
         click.echo(f"Ready to install: {to_install}\n")
         for library in to_install:
             ctx.obj["backend"].install_module(
-                ctx.obj["DEVICE_PATH"], device_modules, library, pyext, mod_names
+                ctx.obj["DEVICE_PATH"],
+                device_modules,
+                library,
+                pyext,
+                mod_names,
+                upgrade,
+            )
+
+
+@main.command()
+@click.option("--overwrite", is_flag=True, help="Overwrite the file if it exists.")
+@click.argument(
+    "examples", required=True, nargs=-1, shell_complete=completion_for_example
+)
+@click.pass_context
+def example(ctx, examples, overwrite):
+    """
+    Copy named example(s) from a bundle onto the device. Multiple examples
+    can be installed at once by providing more than one example name, each
+    separated by a space.
+    """
+
+    for example_arg in examples:
+        available_examples = get_bundle_examples(
+            get_bundles_list(), avoid_download=True
+        )
+        if example_arg in available_examples:
+            filename = available_examples[example_arg].split(os.path.sep)[-1]
+
+            if overwrite or not ctx.obj["backend"].file_exists(filename):
+                click.echo(
+                    f"{'Copying' if not overwrite else 'Overwriting'}: {filename}"
+                )
+                ctx.obj["backend"].install_module_py(
+                    {"path": available_examples[example_arg]}, location=""
+                )
+            else:
+                click.secho(
+                    f"File: {filename} already exists. Use --overwrite if you wish to replace it.",
+                    fg="red",
+                )
+        else:
+            click.secho(
+                f"Error: {example_arg} was not found in any local bundle examples.",
+                fg="red",
             )
 
 
 # pylint: enable=too-many-arguments,too-many-locals
 
 
 @main.command()
```

### Comparing `circup-1.7.0/circup/logging.py` & `circup-1.8.0/circup/logging.py`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/circup/module.py` & `circup-1.8.0/circup/module.py`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/circup/shared.py` & `circup-1.8.0/circup/shared.py`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/circup.egg-info/PKG-INFO` & `circup-1.8.0/circup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circup
-Version: 1.7.0
+Version: 1.8.0
 Summary: A tool to manage/update libraries on CircuitPython devices.
 Home-page: https://github.com/adafruit/circup
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit,blinka,circuitpython,micropython,libraries
 Classifier: Development Status :: 3 - Alpha
@@ -55,22 +55,22 @@
 Requires-Dist: black; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: all
 Requires-Dist: wheel; extra == "all"
 Requires-Dist: pytest-faulthandler; extra == "all"
-Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
+Requires-Dist: coverage; extra == "all"
 Requires-Dist: pylint; extra == "all"
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: coverage; extra == "all"
-Requires-Dist: black; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: twine; extra == "all"
 Requires-Dist: sphinx; extra == "all"
+Requires-Dist: black; extra == "all"
+Requires-Dist: pytest-random-order>=1.0.0; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
 
 
 CircUp
 ======
 
 .. image:: https://readthedocs.org/projects/circup/badge/?version=latest
     :target: https://circuitpython.readthedocs.io/projects/circup/en/latest/
@@ -161,26 +161,29 @@
     Options:
       --verbose           Comprehensive logging is sent to stdout.
       --path DIRECTORY    Path to CircuitPython directory. Overrides automatic
                           path detection.
       --host TEXT         Hostname or IP address of a device. Overrides automatic
                           path detection.
       --password TEXT     Password to use for authentication when --host is used.
+      --timeout INTEGER   Specify the timeout in seconds for any network
+                          operations.
       --board-id TEXT     Manual Board ID of the CircuitPython device. If provided
                           in combination with --cpy-version, it overrides the
                           detected board ID.
       --cpy-version TEXT  Manual CircuitPython version. If provided in combination
                           with --board-id, it overrides the detected CPy version.
       --version           Show the version and exit.
       --help              Show this message and exit.
 
     Commands:
       bundle-add     Add bundles to the local bundles list, by "user/repo"...
       bundle-remove  Remove one or more bundles from the local bundles list.
       bundle-show    Show the list of bundles, default and local, with URL,...
+      example        Copy named example(s) from a bundle onto the device.
       freeze         Output details of all the modules found on the connected...
       install        Install a named module(s) onto the device.
       list           Lists all out of date modules found on the connected...
       show           Show a list of available modules in the bundle.
       uninstall      Uninstall a named module(s) from the connected device.
       update         Update modules on the device. Use --all to automatically
                      update all modules without Major Version warnings.
```

### Comparing `circup-1.7.0/circup.egg-info/SOURCES.txt` & `circup-1.8.0/circup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/docs/_static/favicon.ico` & `circup-1.8.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/docs/conf.py` & `circup-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/docs/logo.png` & `circup-1.8.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/setup.py` & `circup-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/tests/bundle.json` & `circup-1.8.0/tests/bundle.json`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/tests/mount_exists.txt` & `circup-1.8.0/tests/mount_exists.txt`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/tests/test_circup.py` & `circup-1.8.0/tests/test_circup.py`

 * *Files identical despite different names*

### Comparing `circup-1.7.0/tests/test_module.mpy` & `circup-1.8.0/tests/test_module.mpy`

 * *Files identical despite different names*

