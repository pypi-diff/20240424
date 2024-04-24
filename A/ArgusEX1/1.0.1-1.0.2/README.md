# Comparing `tmp/argusex1-1.0.1.tar.gz` & `tmp/argusex1-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argusex1-1.0.1.tar", last modified: Wed Apr 24 18:12:15 2024, max compression
+gzip compressed data, was "argusex1-1.0.2.tar", last modified: Wed Apr 24 18:33:46 2024, max compression
```

## Comparing `argusex1-1.0.1.tar` & `argusex1-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:12:15.351908 argusex1-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-24 18:12:15.348705 argusex1-1.0.1/ArgusEX1.egg-info/
--rw-rw-rw-   0        0        0      187 2024-04-24 18:12:15.000000 argusex1-1.0.1/ArgusEX1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-24 18:12:15.000000 argusex1-1.0.1/ArgusEX1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:12:15.000000 argusex1-1.0.1/ArgusEX1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 18:12:15.000000 argusex1-1.0.1/ArgusEX1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:12:15.000000 argusex1-1.0.1/ArgusEX1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2024-04-24 18:12:15.350912 argusex1-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      148 2024-04-23 18:31:59.000000 argusex1-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 18:12:15.351908 argusex1-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      355 2024-04-24 18:12:03.000000 argusex1-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:33:46.508230 argusex1-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-24 18:33:46.495836 argusex1-1.0.2/ArgusEX1/
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:13:40.000000 argusex1-1.0.2/ArgusEX1/Poc.csv
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:43:37.000000 argusex1-1.0.2/ArgusEX1/__inti__.py
+-rw-rw-rw-   0        0        0     2116 2024-04-24 16:18:34.000000 argusex1-1.0.2/ArgusEX1/ramdon_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:33:46.505173 argusex1-1.0.2/ArgusEX1.egg-info/
+-rw-rw-rw-   0        0        0      187 2024-04-24 18:33:46.000000 argusex1-1.0.2/ArgusEX1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-24 18:33:46.000000 argusex1-1.0.2/ArgusEX1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:33:46.000000 argusex1-1.0.2/ArgusEX1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:33:46.000000 argusex1-1.0.2/ArgusEX1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 18:33:46.000000 argusex1-1.0.2/ArgusEX1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2024-04-24 18:33:46.507213 argusex1-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2024-04-23 18:31:59.000000 argusex1-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:33:46.508230 argusex1-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      368 2024-04-24 18:33:09.000000 argusex1-1.0.2/setup.py
```

