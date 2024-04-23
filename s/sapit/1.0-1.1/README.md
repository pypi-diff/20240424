# Comparing `tmp/sapit-1.0.tar.gz` & `tmp/sapit-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapit-1.0.tar", last modified: Tue Apr 23 22:36:23 2024, max compression
+gzip compressed data, was "sapit-1.1.tar", last modified: Tue Apr 23 22:47:19 2024, max compression
```

## Comparing `sapit-1.0.tar` & `sapit-1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 22:36:23.624092 sapit-1.0/
--rw-rw-rw-   0        0        0       80 2024-04-23 22:36:23.619092 sapit-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 22:36:23.572120 sapit-1.0/sapit/
--rw-rw-rw-   0        0        0       21 2024-04-23 22:25:03.000000 sapit-1.0/sapit/__init__.py
--rw-rw-rw-   0        0        0      201 2024-04-23 22:25:00.000000 sapit-1.0/sapit/main.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:36:23.616094 sapit-1.0/sapit.egg-info/
--rw-rw-rw-   0        0        0       80 2024-04-23 22:36:23.000000 sapit-1.0/sapit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-23 22:36:23.000000 sapit-1.0/sapit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 22:36:23.000000 sapit-1.0/sapit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 22:36:23.000000 sapit-1.0/sapit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-23 22:36:23.000000 sapit-1.0/sapit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 22:36:23.625095 sapit-1.0/setup.cfg
--rw-rw-rw-   0        0        0      194 2024-04-23 22:34:56.000000 sapit-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:47:19.659031 sapit-1.1/
+-rw-rw-rw-   0        0        0       80 2024-04-23 22:47:19.644040 sapit-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 22:47:19.581076 sapit-1.1/sapit/
+-rw-rw-rw-   0        0        0       21 2024-04-23 22:25:03.000000 sapit-1.1/sapit/__init__.py
+-rw-rw-rw-   0        0        0      201 2024-04-23 22:25:00.000000 sapit-1.1/sapit/main.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:47:19.642041 sapit-1.1/sapit.egg-info/
+-rw-rw-rw-   0        0        0       80 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-23 22:47:19.000000 sapit-1.1/sapit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 22:47:19.660031 sapit-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      302 2024-04-23 22:46:05.000000 sapit-1.1/setup.py
```

