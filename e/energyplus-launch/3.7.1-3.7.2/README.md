# Comparing `tmp/energyplus_launch-3.7.1.tar.gz` & `tmp/energyplus_launch-3.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.7.1.tar", last modified: Mon Jun 12 21:52:03 2023, max compression
+gzip compressed data, was "energyplus_launch-3.7.2.tar", last modified: Wed Apr 24 15:29:33 2024, max compression
```

## Comparing `energyplus_launch-3.7.1.tar` & `energyplus_launch-3.7.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.334240 energyplus_launch-3.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-06-12 21:52:03.334240 energyplus_launch-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-12 21:52:03.000000 energyplus_launch-3.7.1/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6211 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     5319 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    78204 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/interface/widget_group_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.330240 energyplus_launch-3.7.1/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 21:52:03.334240 energyplus_launch-3.7.1/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5376 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-12 21:52:03.334240 energyplus_launch-3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-06-12 21:51:55.000000 energyplus_launch-3.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:33.274385 energyplus_launch-3.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-24 15:29:33.274385 energyplus_launch-3.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:33.270385 energyplus_launch-3.7.2/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-24 15:29:33.000000 energyplus_launch-3.7.2/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-24 15:29:33.000000 energyplus_launch-3.7.2/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:29:33.000000 energyplus_launch-3.7.2/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-24 15:29:33.000000 energyplus_launch-3.7.2/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 15:29:33.000000 energyplus_launch-3.7.2/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 15:29:33.000000 energyplus_launch-3.7.2/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:33.274385 energyplus_launch-3.7.2/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:33.274385 energyplus_launch-3.7.2/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78212 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/interface/widget_group_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:33.274385 energyplus_launch-3.7.2/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:33.274385 energyplus_launch-3.7.2/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:33.274385 energyplus_launch-3.7.2/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 15:29:33.278385 energyplus_launch-3.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-24 15:29:19.000000 energyplus_launch-3.7.2/setup.py
```

### Comparing `energyplus_launch-3.7.1/LICENSE` & `energyplus_launch-3.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/PKG-INFO` & `energyplus_launch-3.7.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.7.1
+Version: 3.7.2
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
-Description: # EnergyPlus Launch
-        
-        [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
-        
-        Cross platform replacement for EP-Launch for EnergyPlus, written in Python using the `tkinter` graphics library.
-        
-        ## Documentation
-        
-        [![Documentation](https://img.shields.io/readthedocs/ep-launch?label=Docs&logo=read%20the%20docs&style=for-the-badge)](https://ep-launch.readthedocs.io/en/latest/?badge=latest)
-        
-        The project is documented (currently very sparsely) using Sphinx, and automatically generated in [html](https://ep-launch.readthedocs.io/en/) by ReadTheDocs.
-        
-        ## Testing
-        
-        [![PEP8 Enforcement](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/flake8.yml?label=Flake8&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/flake8.yml)
-        [![Unit Tests](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/unit_tests.yml?label=Unit%20Tests&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/unit_tests.yml)
-        [![Coverage Status](https://img.shields.io/coveralls/github/NREL/EP-Launch?label=Coverage&logo=coveralls&style=for-the-badge)](https://coveralls.io/github/NREL/EP-Launch?branch=main)
-        
-        The project is tested using standard Python unit testing practices.
-        Each commit is automatically tested with Github Actions on Windows, Mac, Ubuntu 20.04 and Ubuntu 22.04.
-        The code coverage across platforms is collected on Coveralls.
-        
-        ## Releases
-        
-        [![Releases](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/pypi.yml?label=Releases&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/pypi.yml)
-        
-        When a tag is created in the GitHub Repo, Github Actions builds a Python wheel and uploads it to PyPi: https://pypi.org/project/ep-launch/.
-        The packages can be downloaded using standard `pip install energyplus-launch` commands.
-        Once Pip installed, desktop shortcuts and launchers can be configured using the `energyplus-launch-configure` command from the same Python environment.
-        
-        ## Development
-        
-        Basic development dependencies are installed with `pip install -r requirements.txt`.
-        This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
-        The application can be run by executing the module as `python -m eplaunch` file.
-        To run the unit test suite, simply execute `nosetests`.
-        Unit test results will appear in the console, and coverage results will be in a `cover` directory.
-        
 Keywords: energyplus_launch,ep_launch,EnergyPlus,eplus,Energy+,Building Simulation,Whole Building Energy Simulation,Heat Transfer,HVAC,Modeling
 Platform: Linux (Tested on Ubuntu)
 Platform: MacOSX
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# EnergyPlus Launch
+
+[![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
+
+Cross platform replacement for EP-Launch for EnergyPlus, written in Python using the `tkinter` graphics library.
+
+## Documentation
+
+[![Documentation](https://img.shields.io/readthedocs/ep-launch?label=Docs&logo=read%20the%20docs&style=for-the-badge)](https://ep-launch.readthedocs.io/en/latest/?badge=latest)
+
+The project is documented (currently very sparsely) using Sphinx, and automatically generated in [html](https://ep-launch.readthedocs.io/en/) by ReadTheDocs.
+
+## Testing
+
+[![PEP8 Enforcement](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/flake8.yml?label=Flake8&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/flake8.yml)
+[![Unit Tests](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/unit_tests.yml?label=Unit%20Tests&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/unit_tests.yml)
+[![Coverage Status](https://img.shields.io/coveralls/github/NREL/EP-Launch?label=Coverage&logo=coveralls&style=for-the-badge)](https://coveralls.io/github/NREL/EP-Launch?branch=main)
+
+The project is tested using standard Python unit testing practices.
+Each commit is automatically tested with Github Actions on Windows, Mac, Ubuntu 20.04 and Ubuntu 22.04.
+The code coverage across platforms is collected on Coveralls.
+
+## Releases
+
+[![Releases](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/pypi.yml?label=Releases&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/pypi.yml)
+
+When a tag is created in the GitHub Repo, Github Actions builds a Python wheel and uploads it to PyPi: https://pypi.org/project/ep-launch/.
+The packages can be downloaded using standard `pip install energyplus-launch` commands.
+Once Pip installed, desktop shortcuts and launchers can be configured using the `energyplus-launch-configure` command from the same Python environment.
+
+## Development
+
+Basic development dependencies are installed with `pip install -r requirements.txt`.
+This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
+The application can be run by executing the module as `python -m eplaunch` file.
+To run the unit test suite, simply execute `nosetests`.
+Unit test results will appear in the console, and coverage results will be in a `cover` directory.
+
+
```

### Comparing `energyplus_launch-3.7.1/README.md` & `energyplus_launch-3.7.2/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.7.2/energyplus_launch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.7.1
+Version: 3.7.2
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
-Description: # EnergyPlus Launch
-        
-        [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
-        
-        Cross platform replacement for EP-Launch for EnergyPlus, written in Python using the `tkinter` graphics library.
-        
-        ## Documentation
-        
-        [![Documentation](https://img.shields.io/readthedocs/ep-launch?label=Docs&logo=read%20the%20docs&style=for-the-badge)](https://ep-launch.readthedocs.io/en/latest/?badge=latest)
-        
-        The project is documented (currently very sparsely) using Sphinx, and automatically generated in [html](https://ep-launch.readthedocs.io/en/) by ReadTheDocs.
-        
-        ## Testing
-        
-        [![PEP8 Enforcement](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/flake8.yml?label=Flake8&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/flake8.yml)
-        [![Unit Tests](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/unit_tests.yml?label=Unit%20Tests&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/unit_tests.yml)
-        [![Coverage Status](https://img.shields.io/coveralls/github/NREL/EP-Launch?label=Coverage&logo=coveralls&style=for-the-badge)](https://coveralls.io/github/NREL/EP-Launch?branch=main)
-        
-        The project is tested using standard Python unit testing practices.
-        Each commit is automatically tested with Github Actions on Windows, Mac, Ubuntu 20.04 and Ubuntu 22.04.
-        The code coverage across platforms is collected on Coveralls.
-        
-        ## Releases
-        
-        [![Releases](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/pypi.yml?label=Releases&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/pypi.yml)
-        
-        When a tag is created in the GitHub Repo, Github Actions builds a Python wheel and uploads it to PyPi: https://pypi.org/project/ep-launch/.
-        The packages can be downloaded using standard `pip install energyplus-launch` commands.
-        Once Pip installed, desktop shortcuts and launchers can be configured using the `energyplus-launch-configure` command from the same Python environment.
-        
-        ## Development
-        
-        Basic development dependencies are installed with `pip install -r requirements.txt`.
-        This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
-        The application can be run by executing the module as `python -m eplaunch` file.
-        To run the unit test suite, simply execute `nosetests`.
-        Unit test results will appear in the console, and coverage results will be in a `cover` directory.
-        
 Keywords: energyplus_launch,ep_launch,EnergyPlus,eplus,Energy+,Building Simulation,Whole Building Energy Simulation,Heat Transfer,HVAC,Modeling
 Platform: Linux (Tested on Ubuntu)
 Platform: MacOSX
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# EnergyPlus Launch
+
+[![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
+
+Cross platform replacement for EP-Launch for EnergyPlus, written in Python using the `tkinter` graphics library.
+
+## Documentation
+
+[![Documentation](https://img.shields.io/readthedocs/ep-launch?label=Docs&logo=read%20the%20docs&style=for-the-badge)](https://ep-launch.readthedocs.io/en/latest/?badge=latest)
+
+The project is documented (currently very sparsely) using Sphinx, and automatically generated in [html](https://ep-launch.readthedocs.io/en/) by ReadTheDocs.
+
+## Testing
+
+[![PEP8 Enforcement](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/flake8.yml?label=Flake8&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/flake8.yml)
+[![Unit Tests](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/unit_tests.yml?label=Unit%20Tests&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/unit_tests.yml)
+[![Coverage Status](https://img.shields.io/coveralls/github/NREL/EP-Launch?label=Coverage&logo=coveralls&style=for-the-badge)](https://coveralls.io/github/NREL/EP-Launch?branch=main)
+
+The project is tested using standard Python unit testing practices.
+Each commit is automatically tested with Github Actions on Windows, Mac, Ubuntu 20.04 and Ubuntu 22.04.
+The code coverage across platforms is collected on Coveralls.
+
+## Releases
+
+[![Releases](https://img.shields.io/github/actions/workflow/status/NREL/EP-Launch/pypi.yml?label=Releases&logo=github&style=for-the-badge)](https://github.com/NREL/EP-Launch/actions/workflows/pypi.yml)
+
+When a tag is created in the GitHub Repo, Github Actions builds a Python wheel and uploads it to PyPi: https://pypi.org/project/ep-launch/.
+The packages can be downloaded using standard `pip install energyplus-launch` commands.
+Once Pip installed, desktop shortcuts and launchers can be configured using the `energyplus-launch-configure` command from the same Python environment.
+
+## Development
+
+Basic development dependencies are installed with `pip install -r requirements.txt`.
+This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
+The application can be run by executing the module as `python -m eplaunch` file.
+To run the unit test suite, simply execute `nosetests`.
+Unit test results will appear in the console, and coverage results will be in a `cover` directory.
+
+
```

### Comparing `energyplus_launch-3.7.1/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.7.2/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/__init__.py` & `energyplus_launch-3.7.2/eplaunch/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/config.py` & `energyplus_launch-3.7.2/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.7.2/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.7.2/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.7.2/eplaunch/interface/dialog_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.7.2/eplaunch/interface/dialog_weather.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.7.2/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/frame_main.py` & `energyplus_launch-3.7.2/eplaunch/interface/frame_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
         # If we really needed to skip some, we could do a small timer that
         # won't let two callbacks happen within 0.5s of each other or something.
         # For now that's not necessary, but could be in the future.
         # As of right now, the only reason we need this is to try to refresh
         # the stale attribute, which should be accomplished with just the call here.
         # It's possible we also need to check the _event.widget to make sure we are only
         # calling this when the main window is focused.
-        self._update_file_list()
+        pass  # self._update_file_list()
 
     @staticmethod
     def _list_keyboard_shortcuts() -> List[Tuple[str, str]]:
         # Mimic the keyboard shortcuts in the function above
         # It helps the dialog text look nice if you make sure the widths are uniform
         return [
             ("Control + F5", "Update File List"),
```

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.7.2/eplaunch/interface/widget_dir_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.7.2/eplaunch/interface/widget_file_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,50 +95,46 @@
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure('all', weight=1)
         scrollbar = Scrollbar(self, orient=VERTICAL, command=self.tree.yview)
         self.tree.configure(yscrollcommand=scrollbar.set)
         scrollbar.grid(row=0, column=1, sticky=NS)
 
 
-def printer(selection: List[str]) -> None:
-    print(selection)
-
-
-counter = 0
-
-
-def set_columns():
-    global counter
-    counter += 1
-    if counter == 1:
-        file_listing.tree.set_new_columns(['hi', 'world'])
-    elif counter == 2:
-        file_listing.tree.set_new_columns(['foo'])
-    elif counter == 3:
-        file_listing.tree.set_new_columns(['hello', 'world', 'bar'])
-    elif counter == 4:
-        file_listing.tree.set_new_columns()
-    elif counter == 5:
-        file_listing.tree.set_new_columns(['edwin', 'lee'])
-
-
 if __name__ == "__main__":
     from tkinter import Button, Tk
 
     root = Tk()
     root.title('File Listing Widget Demo')
 
+    def printer(selection: List[str]) -> None:
+        print(selection)
+
+    def set_columns():
+        global counter
+        counter += 1
+        if counter == 1:
+            file_listing.tree.set_new_columns(['hi', 'world'])
+        elif counter == 2:
+            file_listing.tree.set_new_columns(['foo'])
+        elif counter == 3:
+            file_listing.tree.set_new_columns(['hello', 'world', 'bar'])
+        elif counter == 4:
+            file_listing.tree.set_new_columns()
+        elif counter == 5:
+            file_listing.tree.set_new_columns(['edwin', 'lee'])
+
+    counter = 0
     file_listing = FileListScrollableFrame(root, printer)
     files = []
     for n in range(1, 100):
         rand = randint(1, 10)
         files.append((
             f"FileName{n}.png",
             "true" if rand > 5 else "",
             "PNG Image File",
             rand ** 2
         ))
     file_listing.tree.set_files(files)
     file_listing.pack(side=TOP, expand=True, fill=BOTH)
     file_listing.tree.try_to_reselect(['FileName1.png', 'FileName3.png'])
-    Button(text="add columns", command=set_columns).pack(side=TOP, fill='x')
+    Button(text="Change columns", command=set_columns).pack(side=TOP, fill='x')
     root.mainloop()
```

### Comparing `energyplus_launch-3.7.1/eplaunch/interface/widget_group_list.py` & `energyplus_launch-3.7.2/eplaunch/interface/widget_group_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/utilities/cache.py` & `energyplus_launch-3.7.2/eplaunch/utilities/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,18 @@
 
         :param workflow_name: The name of the workflow to alter, as given by the workflow's name() method
         :param file_name: The file name of the file to alter
         :param config_data: A map of data to write to this config section
         :return: None
         """
         self._print(f"About to add a config attribute for workflow {workflow_name}; file {file_name}")
-        if not self.ok_to_continue():
-            pass  # somehow return an error...?
+        if not self.ok_to_continue():  # pragma: no cover
+            # I'm not sure if we should communicate this or not.
+            # For now let's print to the term, so that we might catch it for debugging
+            print("There was a problem adding a config to a cache file, something blocked for too long maybe?")
         cache_files_currently_updating_or_writing.append(self.file_path)
         self._print("Cache file locked")
         self.read()
         self._add_file_attribute(workflow_name, file_name, self.ParametersKey, config_data, False)
         self.write()
         cache_files_currently_updating_or_writing.remove(self.file_path)
         self._print("Cache file UN-locked")
@@ -163,16 +165,18 @@
         :param workflow_name: The name of the workflow to alter, as given by the workflow's name() method
         :param file_name: The file name of the file to alter
         :param column_data: A map of data to write to this result section, the keys are expected to be defined by
                             the workflow itself as given by the get_interface_columns() method
         :return: None
         """
         self._print(f"About to add a result attribute for workflow {workflow_name}; file {file_name}")
-        if not self.ok_to_continue():
-            pass  # somehow return an error...?
+        if not self.ok_to_continue():  # pragma: no cover
+            # I'm not sure if we should communicate this or not.
+            # For now let's print to the term, so that we might catch it for debugging
+            print("There was a problem adding a config to a cache file, something blocked for too long maybe?")
         cache_files_currently_updating_or_writing.append(self.file_path)
         self._print("Cache file locked")
         self.read()
         self._add_file_attribute(workflow_name, file_name, self.ResultsKey, column_data, True)
         self.write()
         cache_files_currently_updating_or_writing.remove(self.file_path)
         self._print("Cache file UN-locked")
```

### Comparing `energyplus_launch-3.7.1/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.7.2/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/utilities/version.py` & `energyplus_launch-3.7.2/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/workflows/base.py` & `energyplus_launch-3.7.2/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.7.2/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.7.2/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.7.2/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/workflows/manager.py` & `energyplus_launch-3.7.2/eplaunch/workflows/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,23 @@
                     for ep_folder in eplus_folder_matches:  # pragma: no cover, would have to install in system folders
                         ep_workflow_dir = ep_folder / 'workflows'
                         if ep_workflow_dir.exists():
                             self.auto_found_workflow_dirs.append(ep_workflow_dir)
             except PermissionError:  # pragma: no cover -- this could be quite hard to reproduce :)
                 continue  # just skip it, it could be like an empty DVD drive
 
-    def instantiate_all_workflows(self, disable_builtins=False, extra_workflow_dir: Optional[Path] = None) -> None:
+    def instantiate_all_workflows(self, disable_builtins=False, extra_workflow_dir: Optional[Path] = None,
+                                  skip_ep_search: bool = False) -> None:
         this_file_directory_path = Path(__file__).parent.resolve()
         this_project_root_dir = this_file_directory_path.parent
         built_in_workflow_dir = this_project_root_dir / 'workflows' / 'default'
-        all_workflow_directories = self.workflow_directories
+        if skip_ep_search:
+            all_workflow_directories = []
+        else:
+            all_workflow_directories = self.workflow_directories
         if disable_builtins:
             # don't add built-in default workflows
             pass
         elif built_in_workflow_dir not in all_workflow_directories and built_in_workflow_dir.exists():
             # add the built-in directory if it exists
             all_workflow_directories.append(built_in_workflow_dir)
         if extra_workflow_dir is not None:
```

### Comparing `energyplus_launch-3.7.1/eplaunch/workflows/workflow.py` & `energyplus_launch-3.7.2/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.7.2/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.7.2/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.7.1/setup.py` & `energyplus_launch-3.7.2/setup.py`

 * *Files identical despite different names*

