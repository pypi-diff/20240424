# Comparing `tmp/pyslth-0.0.9.tar.gz` & `tmp/pyslth-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.0.9.tar", last modified: Mon Apr 22 13:50:55 2024, max compression
+gzip compressed data, was "pyslth-0.1.0.tar", last modified: Wed Apr 24 16:44:55 2024, max compression
```

## Comparing `pyslth-0.0.9.tar` & `pyslth-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.194055 pyslth-0.0.9/
--rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.9/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-22 13:50:55.193858 pyslth-0.0.9/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.180325 pyslth-0.0.9/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-22 13:50:55.000000 pyslth-0.0.9/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)      984 2024-04-22 13:50:55.000000 pyslth-0.0.9/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-22 13:50:55.000000 pyslth-0.0.9/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-22 13:50:55.000000 pyslth-0.0.9/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-22 13:50:55.000000 pyslth-0.0.9/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.0.9/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-22 13:50:55.194113 pyslth-0.0.9/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-22 13:48:41.000000 pyslth-0.0.9/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.186705 pyslth-0.0.9/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3758 2024-04-21 03:08:32.000000 pyslth-0.0.9/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6908 2024-04-16 09:47:23.000000 pyslth-0.0.9/slth/components.py
--rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.0.9/slth/conf.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.188117 pyslth-0.0.9/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.0.9/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     3360 2024-04-19 14:28:46.000000 pyslth-0.0.9/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20178 2024-04-22 11:56:59.000000 pyslth-0.0.9/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.9/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2174 2024-04-22 07:56:01.000000 pyslth-0.0.9/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    22623 2024-04-22 11:41:20.000000 pyslth-0.0.9/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.189475 pyslth-0.0.9/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.9/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.190112 pyslth-0.0.9/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.9/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.9/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.9/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.191443 pyslth-0.0.9/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.9/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.0.9/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.0.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.9/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5261 2024-04-18 19:49:35.000000 pyslth-0.0.9/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.9/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.9/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19065 2024-04-21 20:03:47.000000 pyslth-0.0.9/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.0.9/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.191964 pyslth-0.0.9/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.9/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.9/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.0.9/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.178835 pyslth-0.0.9/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-22 13:50:55.193171 pyslth-0.0.9/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.0.9/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.9/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.0.9/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.9/slth/statistics.py
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.0.9/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.9/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1346 2024-04-19 18:20:03.000000 pyslth-0.0.9/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     1995 2024-04-18 12:26:48.000000 pyslth-0.0.9/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.661866 pyslth-0.1.0/
+-rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.1.0/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-24 16:44:55.661653 pyslth-0.1.0/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.648446 pyslth-0.1.0/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-24 16:44:55.000000 pyslth-0.1.0/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1072 2024-04-24 16:44:55.000000 pyslth-0.1.0/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-24 16:44:55.000000 pyslth-0.1.0/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      146 2024-04-24 16:44:55.000000 pyslth-0.1.0/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-24 16:44:55.000000 pyslth-0.1.0/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      138 2024-04-14 18:56:42.000000 pyslth-0.1.0/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-24 16:44:55.661928 pyslth-0.1.0/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-24 16:44:23.000000 pyslth-0.1.0/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.654782 pyslth-0.1.0/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.0/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6908 2024-04-16 09:47:23.000000 pyslth-0.1.0/slth/components.py
+-rw-r--r--   0 breno      (501) staff       (20)     2149 2024-04-14 19:04:32.000000 pyslth-0.1.0/slth/conf.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.655412 pyslth-0.1.0/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.0/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.0/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20164 2024-04-23 08:03:17.000000 pyslth-0.1.0/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.0/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2174 2024-04-22 07:56:01.000000 pyslth-0.1.0/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25116 2024-04-24 14:52:21.000000 pyslth-0.1.0/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.655734 pyslth-0.1.0/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.0/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.656497 pyslth-0.1.0/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.0/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.0/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.0/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.659196 pyslth-0.1.0/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.0/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.0/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.0/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.0/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.0/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.0/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5330 2024-04-23 11:48:55.000000 pyslth-0.1.0/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.0/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.0/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19216 2024-04-23 12:45:08.000000 pyslth-0.1.0/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.0/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.659708 pyslth-0.1.0/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.0/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.0/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.0/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.646907 pyslth-0.1.0/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-24 16:44:55.660843 pyslth-0.1.0/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.0/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.0/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.0/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.0/slth/statistics.py
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.0/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.1.0/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1112 2024-04-24 15:04:09.000000 pyslth-0.1.0/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     1995 2024-04-18 12:26:48.000000 pyslth-0.1.0/slth/views.py
```

### Comparing `pyslth-0.0.9/PKG-INFO` & `pyslth-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.9
+Version: 0.1.0
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.9/pyslth.egg-info/PKG-INFO` & `pyslth-0.1.0/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.9
+Version: 0.1.0
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.9/pyslth.egg-info/SOURCES.txt` & `pyslth-0.1.0/pyslth.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -29,13 +29,15 @@
 slth/management/__init__.py
 slth/management/commands/__init__.py
 slth/management/commands/integration_test.py
 slth/management/commands/sync.py
 slth/migrations/0001_initial.py
 slth/migrations/0002_email_role_pushsubscription_error.py
 slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+slth/migrations/0004_alter_profile_photo.py
+slth/migrations/0005_alter_profile_photo.py
 slth/migrations/__init__.py
 slth/selenium/__init__.py
 slth/selenium/browser.py
 slth/static/images/logo.png
 slth/static/images/logo.svg
 slth/static/images/user.png
```

### Comparing `pyslth-0.0.9/setup.py` & `pyslth-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.0.9',
+    version='0.1.0',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.0.9/slth/__init__.py` & `pyslth-0.1.0/slth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 class Manager(BaseManager.from_queryset(QuerySet)):
     pass
 
 
 models.QuerySet = QuerySet
 models.Manager = Manager
-setattr(options, 'DEFAULT_NAMES', options.DEFAULT_NAMES + ('icon',))
+setattr(options, 'DEFAULT_NAMES', options.DEFAULT_NAMES + ('icon', 'search_fields'))
 
 
 
 class ModelMixin(object):
 
     @classmethod
     def get_field(cls, lookup):
```

### Comparing `pyslth-0.0.9/slth/components.py` & `pyslth-0.1.0/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/conf.py` & `pyslth-0.1.0/slth/conf.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/endpoints.py` & `pyslth-0.1.0/slth/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.core.cache import cache
 from django.conf import settings
 from django.utils.text import slugify
 from django.db import transaction, models
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 from .factory import FormFactory
-from .forms import LoginForm, ModelForm, Form, SendPushNotificationForm
+from .forms import LoginForm, ModelForm, Form, SendPushNotificationForm, EditProfileForm
 from .serializer import serialize, Serializer
 from .components import Application as Application_, Navbar, Menu, Footer, Response, Boxes, IconSet
 from .exceptions import JsonResponseException
 from .utils import build_url, append_url
 from .models import PushSubscription, Profile
 from slth.queryset import QuerySet
 from slth import APPLICATON, ENDPOINTS
@@ -379,15 +379,15 @@
         return self.get_instance().formfactory()
    
 class Delete(ChildInstanceEndpoint):
     class Meta:
         icon = 'trash'
         verbose_name = 'Excluir'
     def get(self):
-        return self.formfactory(self.get_instance(), delete=True)
+        return self.formfactory(delete=True)
 
 class Login(Endpoint):
     def get(self):
         return LoginForm(request=self.request)
 
 class Logout(PublicEndpoint):
     class Meta:
@@ -575,13 +575,13 @@
 
 class EditProfile(Endpoint):
     class Meta:
         verbose_name = 'Editar Perfil'
 
     def get(self):
         profile = Profile.objects.filter(user=self.request.user).first() or Profile(user=self.request.user)
-        return FormFactory(instance=profile).fieldset('Dados Gerais', ['photo'])
+        return EditProfileForm(instance=profile, request=self.request)
 
     def check_permission(self):
         return self.request.user.is_authenticated
```

### Comparing `pyslth-0.0.9/slth/factory.py` & `pyslth-0.1.0/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/forms.py` & `pyslth-0.1.0/slth/forms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 import json
 from typing import Any
 import datetime
 from django.forms import *
 from django.utils.translation import gettext_lazy as _
 from django.contrib.auth import authenticate
-from django.db.models.fields.files import FieldFile
+from django.db.models.fields.files import FieldFile, ImageFieldFile
 from django.forms.models import ModelChoiceIterator, ModelMultipleChoiceField
 from django.db.models import Model, QuerySet, Manager
-from .models import Token
+from .models import Token, Profile
 from django.db import transaction
 from django.db.models import Manager
 from .exceptions import JsonResponseException
 from .utils import absolute_url, build_url
 from .serializer import Serializer
 from .components import Response
 from .notifications import send_push_web_notification
@@ -20,14 +20,16 @@
 
 
 DjangoModelForm = ModelForm
 DjangoForm = Form
 DjangoModelChoiceField = ModelChoiceField
 DjangoMultipleChoiceField = MultipleChoiceField
 DjangoModelMultipleChoiceField = ModelMultipleChoiceField
+DjangoFileField = FileField
+DjangoImageField = ImageField
 
 MASKS = dict(
     cpf_cnpj='999.999.999-99|99.999.999/9999-99',
     cpf='999.999.999-99',
     cnpj='99.999.999/9999-99',
     telefone='(99) 99999-9999',
 )
@@ -150,14 +152,15 @@
                 kwargs = dict(instance=instance, request=self.request) if isinstance(field, InlineModelField) else dict(request=self.request)
                 value.append(field.form(**kwargs).to_dict(prefix=prefix))
             if not is_one_to_one:
                 value.append(field.form(request=self.request).to_dict(prefix=f'{name}__n'))
             required = getattr(field, 'required2', field.required)
             data = dict(type='inline', min=field.min, max=field.max, name=name, count=len(instances), label=field.label, required=required, value=value)
         else:
+            extra = {}
             ftype = FIELD_TYPES.get(type(field).__name__, 'text')
             if name in self._values:
                 ftype = 'hidden'
                 value = self._values[name]
                 value = value.pk if isinstance(value, Model) else value
             else:
                 value = field.initial or self.initial.get(name)
@@ -167,23 +170,28 @@
                 if isinstance(field, ModelMultipleChoiceField) or isinstance(field, DjangoModelMultipleChoiceField):
                     value = [dict(id=obj.id, label=str(obj)) for obj in value] if value else []
                 elif isinstance(field, MultipleChoiceField) or isinstance(field,DjangoMultipleChoiceField):
                     value = value if value else []
                 elif value and (isinstance(field, ModelChoiceField) or isinstance(field, DjangoModelChoiceField)):
                     obj = field.queryset.get(pk=value)
                     value = dict(id=obj.id, label=str(obj))
+                elif isinstance(value, ImageFieldFile):
+                    value = build_url(self.request, value.url) if value else None
+                    extra.update(extensions=field.extensions, width=field.width, height=field.height)
                 elif isinstance(value, FieldFile):
                     value = build_url(self.request, value.url) if value else None
+                    extra.update(extensions=field.extensions, max_size=field.max_size)
             
             if isinstance(field.widget, HiddenInput):
                 ftype = 'hidden'
                 value = value['id'] if isinstance(value, dict) else value
 
             fname = name if prefix is None else f'{prefix}__{name}'
             data = dict(type=ftype, name=fname, label=field.label, required=field.required, value=value, help_text=field.help_text, mask=None)
+            data.update(**extra)
             for word in MASKS:
                 if word in name:
                     data.update(mask=MASKS[word])
             for word in ('password', 'senha'):
                 if word in name:
                     data.update(type='password')
             if isinstance(field, CharField) or isinstance(field, IntegerField):
@@ -196,23 +204,32 @@
                 data.update(mask='decimal')
             elif ftype == 'choice':
                 if name in self.request.GET:
                     data.update(type='hidden', value=self.request.GET[name])
                 else:
                     if isinstance(field.choices, ModelChoiceIterator):
                         if choices_field_name == fname:
-                            method_name = f'get_{fname}_queryset'
                             qs = field.choices.queryset
+                            
+                            method_attr = None
+                            method_name = f'get_{fname}_queryset'
                             if hasattr(self, method_name):
-                                values = {}
+                                method_attr = getattr(self, method_name)
+                            elif hasattr(self, 'instance') and hasattr(self.instance, method_name):
+                                method_attr = getattr(self.instance, method_name)
+
+                            if method_attr:
+                                values = dict(user=self.request.user)
+                                values.update(**self._values)
                                 for name2 in self.fields:
                                     value2 = self.getdata(name2, self.request.GET.get(name2))
                                     if value2:
                                         values[name2] = value2
-                                qs = getattr(self, method_name)(qs, values)
+                                qs = method_attr(qs, values)
+                            
                             if 'term' in self.request.GET:
                                 qs = qs.apply_search(self.request.GET['term'])
                             raise JsonResponseException([dict(id=obj.id, value=str(obj)) for obj in qs[0:10]])
                         else:
                             data['choices'] = absolute_url(self.request, f'choices={fname}')
                     else:
                         data['choices'] = [dict(id=k, value=v) for k, v in field.choices]
@@ -280,20 +297,19 @@
                             obj.save()
                             # set one-to-one
                             if hasattr(self.instance, f'{inline_field_name}_id'):
                                 if hasattr(obj, 'deleting'):
                                     setattr(self.instance, inline_field_name, None)
                                 else:
                                     setattr(self.instance, inline_field_name, obj)
-                    self.submit()
+                    response = self.submit()
                     for inline_field_name in inline_fields:
                         for obj in self.cleaned_data[inline_field_name]:
                             if hasattr(obj, 'deleting'):
                                 obj.delete()
-                    response = Response(message='Ação realizada com sucesso')
                 else:
                     response = self.submit()
             return response
                 
     def hide(self, *names):
         self.controls['hide'].extend(names)
 
@@ -402,14 +418,15 @@
         kwargs.update(data=data)
         if self.request:
             kwargs.update(files=self.request.FILES or None)
         super().__init__(instance=instance, **kwargs)
 
     def submit(self):
         self.instance.delete() if self.delete else self.save()
+        return Response(message='Ação realizada com sucesso')
 
     def get_fieldsets(self):
         return self.fieldsets
     
     def info(self, message):
         self._info = message
         return self
@@ -459,14 +476,30 @@
         if isinstance(value, str) and ',' in value:
             value = value.replace('.', '').replace(',', '.')
         return super().to_python(value)
     
 class ColorField(CharField):
     pass
 
+class FileField(FileField):
+    def __init__(self, *args, extensions=('pdf',), max_size=5, **kwargs):
+        self.extensions = extensions
+        self.max_size = max_size
+        super().__init__(*args, **kwargs)
+
+class ImageField(ImageField):
+    def __init__(self, *args, extensions=('png', 'jpg', 'jpeg'), width=None, height=None, **kwargs):
+        self.extensions = extensions
+        if width or height:
+            self.width = width or height
+            self.height = height or width
+        else:
+            self.width = self.height = 500
+        super().__init__(*args, **kwargs)
+
 class ChoiceField(ChoiceField):
     
     def __init__(self, *args, **kwargs):
         self.pick = kwargs.pop('pick', False)
         super().__init__(*args, **kwargs)
     
 class MultipleChoiceField(MultipleChoiceField):
@@ -507,14 +540,42 @@
         else:
             self.token = Token.objects.create(user=user)
             return cleaned_data
         
     def submit(self):
         return Response(message='Bem-vindo!', redirect='/api/dashboard/', store=dict(token=self.token.key, application=None))
 
+class EditProfileForm(ModelForm):
+    password = CharField(label=_('Senha'), required=False)
+    password2 = CharField(label=_('Confirmação'), required=False)
+
+    class Meta:
+        title = 'Editar Perfil'
+        model = Profile
+        fields = 'photo',
+
+    def get_fieldsets(self):
+        return {
+            'Dados Gerais': ('photo',),
+            'Dados de Acesso': (('password', 'password2'),)
+        }
+
+    def clean_password(self):
+        password = self.data.get('password')
+        password2 = self.data.get('password2')
+        if password and password != password2:
+            raise ValidationError('As senhas devem ser iguais.')
+        return password
+        
+    def submit(self):
+        self.save()
+        self.instance.user.set_password(self.cleaned_data.get('password'))
+        self.instance.user.save()
+        return Response(message='Ação realizada com sucesso.', redirect='/api/dashboard/', store=dict(application=None))
+
 class SendPushNotificationForm(Form):
     message = CharField(label='Text', widget=Textarea())
 
     def submit(self):
         send_push_web_notification(self.endpoint.source, self.cleaned_data['message'])
         return Response(message='Notificação enviada com sucesso.')
```

### Comparing `pyslth-0.0.9/slth/management/commands/integration_test.py` & `pyslth-0.1.0/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/management/commands/sync.py` & `pyslth-0.1.0/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/migrations/0001_initial.py` & `pyslth-0.1.0/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.1.0/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.1.0/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/models.py` & `pyslth-0.1.0/slth/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             self.sent_at = datetime.now()
         super().save(*args, **kwargs)
 
 
 class Profile(models.Model):
     
     user = models.OneToOneField(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
-    photo = models.ImageField(verbose_name=_("Photo"))
+    photo = models.ImageField(verbose_name=_("Photo"), width=500, blank=True, null=True, extensions=['png', 'jpg', 'jpeg'])
 
     class Meta:
         verbose_name = _("Profile")
         verbose_name_plural = _("Profile")
 
 
 class Token(models.Model):
```

### Comparing `pyslth-0.0.9/slth/permissions.py` & `pyslth-0.1.0/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/queryset.py` & `pyslth-0.1.0/slth/queryset.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,16 +180,18 @@
             value = datetime.strptime(value, '%Y-%m-%d');
         if value in booleans:
             value = booleans[value]
         return self.filter(**{lookup: value}) if value != '' else self
 
     def apply_search(self, term, lookups=None):
         if lookups is None:
-            lookups = [f'{field.name}__icontains' for field in self.model._meta.get_fields()
-                       if isinstance(field, CharField)] or []
+            search_fields = getattr(self.model._meta, 'search_fields', None)
+            if search_fields is None:
+                search_fields = [field.name for field in self.model._meta.get_fields() if isinstance(field, CharField)]
+            lookups = [f'{name}__icontains' for name in search_fields]
         if lookups:
             terms = term.split(' ') if term else []
             conditions = []
             for term in terms:
                 queries = [
                     Q(**{lookup: term})
                     for lookup in lookups
```

### Comparing `pyslth-0.0.9/slth/roles.py` & `pyslth-0.1.0/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/selenium/__init__.py` & `pyslth-0.1.0/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/selenium/browser.py` & `pyslth-0.1.0/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/serializer.py` & `pyslth-0.1.0/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/static/images/logo.png` & `pyslth-0.1.0/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/static/images/logo.svg` & `pyslth-0.1.0/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/static/images/user.png` & `pyslth-0.1.0/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/statistics.py` & `pyslth-0.1.0/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/tests.py` & `pyslth-0.1.0/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/urls.py` & `pyslth-0.1.0/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.9/slth/utils.py` & `pyslth-0.1.0/slth/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-
+from django.conf import settings
 
 def build_url(request, path=None):
-    url = ''
     if path and path.startswith('http'):
-        url = path
+        return path
     elif request:
-        port = request.META.get('HTTP_X_FORWARDED_PORT', request.get_port())
-        port = '' if port in (80, 443) else f':{port}'
-        url = "{}://{}{}{}".format(
-            request.META.get('HTTP_X_FORWARDED_PROTO', request.scheme),
-            request.get_host().split(':')[0], port, path or request.path
-        )
-    return url
+        return '{}{}'.format(settings.SITE_URL, path or request.path)
+    return ''
 
 def absolute_url(request, *querystrings):
     url = build_url(request)
     if url:
         querstring = request.META.get('QUERY_STRING')
         url = append_url(url, querstring)
         for querystring in querystrings:
```

### Comparing `pyslth-0.0.9/slth/views.py` & `pyslth-0.1.0/slth/views.py`

 * *Files identical despite different names*

