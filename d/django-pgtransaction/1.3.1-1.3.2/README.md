# Comparing `tmp/django_pgtransaction-1.3.1.tar.gz` & `tmp/django_pgtransaction-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgtransaction-1.3.1.tar", max compression
+gzip compressed data, was "django_pgtransaction-1.3.2.tar", max compression
```

## Comparing `django_pgtransaction-1.3.1.tar` & `django_pgtransaction-1.3.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1456 2024-04-06 16:50:31.417333 django_pgtransaction-1.3.1/LICENSE
--rw-r--r--   0        0        0     3038 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/README.md
--rw-r--r--   0        0        0      224 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/pgtransaction/__init__.py
--rw-r--r--   0        0        0      731 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/pgtransaction/config.py
--rw-r--r--   0        0        0     7377 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/pgtransaction/transaction.py
--rw-r--r--   0        0        0       87 2024-04-06 16:50:31.421333 django_pgtransaction-1.3.1/pgtransaction/version.py
--rw-r--r--   0        0        0     2297 2024-04-06 16:51:16.085864 django_pgtransaction-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4374 1970-01-01 00:00:00.000000 django_pgtransaction-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-24 03:34:44.331607 django_pgtransaction-1.3.2/LICENSE
+-rw-r--r--   0        0        0     3030 2024-04-24 03:34:44.331607 django_pgtransaction-1.3.2/README.md
+-rw-r--r--   0        0        0      224 2024-04-24 03:34:44.331607 django_pgtransaction-1.3.2/pgtransaction/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-24 03:34:44.331607 django_pgtransaction-1.3.2/pgtransaction/config.py
+-rw-r--r--   0        0        0        0 2024-04-24 03:34:44.331607 django_pgtransaction-1.3.2/pgtransaction/py.typed
+-rw-r--r--   0        0        0     7377 2024-04-24 03:34:44.331607 django_pgtransaction-1.3.2/pgtransaction/transaction.py
+-rw-r--r--   0        0        0       87 2024-04-24 03:34:44.331607 django_pgtransaction-1.3.2/pgtransaction/version.py
+-rw-r--r--   0        0        0     2593 2024-04-24 03:35:32.239899 django_pgtransaction-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 django_pgtransaction-1.3.2/PKG-INFO
```

### Comparing `django_pgtransaction-1.3.1/LICENSE` & `django_pgtransaction-1.3.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023, Opus 10
+Copyright (c) 2024, Opus 10
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright
   notice, this list of conditions and the following disclaimer.
```

### Comparing `django_pgtransaction-1.3.1/README.md` & `django_pgtransaction-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,18 @@
 [View the django-pgtransaction docs here](https://django-pgtransaction.readthedocs.io/)
 
 ## Installation
 
 Install `django-pgtransaction` with:
 
     pip3 install django-pgtransaction
-
 After this, add `pgtransaction` to the `INSTALLED_APPS` setting of your Django project.
 
 ## Contributing Guide
 
 For information on setting up django-pgtransaction for development and contributing changes, view [CONTRIBUTING.md](CONTRIBUTING.md).
 
-## Primary Authors
+## Creators
 
 - [Paul Gilmartin](https://github.com/PaulGilmartin)
 - [Wes Kendall](https://github.com/wesleykendall)
```

### Comparing `django_pgtransaction-1.3.1/pgtransaction/config.py` & `django_pgtransaction-1.3.2/pgtransaction/config.py`

 * *Files identical despite different names*

### Comparing `django_pgtransaction-1.3.1/pgtransaction/transaction.py` & `django_pgtransaction-1.3.2/pgtransaction/transaction.py`

 * *Files identical despite different names*

### Comparing `django_pgtransaction-1.3.1/PKG-INFO` & `django_pgtransaction-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgtransaction
-Version: 1.3.1
+Version: 1.3.2
 Summary: A context manager/decorator which extends Django's atomic function with the ability to set isolation level and retries for a given transaction.
 Home-page: https://github.com/Opus10/django-pgtransaction
 License: BSD-3-Clause
 Author: Opus 10 Engineering
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -17,16 +17,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: django (>=3)
 Project-URL: Documentation, https://django-pgtransaction.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pgtransaction
 Description-Content-Type: text/markdown
 
 # django-pgtransaction
 
@@ -75,20 +75,19 @@
 [View the django-pgtransaction docs here](https://django-pgtransaction.readthedocs.io/)
 
 ## Installation
 
 Install `django-pgtransaction` with:
 
     pip3 install django-pgtransaction
-
 After this, add `pgtransaction` to the `INSTALLED_APPS` setting of your Django project.
 
 ## Contributing Guide
 
 For information on setting up django-pgtransaction for development and contributing changes, view [CONTRIBUTING.md](CONTRIBUTING.md).
 
-## Primary Authors
+## Creators
 
 - [Paul Gilmartin](https://github.com/PaulGilmartin)
 - [Wes Kendall](https://github.com/wesleykendall)
```

