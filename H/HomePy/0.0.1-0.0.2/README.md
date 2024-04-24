# Comparing `tmp/HomePy-0.0.1.tar.gz` & `tmp/homepy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomePy-0.0.1.tar", last modified: Fri Dec 22 09:11:15 2023, max compression
+gzip compressed data, was "homepy-0.0.2.tar", last modified: Wed Apr 24 10:12:47 2024, max compression
```

## Comparing `HomePy-0.0.1.tar` & `homepy-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-12-22 09:11:15.807918 HomePy-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-12-22 08:50:46.000000 HomePy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      570 2023-12-22 09:11:15.806921 HomePy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       72 2023-12-22 08:39:42.000000 HomePy-0.0.1/README.md
--rw-rw-rw-   0        0        0      619 2023-12-22 08:57:40.000000 HomePy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0        0 2023-12-22 08:52:09.000000 HomePy-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-12-22 09:11:15.808915 HomePy-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-12-22 09:11:15.779891 HomePy-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-12-22 09:11:15.779891 HomePy-0.0.1/src/HomePy/
--rw-rw-rw-   0        0        0      358 2023-12-22 09:06:59.000000 HomePy-0.0.1/src/HomePy/test.py
-drwxrwxrwx   0        0        0        0 2023-12-22 09:11:15.806921 HomePy-0.0.1/src/HomePy.egg-info/
--rw-rw-rw-   0        0        0      570 2023-12-22 09:11:15.000000 HomePy-0.0.1/src/HomePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-12-22 09:11:15.000000 HomePy-0.0.1/src/HomePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-22 09:11:15.000000 HomePy-0.0.1/src/HomePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-12-22 09:11:15.000000 HomePy-0.0.1/src/HomePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      177 2023-12-22 08:52:34.000000 HomePy-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0      364 2023-12-22 08:53:10.000000 HomePy-0.0.1/src/homeTools.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:12:47.551741 homepy-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-12-22 08:50:46.000000 homepy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      601 2024-04-24 10:12:47.550743 homepy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2023-12-22 08:39:42.000000 homepy-0.0.2/README.md
+-rw-rw-rw-   0        0        0      619 2023-12-22 08:57:40.000000 homepy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       14 2023-12-22 09:47:50.000000 homepy-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 10:12:47.551741 homepy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 10:12:47.544759 homepy-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 10:12:47.545756 homepy-0.0.2/src/HomePy/
+-rw-rw-rw-   0        0        0      146 2023-12-22 09:36:38.000000 homepy-0.0.2/src/HomePy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:12:47.550743 homepy-0.0.2/src/HomePy.egg-info/
+-rw-rw-rw-   0        0        0      601 2024-04-24 10:12:47.000000 homepy-0.0.2/src/HomePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-04-24 10:12:47.000000 homepy-0.0.2/src/HomePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:12:47.000000 homepy-0.0.2/src/HomePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 10:12:47.000000 homepy-0.0.2/src/HomePy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-24 10:12:47.000000 homepy-0.0.2/src/HomePy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      177 2023-12-22 09:35:52.000000 homepy-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-12-22 09:59:46.000000 homepy-0.0.2/src/homeTools.py
```

### Comparing `HomePy-0.0.1/LICENSE` & `homepy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HomePy-0.0.1/pyproject.toml` & `homepy-0.0.2/pyproject.toml`

 * *Files identical despite different names*

