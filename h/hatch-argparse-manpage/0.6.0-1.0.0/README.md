# Comparing `tmp/hatch_argparse_manpage-0.6.0.tar.gz` & `tmp/hatch_argparse_manpage-1.0.0.tar.gz`

## Comparing `hatch_argparse_manpage-0.6.0.tar` & `hatch_argparse_manpage-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/CHANGES.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/.gitignore
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/hatch-argparse-manpage.iml
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/vcs.xml
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/hooks.py
--rw-r--r--   0        0        0    19363 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/py.typed
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0    12052 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/README.md
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 hatch_argparse_manpage-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/CHANGES.md
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/.idea/.gitignore
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/.idea/hatch-argparse-manpage.iml
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/docs/hatch-argparse-manpage.3.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/hatch_argparse_manpage/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/hatch_argparse_manpage/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/hatch_argparse_manpage/hooks.py
+-rw-r--r--   0        0        0    19363 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/hatch_argparse_manpage/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/hatch_argparse_manpage/py.typed
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0    12053 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/README.md
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 hatch_argparse_manpage-1.0.0/PKG-INFO
```

### Comparing `hatch_argparse_manpage-0.6.0/.idea/inspectionProfiles/Project_Default.xml` & `hatch_argparse_manpage-1.0.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `hatch_argparse_manpage-0.6.0/hatch_argparse_manpage/plugin.py` & `hatch_argparse_manpage-1.0.0/hatch_argparse_manpage/plugin.py`

 * *Files identical despite different names*

### Comparing `hatch_argparse_manpage-0.6.0/.gitignore` & `hatch_argparse_manpage-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_argparse_manpage-0.6.0/LICENSE.txt` & `hatch_argparse_manpage-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_argparse_manpage-0.6.0/README.md` & `hatch_argparse_manpage-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 requires = ["hatchling", "hatch-argparse-manpage"]
 build-backend = "hatchling.build"
 ```
 
 ### Generating the manual page
 
 This plugin requires the directories storing the generated man pages are 
-within the project's base directory, and is not equal to the project's base 
+within the project's base directory, and are not equal to the project's base 
 directory.
 
 For example, for a project named `myproject`, and a src layout
 `src/myproject`, an acceptable directory in which to store a
 man page would be `man`.
 
 Using the configuration option `[tool.hatch.build.hooks.argparse-manpage]`,
```

### Comparing `hatch_argparse_manpage-0.6.0/pyproject.toml` & `hatch_argparse_manpage-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,22 @@
   "build",
   "hatch",
   "plugin",
   "typing",
   "documentation",
   "manpage",
   "manual page",
-  "help"
+  "help",
+  "man page",
 ]
 authors = [
   { name = "Damon Lynch", email = "damonlynch@gmail.com" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
   "Framework :: Hatch",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
```

### Comparing `hatch_argparse_manpage-0.6.0/PKG-INFO` & `hatch_argparse_manpage-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: hatch-argparse-manpage
-Version: 0.6.0
+Version: 1.0.0
 Summary: Hatch build hook plugin to generate manual pages
 Project-URL: Documentation, https://github.com/damonlynch/hatch-argparse-manpage#readme
 Project-URL: Issues, https://github.com/damonlynch/hatch-argparse-manpage/issues
 Project-URL: Homepage, https://github.com/damonlynch/hatch-argparse-manpage
 Author-email: Damon Lynch <damonlynch@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.txt
-Keywords: build,documentation,hatch,help,manpage,manual page,plugin,typing
-Classifier: Development Status :: 4 - Beta
+Keywords: build,documentation,hatch,help,man page,manpage,manual page,plugin,typing
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -80,15 +80,15 @@
 requires = ["hatchling", "hatch-argparse-manpage"]
 build-backend = "hatchling.build"
 ```
 
 ### Generating the manual page
 
 This plugin requires the directories storing the generated man pages are 
-within the project's base directory, and is not equal to the project's base 
+within the project's base directory, and are not equal to the project's base 
 directory.
 
 For example, for a project named `myproject`, and a src layout
 `src/myproject`, an acceptable directory in which to store a
 man page would be `man`.
 
 Using the configuration option `[tool.hatch.build.hooks.argparse-manpage]`,
```

