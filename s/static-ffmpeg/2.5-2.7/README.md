# Comparing `tmp/static_ffmpeg-2.5.tar.gz` & `tmp/static_ffmpeg-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static_ffmpeg-2.5.tar", last modified: Sun Feb 19 22:42:19 2023, max compression
+gzip compressed data, was "static_ffmpeg-2.7.tar", last modified: Wed Apr 24 00:29:44 2024, max compression
```

## Comparing `static_ffmpeg-2.5.tar` & `static_ffmpeg-2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 22:42:19.392073 static_ffmpeg-2.5/
--rw-rw-rw-   0        0        0     1064 2022-09-27 06:03:03.000000 static_ffmpeg-2.5/LICENSE
--rw-rw-rw-   0        0        0       24 2022-09-27 06:03:03.000000 static_ffmpeg-2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5725 2023-02-19 22:42:19.391070 static_ffmpeg-2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4906 2023-02-19 22:41:01.000000 static_ffmpeg-2.5/README.md
--rw-rw-rw-   0        0        0       18 2022-09-27 06:03:03.000000 static_ffmpeg-2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-19 22:42:19.393073 static_ffmpeg-2.5/setup.cfg
--rw-rw-rw-   0        0        0     2737 2023-02-19 22:31:16.000000 static_ffmpeg-2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-19 22:42:19.371074 static_ffmpeg-2.5/static_ffmpeg/
--rw-rw-rw-   0        0        0       49 2023-02-19 22:36:13.000000 static_ffmpeg-2.5/static_ffmpeg/__init__.py
--rw-rw-rw-   0        0        0      724 2023-02-19 22:37:06.000000 static_ffmpeg-2.5/static_ffmpeg/_add_paths.py
--rw-rw-rw-   0        0        0     5512 2023-02-19 22:37:06.000000 static_ffmpeg-2.5/static_ffmpeg/run.py
-drwxrwxrwx   0        0        0        0 2023-02-19 22:42:19.390070 static_ffmpeg-2.5/static_ffmpeg.egg-info/
--rw-rw-rw-   0        0        0     5725 2023-02-19 22:42:19.000000 static_ffmpeg-2.5/static_ffmpeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-02-19 22:42:19.000000 static_ffmpeg-2.5/static_ffmpeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 22:42:19.000000 static_ffmpeg-2.5/static_ffmpeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      183 2023-02-19 22:42:19.000000 static_ffmpeg-2.5/static_ffmpeg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-02-19 22:42:19.000000 static_ffmpeg-2.5/static_ffmpeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-19 22:42:19.000000 static_ffmpeg-2.5/static_ffmpeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 00:29:44.285720 static_ffmpeg-2.7/
+-rw-rw-rw-   0        0        0     1064 2022-09-27 06:03:03.000000 static_ffmpeg-2.7/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-09-27 06:03:03.000000 static_ffmpeg-2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6009 2024-04-24 00:29:44.284719 static_ffmpeg-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5187 2024-04-24 00:27:56.000000 static_ffmpeg-2.7/README.md
+-rw-rw-rw-   0        0        0       18 2022-09-27 06:03:03.000000 static_ffmpeg-2.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 00:29:44.285720 static_ffmpeg-2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2737 2024-04-24 00:28:11.000000 static_ffmpeg-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 00:29:44.265055 static_ffmpeg-2.7/static_ffmpeg/
+-rw-rw-rw-   0        0        0       49 2023-02-19 22:36:13.000000 static_ffmpeg-2.7/static_ffmpeg/__init__.py
+-rw-rw-rw-   0        0        0      804 2024-03-07 06:43:00.000000 static_ffmpeg-2.7/static_ffmpeg/_add_paths.py
+-rw-rw-rw-   0        0        0     5517 2024-04-24 00:28:39.000000 static_ffmpeg-2.7/static_ffmpeg/run.py
+drwxrwxrwx   0        0        0        0 2024-04-24 00:29:44.283737 static_ffmpeg-2.7/static_ffmpeg.egg-info/
+-rw-rw-rw-   0        0        0     6009 2024-04-24 00:29:44.000000 static_ffmpeg-2.7/static_ffmpeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-04-24 00:29:44.000000 static_ffmpeg-2.7/static_ffmpeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 00:29:44.000000 static_ffmpeg-2.7/static_ffmpeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      183 2024-04-24 00:29:44.000000 static_ffmpeg-2.7/static_ffmpeg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-04-24 00:29:44.000000 static_ffmpeg-2.7/static_ffmpeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 00:29:44.000000 static_ffmpeg-2.7/static_ffmpeg.egg-info/top_level.txt
```

### Comparing `static_ffmpeg-2.5/LICENSE` & `static_ffmpeg-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `static_ffmpeg-2.5/PKG-INFO` & `static_ffmpeg-2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static_ffmpeg
-Version: 2.5
+Version: 2.7
 Summary: Cross platform ffmpeg to work on various systems.
 Home-page: https://github.com/zackees/static_ffmpeg
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -21,28 +21,29 @@
 
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_macos.yml)
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/Win_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_win.yml)
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_ubuntu.yml)
 
 # static-ffmpeg
 
-The easiest way to get ffmpeg installed through python.
+The easiest way to get ffmpeg v5 installed through python.
 
 ## Install
 
 ```bash
 > pip install static-ffmpeg
 ```
 
 ## Usage
 
 ```py
 import static_ffmpeg
 # ffmpeg installed on first call to add_paths(), threadsafe.
 static_ffmpeg.add_paths()  # blocks until files are downloaded
+# or static_ffmpeg.add_paths(weak=True) to only add if ffmpeg/ffprobe not already on path
 # Now ffmpeg and ffprobe will use static_ffmpeg versions.
 os.system("ffmpeg -i myfile.mp4 ...")
 ```
 
 Or if you want more lazy behavior to install on first use, or you don't want to modify system paths, use `static_ffmpeg`
 
 
@@ -140,14 +141,16 @@
   * https://github.com/zackees/ffmpeg_bins
 
 ## Version
 
 ffmpeg and ffprobe are both version: 5.0
 
 ## Release History
+  * 2.7: Bugfix, increase the timeout to download for slow connections to 10 minutes.
+  * 2.6: Bugfix, `add_paths(...)` can now be called multiple times without polluting the os env path.
   * 2.5: `add_paths()` now has optional `weak` parameter (default False). If True then `ffmpeg/ffprobe` binaries are only only if either `ffmpeg` OR `ffprobe` doesn't already exist on path
   * 2.3: Adds `static_ffmpeg.add_paths()`
   * 2.2: Addressed [bug 9](https://github.com/zackees/static_ffmpeg/issues/9) in some cases static_ffmpeg couldn't handle spaces in mp4 names.
   * 2.1: Addressed [bug 7](https://github.com/zackees/static_ffmpeg/issues/7) on Win32 for not handling spaces in directory names in the site packages path.
   * 2.0:
     * ffmpeg upgraded to 5.0
     * added ffprobe (static_ffprobe or get run.get_platform_executables_or_raise() to get the binary location)
```

### Comparing `static_ffmpeg-2.5/README.md` & `static_ffmpeg-2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_macos.yml)
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/Win_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_win.yml)
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_ubuntu.yml)
 
 # static-ffmpeg
 
-The easiest way to get ffmpeg installed through python.
+The easiest way to get ffmpeg v5 installed through python.
 
 ## Install
 
 ```bash
 > pip install static-ffmpeg
 ```
 
 ## Usage
 
 ```py
 import static_ffmpeg
 # ffmpeg installed on first call to add_paths(), threadsafe.
 static_ffmpeg.add_paths()  # blocks until files are downloaded
+# or static_ffmpeg.add_paths(weak=True) to only add if ffmpeg/ffprobe not already on path
 # Now ffmpeg and ffprobe will use static_ffmpeg versions.
 os.system("ffmpeg -i myfile.mp4 ...")
 ```
 
 Or if you want more lazy behavior to install on first use, or you don't want to modify system paths, use `static_ffmpeg`
 
 
@@ -120,14 +121,16 @@
   * https://github.com/zackees/ffmpeg_bins
 
 ## Version
 
 ffmpeg and ffprobe are both version: 5.0
 
 ## Release History
+  * 2.7: Bugfix, increase the timeout to download for slow connections to 10 minutes.
+  * 2.6: Bugfix, `add_paths(...)` can now be called multiple times without polluting the os env path.
   * 2.5: `add_paths()` now has optional `weak` parameter (default False). If True then `ffmpeg/ffprobe` binaries are only only if either `ffmpeg` OR `ffprobe` doesn't already exist on path
   * 2.3: Adds `static_ffmpeg.add_paths()`
   * 2.2: Addressed [bug 9](https://github.com/zackees/static_ffmpeg/issues/9) in some cases static_ffmpeg couldn't handle spaces in mp4 names.
   * 2.1: Addressed [bug 7](https://github.com/zackees/static_ffmpeg/issues/7) on Win32 for not handling spaces in directory names in the site packages path.
   * 2.0:
     * ffmpeg upgraded to 5.0
     * added ffprobe (static_ffprobe or get run.get_platform_executables_or_raise() to get the binary location)
```

### Comparing `static_ffmpeg-2.5/setup.py` & `static_ffmpeg-2.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 NAME = "static_ffmpeg"
 DESCRIPTION = "Cross platform ffmpeg to work on various systems."
 URL = "https://github.com/zackees/static_ffmpeg"
 EMAIL = "dont@email.me"
 AUTHOR = "Zach Vorhies"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "2.5"
+VERSION = "2.7"
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fd:
     LONG_DESCRIPTION = fd.read()
 
 with open(os.path.join(HERE, "requirements.txt")) as fd:
     REQUIREMENTS = [line.strip() for line in fd.readlines() if line.strip()]
```

### Comparing `static_ffmpeg-2.5/static_ffmpeg/run.py` & `static_ffmpeg-2.7/static_ffmpeg/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     return os.path.join(SELF_DIR, "bin", sys.platform)
 
 
 def download_file(url, local_path):
     """Downloads a file to the give path."""
     # NOTE the stream=True parameter below
     print(f"Downloading {url} -> {local_path}")
-    with requests.get(url, stream=True, timeout=60) as req:
+    with requests.get(url, stream=True, timeout=TIMEOUT) as req:
         req.raise_for_status()
         with open(local_path, "wb") as file_d:
             for chunk in req.iter_content(chunk_size=8192 * 16):
                 # If you have chunk encoded response uncomment if
                 # and set chunk_size parameter to None.
                 # if chunk:
                 sys.stdout.write(".")
```

### Comparing `static_ffmpeg-2.5/static_ffmpeg.egg-info/PKG-INFO` & `static_ffmpeg-2.7/static_ffmpeg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-ffmpeg
-Version: 2.5
+Version: 2.7
 Summary: Cross platform ffmpeg to work on various systems.
 Home-page: https://github.com/zackees/static_ffmpeg
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
@@ -21,28 +21,29 @@
 
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_macos.yml)
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/Win_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_win.yml)
 [![Actions Status](https://github.com/zackees/static_ffmpeg/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/static_ffmpeg/actions/workflows/push_ubuntu.yml)
 
 # static-ffmpeg
 
-The easiest way to get ffmpeg installed through python.
+The easiest way to get ffmpeg v5 installed through python.
 
 ## Install
 
 ```bash
 > pip install static-ffmpeg
 ```
 
 ## Usage
 
 ```py
 import static_ffmpeg
 # ffmpeg installed on first call to add_paths(), threadsafe.
 static_ffmpeg.add_paths()  # blocks until files are downloaded
+# or static_ffmpeg.add_paths(weak=True) to only add if ffmpeg/ffprobe not already on path
 # Now ffmpeg and ffprobe will use static_ffmpeg versions.
 os.system("ffmpeg -i myfile.mp4 ...")
 ```
 
 Or if you want more lazy behavior to install on first use, or you don't want to modify system paths, use `static_ffmpeg`
 
 
@@ -140,14 +141,16 @@
   * https://github.com/zackees/ffmpeg_bins
 
 ## Version
 
 ffmpeg and ffprobe are both version: 5.0
 
 ## Release History
+  * 2.7: Bugfix, increase the timeout to download for slow connections to 10 minutes.
+  * 2.6: Bugfix, `add_paths(...)` can now be called multiple times without polluting the os env path.
   * 2.5: `add_paths()` now has optional `weak` parameter (default False). If True then `ffmpeg/ffprobe` binaries are only only if either `ffmpeg` OR `ffprobe` doesn't already exist on path
   * 2.3: Adds `static_ffmpeg.add_paths()`
   * 2.2: Addressed [bug 9](https://github.com/zackees/static_ffmpeg/issues/9) in some cases static_ffmpeg couldn't handle spaces in mp4 names.
   * 2.1: Addressed [bug 7](https://github.com/zackees/static_ffmpeg/issues/7) on Win32 for not handling spaces in directory names in the site packages path.
   * 2.0:
     * ffmpeg upgraded to 5.0
     * added ffprobe (static_ffprobe or get run.get_platform_executables_or_raise() to get the binary location)
```

