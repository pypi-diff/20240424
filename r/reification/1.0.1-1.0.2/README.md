# Comparing `tmp/reification-1.0.1.tar.gz` & `tmp/reification-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reification-1.0.1.tar", last modified: Wed Mar 20 16:28:32 2024, max compression
+gzip compressed data, was "reification-1.0.2.tar", last modified: Wed Apr 24 16:11:19 2024, max compression
```

## Comparing `reification-1.0.1.tar` & `reification-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-03-20 16:28:32.782104 reification-1.0.1/
--rw-r--r--   0 shunsuke   (501) staff       (20)      461 2024-03-20 16:16:28.000000 reification-1.0.1/LICENSE
--rw-r--r--   0 shunsuke   (501) staff       (20)     7073 2024-03-20 16:28:32.781875 reification-1.0.1/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)     6057 2024-03-20 16:16:28.000000 reification-1.0.1/README.md
--rw-r--r--   0 shunsuke   (501) staff       (20)     1060 2024-03-20 16:24:35.000000 reification-1.0.1/pyproject.toml
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-03-20 16:28:32.779968 reification-1.0.1/reification/
--rw-r--r--   0 shunsuke   (501) staff       (20)       71 2024-03-20 16:16:41.000000 reification-1.0.1/reification/__init__.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     2024 2024-03-20 16:16:28.000000 reification-1.0.1/reification/abs.py
--rw-r--r--   0 shunsuke   (501) staff       (20)      825 2024-03-20 16:16:28.000000 reification-1.0.1/reification/utils.py
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-03-20 16:28:32.781397 reification-1.0.1/reification.egg-info/
--rw-r--r--   0 shunsuke   (501) staff       (20)     7073 2024-03-20 16:28:32.000000 reification-1.0.1/reification.egg-info/PKG-INFO
--rw-r--r--   0 shunsuke   (501) staff       (20)      424 2024-03-20 16:28:32.000000 reification-1.0.1/reification.egg-info/SOURCES.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-03-20 16:28:32.000000 reification-1.0.1/reification.egg-info/dependency_links.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       45 2024-03-20 16:28:32.000000 reification-1.0.1/reification.egg-info/requires.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       12 2024-03-20 16:28:32.000000 reification-1.0.1/reification.egg-info/top_level.txt
--rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-03-20 16:28:32.782152 reification-1.0.1/setup.cfg
-drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-03-20 16:28:32.781216 reification-1.0.1/tests/
--rw-r--r--   0 shunsuke   (501) staff       (20)     1718 2024-03-20 16:16:28.000000 reification-1.0.1/tests/test_reified.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     3418 2024-03-20 16:16:28.000000 reification-1.0.1/tests/test_reified_dict.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     3346 2024-03-20 16:16:28.000000 reification-1.0.1/tests/test_reified_list.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     1232 2024-03-20 16:16:28.000000 reification-1.0.1/tests/test_reified_stack.py
--rw-r--r--   0 shunsuke   (501) staff       (20)      881 2024-03-20 16:16:28.000000 reification-1.0.1/tests/test_threading.py
--rw-r--r--   0 shunsuke   (501) staff       (20)     1535 2024-03-20 16:16:28.000000 reification-1.0.1/tests/test_type_basics.py
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-24 16:11:19.668536 reification-1.0.2/
+-rw-r--r--   0 shunsuke   (501) staff       (20)      461 2024-04-24 13:41:53.000000 reification-1.0.2/LICENSE
+-rw-r--r--   0 shunsuke   (501) staff       (20)     7073 2024-04-24 16:11:19.668320 reification-1.0.2/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)     6057 2024-04-24 13:41:53.000000 reification-1.0.2/README.md
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1060 2024-04-24 13:41:53.000000 reification-1.0.2/pyproject.toml
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-24 16:11:19.665505 reification-1.0.2/reification/
+-rw-r--r--   0 shunsuke   (501) staff       (20)       71 2024-04-24 14:12:42.000000 reification-1.0.2/reification/__init__.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     2024 2024-04-24 13:41:53.000000 reification-1.0.2/reification/abs.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)        0 2024-04-24 14:12:00.000000 reification-1.0.2/reification/py.typed
+-rw-r--r--   0 shunsuke   (501) staff       (20)      825 2024-04-24 13:41:53.000000 reification-1.0.2/reification/utils.py
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-24 16:11:19.667757 reification-1.0.2/reification.egg-info/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     7073 2024-04-24 16:11:19.000000 reification-1.0.2/reification.egg-info/PKG-INFO
+-rw-r--r--   0 shunsuke   (501) staff       (20)      445 2024-04-24 16:11:19.000000 reification-1.0.2/reification.egg-info/SOURCES.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)        1 2024-04-24 16:11:19.000000 reification-1.0.2/reification.egg-info/dependency_links.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       45 2024-04-24 16:11:19.000000 reification-1.0.2/reification.egg-info/requires.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       12 2024-04-24 16:11:19.000000 reification-1.0.2/reification.egg-info/top_level.txt
+-rw-r--r--   0 shunsuke   (501) staff       (20)       38 2024-04-24 16:11:19.668577 reification-1.0.2/setup.cfg
+drwxr-xr-x   0 shunsuke   (501) staff       (20)        0 2024-04-24 16:11:19.667573 reification-1.0.2/tests/
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1718 2024-04-24 13:41:53.000000 reification-1.0.2/tests/test_reified.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     3418 2024-04-24 13:41:53.000000 reification-1.0.2/tests/test_reified_dict.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     3346 2024-04-24 13:41:53.000000 reification-1.0.2/tests/test_reified_list.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1232 2024-04-24 13:41:53.000000 reification-1.0.2/tests/test_reified_stack.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)      881 2024-04-24 13:41:53.000000 reification-1.0.2/tests/test_threading.py
+-rw-r--r--   0 shunsuke   (501) staff       (20)     1535 2024-04-24 13:41:53.000000 reification-1.0.2/tests/test_type_basics.py
```

### Comparing `reification-1.0.1/PKG-INFO` & `reification-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reification
-Version: 1.0.1
+Version: 1.0.2
 Summary: Reified generics in Python to get type parameters at runtime
 Maintainer-email: curegit <contact@curegit.jp>
 License: WTFPL
 Project-URL: homepage, https://github.com/curegit/reification
 Project-URL: repository, https://github.com/curegit/reification.git
 Keywords: typing,generics,parametric polymorphism,reification,type parameter,reflection
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `reification-1.0.1/README.md` & `reification-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/pyproject.toml` & `reification-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/reification/abs.py` & `reification-1.0.2/reification/abs.py`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/reification/utils.py` & `reification-1.0.2/reification/utils.py`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/reification.egg-info/PKG-INFO` & `reification-1.0.2/reification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reification
-Version: 1.0.1
+Version: 1.0.2
 Summary: Reified generics in Python to get type parameters at runtime
 Maintainer-email: curegit <contact@curegit.jp>
 License: WTFPL
 Project-URL: homepage, https://github.com/curegit/reification
 Project-URL: repository, https://github.com/curegit/reification.git
 Keywords: typing,generics,parametric polymorphism,reification,type parameter,reflection
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `reification-1.0.1/tests/test_reified.py` & `reification-1.0.2/tests/test_reified.py`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/tests/test_reified_dict.py` & `reification-1.0.2/tests/test_reified_dict.py`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/tests/test_reified_list.py` & `reification-1.0.2/tests/test_reified_list.py`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/tests/test_reified_stack.py` & `reification-1.0.2/tests/test_reified_stack.py`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/tests/test_threading.py` & `reification-1.0.2/tests/test_threading.py`

 * *Files identical despite different names*

### Comparing `reification-1.0.1/tests/test_type_basics.py` & `reification-1.0.2/tests/test_type_basics.py`

 * *Files identical despite different names*

