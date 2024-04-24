# Comparing `tmp/MediaCurator-0.0.8.tar.gz` & `tmp/MediaCurator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MediaCurator-0.0.8.tar", last modified: Sat Dec  4 09:21:02 2021, max compression
+gzip compressed data, was "MediaCurator-0.0.9.tar", last modified: Sat Aug 20 10:06:49 2022, max compression
```

## Comparing `MediaCurator-0.0.8.tar` & `MediaCurator-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 fabrice   (1000) fabrice   (1000)        0 2021-12-04 09:21:02.173516 MediaCurator-0.0.8/
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)       38 2020-12-16 08:07:17.000000 MediaCurator-0.0.8/MANIFEST.in
-drwxrwxr-x   0 fabrice   (1000) fabrice   (1000)        0 2021-12-04 09:21:02.171516 MediaCurator-0.0.8/MediaCurator.egg-info/
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)     2986 2021-12-04 09:21:01.000000 MediaCurator-0.0.8/MediaCurator.egg-info/PKG-INFO
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)      494 2021-12-04 09:21:02.000000 MediaCurator-0.0.8/MediaCurator.egg-info/SOURCES.txt
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        1 2021-12-04 09:21:01.000000 MediaCurator-0.0.8/MediaCurator.egg-info/dependency_links.txt
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)       65 2021-12-04 09:21:01.000000 MediaCurator-0.0.8/MediaCurator.egg-info/entry_points.txt
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)       17 2021-12-04 09:21:01.000000 MediaCurator-0.0.8/MediaCurator.egg-info/requires.txt
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)       13 2021-12-04 09:21:01.000000 MediaCurator-0.0.8/MediaCurator.egg-info/top_level.txt
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        1 2020-12-16 09:58:34.000000 MediaCurator-0.0.8/MediaCurator.egg-info/zip-safe
--rw-rw-r--   0 fabrice   (1000) fabrice   (1000)     2986 2021-12-04 09:21:02.173516 MediaCurator-0.0.8/PKG-INFO
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)     1589 2020-12-26 17:34:05.000000 MediaCurator-0.0.8/README.md
-drwxrwxr-x   0 fabrice   (1000) fabrice   (1000)        0 2021-12-04 09:21:02.172516 MediaCurator-0.0.8/mediacurator/
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)       26 2020-12-16 07:52:02.000000 MediaCurator-0.0.8/mediacurator/__init__.py
-drwxrwxr-x   0 fabrice   (1000) fabrice   (1000)        0 2021-12-04 09:21:02.172516 MediaCurator-0.0.8/mediacurator/library/
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)       55 2020-11-19 02:17:35.000000 MediaCurator-0.0.8/mediacurator/library/__init__.py
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)     9006 2021-12-04 09:19:45.000000 MediaCurator-0.0.8/mediacurator/library/medialibrary.py
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)     4368 2021-11-15 04:27:05.000000 MediaCurator-0.0.8/mediacurator/library/tools.py
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)    12497 2021-04-20 00:37:29.000000 MediaCurator-0.0.8/mediacurator/library/video.py
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)     7641 2021-04-20 02:13:45.000000 MediaCurator-0.0.8/mediacurator/mediacurator.py
-drwxrwxr-x   0 fabrice   (1000) fabrice   (1000)        0 2021-12-04 09:21:02.172516 MediaCurator-0.0.8/mediacurator/tests/
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)      155 2020-12-16 06:14:56.000000 MediaCurator-0.0.8/mediacurator/tests/__init__.py
--rw-rw-r--   0 fabrice   (1000) fabrice   (1000)       38 2021-12-04 09:21:02.173516 MediaCurator-0.0.8/setup.cfg
--rwxr-xr-x   0 fabrice   (1000) fabrice   (1000)     1645 2021-12-04 09:19:53.000000 MediaCurator-0.0.8/setup.py
+drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2022-08-20 10:06:49.451566 MediaCurator-0.0.9/
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)       38 2020-12-16 08:07:17.000000 MediaCurator-0.0.9/MANIFEST.in
+drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2022-08-20 10:06:49.447566 MediaCurator-0.0.9/MediaCurator.egg-info/
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)     2986 2022-08-20 10:06:49.000000 MediaCurator-0.0.9/MediaCurator.egg-info/PKG-INFO
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)      494 2022-08-20 10:06:49.000000 MediaCurator-0.0.9/MediaCurator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)        1 2022-08-20 10:06:49.000000 MediaCurator-0.0.9/MediaCurator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)       65 2022-08-20 10:06:49.000000 MediaCurator-0.0.9/MediaCurator.egg-info/entry_points.txt
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)       17 2022-08-20 10:06:49.000000 MediaCurator-0.0.9/MediaCurator.egg-info/requires.txt
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)       13 2022-08-20 10:06:49.000000 MediaCurator-0.0.9/MediaCurator.egg-info/top_level.txt
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)        1 2020-12-16 09:58:34.000000 MediaCurator-0.0.9/MediaCurator.egg-info/zip-safe
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)     2986 2022-08-20 10:06:49.447566 MediaCurator-0.0.9/PKG-INFO
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)     1589 2020-12-26 17:34:05.000000 MediaCurator-0.0.9/README.md
+drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2022-08-20 10:06:49.447566 MediaCurator-0.0.9/mediacurator/
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)       26 2020-12-16 07:52:02.000000 MediaCurator-0.0.9/mediacurator/__init__.py
+drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2022-08-20 10:06:49.447566 MediaCurator-0.0.9/mediacurator/library/
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)       55 2020-11-19 02:17:35.000000 MediaCurator-0.0.9/mediacurator/library/__init__.py
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)     9160 2022-08-20 10:01:12.000000 MediaCurator-0.0.9/mediacurator/library/medialibrary.py
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)     4368 2022-08-20 10:02:37.000000 MediaCurator-0.0.9/mediacurator/library/tools.py
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)    12497 2021-04-20 00:37:29.000000 MediaCurator-0.0.9/mediacurator/library/video.py
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)     7641 2021-04-20 02:13:45.000000 MediaCurator-0.0.9/mediacurator/mediacurator.py
+drwxr-xr-x   0 fabrice   (1000) fabrice   (1000)        0 2022-08-20 10:06:49.447566 MediaCurator-0.0.9/mediacurator/tests/
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)      155 2020-12-16 06:14:56.000000 MediaCurator-0.0.9/mediacurator/tests/__init__.py
+-rw-r--r--   0 fabrice   (1000) fabrice   (1000)       38 2022-08-20 10:06:49.451566 MediaCurator-0.0.9/setup.cfg
+-rwxrwxrwx   0 fabrice   (1000) fabrice   (1000)     1645 2022-08-20 10:01:39.000000 MediaCurator-0.0.9/setup.py
```

### Comparing `MediaCurator-0.0.8/MediaCurator.egg-info/PKG-INFO` & `MediaCurator-0.0.9/MediaCurator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MediaCurator
-Version: 0.0.8
+Version: 0.0.9
 Summary: MediaCurator is a Python command line tool to manage a media database.
 Home-page: https://github.com/fabquenneville/MediaCurator
 Author: Fabrice Quenneville
 Author-email: fab@fabq.ca
 License: GPL-3.0
 Download-URL: https://pypi.python.org/pypi/MediaCurator
 Project-URL: Bug Tracker, https://github.com/fabquenneville/MediaCurator/issues
```

### Comparing `MediaCurator-0.0.8/PKG-INFO` & `MediaCurator-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MediaCurator
-Version: 0.0.8
+Version: 0.0.9
 Summary: MediaCurator is a Python command line tool to manage a media database.
 Home-page: https://github.com/fabquenneville/MediaCurator
 Author: Fabrice Quenneville
 Author-email: fab@fabq.ca
 License: GPL-3.0
 Download-URL: https://pypi.python.org/pypi/MediaCurator
 Project-URL: Bug Tracker, https://github.com/fabquenneville/MediaCurator/issues
```

### Comparing `MediaCurator-0.0.8/README.md` & `MediaCurator-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `MediaCurator-0.0.8/mediacurator/library/medialibrary.py` & `MediaCurator-0.0.9/mediacurator/library/medialibrary.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,16 @@
                 videolist += list(path.rglob("*.[vV][iI][dD]"))
             if "vob" in self.inputs or "any" in self.inputs or len(self.inputs) < 1:
                 videolist += list(path.rglob("*.[vV][oO][bB]"))
             if "divx" in self.inputs or "any" in self.inputs or len(self.inputs) < 1:
                 videolist += list(path.rglob("*.[dD][iI][vV][xX]"))
             if "ogm" in self.inputs or "any" in self.inputs or len(self.inputs) < 1:
                 videolist += list(path.rglob("*.[oO][gG][mM]"))
+            if "webm" in self.inputs or "any" in self.inputs or len(self.inputs) < 1:
+                videolist += list(path.rglob("*.[wW][eE][bB][mM]"))
         
         # Remove folders
         videolist_tmp = videolist
         videolist = [video for video in videolist_tmp if video.is_file()]
 
         # Map it all to the videos dictionary as initiated Video objects
         print(f"{colorama.Fore.GREEN}Analazing {len(videolist)} videos in {', '.join(map(str, self.directories))}{colorama.Fore.RESET}")
```

### Comparing `MediaCurator-0.0.8/mediacurator/library/tools.py` & `MediaCurator-0.0.9/mediacurator/library/tools.py`

 * *Files identical despite different names*

### Comparing `MediaCurator-0.0.8/mediacurator/library/video.py` & `MediaCurator-0.0.9/mediacurator/library/video.py`

 * *Files identical despite different names*

### Comparing `MediaCurator-0.0.8/mediacurator/mediacurator.py` & `MediaCurator-0.0.9/mediacurator/mediacurator.py`

 * *Files identical despite different names*

### Comparing `MediaCurator-0.0.8/setup.py` & `MediaCurator-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MediaCurator",
-    version="0.0.8",
+    version="0.0.9",
     author="Fabrice Quenneville",
     author_email="fab@fabq.ca",
     url="https://github.com/fabquenneville/MediaCurator",
     download_url="https://pypi.python.org/pypi/MediaCurator",
     project_urls={
         "Bug Tracker": "https://github.com/fabquenneville/MediaCurator/issues",
         "Documentation": "https://fabquenneville.github.io/MediaCurator/",
```

