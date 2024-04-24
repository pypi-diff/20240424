# Comparing `tmp/peracotta-2.3.1.tar.gz` & `tmp/peracotta-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peracotta-2.3.1.tar", last modified: Tue Apr 23 12:33:06 2024, max compression
+gzip compressed data, was "peracotta-2.3.2.tar", last modified: Wed Apr 24 20:59:29 2024, max compression
```

## Comparing `peracotta-2.3.1.tar` & `peracotta-2.3.2.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.634646 peracotta-2.3.1/
--rw-r--r--   0 basilef   (1000) users      (100)     1066 2024-02-28 15:11:29.000000 peracotta-2.3.1/LICENSE
--rw-r--r--   0 basilef   (1000) users      (100)     9829 2024-04-23 12:33:06.634646 peracotta-2.3.1/PKG-INFO
--rw-r--r--   0 basilef   (1000) users      (100)     7847 2024-02-28 15:11:32.000000 peracotta-2.3.1/README.md
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.634646 peracotta-2.3.1/peracotta.egg-info/
--rw-r--r--   0 basilef   (1000) users      (100)     9829 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) users      (100)     1614 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) users      (100)        1 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) users      (100)       95 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) users      (100)      174 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) users      (100)       10 2024-04-23 12:33:06.000000 peracotta-2.3.1/peracotta.egg-info/top_level.txt
--rw-r--r--   0 basilef   (1000) users      (100)     1071 2024-03-15 15:08:55.000000 peracotta-2.3.1/pyproject.toml
--rw-r--r--   0 basilef   (1000) users      (100)       38 2024-04-23 12:33:06.634646 peracotta-2.3.1/setup.cfg
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.631646 peracotta-2.3.1/src/
--rw-r--r--   0 basilef   (1000) users      (100)     4432 2024-03-27 15:00:33.000000 peracotta-2.3.1/src/__init__.py
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.632646 peracotta-2.3.1/src/assets/
--rw-r--r--   0 basilef   (1000) users      (100)     8050 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/Installing.gif
--rw-r--r--   0 basilef   (1000) users      (100)     2651 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/error.ui
--rw-r--r--   0 basilef   (1000) users      (100)    13414 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/interface.ui
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.632646 peracotta-2.3.1/src/assets/themes/
--rw-r--r--   0 basilef   (1000) users      (100)     5952 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/themes/Dark.css
--rw-r--r--   0 basilef   (1000) users      (100)     6478 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/themes/WEEE Open.css
--rw-r--r--   0 basilef   (1000) users      (100)       33 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/themes/default.css
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.632646 peracotta-2.3.1/src/assets/toolbox/
--rw-r--r--   0 basilef   (1000) users      (100)     9745 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/case.png
--rw-r--r--   0 basilef   (1000) users      (100)    14546 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/cpu.png
--rw-r--r--   0 basilef   (1000) users      (100)    16694 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/gpu.png
--rw-r--r--   0 basilef   (1000) users      (100)    20523 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/hdd.png
--rw-r--r--   0 basilef   (1000) users      (100)    13943 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/keyboard.png
--rw-r--r--   0 basilef   (1000) users      (100)     6966 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/monitor.png
--rw-r--r--   0 basilef   (1000) users      (100)    17156 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/motherboard.png
--rw-r--r--   0 basilef   (1000) users      (100)     9567 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/mouse.png
--rw-r--r--   0 basilef   (1000) users      (100)    10348 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/odd.png
--rw-r--r--   0 basilef   (1000) users      (100)    28645 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/psu.png
--rw-r--r--   0 basilef   (1000) users      (100)     8639 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/ram.png
--rw-r--r--   0 basilef   (1000) users      (100)    10601 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/ssd.png
--rw-r--r--   0 basilef   (1000) users      (100)    11950 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/toolbox/wifi-card.png
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.633646 peracotta-2.3.1/src/assets/ui/
--rw-r--r--   0 basilef   (1000) users      (100)     1444 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/light_down_arrow.png
--rw-r--r--   0 basilef   (1000) users      (100)     6790 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/light_split_handle.png
--rw-r--r--   0 basilef   (1000) users      (100)    28552 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/pear_emoji.png
--rw-r--r--   0 basilef   (1000) users      (100)    14674 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/radio_ckd.png
--rw-r--r--   0 basilef   (1000) users      (100)    12489 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/ui/radio_unckd.png
--rw-r--r--   0 basilef   (1000) users      (100)     5226 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/assets/uploadTaralloDialog.ui
--rw-r--r--   0 basilef   (1000) users      (100)    16567 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/commons.py
--rw-r--r--   0 basilef   (1000) users      (100)     2361 2024-03-27 15:00:33.000000 peracotta-2.3.1/src/config.py
--rw-r--r--   0 basilef   (1000) users      (100)      307 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/config.toml
--rw-r--r--   0 basilef   (1000) users      (100)     1360 2024-04-23 12:31:03.000000 peracotta-2.3.1/src/constants.py
--rw-r--r--   0 basilef   (1000) users      (100)    43091 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/features.json
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.633646 peracotta-2.3.1/src/gui/
--rw-r--r--   0 basilef   (1000) users      (100)     3273 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/gui/PeraThread.py
--rw-r--r--   0 basilef   (1000) users      (100)    26699 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/gui/Toolbox.py
--rw-r--r--   0 basilef   (1000) users      (100)      102 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/gui/__init__.py
--rw-r--r--   0 basilef   (1000) users      (100)     1108 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/gui/exception_handler.py
--rw-r--r--   0 basilef   (1000) users      (100)       48 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/gui/exceptions.py
--rw-r--r--   0 basilef   (1000) users      (100)    20818 2024-04-23 12:16:45.000000 peracotta-2.3.1/src/gui/gui.py
--rw-r--r--   0 basilef   (1000) users      (100)     2989 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/gui/prettyprinter.py
--rw-r--r--   0 basilef   (1000) users      (100)     1362 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/gui/widgets.py
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.633646 peracotta-2.3.1/src/parsers/
--rwxr-xr-x   0 basilef   (1000) users      (100)     5274 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_decode_dimms.py
--rw-r--r--   0 basilef   (1000) users      (100)    14087 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_dmidecode.py
--rwxr-xr-x   0 basilef   (1000) users      (100)     4008 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_lscpu.py
--rwxr-xr-x   0 basilef   (1000) users      (100)    10890 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_lspci_and_glxinfo.py
--rwxr-xr-x   0 basilef   (1000) users      (100)    26973 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/read_smartctl.py
--rw-r--r--   0 basilef   (1000) users      (100)     3766 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/parsers/windows_parser.py
--rwxr-xr-x   0 basilef   (1000) users      (100)    12449 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/peracruda.py
--rw-r--r--   0 basilef   (1000) users      (100)      639 2024-03-15 15:10:11.000000 peracotta-2.3.1/src/peralog.py
--rw-r--r--   0 basilef   (1000) users      (100)      337 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/reporter.py
-drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-23 12:33:06.634646 peracotta-2.3.1/src/scripts/
--rwxr-xr-x   0 basilef   (1000) users      (100)     1628 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/scripts/check_dependencies.sh
--rwxr-xr-x   0 basilef   (1000) users      (100)     1718 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/scripts/generate_files.sh
--rw-r--r--   0 basilef   (1000) users      (100)     2694 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/scripts/get_windows_specs.py
--rwxr-xr-x   0 basilef   (1000) users      (100)      172 2024-02-28 15:11:29.000000 peracotta-2.3.1/src/scripts/install_dependencies_all.sh
--rw-r--r--   0 basilef   (1000) users      (100)     3216 2024-03-15 15:08:55.000000 peracotta-2.3.1/src/tarallo.py
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.150149 peracotta-2.3.2/
+-rw-r--r--   0 basilef   (1000) users      (100)     1066 2024-02-28 15:11:29.000000 peracotta-2.3.2/LICENSE
+-rw-r--r--   0 basilef   (1000) users      (100)     9953 2024-04-24 20:59:29.150149 peracotta-2.3.2/PKG-INFO
+-rw-r--r--   0 basilef   (1000) users      (100)     7847 2024-04-24 14:45:45.000000 peracotta-2.3.2/README.md
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.149149 peracotta-2.3.2/peracotta.egg-info/
+-rw-r--r--   0 basilef   (1000) users      (100)     9953 2024-04-24 20:59:29.000000 peracotta-2.3.2/peracotta.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) users      (100)     2176 2024-04-24 20:59:29.000000 peracotta-2.3.2/peracotta.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) users      (100)        1 2024-04-24 20:59:29.000000 peracotta-2.3.2/peracotta.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) users      (100)       95 2024-04-24 20:59:29.000000 peracotta-2.3.2/peracotta.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) users      (100)      131 2024-04-24 20:59:29.000000 peracotta-2.3.2/peracotta.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) users      (100)       10 2024-04-24 20:59:29.000000 peracotta-2.3.2/peracotta.egg-info/top_level.txt
+-rw-r--r--   0 basilef   (1000) users      (100)     1571 2024-04-24 18:36:52.000000 peracotta-2.3.2/pyproject.toml
+-rw-r--r--   0 basilef   (1000) users      (100)       38 2024-04-24 20:59:29.150149 peracotta-2.3.2/setup.cfg
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.135149 peracotta-2.3.2/src/
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.140149 peracotta-2.3.2/src/peracotta/
+-rw-r--r--   0 basilef   (1000) users      (100)     4432 2024-04-24 14:46:05.000000 peracotta-2.3.2/src/peracotta/__init__.py
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.141149 peracotta-2.3.2/src/peracotta/assets/
+-rw-r--r--   0 basilef   (1000) users      (100)     8050 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/Installing.gif
+-rw-r--r--   0 basilef   (1000) users      (100)     2651 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/error.ui
+-rw-r--r--   0 basilef   (1000) users      (100)    13414 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/interface.ui
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.142149 peracotta-2.3.2/src/peracotta/assets/themes/
+-rw-r--r--   0 basilef   (1000) users      (100)     5952 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/assets/themes/Dark.css
+-rw-r--r--   0 basilef   (1000) users      (100)     6478 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/assets/themes/WEEE Open.css
+-rw-r--r--   0 basilef   (1000) users      (100)       33 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/assets/themes/default.css
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.145149 peracotta-2.3.2/src/peracotta/assets/toolbox/
+-rw-r--r--   0 basilef   (1000) users      (100)     9745 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/case.png
+-rw-r--r--   0 basilef   (1000) users      (100)    14546 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/cpu.png
+-rw-r--r--   0 basilef   (1000) users      (100)    16694 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/gpu.png
+-rw-r--r--   0 basilef   (1000) users      (100)    20523 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/hdd.png
+-rw-r--r--   0 basilef   (1000) users      (100)    13943 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/keyboard.png
+-rw-r--r--   0 basilef   (1000) users      (100)     6966 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/monitor.png
+-rw-r--r--   0 basilef   (1000) users      (100)    17156 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/motherboard.png
+-rw-r--r--   0 basilef   (1000) users      (100)     9567 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/mouse.png
+-rw-r--r--   0 basilef   (1000) users      (100)    10348 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/odd.png
+-rw-r--r--   0 basilef   (1000) users      (100)    28645 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/psu.png
+-rw-r--r--   0 basilef   (1000) users      (100)     8639 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/ram.png
+-rw-r--r--   0 basilef   (1000) users      (100)    10601 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/ssd.png
+-rw-r--r--   0 basilef   (1000) users      (100)    11950 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/toolbox/wifi-card.png
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.146149 peracotta-2.3.2/src/peracotta/assets/ui/
+-rw-r--r--   0 basilef   (1000) users      (100)     1444 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/ui/light_down_arrow.png
+-rw-r--r--   0 basilef   (1000) users      (100)     6790 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/ui/light_split_handle.png
+-rw-r--r--   0 basilef   (1000) users      (100)    28552 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/ui/pear_emoji.png
+-rw-r--r--   0 basilef   (1000) users      (100)    14674 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/ui/radio_ckd.png
+-rw-r--r--   0 basilef   (1000) users      (100)    12489 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/ui/radio_unckd.png
+-rw-r--r--   0 basilef   (1000) users      (100)     5226 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/assets/uploadTaralloDialog.ui
+-rw-r--r--   0 basilef   (1000) users      (100)    16567 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/commons.py
+-rw-r--r--   0 basilef   (1000) users      (100)     2361 2024-04-24 14:46:05.000000 peracotta-2.3.2/src/peracotta/config.py
+-rw-r--r--   0 basilef   (1000) users      (100)      307 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/config.toml
+-rw-r--r--   0 basilef   (1000) users      (100)     1566 2024-04-24 20:57:38.000000 peracotta-2.3.2/src/peracotta/constants.py
+-rw-r--r--   0 basilef   (1000) users      (100)    43091 2024-02-28 15:11:29.000000 peracotta-2.3.2/src/peracotta/features.json
+-rw-r--r--   0 basilef   (1000) users      (100)    43091 2024-02-28 15:11:29.000000 peracotta-2.3.2/src/peracotta/features.json.bak
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.147149 peracotta-2.3.2/src/peracotta/gui/
+-rw-r--r--   0 basilef   (1000) users      (100)     3273 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/gui/PeraThread.py
+-rw-r--r--   0 basilef   (1000) users      (100)    26748 2024-04-24 18:55:28.000000 peracotta-2.3.2/src/peracotta/gui/Toolbox.py
+-rw-r--r--   0 basilef   (1000) users      (100)      102 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/gui/__init__.py
+-rw-r--r--   0 basilef   (1000) users      (100)     1108 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/gui/exception_handler.py
+-rw-r--r--   0 basilef   (1000) users      (100)       48 2024-04-24 14:45:26.000000 peracotta-2.3.2/src/peracotta/gui/exceptions.py
+-rw-r--r--   0 basilef   (1000) users      (100)    20818 2024-04-24 14:46:05.000000 peracotta-2.3.2/src/peracotta/gui/gui.py
+-rw-r--r--   0 basilef   (1000) users      (100)     2989 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/gui/prettyprinter.py
+-rw-r--r--   0 basilef   (1000) users      (100)     1386 2024-04-24 18:56:51.000000 peracotta-2.3.2/src/peracotta/gui/widgets.py
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.148149 peracotta-2.3.2/src/peracotta/parsers/
+-rwxr-xr-x   0 basilef   (1000) users      (100)     5274 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/parsers/read_decode_dimms.py
+-rw-r--r--   0 basilef   (1000) users      (100)    14087 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/parsers/read_dmidecode.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)     4008 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/parsers/read_lscpu.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)    10890 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/parsers/read_lspci_and_glxinfo.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)    26973 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/parsers/read_smartctl.py
+-rw-r--r--   0 basilef   (1000) users      (100)     3766 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/parsers/windows_parser.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)    12449 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/peracruda.py
+-rw-r--r--   0 basilef   (1000) users      (100)      639 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/peralog.py
+-rw-r--r--   0 basilef   (1000) users      (100)      337 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/reporter.py
+drwxr-xr-x   0 basilef   (1000) users      (100)        0 2024-04-24 20:59:29.149149 peracotta-2.3.2/src/peracotta/scripts/
+-rwxr-xr-x   0 basilef   (1000) users      (100)     1628 2024-04-24 14:45:45.000000 peracotta-2.3.2/src/peracotta/scripts/check_dependencies.sh
+-rwxr-xr-x   0 basilef   (1000) users      (100)     1718 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/scripts/generate_files.sh
+-rw-r--r--   0 basilef   (1000) users      (100)     2694 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/scripts/get_windows_specs.py
+-rwxr-xr-x   0 basilef   (1000) users      (100)      172 2024-04-24 14:42:28.000000 peracotta-2.3.2/src/peracotta/scripts/install_dependencies_all.sh
+-rw-r--r--   0 basilef   (1000) users      (100)     3240 2024-04-24 18:56:51.000000 peracotta-2.3.2/src/peracotta/tarallo.py
```

### Comparing `peracotta-2.3.1/LICENSE` & `peracotta-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/PKG-INFO` & `peracotta-2.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peracotta
-Version: 2.3.1
+Version: 2.3.2
 License: MIT License
         
         Copyright (c) 2018 WEEE Open
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,33 +20,37 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: colorama==0.4
-Requires-Dist: commonmark==0.9
+Requires-Dist: colorama
+Requires-Dist: commonmark
 Requires-Dist: PyQt5
-Requires-Dist: pytarallo>=2.3
-Requires-Dist: python-dotenv==0.17
-Requires-Dist: requests==2.25
-Requires-Dist: typing-extensions>=3.7.4
-Requires-Dist: urllib3>=1.26
-Requires-Dist: loguru>=0.7
-Requires-Dist: rich>=13.0
-Requires-Dist: requests>=2.25
-Requires-Dist: toml>=0.10
+Requires-Dist: pytarallo
+Requires-Dist: python-dotenv
+Requires-Dist: requests
+Requires-Dist: typing-extensions
+Requires-Dist: urllib3
+Requires-Dist: importlib_resources
+Requires-Dist: loguru
+Requires-Dist: rich
+Requires-Dist: requests
+Requires-Dist: toml
 
 [![Python Tests](https://github.com/WEEE-Open/peracotta/actions/workflows/python-tests.yml/badge.svg)](https://github.com/WEEE-Open/peracotta/actions/workflows/python-tests.yml)
 [![Docker Image CI](https://github.com/WEEE-Open/peracotta/actions/workflows/docker-image.yml/badge.svg)](https://github.com/WEEE-Open/peracotta/actions/workflows/docker-image.yml)
 [![Linting](https://github.com/WEEE-Open/peracotta/actions/workflows/lint.yml/badge.svg)](https://github.com/WEEE-Open/peracotta/actions/workflows/lint.yml)
 
 ![Peracotta](assets/ui/pear_emoji.png)
```

### Comparing `peracotta-2.3.1/README.md` & `peracotta-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/peracotta.egg-info/PKG-INFO` & `peracotta-2.3.2/peracotta.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peracotta
-Version: 2.3.1
+Version: 2.3.2
 License: MIT License
         
         Copyright (c) 2018 WEEE Open
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,33 +20,37 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: colorama==0.4
-Requires-Dist: commonmark==0.9
+Requires-Dist: colorama
+Requires-Dist: commonmark
 Requires-Dist: PyQt5
-Requires-Dist: pytarallo>=2.3
-Requires-Dist: python-dotenv==0.17
-Requires-Dist: requests==2.25
-Requires-Dist: typing-extensions>=3.7.4
-Requires-Dist: urllib3>=1.26
-Requires-Dist: loguru>=0.7
-Requires-Dist: rich>=13.0
-Requires-Dist: requests>=2.25
-Requires-Dist: toml>=0.10
+Requires-Dist: pytarallo
+Requires-Dist: python-dotenv
+Requires-Dist: requests
+Requires-Dist: typing-extensions
+Requires-Dist: urllib3
+Requires-Dist: importlib_resources
+Requires-Dist: loguru
+Requires-Dist: rich
+Requires-Dist: requests
+Requires-Dist: toml
 
 [![Python Tests](https://github.com/WEEE-Open/peracotta/actions/workflows/python-tests.yml/badge.svg)](https://github.com/WEEE-Open/peracotta/actions/workflows/python-tests.yml)
 [![Docker Image CI](https://github.com/WEEE-Open/peracotta/actions/workflows/docker-image.yml/badge.svg)](https://github.com/WEEE-Open/peracotta/actions/workflows/docker-image.yml)
 [![Linting](https://github.com/WEEE-Open/peracotta/actions/workflows/lint.yml/badge.svg)](https://github.com/WEEE-Open/peracotta/actions/workflows/lint.yml)
 
 ![Peracotta](assets/ui/pear_emoji.png)
```

### Comparing `peracotta-2.3.1/pyproject.toml` & `peracotta-2.3.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peracotta"
 dynamic = ["version"]
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
-  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Environment :: X11 Applications :: Qt",
   "License :: OSI Approved :: MIT License",
 ]
 
+# Unless really needed, dependencies in pyproject.toml should be unpinned.
+# For deployments, use the classic pip freeze > requirements.txt
+# Remember to manually move the dependencies that are not needed in the final package to requirements-dev.txt
 dependencies = [
-  "colorama==0.4",
-  "commonmark==0.9",
+  "colorama",
+  "commonmark",
   "PyQt5",
-  "pytarallo>=2.3",
-  "python-dotenv==0.17",
-  "requests==2.25",
-  "typing-extensions>=3.7.4",
-  "urllib3>=1.26",
-  "loguru>=0.7",
-  "rich>=13.0",
-  "requests>=2.25",
-  "toml>=0.10"
+  "pytarallo",
+  "python-dotenv",
+  "requests",
+  "typing-extensions",
+  "urllib3",
+  "importlib_resources",
+  "loguru",
+  "rich",
+  "requests",
+  "toml",
 ]
 
 [project.scripts]
 peracruda = "peracotta:main_cli"
 
 [project.gui-scripts]
 peracotta = "peracotta:main_gui"
 
 [tool.setuptools.package-dir]
-peracotta = "src"
+peracotta = "src/peracotta"
 
 [tool.setuptools.package-data]
 peracotta = ["*"]
 "peracotta.scripts" = ["*"]
 "peracotta.assets" = ["*", "*/*"]
 
 [tool.setuptools.dynamic]
 version = { attr = "peracotta.constants.VERSION" }
 
 [tool.black]
 line-length = 160
+
+[tool.pytest.ini_options]
+pythonpath = ["src", "."]
+markers = ["upload", "gui", "prettyprint", "smartctl"]
+addopts = ["--import-mode=importlib"]
```

### Comparing `peracotta-2.3.1/src/__init__.py` & `peracotta-2.3.2/src/peracotta/__init__.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/Installing.gif` & `peracotta-2.3.2/src/peracotta/assets/Installing.gif`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/error.ui` & `peracotta-2.3.2/src/peracotta/assets/error.ui`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/interface.ui` & `peracotta-2.3.2/src/peracotta/assets/interface.ui`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/themes/Dark.css` & `peracotta-2.3.2/src/peracotta/assets/themes/Dark.css`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/themes/WEEE Open.css` & `peracotta-2.3.2/src/peracotta/assets/themes/WEEE Open.css`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/case.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/case.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/cpu.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/cpu.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/gpu.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/gpu.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/hdd.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/hdd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/keyboard.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/keyboard.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/monitor.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/monitor.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/motherboard.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/motherboard.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/mouse.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/mouse.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/odd.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/odd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/psu.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/psu.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/ram.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/ram.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/ssd.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/ssd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/toolbox/wifi-card.png` & `peracotta-2.3.2/src/peracotta/assets/toolbox/wifi-card.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/ui/light_down_arrow.png` & `peracotta-2.3.2/src/peracotta/assets/ui/light_down_arrow.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/ui/light_split_handle.png` & `peracotta-2.3.2/src/peracotta/assets/ui/light_split_handle.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/ui/pear_emoji.png` & `peracotta-2.3.2/src/peracotta/assets/ui/pear_emoji.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/ui/radio_ckd.png` & `peracotta-2.3.2/src/peracotta/assets/ui/radio_ckd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/ui/radio_unckd.png` & `peracotta-2.3.2/src/peracotta/assets/ui/radio_unckd.png`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/assets/uploadTaralloDialog.ui` & `peracotta-2.3.2/src/peracotta/assets/uploadTaralloDialog.ui`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/commons.py` & `peracotta-2.3.2/src/peracotta/commons.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/config.py` & `peracotta-2.3.2/src/peracotta/config.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/features.json` & `peracotta-2.3.2/src/peracotta/features.json`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/gui/PeraThread.py` & `peracotta-2.3.2/src/peracotta/gui/PeraThread.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/gui/Toolbox.py` & `peracotta-2.3.2/src/peracotta/gui/Toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Optional
+from typing import Dict, List, Optional, Tuple, Union
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 from ..commons import item_only_features
 from ..constants import ICON
 
 from . import prettyprinter
@@ -68,27 +68,27 @@
         h = header + rows + frame
         # print(f"{header} + {rows} + {frame} = {h} > {default_size.height()}")
 
         return QtCore.QSize(default_size.width(), h)
 
     def contextMenuEvent(self, event: QtGui.QContextMenuEvent) -> None:
         menu = QtWidgets.QMenu(self)
-        remove_action = QtGui.QAction("Remove feature", self)
+        remove_action = QtWidgets.QAction("Remove feature", self)
         remove_action.triggered.connect(self.remove_row)
         menu.addAction(remove_action)
         menu.popup(QtGui.QCursor.pos())
 
     def remove_row(self):
         self.model().removeRow(self.selectedIndexes()[1].row(), self.selectedIndexes()[1].parent())
 
 
 class CustomTableModel(QtCore.QAbstractTableModel):
     emergency_resize = QtCore.pyqtSignal(name="emergency_resize")
 
-    def __init__(self, data: list[dict], item_features: dict, product: Optional[dict], default_features: dict):
+    def __init__(self, data: List[dict], item_features: dict, product: Optional[dict], default_features: dict):
         super().__init__()
 
         self._data = data
         self.ref_features = item_features
         self.ref_product = product
         self.default_features = default_features
 
@@ -121,15 +121,15 @@
 
     def flags(self, index):
         if index.column() == 1:
             return QtCore.Qt.ItemFlag.ItemIsEditable | QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
         else:
             return QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
 
-    def row_all_enum_values_for_editor(self, row: int) -> Optional[dict[str, str]]:
+    def row_all_enum_values_for_editor(self, row: int) -> Optional[Dict[str, str]]:
         if row < 0 or row >= len(self.feature_keys):
             return None
 
         name = self.feature_keys[row]
         feature_type = self._get_feature_type(name)
         if feature_type == "e":
             return self.default_features["values"][name]
@@ -222,15 +222,15 @@
                     self._add_to_ref(name, value)
                 if product_to_add:
                     self.endResetModel()
                     self.emergency_resize.emit()
             return ok
         return False
 
-    def extreme_validation(self, name: str, value: [str, int, float]) -> [bool, [str, int, float]]:
+    def extreme_validation(self, name: str, value: Union[str, int, float]) -> Tuple[bool, Union[str, int, float]]:
         feature_type = self._get_feature_type(name)
         if isinstance(value, str):
             value = value.strip()
         if feature_type == "e":
             value = str(value).lower()
             if value not in self.default_features["values"][name]:
                 return False, None
@@ -341,15 +341,15 @@
             target = self.ref_product["features"]
         else:
             target = self.ref_features
         target[name] = value
 
 
 class ToolBoxItem(QtWidgets.QWidget):
-    def __init__(self, data: list[dict], features: dict, product: Optional[dict], default_features: dict):
+    def __init__(self, data: List[dict], features: dict, product: Optional[dict], default_features: dict):
         super().__init__()
         self.default_features = default_features
 
         self.main_layout = QtWidgets.QVBoxLayout()
         self.table = CustomTableView()
         self.features_combo_box = QtWidgets.QComboBox()
         self.feature_line_edit = QtWidgets.QLineEdit()
@@ -366,15 +366,15 @@
 
     def external_size_hint_height(self):
         h1 = max(self.table.minimumSizeHint().height(), self.table.sizeHint().height())
         h2 = self.adder_layout.sizeHint().height()
 
         return h1 + h2
 
-    def table_setup(self, data: list[dict], features: dict, product: Optional[dict], default_features: dict):
+    def table_setup(self, data: List[dict], features: dict, product: Optional[dict], default_features: dict):
         ctm = CustomTableModel(data, features, product, default_features)
         ctm.emergency_resize.connect(self._do_the_emergency_resize)
         self.table.verticalHeader().hide()
         self.table.horizontalHeader().setStretchLastSection(True)
         self.table.setModel(ctm)
         self.table.setShowGrid(False)
         self.table.setAlternatingRowColors(True)
@@ -448,15 +448,15 @@
         self.feature_selector.setEnabled(flag)
 
     def minimumSizeHint(self) -> QtCore.QSize:
         return self.table.minimumSizeHint()
 
 
 class ToolBoxWidget(QtWidgets.QToolBox):
-    def __init__(self, data: list[dict], default_features: dict, encountered_types_count: dict):
+    def __init__(self, data: List[dict], default_features: dict, encountered_types_count: dict):
         super().__init__()
         self.data = data
         self.default_features = default_features
         self.encountered_types_count = encountered_types_count
         self.menu = None
 
         # variables
@@ -464,15 +464,15 @@
 
     def clear(self):
         for idx in range(self.count()):
             self.removeItem(0)
         self.encountered_types_count.clear()
         self.encountered_types_current_count.clear()
 
-    def load_items(self, data: list[dict]):
+    def load_items(self, data: List[dict]):
         if data:
             self.clear()
             self.data = data
             self.types_count()
 
         # find brand, model and variant of all products in data
         products = {}
@@ -525,15 +525,15 @@
         if item_type in ICON:
             icon = QtGui.QIcon(ICON[item_type])
             self.setItemIcon(self.count() - 1, icon)
 
         self.set_context_menu()
 
     @staticmethod
-    def find_matching_product(data: list[dict], features: dict):
+    def find_matching_product(data: List[dict], features: dict):
         if "model" in features and "brand" in features and "variant" in features:
             for maybe in data:
                 if maybe.get("type") == "P":
                     if ToolBoxWidget.bmv_match(features, maybe):
                         return maybe
         return None
 
@@ -555,15 +555,15 @@
             return self.default_features["values"]["type"][the_type]
         else:
             return the_type.title()
 
     def show_menu(self):
         button = self.sender()
         self.menu = QtWidgets.QMenu()
-        remove_action = QtGui.QAction("Remove item", self)
+        remove_action = QtWidgets.QAction("Remove item", self)
         remove_action.triggered.connect(lambda: self.remove_item_from_toolbox(button))
         self.menu.addAction(remove_action)
         self.menu.popup(QtGui.QCursor.pos())
 
     def minimumSizeHint(self) -> QtCore.QSize:
         h = 0
         for child in self.children():
```

### Comparing `peracotta-2.3.1/src/gui/exception_handler.py` & `peracotta-2.3.2/src/peracotta/gui/exception_handler.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/gui/gui.py` & `peracotta-2.3.2/src/peracotta/gui/gui.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/gui/prettyprinter.py` & `peracotta-2.3.2/src/peracotta/gui/prettyprinter.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/gui/widgets.py` & `peracotta-2.3.2/src/peracotta/gui/widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 from cgitb import text
+from typing import List
 
 from PyQt5 import QtCore, QtGui, QtWidgets, uic
 
 from ..constants import PATH
 
 
 class JsonWidget(QtWidgets.QDialog):
-    def __init__(self, data: list[dict], window_size: QtCore.QSize):
+    def __init__(self, data: List[dict], window_size: QtCore.QSize):
         super().__init__()
         layout = QtWidgets.QVBoxLayout()
         text_edit = QtWidgets.QPlainTextEdit()
         text_edit = QtWidgets.QTextEdit()
         text_edit.setWordWrapMode(QtGui.QTextOption.WrapMode.NoWrap)
         text_edit.setPlainText(f"{json.dumps(data, indent=2)}")
         text_edit.setReadOnly(True)
```

### Comparing `peracotta-2.3.1/src/parsers/read_decode_dimms.py` & `peracotta-2.3.2/src/peracotta/parsers/read_decode_dimms.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/parsers/read_dmidecode.py` & `peracotta-2.3.2/src/peracotta/parsers/read_dmidecode.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/parsers/read_lscpu.py` & `peracotta-2.3.2/src/peracotta/parsers/read_lscpu.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/parsers/read_lspci_and_glxinfo.py` & `peracotta-2.3.2/src/peracotta/parsers/read_lspci_and_glxinfo.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/parsers/read_smartctl.py` & `peracotta-2.3.2/src/peracotta/parsers/read_smartctl.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/parsers/windows_parser.py` & `peracotta-2.3.2/src/peracotta/parsers/windows_parser.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/peracruda.py` & `peracotta-2.3.2/src/peracotta/peracruda.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/peralog.py` & `peracotta-2.3.2/src/peracotta/peralog.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/scripts/check_dependencies.sh` & `peracotta-2.3.2/src/peracotta/scripts/check_dependencies.sh`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/scripts/generate_files.sh` & `peracotta-2.3.2/src/peracotta/scripts/generate_files.sh`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/scripts/get_windows_specs.py` & `peracotta-2.3.2/src/peracotta/scripts/get_windows_specs.py`

 * *Files identical despite different names*

### Comparing `peracotta-2.3.1/src/tarallo.py` & `peracotta-2.3.2/src/peracotta/tarallo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from typing import List
 import pytarallo.Errors
 from PyQt5 import QtCore, QtGui, QtWidgets, uic
 from pytarallo import Tarallo
 
 from .constants import PATH
 
 
 class Uploader(QtCore.QThread):
     successEvent = QtCore.pyqtSignal(str)
     failureEvent = QtCore.pyqtSignal(str, str)
 
     def __init__(
         self,
-        data: list[dict],
+        data: List[dict],
         tarallo_url: str,
         tarallo_token: str,
         bulk_identifier: str,
         overwrite: bool,
     ):
         super().__init__()
         self.data = data
```

