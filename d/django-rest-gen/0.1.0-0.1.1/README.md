# Comparing `tmp/django_rest_gen-0.1.0.tar.gz` & `tmp/django_rest_gen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rest_gen-0.1.0.tar", last modified: Tue Apr 23 18:08:42 2024, max compression
+gzip compressed data, was "django_rest_gen-0.1.1.tar", last modified: Tue Apr 23 19:56:21 2024, max compression
```

## Comparing `django_rest_gen-0.1.0.tar` & `django_rest_gen-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.837767 django_rest_gen-0.1.0/
--rw-r--r--   0 aalobaid   (501) staff       (20)    11357 2023-09-15 17:27:36.000000 django_rest_gen-0.1.0/LICENSE
--rw-r--r--   0 aalobaid   (501) staff       (20)     1820 2024-04-23 18:08:42.837586 django_rest_gen-0.1.0/PKG-INFO
--rw-r--r--   0 aalobaid   (501) staff       (20)     1299 2024-04-23 15:59:50.000000 django_rest_gen-0.1.0/README.md
--rw-r--r--   0 aalobaid   (501) staff       (20)      594 2024-04-23 18:08:24.000000 django_rest_gen-0.1.0/pyproject.toml
--rw-r--r--   0 aalobaid   (501) staff       (20)       38 2024-04-23 18:08:42.837812 django_rest_gen-0.1.0/setup.cfg
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.834946 django_rest_gen-0.1.0/src/
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.836373 django_rest_gen-0.1.0/src/django_rest_gen/
--rw-r--r--   0 aalobaid   (501) staff       (20)        0 2023-09-15 17:31:56.000000 django_rest_gen-0.1.0/src/django_rest_gen/__init__.py
--rw-r--r--   0 aalobaid   (501) staff       (20)      961 2023-09-19 13:33:46.000000 django_rest_gen-0.1.0/src/django_rest_gen/__main__.py
--rw-r--r--   0 aalobaid   (501) staff       (20)    10461 2024-04-22 17:00:14.000000 django_rest_gen-0.1.0/src/django_rest_gen/apigen.py
--rw-r--r--   0 aalobaid   (501) staff       (20)      319 2023-09-17 17:32:50.000000 django_rest_gen-0.1.0/src/django_rest_gen/utils.py
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.837381 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/
--rw-r--r--   0 aalobaid   (501) staff       (20)     1820 2024-04-23 18:08:42.000000 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/PKG-INFO
--rw-r--r--   0 aalobaid   (501) staff       (20)      352 2024-04-23 18:08:42.000000 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/SOURCES.txt
--rw-r--r--   0 aalobaid   (501) staff       (20)        1 2024-04-23 18:08:42.000000 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/dependency_links.txt
--rw-r--r--   0 aalobaid   (501) staff       (20)       16 2024-04-23 18:08:42.000000 django_rest_gen-0.1.0/src/django_rest_gen.egg-info/top_level.txt
-drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 18:08:42.837078 django_rest_gen-0.1.0/tests/
--rw-r--r--   0 aalobaid   (501) staff       (20)     3120 2024-04-23 15:49:34.000000 django_rest_gen-0.1.0/tests/test_serializer.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 19:56:21.608933 django_rest_gen-0.1.1/
+-rw-r--r--   0 aalobaid   (501) staff       (20)    11357 2023-09-15 17:27:36.000000 django_rest_gen-0.1.1/LICENSE
+-rw-r--r--   0 aalobaid   (501) staff       (20)     2155 2024-04-23 19:56:21.608749 django_rest_gen-0.1.1/PKG-INFO
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1634 2024-04-23 18:54:32.000000 django_rest_gen-0.1.1/README.md
+-rw-r--r--   0 aalobaid   (501) staff       (20)      594 2024-04-23 19:56:03.000000 django_rest_gen-0.1.1/pyproject.toml
+-rw-r--r--   0 aalobaid   (501) staff       (20)       38 2024-04-23 19:56:21.608978 django_rest_gen-0.1.1/setup.cfg
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 19:56:21.605389 django_rest_gen-0.1.1/src/
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 19:56:21.606924 django_rest_gen-0.1.1/src/django_rest_gen/
+-rw-r--r--   0 aalobaid   (501) staff       (20)        0 2023-09-15 17:31:56.000000 django_rest_gen-0.1.1/src/django_rest_gen/__init__.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)      963 2024-04-23 18:51:14.000000 django_rest_gen-0.1.1/src/django_rest_gen/__main__.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)    12473 2024-04-23 19:31:51.000000 django_rest_gen-0.1.1/src/django_rest_gen/apigen.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)      319 2023-09-17 17:32:50.000000 django_rest_gen-0.1.1/src/django_rest_gen/utils.py
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 19:56:21.608563 django_rest_gen-0.1.1/src/django_rest_gen.egg-info/
+-rw-r--r--   0 aalobaid   (501) staff       (20)     2155 2024-04-23 19:56:21.000000 django_rest_gen-0.1.1/src/django_rest_gen.egg-info/PKG-INFO
+-rw-r--r--   0 aalobaid   (501) staff       (20)      415 2024-04-23 19:56:21.000000 django_rest_gen-0.1.1/src/django_rest_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 aalobaid   (501) staff       (20)        1 2024-04-23 19:56:21.000000 django_rest_gen-0.1.1/src/django_rest_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 aalobaid   (501) staff       (20)       16 2024-04-23 19:56:21.000000 django_rest_gen-0.1.1/src/django_rest_gen.egg-info/top_level.txt
+drwxr-xr-x   0 aalobaid   (501) staff       (20)        0 2024-04-23 19:56:21.608181 django_rest_gen-0.1.1/tests/
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1969 2024-04-23 19:53:55.000000 django_rest_gen-0.1.1/tests/test_guess_app_path.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)     1893 2024-04-23 19:53:55.000000 django_rest_gen-0.1.1/tests/test_guess_settings_path.py
+-rw-r--r--   0 aalobaid   (501) staff       (20)     3120 2024-04-23 19:53:45.000000 django_rest_gen-0.1.1/tests/test_serializer.py
```

### Comparing `django_rest_gen-0.1.0/LICENSE` & `django_rest_gen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rest_gen-0.1.0/PKG-INFO` & `django_rest_gen-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-gen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rest API Code Generator
 Author-email: Ahmad Alobaid <ahmad88me@gmail.com>
 Project-URL: Homepage, https://github.com/ahmad88me/django-rest-gen
 Project-URL: Bug Tracker, https://github.com/ahmad88me/django-rest-gen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,29 +21,36 @@
 # How to use it
 1. Install it in your django project `pip install django-rest-gen`.
 2. Run it and specify your app `python -m django_rest_gen`. You should also
 specify the appropriate arguments (e.g., `python -m django_rest_gen  --settings iires/settings.py --apppath iirapp`)
 *Note: if the file already exists and is not empty, the content will be printed instead in the stdout*
 
 ## Arguments
-```
-usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
+``` 
+usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] [--settings SETTINGS] [--apppath APPPATH] [--overwrite] [--dummy]
 
 Generate Django REST API code
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --pythonpath PYTHONPATH
                         Python Path directory.
   --settings SETTINGS   The path to the django project settings
   --apppath APPPATH     The path to the app
   --overwrite           Whether to overwrite existing files if any
   --dummy               Whether to generate dummy data generator
+
 ```
 
+## Automatic detection
+If `--settings` and `--apppath` are not passed, it will try to detect them. It will look for anypath
+within your project that has `settings.py` to be the default settings path and any directory that has
+`models.py` to be the app path. You need to specify this in case you have multiple apps in your django 
+project.
+
 
 # Limitations
 * Flat. No nesting is provided as it depends on user preferences.
 
 
 # Rebuild package
 1. `python3 -m build`
```

### Comparing `django_rest_gen-0.1.0/README.md` & `django_rest_gen-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,36 @@
 # How to use it
 1. Install it in your django project `pip install django-rest-gen`.
 2. Run it and specify your app `python -m django_rest_gen`. You should also
 specify the appropriate arguments (e.g., `python -m django_rest_gen  --settings iires/settings.py --apppath iirapp`)
 *Note: if the file already exists and is not empty, the content will be printed instead in the stdout*
 
 ## Arguments
-```
-usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
+``` 
+usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] [--settings SETTINGS] [--apppath APPPATH] [--overwrite] [--dummy]
 
 Generate Django REST API code
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --pythonpath PYTHONPATH
                         Python Path directory.
   --settings SETTINGS   The path to the django project settings
   --apppath APPPATH     The path to the app
   --overwrite           Whether to overwrite existing files if any
   --dummy               Whether to generate dummy data generator
+
 ```
 
+## Automatic detection
+If `--settings` and `--apppath` are not passed, it will try to detect them. It will look for anypath
+within your project that has `settings.py` to be the default settings path and any directory that has
+`models.py` to be the app path. You need to specify this in case you have multiple apps in your django 
+project.
+
 
 # Limitations
 * Flat. No nesting is provided as it depends on user preferences.
 
 
 # Rebuild package
 1. `python3 -m build`
```

### Comparing `django_rest_gen-0.1.0/pyproject.toml` & `django_rest_gen-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-rest-gen"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Ahmad Alobaid", email="ahmad88me@gmail.com" },
 ]
 description = "Rest API Code Generator"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_rest_gen-0.1.0/src/django_rest_gen/__main__.py` & `django_rest_gen-0.1.1/src/django_rest_gen/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 import os
 from . import apigen
 
 
 def main():
-    parser = argparse.ArgumentParser(prog='django-rest-gen', description='Generate Django REST API code')
+    parser = argparse.ArgumentParser(prog='django_rest_gen', description='Generate Django REST API code')
     parser.add_argument('--pythonpath', default=".", help="Python Path directory. ")
-    parser.add_argument('--settings', required=True, help="The path to the django project settings")
-    parser.add_argument('--apppath', required=True, help="The path to the app")
+    parser.add_argument('--settings', required=False, help="The path to the django project settings")
+    parser.add_argument('--apppath', required=False, help="The path to the app")
     parser.add_argument('--overwrite', action='store_true',
                         help="Whether to overwrite existing files if any")
     parser.add_argument('--dummy', action='store_true',
                         help="Whether to generate dummy data generator")
     args = parser.parse_args()
     print(f"args: {args}")
     base_path = os.path.abspath('.')
```

### Comparing `django_rest_gen-0.1.0/src/django_rest_gen/apigen.py` & `django_rest_gen-0.1.1/src/django_rest_gen/apigen.py`

 * *Files 12% similar despite different names*

```diff
@@ -332,24 +332,98 @@
     if empty or overwrite:
         with open(dummy_path, "w") as f:
             f.write(content)
     else:
         print(content)
 
 
+def get_curr_path():
+    p = os.path.abspath(os.getcwd())
+    print(f"current path: {p}")
+    return p
+
+
+def guess_app_path(curr_path=None):
+    if not curr_path:
+        curr_path = get_curr_path()
+
+    dirs = []
+    files = dict()
+    for fp in os.listdir(curr_path):
+        fp_path = os.path.join(curr_path, fp)
+        if os.path.isdir(fp_path):
+            dirs.append(fp_path)
+        elif os.path.isfile(fp_path):
+            files[fp] = fp_path
+
+    if "models.py" in files: # and "views.py" in files:
+        with open(files["models.py"]) as f:
+            text = f.read()
+            if len(text) > 50:
+                return curr_path
+
+    for d in dirs:
+        guessed = guess_app_path(os.path.join(curr_path, d))
+        if guessed:
+            return guessed
+
+    return None
+
+
+def guess_settings_path(curr_path=None):
+    if not curr_path:
+        curr_path = get_curr_path()
+
+    print(f"DEBUG: curr_path: {curr_path}")
+    dirs = []
+    for fp in os.listdir(curr_path):
+        fp_path = os.path.join(curr_path, fp)
+        if os.path.isdir(fp_path):
+            print(f"DEBUG is dir: {fp_path}")
+            dirs.append(fp_path)
+        elif os.path.isfile(fp_path) and fp == "settings.py":
+            print(f"DEBUG: found path: {fp_path}")
+            return fp_path
+
+    print(f"DEBUG: path not found:")
+
+    for d in dirs:
+        print(f"Going into: {d}")
+        print(f"should be going to {os.path.join(curr_path, d)}")
+        guessed = guess_settings_path(d)
+        if guessed:
+            return guessed
+
+    return None
+
+
 def workflow(python_path, app_path, settings_fpath, overwrite, dummy):
     """
     This includes the main workflow of the API generator.
     :param python_path:
     :param app_path:
     :param settings_fpath:
     :param overwrite: bool
     :param dummy: bool
     :return:
     """
+    if not app_path:
+        app_path = guess_app_path()
+        if app_path is None:
+            raise Exception("Unable to detect app path.")
+        else:
+            print(f"Guessed app path: {app_path}")
+
+    if not settings_fpath:
+        settings_fpath = guess_settings_path()
+        if settings_fpath is None:
+            raise Exception("Unable to detect settings path")
+        else:
+            print(f"Guessed settings path: {settings_fpath}")
+
     models_fpath = os.path.join(app_path, "models.py")
     serializers_path = os.path.join(app_path, "serializers.py")
     views_path = os.path.join(app_path, "views.py")
     urls_path = os.path.join(app_path, "urls.py")
     admin_path = os.path.join(app_path, "admin.py")
     dummy_path = os.path.join(app_path, "dummygen.py")
     if overwrite:
```

### Comparing `django_rest_gen-0.1.0/src/django_rest_gen.egg-info/PKG-INFO` & `django_rest_gen-0.1.1/src/django_rest_gen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-gen
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rest API Code Generator
 Author-email: Ahmad Alobaid <ahmad88me@gmail.com>
 Project-URL: Homepage, https://github.com/ahmad88me/django-rest-gen
 Project-URL: Bug Tracker, https://github.com/ahmad88me/django-rest-gen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,29 +21,36 @@
 # How to use it
 1. Install it in your django project `pip install django-rest-gen`.
 2. Run it and specify your app `python -m django_rest_gen`. You should also
 specify the appropriate arguments (e.g., `python -m django_rest_gen  --settings iires/settings.py --apppath iirapp`)
 *Note: if the file already exists and is not empty, the content will be printed instead in the stdout*
 
 ## Arguments
-```
-usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] --settings SETTINGS --apppath APPPATH [--overwrite] [--dummy]
+``` 
+usage: django_rest_gen [-h] [--pythonpath PYTHONPATH] [--settings SETTINGS] [--apppath APPPATH] [--overwrite] [--dummy]
 
 Generate Django REST API code
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --pythonpath PYTHONPATH
                         Python Path directory.
   --settings SETTINGS   The path to the django project settings
   --apppath APPPATH     The path to the app
   --overwrite           Whether to overwrite existing files if any
   --dummy               Whether to generate dummy data generator
+
 ```
 
+## Automatic detection
+If `--settings` and `--apppath` are not passed, it will try to detect them. It will look for anypath
+within your project that has `settings.py` to be the default settings path and any directory that has
+`models.py` to be the app path. You need to specify this in case you have multiple apps in your django 
+project.
+
 
 # Limitations
 * Flat. No nesting is provided as it depends on user preferences.
 
 
 # Rebuild package
 1. `python3 -m build`
```

### Comparing `django_rest_gen-0.1.0/tests/test_serializer.py` & `django_rest_gen-0.1.1/tests/test_serializer.py`

 * *Files identical despite different names*

