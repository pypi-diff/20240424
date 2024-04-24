# Comparing `tmp/twelvelabs-0.1.21.tar.gz` & `tmp/twelvelabs-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twelvelabs-0.1.21.tar", last modified: Tue Apr  9 04:15:32 2024, max compression
+gzip compressed data, was "twelvelabs-0.1.22.tar", last modified: Wed Apr 24 08:07:45 2024, max compression
```

## Comparing `twelvelabs-0.1.21.tar` & `twelvelabs-0.1.22.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.312616 twelvelabs-0.1.21/
--rw-r--r--   0 zini       (501) staff       (20)    10306 2024-04-09 04:06:21.000000 twelvelabs-0.1.21/LICENSE
--rw-r--r--   0 zini       (501) staff       (20)    14535 2024-04-09 04:15:32.312180 twelvelabs-0.1.21/PKG-INFO
--rw-r--r--   0 zini       (501) staff       (20)    14147 2024-04-09 04:06:21.000000 twelvelabs-0.1.21/README.md
--rw-r--r--   0 zini       (501) staff       (20)       38 2024-04-09 04:15:32.312665 twelvelabs-0.1.21/setup.cfg
--rw-r--r--   0 zini       (501) staff       (20)      700 2024-04-09 04:15:10.000000 twelvelabs-0.1.21/setup.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.307667 twelvelabs-0.1.21/twelvelabs/
--rw-r--r--   0 zini       (501) staff       (20)      768 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/__init__.py
--rw-r--r--   0 zini       (501) staff       (20)     3955 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/base_client.py
--rw-r--r--   0 zini       (501) staff       (20)     1371 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/client.py
--rw-r--r--   0 zini       (501) staff       (20)      313 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/constants.py
--rw-r--r--   0 zini       (501) staff       (20)     2069 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/exceptions.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.310010 twelvelabs-0.1.21/twelvelabs/models/
--rw-r--r--   0 zini       (501) staff       (20)     1034 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/models/__init__.py
--rw-r--r--   0 zini       (501) staff       (20)      459 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/models/_base.py
--rw-r--r--   0 zini       (501) staff       (20)      164 2024-04-09 04:06:21.000000 twelvelabs-0.1.21/twelvelabs/models/engine.py
--rw-r--r--   0 zini       (501) staff       (20)      782 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/models/generate.py
--rw-r--r--   0 zini       (501) staff       (20)     7060 2024-03-07 05:18:58.000000 twelvelabs-0.1.21/twelvelabs/models/index.py
--rw-r--r--   0 zini       (501) staff       (20)     2066 2024-03-07 07:44:40.000000 twelvelabs-0.1.21/twelvelabs/models/search.py
--rw-r--r--   0 zini       (501) staff       (20)     2888 2024-04-09 04:06:21.000000 twelvelabs-0.1.21/twelvelabs/models/task.py
--rw-r--r--   0 zini       (501) staff       (20)     4408 2024-04-09 04:15:10.000000 twelvelabs-0.1.21/twelvelabs/models/video.py
--rw-r--r--   0 zini       (501) staff       (20)      505 2024-03-04 08:47:21.000000 twelvelabs-0.1.21/twelvelabs/resource.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.311342 twelvelabs-0.1.21/twelvelabs/resources/
--rw-r--r--   0 zini       (501) staff       (20)      228 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/resources/__init__.py
--rw-r--r--   0 zini       (501) staff       (20)      424 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/resources/engine.py
--rw-r--r--   0 zini       (501) staff       (20)     1551 2024-03-07 05:51:31.000000 twelvelabs-0.1.21/twelvelabs/resources/generate.py
--rw-r--r--   0 zini       (501) staff       (20)     4737 2024-03-07 05:40:16.000000 twelvelabs-0.1.21/twelvelabs/resources/index.py
--rw-r--r--   0 zini       (501) staff       (20)     2671 2024-02-24 15:37:49.000000 twelvelabs-0.1.21/twelvelabs/resources/search.py
--rw-r--r--   0 zini       (501) staff       (20)     7379 2024-03-07 05:51:31.000000 twelvelabs-0.1.21/twelvelabs/resources/task.py
--rw-r--r--   0 zini       (501) staff       (20)     7646 2024-03-07 07:39:37.000000 twelvelabs-0.1.21/twelvelabs/resources/video.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.311719 twelvelabs-0.1.21/twelvelabs/types/
--rw-r--r--   0 zini       (501) staff       (20)       58 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/types/__init__.py
--rw-r--r--   0 zini       (501) staff       (20)      104 2024-02-02 15:17:34.000000 twelvelabs-0.1.21/twelvelabs/types/index.py
--rw-r--r--   0 zini       (501) staff       (20)      885 2024-03-07 07:39:37.000000 twelvelabs-0.1.21/twelvelabs/util.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-09 04:15:32.311919 twelvelabs-0.1.21/twelvelabs.egg-info/
--rw-r--r--   0 zini       (501) staff       (20)    14535 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/PKG-INFO
--rw-r--r--   0 zini       (501) staff       (20)      851 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/SOURCES.txt
--rw-r--r--   0 zini       (501) staff       (20)        1 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/dependency_links.txt
--rw-r--r--   0 zini       (501) staff       (20)       30 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/requires.txt
--rw-r--r--   0 zini       (501) staff       (20)       11 2024-04-09 04:15:32.000000 twelvelabs-0.1.21/twelvelabs.egg-info/top_level.txt
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.642258 twelvelabs-0.1.22/
+-rw-r--r--   0 zini       (501) staff       (20)    10306 2024-04-09 04:06:21.000000 twelvelabs-0.1.22/LICENSE
+-rw-r--r--   0 zini       (501) staff       (20)    14535 2024-04-24 08:07:45.641589 twelvelabs-0.1.22/PKG-INFO
+-rw-r--r--   0 zini       (501) staff       (20)    14147 2024-04-09 04:06:21.000000 twelvelabs-0.1.22/README.md
+-rw-r--r--   0 zini       (501) staff       (20)       38 2024-04-24 08:07:45.642308 twelvelabs-0.1.22/setup.cfg
+-rw-r--r--   0 zini       (501) staff       (20)      700 2024-04-24 08:07:20.000000 twelvelabs-0.1.22/setup.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.636607 twelvelabs-0.1.22/twelvelabs/
+-rw-r--r--   0 zini       (501) staff       (20)      768 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/__init__.py
+-rw-r--r--   0 zini       (501) staff       (20)     3955 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/base_client.py
+-rw-r--r--   0 zini       (501) staff       (20)     1371 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/client.py
+-rw-r--r--   0 zini       (501) staff       (20)      313 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/constants.py
+-rw-r--r--   0 zini       (501) staff       (20)     2069 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/exceptions.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.638799 twelvelabs-0.1.22/twelvelabs/models/
+-rw-r--r--   0 zini       (501) staff       (20)     1034 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/models/__init__.py
+-rw-r--r--   0 zini       (501) staff       (20)      459 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/models/_base.py
+-rw-r--r--   0 zini       (501) staff       (20)      164 2024-04-09 04:06:21.000000 twelvelabs-0.1.22/twelvelabs/models/engine.py
+-rw-r--r--   0 zini       (501) staff       (20)      782 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/models/generate.py
+-rw-r--r--   0 zini       (501) staff       (20)     7060 2024-03-07 05:18:58.000000 twelvelabs-0.1.22/twelvelabs/models/index.py
+-rw-r--r--   0 zini       (501) staff       (20)     2066 2024-03-07 07:44:40.000000 twelvelabs-0.1.22/twelvelabs/models/search.py
+-rw-r--r--   0 zini       (501) staff       (20)     2888 2024-04-09 04:06:21.000000 twelvelabs-0.1.22/twelvelabs/models/task.py
+-rw-r--r--   0 zini       (501) staff       (20)     4408 2024-04-09 04:15:10.000000 twelvelabs-0.1.22/twelvelabs/models/video.py
+-rw-r--r--   0 zini       (501) staff       (20)      505 2024-03-04 08:47:21.000000 twelvelabs-0.1.22/twelvelabs/resource.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.640358 twelvelabs-0.1.22/twelvelabs/resources/
+-rw-r--r--   0 zini       (501) staff       (20)      228 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/resources/__init__.py
+-rw-r--r--   0 zini       (501) staff       (20)      424 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/resources/engine.py
+-rw-r--r--   0 zini       (501) staff       (20)     1551 2024-03-07 05:51:31.000000 twelvelabs-0.1.22/twelvelabs/resources/generate.py
+-rw-r--r--   0 zini       (501) staff       (20)     4737 2024-03-07 05:40:16.000000 twelvelabs-0.1.22/twelvelabs/resources/index.py
+-rw-r--r--   0 zini       (501) staff       (20)     2671 2024-02-24 15:37:49.000000 twelvelabs-0.1.22/twelvelabs/resources/search.py
+-rw-r--r--   0 zini       (501) staff       (20)     7380 2024-04-24 08:05:51.000000 twelvelabs-0.1.22/twelvelabs/resources/task.py
+-rw-r--r--   0 zini       (501) staff       (20)     7646 2024-03-07 07:39:37.000000 twelvelabs-0.1.22/twelvelabs/resources/video.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.640958 twelvelabs-0.1.22/twelvelabs/types/
+-rw-r--r--   0 zini       (501) staff       (20)       58 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/types/__init__.py
+-rw-r--r--   0 zini       (501) staff       (20)      104 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/types/index.py
+-rw-r--r--   0 zini       (501) staff       (20)      885 2024-03-07 07:39:37.000000 twelvelabs-0.1.22/twelvelabs/util.py
+drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.641212 twelvelabs-0.1.22/twelvelabs.egg-info/
+-rw-r--r--   0 zini       (501) staff       (20)    14535 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/PKG-INFO
+-rw-r--r--   0 zini       (501) staff       (20)      851 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/SOURCES.txt
+-rw-r--r--   0 zini       (501) staff       (20)        1 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/dependency_links.txt
+-rw-r--r--   0 zini       (501) staff       (20)       30 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/requires.txt
+-rw-r--r--   0 zini       (501) staff       (20)       11 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/top_level.txt
```

### Comparing `twelvelabs-0.1.21/LICENSE` & `twelvelabs-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/PKG-INFO` & `twelvelabs-0.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.21
+Version: 0.1.22
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twelvelabs-0.1.21/README.md` & `twelvelabs-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/setup.py` & `twelvelabs-0.1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="twelvelabs",
-    version="0.1.21",
+    version="0.1.22",
     author="Twelve Labs",
     description="SDK for Twelve Labs API",
     url="https://github.com/twelvelabs-io/twelvelabs-python",
     packages=find_packages(),
     install_requires=required,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `twelvelabs-0.1.21/twelvelabs/__init__.py` & `twelvelabs-0.1.22/twelvelabs/__init__.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/base_client.py` & `twelvelabs-0.1.22/twelvelabs/base_client.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/client.py` & `twelvelabs-0.1.22/twelvelabs/client.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/exceptions.py` & `twelvelabs-0.1.22/twelvelabs/exceptions.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/models/__init__.py` & `twelvelabs-0.1.22/twelvelabs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/models/generate.py` & `twelvelabs-0.1.22/twelvelabs/models/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/models/index.py` & `twelvelabs-0.1.22/twelvelabs/models/index.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/models/search.py` & `twelvelabs-0.1.22/twelvelabs/models/search.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/models/task.py` & `twelvelabs-0.1.22/twelvelabs/models/task.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/models/video.py` & `twelvelabs-0.1.22/twelvelabs/models/video.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/resources/generate.py` & `twelvelabs-0.1.22/twelvelabs/resources/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/resources/index.py` & `twelvelabs-0.1.22/twelvelabs/resources/index.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/resources/search.py` & `twelvelabs-0.1.22/twelvelabs/resources/search.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/resources/task.py` & `twelvelabs-0.1.22/twelvelabs/resources/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         if not file and not url:
             raise ValueError("Either file or url must be provided")
         data = {
             "index_id": index_id,
             "video_url": url,
             "transcription_url": transcription_url,
             "language": language,
-            "disable_video_tream": disable_video_stream,
+            "disable_video_stream": disable_video_stream,
         }
 
         files = {}
         opened_files: List[BinaryIO] = []
         # TODO validate video supported (ffmpeg)
         if file is not None:
             if isinstance(file, str):
```

### Comparing `twelvelabs-0.1.21/twelvelabs/resources/video.py` & `twelvelabs-0.1.22/twelvelabs/resources/video.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs/util.py` & `twelvelabs-0.1.22/twelvelabs/util.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.21/twelvelabs.egg-info/PKG-INFO` & `twelvelabs-0.1.22/twelvelabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.21
+Version: 0.1.22
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twelvelabs-0.1.21/twelvelabs.egg-info/SOURCES.txt` & `twelvelabs-0.1.22/twelvelabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

