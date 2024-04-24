# Comparing `tmp/PokeCorky-1.0.0.tar.gz` & `tmp/pokecorky-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokecorky-1.0.0.tar", last modified: Tue Apr 23 17:41:47 2024, max compression
+gzip compressed data, was "pokecorky-1.0.1.tar", last modified: Wed Apr 24 18:07:23 2024, max compression
```

## Comparing `PokeCorky-1.0.0.tar` & `pokecorky-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:41:47.857110 pokecorky-1.0.0/
--rw-rw-rw-   0        0        0      234 2024-04-23 17:41:47.854111 pokecorky-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 17:41:47.850111 pokecorky-1.0.0/PokeCorky.egg-info/
--rw-rw-rw-   0        0        0      234 2024-04-23 17:41:47.000000 pokecorky-1.0.0/PokeCorky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-04-23 17:41:47.000000 pokecorky-1.0.0/PokeCorky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:41:47.000000 pokecorky-1.0.0/PokeCorky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 17:41:47.000000 pokecorky-1.0.0/PokeCorky.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:41:47.000000 pokecorky-1.0.0/PokeCorky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      920 2024-04-23 17:40:37.000000 pokecorky-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 17:41:47.858111 pokecorky-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      413 2024-04-19 15:41:19.000000 pokecorky-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:07:23.928863 pokecorky-1.0.1/
+-rw-rw-rw-   0        0        0      234 2024-04-24 18:07:23.925863 pokecorky-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:07:23.897863 pokecorky-1.0.1/PokeCorky/
+-rw-rw-rw-   0        0        0       41 2024-04-19 15:34:42.000000 pokecorky-1.0.1/PokeCorky/_Init_.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:23:38.000000 pokecorky-1.0.1/PokeCorky/pokemon.csv
+-rw-rw-rw-   0        0        0     2207 2024-04-19 15:34:42.000000 pokecorky-1.0.1/PokeCorky/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:07:23.923863 pokecorky-1.0.1/PokeCorky.egg-info/
+-rw-rw-rw-   0        0        0      234 2024-04-24 18:07:23.000000 pokecorky-1.0.1/PokeCorky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-04-24 18:07:23.000000 pokecorky-1.0.1/PokeCorky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:07:23.000000 pokecorky-1.0.1/PokeCorky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:07:23.000000 pokecorky-1.0.1/PokeCorky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 18:07:23.000000 pokecorky-1.0.1/PokeCorky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      920 2024-04-23 17:40:37.000000 pokecorky-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:07:23.929863 pokecorky-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      426 2024-04-24 18:06:49.000000 pokecorky-1.0.1/setup.py
```

### Comparing `pokecorky-1.0.0/README.md` & `pokecorky-1.0.1/README.md`

 * *Files identical despite different names*

