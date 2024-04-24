# Comparing `tmp/bgtask4django-1.0.0.tar.gz` & `tmp/bgtask4django-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgtask4django-1.0.0.tar", last modified: Wed Apr 17 07:06:25 2024, max compression
+gzip compressed data, was "bgtask4django-1.0.1.tar", last modified: Wed Apr 24 03:44:42 2024, max compression
```

## Comparing `bgtask4django-1.0.0.tar` & `bgtask4django-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 07:06:25.544193 bgtask4django-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-04-17 02:48:45.000000 bgtask4django-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1581 2024-04-17 07:06:25.540172 bgtask4django-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1125 2024-04-17 06:51:21.000000 bgtask4django-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 07:06:25.495305 bgtask4django-1.0.0/bgtask/
--rw-rw-rw-   0        0        0      629 2024-04-17 05:45:09.000000 bgtask4django-1.0.0/bgtask/__init__.py
--rw-rw-rw-   0        0        0      247 2024-04-16 11:38:39.000000 bgtask4django-1.0.0/bgtask/admin.py
--rw-rw-rw-   0        0        0      121 2024-04-17 05:58:27.000000 bgtask4django-1.0.0/bgtask/apps.py
--rw-rw-rw-   0        0        0      856 2024-04-17 02:11:29.000000 bgtask4django-1.0.0/bgtask/client.py
--rw-rw-rw-   0        0        0     4479 2024-04-17 02:03:30.000000 bgtask4django-1.0.0/bgtask/core.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:06:25.524221 bgtask4django-1.0.0/bgtask/management/
--rw-rw-rw-   0        0        0        0 2024-04-17 05:38:57.000000 bgtask4django-1.0.0/bgtask/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:06:25.530229 bgtask4django-1.0.0/bgtask/management/commands/
--rw-rw-rw-   0        0        0       16 2024-04-16 10:37:27.000000 bgtask4django-1.0.0/bgtask/management/commands/__init__.py
--rw-rw-rw-   0        0        0     2318 2024-04-17 05:50:57.000000 bgtask4django-1.0.0/bgtask/management/commands/bgtaskserver.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:06:25.536181 bgtask4django-1.0.0/bgtask/migrations/
--rw-rw-rw-   0        0        0     1512 2024-04-17 01:54:22.000000 bgtask4django-1.0.0/bgtask/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-04-16 09:34:30.000000 bgtask4django-1.0.0/bgtask/migrations/__init__.py
--rw-rw-rw-   0        0        0     1413 2024-04-17 01:23:25.000000 bgtask4django-1.0.0/bgtask/models.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:06:25.539190 bgtask4django-1.0.0/bgtask4django.egg-info/
--rw-rw-rw-   0        0        0     1581 2024-04-17 07:06:25.000000 bgtask4django-1.0.0/bgtask4django.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-04-17 07:06:25.000000 bgtask4django-1.0.0/bgtask4django.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 07:06:25.000000 bgtask4django-1.0.0/bgtask4django.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 07:06:25.000000 bgtask4django-1.0.0/bgtask4django.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 07:06:25.544193 bgtask4django-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      710 2024-04-17 07:01:19.000000 bgtask4django-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:44:41.954165 bgtask4django-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-04-17 02:48:45.000000 bgtask4django-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2376 2024-04-24 03:44:41.952197 bgtask4django-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1915 2024-04-24 03:41:55.000000 bgtask4django-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 03:44:41.883373 bgtask4django-1.0.1/bgtask/
+-rw-rw-rw-   0        0        0      629 2024-04-17 05:45:09.000000 bgtask4django-1.0.1/bgtask/__init__.py
+-rw-rw-rw-   0        0        0      247 2024-04-16 11:38:39.000000 bgtask4django-1.0.1/bgtask/admin.py
+-rw-rw-rw-   0        0        0      121 2024-04-17 05:58:27.000000 bgtask4django-1.0.1/bgtask/apps.py
+-rw-rw-rw-   0        0        0      856 2024-04-17 02:11:29.000000 bgtask4django-1.0.1/bgtask/client.py
+-rw-rw-rw-   0        0        0     4486 2024-04-23 06:59:08.000000 bgtask4django-1.0.1/bgtask/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:44:41.899281 bgtask4django-1.0.1/bgtask/management/
+-rw-rw-rw-   0        0        0        0 2024-04-17 05:38:57.000000 bgtask4django-1.0.1/bgtask/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:44:41.904295 bgtask4django-1.0.1/bgtask/management/commands/
+-rw-rw-rw-   0        0        0       16 2024-04-16 10:37:27.000000 bgtask4django-1.0.1/bgtask/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-04-23 07:02:46.000000 bgtask4django-1.0.1/bgtask/management/commands/bgtaskserver.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:44:41.946159 bgtask4django-1.0.1/bgtask/migrations/
+-rw-rw-rw-   0        0        0     1512 2024-04-17 01:54:22.000000 bgtask4django-1.0.1/bgtask/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-16 09:34:30.000000 bgtask4django-1.0.1/bgtask/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1413 2024-04-17 01:23:25.000000 bgtask4django-1.0.1/bgtask/models.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:44:41.949175 bgtask4django-1.0.1/bgtask4django.egg-info/
+-rw-rw-rw-   0        0        0     2376 2024-04-24 03:44:41.000000 bgtask4django-1.0.1/bgtask4django.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-04-24 03:44:41.000000 bgtask4django-1.0.1/bgtask4django.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:44:41.000000 bgtask4django-1.0.1/bgtask4django.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 03:44:41.000000 bgtask4django-1.0.1/bgtask4django.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:44:41.955132 bgtask4django-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      715 2024-04-24 03:42:55.000000 bgtask4django-1.0.1/setup.py
```

### Comparing `bgtask4django-1.0.0/LICENSE.txt` & `bgtask4django-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bgtask4django-1.0.0/bgtask/__init__.py` & `bgtask4django-1.0.1/bgtask/__init__.py`

 * *Files identical despite different names*

### Comparing `bgtask4django-1.0.0/bgtask/client.py` & `bgtask4django-1.0.1/bgtask/client.py`

 * *Files identical despite different names*

### Comparing `bgtask4django-1.0.0/bgtask/core.py` & `bgtask4django-1.0.1/bgtask/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from logging import getLogger
 from queue import Queue, Full
 from threading import Thread
 from uuid import uuid4
 
 from .models import BgTask, StateEnum, ResultEnum
 
-log = getLogger("bgtask")
+log = getLogger("django.bgtask")
 
 
 class Worker(Thread):
     def __init__(self, queue: Queue, name=None):
         super().__init__(name=name)
         self.queue = queue
```

### Comparing `bgtask4django-1.0.0/bgtask/management/commands/bgtaskserver.py` & `bgtask4django-1.0.1/bgtask/management/commands/bgtaskserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 config = _get_config()
 SERVER = (config[0], config[1])
 WORK_THREADS = config[2]
 
 _queue_size = 100
 
-log = getLogger("bgtask")
+log = getLogger("django.bgtask")
 sel = selectors.DefaultSelector()
 executor = core.Executor(Queue(_queue_size), workers=WORK_THREADS)
 
 
 def read_all(conn) -> bytes:
     data = b""
     while True:
@@ -68,16 +68,11 @@
         .########..##...####....##....##.....##..######..#####...
         .##.....##.##....##.....##....#########.......##.##..##..
         .##.....##.##....##.....##....##.....##.##....##.##...##.
         .########...######......##....##.....##..######..##....##
         """)
 
         while True:
-            try:
-                events = sel.select()
-                for key, mask in events:
-                    callback = key.data
-                    callback(key.fileobj, mask)
-            except KeyboardInterrupt:
-                sock.close()
-                log.info("bye bye!")
-                break
+            events = sel.select()
+            for key, mask in events:
+                callback = key.data
+                callback(key.fileobj, mask)
```

### Comparing `bgtask4django-1.0.0/bgtask/migrations/0001_initial.py` & `bgtask4django-1.0.1/bgtask/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bgtask4django-1.0.0/bgtask/models.py` & `bgtask4django-1.0.1/bgtask/models.py`

 * *Files identical despite different names*

### Comparing `bgtask4django-1.0.0/setup.py` & `bgtask4django-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bgtask4django",
-    version="1.0.0",
+    version="1.0.1",
     author="leon_yang",
     author_email="leiyang_ace@163.com",
-    description="a Django app for background task ",
+    description="A Django app for background task ",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/leiyang23/django-bgtask",
+    url="https://github.com/pypa/leiyang23/django-bgtask",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

