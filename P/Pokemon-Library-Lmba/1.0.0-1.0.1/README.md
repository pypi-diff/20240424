# Comparing `tmp/pokemon_library_lmba-1.0.0.tar.gz` & `tmp/pokemon_library_lmba-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokemon_library_lmba-1.0.0.tar", last modified: Tue Apr 23 17:45:15 2024, max compression
+gzip compressed data, was "pokemon_library_lmba-1.0.1.tar", last modified: Wed Apr 24 18:32:52 2024, max compression
```

## Comparing `pokemon_library_lmba-1.0.0.tar` & `pokemon_library_lmba-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:45:14.998952 pokemon_library_lmba-1.0.0/
--rw-rw-rw-   0        0        0      213 2024-04-23 17:45:14.992001 pokemon_library_lmba-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 17:45:14.915424 pokemon_library_lmba-1.0.0/Pokemon_Library-Lmba/
--rw-rw-rw-   0        0        0       40 2024-04-19 15:54:14.000000 pokemon_library_lmba-1.0.0/Pokemon_Library-Lmba/__init__.py
--rw-rw-rw-   0        0        0     3527 2024-04-19 15:34:31.000000 pokemon_library_lmba-1.0.0/Pokemon_Library-Lmba/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:45:14.987178 pokemon_library_lmba-1.0.0/Pokemon_Library_Lmba.egg-info/
--rw-rw-rw-   0        0        0      213 2024-04-23 17:45:14.000000 pokemon_library_lmba-1.0.0/Pokemon_Library_Lmba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-04-23 17:45:14.000000 pokemon_library_lmba-1.0.0/Pokemon_Library_Lmba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:45:14.000000 pokemon_library_lmba-1.0.0/Pokemon_Library_Lmba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 17:45:14.000000 pokemon_library_lmba-1.0.0/Pokemon_Library_Lmba.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-23 17:45:14.000000 pokemon_library_lmba-1.0.0/Pokemon_Library_Lmba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      207 2024-04-23 17:42:25.000000 pokemon_library_lmba-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 17:45:15.000264 pokemon_library_lmba-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      397 2024-04-19 15:54:14.000000 pokemon_library_lmba-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:32:52.532371 pokemon_library_lmba-1.0.1/
+-rw-rw-rw-   0        0        0      213 2024-04-24 18:32:52.526659 pokemon_library_lmba-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:32:52.495502 pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/
+-rw-rw-rw-   0        0        0       40 2024-04-19 15:54:14.000000 pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:17:45.000000 pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/pokemon.csv
+-rw-rw-rw-   0        0        0     2399 2024-04-24 18:28:00.000000 pokemon_library_lmba-1.0.1/Pokemon_Library-Lmba/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:32:52.523154 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-24 18:32:52.000000 pokemon_library_lmba-1.0.1/Pokemon_Library_Lmba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2024-04-23 17:42:25.000000 pokemon_library_lmba-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:32:52.533391 pokemon_library_lmba-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      406 2024-04-24 18:29:54.000000 pokemon_library_lmba-1.0.1/setup.py
```

