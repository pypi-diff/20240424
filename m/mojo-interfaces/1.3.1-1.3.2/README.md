# Comparing `tmp/mojo_interfaces-1.3.1.tar.gz` & `tmp/mojo_interfaces-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_interfaces-1.3.1.tar", max compression
+gzip compressed data, was "mojo_interfaces-1.3.2.tar", max compression
```

## Comparing `mojo_interfaces-1.3.1.tar` & `mojo_interfaces-1.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:53:59.487475 mojo_interfaces-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0      850 2024-01-26 02:53:59.487659 mojo_interfaces-1.3.1/README.rst
--rw-r--r--   0        0        0      688 2024-02-21 07:25:08.357407 mojo_interfaces-1.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:53:59.488973 mojo_interfaces-1.3.1/source/packages/mojo/interfaces/__init__.py
--rw-r--r--   0        0        0     1551 2024-01-26 02:53:59.489064 mojo_interfaces-1.3.1/source/packages/mojo/interfaces/iexcludefilter.py
--rw-r--r--   0        0        0     1544 2024-01-26 02:53:59.489143 mojo_interfaces-1.3.1/source/packages/mojo/interfaces/iincludefilter.py
--rw-r--r--   0        0        0      762 2024-02-21 07:24:58.082138 mojo_interfaces-1.3.1/source/packages/mojo/interfaces/iserializable.py
--rw-r--r--   0        0        0     6271 2024-01-26 02:53:59.489239 mojo_interfaces-1.3.1/source/packages/mojo/interfaces/isystemcontext.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.1/setup.py
--rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:53:59.487475 mojo_interfaces-1.3.2/LICENSE.txt
+-rw-r--r--   0        0        0      850 2024-01-26 02:53:59.487659 mojo_interfaces-1.3.2/README.rst
+-rw-r--r--   0        0        0      688 2024-04-24 04:02:16.107538 mojo_interfaces-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:59.488973 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/__init__.py
+-rw-r--r--   0        0        0     1551 2024-01-26 02:53:59.489064 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iexcludefilter.py
+-rw-r--r--   0        0        0     1544 2024-01-26 02:53:59.489143 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iincludefilter.py
+-rw-r--r--   0        0        0      762 2024-02-21 07:24:58.082138 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iserializable.py
+-rw-r--r--   0        0        0     6271 2024-01-26 02:53:59.489239 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/isystemcontext.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.2/setup.py
+-rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.2/PKG-INFO
```

### Comparing `mojo_interfaces-1.3.1/LICENSE.txt` & `mojo_interfaces-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.1/README.rst` & `mojo_interfaces-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.1/pyproject.toml` & `mojo_interfaces-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-interfaces"
 description = "Automation Mojo Interfaces Package"
-version = "1.3.1"
+version = "1.3.2"
 authors = ["Myron W Walker"]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_interfaces-1.3.1/source/packages/mojo/interfaces/iexcludefilter.py` & `mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iexcludefilter.py`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.1/source/packages/mojo/interfaces/iincludefilter.py` & `mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iincludefilter.py`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.1/source/packages/mojo/interfaces/iserializable.py` & `mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iserializable.py`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.1/source/packages/mojo/interfaces/isystemcontext.py` & `mojo_interfaces-1.3.2/source/packages/mojo/interfaces/isystemcontext.py`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.1/setup.py` & `mojo_interfaces-1.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['mojo', 'mojo.interfaces']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-interfaces',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': 'Automation Mojo Interfaces Package',
     'long_description': "=======================\nmojo-interfaces\n=======================\nThis is a package that contains a collection or library of interfaces that can be shared by other packages.\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here 'source/packages/(root-module-folder)'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n",
     'author': 'Myron W Walker',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_interfaces-1.3.1/PKG-INFO` & `mojo_interfaces-1.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-interfaces
-Version: 1.3.1
+Version: 1.3.2
 Summary: Automation Mojo Interfaces Package
 License: LICENSE.txt
 Keywords: python
 Author: Myron W Walker
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
```

