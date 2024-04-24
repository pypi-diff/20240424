# Comparing `tmp/alaspo-0.2.5.tar.gz` & `tmp/alaspo-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alaspo-0.2.5.tar", last modified: Thu Jul  6 10:50:11 2023, max compression
+gzip compressed data, was "alaspo-0.2.6.tar", last modified: Wed Apr 24 12:50:56 2024, max compression
```

## Comparing `alaspo-0.2.5.tar` & `alaspo-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-07-06 10:50:11.288180 alaspo-0.2.5/
--rw-r--r--   0 tgeibing   (501) staff       (20)     1047 2023-02-06 12:44:36.000000 alaspo-0.2.5/LICENSE
--rw-r--r--   0 tgeibing   (501) staff       (20)     1381 2023-07-06 10:50:11.288056 alaspo-0.2.5/PKG-INFO
--rw-r--r--   0 tgeibing   (501) staff       (20)      988 2023-02-09 23:05:59.000000 alaspo-0.2.5/README.md
--rw-r--r--   0 tgeibing   (501) staff       (20)      615 2023-02-09 23:05:59.000000 alaspo-0.2.5/READMEPyPi.md
--rw-r--r--   0 tgeibing   (501) staff       (20)     1170 2023-02-24 15:58:56.000000 alaspo-0.2.5/pyproject.toml
--rw-r--r--   0 tgeibing   (501) staff       (20)       38 2023-07-06 10:50:11.288222 alaspo-0.2.5/setup.cfg
-drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-07-06 10:50:11.284202 alaspo-0.2.5/src/
-drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-07-06 10:50:11.287155 alaspo-0.2.5/src/alaspo/
--rw-r--r--   0 tgeibing   (501) staff       (20)       53 2023-02-06 12:44:36.000000 alaspo-0.2.5/src/alaspo/__init__.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     9044 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/__main__.py
--rw-r--r--   0 tgeibing   (501) staff       (20)       24 2023-07-06 10:49:02.000000 alaspo-0.2.5/src/alaspo/__version__.py
--rw-r--r--   0 tgeibing   (501) staff       (20)       51 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/config.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     2051 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/initial.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     1817 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/json_config.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     5450 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/lns.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     7612 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/relax.py
--rw-r--r--   0 tgeibing   (501) staff       (20)     3958 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/search.py
--rw-r--r--   0 tgeibing   (501) staff       (20)    17548 2023-07-06 10:49:02.000000 alaspo-0.2.5/src/alaspo/solver.py
--rw-r--r--   0 tgeibing   (501) staff       (20)    11401 2023-03-16 09:31:25.000000 alaspo-0.2.5/src/alaspo/strategy.py
-drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2023-07-06 10:50:11.287871 alaspo-0.2.5/src/alaspo.egg-info/
--rw-r--r--   0 tgeibing   (501) staff       (20)     1381 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/PKG-INFO
--rw-r--r--   0 tgeibing   (501) staff       (20)      496 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/SOURCES.txt
--rw-r--r--   0 tgeibing   (501) staff       (20)        1 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/dependency_links.txt
--rw-r--r--   0 tgeibing   (501) staff       (20)       48 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/entry_points.txt
--rw-r--r--   0 tgeibing   (501) staff       (20)       52 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/requires.txt
--rw-r--r--   0 tgeibing   (501) staff       (20)        7 2023-07-06 10:50:11.000000 alaspo-0.2.5/src/alaspo.egg-info/top_level.txt
+drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2024-04-24 12:50:56.543410 alaspo-0.2.6/
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1047 2023-02-06 12:44:36.000000 alaspo-0.2.6/LICENSE
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1493 2024-04-24 12:50:56.543209 alaspo-0.2.6/PKG-INFO
+-rw-r--r--   0 tgeibing   (501) staff       (20)      988 2023-02-09 23:05:59.000000 alaspo-0.2.6/README.md
+-rw-r--r--   0 tgeibing   (501) staff       (20)      615 2023-02-09 23:05:59.000000 alaspo-0.2.6/READMEPyPi.md
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1170 2023-02-24 15:58:56.000000 alaspo-0.2.6/pyproject.toml
+-rw-r--r--   0 tgeibing   (501) staff       (20)       38 2024-04-24 12:50:56.543452 alaspo-0.2.6/setup.cfg
+drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2024-04-24 12:50:56.538295 alaspo-0.2.6/src/
+drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2024-04-24 12:50:56.542063 alaspo-0.2.6/src/alaspo/
+-rw-r--r--   0 tgeibing   (501) staff       (20)       53 2023-02-06 12:44:36.000000 alaspo-0.2.6/src/alaspo/__init__.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     9044 2023-03-16 09:31:25.000000 alaspo-0.2.6/src/alaspo/__main__.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)       24 2024-04-24 12:47:33.000000 alaspo-0.2.6/src/alaspo/__version__.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)       51 2023-03-16 09:31:25.000000 alaspo-0.2.6/src/alaspo/config.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     2273 2024-04-24 12:47:33.000000 alaspo-0.2.6/src/alaspo/initial.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1817 2023-03-16 09:31:25.000000 alaspo-0.2.6/src/alaspo/json_config.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     5450 2023-03-16 09:31:25.000000 alaspo-0.2.6/src/alaspo/lns.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     7612 2023-03-16 09:31:25.000000 alaspo-0.2.6/src/alaspo/relax.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)     3958 2023-03-16 09:31:25.000000 alaspo-0.2.6/src/alaspo/search.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)    17548 2023-07-06 10:49:02.000000 alaspo-0.2.6/src/alaspo/solver.py
+-rw-r--r--   0 tgeibing   (501) staff       (20)    11401 2023-03-16 09:31:25.000000 alaspo-0.2.6/src/alaspo/strategy.py
+drwxr-xr-x   0 tgeibing   (501) staff       (20)        0 2024-04-24 12:50:56.543001 alaspo-0.2.6/src/alaspo.egg-info/
+-rw-r--r--   0 tgeibing   (501) staff       (20)     1493 2024-04-24 12:50:56.000000 alaspo-0.2.6/src/alaspo.egg-info/PKG-INFO
+-rw-r--r--   0 tgeibing   (501) staff       (20)      496 2024-04-24 12:50:56.000000 alaspo-0.2.6/src/alaspo.egg-info/SOURCES.txt
+-rw-r--r--   0 tgeibing   (501) staff       (20)        1 2024-04-24 12:50:56.000000 alaspo-0.2.6/src/alaspo.egg-info/dependency_links.txt
+-rw-r--r--   0 tgeibing   (501) staff       (20)       48 2024-04-24 12:50:56.000000 alaspo-0.2.6/src/alaspo.egg-info/entry_points.txt
+-rw-r--r--   0 tgeibing   (501) staff       (20)       52 2024-04-24 12:50:56.000000 alaspo-0.2.6/src/alaspo.egg-info/requires.txt
+-rw-r--r--   0 tgeibing   (501) staff       (20)        7 2024-04-24 12:50:56.000000 alaspo-0.2.6/src/alaspo.egg-info/top_level.txt
```

### Comparing `alaspo-0.2.5/LICENSE` & `alaspo-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/PKG-INFO` & `alaspo-0.2.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: alaspo
-Version: 0.2.5
+Version: 0.2.6
 Summary: ALASPO: ASP + Large-Neighborhood Search
 Author-email: Tobias Geibinger <tobias.geibinger@tuwien.ac.at>, Thomas Eiter <thomas.eiter@tuwien.ac.at>, Johannes Oetsch <johannes.oetsch@tuwien.ac.at>, Nelson Higuera Ruiz <nelson.ruiz@tuwien.ac.at>, Nysret Musliu <nysret.musliu@tuwien.ac.at>, Daria Stepanova <daria.stepanova@de.bosch.com>
 Project-URL: Homepage, https://gitlab.tuwien.ac.at/kbs/BAI/alaspo
 Project-URL: Bug Tracker, https://gitlab.tuwien.ac.at/kbs/BAI/alaspo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cffi>=1.15
+Requires-Dist: clingo>=5.6
+Requires-Dist: clingo-dl>=1.4
+Requires-Dist: clingcon>=5.2
 
 # ALASPO
 
 An (adaptive) LNS framework for the for ASP systems. Currently, the system only supports solvers based on [clingo](https://potassco.org/). 
 
 ## Installation
```

### Comparing `alaspo-0.2.5/README.md` & `alaspo-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/READMEPyPi.md` & `alaspo-0.2.6/READMEPyPi.md`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/pyproject.toml` & `alaspo-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/src/alaspo/__main__.py` & `alaspo-0.2.6/src/alaspo/__main__.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/src/alaspo/initial.py` & `alaspo-0.2.6/src/alaspo/initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-import math
 from .__init__ import logger
 
 
 class AbstractInititalOperator:
 
     def construct(self, global_timeout):
         """construct the initial solution used for lns
@@ -33,18 +31,22 @@
         self.__configuration = configuration
         self.__pre_opt_time = pre_opt_time
 
     def construct(self, global_timeout):
         logger.debug('initial operator executing')
         if self.__pre_opt_time > 0:
             if type(self.__pre_opt_time) == float:
-                t = math.round(global_timeout * self.__pre_opt_time)
+                t = round(global_timeout * self.__pre_opt_time)
             else:
                 t = self.__pre_opt_time
-            return self.__internal_solver.solve(timelimit=min(t, global_timeout), configuration=self.__configuration)
+            res = self.__internal_solver.solve(timelimit=min(t, global_timeout), configuration=self.__configuration)
+            if not res.sat:
+                time_left = global_timeout - min(t, global_timeout)
+                res = self.__internal_solver.solve(timelimit=time_left, configuration=self.__configuration, modellimit=1)
+            return res
         else:
             return self.__internal_solver.solve(timelimit=global_timeout, configuration=self.__configuration, modellimit=1)
 
 
 # InitialOperator Factory
 
 def get_operator(args, internal_solver):
```

### Comparing `alaspo-0.2.5/src/alaspo/json_config.py` & `alaspo-0.2.6/src/alaspo/json_config.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/src/alaspo/lns.py` & `alaspo-0.2.6/src/alaspo/lns.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/src/alaspo/relax.py` & `alaspo-0.2.6/src/alaspo/relax.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/src/alaspo/search.py` & `alaspo-0.2.6/src/alaspo/search.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/src/alaspo/solver.py` & `alaspo-0.2.6/src/alaspo/solver.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/src/alaspo/strategy.py` & `alaspo-0.2.6/src/alaspo/strategy.py`

 * *Files identical despite different names*

### Comparing `alaspo-0.2.5/src/alaspo.egg-info/PKG-INFO` & `alaspo-0.2.6/src/alaspo.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: alaspo
-Version: 0.2.5
+Version: 0.2.6
 Summary: ALASPO: ASP + Large-Neighborhood Search
 Author-email: Tobias Geibinger <tobias.geibinger@tuwien.ac.at>, Thomas Eiter <thomas.eiter@tuwien.ac.at>, Johannes Oetsch <johannes.oetsch@tuwien.ac.at>, Nelson Higuera Ruiz <nelson.ruiz@tuwien.ac.at>, Nysret Musliu <nysret.musliu@tuwien.ac.at>, Daria Stepanova <daria.stepanova@de.bosch.com>
 Project-URL: Homepage, https://gitlab.tuwien.ac.at/kbs/BAI/alaspo
 Project-URL: Bug Tracker, https://gitlab.tuwien.ac.at/kbs/BAI/alaspo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cffi>=1.15
+Requires-Dist: clingo>=5.6
+Requires-Dist: clingo-dl>=1.4
+Requires-Dist: clingcon>=5.2
 
 # ALASPO
 
 An (adaptive) LNS framework for the for ASP systems. Currently, the system only supports solvers based on [clingo](https://potassco.org/). 
 
 ## Installation
```

