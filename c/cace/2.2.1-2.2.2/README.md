# Comparing `tmp/cace-2.2.1.tar.gz` & `tmp/cace-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cace-2.2.1.tar", last modified: Sat Apr 20 13:19:08 2024, max compression
+gzip compressed data, was "cace-2.2.2.tar", last modified: Wed Apr 24 14:18:40 2024, max compression
```

## Comparing `cace-2.2.1.tar` & `cace-2.2.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.933084 cace-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.917084 cace-2.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.921084 cace-2.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-20 13:18:41.000000 cace-2.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-20 13:18:41.000000 cace-2.2.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-20 13:18:41.000000 cace-2.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-20 13:18:41.000000 cace-2.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-20 13:18:41.000000 cace-2.2.1/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-20 13:18:41.000000 cace-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-20 13:18:41.000000 cace-2.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-20 13:19:08.933084 cace-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-20 13:18:41.000000 cace-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.921084 cace-2.2.1/cace/
--rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-04-20 13:18:41.000000 cace-2.2.1/cace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-20 13:18:41.000000 cace-2.2.1/cace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-20 13:18:41.000000 cace-2.2.1/cace/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5906 2024-04-20 13:18:41.000000 cace-2.2.1/cace/cace_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45110 2024-04-20 13:18:41.000000 cace-2.2.1/cace/cace_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.929084 cace-2.2.1/cace/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_calculate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_collate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_gensim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_launch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_makeplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_measure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_regenerate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_simulate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_unused.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    55674 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/cace_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7231 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/electrical_parameter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/layout_estimate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/netlist_precheck.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2451 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/physical_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/safe_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14650 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/simulation_job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19262 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/simulation_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-04-20 13:18:41.000000 cace-2.2.1/cace/common/spiceunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.929084 cace-2.2.1/cace/gui/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/consoletext.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/editparam.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/failreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/helpwindow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/rowwidget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/simhints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/textreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/tksimpledialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-20 13:18:41.000000 cace-2.2.1/cace/gui/tooltip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.933084 cace-2.2.1/cace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-20 13:19:08.000000 cace-2.2.1/cace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-20 13:19:08.000000 cace-2.2.1/cace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:19:08.000000 cace-2.2.1/cace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-20 13:19:08.000000 cace-2.2.1/cace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 13:19:08.000000 cace-2.2.1/cace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-20 13:19:08.000000 cace-2.2.1/cace.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.929084 cace-2.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-20 13:18:41.000000 cace-2.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-20 13:18:41.000000 cace-2.2.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.929084 cace-2.2.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.929084 cace-2.2.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/_static/cace_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/characterization.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.929084 cace-2.2.1/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/dev/codebase.md
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/dev/coding_style.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/dev/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.933084 cace-2.2.1/docs/source/formats/
--rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/formats/format_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/formats/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/formats/schematic_description.md
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.933084 cace-2.2.1/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/usage/cace_cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/usage/cace_gui.md
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/usage/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-20 13:18:41.000000 cace-2.2.1/docs/source/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-20 13:18:41.000000 cace-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 13:18:41.000000 cace-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 13:18:41.000000 cace-2.2.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-20 13:18:41.000000 cace-2.2.1/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:19:08.933084 cace-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:19:08.933084 cace-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-20 13:18:41.000000 cace-2.2.1/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 13:18:41.000000 cace-2.2.1/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.331260 cace-2.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.335260 cace-2.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-24 14:18:17.000000 cace-2.2.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 14:18:17.000000 cace-2.2.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 14:18:17.000000 cace-2.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 14:18:17.000000 cace-2.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-24 14:18:17.000000 cace-2.2.2/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 14:18:17.000000 cace-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-24 14:18:17.000000 cace-2.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-24 14:18:40.347260 cace-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-24 14:18:17.000000 cace-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.335260 cace-2.2.2/cace/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-04-24 14:18:17.000000 cace-2.2.2/cace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 14:18:17.000000 cace-2.2.2/cace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 14:18:17.000000 cace-2.2.2/cace/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5906 2024-04-24 14:18:17.000000 cace-2.2.2/cace/cace_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45110 2024-04-24 14:18:17.000000 cace-2.2.2/cace/cace_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.339260 cace-2.2.2/cace/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_calculate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_collate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_gensim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_launch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_makeplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_measure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_regenerate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_simulate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_unused.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55674 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/cace_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7231 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/electrical_parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/layout_estimate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/netlist_precheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2451 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/physical_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/safe_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14650 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/simulation_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19262 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/simulation_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-04-24 14:18:17.000000 cace-2.2.2/cace/common/spiceunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.343260 cace-2.2.2/cace/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/consoletext.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/editparam.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/failreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/helpwindow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/rowwidget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/simhints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/textreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/tksimpledialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-24 14:18:17.000000 cace-2.2.2/cace/gui/tooltip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/cace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 14:18:40.000000 cace-2.2.2/cace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.343260 cace-2.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 14:18:17.000000 cace-2.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 14:18:17.000000 cace-2.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.343260 cace-2.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.343260 cace-2.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/_static/cace_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/characterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/dev/codebase.md
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/dev/coding_style.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/dev/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/docs/source/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/formats/format_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/formats/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/formats/schematic_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/usage/cace_cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/usage/cace_gui.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/usage/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 14:18:17.000000 cace-2.2.2/docs/source/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-24 14:18:17.000000 cace-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 14:18:17.000000 cace-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 14:18:17.000000 cace-2.2.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 14:18:17.000000 cace-2.2.2/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:18:40.347260 cace-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:18:40.347260 cace-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 14:18:17.000000 cace-2.2.2/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 14:18:17.000000 cace-2.2.2/tests/test1.py
```

### Comparing `cace-2.2.1/.github/workflows/ci.yaml` & `cace-2.2.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/.github/workflows/pypi.yaml` & `cace-2.2.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/.readthedocs.yaml` & `cace-2.2.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/Changelog.md` & `cace-2.2.2/Changelog.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/LICENSE` & `cace-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/Makefile` & `cace-2.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/PKG-INFO` & `cace-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.1
+Version: 2.2.2
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.1 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.2 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.2.1/README.md` & `cace-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/__init__.py` & `cace-2.2.2/cace/__init__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/__main__.py` & `cace-2.2.2/cace/__main__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/__version__.py` & `cace-2.2.2/cace/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = '2.2.1'
+__version__ = '2.2.2'
 
 if __name__ == '__main__':
     print(__version__, end='')
```

### Comparing `cace-2.2.1/cace/cace_cli.py` & `cace-2.2.2/cace/cace_cli.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/cace_gui.py` & `cace-2.2.2/cace/cace_gui.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_calculate.py` & `cace-2.2.2/cace/common/cace_calculate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_collate.py` & `cace-2.2.2/cace/common/cace_collate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_compat.py` & `cace-2.2.2/cace/common/cace_compat.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_evaluate.py` & `cace-2.2.2/cace/common/cace_evaluate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_gensim.py` & `cace-2.2.2/cace/common/cace_gensim.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_launch.py` & `cace-2.2.2/cace/common/cace_launch.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_makeplot.py` & `cace-2.2.2/cace/common/cace_makeplot.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_measure.py` & `cace-2.2.2/cace/common/cace_measure.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_read.py` & `cace-2.2.2/cace/common/cace_read.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_regenerate.py` & `cace-2.2.2/cace/common/cace_regenerate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_simulate.py` & `cace-2.2.2/cace/common/cace_simulate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_unused.txt` & `cace-2.2.2/cace/common/cace_unused.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/cace_write.py` & `cace-2.2.2/cace/common/cace_write.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/electrical_parameter.py` & `cace-2.2.2/cace/common/electrical_parameter.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/layout_estimate.py` & `cace-2.2.2/cace/common/layout_estimate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/netlist_precheck.py` & `cace-2.2.2/cace/common/netlist_precheck.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/physical_parameter.py` & `cace-2.2.2/cace/common/physical_parameter.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/safe_eval.py` & `cace-2.2.2/cace/common/safe_eval.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/simulation_job.py` & `cace-2.2.2/cace/common/simulation_job.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/simulation_manager.py` & `cace-2.2.2/cace/common/simulation_manager.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/common/spiceunits.py` & `cace-2.2.2/cace/common/spiceunits.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/consoletext.py` & `cace-2.2.2/cace/gui/consoletext.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/editparam.py` & `cace-2.2.2/cace/gui/editparam.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/failreport.py` & `cace-2.2.2/cace/gui/failreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/helpwindow.py` & `cace-2.2.2/cace/gui/helpwindow.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/rowwidget.py` & `cace-2.2.2/cace/gui/rowwidget.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/settings.py` & `cace-2.2.2/cace/gui/settings.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/simhints.py` & `cace-2.2.2/cace/gui/simhints.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/style.py` & `cace-2.2.2/cace/gui/style.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/textreport.py` & `cace-2.2.2/cace/gui/textreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/tksimpledialog.py` & `cace-2.2.2/cace/gui/tksimpledialog.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace/gui/tooltip.py` & `cace-2.2.2/cace/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/cace.egg-info/PKG-INFO` & `cace-2.2.2/cace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.1
+Version: 2.2.2
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.1 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.2 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.2.1/cace.egg-info/SOURCES.txt` & `cace-2.2.2/cace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/Makefile` & `cace-2.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/make.bat` & `cace-2.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/_static/cace_screenshot.png` & `cace-2.2.2/docs/source/_static/cace_screenshot.png`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/characterization.md` & `cace-2.2.2/docs/source/characterization.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/conf.py` & `cace-2.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/formats/format_description.md` & `cace-2.2.2/docs/source/formats/format_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/formats/schematic_description.md` & `cace-2.2.2/docs/source/formats/schematic_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/index.md` & `cace-2.2.2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/usage/cace_cli.md` & `cace-2.2.2/docs/source/usage/cace_cli.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/usage/cace_gui.md` & `cace-2.2.2/docs/source/usage/cace_gui.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/docs/source/usage/getting_started.md` & `cace-2.2.2/docs/source/usage/getting_started.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.1/pyproject.toml` & `cace-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 Homepage = "https://github.com/efabless/cace"
 Issues = "https://github.com/efabless/cace/issues"
 
 [build-system]
-requires = ["setuptools>=64", "setuptools_scm>=8"]
+requires = ["setuptools>=64", "setuptools_scm>=7"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["cace*"]
 
 [project.scripts]
 cace = "cace.cace_cli:cli"
```

