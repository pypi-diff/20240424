# Comparing `tmp/pokegipsy-1.0.0.tar.gz` & `tmp/pokegipsy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokegipsy-1.0.0.tar", last modified: Tue Apr 23 18:44:47 2024, max compression
+gzip compressed data, was "pokegipsy-1.0.1.tar", last modified: Wed Apr 24 18:14:37 2024, max compression
```

## Comparing `pokegipsy-1.0.0.tar` & `pokegipsy-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:44:47.696208 pokegipsy-1.0.0/
--rw-rw-rw-   0        0        0      194 2024-04-23 18:44:47.695179 pokegipsy-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 18:44:47.670033 pokegipsy-1.0.0/Pokegipsy/
--rw-rw-rw-   0        0        0       41 2024-04-23 15:15:49.000000 pokegipsy-1.0.0/Pokegipsy/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:34:43.000000 pokegipsy-1.0.0/Pokegipsy/pokemon.csv
--rw-rw-rw-   0        0        0     2105 2024-04-23 17:42:01.000000 pokegipsy-1.0.0/Pokegipsy/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:44:47.693110 pokegipsy-1.0.0/Pokegipsy.egg-info/
--rw-rw-rw-   0        0        0      194 2024-04-23 18:44:47.000000 pokegipsy-1.0.0/Pokegipsy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-23 18:44:47.000000 pokegipsy-1.0.0/Pokegipsy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:44:47.000000 pokegipsy-1.0.0/Pokegipsy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 18:44:47.000000 pokegipsy-1.0.0/Pokegipsy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-23 18:44:47.000000 pokegipsy-1.0.0/Pokegipsy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2024-04-23 18:04:03.000000 pokegipsy-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 18:44:47.697244 pokegipsy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      370 2024-04-23 18:44:45.000000 pokegipsy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:14:37.630932 pokegipsy-1.0.1/
+-rw-rw-rw-   0        0        0      194 2024-04-24 18:14:37.628724 pokegipsy-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:14:37.622387 pokegipsy-1.0.1/Pokegipsy/
+-rw-rw-rw-   0        0        0       41 2024-04-23 15:15:49.000000 pokegipsy-1.0.1/Pokegipsy/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:34:43.000000 pokegipsy-1.0.1/Pokegipsy/pokemon.csv
+-rw-rw-rw-   0        0        0     2105 2024-04-23 17:42:01.000000 pokegipsy-1.0.1/Pokegipsy/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:14:37.625538 pokegipsy-1.0.1/Pokegipsy.egg-info/
+-rw-rw-rw-   0        0        0      194 2024-04-24 18:14:37.000000 pokegipsy-1.0.1/Pokegipsy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-04-24 18:14:37.000000 pokegipsy-1.0.1/Pokegipsy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:14:37.000000 pokegipsy-1.0.1/Pokegipsy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:14:37.000000 pokegipsy-1.0.1/Pokegipsy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 18:14:37.000000 pokegipsy-1.0.1/Pokegipsy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      958 2024-04-24 17:27:32.000000 pokegipsy-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:14:37.631930 pokegipsy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      368 2024-04-24 18:11:57.000000 pokegipsy-1.0.1/setup.py
```

### Comparing `pokegipsy-1.0.0/Pokegipsy/pokemon.csv` & `pokegipsy-1.0.1/Pokegipsy/pokemon.csv`

 * *Files identical despite different names*

### Comparing `pokegipsy-1.0.0/Pokegipsy/random_pokemon.py` & `pokegipsy-1.0.1/Pokegipsy/random_pokemon.py`

 * *Files identical despite different names*

