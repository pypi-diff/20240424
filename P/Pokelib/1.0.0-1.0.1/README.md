# Comparing `tmp/pokelib-1.0.0.tar.gz` & `tmp/pokelib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokelib-1.0.0.tar", last modified: Tue Apr 23 17:36:04 2024, max compression
+gzip compressed data, was "pokelib-1.0.1.tar", last modified: Wed Apr 24 18:43:57 2024, max compression
```

## Comparing `pokelib-1.0.0.tar` & `pokelib-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:36:04.583412 pokelib-1.0.0/
--rw-rw-rw-   0        0        0      202 2024-04-23 17:36:04.581423 pokelib-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 17:36:04.537876 pokelib-1.0.0/Pokelib/
--rw-rw-rw-   0        0        0       41 2024-04-19 15:46:54.000000 pokelib-1.0.0/Pokelib/__init__.py
--rw-rw-rw-   0        0        0    44028 2024-04-16 17:14:28.000000 pokelib-1.0.0/Pokelib/pokemon.csv
--rw-rw-rw-   0        0        0     2842 2024-04-19 03:13:41.000000 pokelib-1.0.0/Pokelib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:36:04.579420 pokelib-1.0.0/Pokelib.egg-info/
--rw-rw-rw-   0        0        0      202 2024-04-23 17:36:04.000000 pokelib-1.0.0/Pokelib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-04-23 17:36:04.000000 pokelib-1.0.0/Pokelib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:36:04.000000 pokelib-1.0.0/Pokelib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 17:36:04.000000 pokelib-1.0.0/Pokelib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 17:36:04.000000 pokelib-1.0.0/Pokelib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      148 2024-04-23 17:20:35.000000 pokelib-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 17:36:04.583412 pokelib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      362 2024-04-23 17:25:25.000000 pokelib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:43:57.489894 pokelib-1.0.1/
+-rw-rw-rw-   0        0        0      202 2024-04-24 18:43:57.488886 pokelib-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:43:57.473938 pokelib-1.0.1/Pokelib/
+-rw-rw-rw-   0        0        0       41 2024-04-19 15:46:54.000000 pokelib-1.0.1/Pokelib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2024-04-16 17:14:28.000000 pokelib-1.0.1/Pokelib/pokemon.csv
+-rw-rw-rw-   0        0        0     2376 2024-04-24 18:10:41.000000 pokelib-1.0.1/Pokelib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:43:57.486894 pokelib-1.0.1/Pokelib.egg-info/
+-rw-rw-rw-   0        0        0      202 2024-04-24 18:43:57.000000 pokelib-1.0.1/Pokelib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-04-24 18:43:57.000000 pokelib-1.0.1/Pokelib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:43:57.000000 pokelib-1.0.1/Pokelib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:43:57.000000 pokelib-1.0.1/Pokelib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 18:43:57.000000 pokelib-1.0.1/Pokelib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1015 2024-04-24 18:19:48.000000 pokelib-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:43:57.489894 pokelib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      358 2024-04-24 18:36:36.000000 pokelib-1.0.1/setup.py
```

### Comparing `pokelib-1.0.0/Pokelib/pokemon.csv` & `pokelib-1.0.1/Pokelib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `pokelib-1.0.0/Pokelib/random_pokemon.py` & `pokelib-1.0.1/Pokelib/random_pokemon.py`

 * *Files 23% similar despite different names*

```diff
@@ -78,27 +78,8 @@
     def getSpeed(self):
         return self._speed
 
     def getGeneration(self):
         return self._generation
 
     def getLegendary(self):
-        return self._legendary
-
-
-#Probando la clase
-pokemon = RandomPokemon()
-pokemon.generate_random()
-print(pokemon.getPokemon())
-print(pokemon.getNumber())
-print(pokemon.getName())
-print(pokemon.getType1())
-print(pokemon.getType2())
-print(pokemon.getTotal())
-print(pokemon.getHp())
-print(pokemon.getAtk())
-print(pokemon.getDefense())
-print(pokemon.getspAtk())
-print(pokemon.getspDef())
-print(pokemon.getSpeed())
-print(pokemon.getGeneration())
-print(pokemon.getLegendary())
+        return self._legendary
```

