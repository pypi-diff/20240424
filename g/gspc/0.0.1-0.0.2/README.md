# Comparing `tmp/gspc-0.0.1.tar.gz` & `tmp/gspc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspc-0.0.1.tar", last modified: Sat Apr 13 08:43:39 2024, max compression
+gzip compressed data, was "gspc-0.0.2.tar", last modified: Wed Apr 24 09:15:50 2024, max compression
```

## Comparing `gspc-0.0.1.tar` & `gspc-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,41 @@
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-13 08:43:39.254237 gspc-0.0.1/
--rw-r--r--   0 perraju   (1000) perraju   (1000)      361 2024-04-13 08:43:39.254237 gspc-0.0.1/PKG-INFO
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       45 2024-03-25 13:49:46.000000 gspc-0.0.1/README.md
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-13 08:43:39.250237 gspc-0.0.1/gspc/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2024-04-13 08:42:32.000000 gspc-0.0.1/gspc/__init__.py
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2024-04-13 08:42:35.000000 gspc-0.0.1/gspc/main.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-13 08:43:39.254237 gspc-0.0.1/gspc/settings/
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        0 2024-04-13 08:42:58.000000 gspc-0.0.1/gspc/settings/__init__.py
-drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-13 08:43:39.254237 gspc-0.0.1/gspc.egg-info/
--rw-r--r--   0 perraju   (1000) perraju   (1000)      361 2024-04-13 08:43:39.000000 gspc-0.0.1/gspc.egg-info/PKG-INFO
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      213 2024-04-13 08:43:39.000000 gspc-0.0.1/gspc.egg-info/SOURCES.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        1 2024-04-13 08:43:39.000000 gspc-0.0.1/gspc.egg-info/dependency_links.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       36 2024-04-13 08:43:39.000000 gspc-0.0.1/gspc.egg-info/requires.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)        5 2024-04-13 08:43:39.000000 gspc-0.0.1/gspc.egg-info/top_level.txt
--rw-rw-r--   0 perraju   (1000) perraju   (1000)       38 2024-04-13 08:43:39.254237 gspc-0.0.1/setup.cfg
--rw-rw-r--   0 perraju   (1000) perraju   (1000)      465 2024-04-13 08:43:29.000000 gspc-0.0.1/setup.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.543172 gspc-0.0.2/
+-rw-r--r--   0 perraju   (1000) perraju   (1000)      361 2024-04-24 09:15:50.543172 gspc-0.0.2/PKG-INFO
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       45 2024-03-25 13:49:46.000000 gspc-0.0.2/README.md
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.539172 gspc-0.0.2/gspc/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      181 2024-04-24 09:15:40.000000 gspc-0.0.2/gspc/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.539172 gspc-0.0.2/gspc/core/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      150 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/core/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    13851 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/core/atom.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     3631 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/core/box.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     2141 2024-04-13 09:32:34.000000 gspc-0.0.2/gspc/core/cutoff.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    20121 2024-04-24 08:49:26.000000 gspc-0.0.2/gspc/core/system.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.539172 gspc-0.0.2/gspc/data/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     7530 2024-04-13 09:32:58.000000 gspc-0.0.2/gspc/data/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.539172 gspc-0.0.2/gspc/extensions/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)    14079 2024-04-24 09:09:33.000000 gspc-0.0.2/gspc/extensions/SiO2.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       18 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/extensions/__init__.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.539172 gspc-0.0.2/gspc/io/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      347 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/io/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      707 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/io/make_lines_unique.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     5565 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/io/read_and_create_system.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1031 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/io/read_lattice_properties.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      662 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/io/read_number_of_configurations.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     7112 2024-04-24 09:12:00.000000 gspc-0.0.2/gspc/io/result.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      722 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/io/write_list_of_files.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     6752 2024-04-24 09:03:40.000000 gspc-0.0.2/gspc/main.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.539172 gspc-0.0.2/gspc/settings/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       30 2024-04-13 08:50:02.000000 gspc-0.0.2/gspc/settings/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     5989 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/settings/parameter.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     5761 2024-04-24 08:25:44.000000 gspc-0.0.2/gspc/settings/settings.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.539172 gspc-0.0.2/gspc/utils/
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       97 2024-04-13 08:59:15.000000 gspc-0.0.2/gspc/utils/__init__.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)     1150 2024-04-13 08:58:53.000000 gspc-0.0.2/gspc/utils/generate_color_gradient.py
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      635 2024-04-13 08:55:28.000000 gspc-0.0.2/gspc/utils/print_title.py
+drwxrwxr-x   0 perraju   (1000) perraju   (1000)        0 2024-04-24 09:15:50.539172 gspc-0.0.2/gspc.egg-info/
+-rw-r--r--   0 perraju   (1000) perraju   (1000)      361 2024-04-24 09:15:50.000000 gspc-0.0.2/gspc.egg-info/PKG-INFO
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      732 2024-04-24 09:15:50.000000 gspc-0.0.2/gspc.egg-info/SOURCES.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        1 2024-04-24 09:15:50.000000 gspc-0.0.2/gspc.egg-info/dependency_links.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       36 2024-04-24 09:15:50.000000 gspc-0.0.2/gspc.egg-info/requires.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)        5 2024-04-24 09:15:50.000000 gspc-0.0.2/gspc.egg-info/top_level.txt
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)       38 2024-04-24 09:15:50.543172 gspc-0.0.2/setup.cfg
+-rw-rw-r--   0 perraju   (1000) perraju   (1000)      465 2024-04-24 09:15:33.000000 gspc-0.0.2/setup.py
```

