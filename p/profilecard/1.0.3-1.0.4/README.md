# Comparing `tmp/profilecard-1.0.3.tar.gz` & `tmp/profilecard-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profilecard-1.0.3.tar", last modified: Tue Apr 23 18:07:44 2024, max compression
+gzip compressed data, was "profilecard-1.0.4.tar", last modified: Wed Apr 24 08:13:00 2024, max compression
```

## Comparing `profilecard-1.0.3.tar` & `profilecard-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:07:44.276560 profilecard-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 18:07:26.000000 profilecard-1.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-23 18:07:44.276560 profilecard-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-23 18:07:26.000000 profilecard-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:07:44.272560 profilecard-1.0.3/profilecard/
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:07:44.276560 profilecard-1.0.3/profilecard/simple/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/simple/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/simple/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/simple/valmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:07:44.276560 profilecard-1.0.3/profilecard/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/styles/style1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/styles/style2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-23 18:07:26.000000 profilecard-1.0.3/profilecard/styles/style3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:07:44.276560 profilecard-1.0.3/profilecard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-23 18:07:44.000000 profilecard-1.0.3/profilecard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-23 18:07:44.000000 profilecard-1.0.3/profilecard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:07:44.000000 profilecard-1.0.3/profilecard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 18:07:44.000000 profilecard-1.0.3/profilecard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 18:07:44.000000 profilecard-1.0.3/profilecard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:07:44.276560 profilecard-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-23 18:07:26.000000 profilecard-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.262095 profilecard-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 08:12:44.000000 profilecard-1.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-24 08:13:00.262095 profilecard-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-24 08:12:44.000000 profilecard-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.258095 profilecard-1.0.4/profilecard/
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.262095 profilecard-1.0.4/profilecard/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/simple/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/simple/pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/simple/valmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.262095 profilecard-1.0.4/profilecard/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/styles/style1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/styles/style2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-24 08:12:44.000000 profilecard-1.0.4/profilecard/styles/style3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:13:00.262095 profilecard-1.0.4/profilecard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 08:13:00.000000 profilecard-1.0.4/profilecard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:13:00.262095 profilecard-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 08:12:44.000000 profilecard-1.0.4/setup.py
```

### Comparing `profilecard-1.0.3/LICENSE.md` & `profilecard-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.3/PKG-INFO` & `profilecard-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profilecard
-Version: 1.0.3
+Version: 1.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests
 
 # Personal Profile Card Module
 
@@ -115,8 +115,8 @@
 ## Contributing
 
 Contributions are welcome! Please fork the repository and open a pull request with your changes.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.
-```
+
```

### Comparing `profilecard-1.0.3/README.md` & `profilecard-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,8 +107,8 @@
 ## Contributing
 
 Contributions are welcome! Please fork the repository and open a pull request with your changes.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.
-```
+
```

### Comparing `profilecard-1.0.3/profilecard/__init__.py` & `profilecard-1.0.4/profilecard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from .simple import Pack, show
 from .simple import set_val, get_val
 
 
 class Pf:
     """
     This class is use to setup a personal profile card
     """
     def __init__(self, *, first : bool = False):
-        self.style = '1'
+        self.style = "1"
         self.type = None
         self.link = None
         self.pic = None
         self.name = None
         self.stitle = 'About Author'
         self.ctitle = 'About Me'
         self.theme = 'dark'
```

### Comparing `profilecard-1.0.3/profilecard/simple/pack.py` & `profilecard-1.0.4/profilecard/simple/pack.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.3/profilecard/simple/valmanager.py` & `profilecard-1.0.4/profilecard/simple/valmanager.py`

 * *Files 15% similar despite different names*

```diff
@@ -53,7 +53,12 @@
         'badge0': ''
     }
 
     with open(file_name, 'w') as configfile:
         config.write(configfile)
 
     print("Configuration reset to default values.")
+
+
+if __name__ == '__main__':
+    a = "1"
+    set_val(type="Optional", name="style", val=a)
```

### Comparing `profilecard-1.0.3/profilecard/styles/style1.py` & `profilecard-1.0.4/profilecard/styles/style1.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.3/profilecard/styles/style2.py` & `profilecard-1.0.4/profilecard/styles/style2.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.3/profilecard/styles/style3.py` & `profilecard-1.0.4/profilecard/styles/style3.py`

 * *Files identical despite different names*

### Comparing `profilecard-1.0.3/profilecard.egg-info/PKG-INFO` & `profilecard-1.0.4/profilecard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profilecard
-Version: 1.0.3
+Version: 1.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: beautifulsoup4
 Requires-Dist: requests
 
 # Personal Profile Card Module
 
@@ -115,8 +115,8 @@
 ## Contributing
 
 Contributions are welcome! Please fork the repository and open a pull request with your changes.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.
-```
+
```

