# Comparing `tmp/vite_transporter-0.4.1.tar.gz` & `tmp/vite_transporter-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_transporter-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_transporter-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_transporter-0.4.1.tar` & `vite_transporter-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.4.1/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.4.1/LICENSE
--rw-r--r--   0        0        0     4082 2024-04-23 17:32:46.753620 vite_transporter-0.4.1/README.md
--rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.4.1/app_flask_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.4.1/app_flask_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-23 17:26:19.313411 vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    21365 2024-04-23 17:26:19.313250 vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/index-45b871c7.js
--rw-r--r--   0        0        0    33644 2024-04-23 17:26:19.312967 vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/index-cc24c663.css
--rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.4.1/app_quart_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.4.1/app_quart_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.4.1/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.4.1/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.4.1/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.4.1/app_vite_demo/index.css
--rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.4.1/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-04-23 17:26:15.620700 vite_transporter-0.4.1/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.4.1/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.4.1/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.4.1/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.4.1/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0     1257 2024-04-21 15:37:04.537415 vite_transporter-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.4.1/requirements/demos.txt
--rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.4.1/requirements/development.txt
--rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.4.1/requirements/main.txt
--rw-r--r--   0        0        0     2185 2024-04-23 17:33:31.994141 vite_transporter-0.4.1/vite_transporter/__init__.py
--rw-r--r--   0        0        0     2654 2024-04-21 13:26:49.370076 vite_transporter-0.4.1/vite_transporter/_headers.py
--rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.4.1/vite_transporter/_html_tags.py
--rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.4.1/vite_transporter/helpers.py
--rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.4.1/vite_transporter/parser.py
--rw-r--r--   0        0        0      178 2024-04-23 08:21:21.096283 vite_transporter-0.4.1/vite_transporter/platform/__init__.py
--rw-r--r--   0        0        0     4679 2024-04-23 08:25:01.100158 vite_transporter-0.4.1/vite_transporter/platform/flask.py
--rw-r--r--   0        0        0     4743 2024-04-23 08:25:01.103735 vite_transporter-0.4.1/vite_transporter/platform/quart.py
--rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 vite_transporter-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4078 2024-04-23 17:38:10.489230 vite_transporter-0.4.2/README.md
+-rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.4.2/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.4.2/app_flask_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-23 17:26:19.313411 vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    21365 2024-04-23 17:26:19.313250 vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/index-45b871c7.js
+-rw-r--r--   0        0        0    33644 2024-04-23 17:26:19.312967 vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/index-cc24c663.css
+-rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.4.2/app_quart_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.4.2/app_quart_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/index-621914e8.css
+-rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/index-6e585489.js
+-rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.4.2/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.4.2/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.4.2/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.4.2/app_vite_demo/index.css
+-rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.4.2/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-04-23 17:26:15.620700 vite_transporter-0.4.2/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.4.2/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.4.2/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.4.2/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.4.2/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0     1257 2024-04-21 15:37:04.537415 vite_transporter-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.4.2/requirements/demos.txt
+-rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.4.2/requirements/development.txt
+-rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.4.2/requirements/main.txt
+-rw-r--r--   0        0        0     2185 2024-04-23 17:38:19.453468 vite_transporter-0.4.2/vite_transporter/__init__.py
+-rw-r--r--   0        0        0     2654 2024-04-21 13:26:49.370076 vite_transporter-0.4.2/vite_transporter/_headers.py
+-rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.4.2/vite_transporter/_html_tags.py
+-rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.4.2/vite_transporter/helpers.py
+-rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.4.2/vite_transporter/parser.py
+-rw-r--r--   0        0        0      178 2024-04-23 08:21:21.096283 vite_transporter-0.4.2/vite_transporter/platform/__init__.py
+-rw-r--r--   0        0        0     4679 2024-04-23 08:25:01.100158 vite_transporter-0.4.2/vite_transporter/platform/flask.py
+-rw-r--r--   0        0        0     4743 2024-04-23 08:25:01.103735 vite_transporter-0.4.2/vite_transporter/platform/quart.py
+-rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 vite_transporter-0.4.2/PKG-INFO
```

### Comparing `vite_transporter-0.4.1/.gitignore` & `vite_transporter-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/LICENSE` & `vite_transporter-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/README.md` & `vite_transporter-0.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 **Currently compatible with:**
 
 - Flask
 - Quart
 
 **Note (Flask/Quart):** When including credentials in fetch requests in the vite app.
-You must visit the serve app add first to set the credentials.
+You must visit the serve app first to set the credentials.
 
 For example, if the serve app is running on `http://127.0.0.1:5001`, you must visit this address first.
 
 This won't be needed in production, as it's expected that the Vite app will be served from the same domain.
 
 ## How it works
```

### Comparing `vite_transporter-0.4.1/app_flask_demo/__init__.py` & `vite_transporter-0.4.2/app_flask_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/index-45b871c7.js` & `vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/index-45b871c7.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/index-cc24c663.css` & `vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/index-cc24c663.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_quart_demo/__init__.py` & `vite_transporter-0.4.2/app_quart_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/index-621914e8.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/index-6e585489.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_vite_demo/Index.jsx` & `vite_transporter-0.4.2/app_vite_demo/Index.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_vite_demo/__router__.jsx` & `vite_transporter-0.4.2/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_vite_demo/assets/ili.gif` & `vite_transporter-0.4.2/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_vite_demo/index.css` & `vite_transporter-0.4.2/app_vite_demo/index.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_vite_demo/package-lock.json` & `vite_transporter-0.4.2/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/app_vite_demo/package.json` & `vite_transporter-0.4.2/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/pyproject.toml` & `vite_transporter-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/vite_transporter/__init__.py` & `vite_transporter-0.4.2/vite_transporter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from .helpers import Colr as _Colr
 from .helpers import PyProjectConfig as _PyProjectConfig
 from .helpers import _compile
 from .parser import ArgumentParser as _ArgumentParser
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 def _cli():
     pars = _ArgumentParser(prog="vtf", add_help=False)
     pars.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
     )
```

### Comparing `vite_transporter-0.4.1/vite_transporter/_headers.py` & `vite_transporter-0.4.2/vite_transporter/_headers.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/vite_transporter/_html_tags.py` & `vite_transporter-0.4.2/vite_transporter/_html_tags.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/vite_transporter/helpers.py` & `vite_transporter-0.4.2/vite_transporter/helpers.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/vite_transporter/parser.py` & `vite_transporter-0.4.2/vite_transporter/parser.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/vite_transporter/platform/flask.py` & `vite_transporter-0.4.2/vite_transporter/platform/flask.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/vite_transporter/platform/quart.py` & `vite_transporter-0.4.2/vite_transporter/platform/quart.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.1/PKG-INFO` & `vite_transporter-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-transporter
-Version: 0.4.1
+Version: 0.4.2
 Summary: Transport Vite apps.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,15 @@
 
 **Currently compatible with:**
 
 - Flask
 - Quart
 
 **Note (Flask/Quart):** When including credentials in fetch requests in the vite app.
-You must visit the serve app add first to set the credentials.
+You must visit the serve app first to set the credentials.
 
 For example, if the serve app is running on `http://127.0.0.1:5001`, you must visit this address first.
 
 This won't be needed in production, as it's expected that the Vite app will be served from the same domain.
 
 ## How it works
```

