# Comparing `tmp/commitizen_lrplugin-0.1.0.tar.gz` & `tmp/commitizen_lrplugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen_lrplugin-0.1.0.tar", max compression
+gzip compressed data, was "commitizen_lrplugin-0.1.1.tar", max compression
```

## Comparing `commitizen_lrplugin-0.1.0.tar` & `commitizen_lrplugin-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-16 14:45:27.088544 commitizen_lrplugin-0.1.0/README.md
--rw-r--r--   0        0        0      985 2024-04-16 14:46:01.853893 commitizen_lrplugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 14:45:27.088951 commitizen_lrplugin-0.1.0/src/commitizen_lrplugin/__init__.py
--rw-r--r--   0        0        0     1074 2024-04-16 14:45:27.111910 commitizen_lrplugin-0.1.0/src/commitizen_lrplugin/lrplugin_version_provider.py
--rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 commitizen_lrplugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1129 2024-04-16 15:34:10.351029 commitizen_lrplugin-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1628 2024-04-16 15:34:10.368308 commitizen_lrplugin-0.1.1/README.md
+-rw-r--r--   0        0        0      985 2024-04-24 08:54:53.028698 commitizen_lrplugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 15:34:10.344878 commitizen_lrplugin-0.1.1/src/commitizen_lrplugin/__init__.py
+-rw-r--r--   0        0        0     1074 2024-04-16 15:34:10.362439 commitizen_lrplugin-0.1.1/src/commitizen_lrplugin/lrplugin_version_provider.py
+-rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 commitizen_lrplugin-0.1.1/PKG-INFO
```

### Comparing `commitizen_lrplugin-0.1.0/pyproject.toml` & `commitizen_lrplugin-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "commitizen-lrplugin"
-version = "0.1.0"
+version = "0.1.1"
 description = "Commitizen version provider for Lua Lightroom plug-ins."
 authors = ["Karsten Silkenbäumer <993392+kassi@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "commitizen_lrplugin", from = "src"}]
 
 [tool.poetry.plugins."commitizen.provider"]
 commitizen-lrplugin = "commitizen_lrplugin.lrplugin_version_provider:LRPluginVersionProvider"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
 
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.22.0"
 pytest = "^8.1.1"
 pytest-watcher = "^0.4.2"
 pytest-mock = "^3.14.0"
```

### Comparing `commitizen_lrplugin-0.1.0/src/commitizen_lrplugin/lrplugin_version_provider.py` & `commitizen_lrplugin-0.1.1/src/commitizen_lrplugin/lrplugin_version_provider.py`

 * *Files identical despite different names*

