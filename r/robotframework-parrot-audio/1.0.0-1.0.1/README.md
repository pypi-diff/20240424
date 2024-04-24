# Comparing `tmp/robotframework_parrot_audio-1.0.0.tar.gz` & `tmp/robotframework_parrot_audio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_parrot_audio-1.0.0.tar", last modified: Tue Apr 16 10:31:25 2024, max compression
+gzip compressed data, was "robotframework_parrot_audio-1.0.1.tar", last modified: Wed Apr 24 05:42:44 2024, max compression
```

## Comparing `robotframework_parrot_audio-1.0.0.tar` & `robotframework_parrot_audio-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:31:25.378958 robotframework_parrot_audio-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_audio-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      776 2024-04-16 10:31:25.378958 robotframework_parrot_audio-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      309 2024-04-10 13:00:01.000000 robotframework_parrot_audio-1.0.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:31:25.374958 robotframework_parrot_audio-1.0.0/audio/
--rw-rw-r--   0 user      (1000) user      (1000)     6325 2024-04-10 06:17:16.000000 robotframework_parrot_audio-1.0.0/audio/Audio.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-10 12:56:46.000000 robotframework_parrot_audio-1.0.0/audio/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-10 13:00:14.000000 robotframework_parrot_audio-1.0.0/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:31:25.378958 robotframework_parrot_audio-1.0.0/robotframework_parrot_audio.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      776 2024-04-16 10:31:25.000000 robotframework_parrot_audio-1.0.0/robotframework_parrot_audio.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      329 2024-04-16 10:31:25.000000 robotframework_parrot_audio-1.0.0/robotframework_parrot_audio.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-16 10:31:25.000000 robotframework_parrot_audio-1.0.0/robotframework_parrot_audio.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       29 2024-04-16 10:31:25.000000 robotframework_parrot_audio-1.0.0/robotframework_parrot_audio.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2024-04-16 10:31:25.000000 robotframework_parrot_audio-1.0.0/robotframework_parrot_audio.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      555 2024-04-16 10:31:25.378958 robotframework_parrot_audio-1.0.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:42:44.354580 robotframework_parrot_audio-1.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_audio-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      776 2024-04-24 05:42:44.354580 robotframework_parrot_audio-1.0.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      309 2024-04-10 13:00:01.000000 robotframework_parrot_audio-1.0.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-10 13:00:14.000000 robotframework_parrot_audio-1.0.1/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      595 2024-04-24 05:42:44.354580 robotframework_parrot_audio-1.0.1/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:42:44.354580 robotframework_parrot_audio-1.0.1/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:42:44.354580 robotframework_parrot_audio-1.0.1/src/parrot/
+-rw-rw-r--   0 user      (1000) user      (1000)     6325 2024-04-10 06:17:16.000000 robotframework_parrot_audio-1.0.1/src/parrot/Audio.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-10 12:56:46.000000 robotframework_parrot_audio-1.0.1/src/parrot/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:42:44.354580 robotframework_parrot_audio-1.0.1/src/robotframework_parrot_audio.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      776 2024-04-24 05:42:44.000000 robotframework_parrot_audio-1.0.1/src/robotframework_parrot_audio.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      359 2024-04-24 05:42:44.000000 robotframework_parrot_audio-1.0.1/src/robotframework_parrot_audio.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-24 05:42:44.000000 robotframework_parrot_audio-1.0.1/src/robotframework_parrot_audio.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       29 2024-04-24 05:42:44.000000 robotframework_parrot_audio-1.0.1/src/robotframework_parrot_audio.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-24 05:42:44.000000 robotframework_parrot_audio-1.0.1/src/robotframework_parrot_audio.egg-info/top_level.txt
```

### Comparing `robotframework_parrot_audio-1.0.0/LICENSE` & `robotframework_parrot_audio-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_audio-1.0.0/PKG-INFO` & `robotframework_parrot_audio-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-audio
-Version: 1.0.0
+Version: 1.0.1
 Summary: Audio controller to play, record audio file and convert audio formats
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_audio-1.0.0/audio/Audio.py` & `robotframework_parrot_audio-1.0.1/src/parrot/Audio.py`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_audio-1.0.0/robotframework_parrot_audio.egg-info/PKG-INFO` & `robotframework_parrot_audio-1.0.1/src/robotframework_parrot_audio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-audio
-Version: 1.0.0
+Version: 1.0.1
 Summary: Audio controller to play, record audio file and convert audio formats
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_audio-1.0.0/setup.cfg` & `robotframework_parrot_audio-1.0.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [metadata]
 name = robotframework-parrot-audio
-version = 1.0.0
+version = 1.0.1
 author = Zilogic Systems
 author_email = code@zilogic.com
 description = Audio controller to play, record audio file and convert audio formats
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zilogic-systems/parrot
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 install_requires = 
 	pyaudio
 	pydub
 	robotframework
-packages = find:
+package_dir = 
+	=src
+packages = find_namespace:
 python_requires = >=3.6
-include_package_data = True
+
+[options.packages.find]
+where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

