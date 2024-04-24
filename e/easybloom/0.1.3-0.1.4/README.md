# Comparing `tmp/easybloom-0.1.3.tar.gz` & `tmp/easybloom-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybloom-0.1.3.tar", last modified: Wed Apr 24 00:40:38 2024, max compression
+gzip compressed data, was "easybloom-0.1.4.tar", last modified: Wed Apr 24 12:13:14 2024, max compression
```

## Comparing `easybloom-0.1.3.tar` & `easybloom-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:40:38.263469 easybloom-0.1.3/
--rw-r--r--   0 pohie      (501) staff       (20)     1211 2024-04-23 23:41:16.000000 easybloom-0.1.3/LICENSE.txt
--rw-r--r--   0 pohie      (501) staff       (20)      805 2024-04-24 00:40:38.263222 easybloom-0.1.3/PKG-INFO
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:40:38.262686 easybloom-0.1.3/easybloom.egg-info/
--rw-r--r--   0 pohie      (501) staff       (20)      805 2024-04-24 00:40:38.000000 easybloom-0.1.3/easybloom.egg-info/PKG-INFO
--rw-r--r--   0 pohie      (501) staff       (20)      204 2024-04-24 00:40:38.000000 easybloom-0.1.3/easybloom.egg-info/SOURCES.txt
--rw-r--r--   0 pohie      (501) staff       (20)        1 2024-04-24 00:40:38.000000 easybloom-0.1.3/easybloom.egg-info/dependency_links.txt
--rw-r--r--   0 pohie      (501) staff       (20)        9 2024-04-24 00:40:38.000000 easybloom-0.1.3/easybloom.egg-info/requires.txt
--rw-r--r--   0 pohie      (501) staff       (20)        8 2024-04-24 00:40:38.000000 easybloom-0.1.3/easybloom.egg-info/top_level.txt
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:40:38.262812 easybloom-0.1.3/ezbloom/
--rw-r--r--   0 pohie      (501) staff       (20)     2953 2024-04-24 00:17:32.000000 easybloom-0.1.3/ezbloom/__init__.py
--rw-r--r--   0 pohie      (501) staff       (20)       38 2024-04-24 00:40:38.263518 easybloom-0.1.3/setup.cfg
--rw-r--r--   0 pohie      (501) staff       (20)      965 2024-04-24 00:40:36.000000 easybloom-0.1.3/setup.py
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 12:13:14.839355 easybloom-0.1.4/
+-rw-r--r--   0 pohie      (501) staff       (20)     1211 2024-04-23 23:41:16.000000 easybloom-0.1.4/LICENSE.txt
+-rw-r--r--   0 pohie      (501) staff       (20)      813 2024-04-24 12:13:14.839149 easybloom-0.1.4/PKG-INFO
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 12:13:14.838673 easybloom-0.1.4/easybloom.egg-info/
+-rw-r--r--   0 pohie      (501) staff       (20)      813 2024-04-24 12:13:14.000000 easybloom-0.1.4/easybloom.egg-info/PKG-INFO
+-rw-r--r--   0 pohie      (501) staff       (20)      204 2024-04-24 12:13:14.000000 easybloom-0.1.4/easybloom.egg-info/SOURCES.txt
+-rw-r--r--   0 pohie      (501) staff       (20)        1 2024-04-24 12:13:14.000000 easybloom-0.1.4/easybloom.egg-info/dependency_links.txt
+-rw-r--r--   0 pohie      (501) staff       (20)        9 2024-04-24 12:13:14.000000 easybloom-0.1.4/easybloom.egg-info/requires.txt
+-rw-r--r--   0 pohie      (501) staff       (20)        8 2024-04-24 12:13:14.000000 easybloom-0.1.4/easybloom.egg-info/top_level.txt
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 12:13:14.838787 easybloom-0.1.4/ezbloom/
+-rw-r--r--   0 pohie      (501) staff       (20)     2953 2024-04-24 00:17:32.000000 easybloom-0.1.4/ezbloom/__init__.py
+-rw-r--r--   0 pohie      (501) staff       (20)       38 2024-04-24 12:13:14.839397 easybloom-0.1.4/setup.cfg
+-rw-r--r--   0 pohie      (501) staff       (20)      997 2024-04-24 12:13:10.000000 easybloom-0.1.4/setup.py
```

### Comparing `easybloom-0.1.3/LICENSE.txt` & `easybloom-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easybloom-0.1.3/PKG-INFO` & `easybloom-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: easybloom
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simplifies using bloom ai. Brings it down to only 1 line of code.
 Author: Abbott Broughton
 Author-email: abbottbroughton@icloud.com
 License: The Unlicense
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 Requires-Dist: requests
 
 Use ezbloom.bloom_ans() to ask bloom questions like a chatbot.
-For example, to ask bloom "Whats a unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use ezbloom.bloom_gen() togenerate the rest of a story you give it. It uses the same syntax as ezbloom.bloom_ans().
+For example, to ask bloom "Whats a unicorn?" you would do this: ezbloom.bloom_ans("Whats a unicorn?") and you can use ezbloom.bloom_gen() togenerate the rest of a story you give it. It uses the same syntax as ezbloom.bloom_ans().
```

### Comparing `easybloom-0.1.3/easybloom.egg-info/PKG-INFO` & `easybloom-0.1.4/easybloom.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: easybloom
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simplifies using bloom ai. Brings it down to only 1 line of code.
 Author: Abbott Broughton
 Author-email: abbottbroughton@icloud.com
 License: The Unlicense
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 Requires-Dist: requests
 
 Use ezbloom.bloom_ans() to ask bloom questions like a chatbot.
-For example, to ask bloom "Whats a unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use ezbloom.bloom_gen() togenerate the rest of a story you give it. It uses the same syntax as ezbloom.bloom_ans().
+For example, to ask bloom "Whats a unicorn?" you would do this: ezbloom.bloom_ans("Whats a unicorn?") and you can use ezbloom.bloom_gen() togenerate the rest of a story you give it. It uses the same syntax as ezbloom.bloom_ans().
```

### Comparing `easybloom-0.1.3/ezbloom/__init__.py` & `easybloom-0.1.4/ezbloom/__init__.py`

 * *Files identical despite different names*

### Comparing `easybloom-0.1.3/setup.py` & `easybloom-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup
 
 setup(
     name='easybloom',
-    version='0.1.3',
+    version='0.1.4',
     description='Simplifies using bloom ai. Brings it down to only 1 line of code.',
     author='Abbott Broughton',
     author_email='abbottbroughton@icloud.com',
     license='The Unlicense',
     packages=['ezbloom'],
     install_requires=['requests'],
     long_description='Use ezbloom.bloom_ans() to ask bloom questions like a chatbot.\nFor example, to ask bloom "Whats a '
-                     'unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use ezbloom.bloom_gen() to'
+                     'unicorn?" you would do this: ezbloom.bloom_ans("Whats a unicorn?") and you can use '
+                     'ezbloom.bloom_gen() to'
                      'generate the rest of a story you give it. It uses the same syntax as ezbloom.bloom_ans().',
 
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

