# Comparing `tmp/dosmaster-1.8.3.tar.gz` & `tmp/dosmaster-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.8.3.tar", last modified: Mon Mar 11 04:41:21 2024, max compression
+gzip compressed data, was "dist/dosmaster-1.8.4.tar", last modified: Wed Apr 24 18:13:33 2024, max compression
```

## Comparing `dosmaster-1.8.3.tar` & `dosmaster-1.8.4.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      214 2024-03-11 04:31:06.000000 dosmaster-1.8.3/MANIFEST.in
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2024-03-11 04:41:21.000000 dosmaster-1.8.3/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2689 2024-03-11 04:34:58.000000 dosmaster-1.8.3/README.md
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/__init__.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster/base/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/base/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3535 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/base/data_generation.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5276 2024-03-11 04:39:50.000000 dosmaster-1.8.3/dosmaster/base/printer.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster/custom_setting/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      288 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/custom_setting/example_default.yaml
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/custom_setting/example_figure_size_up.yaml
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/custom_setting/example_font_size_up.yaml
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster/features/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4281 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/a_add_atom_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11865 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/b_dos_projection.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2128 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/c_dos_sum.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3189 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/d_average_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2404 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/e_remove_dos.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/f_change_sign.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    12152 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/g_graph_editor.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5897 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/h_axis_optimization.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2061 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/i_import_custom_setting.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1241 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/j_save_custom_setting.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1963 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/k_import_dosmaster_data.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      961 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/features/l_save_dosmaster_data.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster/fileparser/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/fileparser/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4777 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/fileparser/doscar_split.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/fileparser/procar_parser.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/fileparser/structure_parser.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster/main/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/main/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7598 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/main/dosmaster.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster/mainplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/mainplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11921 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/mainplotter/dosplot.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster/subplotter/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/subplotter/__init__.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/subplotter/colors.csv
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/subplotter/colortable.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7081 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/subplotter/dosplot_manager.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2024-03-11 04:33:19.000000 dosmaster-1.8.3/dosmaster/subplotter/make_color_list.py
-drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-03-11 04:41:21.000000 dosmaster-1.8.3/dosmaster.egg-info/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2024-03-11 04:41:20.000000 dosmaster-1.8.3/dosmaster.egg-info/PKG-INFO
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1445 2024-03-11 04:41:20.000000 dosmaster-1.8.3/dosmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2024-03-11 04:41:20.000000 dosmaster-1.8.3/dosmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2024-03-11 04:41:20.000000 dosmaster-1.8.3/dosmaster.egg-info/entry_points.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       66 2024-03-11 04:41:20.000000 dosmaster-1.8.3/dosmaster.egg-info/requires.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2024-03-11 04:41:20.000000 dosmaster-1.8.3/dosmaster.egg-info/top_level.txt
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2024-03-11 04:41:21.000000 dosmaster-1.8.3/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1346 2024-03-11 04:31:06.000000 dosmaster-1.8.3/setup.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1069 2024-04-24 17:32:35.000000 dosmaster-1.8.4/LICENSE
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      214 2024-03-11 04:31:06.000000 dosmaster-1.8.4/MANIFEST.in
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      719 2024-04-24 18:13:33.000000 dosmaster-1.8.4/PKG-INFO
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2944 2024-04-24 18:11:32.000000 dosmaster-1.8.4/README.md
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/__init__.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/base/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/base/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3535 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/base/data_generation.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5276 2024-03-11 04:39:50.000000 dosmaster-1.8.4/dosmaster/base/printer.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/custom_setting/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      288 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/custom_setting/example_default.yaml
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/custom_setting/example_figure_size_up.yaml
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      289 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/custom_setting/example_font_size_up.yaml
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/features/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4281 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/a_add_atom_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11865 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/b_dos_projection.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2128 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/c_dos_sum.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3189 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/d_average_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     2404 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/e_remove_dos.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/f_change_sign.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    12152 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/g_graph_editor.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     5897 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/h_axis_optimization.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2061 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/i_import_custom_setting.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1241 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/j_save_custom_setting.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1963 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/k_import_dosmaster_data.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      961 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/features/l_save_dosmaster_data.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/fileparser/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/fileparser/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     4777 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/fileparser/doscar_split.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/fileparser/procar_parser.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/fileparser/structure_parser.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/main/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2024-04-24 17:38:45.000000 dosmaster-1.8.4/dosmaster/main/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7598 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/main/dosmaster.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/mainplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/mainplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)    11921 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/mainplotter/dosplot.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster/subplotter/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/__init__.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/colors.csv
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/colortable.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     7081 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/dosplot_manager.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2024-03-11 04:33:19.000000 dosmaster-1.8.4/dosmaster/subplotter/make_color_list.py
+drwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2024-04-24 18:13:33.000000 dosmaster-1.8.4/dosmaster.egg-info/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      719 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1453 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       66 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/requires.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2024-04-24 18:13:32.000000 dosmaster-1.8.4/dosmaster.egg-info/top_level.txt
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2024-04-24 18:13:33.000000 dosmaster-1.8.4/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1403 2024-04-24 17:41:51.000000 dosmaster-1.8.4/setup.py
```

### Comparing `dosmaster-1.8.3/README.md` & `dosmaster-1.8.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 # DOSMaster
+
+Link for dosmaster-pypi package(click the icon)
+
+[![PyPI](https://img.shields.io/pypi/v/dosmaster.svg)](https://pypi.org/project/dosmaster/)
+
 Program Name : dosmaster Program
 
 Made by Youngjun Park (yjpark29@postech.ac.kr)
 
 Inspired by Jaesun Kim(CNMD)
 
 Tested by Changhun Kim(CNMD), Suyun Chae(CNMD)
@@ -10,14 +15,15 @@
 Edit Date : 24/03/10
 
 Description : DOS Plot Smartly in Terminal Environment
 
 
 version.1.8.3 이 되면 CNMD 구성원 전체에게 공개
 
+### Release History
 
 ver.1.1 : 재시작 시 loading 속도 향상 (by Jaesun Kim)
 
 ver.1.2 : 최종 data 파일 저장 기능 추가
 
 ver.1.3 : 버그 수정
 
@@ -25,14 +31,16 @@
 
 ver 1.7.13 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
 
 ver 1.8.1 : Label 버그 수정, 각종 버그 수정, Setting 저장 및 불러오기 기능 구현, DOS plot 저장 및 불러오기 기능 구현, shift_x_axis 구현, 연속된 숫자 입력 기능 확장, legend display 여부 선택 가능
 
 ver 1.8.3 : ISPIN = 1 calculation 지원 및 각종 버그 수정
 
+ver 1.8.4 : Lisence 수정
+
 
 ## Features
 1) Add Atom DOS : 원하는 atom의 DOS를 추가합니다.
 2) DOS Projection : 특정 DOS를 원하는 orbital로 projection 시킵니다.
 3) Sum DOS : 특정 DOS들의 기여분을 합칩니다.
 4) Average DOS : 특정 DOS들의 기여분을 평균화합니다.
 5) Remove DOS : 특정 DOS를 지웁니다.
@@ -74,7 +82,11 @@
 
     $ chmod 774 dosmaster
 
 ## Run dosmaster
 
     $ cd [DOS 계산한 폴더]
     $ dosmaster
+
+
+## License
+DOSMaster is made available under the MIT License.
```

### Comparing `dosmaster-1.8.3/dosmaster/base/data_generation.py` & `dosmaster-1.8.4/dosmaster/base/data_generation.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/base/printer.py` & `dosmaster-1.8.4/dosmaster/base/printer.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/a_add_atom_dos.py` & `dosmaster-1.8.4/dosmaster/features/a_add_atom_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/b_dos_projection.py` & `dosmaster-1.8.4/dosmaster/features/b_dos_projection.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/c_dos_sum.py` & `dosmaster-1.8.4/dosmaster/features/c_dos_sum.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/d_average_dos.py` & `dosmaster-1.8.4/dosmaster/features/d_average_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/e_remove_dos.py` & `dosmaster-1.8.4/dosmaster/features/e_remove_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/f_change_sign.py` & `dosmaster-1.8.4/dosmaster/features/f_change_sign.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/g_graph_editor.py` & `dosmaster-1.8.4/dosmaster/features/g_graph_editor.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/h_axis_optimization.py` & `dosmaster-1.8.4/dosmaster/features/h_axis_optimization.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/i_import_custom_setting.py` & `dosmaster-1.8.4/dosmaster/features/i_import_custom_setting.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/j_save_custom_setting.py` & `dosmaster-1.8.4/dosmaster/features/j_save_custom_setting.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/k_import_dosmaster_data.py` & `dosmaster-1.8.4/dosmaster/features/k_import_dosmaster_data.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/features/l_save_dosmaster_data.py` & `dosmaster-1.8.4/dosmaster/features/l_save_dosmaster_data.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/fileparser/doscar_split.py` & `dosmaster-1.8.4/dosmaster/fileparser/doscar_split.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/fileparser/structure_parser.py` & `dosmaster-1.8.4/dosmaster/fileparser/structure_parser.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/main/dosmaster.py` & `dosmaster-1.8.4/dosmaster/main/dosmaster.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/mainplotter/dosplot.py` & `dosmaster-1.8.4/dosmaster/mainplotter/dosplot.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/subplotter/colors.csv` & `dosmaster-1.8.4/dosmaster/subplotter/colors.csv`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/subplotter/colortable.py` & `dosmaster-1.8.4/dosmaster/subplotter/colortable.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/subplotter/dosplot_manager.py` & `dosmaster-1.8.4/dosmaster/subplotter/dosplot_manager.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster/subplotter/make_color_list.py` & `dosmaster-1.8.4/dosmaster/subplotter/make_color_list.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.8.3/dosmaster.egg-info/SOURCES.txt` & `dosmaster-1.8.4/dosmaster.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 dosmaster/__init__.py
 dosmaster.egg-info/PKG-INFO
 dosmaster.egg-info/SOURCES.txt
 dosmaster.egg-info/dependency_links.txt
```

### Comparing `dosmaster-1.8.3/setup.py` & `dosmaster-1.8.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 #    long_description = file.read()
 
 setup(
     name="dosmaster",
     version=__version__,
     description="DOS(Density Of States) Plot Smartly in Terminal",
     url="https://github.com/pyj6767/DOSMaster",
-    author="Youngjun Park, Jaeson Kim",
+    author="Youngjun Park, Jaeson Kim in CNMD",
     author_email="yjpark29@postech.ac.kr",
     #long_description=long_description,
-    license="CNMD",
+    license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Scientific/Engineering :: Physics",
+        "License :: OSI Approved :: MIT License",
     ],
     keywords="vasp dos",
     packages=find_packages(),
     python_requires=">=3.7.13",
     install_requires=[
         "numpy",
         "matplotlib",
```

