# Comparing `tmp/Converttentotwenty-2.0.1.tar.gz` & `tmp/converttentotwenty-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Converttentotwenty-2.0.1.tar", last modified: Thu Mar 14 14:05:52 2024, max compression
+gzip compressed data, was "converttentotwenty-3.0.1.tar", last modified: Wed Apr 24 11:09:39 2024, max compression
```

## Comparing `Converttentotwenty-2.0.1.tar` & `converttentotwenty-3.0.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 14:05:52.478000 Converttentotwenty-2.0.1/
-drwxrwxrwx   0        0        0        0 2024-03-14 14:05:52.436000 Converttentotwenty-2.0.1/Converttentotwenty.egg-info/
--rw-rw-rw-   0        0        0     2602 2024-03-14 14:05:52.000000 Converttentotwenty-2.0.1/Converttentotwenty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-03-14 14:05:52.000000 Converttentotwenty-2.0.1/Converttentotwenty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 14:05:52.000000 Converttentotwenty-2.0.1/Converttentotwenty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 14:05:52.000000 Converttentotwenty-2.0.1/Converttentotwenty.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2602 2024-03-14 14:05:52.454000 Converttentotwenty-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2117 2024-03-14 13:54:16.000000 Converttentotwenty-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-03-14 14:05:52.472000 Converttentotwenty-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      776 2024-03-14 14:05:37.000000 Converttentotwenty-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:09:39.668000 converttentotwenty-3.0.1/
+-rw-rw-rw-   0        0        0     2415 2024-04-24 11:09:39.663000 converttentotwenty-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1961 2024-04-24 11:04:44.000000 converttentotwenty-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 11:09:39.625000 converttentotwenty-3.0.1/converttentotwenty/
+-rw-rw-rw-   0        0        0       42 2024-03-13 15:38:18.000000 converttentotwenty-3.0.1/converttentotwenty/__init__.py
+-rw-rw-rw-   0        0        0     1231 2024-04-24 10:59:51.000000 converttentotwenty-3.0.1/converttentotwenty/converttentotwenty.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:09:39.658000 converttentotwenty-3.0.1/converttentotwenty.egg-info/
+-rw-rw-rw-   0        0        0     2415 2024-04-24 11:09:39.000000 converttentotwenty-3.0.1/converttentotwenty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-24 11:09:39.000000 converttentotwenty-3.0.1/converttentotwenty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 11:09:39.000000 converttentotwenty-3.0.1/converttentotwenty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-24 11:09:39.000000 converttentotwenty-3.0.1/converttentotwenty.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 11:09:39.667000 converttentotwenty-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-04-24 11:08:29.000000 converttentotwenty-3.0.1/setup.py
```

### Comparing `Converttentotwenty-2.0.1/Converttentotwenty.egg-info/PKG-INFO` & `converttentotwenty-3.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,79 @@
 Metadata-Version: 2.1
-Name: Converttentotwenty
-Version: 2.0.1
-Summary: Bibliotèque python conversion base 20
+Name: converttentotwenty
+Version: 3.0.1
+Summary: Ma bibliothèque Python
 Home-page: https://github.com/Joris-ROBIN/Converttentotwenty.git
-Author: Skai
+Author: Skairipa
 Author-email: jorisrobin34@gmail.com
 License: MEEF
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Converttentotwenty
-
 ## Resume
-
 Bibliotheque permettant la traduction d'un message d'une base 10 a base 20.
 
-Voici le dictionnaire de la base 20 utilise : "0123456789abcdefghij".
-Par exemple :   
- - 11 (base10) -> b (base20);      
- - 20 (base10) -> j (base20);     
- - 15 (base10) -> f (base20)
+Voici le dictionnaire de la base 20 utilise : "0123456789abcdefghij". Par exemple :
 
+- 11 (base10) -> b (base20);
+- 20 (base10) -> j (base20);
+- 15 (base10) -> f (base20)
 ## Installation
-La bibloteque peut s'installer via pip grace au [site PyPI](https://pypi.org)
-
-    pip install converttentotwenty
+La bibloteque peut s'installer via pip grace au site PyPI
 
+```
+pip install converttentotwenty
+```
 
 ## Utilisation
+La bibloteque comporte une fonction "traduction()" permettant d'effectuer le changement d'une base a l'autre. Pour importer le paquet :
+```
+from converttentotwenty import traduction
+```
+Voici le docstring de la fonction :
+```
+Convertit les elements d'une liste d'une base a l'autre.
 
-La bibloteque comporte une fonction "traduction()" permettant d'effectuer le changement d'une base Ã  l'autre. Pour importer le paquet : 
-
-    from converttentotwenty import traduction
-
-Voici le docstring de la fonction : 
-
-
-    Convertit les Ã©lÃ©ments d'une liste d'une base Ã  l'autre.
-
-    La conversion de chaque Ã©lÃ©ment se fait d'un entier 
-    de base 10 vers un entier de base 20, selon le dictionnaire de la
-    base 20 fournie en documentation
-    
-    Parameters
-    ----------
-    message : list
-        contient des entiers en base 10.
-
-    Returns
-    -------
-    res : list
-        contient les entiers traduit en base 20 sous forme
-        de chaine de caractÃ¨re.
-
-    Examples
-    --------
-    >>> traduction([4, 0, 16])
-    ['4', '0', 'g']
-    >>> traduction([5, 1, 4])
-    ['5', '1', '4']
-    >>> traduction([11, 16])
-    ['b', 'g']
-    
-La fonction necessite un argument qui doit Ãªtre une liste d'entier en base 10 compris entre 0 et 19 inclus.
-La liste n'a pas de longueur minimale ou maximale.
+La conversion de chaque element se fait d'un entier 
+de base 10 vers un entier de base 20, selon le dictionnaire de la
+base 20 fournie en documentation
+
+Parameters
+----------
+message : list
+    contient des entiers en base 10.
+
+Returns
+-------
+res : list
+    contient les entiers traduit en base 20 sous forme
+    de chaine de caractere.
+
+Examples
+--------
+>>> traduction([4, 0, 16])
+['4', '0', 'g']
+>>> traduction([5, 1, 4])
+['5', '1', '4']
+>>> traduction([11, 16])
+['b', 'g']
+```
+La fonction necessite un argument qui doit etre une liste d'entier en base 10 compris entre 0 et 19 inclus. La liste n'a pas de longueur minimale ou maximale.
 
-La fonction renvoie une liste de chaine de caractere.
-Chaque valeur de cette liste ne peut Ãªtre qu'un seul caractere
+La fonction renvoie une liste de chaine de caractere. Chaque valeur de cette liste ne peut etre qu'un seul caractere
 
 ## Exemples d'utilisation
-
 Voici un exemple d'utilisation de ma biblioteque
 ```
 from converttentotwenty import traduction
 ten = [1, 5, 12, 17]
 twenty = traduction(ten)
 print(twenty)
-```
-```
 ['1', '5', 'c', 'h']    
 ```
-
 ## information annexe
-
-Le but de cette bibliotheque est de l'utiliser a des fins pÃ©dagogiques pour des TP de NSI.  
+Le but de cette bibliotheque est de l'utiliser a des fins pedagogiques pour des TP de NSI.
 La base choisie est arbitraire et n'a pas pour but de representer la realite autour d'une base 20 reellement utilise.
+
```

### Comparing `Converttentotwenty-2.0.1/PKG-INFO` & `converttentotwenty-3.0.1/converttentotwenty.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,79 @@
 Metadata-Version: 2.1
-Name: Converttentotwenty
-Version: 2.0.1
-Summary: Bibliotèque python conversion base 20
+Name: converttentotwenty
+Version: 3.0.1
+Summary: Ma bibliothèque Python
 Home-page: https://github.com/Joris-ROBIN/Converttentotwenty.git
-Author: Skai
+Author: Skairipa
 Author-email: jorisrobin34@gmail.com
 License: MEEF
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Converttentotwenty
-
 ## Resume
-
 Bibliotheque permettant la traduction d'un message d'une base 10 a base 20.
 
-Voici le dictionnaire de la base 20 utilise : "0123456789abcdefghij".
-Par exemple :   
- - 11 (base10) -> b (base20);      
- - 20 (base10) -> j (base20);     
- - 15 (base10) -> f (base20)
+Voici le dictionnaire de la base 20 utilise : "0123456789abcdefghij". Par exemple :
 
+- 11 (base10) -> b (base20);
+- 20 (base10) -> j (base20);
+- 15 (base10) -> f (base20)
 ## Installation
-La bibloteque peut s'installer via pip grace au [site PyPI](https://pypi.org)
-
-    pip install converttentotwenty
+La bibloteque peut s'installer via pip grace au site PyPI
 
+```
+pip install converttentotwenty
+```
 
 ## Utilisation
+La bibloteque comporte une fonction "traduction()" permettant d'effectuer le changement d'une base a l'autre. Pour importer le paquet :
+```
+from converttentotwenty import traduction
+```
+Voici le docstring de la fonction :
+```
+Convertit les elements d'une liste d'une base a l'autre.
 
-La bibloteque comporte une fonction "traduction()" permettant d'effectuer le changement d'une base Ã  l'autre. Pour importer le paquet : 
-
-    from converttentotwenty import traduction
-
-Voici le docstring de la fonction : 
-
-
-    Convertit les Ã©lÃ©ments d'une liste d'une base Ã  l'autre.
-
-    La conversion de chaque Ã©lÃ©ment se fait d'un entier 
-    de base 10 vers un entier de base 20, selon le dictionnaire de la
-    base 20 fournie en documentation
-    
-    Parameters
-    ----------
-    message : list
-        contient des entiers en base 10.
-
-    Returns
-    -------
-    res : list
-        contient les entiers traduit en base 20 sous forme
-        de chaine de caractÃ¨re.
-
-    Examples
-    --------
-    >>> traduction([4, 0, 16])
-    ['4', '0', 'g']
-    >>> traduction([5, 1, 4])
-    ['5', '1', '4']
-    >>> traduction([11, 16])
-    ['b', 'g']
-    
-La fonction necessite un argument qui doit Ãªtre une liste d'entier en base 10 compris entre 0 et 19 inclus.
-La liste n'a pas de longueur minimale ou maximale.
+La conversion de chaque element se fait d'un entier 
+de base 10 vers un entier de base 20, selon le dictionnaire de la
+base 20 fournie en documentation
+
+Parameters
+----------
+message : list
+    contient des entiers en base 10.
+
+Returns
+-------
+res : list
+    contient les entiers traduit en base 20 sous forme
+    de chaine de caractere.
+
+Examples
+--------
+>>> traduction([4, 0, 16])
+['4', '0', 'g']
+>>> traduction([5, 1, 4])
+['5', '1', '4']
+>>> traduction([11, 16])
+['b', 'g']
+```
+La fonction necessite un argument qui doit etre une liste d'entier en base 10 compris entre 0 et 19 inclus. La liste n'a pas de longueur minimale ou maximale.
 
-La fonction renvoie une liste de chaine de caractere.
-Chaque valeur de cette liste ne peut Ãªtre qu'un seul caractere
+La fonction renvoie une liste de chaine de caractere. Chaque valeur de cette liste ne peut etre qu'un seul caractere
 
 ## Exemples d'utilisation
-
 Voici un exemple d'utilisation de ma biblioteque
 ```
 from converttentotwenty import traduction
 ten = [1, 5, 12, 17]
 twenty = traduction(ten)
 print(twenty)
-```
-```
 ['1', '5', 'c', 'h']    
 ```
-
 ## information annexe
-
-Le but de cette bibliotheque est de l'utiliser a des fins pÃ©dagogiques pour des TP de NSI.  
+Le but de cette bibliotheque est de l'utiliser a des fins pedagogiques pour des TP de NSI.
 La base choisie est arbitraire et n'a pas pour but de representer la realite autour d'une base 20 reellement utilise.
+
```

### Comparing `Converttentotwenty-2.0.1/README.md` & `converttentotwenty-3.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,66 @@
 # Converttentotwenty
-
 ## Resume
-
 Bibliotheque permettant la traduction d'un message d'une base 10 a base 20.
 
-Voici le dictionnaire de la base 20 utilise : "0123456789abcdefghij".
-Par exemple :   
- - 11 (base10) -> b (base20);      
- - 20 (base10) -> j (base20);     
- - 15 (base10) -> f (base20)
+Voici le dictionnaire de la base 20 utilise : "0123456789abcdefghij". Par exemple :
 
+- 11 (base10) -> b (base20);
+- 20 (base10) -> j (base20);
+- 15 (base10) -> f (base20)
 ## Installation
-La bibloteque peut s'installer via pip grace au [site PyPI](https://pypi.org)
-
-    pip install converttentotwenty
+La bibloteque peut s'installer via pip grace au site PyPI
 
+```
+pip install converttentotwenty
+```
 
 ## Utilisation
+La bibloteque comporte une fonction "traduction()" permettant d'effectuer le changement d'une base a l'autre. Pour importer le paquet :
+```
+from converttentotwenty import traduction
+```
+Voici le docstring de la fonction :
+```
+Convertit les elements d'une liste d'une base a l'autre.
 
-La bibloteque comporte une fonction "traduction()" permettant d'effectuer le changement d'une base à l'autre. Pour importer le paquet : 
-
-    from converttentotwenty import traduction
-
-Voici le docstring de la fonction : 
-
-
-    Convertit les éléments d'une liste d'une base à l'autre.
-
-    La conversion de chaque élément se fait d'un entier 
-    de base 10 vers un entier de base 20, selon le dictionnaire de la
-    base 20 fournie en documentation
-    
-    Parameters
-    ----------
-    message : list
-        contient des entiers en base 10.
-
-    Returns
-    -------
-    res : list
-        contient les entiers traduit en base 20 sous forme
-        de chaine de caractère.
-
-    Examples
-    --------
-    >>> traduction([4, 0, 16])
-    ['4', '0', 'g']
-    >>> traduction([5, 1, 4])
-    ['5', '1', '4']
-    >>> traduction([11, 16])
-    ['b', 'g']
-    
-La fonction necessite un argument qui doit être une liste d'entier en base 10 compris entre 0 et 19 inclus.
-La liste n'a pas de longueur minimale ou maximale.
+La conversion de chaque element se fait d'un entier 
+de base 10 vers un entier de base 20, selon le dictionnaire de la
+base 20 fournie en documentation
+
+Parameters
+----------
+message : list
+    contient des entiers en base 10.
+
+Returns
+-------
+res : list
+    contient les entiers traduit en base 20 sous forme
+    de chaine de caractere.
+
+Examples
+--------
+>>> traduction([4, 0, 16])
+['4', '0', 'g']
+>>> traduction([5, 1, 4])
+['5', '1', '4']
+>>> traduction([11, 16])
+['b', 'g']
+```
+La fonction necessite un argument qui doit etre une liste d'entier en base 10 compris entre 0 et 19 inclus. La liste n'a pas de longueur minimale ou maximale.
 
-La fonction renvoie une liste de chaine de caractere.
-Chaque valeur de cette liste ne peut être qu'un seul caractere
+La fonction renvoie une liste de chaine de caractere. Chaque valeur de cette liste ne peut etre qu'un seul caractere
 
 ## Exemples d'utilisation
-
 Voici un exemple d'utilisation de ma biblioteque
 ```
 from converttentotwenty import traduction
 ten = [1, 5, 12, 17]
 twenty = traduction(ten)
 print(twenty)
-```
-```
 ['1', '5', 'c', 'h']    
 ```
-
 ## information annexe
-
-Le but de cette bibliotheque est de l'utiliser a des fins pédagogiques pour des TP de NSI.  
+Le but de cette bibliotheque est de l'utiliser a des fins pedagogiques pour des TP de NSI.
 La base choisie est arbitraire et n'a pas pour but de representer la realite autour d'une base 20 reellement utilise.
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Converttentotwenty-2.0.1/setup.py` & `converttentotwenty-3.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Mar 13 13:34:20 2024
-
-@author: Joris
-"""
-
 from setuptools import setup, find_packages
 
 setup(
-    name="Converttentotwenty",
-    version="2.0.1",
-    description="Bibliotèque python conversion base 20",
+    name="converttentotwenty",
+    version="3.0.1",
+    description="Ma bibliothèque Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Joris-ROBIN/Converttentotwenty.git",
-    author="Skai",
+    author="Skairipa",
     author_email="jorisrobin34@gmail.com",
     license="MEEF",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(),
     install_requires=[
-    ],
+    ]
 )
```

