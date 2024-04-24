# Comparing `tmp/pyspde-0.0.1.tar.gz` & `tmp/pyspde-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspde-0.0.1.tar", last modified: Tue Apr 23 22:54:11 2024, max compression
+gzip compressed data, was "pyspde-0.0.2.tar", last modified: Tue Apr 23 23:38:12 2024, max compression
```

## Comparing `pyspde-0.0.1.tar` & `pyspde-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 22:54:11.064204 pyspde-0.0.1/
--rw-rw-rw-   0        0        0     1085 2024-04-09 03:25:05.000000 pyspde-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1454 2024-04-23 22:54:11.064204 pyspde-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      758 2024-04-12 05:39:27.000000 pyspde-0.0.1/README.md
--rw-rw-rw-   0        0        0     1181 2024-04-23 22:54:01.000000 pyspde-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 22:54:11.064204 pyspde-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-23 22:54:11.047881 pyspde-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 22:54:11.053194 pyspde-0.0.1/src/pyspde/
--rw-rw-rw-   0        0        0       69 2024-04-11 06:43:36.000000 pyspde-0.0.1/src/pyspde/__init__.py
--rw-rw-rw-   0        0        0     8686 2024-04-23 00:07:28.000000 pyspde-0.0.1/src/pyspde/anisotropy.py
--rw-rw-rw-   0        0        0     4632 2024-04-23 00:01:53.000000 pyspde-0.0.1/src/pyspde/grid.py
--rw-rw-rw-   0        0        0     3606 2024-04-23 06:08:32.000000 pyspde-0.0.1/src/pyspde/neighbours.py
--rw-rw-rw-   0        0        0    10608 2024-04-23 06:10:05.000000 pyspde-0.0.1/src/pyspde/spde.py
--rw-rw-rw-   0        0        0     5013 2024-04-23 06:10:05.000000 pyspde-0.0.1/src/pyspde/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 22:54:11.063205 pyspde-0.0.1/src/pyspde.egg-info/
--rw-rw-rw-   0        0        0     1454 2024-04-23 22:54:11.000000 pyspde-0.0.1/src/pyspde.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-04-23 22:54:11.000000 pyspde-0.0.1/src/pyspde.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 22:54:11.000000 pyspde-0.0.1/src/pyspde.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 22:54:11.000000 pyspde-0.0.1/src/pyspde.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 23:38:12.923477 pyspde-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2024-04-09 03:25:05.000000 pyspde-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1563 2024-04-23 23:38:12.923477 pyspde-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2024-04-23 23:20:23.000000 pyspde-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1190 2024-04-23 23:37:01.000000 pyspde-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 23:38:12.923477 pyspde-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 23:38:12.912465 pyspde-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 23:38:12.917475 pyspde-0.0.2/src/pyspde/
+-rw-rw-rw-   0        0        0       69 2024-04-11 06:43:36.000000 pyspde-0.0.2/src/pyspde/__init__.py
+-rw-rw-rw-   0        0        0     8686 2024-04-23 00:07:28.000000 pyspde-0.0.2/src/pyspde/anisotropy.py
+-rw-rw-rw-   0        0        0     4632 2024-04-23 00:01:53.000000 pyspde-0.0.2/src/pyspde/grid.py
+-rw-rw-rw-   0        0        0     3606 2024-04-23 06:08:32.000000 pyspde-0.0.2/src/pyspde/neighbours.py
+-rw-rw-rw-   0        0        0    10608 2024-04-23 06:10:05.000000 pyspde-0.0.2/src/pyspde/spde.py
+-rw-rw-rw-   0        0        0     5013 2024-04-23 06:10:05.000000 pyspde-0.0.2/src/pyspde/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 23:38:12.922477 pyspde-0.0.2/src/pyspde.egg-info/
+-rw-rw-rw-   0        0        0     1563 2024-04-23 23:38:12.000000 pyspde-0.0.2/src/pyspde.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-04-23 23:38:12.000000 pyspde-0.0.2/src/pyspde.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 23:38:12.000000 pyspde-0.0.2/src/pyspde.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-23 23:38:12.000000 pyspde-0.0.2/src/pyspde.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 23:38:12.000000 pyspde-0.0.2/src/pyspde.egg-info/top_level.txt
```

### Comparing `pyspde-0.0.1/LICENSE` & `pyspde-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.1/PKG-INFO` & `pyspde-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: pyspde
-Version: 0.0.1
+Version: 0.0.2
 Summary: PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)
 Author-email: Esteban Jimenez <ejimenez@minerai.com.au>
 Project-URL: Homepage, https://github.com/M1nerAI/pyspde
 Project-URL: Issues, https://github.com/M1nerAI/pyspde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scikit-sparse
 
 # PySPDE
 
 PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs):
 
-$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \R^2
+$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \mathbb{R}^2
 $$
 
 The theory is proposed in Fuglstad (2014).
 
 ## Instalation
 
 ```
```

### Comparing `pyspde-0.0.1/README.md` & `pyspde-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PySPDE
 
 PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs):
 
-$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \R^2
+$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \mathbb{R}^2
 $$
 
 The theory is proposed in Fuglstad (2014).
 
 ## Instalation
 
 ```
```

### Comparing `pyspde-0.0.1/pyproject.toml` & `pyspde-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
-requires = ["setuptools>=61.0", "scipy", "numpy", "matplotlib", "scikit-sparse==0.4.12"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyspde"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Esteban Jimenez", email="ejimenez@minerai.com.au" },
 ]
 description = "PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = ["scipy", "numpy", "matplotlib", "scikit-sparse"]
 
 [project.urls]
 Homepage = "https://github.com/M1nerAI/pyspde"
 Issues = "https://github.com/M1nerAI/pyspde/issues"
 
 
 [tool.ruff.lint]
```

### Comparing `pyspde-0.0.1/src/pyspde/anisotropy.py` & `pyspde-0.0.2/src/pyspde/anisotropy.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.1/src/pyspde/grid.py` & `pyspde-0.0.2/src/pyspde/grid.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.1/src/pyspde/neighbours.py` & `pyspde-0.0.2/src/pyspde/neighbours.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.1/src/pyspde/spde.py` & `pyspde-0.0.2/src/pyspde/spde.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.1/src/pyspde/utils.py` & `pyspde-0.0.2/src/pyspde/utils.py`

 * *Files identical despite different names*

### Comparing `pyspde-0.0.1/src/pyspde.egg-info/PKG-INFO` & `pyspde-0.0.2/src/pyspde.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: pyspde
-Version: 0.0.1
+Version: 0.0.2
 Summary: PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs)
 Author-email: Esteban Jimenez <ejimenez@minerai.com.au>
 Project-URL: Homepage, https://github.com/M1nerAI/pyspde
 Project-URL: Issues, https://github.com/M1nerAI/pyspde/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scipy
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scikit-sparse
 
 # PySPDE
 
 PySPDE is a Python library for performing simulations and kriging of non-stationary spatial gaussian random fields with Matérn covariance, by solving the following Stochastic Partial Differential Equations (SPDEs):
 
-$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \R^2
+$$ ({\kappa}^2 - {\nabla} {\cdot} H(x) {\nabla} )Z(x) = {\tau}W(x) \quad x \in \mathbb{R}^2
 $$
 
 The theory is proposed in Fuglstad (2014).
 
 ## Instalation
 
 ```
```
