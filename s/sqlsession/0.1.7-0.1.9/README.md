# Comparing `tmp/sqlsession-0.1.7.tar.gz` & `tmp/sqlsession-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlsession-0.1.7.tar", last modified: Thu Oct  6 13:07:40 2016, max compression
+gzip compressed data, was "dist/sqlsession-0.1.9.tar", last modified: Wed Mar  8 12:39:14 2017, max compression
```

## Comparing `sqlsession-0.1.7.tar` & `sqlsession-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2016-10-06 13:07:40.000000 sqlsession-0.1.7/
--rw-r--r--   0 qalt      (1000) qalt      (1000)      721 2016-10-06 13:07:40.000000 sqlsession-0.1.7/PKG-INFO
--rw-r--r--   0 qalt      (1000) qalt      (1000)       59 2016-10-06 13:07:40.000000 sqlsession-0.1.7/setup.cfg
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2016-10-06 13:07:40.000000 sqlsession-0.1.7/sqlsession.egg-info/
--rw-r--r--   0 qalt      (1000) qalt      (1000)      721 2016-10-06 13:07:39.000000 sqlsession-0.1.7/sqlsession.egg-info/PKG-INFO
--rw-r--r--   0 qalt      (1000) qalt      (1000)       34 2016-10-06 13:07:39.000000 sqlsession-0.1.7/sqlsession.egg-info/requires.txt
--rw-r--r--   0 qalt      (1000) qalt      (1000)        1 2016-10-06 13:07:39.000000 sqlsession-0.1.7/sqlsession.egg-info/dependency_links.txt
--rw-r--r--   0 qalt      (1000) qalt      (1000)       11 2016-10-06 13:07:39.000000 sqlsession-0.1.7/sqlsession.egg-info/top_level.txt
--rw-r--r--   0 qalt      (1000) qalt      (1000)        1 2016-04-12 15:04:42.000000 sqlsession-0.1.7/sqlsession.egg-info/not-zip-safe
--rw-r--r--   0 qalt      (1000) qalt      (1000)      233 2016-10-06 13:07:40.000000 sqlsession-0.1.7/sqlsession.egg-info/SOURCES.txt
--rwxr-xr-x   0 qalt      (1000) qalt      (1000)      954 2016-10-06 13:01:59.000000 sqlsession-0.1.7/setup.py
-drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2016-10-06 13:07:40.000000 sqlsession-0.1.7/sqlsession/
--rw-r--r--   0 qalt      (1000) qalt      (1000)     6738 2016-10-04 17:18:56.000000 sqlsession-0.1.7/sqlsession/__init__.py
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-03-08 12:39:14.000000 sqlsession-0.1.9/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      721 2017-03-08 12:39:14.000000 sqlsession-0.1.9/PKG-INFO
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       59 2017-03-08 12:39:14.000000 sqlsession-0.1.9/setup.cfg
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-03-08 12:39:14.000000 sqlsession-0.1.9/sqlsession.egg-info/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      721 2017-03-08 12:39:14.000000 sqlsession-0.1.9/sqlsession.egg-info/PKG-INFO
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       34 2017-03-08 12:39:14.000000 sqlsession-0.1.9/sqlsession.egg-info/requires.txt
+-rw-r--r--   0 qalt      (1000) qalt      (1000)        1 2017-03-08 12:39:14.000000 sqlsession-0.1.9/sqlsession.egg-info/dependency_links.txt
+-rw-r--r--   0 qalt      (1000) qalt      (1000)       11 2017-03-08 12:39:14.000000 sqlsession-0.1.9/sqlsession.egg-info/top_level.txt
+-rw-r--r--   0 qalt      (1000) qalt      (1000)        1 2016-04-12 15:04:42.000000 sqlsession-0.1.9/sqlsession.egg-info/not-zip-safe
+-rw-r--r--   0 qalt      (1000) qalt      (1000)      233 2017-03-08 12:39:14.000000 sqlsession-0.1.9/sqlsession.egg-info/SOURCES.txt
+-rwxr-xr-x   0 qalt      (1000) qalt      (1000)      954 2017-03-08 12:36:19.000000 sqlsession-0.1.9/setup.py
+drwxr-xr-x   0 qalt      (1000) qalt      (1000)        0 2017-03-08 12:39:14.000000 sqlsession-0.1.9/sqlsession/
+-rw-r--r--   0 qalt      (1000) qalt      (1000)     9766 2017-03-08 11:38:30.000000 sqlsession-0.1.9/sqlsession/__init__.py
```

### Comparing `sqlsession-0.1.7/PKG-INFO` & `sqlsession-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sqlsession
-Version: 0.1.7
+Version: 0.1.9
 Summary: Dirt simple CRUD API to access SQL databases
 Home-page: https://bitbucket.org/trackingwire/sqlsession
 Author: Peter Facka
 Author-email: pfacka@trackingwire.com
 License: MIT Licence (http://opensource.org/licenses/MIT)
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -12,8 +12,8 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: MIT License
-Provides: sqlsession (0.1.7)
+Provides: sqlsession (0.1.9)
```

### Comparing `sqlsession-0.1.7/sqlsession.egg-info/PKG-INFO` & `sqlsession-0.1.9/sqlsession.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sqlsession
-Version: 0.1.7
+Version: 0.1.9
 Summary: Dirt simple CRUD API to access SQL databases
 Home-page: https://bitbucket.org/trackingwire/sqlsession
 Author: Peter Facka
 Author-email: pfacka@trackingwire.com
 License: MIT Licence (http://opensource.org/licenses/MIT)
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -12,8 +12,8 @@
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: MIT License
-Provides: sqlsession (0.1.7)
+Provides: sqlsession (0.1.9)
```

### Comparing `sqlsession-0.1.7/setup.py` & `sqlsession-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name="sqlsession",
-    version="0.1.7",
+    version="0.1.9",
     description='Dirt simple CRUD API to access SQL databases',
     author='Peter Facka',
     url='https://bitbucket.org/trackingwire/sqlsession',
     author_email='pfacka@trackingwire.com',
     license='MIT Licence (http://opensource.org/licenses/MIT)',
     packages=[
         'sqlsession',
     ],
     zip_safe=False,	
     install_requires=[
         'SQLAlchemy>=1.0.6',
         'psycopg2>=2.6.1'
     ],
-    provides=['sqlsession (0.1.7)'],
+    provides=['sqlsession (0.1.9)'],
     include_package_data=True,
     classifiers=[
       'Development Status :: 3 - Alpha',
       'Environment :: Web Environment',
       'Intended Audience :: Developers',
       'Operating System :: Microsoft :: Windows',
       'Operating System :: MacOS :: MacOS X',
```

