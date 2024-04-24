# Comparing `tmp/paebot-0.1.0.tar.gz` & `tmp/paebot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paebot-0.1.0.tar", last modified: Tue Apr 23 19:30:51 2024, max compression
+gzip compressed data, was "paebot-0.1.1.tar", last modified: Tue Apr 23 19:41:12 2024, max compression
```

## Comparing `paebot-0.1.0.tar` & `paebot-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-23 19:30:51.794957 paebot-0.1.0/
--rw-r--r--   0 null       (501) staff       (20)     1063 2024-04-23 07:54:28.000000 paebot-0.1.0/LICENSE
--rw-r--r--   0 null       (501) staff       (20)      266 2024-04-23 19:30:51.794707 paebot-0.1.0/PKG-INFO
--rw-r--r--   0 null       (501) staff       (20)        8 2024-04-23 16:36:52.000000 paebot-0.1.0/README.md
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-23 19:30:51.793317 paebot-0.1.0/paebot/
--rw-r--r--   0 null       (501) staff       (20)       48 2024-04-23 19:29:16.000000 paebot-0.1.0/paebot/__init__.py
--rw-r--r--   0 null       (501) staff       (20)     1116 2024-04-23 19:30:24.000000 paebot-0.1.0/paebot/paebot.py
-drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-23 19:30:51.794458 paebot-0.1.0/paebot.egg-info/
--rw-r--r--   0 null       (501) staff       (20)      266 2024-04-23 19:30:51.000000 paebot-0.1.0/paebot.egg-info/PKG-INFO
--rw-r--r--   0 null       (501) staff       (20)      211 2024-04-23 19:30:51.000000 paebot-0.1.0/paebot.egg-info/SOURCES.txt
--rw-r--r--   0 null       (501) staff       (20)        1 2024-04-23 19:30:51.000000 paebot-0.1.0/paebot.egg-info/dependency_links.txt
--rw-r--r--   0 null       (501) staff       (20)        9 2024-04-23 19:30:51.000000 paebot-0.1.0/paebot.egg-info/requires.txt
--rw-r--r--   0 null       (501) staff       (20)        7 2024-04-23 19:30:51.000000 paebot-0.1.0/paebot.egg-info/top_level.txt
--rw-r--r--   0 null       (501) staff       (20)       38 2024-04-23 19:30:51.795011 paebot-0.1.0/setup.cfg
--rw-r--r--   0 null       (501) staff       (20)      379 2024-04-23 19:30:29.000000 paebot-0.1.0/setup.py
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-23 19:41:12.748487 paebot-0.1.1/
+-rw-r--r--   0 null       (501) staff       (20)     1063 2024-04-23 07:54:28.000000 paebot-0.1.1/LICENSE
+-rw-r--r--   0 null       (501) staff       (20)      266 2024-04-23 19:41:12.748229 paebot-0.1.1/PKG-INFO
+-rw-r--r--   0 null       (501) staff       (20)        8 2024-04-23 16:36:52.000000 paebot-0.1.1/README.md
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-23 19:41:12.746754 paebot-0.1.1/paebot/
+-rw-r--r--   0 null       (501) staff       (20)     1116 2024-04-23 19:39:24.000000 paebot-0.1.1/paebot/__init__.py
+drwxr-xr-x   0 null       (501) staff       (20)        0 2024-04-23 19:41:12.747922 paebot-0.1.1/paebot.egg-info/
+-rw-r--r--   0 null       (501) staff       (20)      266 2024-04-23 19:41:12.000000 paebot-0.1.1/paebot.egg-info/PKG-INFO
+-rw-r--r--   0 null       (501) staff       (20)      194 2024-04-23 19:41:12.000000 paebot-0.1.1/paebot.egg-info/SOURCES.txt
+-rw-r--r--   0 null       (501) staff       (20)        1 2024-04-23 19:41:12.000000 paebot-0.1.1/paebot.egg-info/dependency_links.txt
+-rw-r--r--   0 null       (501) staff       (20)        9 2024-04-23 19:41:12.000000 paebot-0.1.1/paebot.egg-info/requires.txt
+-rw-r--r--   0 null       (501) staff       (20)        7 2024-04-23 19:41:12.000000 paebot-0.1.1/paebot.egg-info/top_level.txt
+-rw-r--r--   0 null       (501) staff       (20)       38 2024-04-23 19:41:12.748568 paebot-0.1.1/setup.cfg
+-rw-r--r--   0 null       (501) staff       (20)      379 2024-04-23 19:40:38.000000 paebot-0.1.1/setup.py
```

### Comparing `paebot-0.1.0/LICENSE` & `paebot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paebot-0.1.0/paebot/paebot.py` & `paebot-0.1.1/paebot/__init__.py`

 * *Files identical despite different names*

