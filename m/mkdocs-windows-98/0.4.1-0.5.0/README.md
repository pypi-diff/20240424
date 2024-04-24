# Comparing `tmp/mkdocs-windows-98-0.4.1.tar.gz` & `tmp/mkdocs_windows_98-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-windows-98-0.4.1.tar", last modified: Wed Apr 10 13:58:55 2024, max compression
+gzip compressed data, was "mkdocs_windows_98-0.5.0.tar", last modified: Wed Apr 24 09:49:08 2024, max compression
```

## Comparing `mkdocs-windows-98-0.4.1.tar` & `mkdocs_windows_98-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 13:58:45.000000 mkdocs-windows-98-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-10 13:58:45.000000 mkdocs-windows-98-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-10 13:58:45.000000 mkdocs-windows-98-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:45.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:58:55.525477 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 13:58:55.000000 mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:49:08.751278 mkdocs_windows_98-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-24 09:49:08.751278 mkdocs_windows_98-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:49:08.751278 mkdocs_windows_98-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:49:08.747278 mkdocs_windows_98-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:49:08.747278 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/
+-rw-r--r--   0 runner    (1001) docker     (127)    55337 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:49:08.751278 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/css/mkdocs-windows-98.css
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/head.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:49:08.751278 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    12361 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/icons/browse-ui-icons-grayscale.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/icons/browse-ui-icons.png
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/icons/windows-98-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/mkdocs_theme.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/taskbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-24 09:48:58.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98/window-page-content.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:49:08.751278 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-24 09:49:08.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 09:49:08.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:49:08.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 09:49:08.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 09:49:08.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 09:49:08.000000 mkdocs_windows_98-0.5.0/src/mkdocs_windows_98.egg-info/top_level.txt
```

### Comparing `mkdocs-windows-98-0.4.1/LICENSE` & `mkdocs_windows_98-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-windows-98-0.4.1/PKG-INFO` & `mkdocs_windows_98-0.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: mkdocs-windows-98
-Version: 0.4.1
+Version: 0.5.0
 Summary: Windows 98 MkDocs Theme
 Author-email: Useless DevLab <useless.devlab@gmail.com>
+Project-URL: Documentation, https://Useless-DevLab.github.io/mkdocs-windows-98/
+Project-URL: Issues, https://github.com/Useless-DevLab/mkdocs-windows-98/issues
+Project-URL: Source, https://github.com/Useless-DevLab/mkdocs-windows-98
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `mkdocs-windows-98-0.4.1/README.md` & `mkdocs_windows_98-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-windows-98-0.4.1/pyproject.toml` & `mkdocs_windows_98-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 [project]
 name = "mkdocs-windows-98"
-version = "0.4.1"
+version = "0.5.0"
 description = "Windows 98 MkDocs Theme"
 readme = "README.md"
 authors = [
   {name = "Useless DevLab", email = "useless.devlab@gmail.com"}
 ]
 requires-python = ">=3.9"
-
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Operating System :: POSIX",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: System Administrators",
   "Topic :: Software Development :: Build Tools",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.9",
   "Topic :: Utilities",
   "Topic :: Software Development :: Documentation",
 ]
-
 dependencies = [
   "mkdocs>=1.5.3",
 ]
 
+[project.urls]
+Documentation = "https://Useless-DevLab.github.io/mkdocs-windows-98/"
+Issues = "https://github.com/Useless-DevLab/mkdocs-windows-98/issues"
+Source = "https://github.com/Useless-DevLab/mkdocs-windows-98"
+
 [project.optional-dependencies]
 lint = [
   "djlint==1.34.0",
   "yamllint==1.32.0",
 ]
 
 [project.entry-points."mkdocs.themes"]
```

### Comparing `mkdocs-windows-98-0.4.1/src/mkdocs_windows_98.egg-info/PKG-INFO` & `mkdocs_windows_98-0.5.0/src/mkdocs_windows_98.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: mkdocs-windows-98
-Version: 0.4.1
+Version: 0.5.0
 Summary: Windows 98 MkDocs Theme
 Author-email: Useless DevLab <useless.devlab@gmail.com>
+Project-URL: Documentation, https://Useless-DevLab.github.io/mkdocs-windows-98/
+Project-URL: Issues, https://github.com/Useless-DevLab/mkdocs-windows-98/issues
+Project-URL: Source, https://github.com/Useless-DevLab/mkdocs-windows-98
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Build Tools
```

