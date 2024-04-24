# Comparing `tmp/jobmaster-0.1.0.tar.gz` & `tmp/jobmaster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobmaster-0.1.0.tar", last modified: Wed Apr 24 15:08:09 2024, max compression
+gzip compressed data, was "jobmaster-0.1.1.tar", last modified: Wed Apr 24 15:29:53 2024, max compression
```

## Comparing `jobmaster-0.1.0.tar` & `jobmaster-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-24 15:08:09.867171 jobmaster-0.1.0/
--rw-r--r--   0 joshua     (501) staff       (20)     9672 2024-04-24 15:08:09.866870 jobmaster-0.1.0/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)     8979 2024-04-23 16:33:55.000000 jobmaster-0.1.0/README.md
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-24 15:08:09.865746 jobmaster-0.1.0/jobmaster/
--rw-r--r--   0 joshua     (501) staff       (20)      372 2024-04-24 08:31:27.000000 jobmaster-0.1.0/jobmaster/__init__.py
--rw-r--r--   0 joshua     (501) staff       (20)      953 2024-04-24 08:07:57.000000 jobmaster-0.1.0/jobmaster/decorator.py
--rw-r--r--   0 joshua     (501) staff       (20)    14066 2024-04-24 15:06:50.000000 jobmaster-0.1.0/jobmaster/deploy.py
--rw-r--r--   0 joshua     (501) staff       (20)    31694 2024-04-24 13:29:50.000000 jobmaster-0.1.0/jobmaster/jobs.py
--rw-r--r--   0 joshua     (501) staff       (20)    12209 2024-04-24 08:31:07.000000 jobmaster-0.1.0/jobmaster/tasks.py
--rw-r--r--   0 joshua     (501) staff       (20)     3029 2024-04-23 09:47:11.000000 jobmaster-0.1.0/jobmaster/utils.py
-drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-24 15:08:09.866572 jobmaster-0.1.0/jobmaster.egg-info/
--rw-r--r--   0 joshua     (501) staff       (20)     9672 2024-04-24 15:08:09.000000 jobmaster-0.1.0/jobmaster.egg-info/PKG-INFO
--rw-r--r--   0 joshua     (501) staff       (20)      303 2024-04-24 15:08:09.000000 jobmaster-0.1.0/jobmaster.egg-info/SOURCES.txt
--rw-r--r--   0 joshua     (501) staff       (20)        1 2024-04-24 15:08:09.000000 jobmaster-0.1.0/jobmaster.egg-info/dependency_links.txt
--rw-r--r--   0 joshua     (501) staff       (20)       18 2024-04-24 15:08:09.000000 jobmaster-0.1.0/jobmaster.egg-info/requires.txt
--rw-r--r--   0 joshua     (501) staff       (20)       10 2024-04-24 15:08:09.000000 jobmaster-0.1.0/jobmaster.egg-info/top_level.txt
--rw-r--r--   0 joshua     (501) staff       (20)       38 2024-04-24 15:08:09.867219 jobmaster-0.1.0/setup.cfg
--rw-r--r--   0 joshua     (501) staff       (20)     1005 2024-04-23 11:01:47.000000 jobmaster-0.1.0/setup.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-24 15:29:53.099208 jobmaster-0.1.1/
+-rw-r--r--   0 joshua     (501) staff       (20)     1073 2024-04-24 15:11:53.000000 jobmaster-0.1.1/LICENCE
+-rw-r--r--   0 joshua     (501) staff       (20)     9780 2024-04-24 15:29:53.098907 jobmaster-0.1.1/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)     9065 2024-04-24 15:27:56.000000 jobmaster-0.1.1/README.md
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-24 15:29:53.097903 jobmaster-0.1.1/jobmaster/
+-rw-r--r--   0 joshua     (501) staff       (20)      372 2024-04-24 15:29:18.000000 jobmaster-0.1.1/jobmaster/__init__.py
+-rw-r--r--   0 joshua     (501) staff       (20)      953 2024-04-24 08:07:57.000000 jobmaster-0.1.1/jobmaster/decorator.py
+-rw-r--r--   0 joshua     (501) staff       (20)    14066 2024-04-24 15:06:50.000000 jobmaster-0.1.1/jobmaster/deploy.py
+-rw-r--r--   0 joshua     (501) staff       (20)    31694 2024-04-24 13:29:50.000000 jobmaster-0.1.1/jobmaster/jobs.py
+-rw-r--r--   0 joshua     (501) staff       (20)    12209 2024-04-24 08:31:07.000000 jobmaster-0.1.1/jobmaster/tasks.py
+-rw-r--r--   0 joshua     (501) staff       (20)     3029 2024-04-23 09:47:11.000000 jobmaster-0.1.1/jobmaster/utils.py
+drwxr-xr-x   0 joshua     (501) staff       (20)        0 2024-04-24 15:29:53.098644 jobmaster-0.1.1/jobmaster.egg-info/
+-rw-r--r--   0 joshua     (501) staff       (20)     9780 2024-04-24 15:29:53.000000 jobmaster-0.1.1/jobmaster.egg-info/PKG-INFO
+-rw-r--r--   0 joshua     (501) staff       (20)      311 2024-04-24 15:29:53.000000 jobmaster-0.1.1/jobmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua     (501) staff       (20)        1 2024-04-24 15:29:53.000000 jobmaster-0.1.1/jobmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       18 2024-04-24 15:29:53.000000 jobmaster-0.1.1/jobmaster.egg-info/requires.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       10 2024-04-24 15:29:53.000000 jobmaster-0.1.1/jobmaster.egg-info/top_level.txt
+-rw-r--r--   0 joshua     (501) staff       (20)       38 2024-04-24 15:29:53.099258 jobmaster-0.1.1/setup.cfg
+-rw-r--r--   0 joshua     (501) staff       (20)     1005 2024-04-24 15:29:18.000000 jobmaster-0.1.1/setup.py
```

### Comparing `jobmaster-0.1.0/PKG-INFO` & `jobmaster-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: jobmaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: JobMaster allows a user to quickly and simply deploy and manage a collection of tasks.
 Home-page: https://github.com/DrPrettyman/jobmaster
 Author: DrPrettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENCE
 Requires-Dist: pg8000
 Requires-Dist: sqlalchemy
 
 # JobMaster
 
 JobMaster is a simple job scheduling library for Python. 
 It works with any PostgreSQL database, and is designed to be simple to use and easy to integrate into your existing codebase.
 
 ## Installation
 
-Not yet publised on pip.
+Published to PyPi at https://pypi.org/project/jobmaster/.
+
+Simply use pip:
+
+```shell
+pip install jobmaster
+```
 
 ## Usage
 
 Any function in your project can become a JobMaster Task by using the `@task` decorator.
 For example, you may have a function like this:
 ```python
 # jmtests/awesome_things/things1.py
```

### Comparing `jobmaster-0.1.0/README.md` & `jobmaster-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # JobMaster
 
 JobMaster is a simple job scheduling library for Python. 
 It works with any PostgreSQL database, and is designed to be simple to use and easy to integrate into your existing codebase.
 
 ## Installation
 
-Not yet publised on pip.
+Published to PyPi at https://pypi.org/project/jobmaster/.
+
+Simply use pip:
+
+```shell
+pip install jobmaster
+```
 
 ## Usage
 
 Any function in your project can become a JobMaster Task by using the `@task` decorator.
 For example, you may have a function like this:
 ```python
 # jmtests/awesome_things/things1.py
```

### Comparing `jobmaster-0.1.0/jobmaster/decorator.py` & `jobmaster-0.1.1/jobmaster/decorator.py`

 * *Files identical despite different names*

### Comparing `jobmaster-0.1.0/jobmaster/deploy.py` & `jobmaster-0.1.1/jobmaster/deploy.py`

 * *Files identical despite different names*

### Comparing `jobmaster-0.1.0/jobmaster/jobs.py` & `jobmaster-0.1.1/jobmaster/jobs.py`

 * *Files identical despite different names*

### Comparing `jobmaster-0.1.0/jobmaster/tasks.py` & `jobmaster-0.1.1/jobmaster/tasks.py`

 * *Files identical despite different names*

### Comparing `jobmaster-0.1.0/jobmaster/utils.py` & `jobmaster-0.1.1/jobmaster/utils.py`

 * *Files identical despite different names*

### Comparing `jobmaster-0.1.0/jobmaster.egg-info/PKG-INFO` & `jobmaster-0.1.1/jobmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: jobmaster
-Version: 0.1.0
+Version: 0.1.1
 Summary: JobMaster allows a user to quickly and simply deploy and manage a collection of tasks.
 Home-page: https://github.com/DrPrettyman/jobmaster
 Author: DrPrettyman
 Author-email: joshua@blinkseo.co.uk
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENCE
 Requires-Dist: pg8000
 Requires-Dist: sqlalchemy
 
 # JobMaster
 
 JobMaster is a simple job scheduling library for Python. 
 It works with any PostgreSQL database, and is designed to be simple to use and easy to integrate into your existing codebase.
 
 ## Installation
 
-Not yet publised on pip.
+Published to PyPi at https://pypi.org/project/jobmaster/.
+
+Simply use pip:
+
+```shell
+pip install jobmaster
+```
 
 ## Usage
 
 Any function in your project can become a JobMaster Task by using the `@task` decorator.
 For example, you may have a function like this:
 ```python
 # jmtests/awesome_things/things1.py
```

### Comparing `jobmaster-0.1.0/setup.py` & `jobmaster-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # python setup.py bdist_wheel --universal
 # twine upload dist/*
 
 _desc = """JobMaster allows a user to quickly and simply deploy and manage a collection of tasks."""
 
 setup(
     name='jobmaster',
-    version='0.1.0',
+    version='0.1.1',
     description=_desc,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/DrPrettyman/jobmaster',
     author='DrPrettyman',
     author_email='joshua@blinkseo.co.uk',
     license='MIT',
```

