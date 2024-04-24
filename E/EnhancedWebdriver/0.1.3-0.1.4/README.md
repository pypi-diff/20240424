# Comparing `tmp/EnhancedWebdriver-0.1.3.tar.gz` & `tmp/enhancedwebdriver-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnhancedWebdriver-0.1.3.tar", last modified: Sat Apr 13 12:20:20 2024, max compression
+gzip compressed data, was "enhancedwebdriver-0.1.4.tar", last modified: Wed Apr 24 07:06:14 2024, max compression
```

## Comparing `EnhancedWebdriver-0.1.3.tar` & `enhancedwebdriver-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-13 12:20:20.766434 EnhancedWebdriver-0.1.3/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 EnhancedWebdriver-0.1.3/LICENSE
--rw-r--r--   0 tesla     (1000) tesla     (1000)      622 2024-04-13 12:20:20.766434 EnhancedWebdriver-0.1.3/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 EnhancedWebdriver-0.1.3/pyproject.toml
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      726 2024-04-13 12:20:20.766434 EnhancedWebdriver-0.1.3/setup.cfg
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-13 12:20:20.762434 EnhancedWebdriver-0.1.3/src/
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-13 12:20:20.766434 EnhancedWebdriver-0.1.3/src/EnhancedWebdriver.egg-info/
--rw-r--r--   0 tesla     (1000) tesla     (1000)      622 2024-04-13 12:20:20.000000 EnhancedWebdriver-0.1.3/src/EnhancedWebdriver.egg-info/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      335 2024-04-13 12:20:20.000000 EnhancedWebdriver-0.1.3/src/EnhancedWebdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-13 12:20:20.000000 EnhancedWebdriver-0.1.3/src/EnhancedWebdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       46 2024-04-13 12:20:20.000000 EnhancedWebdriver-0.1.3/src/EnhancedWebdriver.egg-info/requires.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-13 12:20:20.000000 EnhancedWebdriver-0.1.3/src/EnhancedWebdriver.egg-info/top_level.txt
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-13 12:20:20.766434 EnhancedWebdriver-0.1.3/src/enhanced_webdriver/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)    14226 2024-04-13 12:19:19.000000 EnhancedWebdriver-0.1.3/src/enhanced_webdriver/EnhancedWebdriver.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 EnhancedWebdriver-0.1.3/src/enhanced_webdriver/__init__.py
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.4/LICENSE
+-rw-r--r--   0 tesla     (1000) tesla     (1000)     1089 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      465 2024-04-13 15:12:35.000000 enhancedwebdriver-0.1.4/README.md
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.4/pyproject.toml
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      726 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/setup.cfg
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-24 07:06:14.307576 enhancedwebdriver-0.1.4/src/
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/
+-rw-r--r--   0 tesla     (1000) tesla     (1000)     1089 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      345 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       46 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/requires.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-24 07:06:14.000000 enhancedwebdriver-0.1.4/src/EnhancedWebdriver.egg-info/top_level.txt
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-24 07:06:14.311576 enhancedwebdriver-0.1.4/src/enhanced_webdriver/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)    14311 2024-04-24 07:04:55.000000 enhancedwebdriver-0.1.4/src/enhanced_webdriver/EnhancedWebdriver.py
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.4/src/enhanced_webdriver/__init__.py
```

### Comparing `EnhancedWebdriver-0.1.3/LICENSE` & `enhancedwebdriver-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EnhancedWebdriver-0.1.3/setup.cfg` & `enhancedwebdriver-0.1.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EnhancedWebdriver
-version = 0.1.3
+version = 0.1.4
 author = Tesla2000
 author_email = fratajczak124@gmail.com
 description = Extension of webdriver with less boilerplate
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Tesla2000/EnhancedWebdriver
 project_urls =
```

### Comparing `EnhancedWebdriver-0.1.3/src/enhanced_webdriver/EnhancedWebdriver.py` & `enhancedwebdriver-0.1.4/src/enhanced_webdriver/EnhancedWebdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,30 +35,31 @@
 
     """
 
     _driver_name = "driver{}.exe" if "win" in platform.system() else "driver{}"
 
     def __init__(self):
         raise ValueError(
-            "__init__ function of EnhancedWebdriver shouldn't be used use EnhancedWebdriver.create to create driver instance."
+            "__init__ function of EnhancedWebdriver shouldn't be used. Use EnhancedWebdriver.create to create driver instance."
         )
 
     @classmethod
     def create(
         cls,
         web_driver: Optional[WebDriver] = None,
         undetected: bool = False,
-        options: Options = None,
+        options: BaseOptions = None,
         service: Service = None,
         keep_alive: bool = True,
     ) -> "EnhancedWebdriver":
         """
         Create an instance of EnhancedWebDriver.
 
         :param web_driver: An optional instance of WebDriver.[WebDriver], optional
+        :param undetected: Whether to run an instance of UndetectedChromedriver
         :param keep_alive: Whether to configure ChromeRemoteConnection to use HTTP keep-alive
         :param service: Service object for handling the browser driver if you need to pass extra details
         :param options: this takes an instance of ChromeOptions
         :return: An instance of EnhancedWebDriver.
 
         """
         instance = object.__new__(EnhancedWebdriver)
```

