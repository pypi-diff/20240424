# Comparing `tmp/simplesingletable-4.0.0.tar.gz` & `tmp/simplesingletable-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesingletable-4.0.0.tar", last modified: Tue Apr 16 16:36:03 2024, max compression
+gzip compressed data, was "simplesingletable-4.0.1.tar", last modified: Tue Apr 23 20:10:12 2024, max compression
```

## Comparing `simplesingletable-4.0.0.tar` & `simplesingletable-4.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-16 16:36:03.927348 simplesingletable-4.0.0/
--rw-r--r--   0 msull      (501) staff       (20)     1092 2023-10-16 15:46:21.000000 simplesingletable-4.0.0/LICENSE
--rw-r--r--   0 msull      (501) staff       (20)     5813 2024-04-16 16:36:03.926864 simplesingletable-4.0.0/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)     3278 2024-04-16 16:35:57.000000 simplesingletable-4.0.0/README.md
--rw-r--r--   0 msull      (501) staff       (20)     1924 2024-04-16 16:35:57.000000 simplesingletable-4.0.0/pyproject.toml
--rw-r--r--   0 msull      (501) staff       (20)       38 2024-04-16 16:36:03.927446 simplesingletable-4.0.0/setup.cfg
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-16 16:36:03.915047 simplesingletable-4.0.0/src/
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-16 16:36:03.917684 simplesingletable-4.0.0/src/simplesingletable/
--rw-r--r--   0 msull      (501) staff       (20)      288 2024-04-16 16:35:57.000000 simplesingletable-4.0.0/src/simplesingletable/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)    27017 2024-04-08 19:04:26.000000 simplesingletable-4.0.0/src/simplesingletable/dynamodb_memory.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-16 16:36:03.921361 simplesingletable-4.0.0/src/simplesingletable/extras/
--rw-r--r--   0 msull      (501) staff       (20)        0 2024-02-12 18:26:56.000000 simplesingletable-4.0.0/src/simplesingletable/extras/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)    22116 2024-04-16 16:34:34.000000 simplesingletable-4.0.0/src/simplesingletable/extras/form_data.py
--rw-r--r--   0 msull      (501) staff       (20)     1704 2024-02-12 19:18:43.000000 simplesingletable-4.0.0/src/simplesingletable/extras/singleton.py
--rw-r--r--   0 msull      (501) staff       (20)    12772 2024-03-18 18:58:28.000000 simplesingletable-4.0.0/src/simplesingletable/models.py
--rw-r--r--   0 msull      (501) staff       (20)     5351 2024-03-05 17:53:29.000000 simplesingletable-4.0.0/src/simplesingletable/utils.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-16 16:36:03.924145 simplesingletable-4.0.0/src/simplesingletable.egg-info/
--rw-r--r--   0 msull      (501) staff       (20)     5813 2024-04-16 16:36:03.000000 simplesingletable-4.0.0/src/simplesingletable.egg-info/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      664 2024-04-16 16:36:03.000000 simplesingletable-4.0.0/src/simplesingletable.egg-info/SOURCES.txt
--rw-r--r--   0 msull      (501) staff       (20)        1 2024-04-16 16:36:03.000000 simplesingletable-4.0.0/src/simplesingletable.egg-info/dependency_links.txt
--rw-r--r--   0 msull      (501) staff       (20)      214 2024-04-16 16:36:03.000000 simplesingletable-4.0.0/src/simplesingletable.egg-info/requires.txt
--rw-r--r--   0 msull      (501) staff       (20)       32 2024-04-16 16:36:03.000000 simplesingletable-4.0.0/src/simplesingletable.egg-info/top_level.txt
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-16 16:36:03.921747 simplesingletable-4.0.0/src/streamlit_app/
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-16 16:36:03.922112 simplesingletable-4.0.0/src/streamlit_app/pages/
--rw-r--r--   0 msull      (501) staff       (20)    13081 2024-03-18 19:07:04.000000 simplesingletable-4.0.0/src/streamlit_app/pages/Form Data demo.py
--rw-r--r--   0 msull      (501) staff       (20)     7517 2024-02-23 20:37:38.000000 simplesingletable-4.0.0/src/streamlit_app/streamlit_app.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-16 16:36:03.923285 simplesingletable-4.0.0/tests/
--rw-r--r--   0 msull      (501) staff       (20)     1091 2024-02-23 20:37:38.000000 simplesingletable-4.0.0/tests/test_nonversioned_resource.py
--rw-r--r--   0 msull      (501) staff       (20)     9155 2024-04-08 19:12:12.000000 simplesingletable-4.0.0/tests/test_simplesingletable.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-23 20:10:12.378365 simplesingletable-4.0.1/
+-rw-r--r--   0 msull      (501) staff       (20)     1092 2023-10-16 15:46:21.000000 simplesingletable-4.0.1/LICENSE
+-rw-r--r--   0 msull      (501) staff       (20)     5813 2024-04-23 20:10:12.377806 simplesingletable-4.0.1/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)     3278 2024-04-23 20:10:04.000000 simplesingletable-4.0.1/README.md
+-rw-r--r--   0 msull      (501) staff       (20)     1924 2024-04-23 20:10:04.000000 simplesingletable-4.0.1/pyproject.toml
+-rw-r--r--   0 msull      (501) staff       (20)       38 2024-04-23 20:10:12.378476 simplesingletable-4.0.1/setup.cfg
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-23 20:10:12.365120 simplesingletable-4.0.1/src/
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-23 20:10:12.368901 simplesingletable-4.0.1/src/simplesingletable/
+-rw-r--r--   0 msull      (501) staff       (20)      288 2024-04-23 20:10:04.000000 simplesingletable-4.0.1/src/simplesingletable/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)    27017 2024-04-08 19:04:26.000000 simplesingletable-4.0.1/src/simplesingletable/dynamodb_memory.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-23 20:10:12.372100 simplesingletable-4.0.1/src/simplesingletable/extras/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2024-02-12 18:26:56.000000 simplesingletable-4.0.1/src/simplesingletable/extras/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)    22331 2024-04-23 20:07:18.000000 simplesingletable-4.0.1/src/simplesingletable/extras/form_data.py
+-rw-r--r--   0 msull      (501) staff       (20)     1704 2024-02-12 19:18:43.000000 simplesingletable-4.0.1/src/simplesingletable/extras/singleton.py
+-rw-r--r--   0 msull      (501) staff       (20)    12772 2024-03-18 18:58:28.000000 simplesingletable-4.0.1/src/simplesingletable/models.py
+-rw-r--r--   0 msull      (501) staff       (20)     5351 2024-03-05 17:53:29.000000 simplesingletable-4.0.1/src/simplesingletable/utils.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-23 20:10:12.375095 simplesingletable-4.0.1/src/simplesingletable.egg-info/
+-rw-r--r--   0 msull      (501) staff       (20)     5813 2024-04-23 20:10:12.000000 simplesingletable-4.0.1/src/simplesingletable.egg-info/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      664 2024-04-23 20:10:12.000000 simplesingletable-4.0.1/src/simplesingletable.egg-info/SOURCES.txt
+-rw-r--r--   0 msull      (501) staff       (20)        1 2024-04-23 20:10:12.000000 simplesingletable-4.0.1/src/simplesingletable.egg-info/dependency_links.txt
+-rw-r--r--   0 msull      (501) staff       (20)      214 2024-04-23 20:10:12.000000 simplesingletable-4.0.1/src/simplesingletable.egg-info/requires.txt
+-rw-r--r--   0 msull      (501) staff       (20)       32 2024-04-23 20:10:12.000000 simplesingletable-4.0.1/src/simplesingletable.egg-info/top_level.txt
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-23 20:10:12.372495 simplesingletable-4.0.1/src/streamlit_app/
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-23 20:10:12.372879 simplesingletable-4.0.1/src/streamlit_app/pages/
+-rw-r--r--   0 msull      (501) staff       (20)    13081 2024-03-18 19:07:04.000000 simplesingletable-4.0.1/src/streamlit_app/pages/Form Data demo.py
+-rw-r--r--   0 msull      (501) staff       (20)     7517 2024-02-23 20:37:38.000000 simplesingletable-4.0.1/src/streamlit_app/streamlit_app.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-04-23 20:10:12.374112 simplesingletable-4.0.1/tests/
+-rw-r--r--   0 msull      (501) staff       (20)     1091 2024-02-23 20:37:38.000000 simplesingletable-4.0.1/tests/test_nonversioned_resource.py
+-rw-r--r--   0 msull      (501) staff       (20)     9155 2024-04-08 19:12:12.000000 simplesingletable-4.0.1/tests/test_simplesingletable.py
```

### Comparing `simplesingletable-4.0.0/LICENSE` & `simplesingletable-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/PKG-INFO` & `simplesingletable-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesingletable
-Version: 4.0.0
+Version: 4.0.1
 Summary: A simple boto3/Pydantic implementation of DynamoDB Single Table Design and related utilities.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -42,15 +42,15 @@
 Requires-Dist: watchdog; extra == "dev"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 # Simple Single Table
 
-**Latest Version:** 4.0.0
+**Latest Version:** 4.0.1
 
 **simplesingletable** is a Python library that offers an abstraction layer for AWS DynamoDB operations, particularly for
 those tables using single-table design. It uses Pydantic to define the models, and tries to be as "batteries-included"
 based on how I personally have come to use DynamoDb.
 
 I've used and written variations of this same code many times, and finally decided to try and package it all up into a
 single library I could pip install and use whenever I needed cheap, easy, fast storage with few access patterns. So far
```

### Comparing `simplesingletable-4.0.0/README.md` & `simplesingletable-4.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Simple Single Table
 
-**Latest Version:** 4.0.0
+**Latest Version:** 4.0.1
 
 **simplesingletable** is a Python library that offers an abstraction layer for AWS DynamoDB operations, particularly for
 those tables using single-table design. It uses Pydantic to define the models, and tries to be as "batteries-included"
 based on how I personally have come to use DynamoDb.
 
 I've used and written variations of this same code many times, and finally decided to try and package it all up into a
 single library I could pip install and use whenever I needed cheap, easy, fast storage with few access patterns. So far
```

### Comparing `simplesingletable-4.0.0/pyproject.toml` & `simplesingletable-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplesingletable"
-version = "4.0.0"
+version = "4.0.1"
 description = "A simple boto3/Pydantic implementation of DynamoDB Single Table Design and related utilities."
 readme = "README.md"
 authors = [{ name = "Sully", email = "sully@sadburger.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -57,15 +57,15 @@
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 
 [tool.bumpver]
-current_version = "4.0.0"
+current_version = "4.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `simplesingletable-4.0.0/src/simplesingletable/dynamodb_memory.py` & `simplesingletable-4.0.1/src/simplesingletable/dynamodb_memory.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/src/simplesingletable/extras/form_data.py` & `simplesingletable-4.0.1/src/simplesingletable/extras/form_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,21 @@
         self._data = None
 
         # use the specified group, or the first one
         self.active_group = ""
         self.switch_active_group(active_group or self.form.groups[0])
 
         if logger is None:
-            from logzero import logger
+            try:
+                from logzero import logger
+            except ImportError:
+                import logging
+
+                logging.basicConfig(level=logging.DEBUG)
+                logger = logging.getLogger(__file__)
 
         self.logger = logger
 
         if preload:
             self.load_data()
 
     def load_data(self, reload=False):
@@ -507,15 +513,15 @@
     def create_form(self, new_form: NewFormRequest) -> Form:
         return self.memory.create_new(Form, new_form)
 
     def update_form(self, existing_form: Form, update: UpdateFormRequest) -> Form:
         return self.memory.update_existing(existing_form, update)
 
     def get_mapping(self, existing_form: Form):
-        return FormDataMapping(form=existing_form, form_manager=self, preload=False)
+        return FormDataMapping(form=existing_form, form_manager=self, preload=False, logger=self.logger)
 
     def store_form_data(
         self,
         existing_form: Form,
         data: (
             StoredFormData
             | tuple[FormEntry | None, StoredFormData]
```

### Comparing `simplesingletable-4.0.0/src/simplesingletable/extras/singleton.py` & `simplesingletable-4.0.1/src/simplesingletable/extras/singleton.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/src/simplesingletable/models.py` & `simplesingletable-4.0.1/src/simplesingletable/models.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/src/simplesingletable/utils.py` & `simplesingletable-4.0.1/src/simplesingletable/utils.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/src/simplesingletable.egg-info/PKG-INFO` & `simplesingletable-4.0.1/src/simplesingletable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesingletable
-Version: 4.0.0
+Version: 4.0.1
 Summary: A simple boto3/Pydantic implementation of DynamoDB Single Table Design and related utilities.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -42,15 +42,15 @@
 Requires-Dist: watchdog; extra == "dev"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 # Simple Single Table
 
-**Latest Version:** 4.0.0
+**Latest Version:** 4.0.1
 
 **simplesingletable** is a Python library that offers an abstraction layer for AWS DynamoDB operations, particularly for
 those tables using single-table design. It uses Pydantic to define the models, and tries to be as "batteries-included"
 based on how I personally have come to use DynamoDb.
 
 I've used and written variations of this same code many times, and finally decided to try and package it all up into a
 single library I could pip install and use whenever I needed cheap, easy, fast storage with few access patterns. So far
```

### Comparing `simplesingletable-4.0.0/src/simplesingletable.egg-info/SOURCES.txt` & `simplesingletable-4.0.1/src/simplesingletable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/src/streamlit_app/pages/Form Data demo.py` & `simplesingletable-4.0.1/src/streamlit_app/pages/Form Data demo.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/src/streamlit_app/streamlit_app.py` & `simplesingletable-4.0.1/src/streamlit_app/streamlit_app.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/tests/test_nonversioned_resource.py` & `simplesingletable-4.0.1/tests/test_nonversioned_resource.py`

 * *Files identical despite different names*

### Comparing `simplesingletable-4.0.0/tests/test_simplesingletable.py` & `simplesingletable-4.0.1/tests/test_simplesingletable.py`

 * *Files identical despite different names*

