# Comparing `tmp/revpref-1.0.0.tar.gz` & `tmp/revpref-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revpref-1.0.0.tar", last modified: Tue Apr 23 09:54:16 2024, max compression
+gzip compressed data, was "revpref-1.0.1.tar", last modified: Tue Apr 23 12:07:40 2024, max compression
```

## Comparing `revpref-1.0.0.tar` & `revpref-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-23 09:54:16.354067 revpref-1.0.0/
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     5378 2024-04-23 09:54:16.353840 revpref-1.0.0/PKG-INFO
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     4808 2024-04-23 09:23:51.000000 revpref-1.0.0/README.md
--rw-r--r--   0 aliebcxiang   (501) staff       (20)      582 2024-04-23 09:53:56.000000 revpref-1.0.0/pyproject.toml
-drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-23 09:54:16.352181 revpref-1.0.0/revpref/
--rw-r--r--   0 aliebcxiang   (501) staff       (20)      113 2024-04-21 16:08:26.000000 revpref-1.0.0/revpref/__init__.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     1534 2024-04-23 06:18:25.000000 revpref-1.0.0/revpref/_legacy.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     1836 2024-04-23 08:28:55.000000 revpref-1.0.0/revpref/_utils.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     1955 2024-04-23 06:28:47.000000 revpref-1.0.0/revpref/avi.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     3001 2024-04-23 04:29:49.000000 revpref-1.0.0/revpref/ccei.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     5371 2024-04-23 06:12:12.000000 revpref-1.0.0/revpref/garp.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     5243 2024-04-23 06:30:08.000000 revpref-1.0.0/revpref/hmi.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     4408 2024-04-23 06:50:42.000000 revpref-1.0.0/revpref/mci.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     2363 2024-04-23 06:25:50.000000 revpref-1.0.0/revpref/mpi.py
-drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-23 09:54:16.353485 revpref-1.0.0/revpref.egg-info/
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     5378 2024-04-23 09:54:16.000000 revpref-1.0.0/revpref.egg-info/PKG-INFO
--rw-r--r--   0 aliebcxiang   (501) staff       (20)      336 2024-04-23 09:54:16.000000 revpref-1.0.0/revpref.egg-info/SOURCES.txt
--rw-r--r--   0 aliebcxiang   (501) staff       (20)        1 2024-04-23 09:54:16.000000 revpref-1.0.0/revpref.egg-info/dependency_links.txt
--rw-r--r--   0 aliebcxiang   (501) staff       (20)       37 2024-04-23 09:54:16.000000 revpref-1.0.0/revpref.egg-info/requires.txt
--rw-r--r--   0 aliebcxiang   (501) staff       (20)        8 2024-04-23 09:54:16.000000 revpref-1.0.0/revpref.egg-info/top_level.txt
--rw-r--r--   0 aliebcxiang   (501) staff       (20)       38 2024-04-23 09:54:16.354113 revpref-1.0.0/setup.cfg
--rw-r--r--   0 aliebcxiang   (501) staff       (20)      473 2024-04-23 07:01:08.000000 revpref-1.0.0/setup.py
+drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-23 12:07:40.914782 revpref-1.0.1/
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     5405 2024-04-23 12:07:40.914563 revpref-1.0.1/PKG-INFO
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     4823 2024-04-23 12:00:21.000000 revpref-1.0.1/README.md
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)      601 2024-04-23 12:01:04.000000 revpref-1.0.1/pyproject.toml
+drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-23 12:07:40.909253 revpref-1.0.1/revpref/
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)      113 2024-04-21 16:08:26.000000 revpref-1.0.1/revpref/__init__.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     1534 2024-04-23 06:18:25.000000 revpref-1.0.1/revpref/_legacy.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     1836 2024-04-23 08:28:55.000000 revpref-1.0.1/revpref/_utils.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     1955 2024-04-23 06:28:47.000000 revpref-1.0.1/revpref/avi.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     3001 2024-04-23 11:59:47.000000 revpref-1.0.1/revpref/ccei.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     5371 2024-04-23 11:59:32.000000 revpref-1.0.1/revpref/garp.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     5243 2024-04-23 06:30:08.000000 revpref-1.0.1/revpref/hmi.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     4408 2024-04-23 06:50:42.000000 revpref-1.0.1/revpref/mci.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     2363 2024-04-23 06:25:50.000000 revpref-1.0.1/revpref/mpi.py
+drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-23 12:07:40.914311 revpref-1.0.1/revpref.egg-info/
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     5405 2024-04-23 12:07:40.000000 revpref-1.0.1/revpref.egg-info/PKG-INFO
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)      336 2024-04-23 12:07:40.000000 revpref-1.0.1/revpref.egg-info/SOURCES.txt
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)        1 2024-04-23 12:07:40.000000 revpref-1.0.1/revpref.egg-info/dependency_links.txt
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)       49 2024-04-23 12:07:40.000000 revpref-1.0.1/revpref.egg-info/requires.txt
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)        8 2024-04-23 12:07:40.000000 revpref-1.0.1/revpref.egg-info/top_level.txt
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)       38 2024-04-23 12:07:40.914828 revpref-1.0.1/setup.cfg
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)      473 2024-04-23 07:01:08.000000 revpref-1.0.1/setup.py
```

### Comparing `revpref-1.0.0/PKG-INFO` & `revpref-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: revpref
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Tools for Computational Revealed Preference Analysis
 Home-page: https://github.com/Aliebc/revpref
 Author: Yi Xiang
 Author-email: Yi Xiang <xiangy.i@outlook.com>
 Project-URL: Homepage, https://github.com/Aliebc/revpref
 Project-URL: Bug Tracker, https://github.com/Aliebc/revpref
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: networkx
-Requires-Dist: pulp
-Requires-Dist: scipy
+Requires-Dist: pulp>=2.6.0
+Requires-Dist: scipy>1.10
 Requires-Dist: matplotlib
 
 # revpref
 
 Python Tools for Computational Revealed Preference Analysis
 
 ## Synopsis
@@ -30,15 +30,15 @@
 
 We implement various method to compute following indices:
 
 CCEI (Critical Cost Efficiency index, *Afrait 1972*)
 
 * CCEI (also known as the Afriat efficiency index). The CCEI is defined as the maximal value of the efficiency level e at which the data set is consistent with GARP.
 * Generally, A is directly prefered to B when $p^Aq^A>p^Aq^B$, and CCEI is the suprema of e under constraint $e p^Aq^A>p^Aq^B$ to satisfy GARP .
-* We provide three method to compute CCEI. (Warshall, MTZ and dichotomy)
+* We provide three method to compute CCEI. (Warshall, MTZ and bisection)
 
 HMI (Houtman and Maks index, *Houtman and Maks, 1985*)
 
 * The Houtman-Maks index gives the relative size of the largest subset of observations that is still consistent with GARP.
 * For instance, if we delete the tenth choice from a 10-choice dataset and find it satisfy GARP, then the HMI is (10 - 1)/10 = 0.9
 * We provide two methods to compute CCEI. (GrossKaiser, MTZ)
 
@@ -81,15 +81,15 @@
 numpy, scipy, networkx and pulp are needed.
 
 ## Example
 
 Below we provide some simple examples to illustrate the main class in our package.
 
 ```python
-import revpref as rp
+bisectionimport revpref as rp
 import numpy as np
 
 p = np.array(
     [[4, 4, 4], 
      [1, 9, 3], 
      [2, 8, 3], 
      [1, 8, 4], 
@@ -115,15 +115,15 @@
 )
 
 pref = rp.RevealedPreference(p, q) # Construct the class
 print(pref.check_garp()) # Check if satisfy GARP
 
 print("---CCEI---")
 print(pref.ccei()) # Compute the CCEI
-print(pref.ccei(method='dichotomy', tol = 1e-10))
+print(pref.ccei(method='bisection', tol = 1e-10))
 print(pref.ccei(method='mtz')) # Use other methods
 
 print("---AVI---")
 print(pref.avi())
 
 print("---MPI---")
 print(pref.mpi())
@@ -159,19 +159,19 @@
 ---HMI---
 0.9
 0.9
 ```
 
 ## Reference
 
-[1]  Afriat, Sidney N."Efficiency estimation of production functions."International economic review (1972): 568-598.
+[1]  Afriat, Sidney N."Efficiency estimation of production functions."*International economic review* (1972): 568-598.
 
-[2]  Houtman, Martijn, and Julian Maks. "Determining all maximal data subsets consistent with revealed preference." Kwantitatieve methoden 19, no. 1 (1985): 89-104.
+[2]  Houtman, Martijn, and Julian Maks. "Determining all maximal data subsets consistent with revealed preference." *Kwantitatieve methoden* 19, no. 1 (1985): 89-104.
 
-[3]  Varian, Hal R. "Goodness-of-fit in optimizing models." Journal of Econometrics 46, no. 1-2 (1990): 125-140. 
+[3]  Varian, Hal R. "Goodness-of-fit in optimizing models." *Journal of Econometrics* 46, no. 1-2 (1990): 125-140. 
 
 [4]  Echenique, Federico, Sangmok Lee, and Matthew Shum. "The money pump as a measure of revealed preference violations." Journal of Political Economy 119, no. 6 (2011): 1201-1223.
 
 [5]  Dean, Mark, and Daniel Martin. "Measuring rationality with the minimum cost of revealed preference violations." Review of Economics and Statistics 98, no. 3 (2016): 524-534.
 
 [6]  Demuynck, Thomas, and John Rehbeck. "Computing revealed preference goodness-of-fit measures with integer programming." *Economic Theory* 76, no. 4 (2023): 1175-1195.
```

### Comparing `revpref-1.0.0/README.md` & `revpref-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 We implement various method to compute following indices:
 
 CCEI (Critical Cost Efficiency index, *Afrait 1972*)
 
 * CCEI (also known as the Afriat efficiency index). The CCEI is defined as the maximal value of the efficiency level e at which the data set is consistent with GARP.
 * Generally, A is directly prefered to B when $p^Aq^A>p^Aq^B$, and CCEI is the suprema of e under constraint $e p^Aq^A>p^Aq^B$ to satisfy GARP .
-* We provide three method to compute CCEI. (Warshall, MTZ and dichotomy)
+* We provide three method to compute CCEI. (Warshall, MTZ and bisection)
 
 HMI (Houtman and Maks index, *Houtman and Maks, 1985*)
 
 * The Houtman-Maks index gives the relative size of the largest subset of observations that is still consistent with GARP.
 * For instance, if we delete the tenth choice from a 10-choice dataset and find it satisfy GARP, then the HMI is (10 - 1)/10 = 0.9
 * We provide two methods to compute CCEI. (GrossKaiser, MTZ)
 
@@ -63,15 +63,15 @@
 numpy, scipy, networkx and pulp are needed.
 
 ## Example
 
 Below we provide some simple examples to illustrate the main class in our package.
 
 ```python
-import revpref as rp
+bisectionimport revpref as rp
 import numpy as np
 
 p = np.array(
     [[4, 4, 4], 
      [1, 9, 3], 
      [2, 8, 3], 
      [1, 8, 4], 
@@ -97,15 +97,15 @@
 )
 
 pref = rp.RevealedPreference(p, q) # Construct the class
 print(pref.check_garp()) # Check if satisfy GARP
 
 print("---CCEI---")
 print(pref.ccei()) # Compute the CCEI
-print(pref.ccei(method='dichotomy', tol = 1e-10))
+print(pref.ccei(method='bisection', tol = 1e-10))
 print(pref.ccei(method='mtz')) # Use other methods
 
 print("---AVI---")
 print(pref.avi())
 
 print("---MPI---")
 print(pref.mpi())
@@ -141,19 +141,19 @@
 ---HMI---
 0.9
 0.9
 ```
 
 ## Reference
 
-[1]  Afriat, Sidney N."Efficiency estimation of production functions."International economic review (1972): 568-598.
+[1]  Afriat, Sidney N."Efficiency estimation of production functions."*International economic review* (1972): 568-598.
 
-[2]  Houtman, Martijn, and Julian Maks. "Determining all maximal data subsets consistent with revealed preference." Kwantitatieve methoden 19, no. 1 (1985): 89-104.
+[2]  Houtman, Martijn, and Julian Maks. "Determining all maximal data subsets consistent with revealed preference." *Kwantitatieve methoden* 19, no. 1 (1985): 89-104.
 
-[3]  Varian, Hal R. "Goodness-of-fit in optimizing models." Journal of Econometrics 46, no. 1-2 (1990): 125-140. 
+[3]  Varian, Hal R. "Goodness-of-fit in optimizing models." *Journal of Econometrics* 46, no. 1-2 (1990): 125-140. 
 
 [4]  Echenique, Federico, Sangmok Lee, and Matthew Shum. "The money pump as a measure of revealed preference violations." Journal of Political Economy 119, no. 6 (2011): 1201-1223.
 
 [5]  Dean, Mark, and Daniel Martin. "Measuring rationality with the minimum cost of revealed preference violations." Review of Economics and Statistics 98, no. 3 (2016): 524-534.
 
 [6]  Demuynck, Thomas, and John Rehbeck. "Computing revealed preference goodness-of-fit measures with integer programming." *Economic Theory* 76, no. 4 (2023): 1175-1195.
```

### Comparing `revpref-1.0.0/pyproject.toml` & `revpref-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "revpref"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {"name" = "Yi Xiang", "email" = "xiangy.i@outlook.com"}
 ]
 description = "Python Tools for Computational Revealed Preference Analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
-dependencies = ["numpy", "networkx", "pulp", "scipy", "matplotlib"]
+dependencies = ["numpy", "networkx", "pulp>=2.6.0", "scipy>1.10", "matplotlib"]
 
 [project.urls]
 "Homepage" = "https://github.com/Aliebc/revpref"
 "Bug Tracker" = "https://github.com/Aliebc/revpref"
 
 [build-system]
-requires = ["setuptools", "numpy", "networkx", "pulp", "scipy", "matplotlib"]
+requires = ["setuptools", "numpy", "networkx", "pulp>=2.6.0", "scipy", "matplotlib"]
```

### Comparing `revpref-1.0.0/revpref/_legacy.py` & `revpref-1.0.1/revpref/_legacy.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.0/revpref/_utils.py` & `revpref-1.0.1/revpref/_utils.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.0/revpref/avi.py` & `revpref-1.0.1/revpref/avi.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.0/revpref/ccei.py` & `revpref-1.0.1/revpref/ccei.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,17 @@
             for i in range(len(Cs)):
                 Es[i, j] = max(min(
                     max(Es[i, k],0), max(Es[k, j],0)
                 ), Es[i, j])
     
     return 1 - max(np.diag(Es))
 
-def _dichotomy_ccei(p: np.ndarray, q: np.ndarray, tol = 1e-6):
+def _bisection_ccei(p: np.ndarray, q: np.ndarray, tol = 1e-6):
     '''
-    Dichotomy algorithm for CCEI
+    bisection algorithm for CCEI
     
     This method is the most standard way to calculate CCEI.
     '''
     f = lambda iccei, p, q: _has_cycle(_generate_graph(p, q, iccei))
     l, r = 0, 1
     while r - l > tol:
         mid = (l + r) / 2
@@ -105,11 +105,11 @@
     prob.solve(solver = sl)
     e = pl.value(prob.objective) 
     
     return e
 
 ###########################
 ccei_warshall = _warshall_ccei
-ccei_dichotomy = _dichotomy_ccei
+ccei_bisection = _bisection_ccei
 ccei_mtz = _mtz_ccei
 
-__all__ = ['ccei_warshall', 'ccei_dichotomy', 'ccei_mtz']
+__all__ = ['ccei_warshall', 'ccei_bisection', 'ccei_mtz']
```

### Comparing `revpref-1.0.0/revpref/garp.py` & `revpref-1.0.1/revpref/garp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __author__ = 'Yi Xiang'
 
 import networkx as nx
 import numpy as np
 from typing import List, Tuple, Literal
 from matplotlib import pyplot as plt
 
 from ._utils import generate_graph
 
-from .ccei import _warshall_ccei, _dichotomy_ccei, _mtz_ccei
+from .ccei import _warshall_ccei, _bisection_ccei, _mtz_ccei
 from .mpi import _cycle_mpi, _matrix_mpi
 from .mci import _mtz_mci, _optimize_mci, _milp_mci
 from .hmi import _mtz_hmi, _gross_hmi
 from .avi import _mtz_avi
 
 def _generate_graph(p, q, e = 1):
     return generate_graph(p, q, e)
@@ -68,25 +68,25 @@
     ):
         '''
         CCEI (Critical Cost Efficiency Index)
         -- Afriat (1972)
         
         Our package provides three methods to calculate CCEI:
         1. Warshall Algorithm (default, suggested)
-        2. Dichotomy
+        2. Bisection
         3. MTZ
         '''
         match method:
             case 'warshall':
                 return _warshall_ccei(self.p, self.q)
-            case 'dichotomy':
-                return _dichotomy_ccei(self.p, self.q, tol)
+            case 'bisection':
+                return _bisection_ccei(self.p, self.q, tol)
             case 'mtz':
                 return _mtz_ccei(self.p, self.q, lp_solver)
-        raise ValueError("method should be 'warshall' or 'dichotomy' or 'mtz'")
+        raise ValueError("method should be 'warshall' or 'bisection' or 'mtz'")
     
     def avi(self, 
         method : Literal['mtz'] = 'mtz',
         lp_solver : Literal[
             'GUROBI_CMD', 'PULP_CBC_CMD', 'COIN_CMD',
             'CPLEX_CMD', 'GLPK_CMD', 'XPRESS', 'CPLEX_PY'
         ] = 'PULP_CBC_CMD'
```

### Comparing `revpref-1.0.0/revpref/hmi.py` & `revpref-1.0.1/revpref/hmi.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.0/revpref/mci.py` & `revpref-1.0.1/revpref/mci.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.0/revpref/mpi.py` & `revpref-1.0.1/revpref/mpi.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.0/revpref.egg-info/PKG-INFO` & `revpref-1.0.1/revpref.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: revpref
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Tools for Computational Revealed Preference Analysis
 Home-page: https://github.com/Aliebc/revpref
 Author: Yi Xiang
 Author-email: Yi Xiang <xiangy.i@outlook.com>
 Project-URL: Homepage, https://github.com/Aliebc/revpref
 Project-URL: Bug Tracker, https://github.com/Aliebc/revpref
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: networkx
-Requires-Dist: pulp
-Requires-Dist: scipy
+Requires-Dist: pulp>=2.6.0
+Requires-Dist: scipy>1.10
 Requires-Dist: matplotlib
 
 # revpref
 
 Python Tools for Computational Revealed Preference Analysis
 
 ## Synopsis
@@ -30,15 +30,15 @@
 
 We implement various method to compute following indices:
 
 CCEI (Critical Cost Efficiency index, *Afrait 1972*)
 
 * CCEI (also known as the Afriat efficiency index). The CCEI is defined as the maximal value of the efficiency level e at which the data set is consistent with GARP.
 * Generally, A is directly prefered to B when $p^Aq^A>p^Aq^B$, and CCEI is the suprema of e under constraint $e p^Aq^A>p^Aq^B$ to satisfy GARP .
-* We provide three method to compute CCEI. (Warshall, MTZ and dichotomy)
+* We provide three method to compute CCEI. (Warshall, MTZ and bisection)
 
 HMI (Houtman and Maks index, *Houtman and Maks, 1985*)
 
 * The Houtman-Maks index gives the relative size of the largest subset of observations that is still consistent with GARP.
 * For instance, if we delete the tenth choice from a 10-choice dataset and find it satisfy GARP, then the HMI is (10 - 1)/10 = 0.9
 * We provide two methods to compute CCEI. (GrossKaiser, MTZ)
 
@@ -81,15 +81,15 @@
 numpy, scipy, networkx and pulp are needed.
 
 ## Example
 
 Below we provide some simple examples to illustrate the main class in our package.
 
 ```python
-import revpref as rp
+bisectionimport revpref as rp
 import numpy as np
 
 p = np.array(
     [[4, 4, 4], 
      [1, 9, 3], 
      [2, 8, 3], 
      [1, 8, 4], 
@@ -115,15 +115,15 @@
 )
 
 pref = rp.RevealedPreference(p, q) # Construct the class
 print(pref.check_garp()) # Check if satisfy GARP
 
 print("---CCEI---")
 print(pref.ccei()) # Compute the CCEI
-print(pref.ccei(method='dichotomy', tol = 1e-10))
+print(pref.ccei(method='bisection', tol = 1e-10))
 print(pref.ccei(method='mtz')) # Use other methods
 
 print("---AVI---")
 print(pref.avi())
 
 print("---MPI---")
 print(pref.mpi())
@@ -159,19 +159,19 @@
 ---HMI---
 0.9
 0.9
 ```
 
 ## Reference
 
-[1]  Afriat, Sidney N."Efficiency estimation of production functions."International economic review (1972): 568-598.
+[1]  Afriat, Sidney N."Efficiency estimation of production functions."*International economic review* (1972): 568-598.
 
-[2]  Houtman, Martijn, and Julian Maks. "Determining all maximal data subsets consistent with revealed preference." Kwantitatieve methoden 19, no. 1 (1985): 89-104.
+[2]  Houtman, Martijn, and Julian Maks. "Determining all maximal data subsets consistent with revealed preference." *Kwantitatieve methoden* 19, no. 1 (1985): 89-104.
 
-[3]  Varian, Hal R. "Goodness-of-fit in optimizing models." Journal of Econometrics 46, no. 1-2 (1990): 125-140. 
+[3]  Varian, Hal R. "Goodness-of-fit in optimizing models." *Journal of Econometrics* 46, no. 1-2 (1990): 125-140. 
 
 [4]  Echenique, Federico, Sangmok Lee, and Matthew Shum. "The money pump as a measure of revealed preference violations." Journal of Political Economy 119, no. 6 (2011): 1201-1223.
 
 [5]  Dean, Mark, and Daniel Martin. "Measuring rationality with the minimum cost of revealed preference violations." Review of Economics and Statistics 98, no. 3 (2016): 524-534.
 
 [6]  Demuynck, Thomas, and John Rehbeck. "Computing revealed preference goodness-of-fit measures with integer programming." *Economic Theory* 76, no. 4 (2023): 1175-1195.
```

