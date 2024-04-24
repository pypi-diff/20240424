# Comparing `tmp/crumbly-1.2.tar.gz` & `tmp/crumbly-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crumbly-1.2.tar", last modified: Tue Sep 26 01:35:59 2023, max compression
+gzip compressed data, was "crumbly-1.2.1.tar", last modified: Wed Apr 24 00:28:38 2024, max compression
```

## Comparing `crumbly-1.2.tar` & `crumbly-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 01:35:59.192393 crumbly-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-09-26 01:35:49.000000 crumbly-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-09-26 01:35:59.192393 crumbly-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2023-09-26 01:35:49.000000 crumbly-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 01:35:59.192393 crumbly-1.2/crumbly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-09-26 01:35:59.000000 crumbly-1.2/crumbly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-09-26 01:35:59.000000 crumbly-1.2/crumbly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 01:35:59.000000 crumbly-1.2/crumbly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 01:35:59.000000 crumbly-1.2/crumbly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 01:35:59.192393 crumbly-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      895 2023-09-26 01:35:49.000000 crumbly-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:38.063997 crumbly-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 00:28:30.000000 crumbly-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-24 00:28:38.063997 crumbly-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-24 00:28:30.000000 crumbly-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:38.063997 crumbly-1.2.1/crumbly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-24 00:28:38.000000 crumbly-1.2.1/crumbly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 00:28:38.000000 crumbly-1.2.1/crumbly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:28:38.000000 crumbly-1.2.1/crumbly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:28:38.000000 crumbly-1.2.1/crumbly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:28:38.063997 crumbly-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-24 00:28:30.000000 crumbly-1.2.1/setup.py
```

### Comparing `crumbly-1.2/LICENSE` & `crumbly-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crumbly-1.2/PKG-INFO` & `crumbly-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: crumbly
-Version: 1.2
+Version: 1.2.1
 Summary: A Python library for versatile and user-friendly data storage and management.
-Home-page: https://github.com/noodledx/crumbly
-Author: NoodleDX
+Home-page: https://github.com/CapnSushiOfTheSea/crumbly
+Author: CapnSushiOfTheSea
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `crumbly-1.2/README.md` & `crumbly-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `crumbly-1.2/crumbly.egg-info/PKG-INFO` & `crumbly-1.2.1/crumbly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: crumbly
-Version: 1.2
+Version: 1.2.1
 Summary: A Python library for versatile and user-friendly data storage and management.
-Home-page: https://github.com/noodledx/crumbly
-Author: NoodleDX
+Home-page: https://github.com/CapnSushiOfTheSea/crumbly
+Author: CapnSushiOfTheSea
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `crumbly-1.2/setup.py` & `crumbly-1.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='crumbly',
-    version='1.2',
-    author='NoodleDX',
+    version='1.2.1',
+    author='CapnSushiOfTheSea',
     packages=find_packages(),
     description='A Python library for versatile and user-friendly data storage and management.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/noodledx/crumbly',
+    url='https://github.com/CapnSushiOfTheSea/crumbly',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

