# Comparing `tmp/Catvibes-1.0.8.tar.gz` & `tmp/Catvibes-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Catvibes-1.0.8.tar", last modified: Fri Dec 29 16:05:03 2023, max compression
+gzip compressed data, was "Catvibes-1.0.9.tar", last modified: Fri Dec 29 16:22:38 2023, max compression
```

## Comparing `Catvibes-1.0.8.tar` & `Catvibes-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:05:03.396681 Catvibes-1.0.8/
--rw-r--r--   0 fabian    (1000) fabian    (1000)    35149 2023-12-03 13:32:58.000000 Catvibes-1.0.8/LICENSE
--rw-r--r--   0 fabian    (1000) fabian    (1000)       59 2023-12-21 20:25:09.000000 Catvibes-1.0.8/MANIFEST.in
--rw-r--r--   0 fabian    (1000) fabian    (1000)    42406 2023-12-29 16:05:03.393347 Catvibes-1.0.8/PKG-INFO
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1416 2023-12-21 20:25:09.000000 Catvibes-1.0.8/PyPIREADME.md
--rw-r--r--   0 fabian    (1000) fabian    (1000)     1223 2023-12-22 12:39:49.000000 Catvibes-1.0.8/README.md
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:05:03.390014 Catvibes-1.0.8/images/
--rw-r--r--   0 fabian    (1000) fabian    (1000)   203930 2023-12-21 20:25:09.000000 Catvibes-1.0.8/images/qtui.png
--rw-r--r--   0 fabian    (1000) fabian    (1000)    42570 2023-12-21 20:25:09.000000 Catvibes-1.0.8/images/terminalui.png
--rw-r--r--   0 fabian    (1000) fabian    (1000)   152134 2023-12-21 20:25:09.000000 Catvibes-1.0.8/images/windows.png
--rw-r--r--   0 fabian    (1000) fabian    (1000)      591 2023-12-29 16:04:33.000000 Catvibes-1.0.8/pyproject.toml
--rw-r--r--   0 fabian    (1000) fabian    (1000)       38 2023-12-29 16:05:03.396681 Catvibes-1.0.8/setup.cfg
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:05:03.390014 Catvibes-1.0.8/src/
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:05:03.393347 Catvibes-1.0.8/src/Catvibes.egg-info/
--rw-r--r--   0 fabian    (1000) fabian    (1000)    42406 2023-12-29 16:05:03.000000 Catvibes-1.0.8/src/Catvibes.egg-info/PKG-INFO
--rw-r--r--   0 fabian    (1000) fabian    (1000)      480 2023-12-29 16:05:03.000000 Catvibes-1.0.8/src/Catvibes.egg-info/SOURCES.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)        1 2023-12-29 16:05:03.000000 Catvibes-1.0.8/src/Catvibes.egg-info/dependency_links.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)       52 2023-12-29 16:05:03.000000 Catvibes-1.0.8/src/Catvibes.egg-info/entry_points.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)      113 2023-12-29 16:05:03.000000 Catvibes-1.0.8/src/Catvibes.egg-info/requires.txt
--rw-r--r--   0 fabian    (1000) fabian    (1000)        9 2023-12-29 16:05:03.000000 Catvibes-1.0.8/src/Catvibes.egg-info/top_level.txt
-drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:05:03.393347 Catvibes-1.0.8/src/catvibes/
--rw-r--r--   0 fabian    (1000) fabian    (1000)       37 2023-12-29 16:04:40.000000 Catvibes-1.0.8/src/catvibes/__init__.py
--rw-r--r--   0 fabian    (1000) fabian    (1000)      312 2023-12-21 20:25:09.000000 Catvibes-1.0.8/src/catvibes/__main__.py
--rw-r--r--   0 fabian    (1000) fabian    (1000)     2990 2023-12-21 20:25:09.000000 Catvibes-1.0.8/src/catvibes/catvibes.py
--rw-r--r--   0 fabian    (1000) fabian    (1000)    16923 2023-12-29 16:04:26.000000 Catvibes-1.0.8/src/catvibes/catvibes_lib.py
--rw-r--r--   0 fabian    (1000) fabian    (1000)      190 2023-12-21 20:25:09.000000 Catvibes-1.0.8/src/catvibes/config
--rw-r--r--   0 fabian    (1000) fabian    (1000)    12020 2023-12-25 18:35:19.000000 Catvibes-1.0.8/src/catvibes/qt_gui.py
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:22:38.733403 Catvibes-1.0.9/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    35149 2023-12-03 13:32:58.000000 Catvibes-1.0.9/LICENSE
+-rw-r--r--   0 fabian    (1000) fabian    (1000)       59 2023-12-21 20:25:09.000000 Catvibes-1.0.9/MANIFEST.in
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    42406 2023-12-29 16:22:38.733403 Catvibes-1.0.9/PKG-INFO
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1416 2023-12-21 20:25:09.000000 Catvibes-1.0.9/PyPIREADME.md
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     1223 2023-12-22 12:39:49.000000 Catvibes-1.0.9/README.md
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:22:38.730070 Catvibes-1.0.9/images/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   203930 2023-12-21 20:25:09.000000 Catvibes-1.0.9/images/qtui.png
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    42570 2023-12-21 20:25:09.000000 Catvibes-1.0.9/images/terminalui.png
+-rw-r--r--   0 fabian    (1000) fabian    (1000)   152134 2023-12-21 20:25:09.000000 Catvibes-1.0.9/images/windows.png
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      591 2023-12-29 16:22:12.000000 Catvibes-1.0.9/pyproject.toml
+-rw-r--r--   0 fabian    (1000) fabian    (1000)       38 2023-12-29 16:22:38.733403 Catvibes-1.0.9/setup.cfg
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:22:38.730070 Catvibes-1.0.9/src/
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:22:38.733403 Catvibes-1.0.9/src/Catvibes.egg-info/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    42406 2023-12-29 16:22:38.000000 Catvibes-1.0.9/src/Catvibes.egg-info/PKG-INFO
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      480 2023-12-29 16:22:38.000000 Catvibes-1.0.9/src/Catvibes.egg-info/SOURCES.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)        1 2023-12-29 16:22:38.000000 Catvibes-1.0.9/src/Catvibes.egg-info/dependency_links.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)       52 2023-12-29 16:22:38.000000 Catvibes-1.0.9/src/Catvibes.egg-info/entry_points.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      113 2023-12-29 16:22:38.000000 Catvibes-1.0.9/src/Catvibes.egg-info/requires.txt
+-rw-r--r--   0 fabian    (1000) fabian    (1000)        9 2023-12-29 16:22:38.000000 Catvibes-1.0.9/src/Catvibes.egg-info/top_level.txt
+drwxr-xr-x   0 fabian    (1000) fabian    (1000)        0 2023-12-29 16:22:38.733403 Catvibes-1.0.9/src/catvibes/
+-rw-r--r--   0 fabian    (1000) fabian    (1000)       37 2023-12-29 16:22:16.000000 Catvibes-1.0.9/src/catvibes/__init__.py
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      312 2023-12-21 20:25:09.000000 Catvibes-1.0.9/src/catvibes/__main__.py
+-rw-r--r--   0 fabian    (1000) fabian    (1000)     2990 2023-12-21 20:25:09.000000 Catvibes-1.0.9/src/catvibes/catvibes.py
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    17092 2023-12-29 16:17:10.000000 Catvibes-1.0.9/src/catvibes/catvibes_lib.py
+-rw-r--r--   0 fabian    (1000) fabian    (1000)      190 2023-12-21 20:25:09.000000 Catvibes-1.0.9/src/catvibes/config
+-rw-r--r--   0 fabian    (1000) fabian    (1000)    12020 2023-12-25 18:35:19.000000 Catvibes-1.0.9/src/catvibes/qt_gui.py
```

### Comparing `Catvibes-1.0.8/LICENSE` & `Catvibes-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Catvibes-1.0.8/PKG-INFO` & `Catvibes-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Catvibes
-Version: 1.0.8
+Version: 1.0.9
 Summary: A musicplayer with a terminal and a Qt frontend
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `Catvibes-1.0.8/PyPIREADME.md` & `Catvibes-1.0.9/PyPIREADME.md`

 * *Files identical despite different names*

### Comparing `Catvibes-1.0.8/README.md` & `Catvibes-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Catvibes-1.0.8/images/qtui.png` & `Catvibes-1.0.9/images/qtui.png`

 * *Files identical despite different names*

### Comparing `Catvibes-1.0.8/images/terminalui.png` & `Catvibes-1.0.9/images/terminalui.png`

 * *Files identical despite different names*

### Comparing `Catvibes-1.0.8/images/windows.png` & `Catvibes-1.0.9/images/windows.png`

 * *Files identical despite different names*

### Comparing `Catvibes-1.0.8/pyproject.toml` & `Catvibes-1.0.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Catvibes"
-version = "1.0.8"
+version = "1.0.9"
 description = "A musicplayer with a terminal and a Qt frontend"
 readme = "PyPIREADME.md"
 license = {file = "LICENSE"}
 dependencies = [
     "yt-dlp >= 2023.11.16",
     "ytmusicapi >= 1.3.2",
     "eyed3 >= 0.9.7",
```

### Comparing `Catvibes-1.0.8/src/Catvibes.egg-info/PKG-INFO` & `Catvibes-1.0.9/src/Catvibes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Catvibes
-Version: 1.0.8
+Version: 1.0.9
 Summary: A musicplayer with a terminal and a Qt frontend
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `Catvibes-1.0.8/src/catvibes/catvibes.py` & `Catvibes-1.0.9/src/catvibes/catvibes.py`

 * *Files identical despite different names*

### Comparing `Catvibes-1.0.8/src/catvibes/catvibes_lib.py` & `Catvibes-1.0.9/src/catvibes/catvibes_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import random
 import re
 import shutil
 import signal
 import subprocess as sp
 import time
 from pathlib import Path
+from platform import system
 
 import ytmusicapi
 
 yt = ytmusicapi.YTMusic()
 
 # placeholders for directories
 main_dir: Path
@@ -286,15 +287,18 @@
 
 class MusicPlayerClass:
     """a class for playing files"""
 
     def __init__(self):
         self.playlist: list = []
         self.counter: int = -1
-        self.proc = sp.Popen("ls")
+        if system() == "Linux" or system() == "Darwin":
+            self.proc = sp.Popen("echo")
+        else:
+            self.proc = sp.Popen(["powershell","-Command","ls"])
         self.playing: bool = False
         self.timer = 0
 
     def play(self, file: Path):
         self.proc.kill()
         self.proc = sp.Popen(["ffplay", "-v", "0", "-nodisp", "-autoexit", file])
         self.playing = True
```

### Comparing `Catvibes-1.0.8/src/catvibes/qt_gui.py` & `Catvibes-1.0.9/src/catvibes/qt_gui.py`

 * *Files identical despite different names*

