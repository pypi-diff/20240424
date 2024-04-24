# Comparing `tmp/alert_on_exception-0.1.0.tar.gz` & `tmp/alert_on_exception-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alert_on_exception-0.1.0.tar", last modified: Wed Apr 24 09:58:44 2024, max compression
+gzip compressed data, was "alert_on_exception-0.1.1.tar", last modified: Wed Apr 24 10:17:35 2024, max compression
```

## Comparing `alert_on_exception-0.1.0.tar` & `alert_on_exception-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 09:58:44.451190 alert_on_exception-0.1.0/
--rw-rw-r--   0 user1     (1001) user1     (1001)     1112 2024-04-24 09:35:45.000000 alert_on_exception-0.1.0/LICENSE
--rw-r--r--   0 user1     (1001) user1     (1001)      136 2024-04-24 09:58:44.451190 alert_on_exception-0.1.0/PKG-INFO
--rw-rw-r--   0 user1     (1001) user1     (1001)      864 2024-04-24 09:58:41.000000 alert_on_exception-0.1.0/README.md
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 09:58:44.451190 alert_on_exception-0.1.0/alert_on_exception.egg-info/
--rw-r--r--   0 user1     (1001) user1     (1001)      136 2024-04-24 09:58:44.000000 alert_on_exception-0.1.0/alert_on_exception.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1001) user1     (1001)      292 2024-04-24 09:58:44.000000 alert_on_exception-0.1.0/alert_on_exception.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-24 09:58:44.000000 alert_on_exception-0.1.0/alert_on_exception.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)       14 2024-04-24 09:58:44.000000 alert_on_exception-0.1.0/alert_on_exception.egg-info/requires.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)        4 2024-04-24 09:58:44.000000 alert_on_exception-0.1.0/alert_on_exception.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)       90 2024-04-24 09:33:49.000000 alert_on_exception-0.1.0/pyproject.toml
--rw-rw-r--   0 user1     (1001) user1     (1001)       38 2024-04-24 09:58:44.451190 alert_on_exception-0.1.0/setup.cfg
--rw-rw-r--   0 user1     (1001) user1     (1001)      265 2024-04-24 09:58:06.000000 alert_on_exception-0.1.0/setup.py
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 09:58:44.451190 alert_on_exception-0.1.0/src/
--rw-rw-r--   0 user1     (1001) user1     (1001)       49 2024-04-24 09:54:19.000000 alert_on_exception-0.1.0/src/__init__.py
--rw-rw-r--   0 user1     (1001) user1     (1001)      987 2024-04-24 09:54:22.000000 alert_on_exception-0.1.0/src/alert_on_exception.py
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/
+-rw-rw-r--   0 user1     (1001) user1     (1001)     1112 2024-04-24 09:35:45.000000 alert_on_exception-0.1.1/LICENSE
+-rw-r--r--   0 user1     (1001) user1     (1001)     1100 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/PKG-INFO
+-rw-rw-r--   0 user1     (1001) user1     (1001)      864 2024-04-24 09:58:41.000000 alert_on_exception-0.1.1/README.md
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/alert_on_exception.egg-info/
+-rw-r--r--   0 user1     (1001) user1     (1001)     1100 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1001) user1     (1001)      292 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)       14 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)        4 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)       90 2024-04-24 09:33:49.000000 alert_on_exception-0.1.1/pyproject.toml
+-rw-rw-r--   0 user1     (1001) user1     (1001)       38 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/setup.cfg
+-rw-rw-r--   0 user1     (1001) user1     (1001)      652 2024-04-24 10:17:30.000000 alert_on_exception-0.1.1/setup.py
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/src/
+-rw-rw-r--   0 user1     (1001) user1     (1001)       49 2024-04-24 09:54:19.000000 alert_on_exception-0.1.1/src/__init__.py
+-rw-rw-r--   0 user1     (1001) user1     (1001)      987 2024-04-24 09:54:22.000000 alert_on_exception-0.1.1/src/alert_on_exception.py
```

### Comparing `alert_on_exception-0.1.0/LICENSE` & `alert_on_exception-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alert_on_exception-0.1.0/README.md` & `alert_on_exception-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alert_on_exception-0.1.0/src/alert_on_exception.py` & `alert_on_exception-0.1.1/src/alert_on_exception.py`

 * *Files identical despite different names*

