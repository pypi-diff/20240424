# Comparing `tmp/MVComp-0.9.3.tar.gz` & `tmp/MVComp-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MVComp-0.9.3.tar", last modified: Sun Apr 21 18:38:17 2024, max compression
+gzip compressed data, was "MVComp-0.9.4.tar", last modified: Wed Apr 24 00:23:25 2024, max compression
```

## Comparing `MVComp-0.9.3.tar` & `MVComp-0.9.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 zklsmr    (1000) zklsmr    (1000)        0 2024-04-21 18:38:17.504913 MVComp-0.9.3/
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)    11351 2024-04-11 15:03:25.000000 MVComp-0.9.3/LICENSE
-drwxr-xr-x   0 zklsmr    (1000) zklsmr    (1000)        0 2024-04-21 18:38:17.504913 MVComp-0.9.3/MVComp.egg-info/
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      363 2024-04-21 18:38:17.000000 MVComp-0.9.3/MVComp.egg-info/PKG-INFO
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      175 2024-04-21 18:38:17.000000 MVComp-0.9.3/MVComp.egg-info/SOURCES.txt
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)        1 2024-04-21 18:38:17.000000 MVComp-0.9.3/MVComp.egg-info/dependency_links.txt
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)       67 2024-04-21 18:38:17.000000 MVComp-0.9.3/MVComp.egg-info/requires.txt
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)        1 2024-04-21 18:38:17.000000 MVComp-0.9.3/MVComp.egg-info/top_level.txt
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      363 2024-04-21 18:38:17.504913 MVComp-0.9.3/PKG-INFO
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)     8235 2024-04-11 15:03:25.000000 MVComp-0.9.3/README.md
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)       38 2024-04-21 18:38:17.504913 MVComp-0.9.3/setup.cfg
--rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      428 2024-04-21 18:09:26.000000 MVComp-0.9.3/setup.py
+drwxr-xr-x   0 zklsmr    (1000) zklsmr    (1000)        0 2024-04-24 00:23:25.042512 MVComp-0.9.4/
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)    11351 2024-04-11 15:03:25.000000 MVComp-0.9.4/LICENSE
+drwxr-xr-x   0 zklsmr    (1000) zklsmr    (1000)        0 2024-04-24 00:23:25.042512 MVComp-0.9.4/MVComp.egg-info/
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      251 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/PKG-INFO
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      206 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/SOURCES.txt
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)        1 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/dependency_links.txt
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)       67 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/requires.txt
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)       22 2024-04-24 00:23:25.000000 MVComp-0.9.4/MVComp.egg-info/top_level.txt
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      251 2024-04-24 00:23:25.042512 MVComp-0.9.4/PKG-INFO
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)     8235 2024-04-11 15:03:25.000000 MVComp-0.9.4/README.md
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)    44524 2024-04-23 23:26:46.000000 MVComp-0.9.4/mvcomp.py
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)     2404 2024-04-23 23:26:39.000000 MVComp-0.9.4/plotting.py
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)       38 2024-04-24 00:23:25.042512 MVComp-0.9.4/setup.cfg
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)      527 2024-04-24 00:23:06.000000 MVComp-0.9.4/setup.py
+-rw-r--r--   0 zklsmr    (1000) zklsmr    (1000)    14481 2024-04-23 23:26:39.000000 MVComp-0.9.4/utils.py
```

### Comparing `MVComp-0.9.3/LICENSE` & `MVComp-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MVComp-0.9.3/README.md` & `MVComp-0.9.4/README.md`

 * *Files identical despite different names*

