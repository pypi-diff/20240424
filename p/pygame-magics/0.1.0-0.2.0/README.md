# Comparing `tmp/pygame-magics-0.1.0.tar.gz` & `tmp/pygame-magics-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame-magics-0.1.0.tar", last modified: Wed Apr 24 16:34:27 2024, max compression
+gzip compressed data, was "pygame-magics-0.2.0.tar", last modified: Wed Apr 24 17:30:12 2024, max compression
```

## Comparing `pygame-magics-0.1.0.tar` & `pygame-magics-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,20 @@
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 16:34:27.111920 pygame-magics-0.1.0/
--rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 16:34:27.111724 pygame-magics-0.1.0/PKG-INFO
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 16:34:27.111434 pygame-magics-0.1.0/pygame_magics.egg-info/
--rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 16:34:27.000000 pygame-magics-0.1.0/pygame_magics.egg-info/PKG-INFO
--rw-r--r--   0 senya      (501) staff       (20)      192 2024-04-24 16:34:27.000000 pygame-magics-0.1.0/pygame_magics.egg-info/SOURCES.txt
--rw-r--r--   0 senya      (501) staff       (20)        1 2024-04-24 16:34:27.000000 pygame-magics-0.1.0/pygame_magics.egg-info/dependency_links.txt
--rw-r--r--   0 senya      (501) staff       (20)        7 2024-04-24 16:34:27.000000 pygame-magics-0.1.0/pygame_magics.egg-info/requires.txt
--rw-r--r--   0 senya      (501) staff       (20)        1 2024-04-24 16:34:27.000000 pygame-magics-0.1.0/pygame_magics.egg-info/top_level.txt
--rw-r--r--   0 senya      (501) staff       (20)       38 2024-04-24 16:34:27.111971 pygame-magics-0.1.0/setup.cfg
--rw-r--r--   0 senya      (501) staff       (20)      879 2024-04-24 16:34:25.000000 pygame-magics-0.1.0/setup.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:30:12.451623 pygame-magics-0.2.0/
+-rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 17:30:12.451423 pygame-magics-0.2.0/PKG-INFO
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:30:12.449379 pygame-magics-0.2.0/pygame/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:21:17.000000 pygame-magics-0.2.0/pygame/__init__.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:30:12.449610 pygame-magics-0.2.0/pygame/camera/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 16:50:43.000000 pygame-magics-0.2.0/pygame/camera/__init__.py
+-rw-r--r--   0 senya      (501) staff       (20)     2795 2024-04-24 17:17:23.000000 pygame-magics-0.2.0/pygame/camera/camera.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:30:12.450539 pygame-magics-0.2.0/pygame/entities/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:05:40.000000 pygame-magics-0.2.0/pygame/entities/__init__.py
+-rw-r--r--   0 senya      (501) staff       (20)      820 2024-04-24 17:09:08.000000 pygame-magics-0.2.0/pygame/entities/enemy.py
+-rw-r--r--   0 senya      (501) staff       (20)      381 2024-04-24 17:09:08.000000 pygame-magics-0.2.0/pygame/entities/experience_orb.py
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:05:53.000000 pygame-magics-0.2.0/pygame/entities/player.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:30:12.451188 pygame-magics-0.2.0/pygame_magics.egg-info/
+-rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 17:30:12.000000 pygame-magics-0.2.0/pygame_magics.egg-info/PKG-INFO
+-rw-r--r--   0 senya      (501) staff       (20)      374 2024-04-24 17:30:12.000000 pygame-magics-0.2.0/pygame_magics.egg-info/SOURCES.txt
+-rw-r--r--   0 senya      (501) staff       (20)        1 2024-04-24 17:30:12.000000 pygame-magics-0.2.0/pygame_magics.egg-info/dependency_links.txt
+-rw-r--r--   0 senya      (501) staff       (20)        7 2024-04-24 17:30:12.000000 pygame-magics-0.2.0/pygame_magics.egg-info/requires.txt
+-rw-r--r--   0 senya      (501) staff       (20)        7 2024-04-24 17:30:12.000000 pygame-magics-0.2.0/pygame_magics.egg-info/top_level.txt
+-rw-r--r--   0 senya      (501) staff       (20)       38 2024-04-24 17:30:12.451670 pygame-magics-0.2.0/setup.cfg
+-rw-r--r--   0 senya      (501) staff       (20)      879 2024-04-24 17:27:50.000000 pygame-magics-0.2.0/setup.py
```

### Comparing `pygame-magics-0.1.0/PKG-INFO` & `pygame-magics-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-magics
-Version: 0.1.0
+Version: 0.2.0
 Summary: Magic survival funcs
 Home-page: https://github.com/MCtop4ik/pygame-magics
 Author: MCtop4ik
 Author-email: senyaza@mail.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygame-magics-0.1.0/pygame_magics.egg-info/PKG-INFO` & `pygame-magics-0.2.0/pygame_magics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-magics
-Version: 0.1.0
+Version: 0.2.0
 Summary: Magic survival funcs
 Home-page: https://github.com/MCtop4ik/pygame-magics
 Author: MCtop4ik
 Author-email: senyaza@mail.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygame-magics-0.1.0/setup.py` & `pygame-magics-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pygame-magics',
-    version='0.1.0',
+    version='0.2.0',
     author='MCtop4ik',
     author_email='senyaza@mail.ru',
     description='Magic survival funcs',
     long_description='Hyper grest library for magic survival',
     long_description_content_type='text/markdown',
     url='https://github.com/MCtop4ik/pygame-magics',
     packages=find_packages(),
```

