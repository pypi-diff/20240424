# Comparing `tmp/cppiniter-1.1.8.tar.gz` & `tmp/cppiniter-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppiniter-1.1.8.tar", last modified: Fri Mar  1 03:17:23 2024, max compression
+gzip compressed data, was "cppiniter-1.1.9.tar", last modified: Fri Mar  1 07:07:59 2024, max compression
```

## Comparing `cppiniter-1.1.8.tar` & `cppiniter-1.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 03:17:23.681392 cppiniter-1.1.8/
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     1051 2024-01-22 10:59:08.000000 cppiniter-1.1.8/LICENSE
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       30 2024-01-22 10:59:08.000000 cppiniter-1.1.8/MANIFEST.in
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      385 2024-03-01 03:17:23.681392 cppiniter-1.1.8/PKG-INFO
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     2020 2024-02-04 02:47:37.000000 cppiniter-1.1.8/README.md
-drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 03:17:23.681392 cppiniter-1.1.8/cppiniter/
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)        0 2024-01-22 10:59:08.000000 cppiniter-1.1.8/cppiniter/__init__.py
--rwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)     4133 2024-03-01 03:04:53.000000 cppiniter-1.1.8/cppiniter/cppiniter.py
-drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 03:17:23.681392 cppiniter-1.1.8/cppiniter/files/
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     2093 2024-01-22 10:59:08.000000 cppiniter-1.1.8/cppiniter/files/.clang-format
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      892 2024-03-01 02:44:27.000000 cppiniter-1.1.8/cppiniter/files/.clang-tidy
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      858 2024-01-22 10:59:08.000000 cppiniter-1.1.8/cppiniter/files/.gitignore
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      464 2024-01-25 01:39:25.000000 cppiniter-1.1.8/cppiniter/files/.pre-commit-config.yaml
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     3874 2024-03-01 02:44:27.000000 cppiniter-1.1.8/cppiniter/files/CMakeLists.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     1388 2024-01-22 10:59:08.000000 cppiniter-1.1.8/cppiniter/files/CMakeSettings.json
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       21 2024-01-22 10:59:08.000000 cppiniter-1.1.8/cppiniter/files/README.md
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     2972 2024-03-01 03:15:26.000000 cppiniter-1.1.8/cppiniter/files/conanfile.py
-drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 03:17:23.681392 cppiniter-1.1.8/cppiniter/files/example/
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      486 2024-02-04 07:46:52.000000 cppiniter-1.1.8/cppiniter/files/example/CMakeLists.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      145 2024-02-04 02:47:37.000000 cppiniter-1.1.8/cppiniter/files/example/main.cpp
-drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 03:17:23.681392 cppiniter-1.1.8/cppiniter/files/src/
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     1361 2024-02-04 07:46:35.000000 cppiniter-1.1.8/cppiniter/files/src/CMakeLists.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      210 2024-02-04 02:47:37.000000 cppiniter-1.1.8/cppiniter/files/src/main.cpp
-drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 03:17:23.681392 cppiniter-1.1.8/cppiniter/files/src/project_name/
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     2062 2024-02-04 02:47:37.000000 cppiniter-1.1.8/cppiniter/files/src/project_name/export.h
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)        0 2024-02-04 02:47:37.000000 cppiniter-1.1.8/cppiniter/files/src/project_name/project_name.cpp
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)        0 2024-02-04 02:47:37.000000 cppiniter-1.1.8/cppiniter/files/src/project_name/project_name.h
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      182 2024-02-04 02:47:37.000000 cppiniter-1.1.8/cppiniter/files/src/project_name/version.h.in
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      182 2024-02-04 02:47:37.000000 cppiniter-1.1.8/cppiniter/files/src/version.h.in
-drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 03:17:23.681392 cppiniter-1.1.8/cppiniter/files/test/
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      535 2024-02-04 06:29:37.000000 cppiniter-1.1.8/cppiniter/files/test/CMakeLists.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      166 2024-01-22 10:59:08.000000 cppiniter-1.1.8/cppiniter/files/test/main.cpp
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       49 2024-01-22 10:59:08.000000 cppiniter-1.1.8/cppiniter/files/version.properties
-drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 03:17:23.681392 cppiniter-1.1.8/cppiniter.egg-info/
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      385 2024-03-01 03:17:23.000000 cppiniter-1.1.8/cppiniter.egg-info/PKG-INFO
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      985 2024-03-01 03:17:23.000000 cppiniter-1.1.8/cppiniter.egg-info/SOURCES.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)        1 2024-03-01 03:17:23.000000 cppiniter-1.1.8/cppiniter.egg-info/dependency_links.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       55 2024-03-01 03:17:23.000000 cppiniter-1.1.8/cppiniter.egg-info/entry_points.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       25 2024-03-01 03:17:23.000000 cppiniter-1.1.8/cppiniter.egg-info/requires.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       10 2024-03-01 03:17:23.000000 cppiniter-1.1.8/cppiniter.egg-info/top_level.txt
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       38 2024-03-01 03:17:23.681392 cppiniter-1.1.8/setup.cfg
--rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      808 2024-03-01 03:17:04.000000 cppiniter-1.1.8/setup.py
+drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 07:07:59.739986 cppiniter-1.1.9/
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     1051 2024-01-22 10:59:08.000000 cppiniter-1.1.9/LICENSE
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       30 2024-01-22 10:59:08.000000 cppiniter-1.1.9/MANIFEST.in
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      385 2024-03-01 07:07:59.739986 cppiniter-1.1.9/PKG-INFO
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     2020 2024-02-04 02:47:37.000000 cppiniter-1.1.9/README.md
+drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 07:07:59.739986 cppiniter-1.1.9/cppiniter/
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)        0 2024-01-22 10:59:08.000000 cppiniter-1.1.9/cppiniter/__init__.py
+-rwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)     4133 2024-03-01 03:04:53.000000 cppiniter-1.1.9/cppiniter/cppiniter.py
+drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 07:07:59.739986 cppiniter-1.1.9/cppiniter/files/
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     2093 2024-01-22 10:59:08.000000 cppiniter-1.1.9/cppiniter/files/.clang-format
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      892 2024-03-01 02:44:27.000000 cppiniter-1.1.9/cppiniter/files/.clang-tidy
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      858 2024-01-22 10:59:08.000000 cppiniter-1.1.9/cppiniter/files/.gitignore
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      464 2024-01-25 01:39:25.000000 cppiniter-1.1.9/cppiniter/files/.pre-commit-config.yaml
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     3874 2024-03-01 02:44:27.000000 cppiniter-1.1.9/cppiniter/files/CMakeLists.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     1388 2024-01-22 10:59:08.000000 cppiniter-1.1.9/cppiniter/files/CMakeSettings.json
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       21 2024-01-22 10:59:08.000000 cppiniter-1.1.9/cppiniter/files/README.md
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     2972 2024-03-01 03:15:26.000000 cppiniter-1.1.9/cppiniter/files/conanfile.py
+drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 07:07:59.739986 cppiniter-1.1.9/cppiniter/files/example/
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      486 2024-02-04 07:46:52.000000 cppiniter-1.1.9/cppiniter/files/example/CMakeLists.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      145 2024-02-04 02:47:37.000000 cppiniter-1.1.9/cppiniter/files/example/main.cpp
+drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 07:07:59.739986 cppiniter-1.1.9/cppiniter/files/src/
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     1361 2024-02-04 07:46:35.000000 cppiniter-1.1.9/cppiniter/files/src/CMakeLists.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      210 2024-02-04 02:47:37.000000 cppiniter-1.1.9/cppiniter/files/src/main.cpp
+drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 07:07:59.739986 cppiniter-1.1.9/cppiniter/files/src/project_name/
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)     2062 2024-02-04 02:47:37.000000 cppiniter-1.1.9/cppiniter/files/src/project_name/export.h
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)        0 2024-02-04 02:47:37.000000 cppiniter-1.1.9/cppiniter/files/src/project_name/project_name.cpp
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)        0 2024-02-04 02:47:37.000000 cppiniter-1.1.9/cppiniter/files/src/project_name/project_name.h
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      182 2024-02-04 02:47:37.000000 cppiniter-1.1.9/cppiniter/files/src/project_name/version.h.in
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      182 2024-02-04 02:47:37.000000 cppiniter-1.1.9/cppiniter/files/src/version.h.in
+drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 07:07:59.739986 cppiniter-1.1.9/cppiniter/files/test/
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      535 2024-02-04 06:29:37.000000 cppiniter-1.1.9/cppiniter/files/test/CMakeLists.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      166 2024-01-22 10:59:08.000000 cppiniter-1.1.9/cppiniter/files/test/main.cpp
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       48 2024-03-01 07:06:12.000000 cppiniter-1.1.9/cppiniter/files/version.properties
+drwxr-xr-x   0 xyz1001   (1000) xyz1001   (1000)        0 2024-03-01 07:07:59.739986 cppiniter-1.1.9/cppiniter.egg-info/
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      385 2024-03-01 07:07:59.000000 cppiniter-1.1.9/cppiniter.egg-info/PKG-INFO
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      985 2024-03-01 07:07:59.000000 cppiniter-1.1.9/cppiniter.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)        1 2024-03-01 07:07:59.000000 cppiniter-1.1.9/cppiniter.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       55 2024-03-01 07:07:59.000000 cppiniter-1.1.9/cppiniter.egg-info/entry_points.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       25 2024-03-01 07:07:59.000000 cppiniter-1.1.9/cppiniter.egg-info/requires.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       10 2024-03-01 07:07:59.000000 cppiniter-1.1.9/cppiniter.egg-info/top_level.txt
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)       38 2024-03-01 07:07:59.739986 cppiniter-1.1.9/setup.cfg
+-rw-r--r--   0 xyz1001   (1000) xyz1001   (1000)      808 2024-03-01 07:06:49.000000 cppiniter-1.1.9/setup.py
```

### Comparing `cppiniter-1.1.8/LICENSE` & `cppiniter-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/README.md` & `cppiniter-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/cppiniter.py` & `cppiniter-1.1.9/cppiniter/cppiniter.py`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/.clang-format` & `cppiniter-1.1.9/cppiniter/files/.clang-format`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/.clang-tidy` & `cppiniter-1.1.9/cppiniter/files/.clang-tidy`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/.gitignore` & `cppiniter-1.1.9/cppiniter/files/.gitignore`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/CMakeLists.txt` & `cppiniter-1.1.9/cppiniter/files/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/CMakeSettings.json` & `cppiniter-1.1.9/cppiniter/files/CMakeSettings.json`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/conanfile.py` & `cppiniter-1.1.9/cppiniter/files/conanfile.py`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/src/CMakeLists.txt` & `cppiniter-1.1.9/cppiniter/files/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/src/project_name/export.h` & `cppiniter-1.1.9/cppiniter/files/src/project_name/export.h`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter/files/test/CMakeLists.txt` & `cppiniter-1.1.9/cppiniter/files/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/cppiniter.egg-info/SOURCES.txt` & `cppiniter-1.1.9/cppiniter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cppiniter-1.1.8/setup.py` & `cppiniter-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='cppiniter',
-    version="1.1.8",
+    version="1.1.9",
     description="C++项目脚手架",
     long_description="""用于提供C++项目开发环境的初始化""",
     keywords='c++ scaffolding',
     author='xyz1001',
     author_email='zgzf1001@gmail.com',
     url='https://github.com/xyz1001/cppiniter',
     license='MIT',
```

