# Comparing `tmp/mojo_collections-1.3.6.tar.gz` & `tmp/mojo_collections-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_collections-1.3.6.tar", max compression
+gzip compressed data, was "mojo_collections-1.3.7.tar", max compression
```

## Comparing `mojo_collections-1.3.6.tar` & `mojo_collections-1.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:55:06.310687 mojo_collections-1.3.6/LICENSE.txt
--rw-r--r--   0        0        0     1052 2024-01-28 00:27:21.997395 mojo_collections-1.3.6/README.rst
--rw-r--r--   0        0        0      663 2024-04-05 04:29:40.805235 mojo_collections-1.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:55:06.311771 mojo_collections-1.3.6/source/packages/mojo/collections/__init__.py
--rw-r--r--   0        0        0     5971 2024-01-26 02:55:06.311863 mojo_collections-1.3.6/source/packages/mojo/collections/caseinsensitivebytesdict.py
--rw-r--r--   0        0        0     5980 2024-01-26 02:55:06.311946 mojo_collections-1.3.6/source/packages/mojo/collections/caseinsensitivestringdict.py
--rw-r--r--   0        0        0    15470 2024-02-11 20:20:46.484714 mojo_collections-1.3.6/source/packages/mojo/collections/context.py
--rw-r--r--   0        0        0     5166 2024-03-11 17:15:42.649773 mojo_collections-1.3.6/source/packages/mojo/collections/contextpaths.py
--rw-r--r--   0        0        0      565 2024-01-26 02:55:06.312220 mojo_collections-1.3.6/source/packages/mojo/collections/contextuser.py
--rw-r--r--   0        0        0     1128 2024-01-26 02:55:06.312296 mojo_collections-1.3.6/source/packages/mojo/collections/helpers.py
--rw-r--r--   0        0        0     5913 2024-04-05 04:29:52.145043 mojo_collections-1.3.6/source/packages/mojo/collections/mergemap.py
--rw-r--r--   0        0        0     1057 2024-01-26 02:55:06.312475 mojo_collections-1.3.6/source/packages/mojo/collections/wellknown.py
--rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 mojo_collections-1.3.6/setup.py
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 mojo_collections-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:55:06.310687 mojo_collections-1.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     1052 2024-01-28 00:27:21.997395 mojo_collections-1.3.7/README.rst
+-rw-r--r--   0        0        0      663 2024-04-24 03:50:30.607669 mojo_collections-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:55:06.311771 mojo_collections-1.3.7/source/packages/mojo/collections/__init__.py
+-rw-r--r--   0        0        0     5971 2024-01-26 02:55:06.311863 mojo_collections-1.3.7/source/packages/mojo/collections/caseinsensitivebytesdict.py
+-rw-r--r--   0        0        0     5980 2024-01-26 02:55:06.311946 mojo_collections-1.3.7/source/packages/mojo/collections/caseinsensitivestringdict.py
+-rw-r--r--   0        0        0    15470 2024-02-11 20:20:46.484714 mojo_collections-1.3.7/source/packages/mojo/collections/context.py
+-rw-r--r--   0        0        0     5166 2024-03-11 17:15:42.649773 mojo_collections-1.3.7/source/packages/mojo/collections/contextpaths.py
+-rw-r--r--   0        0        0      565 2024-01-26 02:55:06.312220 mojo_collections-1.3.7/source/packages/mojo/collections/contextuser.py
+-rw-r--r--   0        0        0     1128 2024-01-26 02:55:06.312296 mojo_collections-1.3.7/source/packages/mojo/collections/helpers.py
+-rw-r--r--   0        0        0     5913 2024-04-05 04:29:52.145043 mojo_collections-1.3.7/source/packages/mojo/collections/mergemap.py
+-rw-r--r--   0        0        0     1057 2024-01-26 02:55:06.312475 mojo_collections-1.3.7/source/packages/mojo/collections/wellknown.py
+-rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 mojo_collections-1.3.7/setup.py
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 mojo_collections-1.3.7/PKG-INFO
```

### Comparing `mojo_collections-1.3.6/LICENSE.txt` & `mojo_collections-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/README.rst` & `mojo_collections-1.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/pyproject.toml` & `mojo_collections-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-collections"
 description = "Mojo Collections Package"
-version = "1.3.6"
+version = "1.3.7"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_collections-1.3.6/source/packages/mojo/collections/caseinsensitivebytesdict.py` & `mojo_collections-1.3.7/source/packages/mojo/collections/caseinsensitivebytesdict.py`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/source/packages/mojo/collections/caseinsensitivestringdict.py` & `mojo_collections-1.3.7/source/packages/mojo/collections/caseinsensitivestringdict.py`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/source/packages/mojo/collections/context.py` & `mojo_collections-1.3.7/source/packages/mojo/collections/context.py`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/source/packages/mojo/collections/contextpaths.py` & `mojo_collections-1.3.7/source/packages/mojo/collections/contextpaths.py`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/source/packages/mojo/collections/contextuser.py` & `mojo_collections-1.3.7/source/packages/mojo/collections/contextuser.py`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/source/packages/mojo/collections/helpers.py` & `mojo_collections-1.3.7/source/packages/mojo/collections/helpers.py`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/source/packages/mojo/collections/mergemap.py` & `mojo_collections-1.3.7/source/packages/mojo/collections/mergemap.py`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/source/packages/mojo/collections/wellknown.py` & `mojo_collections-1.3.7/source/packages/mojo/collections/wellknown.py`

 * *Files identical despite different names*

### Comparing `mojo_collections-1.3.6/setup.py` & `mojo_collections-1.3.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['mojo', 'mojo.collections']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-collections',
-    'version': '1.3.6',
+    'version': '1.3.7',
     'description': 'Mojo Collections Package',
     'long_description': "===================================\nAutomation Mojo Collections Package\n===================================\nA package that contains specialized collections used for automation and configuration.\n\n===========================\nFeatures of this Repository\n===========================\n* Machine Setup\n* Virtual Environment Setup (Poetry)\n* PyPi Publishing\n* Sphinx Documentation\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here 'source/packages/(root-module-folder)'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_collections-1.3.6/PKG-INFO` & `mojo_collections-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-collections
-Version: 1.3.6
+Version: 1.3.7
 Summary: Mojo Collections Package
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

