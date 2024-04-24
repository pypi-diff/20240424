# Comparing `tmp/rrtask-0.0.1.tar.gz` & `tmp/rrtask-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrtask-0.0.1.tar", max compression
+gzip compressed data, was "rrtask-0.0.2.tar", max compression
```

## Comparing `rrtask-0.0.1.tar` & `rrtask-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.1/LICENSE
--rw-r--r--   0        0        0      544 2024-04-23 08:36:29.008275 rrtask-0.0.1/README.md
--rw-r--r--   0        0        0      605 2024-04-24 08:50:04.004580 rrtask-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 08:32:27.303989 rrtask-0.0.1/rrtask/__init__.py
--rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.1/rrtask/enums.py
--rw-r--r--   0        0        0     5558 2024-04-24 08:48:12.620741 rrtask-0.0.1/rrtask/rrtask.py
--rw-r--r--   0        0        0      394 2024-04-24 08:46:36.628959 rrtask-0.0.1/rrtask/signals.py
--rw-r--r--   0        0        0      298 2024-04-24 08:47:32.948821 rrtask-0.0.1/rrtask/utils.py
--rw-r--r--   0        0        0       18 2024-04-24 08:50:11.428572 rrtask-0.0.1/rrtask/version.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 rrtask-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.2/LICENSE
+-rw-r--r--   0        0        0      210 2024-04-24 08:51:24.908514 rrtask-0.0.2/README.md
+-rw-r--r--   0        0        0      605 2024-04-24 08:51:55.456498 rrtask-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 08:32:27.303989 rrtask-0.0.2/rrtask/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.2/rrtask/enums.py
+-rw-r--r--   0        0        0     5558 2024-04-24 08:50:30.008555 rrtask-0.0.2/rrtask/rrtask.py
+-rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.2/rrtask/signals.py
+-rw-r--r--   0        0        0      298 2024-04-24 08:50:30.008555 rrtask-0.0.2/rrtask/utils.py
+-rw-r--r--   0        0        0       18 2024-04-24 08:52:01.472496 rrtask-0.0.2/rrtask/version.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 rrtask-0.0.2/PKG-INFO
```

### Comparing `rrtask-0.0.1/LICENSE` & `rrtask-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rrtask-0.0.1/pyproject.toml` & `rrtask-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rrtask"
-version = "0.0.1"
+version = "0.0.2"
 description = "Round Robin Task"
 authors = ["François Schmidts <francois@schmidts.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.7.*"
```

### Comparing `rrtask-0.0.1/rrtask/rrtask.py` & `rrtask-0.0.2/rrtask/rrtask.py`

 * *Files identical despite different names*

