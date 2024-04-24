# Comparing `tmp/python_flux-1.1.0.tar.gz` & `tmp/python_flux-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.1.0.tar", max compression
+gzip compressed data, was "python_flux-1.2.0.tar", max compression
```

## Comparing `python_flux-1.1.0.tar` & `python_flux-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7482 2024-04-23 04:13:01.727984 python_flux-1.1.0/README.rst
--rw-r--r--   0        0        0      741 2024-04-23 00:19:45.324741 python_flux-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.1.0/python_flux/__init__.py
--rw-r--r--   0        0        0    19031 2024-04-23 04:13:01.732417 python_flux-1.1.0/python_flux/flux.py
--rw-r--r--   0        0        0      759 2024-04-22 18:08:07.620526 python_flux-1.1.0/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1596 2024-04-18 05:35:27.173339 python_flux-1.1.0/python_flux/producers.py
--rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.1.0/python_flux/subscribers.py
--rw-r--r--   0        0        0     8213 1970-01-01 00:00:00.000000 python_flux-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7482 2024-04-23 04:13:01.727984 python_flux-1.2.0/README.rst
+-rw-r--r--   0        0        0      741 2024-04-24 15:26:03.777873 python_flux-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.2.0/python_flux/__init__.py
+-rw-r--r--   0        0        0    21695 2024-04-24 15:25:21.522783 python_flux-1.2.0/python_flux/flux.py
+-rw-r--r--   0        0        0      759 2024-04-22 18:08:07.620526 python_flux-1.2.0/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1596 2024-04-18 05:35:27.173339 python_flux-1.2.0/python_flux/producers.py
+-rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.2.0/python_flux/subscribers.py
+-rw-r--r--   0        0        0     8213 1970-01-01 00:00:00.000000 python_flux-1.2.0/PKG-INFO
```

### Comparing `python_flux-1.1.0/README.rst` & `python_flux-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_flux-1.1.0/pyproject.toml` & `python_flux-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.1.0"
+version = "1.2.0"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `python_flux-1.1.0/python_flux/flux.py` & `python_flux-1.2.0/python_flux/flux.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
+import sys
 import threading
 import types
 import time
 from datetime import timedelta, datetime
 from functools import partial
 from jsonmerge import merge
 from python_flux.flux_utilis import FluxUtils as fu
 from python_flux.subscribers import SSubscribe
-
+from concurrent.futures.thread import ThreadPoolExecutor
 
 class Flux(object):
 
     def filter(self, predicate, on_mismatch=fu.default_action):
         """
         Permite filtrar un flujo perimtiendo continuar a aquellos valores que cumplen con el
         predicado que se indica.
@@ -32,15 +33,15 @@
         :param map_function: función(valor, contexto) desde donde se obtendrá el valor a subsituir.
         """
         return FMap(map_function, self)
 
     def map_if(self, predicate, map_function):
         """
         Evalúa el predicado, si este es verdadero mapea el valor actual utilizando la función de mapeo.
-        
+
         :param predicate: función(valor, contexto) predicado que se evalúa.
         :param map_function: función(valor, contexto) desde donde se obtendrá el valor a subsituir.
         """
         return FMapIf(predicate, map_function, self)
 
     def map_context(self, map_context_function):
         """
@@ -132,14 +133,22 @@
 
         def log_error(msg, e, c):
             message = msg(e, c)
             logging.error(message)
 
         return FDoOnNext(partial(log_function, level, build_log_message), partial(log_error, build_error_message), True, self)
 
+    def parallel(self, pool_size=5):
+        """
+        Ejecuta la obtención de elementos del stream en paralelo
+
+        :param pool_size: Pool de hilos a utilizar
+        """
+        return FParallel(pool_size, self)
+
     def on_error_resume(self, resume=fu.default_error_resume, exceptions=[Exception]):
         """
         En caso de error, este paso ejecuta la función resume que debe retornar un valor
         a partir del error recibido por parámetro.
 
         :param resume: función(ex, contexto) Debe retornar el valor a substituir en el flujo.
         :param exceptions: Lista de excepciones para los que se aplica el resume.
@@ -227,15 +236,17 @@
         super(Stream, self).__init__()
         self.upstream = up
 
     def prepare_next(self):
         self.upstream.prepare_next()
 
     def next(self, context):
+        t = time.process_time()
         value, e, ctx = self.upstream.next(context)
+        elapsed_time = time.process_time() - t
         return value, e, ctx
 
 
 class FFilter(Stream):
     def __init__(self, p, m, flux):
         super().__init__(flux)
         self.predicate = p
@@ -280,16 +291,14 @@
             if e is not None:
                 return value, e, ctx
             return v, e, ctx
 
         return value, e, ctx
 
 
-
-
 class FTake(Stream):
     def __init__(self, count, flux):
         super().__init__(flux)
         self.count = count
         self.idx = 0
 
     def next(self, context):
@@ -366,14 +375,78 @@
         valid, e = fu.try_or(partial(self.predicate), value, ctx)
         if e is not None:
             return value, e, ctx
         if valid:
             time.sleep(self.delay / 1000)
         return value, e, ctx
 
+from random import randint
+class _Register:
+
+    def __init__(self, id):
+        self.id = id
+        self.value = None
+        self.e = None
+        self.ctx = None
+
+    def execute(self, prepare_next, next, context):
+        self.value, self.e, self.ctx = next(context)
+        prepare_next()
+        time.sleep(randint(1, 3))
+        sys.stdout.write(f'get: {self.id} {self.value}\n')
+        sys.stdout.flush()
+
+
+class FParallel(Stream):
+    def __init__(self, pool, flux):
+        super().__init__(flux)
+        self.pool_size = pool
+        self.jobs = {}
+        self.pool = {}
+        self.ids = 0
+        self.waiting_to_stop = False
+
+    def next(self, context):
+        ctx = context
+        while True:
+            if not self.waiting_to_stop:
+                if len(self.pool) < self.pool_size:
+                    reg = _Register(self.ids)
+                    t = threading.Thread(target=reg.execute, args=[super(FParallel, self).prepare_next, super(FParallel, self).next, context])
+                    self.jobs[self.ids] = reg
+                    self.pool[self.ids] = t
+                    self.ids = self.ids + 1
+                    t.start()
+            jobs = self.pool.copy()
+            for i, t in jobs.items():
+                try:
+                    t.join(0.001)
+                    if t.is_alive():
+                        continue
+                    else:
+                        print(f'pop {i}')
+                        self.pool.pop(i)
+                        r = self.jobs.pop(i)
+                        ctx = merge(ctx, r.ctx)
+                        if isinstance(r.e, StopIteration):
+                            print('StopIteration')
+                            self.waiting_to_stop = True
+                            if len(self.pool) == 0:
+                                return None, StopIteration(), ctx
+                            else:
+                                continue
+                        if self.waiting_to_stop:
+                            if len(self.pool) == 0:
+                                return None, StopIteration(), ctx
+                        print(f'Return {i} {r.value}')
+                        return r.value, r.e, ctx
+                except Exception as e:
+                    print(str(e))
+                    return None, e, ctx
+
 
 class FMap(Stream):
     def __init__(self, func, flux):
         super().__init__(flux)
         self.function = func
 
     def next(self, context):
```

### Comparing `python_flux-1.1.0/python_flux/flux_utilis.py` & `python_flux-1.2.0/python_flux/flux_utilis.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.1.0/python_flux/producers.py` & `python_flux-1.2.0/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.1.0/python_flux/subscribers.py` & `python_flux-1.2.0/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.1.0/PKG-INFO` & `python_flux-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.1.0
+Version: 1.2.0
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

