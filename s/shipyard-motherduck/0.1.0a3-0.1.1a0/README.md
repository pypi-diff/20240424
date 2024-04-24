# Comparing `tmp/shipyard_motherduck-0.1.0a3.tar.gz` & `tmp/shipyard_motherduck-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_motherduck-0.1.0a3.tar", max compression
+gzip compressed data, was "shipyard_motherduck-0.1.1a0.tar", max compression
```

## Comparing `shipyard_motherduck-0.1.0a3.tar` & `shipyard_motherduck-0.1.1a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-11 02:41:42.600015 shipyard_motherduck-0.1.0a3/README.md
--rw-r--r--   0        0        0      618 2024-04-17 16:58:13.635062 shipyard_motherduck-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-11 13:59:39.563880 shipyard_motherduck-0.1.0a3/shipyard_motherduck/__init__.py
--rw-r--r--   0        0        0      547 2024-04-17 00:40:23.894354 shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/authtest.py
--rw-r--r--   0        0        0     1088 2024-04-17 01:51:26.107771 shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/execute.py
--rw-r--r--   0        0        0     1880 2024-04-17 01:39:58.136436 shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/fetch.py
--rw-r--r--   0        0        0     3061 2024-04-17 16:58:08.969443 shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/upload.py
--rw-r--r--   0        0        0      865 2024-04-17 00:40:23.907409 shipyard_motherduck-0.1.0a3/shipyard_motherduck/exceptions.py
--rw-r--r--   0        0        0     7097 2024-04-17 16:58:08.988425 shipyard_motherduck-0.1.0a3/shipyard_motherduck/motherduck.py
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1389 2024-04-19 17:49:25.468173 shipyard_motherduck-0.1.1a0/README.md
+-rw-r--r--   0        0        0      618 2024-04-24 20:34:17.815450 shipyard_motherduck-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-19 17:49:25.469225 shipyard_motherduck-0.1.1a0/shipyard_motherduck/__init__.py
+-rw-r--r--   0        0        0      857 2024-04-23 20:50:28.199375 shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/authtest.py
+-rw-r--r--   0        0        0     1088 2024-04-19 17:49:25.469563 shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/execute.py
+-rw-r--r--   0        0        0     1880 2024-04-19 17:49:25.469691 shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/fetch.py
+-rw-r--r--   0        0        0     3061 2024-04-19 17:49:25.469825 shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/upload.py
+-rw-r--r--   0        0        0      865 2024-04-19 17:49:25.469968 shipyard_motherduck-0.1.1a0/shipyard_motherduck/exceptions.py
+-rw-r--r--   0        0        0     7097 2024-04-19 17:49:25.470169 shipyard_motherduck-0.1.1a0/shipyard_motherduck/motherduck.py
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.1a0/PKG-INFO
```

### Comparing `shipyard_motherduck-0.1.0a3/pyproject.toml` & `shipyard_motherduck-0.1.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-motherduck"
-version = "0.1.0a3"
+version = "0.1.1a0"
 description = "A local client for working with Python and MotherDuck"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shipyard-templates = "^0.8.2"
```

### Comparing `shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/execute.py` & `shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/execute.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/fetch.py` & `shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a3/shipyard_motherduck/cli/upload.py` & `shipyard_motherduck-0.1.1a0/shipyard_motherduck/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a3/shipyard_motherduck/exceptions.py` & `shipyard_motherduck-0.1.1a0/shipyard_motherduck/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.0a3/shipyard_motherduck/motherduck.py` & `shipyard_motherduck-0.1.1a0/shipyard_motherduck/motherduck.py`

 * *Files identical despite different names*

