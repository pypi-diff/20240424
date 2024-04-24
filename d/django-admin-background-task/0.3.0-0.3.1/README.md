# Comparing `tmp/django_admin_background_task-0.3.0.tar.gz` & `tmp/django_admin_background_task-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_background_task-0.3.0.tar", max compression
+gzip compressed data, was "django_admin_background_task-0.3.1.tar", max compression
```

## Comparing `django_admin_background_task-0.3.0.tar` & `django_admin_background_task-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-03-08 11:29:40.116270 django_admin_background_task-0.3.0/LICENSE
--rw-r--r--   0        0        0      597 2024-03-08 15:24:11.483284 django_admin_background_task-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.723481 django_admin_background_task-0.3.0/bgtask/__init__.py
--rw-r--r--   0        0        0      965 2024-04-16 15:31:09.755506 django_admin_background_task-0.3.0/bgtask/admin.py
--rw-r--r--   0        0        0      144 2024-03-08 11:30:13.729684 django_admin_background_task-0.3.0/bgtask/apps.py
--rw-r--r--   0        0        0       57 2024-03-10 23:21:32.768101 django_admin_background_task-0.3.0/bgtask/backends/__init__.py
--rw-r--r--   0        0        0      304 2024-03-10 23:20:51.665708 django_admin_background_task-0.3.0/bgtask/backends/thread_pool.py
--rw-r--r--   0        0        0     1119 2024-04-16 15:15:56.816234 django_admin_background_task-0.3.0/bgtask/decorators.py
--rw-r--r--   0        0        0     2013 2024-03-08 11:30:13.719326 django_admin_background_task-0.3.0/bgtask/migrations/0001_initial.py
--rw-r--r--   0        0        0      968 2024-04-16 14:59:49.149350 django_admin_background_task-0.3.0/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.714396 django_admin_background_task-0.3.0/bgtask/migrations/__init__.py
--rw-r--r--   0        0        0     4402 2024-04-18 14:20:52.036965 django_admin_background_task-0.3.0/bgtask/model_admin.py
--rw-r--r--   0        0        0     9184 2024-04-18 15:16:23.546122 django_admin_background_task-0.3.0/bgtask/models.py
--rw-r--r--   0        0        0      231 2024-03-08 11:30:13.721685 django_admin_background_task-0.3.0/bgtask/stack_contexts.py
--rw-r--r--   0        0        0      746 2024-03-08 11:30:13.732726 django_admin_background_task-0.3.0/bgtask/static/bgtask/js/bgtask-once.js
--rw-r--r--   0        0        0    15026 2024-04-18 15:16:24.511343 django_admin_background_task-0.3.0/bgtask/static/bgtask/js/bgtask.js
--rw-r--r--   0        0        0     1053 2024-04-18 11:36:40.262228 django_admin_background_task-0.3.0/bgtask/templates/bgtask/admin/change_list.html
--rw-r--r--   0        0        0      844 2024-04-18 15:05:43.258568 django_admin_background_task-0.3.0/bgtask/templates/bgtask/bg_changelist_status_column.html
--rw-r--r--   0        0        0      788 2024-04-18 11:08:31.614024 django_admin_background_task-0.3.0/bgtask/templates/bgtask/bg_completed_column.html
--rw-r--r--   0        0        0        1 2024-03-08 11:30:13.737691 django_admin_background_task-0.3.0/bgtask/templates/bgtask/bgtask_templates.html
--rw-r--r--   0        0        0     1845 2024-03-08 11:30:13.736549 django_admin_background_task-0.3.0/bgtask/templates/bgtask/bgtask_view.html
--rw-r--r--   0        0        0      166 2024-03-08 11:30:13.735684 django_admin_background_task-0.3.0/bgtask/templates/bgtask/progress.html
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.710598 django_admin_background_task-0.3.0/bgtask/templatetags/__init__.py
--rw-r--r--   0        0        0      413 2024-03-08 11:30:13.710386 django_admin_background_task-0.3.0/bgtask/templatetags/bgtask.py
--rw-r--r--   0        0        0     1090 2024-03-08 11:30:13.723311 django_admin_background_task-0.3.0/bgtask/tests/test_bgtask.py
--rw-r--r--   0        0        0      161 2024-03-08 11:30:13.738363 django_admin_background_task-0.3.0/bgtask/urls.py
--rw-r--r--   0        0        0     1765 2024-04-18 09:56:48.293063 django_admin_background_task-0.3.0/bgtask/views.py
--rw-r--r--   0        0        0     1706 2024-04-18 15:14:53.319764 django_admin_background_task-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 django_admin_background_task-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-08 11:29:40.116270 django_admin_background_task-0.3.1/LICENSE
+-rw-r--r--   0        0        0      597 2024-03-08 15:24:11.483284 django_admin_background_task-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.723481 django_admin_background_task-0.3.1/bgtask/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-16 15:31:09.755506 django_admin_background_task-0.3.1/bgtask/admin.py
+-rw-r--r--   0        0        0      144 2024-03-08 11:30:13.729684 django_admin_background_task-0.3.1/bgtask/apps.py
+-rw-r--r--   0        0        0       57 2024-03-10 23:21:32.768101 django_admin_background_task-0.3.1/bgtask/backends/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-10 23:20:51.665708 django_admin_background_task-0.3.1/bgtask/backends/thread_pool.py
+-rw-r--r--   0        0        0     1119 2024-04-16 15:15:56.816234 django_admin_background_task-0.3.1/bgtask/decorators.py
+-rw-r--r--   0        0        0     2013 2024-03-08 11:30:13.719326 django_admin_background_task-0.3.1/bgtask/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2024-04-16 14:59:49.149350 django_admin_background_task-0.3.1/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.714396 django_admin_background_task-0.3.1/bgtask/migrations/__init__.py
+-rw-r--r--   0        0        0     4402 2024-04-18 14:20:52.036965 django_admin_background_task-0.3.1/bgtask/model_admin.py
+-rw-r--r--   0        0        0     9184 2024-04-18 15:16:23.546122 django_admin_background_task-0.3.1/bgtask/models.py
+-rw-r--r--   0        0        0      231 2024-03-08 11:30:13.721685 django_admin_background_task-0.3.1/bgtask/stack_contexts.py
+-rw-r--r--   0        0        0      746 2024-03-08 11:30:13.732726 django_admin_background_task-0.3.1/bgtask/static/bgtask/js/bgtask-once.js
+-rw-r--r--   0        0        0    15026 2024-04-18 15:16:24.511343 django_admin_background_task-0.3.1/bgtask/static/bgtask/js/bgtask.js
+-rw-r--r--   0        0        0     1053 2024-04-18 11:36:40.262228 django_admin_background_task-0.3.1/bgtask/templates/bgtask/admin/change_list.html
+-rw-r--r--   0        0        0      844 2024-04-18 15:05:43.258568 django_admin_background_task-0.3.1/bgtask/templates/bgtask/bg_changelist_status_column.html
+-rw-r--r--   0        0        0      788 2024-04-18 11:08:31.614024 django_admin_background_task-0.3.1/bgtask/templates/bgtask/bg_completed_column.html
+-rw-r--r--   0        0        0        1 2024-03-08 11:30:13.737691 django_admin_background_task-0.3.1/bgtask/templates/bgtask/bgtask_templates.html
+-rw-r--r--   0        0        0     1845 2024-03-08 11:30:13.736549 django_admin_background_task-0.3.1/bgtask/templates/bgtask/bgtask_view.html
+-rw-r--r--   0        0        0      166 2024-03-08 11:30:13.735684 django_admin_background_task-0.3.1/bgtask/templates/bgtask/progress.html
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.710598 django_admin_background_task-0.3.1/bgtask/templatetags/__init__.py
+-rw-r--r--   0        0        0      413 2024-03-08 11:30:13.710386 django_admin_background_task-0.3.1/bgtask/templatetags/bgtask.py
+-rw-r--r--   0        0        0     1090 2024-03-08 11:30:13.723311 django_admin_background_task-0.3.1/bgtask/tests/test_bgtask.py
+-rw-r--r--   0        0        0      161 2024-03-08 11:30:13.738363 django_admin_background_task-0.3.1/bgtask/urls.py
+-rw-r--r--   0        0        0     1765 2024-04-18 09:56:48.293063 django_admin_background_task-0.3.1/bgtask/views.py
+-rw-r--r--   0        0        0     1686 2024-04-24 14:09:34.924623 django_admin_background_task-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 django_admin_background_task-0.3.1/PKG-INFO
```

### Comparing `django_admin_background_task-0.3.0/LICENSE` & `django_admin_background_task-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/README.md` & `django_admin_background_task-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/admin.py` & `django_admin_background_task-0.3.1/bgtask/admin.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/decorators.py` & `django_admin_background_task-0.3.1/bgtask/decorators.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/migrations/0001_initial.py` & `django_admin_background_task-0.3.1/bgtask/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py` & `django_admin_background_task-0.3.1/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/model_admin.py` & `django_admin_background_task-0.3.1/bgtask/model_admin.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/models.py` & `django_admin_background_task-0.3.1/bgtask/models.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/static/bgtask/js/bgtask-once.js` & `django_admin_background_task-0.3.1/bgtask/static/bgtask/js/bgtask-once.js`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/static/bgtask/js/bgtask.js` & `django_admin_background_task-0.3.1/bgtask/static/bgtask/js/bgtask.js`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/templates/bgtask/admin/change_list.html` & `django_admin_background_task-0.3.1/bgtask/templates/bgtask/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/templates/bgtask/bg_changelist_status_column.html` & `django_admin_background_task-0.3.1/bgtask/templates/bgtask/bg_changelist_status_column.html`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/templates/bgtask/bg_completed_column.html` & `django_admin_background_task-0.3.1/bgtask/templates/bgtask/bg_completed_column.html`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/templates/bgtask/bgtask_view.html` & `django_admin_background_task-0.3.1/bgtask/templates/bgtask/bgtask_view.html`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/tests/test_bgtask.py` & `django_admin_background_task-0.3.1/bgtask/tests/test_bgtask.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/bgtask/views.py` & `django_admin_background_task-0.3.1/bgtask/views.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.3.0/pyproject.toml` & `django_admin_background_task-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-admin-background-task"
-version = "0.3.0"
+version = "0.3.1"
 description = "A set of tools for django apps to persist and monitor the status of background tasks"
 authors = [
     "David Park <david@greenparksoftware.co.uk>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/daphtdazz/django-bgtask"
@@ -21,15 +21,14 @@
 # These are the minimum versions that are supported. To build a file for testing a specific combination
 # of versions use build_versioned_pyproject using one of the pre-defined sets of dependencies in
 # test_version_combinations.
 # TEST VERSIONS INSERTION POINT
 Django = "~4.2"
 django-model-utils = "~4.4.0"
 # TEST VERSIONS INSERTION POINT END
-psycopg2 = "^2.9.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.0.1"
 syrupy = ">=4.6.0"
 pytest-django = ">=4.2.0"
 pytest-mock = ">=3.6.0"
 black = ">=24.2.0"
```

### Comparing `django_admin_background_task-0.3.0/PKG-INFO` & `django_admin_background_task-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: django-admin-background-task
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of tools for django apps to persist and monitor the status of background tasks
 Home-page: https://github.com/daphtdazz/django-bgtask
 License: Apache-2.0
 Author: David Park
 Author-email: david@greenparksoftware.co.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Requires-Dist: Django (>=4.2,<4.3) ; extra == "all"
 Requires-Dist: django-model-utils (>=4.4.0,<4.5.0)
-Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Project-URL: Repository, https://github.com/daphtdazz/django-bgtask
 Description-Content-Type: text/markdown
 
 # django-bgtask
 
 Background task monitoring tool for django apps
```

