# Comparing `tmp/pika_pokemon_library-1.0.0.tar.gz` & `tmp/pika_pokemon_library-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pika_pokemon_library-1.0.0.tar", last modified: Tue Apr 23 17:47:23 2024, max compression
+gzip compressed data, was "pika_pokemon_library-1.0.1.tar", last modified: Wed Apr 24 18:46:21 2024, max compression
```

## Comparing `pika_pokemon_library-1.0.0.tar` & `pika_pokemon_library-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:23.631186 pika_pokemon_library-1.0.0/
--rw-rw-rw-   0        0        0      205 2024-04-23 17:47:23.630155 pika_pokemon_library-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:23.630155 pika_pokemon_library-1.0.0/Pika_Pokemon_Library.egg-info/
--rw-rw-rw-   0        0        0      205 2024-04-23 17:47:23.000000 pika_pokemon_library-1.0.0/Pika_Pokemon_Library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-04-23 17:47:23.000000 pika_pokemon_library-1.0.0/Pika_Pokemon_Library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:47:23.000000 pika_pokemon_library-1.0.0/Pika_Pokemon_Library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 17:47:23.000000 pika_pokemon_library-1.0.0/Pika_Pokemon_Library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:47:23.000000 pika_pokemon_library-1.0.0/Pika_Pokemon_Library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      170 2024-04-23 17:14:45.000000 pika_pokemon_library-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 17:47:23.631186 pika_pokemon_library-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      389 2024-04-23 17:47:04.000000 pika_pokemon_library-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:46:21.074874 pika_pokemon_library-1.0.1/
+-rw-rw-rw-   0        0        0      205 2024-04-24 18:46:21.073740 pika_pokemon_library-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:46:21.043863 pika_pokemon_library-1.0.1/Pika_Pokemon_Library/
+-rw-rw-rw-   0        0        0       41 2024-04-19 15:46:21.000000 pika_pokemon_library-1.0.1/Pika_Pokemon_Library/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:14:35.000000 pika_pokemon_library-1.0.1/Pika_Pokemon_Library/pokemon.csv
+-rw-rw-rw-   0        0        0     2248 2024-04-19 15:46:21.000000 pika_pokemon_library-1.0.1/Pika_Pokemon_Library/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:46:21.072432 pika_pokemon_library-1.0.1/Pika_Pokemon_Library.egg-info/
+-rw-rw-rw-   0        0        0      205 2024-04-24 18:46:20.000000 pika_pokemon_library-1.0.1/Pika_Pokemon_Library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-24 18:46:20.000000 pika_pokemon_library-1.0.1/Pika_Pokemon_Library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:46:20.000000 pika_pokemon_library-1.0.1/Pika_Pokemon_Library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:46:20.000000 pika_pokemon_library-1.0.1/Pika_Pokemon_Library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-24 18:46:20.000000 pika_pokemon_library-1.0.1/Pika_Pokemon_Library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      170 2024-04-23 17:14:45.000000 pika_pokemon_library-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:46:21.074874 pika_pokemon_library-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      400 2024-04-24 18:46:12.000000 pika_pokemon_library-1.0.1/setup.py
```

