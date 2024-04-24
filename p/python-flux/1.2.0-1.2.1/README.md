# Comparing `tmp/python_flux-1.2.0.tar.gz` & `tmp/python_flux-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.2.0.tar", max compression
+gzip compressed data, was "python_flux-1.2.1.tar", max compression
```

## Comparing `python_flux-1.2.0.tar` & `python_flux-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7482 2024-04-23 04:13:01.727984 python_flux-1.2.0/README.rst
--rw-r--r--   0        0        0      741 2024-04-24 15:26:03.777873 python_flux-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.2.0/python_flux/__init__.py
--rw-r--r--   0        0        0    21695 2024-04-24 15:25:21.522783 python_flux-1.2.0/python_flux/flux.py
--rw-r--r--   0        0        0      759 2024-04-22 18:08:07.620526 python_flux-1.2.0/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1596 2024-04-18 05:35:27.173339 python_flux-1.2.0/python_flux/producers.py
--rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.2.0/python_flux/subscribers.py
--rw-r--r--   0        0        0     8213 1970-01-01 00:00:00.000000 python_flux-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7482 2024-04-23 04:13:01.727984 python_flux-1.2.1/README.rst
+-rw-r--r--   0        0        0      741 2024-04-24 15:44:14.465401 python_flux-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.2.1/python_flux/__init__.py
+-rw-r--r--   0        0        0    21700 2024-04-24 15:44:05.021620 python_flux-1.2.1/python_flux/flux.py
+-rw-r--r--   0        0        0      759 2024-04-22 18:08:07.620526 python_flux-1.2.1/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1596 2024-04-18 05:35:27.173339 python_flux-1.2.1/python_flux/producers.py
+-rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.2.1/python_flux/subscribers.py
+-rw-r--r--   0        0        0     8213 1970-01-01 00:00:00.000000 python_flux-1.2.1/PKG-INFO
```

### Comparing `python_flux-1.2.0/README.rst` & `python_flux-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `python_flux-1.2.0/pyproject.toml` & `python_flux-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.2.0"
+version = "1.2.1"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `python_flux-1.2.0/python_flux/flux.py` & `python_flux-1.2.1/python_flux/flux.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,16 +388,16 @@
         self.e = None
         self.ctx = None
 
     def execute(self, prepare_next, next, context):
         self.value, self.e, self.ctx = next(context)
         prepare_next()
         time.sleep(randint(1, 3))
-        sys.stdout.write(f'get: {self.id} {self.value}\n')
-        sys.stdout.flush()
+        #sys.stdout.write(f'get: {self.id} {self.value}\n')
+        #sys.stdout.flush()
 
 
 class FParallel(Stream):
     def __init__(self, pool, flux):
         super().__init__(flux)
         self.pool_size = pool
         self.jobs = {}
@@ -419,29 +419,29 @@
             jobs = self.pool.copy()
             for i, t in jobs.items():
                 try:
                     t.join(0.001)
                     if t.is_alive():
                         continue
                     else:
-                        print(f'pop {i}')
+                        #print(f'pop {i}')
                         self.pool.pop(i)
                         r = self.jobs.pop(i)
                         ctx = merge(ctx, r.ctx)
                         if isinstance(r.e, StopIteration):
-                            print('StopIteration')
+                            #print('StopIteration')
                             self.waiting_to_stop = True
                             if len(self.pool) == 0:
                                 return None, StopIteration(), ctx
                             else:
                                 continue
                         if self.waiting_to_stop:
                             if len(self.pool) == 0:
                                 return None, StopIteration(), ctx
-                        print(f'Return {i} {r.value}')
+                        #print(f'Return {i} {r.value}')
                         return r.value, r.e, ctx
                 except Exception as e:
                     print(str(e))
                     return None, e, ctx
 
 
 class FMap(Stream):
```

### Comparing `python_flux-1.2.0/python_flux/flux_utilis.py` & `python_flux-1.2.1/python_flux/flux_utilis.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.2.0/python_flux/producers.py` & `python_flux-1.2.1/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.2.0/python_flux/subscribers.py` & `python_flux-1.2.1/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.2.0/PKG-INFO` & `python_flux-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.2.0
+Version: 1.2.1
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

