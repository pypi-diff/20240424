# Comparing `tmp/mojo_config-1.3.8.tar.gz` & `tmp/mojo_config-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_config-1.3.8.tar", max compression
+gzip compressed data, was "mojo_config-1.3.9.tar", max compression
```

## Comparing `mojo_config-1.3.8.tar` & `mojo_config-1.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:52:58.503511 mojo_config-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0     1905 2024-01-26 02:52:58.503687 mojo_config-1.3.8/README.rst
--rw-r--r--   0        0        0     1043 2024-03-08 13:14:01.760031 mojo_config-1.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-14 07:06:33.999395 mojo_config-1.3.8/source/packages/mojo/config/__init__.py
--rw-r--r--   0        0        0       98 2024-01-26 02:52:58.505324 mojo_config-1.3.8/source/packages/mojo/config/configurationformat.py
--rw-r--r--   0        0        0     7257 2024-01-26 02:52:58.505428 mojo_config-1.3.8/source/packages/mojo/config/configurationloader.py
--rw-r--r--   0        0        0     9946 2024-01-26 02:52:58.505520 mojo_config-1.3.8/source/packages/mojo/config/configurationmaps.py
--rw-r--r--   0        0        0     2140 2024-03-08 13:13:47.204459 mojo_config-1.3.8/source/packages/mojo/config/configurationsettings.py
--rw-r--r--   0        0        0     2598 2024-01-26 02:52:58.505617 mojo_config-1.3.8/source/packages/mojo/config/cryptography.py
--rw-r--r--   0        0        0       48 2024-01-26 02:52:58.505680 mojo_config-1.3.8/source/packages/mojo/config/defaultvalues.py
--rw-r--r--   0        0        0     1246 2024-01-26 02:52:58.505767 mojo_config-1.3.8/source/packages/mojo/config/normalize.py
--rw-r--r--   0        0        0     8265 2024-03-08 13:09:28.787631 mojo_config-1.3.8/source/packages/mojo/config/optionoverrides.py
--rw-r--r--   0        0        0        0 2024-02-14 07:06:19.746083 mojo_config-1.3.8/source/packages/mojo/config/sources/__init__.py
--rw-r--r--   0        0        0      597 2024-01-26 02:52:58.506066 mojo_config-1.3.8/source/packages/mojo/config/sources/configurationsourcebase.py
--rw-r--r--   0        0        0     2819 2024-01-26 02:52:58.506171 mojo_config-1.3.8/source/packages/mojo/config/sources/couchdbsource.py
--rw-r--r--   0        0        0     2178 2024-01-26 02:52:58.506265 mojo_config-1.3.8/source/packages/mojo/config/sources/directorysource.py
--rw-r--r--   0        0        0     2152 2024-01-26 02:52:58.506342 mojo_config-1.3.8/source/packages/mojo/config/sources/httpsource.py
--rw-r--r--   0        0        0     2467 2024-01-26 02:52:58.506455 mojo_config-1.3.8/source/packages/mojo/config/sources/mongodbsource.py
--rw-r--r--   0        0        0     9896 2024-03-08 13:09:32.252741 mojo_config-1.3.8/source/packages/mojo/config/variables.py
--rw-r--r--   0        0        0     1785 2024-03-08 02:13:15.968650 mojo_config-1.3.8/source/packages/mojo/config/wellknown.py
--rw-r--r--   0        0        0     2999 1970-01-01 00:00:00.000000 mojo_config-1.3.8/setup.py
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 mojo_config-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:52:58.503511 mojo_config-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     1905 2024-01-26 02:52:58.503687 mojo_config-1.3.9/README.rst
+-rw-r--r--   0        0        0     1044 2024-03-08 13:51:14.884919 mojo_config-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-14 07:06:33.999395 mojo_config-1.3.9/source/packages/mojo/config/__init__.py
+-rw-r--r--   0        0        0       98 2024-01-26 02:52:58.505324 mojo_config-1.3.9/source/packages/mojo/config/configurationformat.py
+-rw-r--r--   0        0        0     7257 2024-01-26 02:52:58.505428 mojo_config-1.3.9/source/packages/mojo/config/configurationloader.py
+-rw-r--r--   0        0        0     9946 2024-01-26 02:52:58.505520 mojo_config-1.3.9/source/packages/mojo/config/configurationmaps.py
+-rw-r--r--   0        0        0     2317 2024-03-08 13:51:03.114194 mojo_config-1.3.9/source/packages/mojo/config/configurationsettings.py
+-rw-r--r--   0        0        0     2598 2024-01-26 02:52:58.505617 mojo_config-1.3.9/source/packages/mojo/config/cryptography.py
+-rw-r--r--   0        0        0       48 2024-01-26 02:52:58.505680 mojo_config-1.3.9/source/packages/mojo/config/defaultvalues.py
+-rw-r--r--   0        0        0     1246 2024-01-26 02:52:58.505767 mojo_config-1.3.9/source/packages/mojo/config/normalize.py
+-rw-r--r--   0        0        0     8265 2024-03-08 13:09:28.787631 mojo_config-1.3.9/source/packages/mojo/config/optionoverrides.py
+-rw-r--r--   0        0        0        0 2024-02-14 07:06:19.746083 mojo_config-1.3.9/source/packages/mojo/config/sources/__init__.py
+-rw-r--r--   0        0        0      597 2024-01-26 02:52:58.506066 mojo_config-1.3.9/source/packages/mojo/config/sources/configurationsourcebase.py
+-rw-r--r--   0        0        0     2819 2024-01-26 02:52:58.506171 mojo_config-1.3.9/source/packages/mojo/config/sources/couchdbsource.py
+-rw-r--r--   0        0        0     2178 2024-01-26 02:52:58.506265 mojo_config-1.3.9/source/packages/mojo/config/sources/directorysource.py
+-rw-r--r--   0        0        0     2152 2024-01-26 02:52:58.506342 mojo_config-1.3.9/source/packages/mojo/config/sources/httpsource.py
+-rw-r--r--   0        0        0     2467 2024-01-26 02:52:58.506455 mojo_config-1.3.9/source/packages/mojo/config/sources/mongodbsource.py
+-rw-r--r--   0        0        0     9896 2024-03-08 13:09:32.252741 mojo_config-1.3.9/source/packages/mojo/config/variables.py
+-rw-r--r--   0        0        0     1785 2024-03-08 02:13:15.968650 mojo_config-1.3.9/source/packages/mojo/config/wellknown.py
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 mojo_config-1.3.9/setup.py
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 mojo_config-1.3.9/PKG-INFO
```

### Comparing `mojo_config-1.3.8/LICENSE.txt` & `mojo_config-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/README.rst` & `mojo_config-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/pyproject.toml` & `mojo_config-1.3.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-config"
 description = "Automation Mojo Configuration Package"
-version = "1.3.8"
+version = "1.3.9"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
@@ -19,15 +19,15 @@
 python = ">=3.8,<4.0"
 pymongo = {extras = ["srv"], version = "^4.0.0", optional = true}
 couchdb = {version = "^1.2", optional = true}
 cryptography = "^41.0.3"
 mojo-errors = ">=1.3.0 <1.4.0"
 mojo-collections = ">=1.3.0 <1.4.0"
 mojo-startup = ">=1.3.5 <1.4.0"
-mojo-extension = ">=1.3.9 <1.4.0"
+mojo-extension = ">=1.3.10 <1.4.0"
 mojo-credentials = ">=1.3.1 <1.4.0"
 
 [tool.poetry.extras]
 mongodb = ["pymongo"]
 couchdb = ["couchdb"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/configurationloader.py` & `mojo_config-1.3.9/source/packages/mojo/config/configurationloader.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/configurationmaps.py` & `mojo_config-1.3.9/source/packages/mojo/config/configurationmaps.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/configurationsettings.py` & `mojo_config-1.3.9/source/packages/mojo/config/configurationsettings.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import Optional
 
 from mojo.startup.wellknown import StartupConfigSingleton
-from mojo.extension.extensionsettings import establish_startup_settings
+from mojo.extension.extensionsettings import establish_extension_settings
 
 default_config = {}
 
 startup_config = StartupConfigSingleton()
 if "DEFAULT" in startup_config:
     default_config = startup_config["DEFAULT"]
 
@@ -52,15 +52,22 @@
                 "console": "INFO",
                 "logfile": "DEBUG"
             }
         }
     }
 
 
+CONFIG_SETTINGS_ESTABLISHED = False
+
 def establish_config_settings(*, name: Optional[str]=None, home_dir: Optional[str]=None,  default_configuration: Optional[dict]=None):
 
-    establish_startup_settings(name=name, home_dir=home_dir)
+    global CONFIG_SETTINGS_ESTABLISHED
+
+    if not CONFIG_SETTINGS_ESTABLISHED:
+        CONFIG_SETTINGS_ESTABLISHED = True
+
+        establish_extension_settings(name=name, home_dir=home_dir)
 
-    if default_configuration is not None:
-        MOJO_CONFIG_DEFAULTS.DEFAULT_CONFIGURATION = default_configuration
+        if default_configuration is not None:
+            MOJO_CONFIG_DEFAULTS.DEFAULT_CONFIGURATION = default_configuration
 
     return
```

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/cryptography.py` & `mojo_config-1.3.9/source/packages/mojo/config/cryptography.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/normalize.py` & `mojo_config-1.3.9/source/packages/mojo/config/normalize.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/optionoverrides.py` & `mojo_config-1.3.9/source/packages/mojo/config/optionoverrides.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/sources/configurationsourcebase.py` & `mojo_config-1.3.9/source/packages/mojo/config/sources/configurationsourcebase.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/sources/couchdbsource.py` & `mojo_config-1.3.9/source/packages/mojo/config/sources/couchdbsource.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/sources/directorysource.py` & `mojo_config-1.3.9/source/packages/mojo/config/sources/directorysource.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/sources/httpsource.py` & `mojo_config-1.3.9/source/packages/mojo/config/sources/httpsource.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/sources/mongodbsource.py` & `mojo_config-1.3.9/source/packages/mojo/config/sources/mongodbsource.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/variables.py` & `mojo_config-1.3.9/source/packages/mojo/config/variables.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/source/packages/mojo/config/wellknown.py` & `mojo_config-1.3.9/source/packages/mojo/config/wellknown.py`

 * *Files identical despite different names*

### Comparing `mojo_config-1.3.8/setup.py` & `mojo_config-1.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 {'': ['*']}
 
 install_requires = \
 ['cryptography>=41.0.3,<42.0.0',
  'mojo-collections>=1.3.0,<1.4.0',
  'mojo-credentials>=1.3.1,<1.4.0',
  'mojo-errors>=1.3.0,<1.4.0',
- 'mojo-extension>=1.3.9,<1.4.0',
+ 'mojo-extension>=1.3.10,<1.4.0',
  'mojo-startup>=1.3.5,<1.4.0']
 
 extras_require = \
 {'couchdb': ['couchdb>=1.2,<2.0'], 'mongodb': ['pymongo[srv]>=4.0.0,<5.0.0']}
 
 setup_kwargs = {
     'name': 'mojo-config',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'Automation Mojo Configuration Package',
     'long_description': '=======================\npython-package-template\n=======================\nThis is a template repository that can be used to quickly create a python package project.\n\n=========================\nFeatures of this Template\n=========================\n* Machine Setup\n* Virtual Environment Setup (Poetry)\n* PyPi Publishing\n* Sphinx Documentation\n\n========================\nHow to Use This Template\n========================\n- Click the \'Use this template\' button\n- Fill in the information to create your repository\n- Checkout your new repository\n- Change the following in \'repository-config.ini\'\n\n  #. \'PROJECT NAME\'\n  #. \'REPOSITORY_NAME\'\n\n- If you have machine dependencies to add, put them in \'setup-ubuntu-machine\'\n- Modify the pyproject.toml file with the correct package-name, author, publishing information, etc.\n- Rename the VSCODE workspace file \'mv workspaces/default-workspace.template workspaces/(project name).template\'\n- Replace the README.rst file with your own README\n- Add your dependencies with python poetry \'poetry add (dependency name)\'\n- Drop your package code in \'source/packages\'\n- Modify the name of your package root in \'pyproject.toml\'\n\n  #. \'packages = [{include="(root folder name)", from="source/packages"}]\'\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here \'source/packages/(root-module-folder)\'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_config-1.3.8/PKG-INFO` & `mojo_config-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-config
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automation Mojo Configuration Package
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
@@ -17,15 +17,15 @@
 Provides-Extra: couchdb
 Provides-Extra: mongodb
 Requires-Dist: couchdb (>=1.2,<2.0) ; extra == "couchdb"
 Requires-Dist: cryptography (>=41.0.3,<42.0.0)
 Requires-Dist: mojo-collections (>=1.3.0,<1.4.0)
 Requires-Dist: mojo-credentials (>=1.3.1,<1.4.0)
 Requires-Dist: mojo-errors (>=1.3.0,<1.4.0)
-Requires-Dist: mojo-extension (>=1.3.9,<1.4.0)
+Requires-Dist: mojo-extension (>=1.3.10,<1.4.0)
 Requires-Dist: mojo-startup (>=1.3.5,<1.4.0)
 Requires-Dist: pymongo[srv] (>=4.0.0,<5.0.0) ; extra == "mongodb"
 Description-Content-Type: text/x-rst
 
 =======================
 python-package-template
 =======================
```

