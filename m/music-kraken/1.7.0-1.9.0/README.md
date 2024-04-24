# Comparing `tmp/music_kraken-1.7.0.tar.gz` & `tmp/music_kraken-1.9.0.tar.gz`

## Comparing `music_kraken-1.7.0.tar` & `music_kraken-1.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1790 2020-02-02 00:00:00.000000 music_kraken-1.7.0/music_kraken/__init__.py
--rwxr-xr-x   0        0        0     3996 2020-02-02 00:00:00.000000 music_kraken-1.7.0/music_kraken/__main__.py
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 music_kraken-1.7.0/.gitignore
--rwxr-xr-x   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-1.7.0/LICENSE
--rwxr-xr-x   0        0        0     6533 2020-02-02 00:00:00.000000 music_kraken-1.7.0/README.md
--rwxr-xr-x   0        0        0     1717 2020-02-02 00:00:00.000000 music_kraken-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 music_kraken-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 music_kraken-1.9.0/music_kraken/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 music_kraken-1.9.0/music_kraken/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 music_kraken-1.9.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 music_kraken-1.9.0/LICENSE
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 music_kraken-1.9.0/README.md
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 music_kraken-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 music_kraken-1.9.0/PKG-INFO
```

### Comparing `music_kraken-1.7.0/music_kraken/__init__.py` & `music_kraken-1.9.0/music_kraken/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from rich.logging import RichHandler
 from rich.console import Console
 
 from .utils.shared import DEBUG, DEBUG_LOGGING
 from .utils.config import logging_settings, main_settings, read_config
 
-__version__ = "1.7.0"
+__version__ = "1.9.0"
 
 read_config()
 
 console: Console = Console()
 def init_logging():
     log_file = main_settings['log_file']
```

### Comparing `music_kraken-1.7.0/music_kraken/__main__.py` & `music_kraken-1.9.0/music_kraken/__main__.py`

 * *Files identical despite different names*

### Comparing `music_kraken-1.7.0/LICENSE` & `music_kraken-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `music_kraken-1.7.0/README.md` & `music_kraken-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `music_kraken-1.7.0/pyproject.toml` & `music_kraken-1.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     "mistune~=3.0.2",
     "html2markdown~=0.1.7",
     "jellyfish~=0.9.0",
     "transliterate~=1.10.2",
     "pycountry~=24.0.1",
     
+    "python-dotenv~=1.0.1",
     "tqdm~=4.65.0",
     "platformdirs~=4.2.0",
     "pathvalidate~=2.5.2",
     "toml~=0.10.2",
     "typing_extensions~=4.7.1",
 
     "sponsorblock~=0.1.3",
```

### Comparing `music_kraken-1.7.0/PKG-INFO` & `music_kraken-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: music-kraken
-Version: 1.7.0
+Version: 1.9.0
 Summary: An extensive music downloader crawling the internet. It gets its metadata from a couple of metadata providers, and it scrapes the audiofiles.
 Author-email: Hellow2 <hazel_is_cute@proton.me>
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -21,14 +21,15 @@
 Requires-Dist: html2markdown~=0.1.7
 Requires-Dist: jellyfish~=0.9.0
 Requires-Dist: mistune~=3.0.2
 Requires-Dist: mutagen~=1.46.0
 Requires-Dist: pathvalidate~=2.5.2
 Requires-Dist: platformdirs~=4.2.0
 Requires-Dist: pycountry~=24.0.1
+Requires-Dist: python-dotenv~=1.0.1
 Requires-Dist: requests~=2.31.0
 Requires-Dist: responses~=0.24.1
 Requires-Dist: sponsorblock~=0.1.3
 Requires-Dist: toml~=0.10.2
 Requires-Dist: tqdm~=4.65.0
 Requires-Dist: transliterate~=1.10.2
 Requires-Dist: typing-extensions~=4.7.1
```

