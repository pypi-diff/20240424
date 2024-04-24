# Comparing `tmp/PKRDPNT-1.0.0.tar.gz` & `tmp/PKRDPNT-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrdpnt-1.0.0.tar", last modified: Wed Apr 24 17:43:43 2024, max compression
+gzip compressed data, was "pkrdpnt-1.0.1.tar", last modified: Wed Apr 24 18:18:03 2024, max compression
```

## Comparing `PKRDPNT-1.0.0.tar` & `PKRDPNT-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 17:43:43.971192 pkrdpnt-1.0.0/
--rw-rw-rw-   0        0        0      200 2024-04-24 17:43:43.969195 pkrdpnt-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 17:43:43.966192 pkrdpnt-1.0.0/PKRDPNT.egg-info/
--rw-rw-rw-   0        0        0      200 2024-04-24 17:43:43.000000 pkrdpnt-1.0.0/PKRDPNT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-24 17:43:43.000000 pkrdpnt-1.0.0/PKRDPNT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 17:43:43.000000 pkrdpnt-1.0.0/PKRDPNT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 17:43:43.000000 pkrdpnt-1.0.0/PKRDPNT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 17:43:43.000000 pkrdpnt-1.0.0/PKRDPNT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      280 2024-04-23 17:30:36.000000 pkrdpnt-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 17:43:43.972192 pkrdpnt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      372 2024-04-24 17:42:18.000000 pkrdpnt-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:18:03.264485 pkrdpnt-1.0.1/
+-rw-rw-rw-   0        0        0      200 2024-04-24 18:18:03.262483 pkrdpnt-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:18:03.261482 pkrdpnt-1.0.1/PKRDPNT.egg-info/
+-rw-rw-rw-   0        0        0      200 2024-04-24 18:18:03.000000 pkrdpnt-1.0.1/PKRDPNT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-24 18:18:03.000000 pkrdpnt-1.0.1/PKRDPNT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:18:03.000000 pkrdpnt-1.0.1/PKRDPNT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:18:03.000000 pkrdpnt-1.0.1/PKRDPNT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:18:03.000000 pkrdpnt-1.0.1/PKRDPNT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      280 2024-04-23 17:30:36.000000 pkrdpnt-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:18:03.265487 pkrdpnt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      405 2024-04-24 18:17:51.000000 pkrdpnt-1.0.1/setup.py
```

