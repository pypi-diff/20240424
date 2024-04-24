# Comparing `tmp/profilecard-1.0.4.tar.gz` & `tmp/profilecard-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profilecard-1.0.4.tar", last modified: Wed Apr 24 08:13:00 2024, max compression
+gzip compressed data, was "profilecard-1.0.6.tar", last modified: Wed Apr 24 08:58:19 2024, max compression
```

## Comparing `profilecard-1.0.4.tar` & `profilecard-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.262095 profilecard-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 08:12:44.000000 profilecard-1.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-24 08:13:00.262095 profilecard-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-24 08:12:44.000000 profilecard-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.258095 profilecard-1.0.4/profilecard/
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.262095 profilecard-1.0.4/profilecard/simple/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/simple/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/simple/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/simple/valmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.262095 profilecard-1.0.4/profilecard/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/styles/style1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/styles/style2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/styles/style3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.262095 profilecard-1.0.4/profilecard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:13:00.262095 profilecard-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 08:12:44.000000 profilecard-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:58:19.370584 profilecard-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 08:58:03.000000 profilecard-1.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-24 08:58:19.370584 profilecard-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-24 08:58:03.000000 profilecard-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:58:19.370584 profilecard-1.0.6/profilecard/
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:58:19.370584 profilecard-1.0.6/profilecard/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/simple/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/simple/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/simple/valmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:58:19.370584 profilecard-1.0.6/profilecard/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/styles/style1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/styles/style2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-24 08:58:03.000000 profilecard-1.0.6/profilecard/styles/style3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:58:19.370584 profilecard-1.0.6/profilecard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-24 08:58:19.000000 profilecard-1.0.6/profilecard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 08:58:19.000000 profilecard-1.0.6/profilecard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:58:19.000000 profilecard-1.0.6/profilecard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 08:58:19.000000 profilecard-1.0.6/profilecard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 08:58:19.000000 profilecard-1.0.6/profilecard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:58:19.370584 profilecard-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 08:58:03.000000 profilecard-1.0.6/setup.py
```

### Comparing `profilecard-1.0.4/LICENSE.md` & `profilecard-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.4/PKG-INFO` & `profilecard-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profilecard
-Version: 1.0.4
+Version: 1.0.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests
 
 # Personal Profile Card Module
```

### Comparing `profilecard-1.0.4/README.md` & `profilecard-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.4/profilecard/__init__.py` & `profilecard-1.0.6/profilecard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.4"
+__version__ = "1.0.6"
 
 from .simple import Pack, show
 from .simple import set_val, get_val
 
 
 class Pf:
     """
```

### Comparing `profilecard-1.0.4/profilecard/simple/pack.py` & `profilecard-1.0.6/profilecard/simple/pack.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.4/profilecard/simple/valmanager.py` & `profilecard-1.0.6/profilecard/simple/valmanager.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.4/profilecard/styles/style1.py` & `profilecard-1.0.6/profilecard/styles/style1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class Style1:
     def __init__(self):
         self.css = '''
                 <!DOCTYPE html>
                 <html lang="zh">
                 <head>
-                    <meta charset="UTF-8">
+                    <meta charset="big-5">
                     <title>{site_title}</title>
                     <style>
                         body {{
                             font-family: Arial, sans-serif;
                             display: flex;
                             justify-content: center;
                             align-items: center;
```

### Comparing `profilecard-1.0.4/profilecard/styles/style2.py` & `profilecard-1.0.6/profilecard/styles/style2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class Style2:
     def __init__(self):
         self.css = '''
                 <!DOCTYPE html>
                 <html lang="zh">
                 <head>
-                    <meta charset="UTF-8">
+                    <meta charset="big-5">
                     <title>{site_title}</title>
                     <style>
                         body {{
                             font-family: 'Helvetica Neue', sans-serif;
                             display: flex;
                             justify-content: center;
                             align-items: center;
```

### Comparing `profilecard-1.0.4/profilecard/styles/style3.py` & `profilecard-1.0.6/profilecard/styles/style3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class Style3:
     def __init__(self):
         self.css = '''
                 <!DOCTYPE html>
                 <html lang="zh">
                 <head>
-                    <meta charset="UTF-8">
+                    <meta charset="big-5">
                     <title>{site_title}</title>
                     <style>
                         body {{
                             font-family: Arial, sans-serif;
                             display: flex;
                             justify-content: center;
                             align-items: center;
```

### Comparing `profilecard-1.0.4/profilecard.egg-info/PKG-INFO` & `profilecard-1.0.6/profilecard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profilecard
-Version: 1.0.4
+Version: 1.0.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests
 
 # Personal Profile Card Module
```

