# Comparing `tmp/sferriol_wamp-0.1.0-py3-none-any.whl.zip` & `tmp/sferriol_wamp-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6639 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 16:49 sferriol/wamp/__init__.py
--rw-r--r--  2.0 unx     6990 b- defN 24-Apr-17 16:32 sferriol/wamp/component.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 16:49 sferriol/wamp/util/__init__.py
--rw-r--r--  2.0 unx     2193 b- defN 24-Apr-17 16:32 sferriol/wamp/util/crossbar.py
--rw-r--r--  2.0 unx     3147 b- defN 24-Apr-17 16:32 sferriol/wamp/util/test.py
--rw-rw-rw-  2.0 unx     1211 b- defN 24-Apr-17 16:49 sferriol_wamp-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      791 b- defN 24-Apr-17 16:49 sferriol_wamp-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 16:49 sferriol_wamp-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-17 16:49 sferriol_wamp-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      830 b- defN 24-Apr-17 16:49 sferriol_wamp-0.1.0.dist-info/RECORD
-10 files, 15263 bytes uncompressed, 5205 bytes compressed:  65.9%
+Zip file size: 6706 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       72 b- defN 24-Apr-24 05:09 sferriol/wamp/__init__.py
+-rw-r--r--  2.0 unx     6954 b- defN 24-Apr-24 05:09 sferriol/wamp/component.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 05:11 sferriol/wamp/util/__init__.py
+-rw-r--r--  2.0 unx     2193 b- defN 24-Apr-24 05:09 sferriol/wamp/util/crossbar.py
+-rw-r--r--  2.0 unx     3147 b- defN 24-Apr-24 05:09 sferriol/wamp/util/test.py
+-rw-rw-rw-  2.0 unx     1211 b- defN 24-Apr-24 05:11 sferriol_wamp-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      782 b- defN 24-Apr-24 05:11 sferriol_wamp-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 05:11 sferriol_wamp-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-24 05:11 sferriol_wamp-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 24-Apr-24 05:11 sferriol_wamp-0.1.1.dist-info/RECORD
+10 files, 15291 bytes uncompressed, 5272 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: sferriol/wamp/util/crossbar.py
 Comment: 
 
 Filename: sferriol/wamp/util/test.py
 Comment: 
 
-Filename: sferriol_wamp-0.1.0.dist-info/LICENSE
+Filename: sferriol_wamp-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: sferriol_wamp-0.1.0.dist-info/METADATA
+Filename: sferriol_wamp-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sferriol_wamp-0.1.0.dist-info/WHEEL
+Filename: sferriol_wamp-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sferriol_wamp-0.1.0.dist-info/top_level.txt
+Filename: sferriol_wamp-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sferriol_wamp-0.1.0.dist-info/RECORD
+Filename: sferriol_wamp-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sferriol/wamp/__init__.py

```diff
@@ -0,0 +1,5 @@
+00000000: 696d 706f 7274 2061 7574 6f62 6168 6e2e  import autobahn.
+00000010: 6173 796e 6369 6f2e 636f 6d70 6f6e 656e  asyncio.componen
+00000020: 740a 0a72 756e 203d 2061 7574 6f62 6168  t..run = autobah
+00000030: 6e2e 6173 796e 6369 6f2e 636f 6d70 6f6e  n.asyncio.compon
+00000040: 656e 742e 7275 6e0a                      ent.run.
```

## sferriol/wamp/component.py

```diff
@@ -211,8 +211,8 @@
                    options=RegisterOptions(force_reregister=True))
     def register__ping():
         return 'pong'
 
     return comp
 
 
-run = autobahn.asyncio.component.run
+
```

## Comparing `sferriol_wamp-0.1.0.dist-info/LICENSE` & `sferriol_wamp-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sferriol_wamp-0.1.0.dist-info/METADATA` & `sferriol_wamp-0.1.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sferriol-wamp
-Version: 0.1.0
+Version: 0.1.1
 Summary: WAMP utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: autobahn ==22.1.1
+Requires-Dist: autobahn
 Requires-Dist: sferriol-python
 Provides-Extra: dev
 Requires-Dist: crossbar ==20.12.3 ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: pytest-doctestplus ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
```

