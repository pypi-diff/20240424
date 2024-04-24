# Comparing `tmp/clickgen-2.2.1.tar.gz` & `tmp/clickgen-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickgen-2.2.1.tar", last modified: Sat Mar  2 11:49:52 2024, max compression
+gzip compressed data, was "clickgen-2.2.2.tar", last modified: Wed Apr 24 13:21:32 2024, max compression
```

## Comparing `clickgen-2.2.1.tar` & `clickgen-2.2.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.265341 clickgen-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-02 11:49:21.000000 clickgen-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-03-02 11:49:52.265341 clickgen-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-02 11:49:21.000000 clickgen-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-02 11:49:21.000000 clickgen-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-02 11:49:52.265341 clickgen-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-02 11:49:21.000000 clickgen-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.253341 clickgen-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.257341 clickgen-2.2.1/src/clickgen/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/configparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/configparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/cursors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.257341 clickgen-2.2.1/src/clickgen/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/libs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/libs/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/libs/colors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.261341 clickgen-2.2.1/src/clickgen/packer/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/packer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/packer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/packer/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/packer/windows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/packer/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/packer/x11.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.261341 clickgen-2.2.1/src/clickgen/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/parser/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/parser/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/parser/png.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/parser/png.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.261341 clickgen-2.2.1/src/clickgen/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/scripts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/scripts/clickgen.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/scripts/clickgen.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/scripts/ctgen.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/scripts/ctgen.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.261341 clickgen-2.2.1/src/clickgen/writer/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/writer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/writer/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/writer/windows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-02 11:49:21.000000 clickgen-2.2.1/src/clickgen/writer/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-02 11:49:49.000000 clickgen-2.2.1/src/clickgen/writer/x11.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.265341 clickgen-2.2.1/src/clickgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-03-02 11:49:52.000000 clickgen-2.2.1/src/clickgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-02 11:49:52.000000 clickgen-2.2.1/src/clickgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 11:49:52.000000 clickgen-2.2.1/src/clickgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-02 11:49:52.000000 clickgen-2.2.1/src/clickgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-02 11:49:52.000000 clickgen-2.2.1/src/clickgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-02 11:49:52.000000 clickgen-2.2.1/src/clickgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 11:49:52.265341 clickgen-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-02 11:49:21.000000 clickgen-2.2.1/tests/test_configparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-02 11:49:21.000000 clickgen-2.2.1/tests/test_cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-02 11:49:21.000000 clickgen-2.2.1/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.017013 clickgen-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 13:21:01.000000 clickgen-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-24 13:21:32.017013 clickgen-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-24 13:21:01.000000 clickgen-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-24 13:21:01.000000 clickgen-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-24 13:21:32.017013 clickgen-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 13:21:01.000000 clickgen-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.005013 clickgen-2.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.009013 clickgen-2.2.2/src/clickgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/configparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/cursors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.009013 clickgen-2.2.2/src/clickgen/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/libs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/libs/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/libs/colors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.013013 clickgen-2.2.2/src/clickgen/packer/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/packer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/packer/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/packer/windows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/packer/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/packer/x11.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.013013 clickgen-2.2.2/src/clickgen/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/parser/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/parser/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/parser/png.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/parser/png.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.013013 clickgen-2.2.2/src/clickgen/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/scripts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/scripts/clickgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/scripts/clickgen.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/scripts/ctgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/scripts/ctgen.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.017013 clickgen-2.2.2/src/clickgen/writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/writer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/writer/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/writer/windows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/writer/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/writer/x11.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.017013 clickgen-2.2.2/src/clickgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 13:21:32.000000 clickgen-2.2.2/src/clickgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.017013 clickgen-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-24 13:21:01.000000 clickgen-2.2.2/tests/test_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-24 13:21:01.000000 clickgen-2.2.2/tests/test_cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 13:21:01.000000 clickgen-2.2.2/tests/test_parser.py
```

### Comparing `clickgen-2.2.1/LICENSE` & `clickgen-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/PKG-INFO` & `clickgen-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickgen
-Version: 2.2.1
+Version: 2.2.2
 Summary: The hassle-free cursor building toolbox.
 Home-page: https://github.com/ful1e5/clickgen
 Author: Abdulkaiz Khatri
 Author-email: kaizmandhu@gmail.com
 Project-URL: Source, https://github.com/ful1e5/clickgen
 Project-URL: Download, https://pypi.org/project/clickgen/#files
 Project-URL: Bug Tracker, https://github.com/ful1e5/clickgen/issues
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: System :: Operating System
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
```

### Comparing `clickgen-2.2.1/README.md` & `clickgen-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/pyproject.toml` & `clickgen-2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/setup.cfg` & `clickgen-2.2.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Multimedia :: Graphics
 	Topic :: System :: Operating System
 	Topic :: Scientific/Engineering :: Image Processing
 	Operating System :: OS Independent
 	Typing :: Typed
 
 [options]
```

### Comparing `clickgen-2.2.1/src/clickgen/configparser.py` & `clickgen-2.2.2/src/clickgen/configparser.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/configparser.pyi` & `clickgen-2.2.2/src/clickgen/configparser.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from clickgen.libs.colors import print_warning as print_warning
 from clickgen.parser import open_blob as open_blob
 from clickgen.parser.png import DELAY as DELAY, SIZES as SIZES
 from clickgen.writer.windows import to_win as to_win
 from clickgen.writer.x11 import to_x11 as to_x11
 from pathlib import Path
-from typing import Any, Dict, List, TypeVar, Union
+from typing import Any, Dict, List, TypeVar
 
 class ThemeSection:
     name: str
     comment: str
     website: str
     def __init__(self, name, comment, website) -> None: ...
     def __lt__(self, other): ...
@@ -28,19 +28,19 @@
     def __gt__(self, other): ...
     def __ge__(self, other): ...
 
 def parse_config_section(fp: Path, d: Dict[str, Any], **kwargs) -> ConfigSection: ...
 T = TypeVar('T')
 
 class CursorSection:
-    x11_cursor_name: Union[str, None]
-    x11_cursor: Union[bytes, None]
+    x11_cursor_name: str | None
+    x11_cursor: bytes | None
     x11_symlinks: List[str]
-    win_cursor_name: Union[str, None]
-    win_cursor: Union[bytes, None]
+    win_cursor_name: str | None
+    win_cursor: bytes | None
     def __init__(self, x11_cursor_name, x11_cursor, x11_symlinks, win_cursor_name, win_cursor) -> None: ...
     def __lt__(self, other): ...
     def __le__(self, other): ...
     def __gt__(self, other): ...
     def __ge__(self, other): ...
 
 def parse_cursors_section(d: Dict[str, Any], config: ConfigSection, **kwargs) -> List[CursorSection]: ...
```

### Comparing `clickgen-2.2.1/src/clickgen/cursors.py` & `clickgen-2.2.2/src/clickgen/cursors.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/cursors.pyi` & `clickgen-2.2.2/src/clickgen/cursors.pyi`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/libs/colors.py` & `clickgen-2.2.2/src/clickgen/libs/colors.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/libs/colors.pyi` & `clickgen-2.2.2/src/clickgen/libs/colors.pyi`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/packer/windows.py` & `clickgen-2.2.2/src/clickgen/packer/windows.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/packer/x11.py` & `clickgen-2.2.2/src/clickgen/packer/x11.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/parser/__init__.py` & `clickgen-2.2.2/src/clickgen/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/parser/png.py` & `clickgen-2.2.2/src/clickgen/parser/png.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/parser/png.pyi` & `clickgen-2.2.2/src/clickgen/parser/png.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from _typeshed import Incomplete
 from clickgen.cursors import CursorFrame as CursorFrame, CursorImage as CursorImage
 from clickgen.parser.base import BaseParser as BaseParser
-from typing import List, Optional, Tuple
+from typing import List, Tuple
 
 SIZES: Incomplete
 DELAY: int
 
 class SinglePNGParser(BaseParser):
     MAGIC: Incomplete
     @classmethod
     def can_parse(cls, blob: bytes) -> bool: ...
     sizes: Incomplete
     delay: Incomplete
     hotspot: Incomplete
     frames: Incomplete
-    def __init__(self, blob: bytes, hotspot: Tuple[int, int], sizes: Optional[List[int]] = None, delay: Optional[int] = None) -> None: ...
+    def __init__(self, blob: bytes, hotspot: Tuple[int, int], sizes: List[int] | None = None, delay: int | None = None) -> None: ...
 
 class MultiPNGParser(BaseParser):
     @classmethod
     def can_parse(cls, blobs: List[bytes]) -> bool: ...
     frames: Incomplete
-    def __init__(self, blobs: List[bytes], hotspot: Tuple[int, int], sizes: Optional[List[int]] = None, delay: Optional[int] = None) -> None: ...
+    def __init__(self, blobs: List[bytes], hotspot: Tuple[int, int], sizes: List[int] | None = None, delay: int | None = None) -> None: ...
```

### Comparing `clickgen-2.2.1/src/clickgen/scripts/clickgen.py` & `clickgen-2.2.2/src/clickgen/scripts/clickgen.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/scripts/ctgen.py` & `clickgen-2.2.2/src/clickgen/scripts/ctgen.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/scripts/ctgen.pyi` & `clickgen-2.2.2/src/clickgen/scripts/ctgen.pyi`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/writer/windows.pyi` & `clickgen-2.2.2/src/clickgen/writer/windows.pyi`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen/writer/x11.py` & `clickgen-2.2.2/src/clickgen/writer/x11.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/src/clickgen.egg-info/PKG-INFO` & `clickgen-2.2.2/src/clickgen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickgen
-Version: 2.2.1
+Version: 2.2.2
 Summary: The hassle-free cursor building toolbox.
 Home-page: https://github.com/ful1e5/clickgen
 Author: Abdulkaiz Khatri
 Author-email: kaizmandhu@gmail.com
 Project-URL: Source, https://github.com/ful1e5/clickgen
 Project-URL: Download, https://pypi.org/project/clickgen/#files
 Project-URL: Bug Tracker, https://github.com/ful1e5/clickgen/issues
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: System :: Operating System
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
```

### Comparing `clickgen-2.2.1/src/clickgen.egg-info/SOURCES.txt` & `clickgen-2.2.2/src/clickgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/tests/test_configparser.py` & `clickgen-2.2.2/tests/test_configparser.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.1/tests/test_cursors.py` & `clickgen-2.2.2/tests/test_cursors.py`

 * *Files identical despite different names*

