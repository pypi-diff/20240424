# Comparing `tmp/py3seed-0.6.4.tar.gz` & `tmp/py3seed-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.6.4.tar", last modified: Thu Dec 14 02:44:36 2023, max compression
+gzip compressed data, was "py3seed-0.6.5.tar", last modified: Wed Apr 24 07:30:34 2024, max compression
```

## Comparing `py3seed-0.6.4.tar` & `py3seed-0.6.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-12-14 02:44:36.128910 py3seed-0.6.4/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.6.4/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      978 2023-12-14 02:44:36.128782 py3seed-0.6.4/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.6.4/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.6.4/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      925 2023-12-14 02:44:36.129515 py3seed-0.6.4/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.6.4/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-12-14 02:44:36.103840 py3seed-0.6.4/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-12-14 02:44:36.118989 py3seed-0.6.4/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      762 2023-08-15 08:24:22.000000 py3seed-0.6.4/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.6.4/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.6.4/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     8285 2023-12-08 02:46:38.000000 py3seed-0.6.4/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-12-14 02:44:36.122774 py3seed-0.6.4/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.6.4/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    25865 2023-12-14 02:22:04.000000 py3seed-0.6.4/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.6.4/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4272 2023-08-11 02:16:21.000000 py3seed-0.6.4/src/py3seed/ext.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.6.4/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.6.4/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.6.4/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    58526 2023-12-14 02:44:15.000000 py3seed-0.6.4/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14779 2023-12-08 02:47:42.000000 py3seed-0.6.4/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    15193 2023-12-11 08:08:55.000000 py3seed-0.6.4/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    10098 2023-12-07 08:30:01.000000 py3seed-0.6.4/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-12-14 02:44:36.128332 py3seed-0.6.4/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      978 2023-12-14 02:44:36.000000 py3seed-0.6.4/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      762 2023-12-14 02:44:36.000000 py3seed-0.6.4/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-12-14 02:44:36.000000 py3seed-0.6.4/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-12-14 02:44:36.000000 py3seed-0.6.4/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       59 2023-12-14 02:44:36.000000 py3seed-0.6.4/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-12-14 02:44:36.000000 py3seed-0.6.4/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-12-14 02:44:36.127580 py3seed-0.6.4/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     4386 2023-12-06 02:47:57.000000 py3seed-0.6.4/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7115 2023-08-10 09:14:34.000000 py3seed-0.6.4/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.6.4/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5286 2023-08-09 06:44:01.000000 py3seed-0.6.4/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2080 2023-12-08 02:08:48.000000 py3seed-0.6.4/tests/test_mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2504 2023-12-07 08:27:56.000000 py3seed-0.6.4/tests/test_websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.705231 py3seed-0.6.5/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.6.5/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      978 2024-04-24 07:30:34.705000 py3seed-0.6.5/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.6.5/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.6.5/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      925 2024-04-24 07:30:34.706529 py3seed-0.6.5/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.6.5/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.675482 py3seed-0.6.5/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.691149 py3seed-0.6.5/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      762 2023-08-15 08:24:22.000000 py3seed-0.6.5/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.6.5/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.6.5/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     8285 2023-12-08 02:46:38.000000 py3seed-0.6.5/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.696456 py3seed-0.6.5/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.6.5/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    26101 2024-04-24 03:39:28.000000 py3seed-0.6.5/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.6.5/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4272 2023-08-11 02:16:21.000000 py3seed-0.6.5/src/py3seed/ext.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.6.5/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.6.5/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.6.5/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    58526 2023-12-14 02:44:15.000000 py3seed-0.6.5/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14779 2023-12-08 02:47:42.000000 py3seed-0.6.5/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    15254 2024-04-24 03:35:30.000000 py3seed-0.6.5/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    10098 2023-12-07 08:30:01.000000 py3seed-0.6.5/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.704178 py3seed-0.6.5/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      978 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      762 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       59 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2024-04-24 07:30:34.000000 py3seed-0.6.5/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2024-04-24 07:30:34.703146 py3seed-0.6.5/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     4386 2023-12-06 02:47:57.000000 py3seed-0.6.5/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7430 2024-04-24 07:26:40.000000 py3seed-0.6.5/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.6.5/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5286 2023-08-09 06:44:01.000000 py3seed-0.6.5/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2080 2023-12-08 02:08:48.000000 py3seed-0.6.5/tests/test_mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2504 2023-12-07 08:27:56.000000 py3seed-0.6.5/tests/test_websupport.py
```

### Comparing `py3seed-0.6.4/LICENSE` & `py3seed-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/PKG-INFO` & `py3seed-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.6.4/setup.cfg` & `py3seed-0.6.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.6.4
+version = 0.6.5
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.6.4/src/py3seed/__init__.py` & `py3seed-0.6.5/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/__main__.py` & `py3seed-0.6.5/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/admin.py` & `py3seed-0.6.5/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/cachesupport.py` & `py3seed-0.6.5/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/commands/gen.py` & `py3seed-0.6.5/src/py3seed/commands/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,16 @@
         logger.info(f'Gen for domain {domain}')
         results[domain] = {}
         #
         # Parse .pyseed-includes in current folder, files whose name ends with jinja2 and folders whose name contains syntax {{ should be included
         # e.g,
         #   www/static/js/enums.js.jinja2
         #   www/templates/{{#blueprints}}
-        #   www/views/{{#blueprints}}.stub.py.jinja2
+        #   www/blueprints/__init__.py.jinja2
+        #   www/blueprints/{{#blueprints}}.py.jinja2
         #
         includes_file = '.pyseed-includes'
         includes = []
         logger.info('Includes:')
         with open(includes_file) as file:
             for line in file:
                 line = line.strip()
@@ -513,14 +514,17 @@
         with work_in(abs_o_base):
             logger.info(f'Working at {abs_o_base}')
             # Set jinja2's path
             env.loader = FileSystemLoader('.')
             #
             for i, o_name in enumerate(out_names):
                 o_file_raw = o_name.replace('.jinja2', '')
+                # Python file namimg convention, e.g, pub-demo.py -> pub_demp.py
+                if o_file_raw.endswith('.py'):
+                    o_file_raw = o_file_raw.replace('-', '_')
                 #
                 # AutoMerge
                 # Check if output with additional suffix exsit, if yes, go into below merging logic, otherwise, render(overwrite) directly
                 #
                 # - Output name with additional suffix .0:
                 # A simple way to preserve custom code, always generate code to the file with suffix .0
                 # e,g,
```

### Comparing `py3seed-0.6.4/src/py3seed/error.py` & `py3seed-0.6.5/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/ext.py` & `py3seed-0.6.5/src/py3seed/ext.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/inflection.py` & `py3seed-0.6.5/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/log.py` & `py3seed-0.6.5/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/merge3.py` & `py3seed-0.6.5/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/model.py` & `py3seed-0.6.5/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/mongosupport.py` & `py3seed-0.6.5/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed/utils.py` & `py3seed-0.6.5/src/py3seed/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,17 @@
         name_hyphen = re.sub(r'[.,?=#+]', '-', ''.join(name.split()))  # e.g, plan.members-form -> plan-members-form
         name_snake = inflection.underscore(name_hyphen)
         name_kebab = inflection.dasherize(name_snake)
         name_title = inflection.titleize(name_hyphen)
         return {
             'name': name,  # => SampleModel
             'name_lower': name.lower(),  # => samplemodel
-            'name_snake': name_snake,  # => sample_model
+            'name_snake': name_snake,  # => sample_model, e.g, python package&module name
             'name_snake_plural': inflection.pluralize(name_snake),  # => sample_models
-            'name_kebab': name_kebab,  # => sample-model
+            'name_kebab': name_kebab,  # => sample-model, e.g, html folder&file name
             'name_kebab_plural': inflection.pluralize(name_kebab),  # => sample-models
             'name_title': name_title,  # => Sample Model
             'name_title_lower': name_title.lower(),  # => sample model
             'name_title_lower_plural': inflection.pluralize(name_title.lower()),  # => sample models
         }
```

### Comparing `py3seed-0.6.4/src/py3seed/websupport.py` & `py3seed-0.6.5/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.6.5/src/py3seed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.6.4/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.6.5/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/tests/test_cachesupport.py` & `py3seed-0.6.5/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/tests/test_gen.py` & `py3seed-0.6.5/tests/test_gen.py`

 * *Files 9% similar despite different names*

```diff
@@ -114,14 +114,16 @@
     #
     # Prepare team-members.html*, which is used to test 3-way merge with conflicts
     # We need to remove the outstanding files generated in last test run
     try:
         os.remove('www/templates/public/team-members.html.BASE')
         os.remove('www/templates/public/team-members.html.THIS')
         os.remove('www/templates/public/team-members.html.OTHER')
+        #
+        os.remove('www/views/admin_demo.py')
     except FileNotFoundError:
         pass
     # Then manually init BASE and THIS file, otherwise then will be overwritten during each test
     base = '''<html>
 <head>
     <title>Members</title>
 </head>
@@ -221,14 +223,18 @@
 //
 
 var global_enums = {
 UserStatus: {'normal': 'Normal', 'rejected': 'Rejected'},
 UserRole: {1: 'Member', 2: 'Editor', 9: 'Admin'},
 }
 '''
+    # py naming convention, for blueprint whose name is kebab-case, e.g, www://admin-demo/user-list
+    # when {{#blueprint}}.py.jinja2 is rendered, the file name should be admin_demo.py, instead of admin-demo.py
+    assert os.path.exists('www/views/admin_demo.py')
+
     # global functions
-    render_env_txt = open('www/templates/public/render_env.txt', encoding='utf-8').read()
+    render_env_txt = open('www/templates/render_env.txt', encoding='utf-8').read()
     assert 'iamhere.html: True' in render_env_txt
     assert 'User title fields: [\'name\']' in render_env_txt
     assert 'User title field: name' in render_env_txt
     assert 'text_welcome: 欢迎' in render_env_txt
     assert '$text_welcome: 欢迎' in render_env_txt
```

### Comparing `py3seed-0.6.4/tests/test_merge3.py` & `py3seed-0.6.5/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/tests/test_model.py` & `py3seed-0.6.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/tests/test_mongosupport.py` & `py3seed-0.6.5/tests/test_mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.6.4/tests/test_websupport.py` & `py3seed-0.6.5/tests/test_websupport.py`

 * *Files identical despite different names*

