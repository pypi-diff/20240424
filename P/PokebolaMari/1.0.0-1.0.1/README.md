# Comparing `tmp/pokebolamari-1.0.0.tar.gz` & `tmp/pokebolamari-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokebolamari-1.0.0.tar", last modified: Tue Apr 23 17:47:34 2024, max compression
+gzip compressed data, was "pokebolamari-1.0.1.tar", last modified: Wed Apr 24 18:14:53 2024, max compression
```

## Comparing `pokebolamari-1.0.0.tar` & `pokebolamari-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:34.034620 pokebolamari-1.0.0/
--rw-rw-rw-   0        0        0      236 2024-04-23 17:47:34.028014 pokebolamari-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:34.017572 pokebolamari-1.0.0/PokebolaMari/
--rw-rw-rw-   0        0        0       56 2024-04-19 15:56:31.000000 pokebolamari-1.0.0/PokebolaMari/__init__.py
--rw-rw-rw-   0        0        0     2454 2024-04-23 17:45:21.000000 pokebolamari-1.0.0/PokebolaMari/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:47:34.028014 pokebolamari-1.0.0/PokebolaMari.egg-info/
--rw-rw-rw-   0        0        0      236 2024-04-23 17:47:33.000000 pokebolamari-1.0.0/PokebolaMari.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-04-23 17:47:33.000000 pokebolamari-1.0.0/PokebolaMari.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:47:33.000000 pokebolamari-1.0.0/PokebolaMari.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 17:47:33.000000 pokebolamari-1.0.0/PokebolaMari.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-23 17:47:33.000000 pokebolamari-1.0.0/PokebolaMari.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      175 2024-04-19 15:56:31.000000 pokebolamari-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 17:47:34.034620 pokebolamari-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      527 2024-04-19 15:56:31.000000 pokebolamari-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:14:53.665583 pokebolamari-1.0.1/
+-rw-rw-rw-   0        0        0      236 2024-04-24 18:14:53.665583 pokebolamari-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 18:14:53.649769 pokebolamari-1.0.1/PokebolaMari/
+-rw-rw-rw-   0        0        0       56 2024-04-19 15:56:31.000000 pokebolamari-1.0.1/PokebolaMari/__init__.py
+-rw-rw-rw-   0        0        0     2347 2024-04-23 17:49:19.000000 pokebolamari-1.0.1/PokebolaMari/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-24 18:14:53.665583 pokebolamari-1.0.1/PokebolaMari.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-04-24 18:14:53.000000 pokebolamari-1.0.1/PokebolaMari.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-04-24 18:14:53.000000 pokebolamari-1.0.1/PokebolaMari.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 18:14:53.000000 pokebolamari-1.0.1/PokebolaMari.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 18:14:53.000000 pokebolamari-1.0.1/PokebolaMari.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 18:14:53.000000 pokebolamari-1.0.1/PokebolaMari.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      175 2024-04-19 15:56:31.000000 pokebolamari-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 18:14:53.665583 pokebolamari-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      409 2024-04-24 18:11:26.000000 pokebolamari-1.0.1/setup.py
```

### Comparing `pokebolamari-1.0.0/PokebolaMari/random_pokemon.py` & `pokebolamari-1.0.1/PokebolaMari/random_pokemon.py`

 * *Files 24% similar despite different names*

```diff
@@ -79,14 +79,9 @@
     def getGeneration(self):
         return self._generation
 
     def getLegendary(self):
         return self._legendary
 
 
-#Probando la clase
-#pokemon=RandomPokemon()
-#pokemon.generate_random ()
-#print(pokemon.getPokemon())
-
```

