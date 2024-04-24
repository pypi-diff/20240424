# Comparing `tmp/wrapper_bar-0.1.3.tar.gz` & `tmp/wrapper_bar-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapper_bar-0.1.3.tar", last modified: Tue Apr 23 07:01:56 2024, max compression
+gzip compressed data, was "wrapper_bar-0.1.4.tar", last modified: Wed Apr 24 17:04:53 2024, max compression
```

## Comparing `wrapper_bar-0.1.3.tar` & `wrapper_bar-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 07:01:56.038994 wrapper_bar-0.1.3/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-22 04:51:36.000000 wrapper_bar-0.1.3/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     5651 2024-04-23 07:01:56.038622 wrapper_bar-0.1.3/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3322 2024-04-23 06:59:51.000000 wrapper_bar-0.1.3/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1210 2024-04-23 05:08:35.000000 wrapper_bar-0.1.3/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-23 07:01:56.039054 wrapper_bar-0.1.3/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 07:01:56.031846 wrapper_bar-0.1.3/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 07:01:56.035028 wrapper_bar-0.1.3/src/wrapper_bar/
--rw-r--r--   0 d33pster   (501) staff       (20)       54 2024-04-23 05:51:01.000000 wrapper_bar-0.1.3/src/wrapper_bar/Exceptions.py
--rw-r--r--   0 d33pster   (501) staff       (20)       24 2024-04-22 20:39:35.000000 wrapper_bar-0.1.3/src/wrapper_bar/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9002 2024-04-23 06:20:49.000000 wrapper_bar-0.1.3/src/wrapper_bar/wrapper.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 07:01:56.038224 wrapper_bar-0.1.3/src/wrapper_bar.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     5651 2024-04-23 07:01:56.000000 wrapper_bar-0.1.3/src/wrapper_bar.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      311 2024-04-23 07:01:56.000000 wrapper_bar-0.1.3/src/wrapper_bar.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-23 07:01:56.000000 wrapper_bar-0.1.3/src/wrapper_bar.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       21 2024-04-23 07:01:56.000000 wrapper_bar-0.1.3/src/wrapper_bar.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       12 2024-04-23 07:01:56.000000 wrapper_bar-0.1.3/src/wrapper_bar.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-24 17:04:53.303448 wrapper_bar-0.1.4/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-22 04:51:36.000000 wrapper_bar-0.1.4/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     5816 2024-04-24 17:04:53.302806 wrapper_bar-0.1.4/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     3487 2024-04-24 16:45:12.000000 wrapper_bar-0.1.4/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1210 2024-04-24 16:40:37.000000 wrapper_bar-0.1.4/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-24 17:04:53.303539 wrapper_bar-0.1.4/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-24 17:04:53.280540 wrapper_bar-0.1.4/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-24 17:04:53.286208 wrapper_bar-0.1.4/src/wrapper_bar/
+-rw-r--r--   0 d33pster   (501) staff       (20)       54 2024-04-23 05:51:01.000000 wrapper_bar-0.1.4/src/wrapper_bar/Exceptions.py
+-rw-r--r--   0 d33pster   (501) staff       (20)       24 2024-04-22 20:39:35.000000 wrapper_bar-0.1.4/src/wrapper_bar/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    13020 2024-04-24 17:04:08.000000 wrapper_bar-0.1.4/src/wrapper_bar/wrapper.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-24 17:04:53.302081 wrapper_bar-0.1.4/src/wrapper_bar.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     5816 2024-04-24 17:04:53.000000 wrapper_bar-0.1.4/src/wrapper_bar.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      311 2024-04-24 17:04:53.000000 wrapper_bar-0.1.4/src/wrapper_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-24 17:04:53.000000 wrapper_bar-0.1.4/src/wrapper_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       21 2024-04-24 17:04:53.000000 wrapper_bar-0.1.4/src/wrapper_bar.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       12 2024-04-24 17:04:53.000000 wrapper_bar-0.1.4/src/wrapper_bar.egg-info/top_level.txt
```

### Comparing `wrapper_bar-0.1.3/LICENSE` & `wrapper_bar-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wrapper_bar-0.1.3/PKG-INFO` & `wrapper_bar-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapper-bar
-Version: 0.1.3
+Version: 0.1.4
 Summary: Progress Bar with command wrapping
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -49,30 +49,32 @@
 
 `Wrapper-Bar` is a python module to help wrap commands with the progress bar. `Wrapper-Bar` helps in wrapping shell commands, or even python scripts with a progress bar and ETA.
 
 ## Badges
 
 ![PyPI - Version](https://img.shields.io/pypi/v/wrapper-bar)
 ![PyPI - Status](https://img.shields.io/pypi/status/wrapper-bar)
+![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/wrapper-bar)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wrapper-bar)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/wrapper-bar)
 ![PyPI - License](https://img.shields.io/pypi/l/wrapper-bar)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Uninstall](#uninstall)
+- [Yanked Versions](#yanked-versions)
 
 ## Installation
 
 To install `wrapper-bar`, use pip.
 
 ```bash
-pip install wrapper-bar==0.1.3
+pip install wrapper-bar==0.1.4
 ```
 
 ## Usage
 
 - Import the Wrapper class.
 
   ```python
@@ -140,15 +142,15 @@
       
       # try to keep one statement only inside """...""", 
       # but if need be, then you can also put multiple 
       # statements followed by '\n'. Like """c=10\nd=20\n"""
 
       # and now we will execute them with the loading bar as the 
       # front.
-      
+
       >>> from wrapper_bar.wrapper import Wrapper
       >>> w = Wrapper("Loading:")
       >>> w.pyShellWrapper(pythoncodes, dependencies) # this will output the following:
       Loading: |▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓|Time: 0:00:10
       
       # To fetch the outputs, we will use a property 'pyShellWrapperResults' 
       # defined under the `Wrapper Class`
@@ -160,7 +162,11 @@
 ## Uninstall
 
 To uninstall `wrapper-bar`, use pip.
 
 ```bash
 pip uninstall wrapper-bar
 ```
+
+## Yanked Versions
+
+- **_v0.1.2_**
```

### Comparing `wrapper_bar-0.1.3/README.md` & `wrapper_bar-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 
 `Wrapper-Bar` is a python module to help wrap commands with the progress bar. `Wrapper-Bar` helps in wrapping shell commands, or even python scripts with a progress bar and ETA.
 
 ## Badges
 
 ![PyPI - Version](https://img.shields.io/pypi/v/wrapper-bar)
 ![PyPI - Status](https://img.shields.io/pypi/status/wrapper-bar)
+![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/wrapper-bar)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wrapper-bar)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/wrapper-bar)
 ![PyPI - License](https://img.shields.io/pypi/l/wrapper-bar)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Uninstall](#uninstall)
+- [Yanked Versions](#yanked-versions)
 
 ## Installation
 
 To install `wrapper-bar`, use pip.
 
 ```bash
-pip install wrapper-bar==0.1.3
+pip install wrapper-bar==0.1.4
 ```
 
 ## Usage
 
 - Import the Wrapper class.
 
   ```python
@@ -93,15 +95,15 @@
       
       # try to keep one statement only inside """...""", 
       # but if need be, then you can also put multiple 
       # statements followed by '\n'. Like """c=10\nd=20\n"""
 
       # and now we will execute them with the loading bar as the 
       # front.
-      
+
       >>> from wrapper_bar.wrapper import Wrapper
       >>> w = Wrapper("Loading:")
       >>> w.pyShellWrapper(pythoncodes, dependencies) # this will output the following:
       Loading: |▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓|Time: 0:00:10
       
       # To fetch the outputs, we will use a property 'pyShellWrapperResults' 
       # defined under the `Wrapper Class`
@@ -113,7 +115,11 @@
 ## Uninstall
 
 To uninstall `wrapper-bar`, use pip.
 
 ```bash
 pip uninstall wrapper-bar
 ```
+
+## Yanked Versions
+
+- **_v0.1.2_**
```

### Comparing `wrapper_bar-0.1.3/pyproject.toml` & `wrapper_bar-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wrapper-bar"
-version = "0.1.3"
+version = "0.1.4"
 description = "Progress Bar with command wrapping"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `wrapper_bar-0.1.3/src/wrapper_bar.egg-info/PKG-INFO` & `wrapper_bar-0.1.4/src/wrapper_bar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapper-bar
-Version: 0.1.3
+Version: 0.1.4
 Summary: Progress Bar with command wrapping
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -49,30 +49,32 @@
 
 `Wrapper-Bar` is a python module to help wrap commands with the progress bar. `Wrapper-Bar` helps in wrapping shell commands, or even python scripts with a progress bar and ETA.
 
 ## Badges
 
 ![PyPI - Version](https://img.shields.io/pypi/v/wrapper-bar)
 ![PyPI - Status](https://img.shields.io/pypi/status/wrapper-bar)
+![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/wrapper-bar)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wrapper-bar)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/wrapper-bar)
 ![PyPI - License](https://img.shields.io/pypi/l/wrapper-bar)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Uninstall](#uninstall)
+- [Yanked Versions](#yanked-versions)
 
 ## Installation
 
 To install `wrapper-bar`, use pip.
 
 ```bash
-pip install wrapper-bar==0.1.3
+pip install wrapper-bar==0.1.4
 ```
 
 ## Usage
 
 - Import the Wrapper class.
 
   ```python
@@ -140,15 +142,15 @@
       
       # try to keep one statement only inside """...""", 
       # but if need be, then you can also put multiple 
       # statements followed by '\n'. Like """c=10\nd=20\n"""
 
       # and now we will execute them with the loading bar as the 
       # front.
-      
+
       >>> from wrapper_bar.wrapper import Wrapper
       >>> w = Wrapper("Loading:")
       >>> w.pyShellWrapper(pythoncodes, dependencies) # this will output the following:
       Loading: |▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓|Time: 0:00:10
       
       # To fetch the outputs, we will use a property 'pyShellWrapperResults' 
       # defined under the `Wrapper Class`
@@ -160,7 +162,11 @@
 ## Uninstall
 
 To uninstall `wrapper-bar`, use pip.
 
 ```bash
 pip uninstall wrapper-bar
 ```
+
+## Yanked Versions
+
+- **_v0.1.2_**
```

