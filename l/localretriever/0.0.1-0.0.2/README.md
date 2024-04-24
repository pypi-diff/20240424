# Comparing `tmp/localretriever-0.0.1.tar.gz` & `tmp/localretriever-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localretriever-0.0.1.tar", last modified: Wed Apr 24 13:52:22 2024, max compression
+gzip compressed data, was "localretriever-0.0.2.tar", last modified: Wed Apr 24 14:22:03 2024, max compression
```

## Comparing `localretriever-0.0.1.tar` & `localretriever-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 13:52:22.942360 localretriever-0.0.1/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 localretriever-0.0.1/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      998 2024-04-24 13:52:22.941937 localretriever-0.0.1/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      409 2024-04-24 08:54:46.000000 localretriever-0.0.1/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 13:52:22.941476 localretriever-0.0.1/localretriever.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      998 2024-04-24 13:52:22.000000 localretriever-0.0.1/localretriever.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      215 2024-04-24 13:52:22.000000 localretriever-0.0.1/localretriever.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 13:52:22.000000 localretriever-0.0.1/localretriever.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-24 13:52:22.000000 localretriever-0.0.1/localretriever.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       15 2024-04-24 13:52:22.000000 localretriever-0.0.1/localretriever.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-24 13:52:22.942449 localretriever-0.0.1/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      733 2024-04-24 13:52:01.000000 localretriever-0.0.1/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:22:03.915070 localretriever-0.0.2/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 localretriever-0.0.2/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      908 2024-04-24 14:22:03.914963 localretriever-0.0.2/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      409 2024-04-24 08:54:46.000000 localretriever-0.0.2/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:22:03.912414 localretriever-0.0.2/localretriever/
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-24 14:22:03.914626 localretriever-0.0.2/localretriever/localretriever.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      908 2024-04-24 14:22:03.000000 localretriever-0.0.2/localretriever/localretriever.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      254 2024-04-24 14:22:03.000000 localretriever-0.0.2/localretriever/localretriever.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 14:22:03.000000 localretriever-0.0.2/localretriever/localretriever.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-24 14:22:03.000000 localretriever-0.0.2/localretriever/localretriever.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      397 2024-04-24 14:20:48.000000 localretriever-0.0.2/pyproject.toml
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      658 2024-04-24 14:22:03.915456 localretriever-0.0.2/setup.cfg
```

### Comparing `localretriever-0.0.1/LICENSE` & `localretriever-0.0.2/LICENSE`

 * *Files identical despite different names*

