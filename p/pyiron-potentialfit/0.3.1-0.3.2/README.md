# Comparing `tmp/pyiron_potentialfit-0.3.1.tar.gz` & `tmp/pyiron_potentialfit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_potentialfit-0.3.1.tar", last modified: Tue Apr 23 19:21:22 2024, max compression
+gzip compressed data, was "pyiron_potentialfit-0.3.2.tar", last modified: Wed Apr 24 11:02:15 2024, max compression
```

## Comparing `pyiron_potentialfit-0.3.1.tar` & `pyiron_potentialfit-0.3.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.415804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/atomicrex_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/fit_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/function_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/general_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    45845 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/potential_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    37753 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/structure_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py
--rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/trainingcontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/meamfit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/meamfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/meamfit/meamfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/ml/potentialfit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/cfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/masters.py
--rw-r--r--   0 runner    (1001) docker     (127)    30245 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/mlip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/mlipdescriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.419804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16918 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/pacemaker/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22529 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/storageclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    16398 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/projectflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    30238 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 19:21:22.000000 pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 19:21:22.423804 pyiron_potentialfit-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-23 19:21:21.000000 pyiron_potentialfit-0.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-23 19:21:17.000000 pyiron_potentialfit-0.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.098661 pyiron_potentialfit-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 11:02:15.098661 pyiron_potentialfit-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.090661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 11:02:15.102661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.094661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/atomicrex_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/fit_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53733 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/function_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/general_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45845 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/potential_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37753 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/structure_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.094661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.094661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomistics/job/trainingcontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.094661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/meamfit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/meamfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/meamfit/meamfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.094661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/ml/potentialfit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.098661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/cfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/masters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30245 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/mlip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/mlipdescriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.098661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16918 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/pacemaker/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.098661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22529 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/runner/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/runner/storageclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.098661 pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15884 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16398 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/projectflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30238 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:02:15.098661 pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 11:02:15.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-24 11:02:15.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:02:15.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 11:02:15.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 11:02:15.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 11:02:15.000000 pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 11:02:15.098661 pyiron_potentialfit-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-24 11:02:14.000000 pyiron_potentialfit-0.3.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-24 11:02:12.000000 pyiron_potentialfit-0.3.2/versioneer.py
```

### Comparing `pyiron_potentialfit-0.3.1/LICENSE` & `pyiron_potentialfit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/PKG-INFO` & `pyiron_potentialfit-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_potentialfit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_potentialfit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyiron_potentialfit-0.3.1/README.md` & `pyiron_potentialfit-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/__init__.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/base.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/fit_properties.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/fit_properties.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/function_factory.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/function_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/general_input.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/general_input.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/interactive.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/parameter_constraints.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/potential_factory.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/potential_factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/structure_list.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/structure_list.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomicrex/utility_functions.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomicrex/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomistics/job/structurelistmasterinteractive.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/atomistics/job/trainingcontainer.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/atomistics/job/trainingcontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/meamfit/meamfit.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/meamfit/meamfit.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/ml/potentialfit.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/ml/potentialfit.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/cfgs.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/cfgs.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/lammps.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/masters.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/masters.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/mlip.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/mlip.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/mlipdescriptors.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/mlipdescriptors.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/parser.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/mlip/potential.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/mlip/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/pacemaker/job.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/pacemaker/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/job.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/runner/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/storageclasses.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/runner/storageclasses.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/runner/utils.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/runner/utils.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/calculations.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/calculations.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/learn.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/learn.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/projectflow.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/projectflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/structures.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/structures.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit/spgfit/util.py` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit/spgfit/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/PKG-INFO` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_potentialfit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Repository for user-generated plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_potentialfit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: huber@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyiron_potentialfit-0.3.1/pyiron_potentialfit.egg-info/SOURCES.txt` & `pyiron_potentialfit-0.3.2/pyiron_potentialfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/setup.py` & `pyiron_potentialfit-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyiron_potentialfit-0.3.1/versioneer.py` & `pyiron_potentialfit-0.3.2/versioneer.py`

 * *Files identical despite different names*

