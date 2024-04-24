# Comparing `tmp/easybloom-0.1.0.tar.gz` & `tmp/easybloom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybloom-0.1.0.tar", last modified: Wed Apr 24 00:27:03 2024, max compression
+gzip compressed data, was "easybloom-0.1.1.tar", last modified: Wed Apr 24 00:29:37 2024, max compression
```

## Comparing `easybloom-0.1.0.tar` & `easybloom-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:27:03.095464 easybloom-0.1.0/
--rw-r--r--   0 pohie      (501) staff       (20)     1211 2024-04-23 23:41:16.000000 easybloom-0.1.0/LICENSE.txt
--rw-r--r--   0 pohie      (501) staff       (20)      830 2024-04-24 00:27:03.095236 easybloom-0.1.0/PKG-INFO
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:27:03.094733 easybloom-0.1.0/easybloom.egg-info/
--rw-r--r--   0 pohie      (501) staff       (20)      830 2024-04-24 00:27:03.000000 easybloom-0.1.0/easybloom.egg-info/PKG-INFO
--rw-r--r--   0 pohie      (501) staff       (20)      204 2024-04-24 00:27:03.000000 easybloom-0.1.0/easybloom.egg-info/SOURCES.txt
--rw-r--r--   0 pohie      (501) staff       (20)        1 2024-04-24 00:27:03.000000 easybloom-0.1.0/easybloom.egg-info/dependency_links.txt
--rw-r--r--   0 pohie      (501) staff       (20)        9 2024-04-24 00:27:03.000000 easybloom-0.1.0/easybloom.egg-info/requires.txt
--rw-r--r--   0 pohie      (501) staff       (20)        8 2024-04-24 00:27:03.000000 easybloom-0.1.0/easybloom.egg-info/top_level.txt
-drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:27:03.094870 easybloom-0.1.0/ezbloom/
--rw-r--r--   0 pohie      (501) staff       (20)     2953 2024-04-24 00:17:32.000000 easybloom-0.1.0/ezbloom/__init__.py
--rw-r--r--   0 pohie      (501) staff       (20)       38 2024-04-24 00:27:03.095512 easybloom-0.1.0/setup.cfg
--rw-r--r--   0 pohie      (501) staff       (20)      990 2024-04-24 00:26:56.000000 easybloom-0.1.0/setup.py
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:29:37.317118 easybloom-0.1.1/
+-rw-r--r--   0 pohie      (501) staff       (20)     1211 2024-04-23 23:41:16.000000 easybloom-0.1.1/LICENSE.txt
+-rw-r--r--   0 pohie      (501) staff       (20)      845 2024-04-24 00:29:37.316901 easybloom-0.1.1/PKG-INFO
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:29:37.316532 easybloom-0.1.1/easybloom.egg-info/
+-rw-r--r--   0 pohie      (501) staff       (20)      845 2024-04-24 00:29:37.000000 easybloom-0.1.1/easybloom.egg-info/PKG-INFO
+-rw-r--r--   0 pohie      (501) staff       (20)      204 2024-04-24 00:29:37.000000 easybloom-0.1.1/easybloom.egg-info/SOURCES.txt
+-rw-r--r--   0 pohie      (501) staff       (20)        1 2024-04-24 00:29:37.000000 easybloom-0.1.1/easybloom.egg-info/dependency_links.txt
+-rw-r--r--   0 pohie      (501) staff       (20)        9 2024-04-24 00:29:37.000000 easybloom-0.1.1/easybloom.egg-info/requires.txt
+-rw-r--r--   0 pohie      (501) staff       (20)        8 2024-04-24 00:29:37.000000 easybloom-0.1.1/easybloom.egg-info/top_level.txt
+drwxr-xr-x   0 pohie      (501) staff       (20)        0 2024-04-24 00:29:37.316672 easybloom-0.1.1/ezbloom/
+-rw-r--r--   0 pohie      (501) staff       (20)     2953 2024-04-24 00:17:32.000000 easybloom-0.1.1/ezbloom/__init__.py
+-rw-r--r--   0 pohie      (501) staff       (20)       38 2024-04-24 00:29:37.317164 easybloom-0.1.1/setup.cfg
+-rw-r--r--   0 pohie      (501) staff       (20)     1005 2024-04-24 00:29:34.000000 easybloom-0.1.1/setup.py
```

### Comparing `easybloom-0.1.0/LICENSE.txt` & `easybloom-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easybloom-0.1.0/PKG-INFO` & `easybloom-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: easybloom
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simplifies using bloom ai. Brings it down to only 1 line of code.
 Home-page: https://github.com/shuds13/pyexample
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
 
-Use bloom_ans() to ask bloom questions like a chatbot.
-For example, to ask bloom "Whats a unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use bloom_gen() to generate the rest of a story you give it. It uses the same syntax as bloom_ans().
+Use ezbloom.bloom_ans() to ask bloom questions like a chatbot.
+For example, to ask bloom "Whats a unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use ezbloom.bloom_gen() togenerate the rest of a story you give it. It uses the same syntax as bloom_ans().
```

### Comparing `easybloom-0.1.0/easybloom.egg-info/PKG-INFO` & `easybloom-0.1.1/easybloom.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: easybloom
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simplifies using bloom ai. Brings it down to only 1 line of code.
 Home-page: https://github.com/shuds13/pyexample
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
 
-Use bloom_ans() to ask bloom questions like a chatbot.
-For example, to ask bloom "Whats a unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use bloom_gen() to generate the rest of a story you give it. It uses the same syntax as bloom_ans().
+Use ezbloom.bloom_ans() to ask bloom questions like a chatbot.
+For example, to ask bloom "Whats a unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use ezbloom.bloom_gen() togenerate the rest of a story you give it. It uses the same syntax as bloom_ans().
```

### Comparing `easybloom-0.1.0/ezbloom/__init__.py` & `easybloom-0.1.1/ezbloom/__init__.py`

 * *Files identical despite different names*

### Comparing `easybloom-0.1.0/setup.py` & `easybloom-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='easybloom',
-    version='0.1.0',
+    version='0.1.1',
     description='Simplifies using bloom ai. Brings it down to only 1 line of code.',
     url='https://github.com/shuds13/pyexample',
     author='Abbott Broughton',
     author_email='abbottbroughton@icloud.com',
     license='The Unlicense',
     packages=['ezbloom'],
     install_requires=['requests'],
-    long_description='Use bloom_ans() to ask bloom questions like a chatbot.\nFor example, to ask bloom "Whats a '
-                     'unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use bloom_gen() to '
+    long_description='Use ezbloom.bloom_ans() to ask bloom questions like a chatbot.\nFor example, to ask bloom "Whats a '
+                     'unicorn?" you would do this: bloom_ans("Whats a unicorn?") and you can use ezbloom.bloom_gen() to'
                      'generate the rest of a story you give it. It uses the same syntax as bloom_ans().',
 
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

