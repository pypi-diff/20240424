# Comparing `tmp/lmwsip-0.9.7.tar.gz` & `tmp/lmwsip-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmwsip-0.9.7.tar", last modified: Sun Apr  7 21:03:48 2024, max compression
+gzip compressed data, was "lmwsip-0.9.8.tar", last modified: Wed Apr 24 14:10:41 2024, max compression
```

## Comparing `lmwsip-0.9.7.tar` & `lmwsip-0.9.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 21:03:48.644086 lmwsip-0.9.7/
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-07 21:03:44.000000 lmwsip-0.9.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2390 2024-04-07 21:03:48.644086 lmwsip-0.9.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1888 2024-04-07 21:03:44.000000 lmwsip-0.9.7/README.md
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-07 21:03:44.000000 lmwsip-0.9.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      618 2024-04-07 21:03:48.644086 lmwsip-0.9.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-07 21:03:44.000000 lmwsip-0.9.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 21:03:48.641086 lmwsip-0.9.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 21:03:48.643086 lmwsip-0.9.7/src/lmwsip/
--rw-r--r--   0 root         (0) root         (0)    35613 2024-04-07 21:03:44.000000 lmwsip-0.9.7/src/lmwsip/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2462 2024-04-07 21:03:44.000000 lmwsip-0.9.7/src/lmwsip/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 21:03:48.644086 lmwsip-0.9.7/src/lmwsip.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2390 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-07 21:03:48.000000 lmwsip-0.9.7/src/lmwsip.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:10:41.049439 lmwsip-0.9.8/
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-24 14:10:36.000000 lmwsip-0.9.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-24 14:10:41.048439 lmwsip-0.9.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-24 14:10:36.000000 lmwsip-0.9.8/README.md
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-24 14:10:36.000000 lmwsip-0.9.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      618 2024-04-24 14:10:41.050439 lmwsip-0.9.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-24 14:10:36.000000 lmwsip-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:10:41.042439 lmwsip-0.9.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:10:41.046439 lmwsip-0.9.8/src/lmwsip/
+-rw-r--r--   0 root         (0) root         (0)    35619 2024-04-24 14:10:36.000000 lmwsip-0.9.8/src/lmwsip/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2462 2024-04-24 14:10:36.000000 lmwsip-0.9.8/src/lmwsip/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:10:41.048439 lmwsip-0.9.8/src/lmwsip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-04-24 14:10:40.000000 lmwsip-0.9.8/src/lmwsip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-04-24 14:10:41.000000 lmwsip-0.9.8/src/lmwsip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 14:10:40.000000 lmwsip-0.9.8/src/lmwsip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-24 14:10:41.000000 lmwsip-0.9.8/src/lmwsip.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-24 14:10:41.000000 lmwsip-0.9.8/src/lmwsip.egg-info/top_level.txt
```

### Comparing `lmwsip-0.9.7/LICENSE` & `lmwsip-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lmwsip-0.9.7/PKG-INFO` & `lmwsip-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwsip
-Version: 0.9.7
+Version: 0.9.8
 Summary: Interface for the lmw sip protocol
 Home-page: https://git.marceln.org/Werk/lmwsip
 Author: Marcel Nijenhof
 Author-email: pypi@marceln.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lmwsip-0.9.7/README.md` & `lmwsip-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `lmwsip-0.9.7/setup.cfg` & `lmwsip-0.9.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmwsip
-version = 0.9.7
+version = 0.9.8
 author = Marcel Nijenhof
 author_email = pypi@marceln.org
 description = Interface for the lmw sip protocol
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://git.marceln.org/Werk/lmwsip
 classifiers =
```

### Comparing `lmwsip-0.9.7/src/lmwsip/__init__.py` & `lmwsip-0.9.8/src/lmwsip/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -838,15 +838,15 @@
     lmw.cmd("WNT", "HOEK", "H10", "+00:20", "13-08-2018", "16:00", "33/10;35/10")
 
 Returns:
     The LMW answer string
 """
         cmdstr=process + " " + self.meetnet + "," + location + "," + \
                parameter + "," + time_delta + "," + day + "," + \
-               time_of_day + values + "\r" 
+               time_of_day + "," + values + "\r" 
         d = self.sendrecv(cmdstr)
         if (d[0] != '!'):
             raise LmwCmdWarn(cmdstr, d)
         return (d[2:-1])
 
     def valueStr(self, process, location, parameter, day = None,
                     time_of_day = None):
```

### Comparing `lmwsip-0.9.7/src/lmwsip/run.py` & `lmwsip-0.9.8/src/lmwsip/run.py`

 * *Files identical despite different names*

### Comparing `lmwsip-0.9.7/src/lmwsip.egg-info/PKG-INFO` & `lmwsip-0.9.8/src/lmwsip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwsip
-Version: 0.9.7
+Version: 0.9.8
 Summary: Interface for the lmw sip protocol
 Home-page: https://git.marceln.org/Werk/lmwsip
 Author: Marcel Nijenhof
 Author-email: pypi@marceln.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

