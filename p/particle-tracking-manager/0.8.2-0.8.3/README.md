# Comparing `tmp/particle_tracking_manager-0.8.2.tar.gz` & `tmp/particle_tracking_manager-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "particle_tracking_manager-0.8.2.tar", last modified: Thu Apr 11 02:15:04 2024, max compression
+gzip compressed data, was "particle_tracking_manager-0.8.3.tar", last modified: Tue Apr 23 19:06:49 2024, max compression
```

## Comparing `particle_tracking_manager-0.8.2.tar` & `particle_tracking_manager-0.8.3.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.126199 particle_tracking_manager-0.8.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.130199 particle_tracking_manager-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.130199 particle_tracking_manager-0.8.2/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/ci/environment-py3.10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/ci/environment-py3.11.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/ci/environment-py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.130199 particle_tracking_manager-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/more_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/docs/whats_new.md
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.130199 particle_tracking_manager-0.8.2/particle_tracking_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/particle_tracking_manager/models/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    51864 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/opendrift.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    24422 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/the_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/particle_tracking_manager/the_manager_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 02:15:04.000000 particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:15:04.134199 particle_tracking_manager-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_opendrift.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_realistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-11 02:14:58.000000 particle_tracking_manager-0.8.2/tests/test_seeding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.989557 particle_tracking_manager-0.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.985557 particle_tracking_manager-0.8.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.985557 particle_tracking_manager-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-23 19:06:49.989557 particle_tracking_manager-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.985557 particle_tracking_manager-0.8.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/ci/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/ci/environment-py3.11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/ci/environment-py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.985557 particle_tracking_manager-0.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/more_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/docs/whats_new.md
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.989557 particle_tracking_manager-0.8.3/particle_tracking_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 19:06:49.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.989557 particle_tracking_manager-0.8.3/particle_tracking_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.989557 particle_tracking_manager-0.8.3/particle_tracking_manager/models/opendrift/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/models/opendrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/models/opendrift/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50773 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/models/opendrift/opendrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24422 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/the_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/particle_tracking_manager/the_manager_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.989557 particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-23 19:06:49.000000 particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-23 19:06:49.000000 particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:06:49.000000 particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 19:06:49.000000 particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 19:06:49.000000 particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 19:06:49.000000 particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-23 19:06:49.989557 particle_tracking_manager-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:06:49.989557 particle_tracking_manager-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/tests/test_opendrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/tests/test_realistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-23 19:06:42.000000 particle_tracking_manager-0.8.3/tests/test_seeding.py
```

### Comparing `particle_tracking_manager-0.8.2/.github/workflows/release.yaml` & `particle_tracking_manager-0.8.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/.github/workflows/test.yaml` & `particle_tracking_manager-0.8.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/.gitignore` & `particle_tracking_manager-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/.pre-commit-config.yaml` & `particle_tracking_manager-0.8.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/LICENSE.txt` & `particle_tracking_manager-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/PKG-INFO` & `particle_tracking_manager-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: particle_tracking_manager
-Version: 0.8.2
+Version: 0.8.3
 Summary: Manager for particle tracking simulations.
 Home-page: https://github.com/axiom-data-science/particle-tracking-manager
 Author: axiom-data-science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `particle_tracking_manager-0.8.2/README.md` & `particle_tracking_manager-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/ci/environment-py3.10.yml` & `particle_tracking_manager-0.8.3/ci/environment-py3.10.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/ci/environment-py3.11.yml` & `particle_tracking_manager-0.8.3/ci/environment-py3.11.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/ci/environment-py3.9.yml` & `particle_tracking_manager-0.8.3/ci/environment-py3.9.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/Makefile` & `particle_tracking_manager-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/conf.py` & `particle_tracking_manager-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/configuration.md` & `particle_tracking_manager-0.8.3/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/environment.yml` & `particle_tracking_manager-0.8.3/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/index.rst` & `particle_tracking_manager-0.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/more_examples.md` & `particle_tracking_manager-0.8.3/docs/more_examples.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/quick_start.md` & `particle_tracking_manager-0.8.3/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/tutorial.md` & `particle_tracking_manager-0.8.3/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/docs/whats_new.md` & `particle_tracking_manager-0.8.3/docs/whats_new.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # What's New
 
+## v0.8.3 (April 23, 2024)
+
+* removed `Dcrit` because realized it is not necessary
+* improved log handling for CLI
+* changed `OpenDrift` default handling so they are now changed to None
+
 ## v0.8.2 (April 10, 2024)
 
 * updated docs
 * improved `drift_model_config()`
 * updated tests
 * now include PTM metadata with output file
```

### Comparing `particle_tracking_manager-0.8.2/particle_tracking_manager/cli.py` & `particle_tracking_manager-0.8.3/particle_tracking_manager/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Command line interface to get inputs from web application."""
 
 import argparse
 import ast
+import logging
 
 from datetime import datetime
 
 import pandas as pd
 
 import particle_tracking_manager as ptm
 
@@ -118,24 +119,50 @@
     to_bool = {
         key: ast.literal_eval(value)
         for key, value in args.kwargs.items()
         if value in ["True", "False"]
     }
     args.kwargs.update(to_bool)
 
+    if "output_file" not in args.kwargs:
+
+        args.kwargs[
+            "output_file"
+        ] = f"output-results_{datetime.utcnow():%Y-%m-%dT%H%M:%SZ}.nc"
+
+    log_file = args.kwargs["output_file"].replace(".nc", ".log")
+
+    # Create a file handler
+    file_handler = logging.FileHandler(log_file)
+
+    # Create a formatter and add it to the handler
+    formatter = logging.Formatter(
+        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    )
+    file_handler.setFormatter(formatter)
+
     m = ptm.OpenDriftModel(**args.kwargs)
 
     if args.dry_run:
 
         # run this to make sure everything is updated fully
         m.add_reader()
         print(m.drift_model_config())
 
     else:
 
+        # Add the handler to the logger
+        m.logger.addHandler(file_handler)
+
+        m.logger.info(f"filename: {args.kwargs['output_file']}")
+
         m.add_reader()
         print(m.drift_model_config())
 
         m.seed()
         m.run()
 
         print(m.outfile_name)
+
+    # Remove the handler at the end of the loop
+    m.logger.removeHandler(file_handler)
+    file_handler.close()
```

### Comparing `particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/config.json` & `particle_tracking_manager-0.8.3/particle_tracking_manager/models/opendrift/config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9711538461538461%*

 * *Differences: {"'max_speed'": "{'default': 5}", 'delete': "['Dcrit']"}*

```diff
@@ -1,13 +1,8 @@
 {
-    "Dcrit": {
-        "default": 0.1,
-        "od_mapping": "general:seafloor_action_dcrit",
-        "ptm_level": 3
-    },
     "biodegradation": {
         "default": true,
         "od_mapping": "processes:biodegradation",
         "ptm_level": 1
     },
     "coastline_action": {
         "default": "previous",
@@ -112,15 +107,15 @@
     },
     "m3_per_hour": {
         "default": 1,
         "od_mapping": "seed:m3_per_hour",
         "ptm_level": 1
     },
     "max_speed": {
-        "default": 2,
+        "default": 5,
         "od_mapping": "drift:max_speed"
     },
     "mixed_layer_depth": {
         "default": 30,
         "od_mapping": "environment:fallback:ocean_mixed_layer_thickness",
         "ptm_level": 3
     },
```

### Comparing `particle_tracking_manager-0.8.2/particle_tracking_manager/models/opendrift/opendrift.py` & `particle_tracking_manager-0.8.3/particle_tracking_manager/models/opendrift/opendrift.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,23 +323,14 @@
             # and name != "config_model"
             # and name != "config_ptm"
             and name in self.config_model.keys()
         ):
             self.config_model[name]["value"] = value
         self._update_config()
 
-        if name == "ocean_model":
-            if value == "NWGOA":
-                self.Dcrit = 0.5
-            elif "CIOFS" in value:
-                self.Dcrit = 0.3
-            else:
-                self.Dcrit = 0.1
-            self.logger.info(f"For ocean_model {value}, setting Dcrit to {self.Dcrit}.")
-
         if name in ["ocean_model", "horizontal_diffusivity"]:
 
             # just set the value and move on if purposely setting a non-None value
             # of horizontal_diffusivity; specifying this for clarity (already set
             # value above).
             if name == "horizontal_diffusivity" and value is not None:
                 self.logger.info(
@@ -427,41 +418,32 @@
 
         # if drift_model is LarvalFish, do3D has to be True
         if name == "do3D" and not value and self.drift_model == "LarvalFish":
             raise ValueError(
                 "drift_model is LarvalFish which is always 3D in OpenDrift so do3D must be True."
             )
 
-        # Make sure vertical_mixing_timestep equals default value if vertical_mixing False
+        # Make sure vertical_mixing_timestep equals None if vertical_mixing False
         if name in ["vertical_mixing", "vertical_mixing_timestep"]:
-            vmtdef = self.config_model["vertical_mixing_timestep"]["default"]
-            if (
-                not self.vertical_mixing
-                and self.vertical_mixing_timestep != vmtdef
-                and self.vertical_mixing_timestep is not None
-            ):
+            if not self.vertical_mixing:
                 self.logger.info(
-                    "vertical_mixing is False, so resetting value of vertical_mixing_timestep to default and not using."
+                    "vertical_mixing is False, so setting value of vertical_mixing_timestep "
+                    "to None."
                 )
-                self.__dict__["vertical_mixing_timestep"] = vmtdef
-                self.config_model["vertical_mixing_timestep"]["value"] = vmtdef
+                self.__dict__["vertical_mixing_timestep"] = None
+                self.config_model["vertical_mixing_timestep"]["value"] = None
 
-        # Make sure diffusivitymodel equals default value if vertical_mixing False
+        # Make sure diffusivitymodel equals None if vertical_mixing False
         if name in ["vertical_mixing", "diffusivitymodel"]:
-            dmodeldef = self.config_model["diffusivitymodel"]["default"]
-            if (
-                not self.vertical_mixing
-                and self.diffusivitymodel != dmodeldef
-                and self.diffusivitymodel is not None
-            ):
+            if not self.vertical_mixing:
                 self.logger.info(
-                    "vertical_mixing is False, so resetting value of diffusivitymodel to default and not using."
+                    "vertical_mixing is False, so setting value of diffusivitymodel to None."
                 )
-                self.__dict__["diffusivitymodel"] = dmodeldef
-                self.config_model["diffusivitymodel"]["value"] = dmodeldef
+                self.__dict__["diffusivitymodel"] = None
+                self.config_model["diffusivitymodel"]["value"] = None
 
         # Make sure mixed_layer_depth equals default value if vertical_mixing False
         if name in ["vertical_mixing", "mixed_layer_depth"]:
             mlddef = self.config_model["mixed_layer_depth"]["default"]
             if (
                 not self.vertical_mixing
                 and self.mixed_layer_depth != mlddef
@@ -469,44 +451,36 @@
             ):
                 self.logger.info(
                     "vertical_mixing is False, so resetting value of mixed_layer_depth to default and not using."
                 )
                 self.__dict__["mixed_layer_depth"] = mlddef
                 self.config_model["mixed_layer_depth"]["value"] = mlddef
 
-        # make sure user isn't try to use Leeway and "wind_drift_factor" at the same time
-        if name in ["drift_model", "wind_drift_factor"]:
-            mdfdef = self.config_model["wind_drift_factor"]["default"]
-            if (
-                self.drift_model == "Leeway"
-                and self.wind_drift_factor != mdfdef
-                and self.wind_drift_factor is not None
-            ):
+        # make sure user isn't try to use Leeway or LarvalFish and "wind_drift_factor" at the same time
+        if name == "wind_drift_factor":
+            if self.drift_model in ["Leeway", "LarvalFish"]:
                 self.logger.info(
-                    "wind_drift_factor cannot be used with Leeway model, so resetting value to default and not using."
+                    "wind_drift_factor cannot be used with Leeway or LarvalFish models, "
+                    "so setting to None."
                 )
-                self.__dict__["wind_drift_factor"] = mdfdef
-                self.config_model["wind_drift_factor"]["value"] = mdfdef
+                self.__dict__["wind_drift_factor"] = None
+                self.config_model["wind_drift_factor"]["value"] = None
 
-        # make sure user isn't try to use Leeway and "wind_drift_depth" at the same time
-        if name in ["drift_model", "wind_drift_depth"]:
-            mdddef = self.config_model["wind_drift_depth"]["default"]
-            if (
-                self.drift_model == "Leeway"
-                and self.wind_drift_depth != mdddef
-                and self.wind_drift_depth is not None
-            ):
+        # make sure user isn't try to use Leeway or LarvalFish models and "wind_drift_depth" at the same time
+        if name == "wind_drift_depth":
+            if self.drift_model in ["Leeway", "LarvalFish"]:
                 self.logger.info(
-                    "wind_drift_depth cannot be used with Leeway model, so resetting value to default and not using."
+                    "wind_drift_depth cannot be used with Leeway or LarvalFish models, "
+                    "so setting to None."
                 )
-                self.__dict__["wind_drift_depth"] = mdddef
-                self.config_model["wind_drift_depth"]["value"] = mdddef
+                self.__dict__["wind_drift_depth"] = None
+                self.config_model["wind_drift_depth"]["value"] = None
 
         # make sure user isn't try to use Leeway and "stokes_drift" at the same time
-        if name in ["drift_model", "stokes_drift"]:
+        if name == "stokes_drift":
             if self.drift_model == "Leeway" and self.stokes_drift:
                 self.logger.info(
                     "stokes_drift cannot be used with Leeway model, so changing to False."
                 )
                 self.__dict__["stokes_drift"] = False
                 self.config_model["stokes_drift"]["value"] = False
 
@@ -1084,24 +1058,26 @@
         """
 
         outlist = [
             (key, value_dict["value"])
             for key, value_dict in self.show_config(
                 substring=":", ptm_level=ptm_level, level=[1, 2, 3], prefix=prefix
             ).items()
-            if "value" in value_dict
+            if "value" in value_dict and value_dict["value"] is not None
         ]
 
         # also PTM config parameters that are separate from OpenDrift parameters
         outlist2 = [
             (key, value_dict["value"])
             for key, value_dict in self.show_config(
                 ptm_level=ptm_level, prefix=prefix
             ).items()
-            if "od_mapping" not in value_dict and "value" in value_dict
+            if "od_mapping" not in value_dict
+            and "value" in value_dict
+            and value_dict["value"] is not None
         ]
 
         # extra parameters that are not in the config_model but are set by PTM indirectly
         extra_keys = [
             "drift:vertical_advection",
             "drift:truncate_ocean_model_below_m",
             "drift:use_tabularised_stokes_drift",
```

### Comparing `particle_tracking_manager-0.8.2/particle_tracking_manager/plotting.py` & `particle_tracking_manager-0.8.3/particle_tracking_manager/plotting.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/particle_tracking_manager/the_manager.py` & `particle_tracking_manager-0.8.3/particle_tracking_manager/the_manager.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/particle_tracking_manager/the_manager_config.json` & `particle_tracking_manager-0.8.3/particle_tracking_manager/the_manager_config.json`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/PKG-INFO` & `particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: particle_tracking_manager
-Version: 0.8.2
+Version: 0.8.3
 Summary: Manager for particle tracking simulations.
 Home-page: https://github.com/axiom-data-science/particle-tracking-manager
 Author: axiom-data-science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `particle_tracking_manager-0.8.2/particle_tracking_manager.egg-info/SOURCES.txt` & `particle_tracking_manager-0.8.3/particle_tracking_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 docs/environment.yml
 docs/index.rst
 docs/more_examples.md
 docs/quick_start.md
 docs/tutorial.md
 docs/whats_new.md
 particle_tracking_manager/__init__.py
+particle_tracking_manager/_version.py
 particle_tracking_manager/cli.py
 particle_tracking_manager/plotting.py
 particle_tracking_manager/the_manager.py
 particle_tracking_manager/the_manager_config.json
 particle_tracking_manager.egg-info/PKG-INFO
 particle_tracking_manager.egg-info/SOURCES.txt
 particle_tracking_manager.egg-info/dependency_links.txt
```

### Comparing `particle_tracking_manager-0.8.2/pyproject.toml` & `particle_tracking_manager-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/setup.cfg` & `particle_tracking_manager-0.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/tests/conftest.py` & `particle_tracking_manager-0.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/tests/test_cli.py` & `particle_tracking_manager-0.8.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/tests/test_config.py` & `particle_tracking_manager-0.8.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/tests/test_manager.py` & `particle_tracking_manager-0.8.3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/tests/test_opendrift.py` & `particle_tracking_manager-0.8.3/tests/test_opendrift.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,15 @@
         self.assertEqual(self.odm.drift_model, config_model["drift_model"]["default"])
         self.assertEqual(self.odm.radius, config_model["radius"]["default"])
         self.assertEqual(self.odm.radius_type, config_model["radius_type"]["default"])
         # self.assertEqual(self.odm.horizontal_diffusivity, config_model["horizontal_diffusivity"]["default"])
         self.assertEqual(
             self.odm.use_auto_landmask, config_model["use_auto_landmask"]["default"]
         )
-        self.assertEqual(
-            self.odm.diffusivitymodel, config_model["diffusivitymodel"]["default"]
-        )
+        self.assertEqual(self.odm.diffusivitymodel, None)
         self.assertEqual(self.odm.stokes_drift, config_model["stokes_drift"]["default"])
         self.assertEqual(
             self.odm.mixed_layer_depth, config_model["mixed_layer_depth"]["default"]
         )
         self.assertEqual(
             self.odm.coastline_action, config_model["coastline_action"]["default"]
         )
@@ -40,15 +38,15 @@
             self.odm.wind_drift_factor, config_model["wind_drift_factor"]["default"]
         )
         self.assertEqual(
             self.odm.wind_drift_depth, config_model["wind_drift_depth"]["default"]
         )
         self.assertEqual(
             self.odm.vertical_mixing_timestep,
-            config_model["vertical_mixing_timestep"]["default"],
+            None,
         )
         self.assertEqual(self.odm.object_type, config_model["object_type"]["default"])
         self.assertEqual(self.odm.diameter, config_model["diameter"]["default"])
         self.assertEqual(
             self.odm.neutral_buoyancy_salinity,
             config_model["neutral_buoyancy_salinity"]["default"],
         )
@@ -271,46 +269,46 @@
         self.m.do3D = True
         # assert self.m.show_config(key="drift:vertical_advection")["value"]
 
     def test_vertical_mixing_false_vertical_mixing_timestep_not_default(self):
         self.m.vertical_mixing = False
         self.m.vertical_mixing_timestep = 10
         d = self.m.show_config(key="vertical_mixing_timestep")
-        assert d["value"] == d["default"]
+        assert d["value"] == None
 
     def test_vertical_mixing_false_diffusivitymodel_not_default(self):
         self.m.vertical_mixing = False
         self.m.diffusivitymodel = "not_default"
         d = self.m.show_config(key="diffusivitymodel")
-        assert d["value"] == d["default"]
+        assert d["value"] == None
 
     def test_vertical_mixing_false_mixed_layer_depth_not_default(self):
         self.m.vertical_mixing = False
         self.m.mixed_layer_depth = 10
         d = self.m.show_config(key="mixed_layer_depth")
-        assert d["value"] == d["default"]
+        assert d["value"] == 30
 
 
 class TestOpenDriftModel_Leeway(unittest.TestCase):
     def setUp(self):
         self.m = OpenDriftModel(
             drift_model="Leeway", object_type=">PIW, scuba suit (face up)"
         )
 
     def test_leeway_model_wind_drift_factor_not_default(self):
         self.m.wind_drift_factor = 10
         d = self.m.show_config(key="wind_drift_factor")
-        assert d["value"] == d["default"]
+        assert d["value"] == None
         assert self.m.object_type == ">PIW, scuba suit (face up)"
         assert self.m.o._config["object_type"]["value"] == ">PIW, scuba suit (face up)"
 
     def test_leeway_model_wind_drift_depth_not_default(self):
         self.m.wind_drift_depth = 10
         d = self.m.show_config(key="wind_drift_depth")
-        assert d["value"] == d["default"]
+        assert d["value"] == None
 
     def test_leeway_model_stokes_drift_true(self):
         self.m.stokes_drift = True
         assert not self.m.stokes_drift
         # assert not self.m.show_config(key="stokes_drift")["value"]
```

### Comparing `particle_tracking_manager-0.8.2/tests/test_realistic.py` & `particle_tracking_manager-0.8.3/tests/test_realistic.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.2/tests/test_seeding.py` & `particle_tracking_manager-0.8.3/tests/test_seeding.py`

 * *Files identical despite different names*

