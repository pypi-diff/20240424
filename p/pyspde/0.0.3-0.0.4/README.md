# Comparing `tmp/pyspde-0.0.3.tar.gz` & `tmp/pyspde-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspde-0.0.3.tar", last modified: Tue Apr 23 23:40:12 2024, max compression
+gzip compressed data, was "pyspde-0.0.4.tar", last modified: Wed Apr 24 00:55:32 2024, max compression
```

## Comparing `pyspde-0.0.3.tar` & `pyspde-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 23:40:12.904405 pyspde-0.0.3/
--rw-rw-rw-   0        0        0     1085 2024-04-09 03:25:05.000000 pyspde-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1571 2024-04-23 23:40:12.903402 pyspde-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      766 2024-04-23 23:20:23.000000 pyspde-0.0.3/README.md
--rw-rw-rw-   0        0        0     1198 2024-04-23 23:40:02.000000 pyspde-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 23:40:12.904405 pyspde-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 23:40:12.884969 pyspde-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 23:40:12.889982 pyspde-0.0.3/src/pyspde/
--rw-rw-rw-   0        0        0       69 2024-04-11 06:43:36.000000 pyspde-0.0.3/src/pyspde/__init__.py
--rw-rw-rw-   0        0        0     8686 2024-04-23 00:07:28.000000 pyspde-0.0.3/src/pyspde/anisotropy.py
--rw-rw-rw-   0        0        0     4632 2024-04-23 00:01:53.000000 pyspde-0.0.3/src/pyspde/grid.py
--rw-rw-rw-   0        0        0     3606 2024-04-23 06:08:32.000000 pyspde-0.0.3/src/pyspde/neighbours.py
--rw-rw-rw-   0        0        0    10608 2024-04-23 06:10:05.000000 pyspde-0.0.3/src/pyspde/spde.py
--rw-rw-rw-   0        0        0     5013 2024-04-23 06:10:05.000000 pyspde-0.0.3/src/pyspde/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:40:12.903402 pyspde-0.0.3/src/pyspde.egg-info/
--rw-rw-rw-   0        0        0     1571 2024-04-23 23:40:12.000000 pyspde-0.0.3/src/pyspde.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-23 23:40:12.000000 pyspde-0.0.3/src/pyspde.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 23:40:12.000000 pyspde-0.0.3/src/pyspde.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-23 23:40:12.000000 pyspde-0.0.3/src/pyspde.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 23:40:12.000000 pyspde-0.0.3/src/pyspde.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 00:55:32.013612 pyspde-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2024-04-09 03:25:05.000000 pyspde-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1732 2024-04-24 00:55:32.012608 pyspde-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      927 2024-04-24 00:22:13.000000 pyspde-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1198 2024-04-24 00:55:20.000000 pyspde-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 00:55:32.013612 pyspde-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 00:55:31.994996 pyspde-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 00:55:32.000758 pyspde-0.0.4/src/pyspde/
+-rw-rw-rw-   0        0        0       91 2024-04-24 00:34:35.000000 pyspde-0.0.4/src/pyspde/__init__.py
+-rw-rw-rw-   0        0        0     8686 2024-04-23 00:07:28.000000 pyspde-0.0.4/src/pyspde/anisotropy.py
+-rw-rw-rw-   0        0        0     4632 2024-04-23 00:01:53.000000 pyspde-0.0.4/src/pyspde/grid.py
+-rw-rw-rw-   0        0        0     3606 2024-04-23 06:08:32.000000 pyspde-0.0.4/src/pyspde/neighbours.py
+-rw-rw-rw-   0        0        0    10608 2024-04-23 06:10:05.000000 pyspde-0.0.4/src/pyspde/spde.py
+-rw-rw-rw-   0        0        0     4904 2024-04-24 00:34:21.000000 pyspde-0.0.4/src/pyspde/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 00:55:32.011264 pyspde-0.0.4/src/pyspde.egg-info/
+-rw-rw-rw-   0        0        0     1732 2024-04-24 00:55:31.000000 pyspde-0.0.4/src/pyspde.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-04-24 00:55:31.000000 pyspde-0.0.4/src/pyspde.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 00:55:31.000000 pyspde-0.0.4/src/pyspde.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-24 00:55:31.000000 pyspde-0.0.4/src/pyspde.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 00:55:31.000000 pyspde-0.0.4/src/pyspde.egg-info/top_level.txt
```

### Comparing `pyspde-0.0.3/LICENSE` & `pyspde-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.3/PKG-INFO` & `pyspde-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspde
-Version: 0.0.3
+Version: 0.0.4
 Summary: PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)
 Author-email: Esteban Jimenez <ejimenez@minerai.com.au>
 Project-URL: Homepage, https://github.com/M1nerAI/pyspde
 Project-URL: Issues, https://github.com/M1nerAI/pyspde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,29 +23,37 @@
 $$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \mathbb{R}^2
 $$
 
 The theory is proposed in Fuglstad (2014).
 
 ## Instalation
 
+On Debian/Ubuntu systems:
 ```
+sudo apt-get install libsuitesparse-dev
+pip install pyspde
+```
+
+On Windows systems:
+```
+conda install -c conda-forge suitesparse
 pip install pyspde
 ```
 
 ## Basic Usage
 
 Imports:
 ```
 from pyspde import anisotropy, Grid, Spde
 ```
 
 Define the anisotropy and the grid:
 ```
-atrp = anisotropy_from_svg(r'assets/anicline.svg', beta=10, gamma=0.1)
-grid = Grid(nx=200, ny=100, anisotropy=atrp)
+atpy = anisotropy_from_svg(r'assets/anicline.svg', beta=10, gamma=0.1)
+grid = Grid(nx=200, ny=100, anisotropy=atpy)
 ```
 
 Define SPDE and Simulate:
 ```
 sp = Spde(grid, sigma=1, a=25)
-Z_M = sp.simulate()
+Z = sp.simulate()
 ```
```

### Comparing `pyspde-0.0.3/README.md` & `pyspde-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,37 @@
 $$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \mathbb{R}^2
 $$
 
 The theory is proposed in Fuglstad (2014).
 
 ## Instalation
 
+On Debian/Ubuntu systems:
 ```
+sudo apt-get install libsuitesparse-dev
+pip install pyspde
+```
+
+On Windows systems:
+```
+conda install -c conda-forge suitesparse
 pip install pyspde
 ```
 
 ## Basic Usage
 
 Imports:
 ```
 from pyspde import anisotropy, Grid, Spde
 ```
 
 Define the anisotropy and the grid:
 ```
-atrp = anisotropy_from_svg(r'assets/anicline.svg', beta=10, gamma=0.1)
-grid = Grid(nx=200, ny=100, anisotropy=atrp)
+atpy = anisotropy_from_svg(r'assets/anicline.svg', beta=10, gamma=0.1)
+grid = Grid(nx=200, ny=100, anisotropy=atpy)
 ```
 
 Define SPDE and Simulate:
 ```
 sp = Spde(grid, sigma=1, a=25)
-Z_M = sp.simulate()
+Z = sp.simulate()
 ```
```

### Comparing `pyspde-0.0.3/pyproject.toml` & `pyspde-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyspde"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Esteban Jimenez", email="ejimenez@minerai.com.au" },
 ]
 description = "PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `pyspde-0.0.3/src/pyspde/anisotropy.py` & `pyspde-0.0.4/src/pyspde/anisotropy.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.3/src/pyspde/grid.py` & `pyspde-0.0.4/src/pyspde/grid.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.3/src/pyspde/neighbours.py` & `pyspde-0.0.4/src/pyspde/neighbours.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.3/src/pyspde/spde.py` & `pyspde-0.0.4/src/pyspde/spde.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.3/src/pyspde/utils.py` & `pyspde-0.0.4/src/pyspde/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import numpy as np
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import xml.etree.ElementTree as Et
 
-__all__ = ['imdict', 'map_2d_1d_nx_ny', 'map_1d_2d_nx', 'sample_grid',
-           'get_inkscape_transform', 'get_inkscape_namespace']
+__all__ = ['sample_grid']
 
 class imdict(dict):
     def __hash__(self) -> None:
         """Return the unique id of the object as its hash value."""
         return id(self)
 
     def _immutable(self, *args, **kws) -> None:
```

### Comparing `pyspde-0.0.3/src/pyspde.egg-info/PKG-INFO` & `pyspde-0.0.4/src/pyspde.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspde
-Version: 0.0.3
+Version: 0.0.4
 Summary: PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)
 Author-email: Esteban Jimenez <ejimenez@minerai.com.au>
 Project-URL: Homepage, https://github.com/M1nerAI/pyspde
 Project-URL: Issues, https://github.com/M1nerAI/pyspde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,29 +23,37 @@
 $$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \mathbb{R}^2
 $$
 
 The theory is proposed in Fuglstad (2014).
 
 ## Instalation
 
+On Debian/Ubuntu systems:
 ```
+sudo apt-get install libsuitesparse-dev
+pip install pyspde
+```
+
+On Windows systems:
+```
+conda install -c conda-forge suitesparse
 pip install pyspde
 ```
 
 ## Basic Usage
 
 Imports:
 ```
 from pyspde import anisotropy, Grid, Spde
 ```
 
 Define the anisotropy and the grid:
 ```
-atrp = anisotropy_from_svg(r'assets/anicline.svg', beta=10, gamma=0.1)
-grid = Grid(nx=200, ny=100, anisotropy=atrp)
+atpy = anisotropy_from_svg(r'assets/anicline.svg', beta=10, gamma=0.1)
+grid = Grid(nx=200, ny=100, anisotropy=atpy)
 ```
 
 Define SPDE and Simulate:
 ```
 sp = Spde(grid, sigma=1, a=25)
-Z_M = sp.simulate()
+Z = sp.simulate()
 ```
```

