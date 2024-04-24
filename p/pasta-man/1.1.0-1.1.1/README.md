# Comparing `tmp/pasta_man-1.1.0.tar.gz` & `tmp/pasta_man-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.1.0.tar", last modified: Sun Apr 21 09:11:02 2024, max compression
+gzip compressed data, was "pasta_man-1.1.1.tar", last modified: Tue Apr 23 18:38:00 2024, max compression
```

## Comparing `pasta_man-1.1.0.tar` & `pasta_man-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:11:02.934868 pasta_man-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-21 09:10:50.000000 pasta_man-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-21 09:11:02.930868 pasta_man-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-21 09:10:50.000000 pasta_man-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-21 09:10:50.000000 pasta_man-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:11:02.934868 pasta_man-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:11:02.926868 pasta_man-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:11:02.926868 pasta_man-1.1.0/src/pasta_man/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:11:02.930868 pasta_man-1.1.0/src/pasta_man/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/architectures/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/architectures/targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/architectures/terminal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5791 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/pasta_man.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:11:02.930868 pasta_man-1.1.0/src/pasta_man/self_launch_thread/
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/self_launch_thread/Launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/self_launch_thread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:11:02.930868 pasta_man-1.1.0/src/pasta_man/utilities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:11:02.930868 pasta_man-1.1.0/src/pasta_man/utilities/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/Exceptions/TerminalExceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/Exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/helptext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/pasta_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/pasta_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-21 09:10:50.000000 pasta_man-1.1.0/src/pasta_man/utilities/retransform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:11:02.930868 pasta_man-1.1.0/src/pasta_man.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2024-04-21 09:11:02.000000 pasta_man-1.1.0/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-21 09:11:02.000000 pasta_man-1.1.0/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:11:02.000000 pasta_man-1.1.0/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-21 09:11:02.000000 pasta_man-1.1.0/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-21 09:11:02.000000 pasta_man-1.1.0/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 09:11:02.000000 pasta_man-1.1.0/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 18:38:00.612521 pasta_man-1.1.1/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-19 00:32:31.000000 pasta_man-1.1.1/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)    12425 2024-04-23 18:38:00.612076 pasta_man-1.1.1/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     9809 2024-04-23 18:28:17.000000 pasta_man-1.1.1/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1592 2024-04-23 18:28:17.000000 pasta_man-1.1.1/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-23 18:38:00.612572 pasta_man-1.1.1/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 18:38:00.594959 pasta_man-1.1.1/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 18:38:00.597887 pasta_man-1.1.1/src/pasta_man/
+-rw-r--r--   0 d33pster   (501) staff       (20)      106 2024-04-20 22:36:51.000000 pasta_man-1.1.1/src/pasta_man/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      183 2024-04-23 18:28:17.000000 pasta_man-1.1.1/src/pasta_man/__main__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 18:38:00.604703 pasta_man-1.1.1/src/pasta_man/architectures/
+-rw-r--r--   0 d33pster   (501) staff       (20)        7 2024-04-23 18:28:17.000000 pasta_man-1.1.1/src/pasta_man/architectures/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    11652 2024-04-23 18:28:17.000000 pasta_man-1.1.1/src/pasta_man/architectures/gui.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    12341 2024-04-23 18:28:17.000000 pasta_man-1.1.1/src/pasta_man/architectures/targets.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9346 2024-04-23 18:28:17.000000 pasta_man-1.1.1/src/pasta_man/architectures/terminal.py
+-rwxr-xr-x   0 d33pster   (501) staff       (20)     6109 2024-04-23 18:28:17.000000 pasta_man-1.1.1/src/pasta_man/pasta_man.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 18:38:00.605917 pasta_man-1.1.1/src/pasta_man/self_launch_thread/
+-rw-r--r--   0 d33pster   (501) staff       (20)     3917 2024-04-20 09:33:27.000000 pasta_man-1.1.1/src/pasta_man/self_launch_thread/Launcher.py
+-rw-r--r--   0 d33pster   (501) staff       (20)       96 2024-04-19 00:32:31.000000 pasta_man-1.1.1/src/pasta_man/self_launch_thread/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 18:38:00.609494 pasta_man-1.1.1/src/pasta_man/utilities/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 18:38:00.611058 pasta_man-1.1.1/src/pasta_man/utilities/Exceptions/
+-rw-r--r--   0 d33pster   (501) staff       (20)      181 2024-04-21 09:14:54.000000 pasta_man-1.1.1/src/pasta_man/utilities/Exceptions/TerminalExceptions.py
+-rw-r--r--   0 d33pster   (501) staff       (20)        7 2024-04-23 18:28:17.000000 pasta_man-1.1.1/src/pasta_man/utilities/Exceptions/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     2088 2024-04-21 09:14:54.000000 pasta_man-1.1.1/src/pasta_man/utilities/Exceptions/exceptions.py
+-rw-r--r--   0 d33pster   (501) staff       (20)       51 2024-04-19 00:32:31.000000 pasta_man-1.1.1/src/pasta_man/utilities/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     4073 2024-04-21 09:14:54.000000 pasta_man-1.1.1/src/pasta_man/utilities/encryption.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     2780 2024-04-23 18:28:17.000000 pasta_man-1.1.1/src/pasta_man/utilities/helptext.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     6713 2024-04-21 09:14:54.000000 pasta_man-1.1.1/src/pasta_man/utilities/pasta_docs.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     7579 2024-04-19 00:32:31.000000 pasta_man-1.1.1/src/pasta_man/utilities/pasta_menu.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     2887 2024-04-20 09:33:27.000000 pasta_man-1.1.1/src/pasta_man/utilities/retransform.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-23 18:38:00.611663 pasta_man-1.1.1/src/pasta_man.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)    12425 2024-04-23 18:38:00.000000 pasta_man-1.1.1/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      957 2024-04-23 18:38:00.000000 pasta_man-1.1.1/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-23 18:38:00.000000 pasta_man-1.1.1/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)      119 2024-04-23 18:38:00.000000 pasta_man-1.1.1/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       99 2024-04-23 18:38:00.000000 pasta_man-1.1.1/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-23 18:38:00.000000 pasta_man-1.1.1/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.1.0/LICENSE` & `pasta_man-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.0/PKG-INFO` & `pasta_man-1.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,131 +1,146 @@
-Metadata-Version: 2.1
-Name: pasta-man
-Version: 1.1.0
-Summary: Password Manager
-Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
-Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2024 Soumyo Deep Gupta
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/d33pster/pasta-man
-Project-URL: Issues, https://github.com/d33pster/pasta-man/issues
-Project-URL: Documentation, https://d33pster.github.io/pasta-man/
-Keywords: d33pster,pasta-man,passman,pastaman,password-manager,password manager,password,manager
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Software Development
-Classifier: Topic :: Security
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: End Users/Desktop
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cryptography
-Requires-Dist: pandas
-Requires-Dist: termcolor
-Requires-Dist: tk
-Requires-Dist: optioner>=1.5.2
-Requires-Dist: pyperclip
-Requires-Dist: ttkthemes
-Requires-Dist: pyinstaller
+# Overview
+
+Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access.
+
+## Project Badges
 
 [![Continuous Deployment](https://github.com/d33pster/pasta-man/actions/workflows/ContinuousDeployment.yml/badge.svg)](https://github.com/d33pster/pasta-man/actions/workflows/ContinuousDeployment.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
 ![PyPI - Status](https://img.shields.io/pypi/status/pasta-man)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
 ![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
 
+## Changelog
 
-# Overview
-Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access. 
+See Changelog [here](CHANGELOG.md).
+
+## Table of Contents
+
+- [Motivation](#motivation)
+- [Features](#features)
+  - [Secure Management of Passwords](#secure-management-of-passwords)
+  - [Tags](#tags)
+  - [Search](#search)
+  - [Copy to Clipboard](#copy-to-clipboard)
+  - [Faster than basic tkinter apps](#faster-than-basic-tkinter-apps)
+  - [Import-Export Passwords](#import-export-passwords)
+  - [Code Description](#code-description)
+  - [Themes](#themes)
+    - [Currently Supported Themes](#currently-supported-themes)
+- [Dependencies](#dependencies)
+- [Installation](#installation)
+- [README before #Usage](#readme-before-usage)
+- [Usage](#usage)
+- [Troubleshooting](#troubleshooting)
+- [Uninstall](#uninstall)
+- [Yanked Versions](#yanked-versions)
 
 ## Motivation
- - In the digital login password age we need a one stop vault for storing all our login credentials with concerned of atmost  security.
- - The repeated use of single password in multiple accounts may lead to data breach or loss of data.
- - Weak passwords are easy to interpreat for attackers, use of strong passwords is recommended,but it is difficult to remember complex passwords.
- - Mostly passwords written in somewhere lead to comprosing of data and privacy of user.
+
+- In the digital login password age we need a one stop vault for storing all our login credentials with concerned of atmost  security.
+- The repeated use of single password in multiple accounts may lead to data breach or loss of data.
+- Weak passwords are easy to interpreat for attackers, use of strong passwords is recommended,but it is difficult to remember complex passwords.
+- Mostly passwords written in somewhere lead to comprosing of data and privacy of user.
 
 ## Features
  <!-- - Securely Managing Passwords
  - Copy passwords to the clipboard
  - One master password for all
  - Exporting all passwords in desired file format
  - Encrypting passwords
  - Search Password by target name/username -->
 
 ### Secure Management of Passwords
+
 `Pasta-Man` uses tripple layer encryption for saving passwords. Once `Pasta-Man` is provided with a password to manage, it encrypts it with a Master Password and stores it in a file, which then again is encrypted with the master password. The so called Master password is stored as an encrypted string (this encryption is done using password and salt not known to users.).
 
 The user will be prompted to provide a master password if it is the first use. If not, `Pasta-Man` will work as usual.
 
 ### Tags
+
 `Pasta-Man` stores passwords with tags such as target (the target application or link or any platform the password is meant for), target-type (target-type can be an app or link or any other category defined by the user. --- `Pasta-Man` supports creation of user defined tags and can easily fetch search results for the same.).
 
 ### Search
+
 User can search for passwords using keywords in keyword-types.
 
-`For Example:`<br>
+`For Example:`  
 If there is a target (say, abcde) which contains a keyword (say, abc), the user can search `abc` in `keyword-type == target`. Similarly, if there is a target-type (say, link) which contains a keyword (say, github), the user can search for `github` in `keyword-type == target-type`.
 
 ### Copy to Clipboard
+
 Upon [Search](#search), `Pasta-Man` allows to copy the password for the found match to user's clipboard (given, the user provides the master password), instead of revealing it because of bad management. `Pasta-Man` also allows to Remove that match search result.
 
 ### Faster than basic tkinter apps
+
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Import-Export Passwords
+
 `Pasta-Man` _v1.0.10_ onwards supports importing and exporting of passwords. **Note:** `Pasta-Man` can only import passwords that were exported by `Pasta-Man`. This Import/Export Feature is a solution to changing your PC or system.
 
 Be relieved that the exported passwords will be in encrypted format.
 
 - **Export Format:** `Pasta-Man` will append all the passwords encrypted by master password and all the data associated with it, to the encrypted master password into the output format chosen by user.
 
 - **Import Mechanism:** `Pasta-Man` will decrypt the master password associated with the passwords file and then decrypt all the data appended to it and then encrypt the data and passwords by using the current system master password, then append it to the currently existing passwords. And finally encrypt everything again.
 
 - **Usage:**
+
     ```bash
     pasta-man -e <output-file-format> # or pasta-man --export <output-file-format>
 
     pasta-man -i # or pasta-man --import
     ```
 
     Both of the commands above will trigger a file/directory selector dialog for selecting the desired directory or files.
 
+### Code Description
+
+To know more about the code structure and module information like -
+
+- Modules that are imported
+
+  - Internal (all the modules used that already come with your python interpreter)
+
+  - External (all the modules used that were installed using pip, these are also mentioned in pyproject.toml and requirements.txt)
+
+  - Project specifiv (all the modules used that were specifically created for this project.)
+
+- Hierarchy
+
+    The hierarchy of classes and functions.
+
+- Individial Object Descriptions
+
+    Descriptions about individual components of the code such as funtions and parameters.
+
+- Working
+
+    If there is any working rule or basic working of the module.
+
+All these can be seen by running the following commands:
+
+```console
+# pasta-man v1.0.9 and above supports docstring fetching, and can be done using:
+
+# in the terminal/CMD, run
+$ pasta-man -dwl # for docs with listing of hierarchy.
+```
 
 ### Themes
+
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
 Themes can be changed using the MenuBar -
 
-<img src="images/MenuBar.png">
+<!-- <img src="images/MenuBar.png"> -->
+![menubarimage](images/MenuBar.png)
 
 ###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
@@ -140,133 +155,109 @@
 - Kroc
 - Plastik
 - Radiance (Ubuntu)
 - Smog
 - Win XP
 - Yaru
 
-## Code Description
-
-To know more about the code structure and module information like - 
-
-- Modules that are imported
-    
-    - Internal (all the modules used that already come with your python interpreter)
-
-    - External (all the modules used that were installed using pip, these are also mentioned in pyproject.toml and requirements.txt)
-
-    - Project specifiv (all the modules used that were specifically created for this project.)
-
-- Hierarchy
-    
-    The hierarchy of classes and functions.
-
-- Individial Object Descriptions
-
-    Descriptions about individual components of the code such as funtions and parameters.
-
-- Working
-
-    If there is any working rule or basic working of the module.
-
-All these can be seen by running the following commands:
-
-```console
-# pasta-man v1.0.9 and above supports docstring fetching, and can be done using:
-
-# in the terminal/CMD, run
-$ pasta-man -dwl # for docs with listing of hierarchy.
-```
-
 ## Dependencies
+
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
-- termcolor
+- colorama
+- wrapper-bar>=0.1.3
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.0
+pip install pasta-man==1.1.1
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
 
-    - This command will launch `pasta-man` as a separate and independent process.
-    
-    - The terminal will be usable after `pasta-man` command is run.
-    
-    - The output logs will be stored in -> `HOME/.pastaman/.log` in Linux and MacOS.
+  - This command will launch `pasta-man` as a separate and independent process.
+
+  - The terminal will be usable after `pasta-man` command is run.
+
+  - The output logs will be stored in -> `HOME/.pastaman/.log` in Linux and MacOS.
 
 - `pasta-man-launcher` Command
-    
-    - This will launch `pasta-man` in the terminal.
 
-    - The terminal wont be available until this process is running.
+  - This will launch `pasta-man` in the terminal.
+
+  - The terminal wont be available until this process is running.
 
-    - All outputs will be logged in `stdin` (in the terminal screen)
+  - All outputs will be logged in `stdin` (in the terminal screen)
 
 ## Usage
 
-- To run `Pasta-Man`, run the following in the terminal/CMD.
+- To run `Pasta-Man`, run the following in the terminal/CMD. This will open up GUI.
 
     ```bash
-    pasta-man
+    $ pasta-man
+    ...
     ```
 
-- To show version information, run the following in terminal/CMD
+- To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
+
     ```bash
-    pasta-man -v # or pasta-man --version
+    $ pasta-man -h # or pasta-man --help
+    Pasta Man v1.1.1
+    helptext
+      |  -h or --help                     : show this help and exit.
+      |  -v or --version                  : show version and exit.
+      |  -p or --path                     : show install path and exit.
+      |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
+      |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
+      |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
+      |                                     Syntax: pasta-man --import
+      |  -e or --export                   : export passwords.
+      |                                     Syntax: pasta-man --export <export-format>
+      |                                     Available export formats -> ['csv', 'xlsx']
+      |  -s or --search                   : search a keyword in keyword-type.
+      |                                     Syntax: pasta-man --search <keyword-type> <keyword>
+      |                                     Available keyword types -> ['target', 'target-type', 'username']
     ```
 
 ## Troubleshooting
 
 - Windows
-    - Running `pasta-man` for the first time will trigger a setup mechanism. If the setup fails for any reason, run the following commands in the CMD.
+  - Running `pasta-man` for the first time will trigger a setup mechanism. If the setup fails for any reason, run the following commands in the CMD.
+
+    ```batch
+    pasta-man -rmc
+    ```
 
-        ```batch
-        pasta-man -rmc
-        ```
-        
-        or
-
-        
-        ```batch
-        pasta-man --remove-configurations
-        ```
-        And then run `pasta-man` again.
-    
-    - For Complete list of Developer Options of pasta-man, run the following commands.
-
-        ```batch
-        pasta-man -h
-        ```
-        
-        or
-
-        ```batch
-        pasta-man --help
-        ```
+    or
+
+    ```batch
+    pasta-man --remove-configurations
+    ```
+
+    And then run `pasta-man` again.  
+    NOTE: This command is irreversible and will also delete master password along with any saved passwords.
 
 ## Uninstall
 
 Uninstall using pip
 
 ```bash
 pip uninstall pasta-man
 ```
 
 ## Yanked Versions
+
 - _v1.0.5_
-    
+
     `Major Bug`: After Threads Update and Threads Patch 1, There was a major bug where the code breaks while initializing the app for the first time.
```

### Comparing `pasta_man-1.1.0/pyproject.toml` & `pasta_man-1.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.1.0"
+version = "1.1.1"
 description = "Password Manager"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Topic :: Security",
     "Programming Language :: Python :: 3.9",
@@ -26,15 +26,15 @@
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"},
     {name = "Sairam Pimple", email = "sairampimple003@gmail.com"},
     {name = "Shubham Narendra Singh", email = "shubh1122000@gmail.com"}
 ]
 maintainers = [
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"}
 ]
-dependencies = ['cryptography', 'pandas', 'termcolor', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes', 'pyinstaller']
+dependencies = ['cryptography', 'pandas', 'colorama', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes', 'pyinstaller', 'wrapper-bar>=0.1.3']
 
 [project.scripts]
 pasta-man-launcher = "pasta_man.pasta_man:main"
 pasta-man = "pasta_man.self_launch_thread.Launcher:main"
 
 [project.urls]
 GitHub = 'https://github.com/d33pster/pasta-man'
```

### Comparing `pasta_man-1.1.0/src/pasta_man/architectures/gui.py` & `pasta_man-1.1.1/src/pasta_man/architectures/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 
 # import libs
 from tkinter import *
 from tkinter import ttk, simpledialog, messagebox
 from os.path import join as jPath
 from pathlib import Path
 import pyperclip
-import threading
+import threading, platform
 
 class pmanager:
     def __init__(self, master:Tk, masterpassword: bytes):
         # create a master object
         self.parent = master
         # set title
         self.parent.title('Pasta-Man')
         # set geometry
-        self.parent.geometry('530x300+400+280')
+        if platform.system()!="Windows":
+            self.parent.geometry('530x300+400+280')
+        else:
+            self.parent.geometry('610x300+350+300')
         # set architecture
         self.arch = targets(masterpassword)
         
         # set menu
         menu = Menu(self.parent)
         self.parent.config(menu=menu)
         # -> add menus
@@ -124,16 +127,19 @@
         self.targtypelist = ttk.OptionMenu(self.FEF, self.varoption, *['target', 'target-type', 'username'])
         self.targtypelist.place(anchor='center', relx=0.75, rely=0.3, relwidth=0.35)
         
         # -> create a status label
         self.fetchstatusvar = StringVar()
         self.fetchstatus = ttk.Label(self.FEF, textvariable=self.fetchstatusvar)
         self.fetchstatus.place(anchor='center', relx=0.5, rely=0.79)
+        
+        # -> bind search entry
+        self.searchEntry.bind('<Return>', self.search)
     
-    def search(self):
+    def search(self, event=None):
         # -> fetch value and search:
         t1 = threading.Thread(target=self.arch.search, args=(self.varsearch.get(), self.varoption.get()))
         t1.start()
         t1.join()
         
         if self.arch.__searchresult__!=None:
             self.fetchstatusvar.set('Match Found!')
@@ -183,36 +189,34 @@
         # prepare alleged pass
         allegedpass = simpledialog.askstring("Master Password", "Enter Master Password to copy password to clipboard: ", show='-')
         
         # get masterpass
         with open(jPath(str(Path.home()), '.pastaman', '.m'), 'rb') as m:
             masterpassword = m.read() # this is encrypted
         
-        def decryptthread(masterpassword: str):
-            denc = Encryption("pastaman".encode('ascii'), masterpassword.encode('ascii'))
-            denc.unlock()
-            self.den = denc.__unencryptedstring__
-            sys.exit(0)
-        
-        
-        t1 = threading.Thread(target=decryptthread, args=(masterpassword.decode('ascii'),))
+        t1 = threading.Thread(target=self.decryptthread, args=(masterpassword.decode('ascii'),))
         t1.start()
         t1.join()
         
         
         if allegedpass == self.den.decode('ascii'):
             t = threading.Thread(target=self.arch.decrypt, args=(self.arch.__searchresult__['password'],))
             t.start()
             t.join()
             
-            pyperclip.copy(self.arch._dec_)
+            pyperclip.copy(self.arch.dec)
             spam = pyperclip.paste()
             self.arch._dec_ = None
         else:
             messagebox.showwarning("Wrong Master Password", "The master password entered by you is wrong!")
+    
+    def decryptthread(self, masterpassword: str):
+            denc = Encryption(masterpassword.encode('ascii'))
+            self.den = denc.unlock()
+            sys.exit(0)
         
     def _makeAdd_(self):
         # -> create enclosing frame under Add
         self.AEF = ttk.Frame(self.addtab)
         self.AEF.pack(expand=True, fill=BOTH)
         
         # -> create target label and input
```

### Comparing `pasta_man-1.1.0/src/pasta_man/architectures/targets.py` & `pasta_man-1.1.1/src/pasta_man/architectures/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,27 +267,44 @@
         self.__searchresult__ = None
         
         for dictionary in self.data:
             if searchkeyword in dictionary[keywordtype]:
                 self.__searchresult__ = dictionary
         
         sys.exit(0)
+    
+    def searchAll(self, searchkeyword:str, keywordtype: str = "target"):
+        valid = ['target', 'target-type', 'username']
+        
+        if keywordtype not in valid:
+            raise InvalidKeyword(f'{keywordtype} cannot be set as keywordtype.')
+        
+        self.__searchAllResult = []
+        
+        for dictionary in self.data:
+            if searchkeyword in dictionary[keywordtype]:
+                self.__searchAllResult.append(dictionary)
+    
+    def __fetchSearchAll(self):
+        return self.__searchAllResult
+    
+    searchAllResults = property(fget=__fetchSearchAll)
 
     def targets(self):
         ts:list[str] = []
         added = []
         for dictionary in self.data:
             if dictionary['target-type']!="init" and dictionary['target-type'] not in added:
                 ts.append(dictionary['target-type'])
                 added.append(dictionary['target-type'])
         
         self.__target_types__ = ts
     
     def decrypt(self, password: bytes):
-        self._dec_ = self.fernet.decrypt(password).decode('ascii')
+        self.dec = self.fernet.decrypt(password).decode('ascii')
         sys.exit(0)
     
     def export(self, exporttype: str = "csv", path: str = pwd()) -> None:
         """General purpose Export. Excludes timestamp.
 
         Args:
             exporttype (str, optional): specify export type. Valid -> ['.csv', '.xlsx']. Defaults to ".csv".
```

### Comparing `pasta_man-1.1.0/src/pasta_man/pasta_man.py` & `pasta_man-1.1.1/src/pasta_man/pasta_man.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
             sys (module)
             platform (module)
     - external:
         - description: Needs to be installed using pip.
         -contents:
             tkinter.* (all)
             tkinter.simpledialog (module)
-            termcolor.colored (function)
+            colorama.init (function)
+            colorama.Fore (variable)
             optioner.options (class)
     - Project Specific
         - description: Modules made for this project.
         - contents:
             pasta_man.architectures.gui.pmanager (class)
             pasta_man.encryption.Encryption (class)
             pasta_man.exceptions.NoneTypeVariable (class)
@@ -55,26 +56,27 @@
 Working:
     - catch and analyse arguments if any. If Found, execute it. Else Move on.
     - Check for master password
     - If found, decrypt it and call pmanager class. If not found, ask the user for master password, encrypt and save it and then call pmanager class.
 """
 
 # version info
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 # import internal modules
 from pathlib import Path
-from os.path import join as jPath, exists as there
+from os.path import join as jPath, exists as there, dirname, abspath
 from os import makedirs
+from shutil import rmtree
 import sys, threading
 
 # import external modules
 from tkinter import *
 from tkinter import simpledialog
-from termcolor import colored
+from colorama import init as color, Fore as f
 
 # import project specific modules
 from pasta_man.architectures.gui import pmanager
 from pasta_man.architectures.terminal import Terminal
 from pasta_man.utilities.encryption import Encryption
 from pasta_man.utilities.Exceptions.exceptions import NoneTypeVariable
 from pasta_man.utilities.Exceptions.TerminalExceptions import EmptyArgument
@@ -158,28 +160,35 @@
     
     return masterpassword
 
 def main():
     """
     The main function of the program.
     """
+    # initialize colorama
+    color()
     # -> home folder
     home = str(Path.home())
     # -> find out if .pastaman folder is there
     if not there(jPath(home, '.pastaman')):
         makedirs(jPath(home, '.pastaman'))
     
     masterpassword = checkmfile()
     
     # define global vars
     global encb, dencb
     
     
     try:
         terminal = Terminal(__version__, sys.argv[1:], masterpassword)
+        # clear __pycache__
+        # -> get directory
+        install_directory = dirname(abspath(__file__))
+        rmtree(jPath(install_directory, '__pycache__'))
+        sys.exit(0)
     except EmptyArgument:
         pass
     
     # define main root gui window
     rootwindow = Tk()
     
     # create pass manager object.
@@ -190,9 +199,9 @@
 
 if __name__=="__main__":
     encb:bytes = ''.encode('ascii')
     dencb:bytes = ''.encode('ascii')
     try:
         sys.exit(main())
     except KeyboardInterrupt:
-        print("\n"+colored("KEYBOARD INTERRUPT", 'red'))
+        print("\n"+f"{f.RED}KEYBOARD INTERRUPT{f.RESET}")
         sys.exit(1)
```

### Comparing `pasta_man-1.1.0/src/pasta_man/self_launch_thread/Launcher.py` & `pasta_man-1.1.1/src/pasta_man/self_launch_thread/Launcher.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.0/src/pasta_man/utilities/Exceptions/exceptions.py` & `pasta_man-1.1.1/src/pasta_man/utilities/Exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.0/src/pasta_man/utilities/encryption.py` & `pasta_man-1.1.1/src/pasta_man/utilities/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.0/src/pasta_man/utilities/pasta_docs.py` & `pasta_man-1.1.1/src/pasta_man/utilities/pasta_docs.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.0/src/pasta_man/utilities/pasta_menu.py` & `pasta_man-1.1.1/src/pasta_man/utilities/pasta_menu.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.0/src/pasta_man/utilities/retransform.py` & `pasta_man-1.1.1/src/pasta_man/utilities/retransform.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.1.0/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.1.0
+Version: 1.1.1
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -41,91 +41,161 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: pandas
-Requires-Dist: termcolor
+Requires-Dist: colorama
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 Requires-Dist: ttkthemes
 Requires-Dist: pyinstaller
+Requires-Dist: wrapper-bar>=0.1.3
+
+# Overview
+
+Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access.
+
+## Project Badges
 
 [![Continuous Deployment](https://github.com/d33pster/pasta-man/actions/workflows/ContinuousDeployment.yml/badge.svg)](https://github.com/d33pster/pasta-man/actions/workflows/ContinuousDeployment.yml)
 ![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
 ![PyPI - Status](https://img.shields.io/pypi/status/pasta-man)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
 ![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
 
+## Changelog
 
-# Overview
-Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access. 
+See Changelog [here](CHANGELOG.md).
+
+## Table of Contents
+
+- [Motivation](#motivation)
+- [Features](#features)
+  - [Secure Management of Passwords](#secure-management-of-passwords)
+  - [Tags](#tags)
+  - [Search](#search)
+  - [Copy to Clipboard](#copy-to-clipboard)
+  - [Faster than basic tkinter apps](#faster-than-basic-tkinter-apps)
+  - [Import-Export Passwords](#import-export-passwords)
+  - [Code Description](#code-description)
+  - [Themes](#themes)
+    - [Currently Supported Themes](#currently-supported-themes)
+- [Dependencies](#dependencies)
+- [Installation](#installation)
+- [README before #Usage](#readme-before-usage)
+- [Usage](#usage)
+- [Troubleshooting](#troubleshooting)
+- [Uninstall](#uninstall)
+- [Yanked Versions](#yanked-versions)
 
 ## Motivation
- - In the digital login password age we need a one stop vault for storing all our login credentials with concerned of atmost  security.
- - The repeated use of single password in multiple accounts may lead to data breach or loss of data.
- - Weak passwords are easy to interpreat for attackers, use of strong passwords is recommended,but it is difficult to remember complex passwords.
- - Mostly passwords written in somewhere lead to comprosing of data and privacy of user.
+
+- In the digital login password age we need a one stop vault for storing all our login credentials with concerned of atmost  security.
+- The repeated use of single password in multiple accounts may lead to data breach or loss of data.
+- Weak passwords are easy to interpreat for attackers, use of strong passwords is recommended,but it is difficult to remember complex passwords.
+- Mostly passwords written in somewhere lead to comprosing of data and privacy of user.
 
 ## Features
  <!-- - Securely Managing Passwords
  - Copy passwords to the clipboard
  - One master password for all
  - Exporting all passwords in desired file format
  - Encrypting passwords
  - Search Password by target name/username -->
 
 ### Secure Management of Passwords
+
 `Pasta-Man` uses tripple layer encryption for saving passwords. Once `Pasta-Man` is provided with a password to manage, it encrypts it with a Master Password and stores it in a file, which then again is encrypted with the master password. The so called Master password is stored as an encrypted string (this encryption is done using password and salt not known to users.).
 
 The user will be prompted to provide a master password if it is the first use. If not, `Pasta-Man` will work as usual.
 
 ### Tags
+
 `Pasta-Man` stores passwords with tags such as target (the target application or link or any platform the password is meant for), target-type (target-type can be an app or link or any other category defined by the user. --- `Pasta-Man` supports creation of user defined tags and can easily fetch search results for the same.).
 
 ### Search
+
 User can search for passwords using keywords in keyword-types.
 
-`For Example:`<br>
+`For Example:`  
 If there is a target (say, abcde) which contains a keyword (say, abc), the user can search `abc` in `keyword-type == target`. Similarly, if there is a target-type (say, link) which contains a keyword (say, github), the user can search for `github` in `keyword-type == target-type`.
 
 ### Copy to Clipboard
+
 Upon [Search](#search), `Pasta-Man` allows to copy the password for the found match to user's clipboard (given, the user provides the master password), instead of revealing it because of bad management. `Pasta-Man` also allows to Remove that match search result.
 
 ### Faster than basic tkinter apps
+
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Import-Export Passwords
+
 `Pasta-Man` _v1.0.10_ onwards supports importing and exporting of passwords. **Note:** `Pasta-Man` can only import passwords that were exported by `Pasta-Man`. This Import/Export Feature is a solution to changing your PC or system.
 
 Be relieved that the exported passwords will be in encrypted format.
 
 - **Export Format:** `Pasta-Man` will append all the passwords encrypted by master password and all the data associated with it, to the encrypted master password into the output format chosen by user.
 
 - **Import Mechanism:** `Pasta-Man` will decrypt the master password associated with the passwords file and then decrypt all the data appended to it and then encrypt the data and passwords by using the current system master password, then append it to the currently existing passwords. And finally encrypt everything again.
 
 - **Usage:**
+
     ```bash
     pasta-man -e <output-file-format> # or pasta-man --export <output-file-format>
 
     pasta-man -i # or pasta-man --import
     ```
 
     Both of the commands above will trigger a file/directory selector dialog for selecting the desired directory or files.
 
+### Code Description
+
+To know more about the code structure and module information like -
+
+- Modules that are imported
+
+  - Internal (all the modules used that already come with your python interpreter)
+
+  - External (all the modules used that were installed using pip, these are also mentioned in pyproject.toml and requirements.txt)
+
+  - Project specifiv (all the modules used that were specifically created for this project.)
+
+- Hierarchy
+
+    The hierarchy of classes and functions.
+
+- Individial Object Descriptions
+
+    Descriptions about individual components of the code such as funtions and parameters.
+
+- Working
+
+    If there is any working rule or basic working of the module.
+
+All these can be seen by running the following commands:
+
+```console
+# pasta-man v1.0.9 and above supports docstring fetching, and can be done using:
+
+# in the terminal/CMD, run
+$ pasta-man -dwl # for docs with listing of hierarchy.
+```
 
 ### Themes
+
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
 Themes can be changed using the MenuBar -
 
-<img src="images/MenuBar.png">
+<!-- <img src="images/MenuBar.png"> -->
+![menubarimage](images/MenuBar.png)
 
 ###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
@@ -140,133 +210,109 @@
 - Kroc
 - Plastik
 - Radiance (Ubuntu)
 - Smog
 - Win XP
 - Yaru
 
-## Code Description
-
-To know more about the code structure and module information like - 
-
-- Modules that are imported
-    
-    - Internal (all the modules used that already come with your python interpreter)
-
-    - External (all the modules used that were installed using pip, these are also mentioned in pyproject.toml and requirements.txt)
-
-    - Project specifiv (all the modules used that were specifically created for this project.)
-
-- Hierarchy
-    
-    The hierarchy of classes and functions.
-
-- Individial Object Descriptions
-
-    Descriptions about individual components of the code such as funtions and parameters.
-
-- Working
-
-    If there is any working rule or basic working of the module.
-
-All these can be seen by running the following commands:
-
-```console
-# pasta-man v1.0.9 and above supports docstring fetching, and can be done using:
-
-# in the terminal/CMD, run
-$ pasta-man -dwl # for docs with listing of hierarchy.
-```
-
 ## Dependencies
+
 - Python>=3.9
 - pandas
 - tk
 - ttkthemes
-- termcolor
+- colorama
+- wrapper-bar>=0.1.3
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 - pyinstaller
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.1.0
+pip install pasta-man==1.1.1
 ```
 
 ## README before [#Usage](#usage)
 
 After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man>=1.0.4` -> `pasta-man` and `pasta-man-launcher`.
 
 - `pasta-man` Command
 
-    - This command will launch `pasta-man` as a separate and independent process.
-    
-    - The terminal will be usable after `pasta-man` command is run.
-    
-    - The output logs will be stored in -> `HOME/.pastaman/.log` in Linux and MacOS.
+  - This command will launch `pasta-man` as a separate and independent process.
+
+  - The terminal will be usable after `pasta-man` command is run.
+
+  - The output logs will be stored in -> `HOME/.pastaman/.log` in Linux and MacOS.
 
 - `pasta-man-launcher` Command
-    
-    - This will launch `pasta-man` in the terminal.
 
-    - The terminal wont be available until this process is running.
+  - This will launch `pasta-man` in the terminal.
 
-    - All outputs will be logged in `stdin` (in the terminal screen)
+  - The terminal wont be available until this process is running.
+
+  - All outputs will be logged in `stdin` (in the terminal screen)
 
 ## Usage
 
-- To run `Pasta-Man`, run the following in the terminal/CMD.
+- To run `Pasta-Man`, run the following in the terminal/CMD. This will open up GUI.
 
     ```bash
-    pasta-man
+    $ pasta-man
+    ...
     ```
 
-- To show version information, run the following in terminal/CMD
+- To show full list of CLI commands supported by `pasta-man`, in terminal/CMD, run:
+
     ```bash
-    pasta-man -v # or pasta-man --version
+    $ pasta-man -h # or pasta-man --help
+    Pasta Man v1.1.1
+    helptext
+      |  -h or --help                     : show this help and exit.
+      |  -v or --version                  : show version and exit.
+      |  -p or --path                     : show install path and exit.
+      |  -rmc or --remove-configurations  : remove existing configs. [Warning] This is irreversible.
+      |  -dwl or --doc-w-list             : list all modules of pasta-man. Enter the full-module-name for docstring.
+      |  -i or --import                   : import a passwords file. Only files exported by pasta-man can be imported.
+      |                                     Syntax: pasta-man --import
+      |  -e or --export                   : export passwords.
+      |                                     Syntax: pasta-man --export <export-format>
+      |                                     Available export formats -> ['csv', 'xlsx']
+      |  -s or --search                   : search a keyword in keyword-type.
+      |                                     Syntax: pasta-man --search <keyword-type> <keyword>
+      |                                     Available keyword types -> ['target', 'target-type', 'username']
     ```
 
 ## Troubleshooting
 
 - Windows
-    - Running `pasta-man` for the first time will trigger a setup mechanism. If the setup fails for any reason, run the following commands in the CMD.
+  - Running `pasta-man` for the first time will trigger a setup mechanism. If the setup fails for any reason, run the following commands in the CMD.
 
-        ```batch
-        pasta-man -rmc
-        ```
-        
-        or
+    ```batch
+    pasta-man -rmc
+    ```
 
-        
-        ```batch
-        pasta-man --remove-configurations
-        ```
-        And then run `pasta-man` again.
-    
-    - For Complete list of Developer Options of pasta-man, run the following commands.
-
-        ```batch
-        pasta-man -h
-        ```
-        
-        or
+    or
+
+    ```batch
+    pasta-man --remove-configurations
+    ```
 
-        ```batch
-        pasta-man --help
-        ```
+    And then run `pasta-man` again.  
+    NOTE: This command is irreversible and will also delete master password along with any saved passwords.
 
 ## Uninstall
 
 Uninstall using pip
 
 ```bash
 pip uninstall pasta-man
 ```
 
 ## Yanked Versions
+
 - _v1.0.5_
-    
+
     `Major Bug`: After Threads Update and Threads Patch 1, There was a major bug where the code breaks while initializing the app for the first time.
```

### Comparing `pasta_man-1.1.0/src/pasta_man.egg-info/SOURCES.txt` & `pasta_man-1.1.1/src/pasta_man.egg-info/SOURCES.txt`

 * *Files identical despite different names*

