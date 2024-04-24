# Comparing `tmp/mojo_startup-1.3.5.tar.gz` & `tmp/mojo_startup-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_startup-1.3.5.tar", max compression
+gzip compressed data, was "mojo_startup-1.3.6.tar", max compression
```

## Comparing `mojo_startup-1.3.5.tar` & `mojo_startup-1.3.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:53:07.681820 mojo_startup-1.3.5/LICENSE.txt
--rw-r--r--   0        0        0     2243 2024-01-27 22:53:25.349475 mojo_startup-1.3.5/README.rst
--rw-r--r--   0        0        0      683 2024-01-27 22:53:41.157442 mojo_startup-1.3.5/pyproject.toml
--rw-r--r--   0        0        0        2 2024-01-26 02:53:07.683481 mojo_startup-1.3.5/source/packages/mojo/startup/__init__.py
--rw-r--r--   0        0        0     1090 2024-01-27 22:22:51.047994 mojo_startup-1.3.5/source/packages/mojo/startup/converters.py
--rw-r--r--   0        0        0     1846 2024-01-27 22:41:19.877478 mojo_startup-1.3.5/source/packages/mojo/startup/startupconfigloader.py
--rw-r--r--   0        0        0      895 2024-01-26 02:53:07.683567 mojo_startup-1.3.5/source/packages/mojo/startup/startupvariables.py
--rw-r--r--   0        0        0      588 2024-01-26 02:53:07.683648 mojo_startup-1.3.5/source/packages/mojo/startup/wellknown.py
--rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 mojo_startup-1.3.5/setup.py
--rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 mojo_startup-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:53:07.681820 mojo_startup-1.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     2243 2024-01-27 22:53:25.349475 mojo_startup-1.3.6/README.rst
+-rw-r--r--   0        0        0      683 2024-04-24 03:46:08.513423 mojo_startup-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0        2 2024-01-26 02:53:07.683481 mojo_startup-1.3.6/source/packages/mojo/startup/__init__.py
+-rw-r--r--   0        0        0     1090 2024-01-27 22:22:51.047994 mojo_startup-1.3.6/source/packages/mojo/startup/converters.py
+-rw-r--r--   0        0        0     1846 2024-01-27 22:41:19.877478 mojo_startup-1.3.6/source/packages/mojo/startup/startupconfigloader.py
+-rw-r--r--   0        0        0      895 2024-02-14 07:33:20.501387 mojo_startup-1.3.6/source/packages/mojo/startup/startupvariables.py
+-rw-r--r--   0        0        0      588 2024-01-26 02:53:07.683648 mojo_startup-1.3.6/source/packages/mojo/startup/wellknown.py
+-rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 mojo_startup-1.3.6/setup.py
+-rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 mojo_startup-1.3.6/PKG-INFO
```

### Comparing `mojo_startup-1.3.5/LICENSE.txt` & `mojo_startup-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_startup-1.3.5/README.rst` & `mojo_startup-1.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_startup-1.3.5/pyproject.toml` & `mojo_startup-1.3.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-startup"
 description = "Automation Mojo Startup Package"
-version = "1.3.5"
+version = "1.3.6"
 authors = ["Myron W. Walker"]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_startup-1.3.5/source/packages/mojo/startup/converters.py` & `mojo_startup-1.3.6/source/packages/mojo/startup/converters.py`

 * *Files identical despite different names*

### Comparing `mojo_startup-1.3.5/source/packages/mojo/startup/startupconfigloader.py` & `mojo_startup-1.3.6/source/packages/mojo/startup/startupconfigloader.py`

 * *Files identical despite different names*

### Comparing `mojo_startup-1.3.5/source/packages/mojo/startup/startupvariables.py` & `mojo_startup-1.3.6/source/packages/mojo/startup/startupvariables.py`

 * *Files identical despite different names*

### Comparing `mojo_startup-1.3.5/source/packages/mojo/startup/wellknown.py` & `mojo_startup-1.3.6/source/packages/mojo/startup/wellknown.py`

 * *Files identical despite different names*

### Comparing `mojo_startup-1.3.5/setup.py` & `mojo_startup-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['mojo', 'mojo.startup']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-startup',
-    'version': '1.3.5',
+    'version': '1.3.6',
     'description': 'Automation Mojo Startup Package',
     'long_description': '=======================\nmojo-startup\n=======================\nThis package sets up a pattern for extremely early pre-configuration of variable extensibility\nhook for the startup configuration.  This module looks for a single environment variable to be set:\n\n.. code::\n\n    MJR_STARTUP_SETTINGS\n\nThe value of this variable is accessed like so:\n\n.. code::\n\n    from mojo.startup.startupvariables import MOJO_STARTUP_VARIABLES\n    \n    print(MOJO_STARTUP_VARIABLES.MJR_STARTUP_SETTINGS)\n\n\nThe `MJR_STARTUP_SETTINGS` variable is set to the path for a config file that should point to the\nconfiguration file that is used to startup the runtime.\n\nThe default value for the `MJR_STARTUP_SETTINGS` variable is `~/.mojo.config`.\n\nThe `mojo-startup` module makes a singleton `ConfigParser` available for other modules to use.  This\nconfiguration parser can be accessed by:\n\n.. code::\n    \n    from mojo.startup.wellknown import StartupConfigSingleton\n    \n    cparser = StartupConfigSingleton()\n    \n    defaults_section = cparser["DEFAULTS"]\n    someval = defaults_section["SOME_VARIABLE"]\n\n===========\nDescription\n===========\nThis module does one very important thing.  It establishes the path for all other \'mojo\' packages\non where to load default config from.  This is very important because it provides extensibility\nas early as possible in the running of any code.\n\nThe pattern established for defaults for variables is:\n* Variable is set to a hard coded default\n* Startup configuration is checked for an override\n* The environment variables are checked for an override\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here \'source/packages/(root-module-folder)\'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'Myron W. Walker',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_startup-1.3.5/PKG-INFO` & `mojo_startup-1.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-startup
-Version: 1.3.5
+Version: 1.3.6
 Summary: Automation Mojo Startup Package
 License: LICENSE.txt
 Keywords: python
 Author: Myron W. Walker
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
```

