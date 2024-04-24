# Comparing `tmp/kungfupanda-0.24.tar.gz` & `tmp/kungfupanda-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kungfupanda-0.24.tar", last modified: Wed Apr 24 09:37:17 2024, max compression
+gzip compressed data, was "kungfupanda-0.25.tar", last modified: Wed Apr 24 10:48:38 2024, max compression
```

## Comparing `kungfupanda-0.24.tar` & `kungfupanda-0.25.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:37:17.547762 kungfupanda-0.24/
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       36 2024-04-24 08:31:59.000000 kungfupanda-0.24/MANIFEST.in
--rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      522 2024-04-24 09:37:17.547762 kungfupanda-0.24/PKG-INFO
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:37:17.543762 kungfupanda-0.24/kungfupanda/
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)     1649 2024-04-24 09:35:15.000000 kungfupanda-0.24/kungfupanda/__init__.py
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)    15325 2024-04-24 09:17:38.000000 kungfupanda-0.24/kungfupanda/kungfupanda.py
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:37:17.543762 kungfupanda-0.24/kungfupanda/resources/
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)  1974158 2024-04-23 19:03:43.000000 kungfupanda-0.24/kungfupanda/resources/gif_1.gif
-drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 09:37:17.547762 kungfupanda-0.24/kungfupanda.egg-info/
--rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      522 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/PKG-INFO
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      277 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/SOURCES.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)        1 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/dependency_links.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       21 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/requires.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       12 2024-04-24 09:37:17.000000 kungfupanda-0.24/kungfupanda.egg-info/top_level.txt
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-24 09:37:17.547762 kungfupanda-0.24/setup.cfg
--rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      702 2024-04-24 09:37:10.000000 kungfupanda-0.24/setup.py
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 10:48:38.845718 kungfupanda-0.25/
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       36 2024-04-24 08:31:59.000000 kungfupanda-0.25/MANIFEST.in
+-rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      522 2024-04-24 10:48:38.845718 kungfupanda-0.25/PKG-INFO
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 10:48:38.841720 kungfupanda-0.25/kungfupanda/
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)     1632 2024-04-24 10:48:24.000000 kungfupanda-0.25/kungfupanda/__init__.py
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)    14611 2024-04-24 10:48:17.000000 kungfupanda-0.25/kungfupanda/kungfupanda.py
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 10:48:38.841720 kungfupanda-0.25/kungfupanda/resources/
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)  1974158 2024-04-23 19:03:43.000000 kungfupanda-0.25/kungfupanda/resources/gif_1.gif
+drwxrwxr-x   0 shtlp_0018  (1000) shtlp_0018  (1000)        0 2024-04-24 10:48:38.845718 kungfupanda-0.25/kungfupanda.egg-info/
+-rw-r--r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      522 2024-04-24 10:48:38.000000 kungfupanda-0.25/kungfupanda.egg-info/PKG-INFO
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      277 2024-04-24 10:48:38.000000 kungfupanda-0.25/kungfupanda.egg-info/SOURCES.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)        1 2024-04-24 10:48:38.000000 kungfupanda-0.25/kungfupanda.egg-info/dependency_links.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       21 2024-04-24 10:48:38.000000 kungfupanda-0.25/kungfupanda.egg-info/requires.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       12 2024-04-24 10:48:38.000000 kungfupanda-0.25/kungfupanda.egg-info/top_level.txt
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)       38 2024-04-24 10:48:38.845718 kungfupanda-0.25/setup.cfg
+-rw-rw-r--   0 shtlp_0018  (1000) shtlp_0018  (1000)      702 2024-04-24 10:48:34.000000 kungfupanda-0.25/setup.py
```

### Comparing `kungfupanda-0.24/PKG-INFO` & `kungfupanda-0.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kungfupanda
-Version: 0.24
+Version: 0.25
 Summary: A simple package to make everything easy for programmers to do everything the cool way
 Home-page: 
 Author: The Big Fat Panda
 Author-email: po_the_big_fat_panda@gmail.com
 Requires-Dist: pandas
 Requires-Dist: opencv-python
```

### Comparing `kungfupanda-0.24/kungfupanda/__init__.py` & `kungfupanda-0.25/kungfupanda/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from kungfupanda import who_is_dragon_warrior,wuxi_finger_hold
+from kungfupanda import who_is_dragon_warrior
 from pandas import *
 
 
 print(r"""
 __          __  _                            _          _   _          
 \ \        / / | |                          | |        | | | |         
  \ \  /\  / /__| | ___ ___  _ __ ___   ___  | |_ ___   | |_| |__   ___
```

### Comparing `kungfupanda-0.24/kungfupanda/kungfupanda.py` & `kungfupanda-0.25/kungfupanda/kungfupanda.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,10 @@
 from pandas import *
 import cv2
 
-def wuxi_finger_hold():
-    # Open the GIF file
-    gif_path = "kungfupanda/resources/gif_1.gif"  # Replace with your actual GIF path
-    cap = cv2.VideoCapture(gif_path)
-
-    # Check if video capture was successful
-    if not cap.isOpened():
-        print("Error opening video capture")
-        exit()
-
-    # Loop through each frame of the GIF
-    while True:
-        ret, frame = cap.read()
-        if not ret:
-            print("Reached the end of the GIF")
-            break
-
-        # Display the frame
-        cv2.imshow("Kung Fu Panda GIF", frame)
-        # Exit on 'q' press
-        if cv2.waitKey(60) == ord("q"):
-            break
-
-    # Release resources
-    cap.release()
-    cv2.destroyAllWindows()
-
-
 def who_is_dragon_warrior():
    print("""
 *********************++++***++++++**++++++**++++++++++++++++++++++*+++++++++++++++++++++++++++++++++++++++++++++++++++++
 *********************++*++**+++++++**+++++*++++++++++++++*++++++++*+++++++++++++++++++++++++++++++++++++++++++++++++++++
 *****************************+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 ******************************+***+++++++++++++++++*++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 ***********************************+++**+++++++++++*++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
```

### Comparing `kungfupanda-0.24/kungfupanda/resources/gif_1.gif` & `kungfupanda-0.25/kungfupanda/resources/gif_1.gif`

 * *Files identical despite different names*

### Comparing `kungfupanda-0.24/kungfupanda.egg-info/PKG-INFO` & `kungfupanda-0.25/kungfupanda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kungfupanda
-Version: 0.24
+Version: 0.25
 Summary: A simple package to make everything easy for programmers to do everything the cool way
 Home-page: 
 Author: The Big Fat Panda
 Author-email: po_the_big_fat_panda@gmail.com
 Requires-Dist: pandas
 Requires-Dist: opencv-python
```

### Comparing `kungfupanda-0.24/setup.py` & `kungfupanda-0.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kungfupanda',
-    version='0.24',
+    version='0.25',
     author='The Big Fat Panda',
     author_email='po_the_big_fat_panda@gmail.com',
     description="A simple package to make everything easy for programmers to do everything the cool way",
     long_description="""A simple package for people who are not bound by societal rules, made by a cute panda trained to be a dragon warrior. For the full story, watch the original trilogy:
     - Kung Fu Panda 1
     - Kung Fu Panda 2
     - Kung Fu Panda 3
```

