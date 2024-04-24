# Comparing `tmp/pasta_man-1.1.2.tar.gz` & `tmp/pasta_man-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.1.2.tar", last modified: Wed Apr 24 14:53:25 2024, max compression
+gzip compressed data, was "pasta_man-1.1.3.tar", last modified: Wed Apr 24 17:28:22 2024, max compression
```

## Comparing `pasta_man-1.1.2.tar` & `pasta_man-1.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:25.215659 pasta_man-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 14:53:18.000000 pasta_man-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-24 14:53:25.215659 pasta_man-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-04-24 14:53:18.000000 pasta_man-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-24 14:53:18.000000 pasta_man-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-04-24 14:53:18.000000 pasta_man-1.1.2/readmeforpypi.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:53:25.215659 pasta_man-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:25.207659 pasta_man-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:25.211659 pasta_man-1.1.2/src/pasta_man/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:25.211659 pasta_man-1.1.2/src/pasta_man/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/architectures/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/architectures/targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/architectures/terminal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6109 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/pasta_man.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:25.211659 pasta_man-1.1.2/src/pasta_man/self_launch_thread/
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/self_launch_thread/Launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/self_launch_thread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:25.215659 pasta_man-1.1.2/src/pasta_man/utilities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:25.215659 pasta_man-1.1.2/src/pasta_man/utilities/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/Exceptions/TerminalExceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/Exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/helptext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/pasta_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/pasta_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-24 14:53:18.000000 pasta_man-1.1.2/src/pasta_man/utilities/retransform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:53:25.215659 pasta_man-1.1.2/src/pasta_man.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-24 14:53:25.000000 pasta_man-1.1.2/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 14:53:25.000000 pasta_man-1.1.2/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:53:25.000000 pasta_man-1.1.2/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 14:53:25.000000 pasta_man-1.1.2/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 14:53:25.000000 pasta_man-1.1.2/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 14:53:25.000000 pasta_man-1.1.2/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 17:28:15.000000 pasta_man-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-24 17:28:22.109753 pasta_man-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-04-24 17:28:15.000000 pasta_man-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-24 17:28:15.000000 pasta_man-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-04-24 17:28:15.000000 pasta_man-1.1.3/readmeforpypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:28:22.109753 pasta_man-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.105753 pasta_man-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.105753 pasta_man-1.1.3/src/pasta_man/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/architectures/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/architectures/targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/architectures/terminal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6109 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/pasta_man.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man/self_launch_thread/
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/self_launch_thread/Launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/self_launch_thread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man/utilities/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/TerminalExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/helptext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/pasta_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/pasta_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-24 17:28:15.000000 pasta_man-1.1.3/src/pasta_man/utilities/retransform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:28:22.109753 pasta_man-1.1.3/src/pasta_man.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 17:28:22.000000 pasta_man-1.1.3/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.1.2/LICENSE` & `pasta_man-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/PKG-INFO` & `pasta_man-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.1.2
+Version: 1.1.3
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -46,15 +46,15 @@
 Requires-Dist: pandas
 Requires-Dist: colorama
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 Requires-Dist: ttkthemes
 Requires-Dist: pyinstaller
-Requires-Dist: wrapper-bar>=0.1.3
+Requires-Dist: wrapper-bar>=0.1.4
 
 # Overview
 
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access.
 
 ## Project Badges
 
@@ -224,26 +224,26 @@
 ## Dependencies
 
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
 - colorama
-- wrapper-bar>=0.1.3
+- wrapper-bar>=0.1.4
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.2
+pip install pasta-man==1.1.3
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
@@ -271,15 +271,15 @@
     ...
     ```
 
 - To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
 
     ```bash
     $ pasta-man -h # or pasta-man --help
-    Pasta Man v1.1.1
+    Pasta Man v1.1.3
     helptext
       |  -h or --help                     : show this help and exit.
       |  -v or --version                  : show version and exit.
       |  -p or --path                     : show install path and exit.
       |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
       |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
       |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
```

### Comparing `pasta_man-1.1.2/README.md` & `pasta_man-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -170,26 +170,26 @@
 ## Dependencies
 
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
 - colorama
-- wrapper-bar>=0.1.3
+- wrapper-bar>=0.1.4
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.2
+pip install pasta-man==1.1.3
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
@@ -217,15 +217,15 @@
     ...
     ```
 
 - To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
 
     ```bash
     $ pasta-man -h # or pasta-man --help
-    Pasta Man v1.1.1
+    Pasta Man v1.1.3
     helptext
       |  -h or --help                     : show this help and exit.
       |  -v or --version                  : show version and exit.
       |  -p or --path                     : show install path and exit.
       |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
       |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
       |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
```

### Comparing `pasta_man-1.1.2/pyproject.toml` & `pasta_man-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.1.2"
+version = "1.1.3"
 description = "Password Manager"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Topic :: Security",
     "Programming Language :: Python :: 3.10",
@@ -25,15 +25,15 @@
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"},
     {name = "Sairam Pimple", email = "sairampimple003@gmail.com"},
     {name = "Shubham Narendra Singh", email = "shubh1122000@gmail.com"}
 ]
 maintainers = [
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"}
 ]
-dependencies = ['cryptography', 'pandas', 'colorama', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes', 'pyinstaller', 'wrapper-bar>=0.1.3']
+dependencies = ['cryptography', 'pandas', 'colorama', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes', 'pyinstaller', 'wrapper-bar>=0.1.4']
 
 [project.scripts]
 pasta-man-launcher = "pasta_man.pasta_man:main"
 pasta-man = "pasta_man.self_launch_thread.Launcher:main"
 
 [project.urls]
 GitHub = 'https://github.com/d33pster/pasta-man'
```

### Comparing `pasta_man-1.1.2/readmeforpypi.md` & `pasta_man-1.1.3/readmeforpypi.md`

 * *Files 0% similar despite different names*

```diff
@@ -170,26 +170,26 @@
 ## Dependencies
 
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
 - colorama
-- wrapper-bar>=0.1.3
+- wrapper-bar>=0.1.4
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.2
+pip install pasta-man==1.1.3
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
@@ -217,15 +217,15 @@
     ...
     ```
 
 - To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
 
     ```bash
     $ pasta-man -h # or pasta-man --help
-    Pasta Man v1.1.1
+    Pasta Man v1.1.3
     helptext
       |  -h or --help                     : show this help and exit.
       |  -v or --version                  : show version and exit.
       |  -p or --path                     : show install path and exit.
       |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
       |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
       |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
```

### Comparing `pasta_man-1.1.2/src/pasta_man/architectures/gui.py` & `pasta_man-1.1.3/src/pasta_man/architectures/gui.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/src/pasta_man/architectures/targets.py` & `pasta_man-1.1.3/src/pasta_man/architectures/targets.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/src/pasta_man/architectures/terminal.py` & `pasta_man-1.1.3/src/pasta_man/architectures/terminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,16 @@
             
             dependencies = [
                 """from pasta_man.architectures.targets import targets""",
                 """import threading""",
                 """import pandas as pd"""
             ]
             
-            wrap = Wrapper("searching:")
-            wrap.pyShellWrapper(codes, dependencies, 0.001)
+            wrap = Wrapper()
+            wrap.pyShellWrapper(codes, dependencies, delay=0.001, label="searching:")
             results = wrap.pyShellWrapperResults['results']
             if not results.empty:
                 print(results.drop(['password', 'timestamp'], axis=1))
             else:
                 print(f"{f.RED}No Match Found{f.RESET}")
                 
             index = int(input(f"{f.BLUE}index>{f.RESET} "))
@@ -185,16 +185,15 @@
                 
                 dependencies = [
                     """import threading""",
                     """import pyperclip""",
                     """from pasta_man.architectures.targets import targets"""
                 ]
                 
-                wrap = Wrapper("decrypting:")
-                wrap.pyShellWrapper(codes, dependencies, 0.001)
+                wrap.pyShellWrapper(codes, dependencies, delay=0.001, label="decrypting:")
                 print(f"{f.GREEN}Password copied to clipboard.{f.RESET}")
             
             
         else:
             pass
     
     def decryptthread(self, masterpassword: str):
```

### Comparing `pasta_man-1.1.2/src/pasta_man/pasta_man.py` & `pasta_man-1.1.3/src/pasta_man/pasta_man.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 Working:
     - catch and analyse arguments if any. If Found, execute it. Else Move on.
     - Check for master password
     - If found, decrypt it and call pmanager class. If not found, ask the user for master password, encrypt and save it and then call pmanager class.
 """
 
 # version info
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 # import internal modules
 from pathlib import Path
 from os.path import join as jPath, exists as there, dirname, abspath
 from os import makedirs
 from shutil import rmtree
 import sys, threading
```

### Comparing `pasta_man-1.1.2/src/pasta_man/self_launch_thread/Launcher.py` & `pasta_man-1.1.3/src/pasta_man/self_launch_thread/Launcher.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,15 +41,17 @@
     - if windows, run first time setup, where an exe and vbs files are created. From next time, run exe.
 """
 
 from platform import system as os
 from os import system as run, makedirs, chdir
 from os.path import exists as there, join as jPath, dirname, abspath, basename
 from pathlib import Path
-import sys, subprocess
+from wrapper_bar.wrapper import Wrapper
+import sys
+from colorama import init as color, Fore as f
 
 def checklogfile():
     """## check for .log file, if not present, create it
     """
     if not there(jPath(str(Path.home()), '.pastaman')):
         makedirs(jPath(str(Path.home()), '.pastaman'))
     
@@ -73,29 +75,68 @@
 copy dist\pasta_man.exe %USERPROFILE%\.pastaman\pasta-man.exe
 
 @REM delete dist
 del dist /s /q
 
 @REM create vbs script
 cd %USERPROFILE%\.pastaman
-echo Set pastaShell = WScript.CreateObject("WScript.Shell") > pasta-man.vbs
+echo Set pastaShell = WScript.CreateObject('WScript.Shell') > pasta-man.vbs
 echo pastaShell.Run "%USERPROFILE%\.pastaman\pasta-man.exe", 0, False >> pasta-man.vbs
 
 @REM copy it 
 """
     directory = dirname(dirname(abspath(__file__))) # pasta_man directory
     chdir(directory)
-    print('(one-time)')
+    print(f'{f.RED}(one-time-setup){f.RESET}')
     print('Operating System: Windows\nsetting up pasta-man...\nThis might take a while.')
-    with open(jPath(directory, 'win-setup.bat'), 'w') as batfile:
-        batfile.write(batdat)
-    subprocess.Popen([f"{jPath(directory, 'win-setup.bat')}"], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()
-    print('complete.')
-
+    
+    wrap = Wrapper()
+    
+    codes = [
+        f"""subprocess.Popen(['pyinstaller', '--onefile', '--noconsole', 'pasta_man.py'], stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL).wait()""",
+    ]
+    
+    dependencies = [
+        """import subprocess"""
+    ]
+    
+    wrap.pyShellWrapper(codes, dependencies, delay=0.2, width=70, label="Making pasta:", timer="ElapsedTime")
+    
+    codes = [
+        """shutil.rmtree(join(pwd(), 'build'))""",
+        """remove(join(pwd(), 'pasta_man.spec'))""",
+        """shutil.copyfile(join(pwd(), 'dist', 'pasta_man.exe'), join(str(Path.home()), '.pastaman', 'pasta-man.exe'))"""
+    ]
+    
+    dependencies = [
+        """import shutil""",
+        """from os.path import join""",
+        """from os import getcwd as pwd, remove""",
+        """from pathlib import Path"""
+    ]
+    
+    wrap.pyShellWrapper(codes, dependencies, delay=0.03, width=62, label="Cleaning up:")
+    
+    codes = ["""
+path = join(str(Path.home()), '.pastaman')
+with open(join(path, 'pasta-man.vbs'), 'w') as vbs:
+    vbs.write("Set pastashell = WScript.CreateObject(\\"WScript.Shell\\")\\n")
+    vbs.write("pastashell.Run \\"%USERPROFILE%\\\\.pastaman\\\\pasta-man.exe\\", 0, False")
+"""]
+    
+    dependencies = [
+        """from pathlib import Path""",
+        """from os.path import join"""
+    ]
+    
+    wrap.pyShellWrapper(codes, dependencies, delay=0.01, width=60, label="Garnishing:")
+    
+    print(f"{f.LIGHTGREEN_EX}Serving...{f.RESET}")
 def main():
+    color()
     checklogfile()
     # check for arguments
     if len(sys.argv[1:])>0:
         sys.argv[0] += sys.argv[0]+'-launcher'
         command = basename(sys.argv[0])
         for i in range(1, len(sys.argv)):
             command += " " + sys.argv[i]
```

### Comparing `pasta_man-1.1.2/src/pasta_man/utilities/Exceptions/exceptions.py` & `pasta_man-1.1.3/src/pasta_man/utilities/Exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/src/pasta_man/utilities/encryption.py` & `pasta_man-1.1.3/src/pasta_man/utilities/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/src/pasta_man/utilities/helptext.py` & `pasta_man-1.1.3/src/pasta_man/utilities/helptext.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/src/pasta_man/utilities/pasta_docs.py` & `pasta_man-1.1.3/src/pasta_man/utilities/pasta_docs.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/src/pasta_man/utilities/pasta_menu.py` & `pasta_man-1.1.3/src/pasta_man/utilities/pasta_menu.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/src/pasta_man/utilities/retransform.py` & `pasta_man-1.1.3/src/pasta_man/utilities/retransform.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.2/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.1.3/src/pasta_man.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.1.2
+Version: 1.1.3
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -46,15 +46,15 @@
 Requires-Dist: pandas
 Requires-Dist: colorama
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 Requires-Dist: ttkthemes
 Requires-Dist: pyinstaller
-Requires-Dist: wrapper-bar>=0.1.3
+Requires-Dist: wrapper-bar>=0.1.4
 
 # Overview
 
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access.
 
 ## Project Badges
 
@@ -224,26 +224,26 @@
 ## Dependencies
 
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
 - colorama
-- wrapper-bar>=0.1.3
+- wrapper-bar>=0.1.4
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.2
+pip install pasta-man==1.1.3
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
@@ -271,15 +271,15 @@
     ...
     ```
 
 - To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
 
     ```bash
     $ pasta-man -h # or pasta-man --help
-    Pasta Man v1.1.1
+    Pasta Man v1.1.3
     helptext
       |  -h or --help                     : show this help and exit.
       |  -v or --version                  : show version and exit.
       |  -p or --path                     : show install path and exit.
       |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
       |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
       |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
```

### Comparing `pasta_man-1.1.2/src/pasta_man.egg-info/SOURCES.txt` & `pasta_man-1.1.3/src/pasta_man.egg-info/SOURCES.txt`

 * *Files identical despite different names*

