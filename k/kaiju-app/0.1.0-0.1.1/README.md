# Comparing `tmp/kaiju_app-0.1.0-py3-none-any.whl.zip` & `tmp/kaiju_app-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17900 bytes, number of entries: 13
--rw-r--r--  2.0 unx      317 b- defN 24-Apr-24 19:13 kaiju_app/__init__.py
--rw-r--r--  2.0 unx    16418 b- defN 24-Apr-24 19:13 kaiju_app/app.py
--rw-r--r--  2.0 unx     1473 b- defN 24-Apr-24 19:13 kaiju_app/bases.py
--rw-r--r--  2.0 unx     4410 b- defN 24-Apr-24 19:13 kaiju_app/configurator.py
--rw-r--r--  2.0 unx      314 b- defN 24-Apr-24 19:13 kaiju_app/interfaces.py
--rw-r--r--  2.0 unx     9992 b- defN 24-Apr-24 19:13 kaiju_app/loader.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 19:13 kaiju_app/py.typed
--rw-r--r--  2.0 unx    11451 b- defN 24-Apr-24 19:13 kaiju_app/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-24 19:23 kaiju_app-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5159 b- defN 24-Apr-24 19:23 kaiju_app-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 19:23 kaiju_app-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Apr-24 19:23 kaiju_app-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1007 b- defN 24-Apr-24 19:23 kaiju_app-0.1.0.dist-info/RECORD
-13 files, 51712 bytes uncompressed, 16236 bytes compressed:  68.6%
+Zip file size: 17898 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      317 b- defN 24-Apr-24 19:38 kaiju_app/__init__.py
+-rw-r--r--  2.0 unx    16418 b- defN 24-Apr-24 19:38 kaiju_app/app.py
+-rw-r--r--  2.0 unx     1473 b- defN 24-Apr-24 19:38 kaiju_app/bases.py
+-rw-r--r--  2.0 unx     4410 b- defN 24-Apr-24 19:38 kaiju_app/configurator.py
+-rw-r--r--  2.0 unx      314 b- defN 24-Apr-24 19:38 kaiju_app/interfaces.py
+-rw-r--r--  2.0 unx     9992 b- defN 24-Apr-24 19:38 kaiju_app/loader.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 19:38 kaiju_app/py.typed
+-rw-r--r--  2.0 unx    11451 b- defN 24-Apr-24 19:38 kaiju_app/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-24 19:38 kaiju_app-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5159 b- defN 24-Apr-24 19:38 kaiju_app-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 19:38 kaiju_app-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-24 19:38 kaiju_app-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1007 b- defN 24-Apr-24 19:38 kaiju_app-0.1.1.dist-info/RECORD
+13 files, 51712 bytes uncompressed, 16234 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: kaiju_app/py.typed
 Comment: 
 
 Filename: kaiju_app/utils.py
 Comment: 
 
-Filename: kaiju_app-0.1.0.dist-info/LICENSE
+Filename: kaiju_app-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_app-0.1.0.dist-info/METADATA
+Filename: kaiju_app-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_app-0.1.0.dist-info/WHEEL
+Filename: kaiju_app-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_app-0.1.0.dist-info/top_level.txt
+Filename: kaiju_app-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_app-0.1.0.dist-info/RECORD
+Filename: kaiju_app-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_app/__init__.py

```diff
@@ -4,8 +4,8 @@
 from kaiju_app.bases import *
 from kaiju_app.configurator import *
 from kaiju_app.loader import *
 
 __python_version__ = "3.12"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "Apache"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `kaiju_app-0.1.0.dist-info/LICENSE` & `kaiju_app-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_app-0.1.0.dist-info/METADATA` & `kaiju_app-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-app
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python modular application and services
 Home-page: https://github.com/violet-black/kaiju-app
 Author: violetblackdev@gmail.com
 License: Apache
 Keywords: application,microservice,asyncio,infrastructure
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `kaiju_app-0.1.0.dist-info/RECORD` & `kaiju_app-0.1.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-kaiju_app/__init__.py,sha256=zFk-OvRsYWq4JM5NhviTOkz_5TX2ZNp5jKbHtwmQHRI,317
+kaiju_app/__init__.py,sha256=FMaImXqWg8oGQFjattfBb7PXizQZvY1Ey1fx3-NAjQ4,317
 kaiju_app/app.py,sha256=7A7yovNokhzJrFN2H66yQ0oq2WxHsVJJqhgWKBFPfiU,16418
 kaiju_app/bases.py,sha256=5I-Icjqe-2MaNV9GseDE0hOHlJPW4tCZkSTLcR0e26k,1473
 kaiju_app/configurator.py,sha256=YnnN3ru-XDAbhU1BaMAdtIse59TCx0yBEpeRUslK6Lw,4410
 kaiju_app/interfaces.py,sha256=Rkz0pDMk_0AUC8MwOSTrq7cbhhCiXQISdpb5CJKIPGw,314
 kaiju_app/loader.py,sha256=zbDOu1QDbacpJgmJ23eo1gzTLz0X6STUCvO0sR3n_9Q,9992
 kaiju_app/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_app/utils.py,sha256=qknmsgrZOowKCfwyCwtaUV__4TxAwD2UHVA74I-oFnw,11451
-kaiju_app-0.1.0.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
-kaiju_app-0.1.0.dist-info/METADATA,sha256=s-0-1w6g4AsKoHOYkj4Q19qzFfh3X9wFZJvFOi7Izd4,5159
-kaiju_app-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-kaiju_app-0.1.0.dist-info/top_level.txt,sha256=oaPejx2Wf_jdrr583PfUJWkCx3c4XqOCJGPVrNTQVbg,10
-kaiju_app-0.1.0.dist-info/RECORD,,
+kaiju_app-0.1.1.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
+kaiju_app-0.1.1.dist-info/METADATA,sha256=Nywlwdq6_G9TFZ018xMCWPM_uAZXCyV_zt74PKgGy1E,5159
+kaiju_app-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+kaiju_app-0.1.1.dist-info/top_level.txt,sha256=oaPejx2Wf_jdrr583PfUJWkCx3c4XqOCJGPVrNTQVbg,10
+kaiju_app-0.1.1.dist-info/RECORD,,
```

