# Comparing `tmp/hatch_gettext-1.0.0.tar.gz` & `tmp/hatch_gettext-1.1.0.tar.gz`

## Comparing `hatch_gettext-1.0.0.tar` & `hatch_gettext-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/CHANGES.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/__about__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/__init__.py
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/hooks.py
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/py.typed
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0    12048 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/README.md
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    13070 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/CHANGES.md
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/docs/hatch-gettext.3.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/hatch_gettext/__about__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/hatch_gettext/__init__.py
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/hatch_gettext/hooks.py
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/hatch_gettext/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/hatch_gettext/py.typed
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    12044 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/README.md
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13066 2020-02-02 00:00:00.000000 hatch_gettext-1.1.0/PKG-INFO
```

### Comparing `hatch_gettext-1.0.0/CHANGES.md` & `hatch_gettext-1.1.0/CHANGES.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog for Hatch Gettext
 ===========================
 
+1.1.0 (2024-04-24)
+------------------
+
+ - Add manpage markdown source file in `docs` directory, to be generated with 
+   `pandoc`.
+
 1.0.0 (2024-04-12)
 ------------------
 
  - Add options to use `intltool` to regenerate the .pot template, check for 
    left out files, and display a status report.
  - If LINGUAS file or environment variable is specified, only generate mo files
    for languages it specifies.
```

### Comparing `hatch_gettext-1.0.0/hatch_gettext/plugin.py` & `hatch_gettext-1.1.0/hatch_gettext/plugin.py`

 * *Files identical despite different names*

### Comparing `hatch_gettext-1.0.0/.gitignore` & `hatch_gettext-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_gettext-1.0.0/LICENSE.txt` & `hatch_gettext-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_gettext-1.0.0/README.md` & `hatch_gettext-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,16 @@
 ```
 
 ### Translating files using intltool-merge
 
 This plugin allows for but does not mandate translating `.xml` and 
 `.desktop` files using `intltool-merge`. Using 
 `[tool.hatch.build.hooks.gettext.files]`, specify the destination directories
-for the translated files on the left, and arrays of source files on the 
-right. For example:  
+for the translated files using keys, and arrays of source files as values. For 
+example:  
 
 ```toml
 [tool.hatch.build.hooks.gettext.files]
 "share/applications" = ["data/net.myproject.desktop.in"]
 "share/solid/actions" = ["data/kde/net.myproject.desktop.in"]
 "share/metainfo" = ["data/net.myproject.metainfo.xml.in"]
 ```
```

### Comparing `hatch_gettext-1.0.0/pyproject.toml` & `hatch_gettext-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_gettext-1.0.0/PKG-INFO` & `hatch_gettext-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-gettext
-Version: 1.0.0
+Version: 1.1.0
 Summary: Hatch build hook plugin for GNU gettext
 Project-URL: Documentation, https://github.com/damonlynch/hatch-gettext#readme
 Project-URL: Issues, https://github.com/damonlynch/hatch-gettext/issues
 Project-URL: Homepage, https://github.com/damonlynch/hatch-gettext
 Author-email: Damon Lynch <damonlynch@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.txt
@@ -137,16 +137,16 @@
 ```
 
 ### Translating files using intltool-merge
 
 This plugin allows for but does not mandate translating `.xml` and 
 `.desktop` files using `intltool-merge`. Using 
 `[tool.hatch.build.hooks.gettext.files]`, specify the destination directories
-for the translated files on the left, and arrays of source files on the 
-right. For example:  
+for the translated files using keys, and arrays of source files as values. For 
+example:  
 
 ```toml
 [tool.hatch.build.hooks.gettext.files]
 "share/applications" = ["data/net.myproject.desktop.in"]
 "share/solid/actions" = ["data/kde/net.myproject.desktop.in"]
 "share/metainfo" = ["data/net.myproject.metainfo.xml.in"]
 ```
```

