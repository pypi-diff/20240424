# Comparing `tmp/django_utilsds-0.5.1.tar.gz` & `tmp/django_utilsds-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_utilsds-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_utilsds-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_utilsds-0.5.1.tar` & `django_utilsds-0.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     6148 2024-03-20 03:28:32.696016 django_utilsds-0.5.1/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-19 12:18:20.163079 django_utilsds-0.5.1/.gitattributes
--rw-r--r--   0        0        0        7 2024-03-19 12:37:16.850744 django_utilsds-0.5.1/.gitignore
--rw-r--r--   0        0        0       52 2024-03-19 12:19:45.020079 django_utilsds-0.5.1/.idea/.gitignore
--rw-r--r--   0        0        0      404 2024-03-19 12:19:44.945056 django_utilsds-0.5.1/.idea/django-utilsds.iml
--rw-r--r--   0        0        0      174 2024-03-19 12:19:44.955607 django_utilsds-0.5.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      419 2024-03-19 12:29:45.901640 django_utilsds-0.5.1/.idea/misc.xml
--rw-r--r--   0        0        0      280 2024-03-19 12:19:44.950172 django_utilsds-0.5.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-19 12:19:44.957383 django_utilsds-0.5.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_utilsds-0.5.1/LICENSE
--rw-r--r--   0        0        0     1068 2024-04-21 07:20:18.847459 django_utilsds-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_utilsds-0.5.1/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_utilsds-0.5.1/django_utilsds/__init__.py
--rw-r--r--   0        0        0       63 2024-03-19 12:26:04.845706 django_utilsds-0.5.1/django_utilsds/admin.py
--rw-r--r--   0        0        0      159 2024-03-19 12:29:42.988859 django_utilsds-0.5.1/django_utilsds/apps.py
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.847399 django_utilsds-0.5.1/django_utilsds/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-03-19 12:26:04.847124 django_utilsds-0.5.1/django_utilsds/models.py
--rw-r--r--   0        0        0      520 2024-04-21 04:44:19.962450 django_utilsds-0.5.1/django_utilsds/templatetags/django_utilsds_tags.py
--rw-r--r--   0        0        0       60 2024-03-19 12:26:04.847256 django_utilsds-0.5.1/django_utilsds/tests.py
--rw-r--r--   0        0        0     1824 2024-03-19 06:52:37.021339 django_utilsds-0.5.1/django_utilsds/utils.py
--rw-r--r--   0        0        0       63 2024-03-19 12:26:04.845433 django_utilsds-0.5.1/django_utilsds/views.py
--rw-r--r--   0        0        0      580 2024-04-21 07:20:18.855562 django_utilsds-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 django_utilsds-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-03-20 03:28:32.696016 django_utilsds-0.5.2/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-19 12:18:20.163079 django_utilsds-0.5.2/.gitattributes
+-rw-r--r--   0        0        0        7 2024-03-19 12:37:16.850744 django_utilsds-0.5.2/.gitignore
+-rw-r--r--   0        0        0       52 2024-03-19 12:19:45.020079 django_utilsds-0.5.2/.idea/.gitignore
+-rw-r--r--   0        0        0      404 2024-03-19 12:19:44.945056 django_utilsds-0.5.2/.idea/django-utilsds.iml
+-rw-r--r--   0        0        0      174 2024-03-19 12:19:44.955607 django_utilsds-0.5.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      419 2024-03-19 12:29:45.901640 django_utilsds-0.5.2/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2024-03-19 12:19:44.950172 django_utilsds-0.5.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-19 12:19:44.957383 django_utilsds-0.5.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_utilsds-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1068 2024-04-21 07:20:18.847459 django_utilsds-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_utilsds-0.5.2/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_utilsds-0.5.2/django_utilsds/__init__.py
+-rw-r--r--   0        0        0       63 2024-03-19 12:26:04.845706 django_utilsds-0.5.2/django_utilsds/admin.py
+-rw-r--r--   0        0        0      159 2024-03-19 12:29:42.988859 django_utilsds-0.5.2/django_utilsds/apps.py
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.847399 django_utilsds-0.5.2/django_utilsds/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-03-19 12:26:04.847124 django_utilsds-0.5.2/django_utilsds/models.py
+-rw-r--r--   0        0        0      520 2024-04-21 04:44:19.962450 django_utilsds-0.5.2/django_utilsds/templatetags/django_utilsds_tags.py
+-rw-r--r--   0        0        0       60 2024-03-19 12:26:04.847256 django_utilsds-0.5.2/django_utilsds/tests.py
+-rw-r--r--   0        0        0     1824 2024-03-19 06:52:37.021339 django_utilsds-0.5.2/django_utilsds/utils.py
+-rw-r--r--   0        0        0       63 2024-03-19 12:26:04.845433 django_utilsds-0.5.2/django_utilsds/views.py
+-rw-r--r--   0        0        0      581 2024-04-24 01:51:50.905059 django_utilsds-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1382 1970-01-01 00:00:00.000000 django_utilsds-0.5.2/PKG-INFO
```

### Comparing `django_utilsds-0.5.1/.DS_Store` & `django_utilsds-0.5.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_utilsds-0.5.1/LICENSE` & `django_utilsds-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_utilsds-0.5.1/README.md` & `django_utilsds-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django_utilsds-0.5.1/django_utilsds/templatetags/django_utilsds_tags.py` & `django_utilsds-0.5.2/django_utilsds/templatetags/django_utilsds_tags.py`

 * *Files identical despite different names*

### Comparing `django_utilsds-0.5.1/django_utilsds/utils.py` & `django_utilsds-0.5.2/django_utilsds/utils.py`

 * *Files identical despite different names*

### Comparing `django_utilsds-0.5.1/pyproject.toml` & `django_utilsds-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-utilsds"
-version = "0.5.1"
+version = "0.5.2"
 description = "One of the my demiansoft apps"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
-    "Django >= 5.0.3",
+    "Django >= 4.2.11",
 ]
 
 [project.urls]
 Home = "https://www.demiansoft.com"
 
 [tool.flit.sdist]
 exclude = [
```

### Comparing `django_utilsds-0.5.1/PKG-INFO` & `django_utilsds-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: django-utilsds
-Version: 0.5.1
+Version: 0.5.2
 Summary: One of the my demiansoft apps
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: Django >= 5.0.3
+Requires-Dist: Django >= 4.2.11
 Project-URL: Home, https://www.demiansoft.com
 
 ### django-utilsds
 
 #### Introduction
 
 demiansoft 에서 사용하는 장고앱 django-utilsds
```

