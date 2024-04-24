# Comparing `tmp/CHJ-3.8-py2.py3-none-any.whl.zip` & `tmp/CHJ-3.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 38010 bytes, number of entries: 25
+Zip file size: 38021 bytes, number of entries: 25
 -rw-rw-r--  2.0 unx     1488 b- defN 16-Oct-12 17:21 _CHJ/LICENSE
 -rw-rw-r--  2.0 unx    16398 b- defN 22-Jul-02 15:02 _CHJ/Media.py
 -rw-rw-r--  2.0 unx    14655 b- defN 22-Jul-02 15:02 _CHJ/Parameters.py
 -rw-rw-r--  2.0 unx      449 b- defN 22-Jul-02 15:50 _CHJ/README.rst
--rw-rw-r--  2.0 unx       62 b- defN 23-May-29 18:58 _CHJ/VERSION.py
+-rw-rw-r--  2.0 unx       62 b- defN 24-Apr-24 16:03 _CHJ/VERSION.py
 -rw-rw-r--  2.0 unx      809 b- defN 22-Jul-02 15:02 _CHJ/__init__.py
 -rw-rw-r--  2.0 unx       26 b- defN 16-Oct-12 17:21 _CHJ/setup.cfg
--rw-rw-r--  2.0 unx     3174 b- defN 23-May-29 18:38 _CHJ/setup.py
+-rw-rw-r--  2.0 unx     3230 b- defN 24-Apr-24 15:45 _CHJ/setup.py
 -rw-rw-r--  2.0 unx     4673 b- defN 22-Jul-02 15:02 _CHJ/_CSS/CS.py
 -rw-rw-r--  2.0 unx     4339 b- defN 22-Jul-02 15:02 _CHJ/_CSS/Calc.py
 -rw-rw-r--  2.0 unx     6014 b- defN 22-Jul-02 15:02 _CHJ/_CSS/Color.py
 -rw-rw-r--  2.0 unx    13618 b- defN 22-Jul-02 15:02 _CHJ/_CSS/Length.py
 -rw-rw-r--  2.0 unx    10544 b- defN 22-Jul-02 15:02 _CHJ/_CSS/Media.py
 -rw-rw-r--  2.0 unx     8218 b- defN 22-Jul-02 15:02 _CHJ/_CSS/Property.py
 -rw-rw-r--  2.0 unx     9356 b- defN 22-Jul-02 15:02 _CHJ/_CSS/Rule.py
 -rw-rw-r--  2.0 unx    12539 b- defN 22-Jul-02 15:02 _CHJ/_CSS/Shape.py
 -rw-rw-r--  2.0 unx     4007 b- defN 22-Jul-02 15:02 _CHJ/_CSS/Style_Sheet.py
 -rw-rw-r--  2.0 unx     2575 b- defN 22-Jul-02 15:02 _CHJ/_CSS/_TRBL_.py
 -rw-rw-r--  2.0 unx      896 b- defN 22-Jul-02 15:02 _CHJ/_CSS/__init__.py
 -rw-rw-r--  2.0 unx     1361 b- defN 22-Jul-02 15:02 _CHJ/_CSS/import_CSS.py
--rw-rw-r--  2.0 unx     1488 b- defN 23-May-29 18:58 CHJ-3.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1445 b- defN 23-May-29 18:58 CHJ-3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-29 18:58 CHJ-3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-May-29 18:58 CHJ-3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1840 b- defN 23-May-29 18:58 CHJ-3.8.dist-info/RECORD
-25 files, 120089 bytes uncompressed, 35138 bytes compressed:  70.7%
+-rw-rw-r--  2.0 unx     1488 b- defN 24-Apr-24 16:03 CHJ-3.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1445 b- defN 24-Apr-24 16:03 CHJ-3.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-24 16:03 CHJ-3.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 24-Apr-24 16:03 CHJ-3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1840 b- defN 24-Apr-24 16:03 CHJ-3.9.dist-info/RECORD
+25 files, 120145 bytes uncompressed, 35149 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: _CHJ/_CSS/__init__.py
 Comment: 
 
 Filename: _CHJ/_CSS/import_CSS.py
 Comment: 
 
-Filename: CHJ-3.8.dist-info/LICENSE
+Filename: CHJ-3.9.dist-info/LICENSE
 Comment: 
 
-Filename: CHJ-3.8.dist-info/METADATA
+Filename: CHJ-3.9.dist-info/METADATA
 Comment: 
 
-Filename: CHJ-3.8.dist-info/WHEEL
+Filename: CHJ-3.9.dist-info/WHEEL
 Comment: 
 
-Filename: CHJ-3.8.dist-info/top_level.txt
+Filename: CHJ-3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: CHJ-3.8.dist-info/RECORD
+Filename: CHJ-3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## _CHJ/VERSION.py

```diff
@@ -1,2 +1,2 @@
-__date__    = "2023-05-29T19:42:12+01:00"
-__version__ = "3.8"
+__date__    = "2024-04-24T16:45:19+01:00"
+__version__ = "3.9"
```

## _CHJ/setup.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# Copyright (C) 2016-2023 Christian Tanzer. All rights reserved
+# Copyright (C) 2016-2024 Christian Tanzer. All rights reserved
 # tanzer@gg32.com                                      https://www.gg32.com
 # Web: https://www.gg32.com/en/ Email: tanzer@swing.co.at
 # All rights reserved
 # ****************************************************************************
 # This module is licensed under the terms of the BSD 3-Clause License
 # <https://www.gg32.com/license/bsd_3c.html>.
 # ****************************************************************************
@@ -19,14 +19,15 @@
 # Revision Dates
 #    11-Oct-2016 (CT) Creation
 #    13-Oct-2016 (CT) Use `find_packages`, `_TFL.fs_find`, not home-grown code
 #    22-Feb-2017 (CT) Use `TFL_STP`, not home-grown code
 #    27-Feb-2017 (CT) Add Python 3.6 to `classifiers`
 #    25-Mar-2020 (CT) Restrict Python versions to >=3.7
 #    29-May-2023 (CT) Restrict Python versions to >=3.8
+#    24-Apr-2024 (CT) Restrict Python versions to >=3.9
 #    ««revision-date»»···
 #--
 
 from   setuptools               import setup
 
 import TFL_STP as STP
 
@@ -61,15 +62,15 @@
         , "Operating System :: OS Independent"
         , "Programming Language :: Python"
         , "Intended Audience :: Developers"
         , "Topic :: Internet :: WWW/HTTP :: Dynamic Content"
         , "Topic :: Software Development :: Libraries :: Python Modules"
         , "Topic :: Text Processing :: Markup :: HTML"
         ]
-    , python_requires      = ">=3.8"
+    , python_requires      = ">=3.9"
     , setup_requires       = ["TFL_STP>=3"]
     , install_requires     = ["TFL>=3"]
     , extras_require       = dict
         ( minified             = ["rcssmin", "rjsmin"]
         , minified_debian_slow = ["cssmin",  "jsmin"]
             ### cssmin and jsmin are available as debian packages but almost an
             ### order of magnitude slower than rcssmin and rjsmin
```

## Comparing `CHJ-3.8.dist-info/LICENSE` & `CHJ-3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `CHJ-3.8.dist-info/METADATA` & `CHJ-3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: CHJ
-Version: 3.8
+Version: 3.9
 Summary: Package for CSS/HTML/Javascript support.
 Home-page: https://codeberg.org/tanzer/tapyr
 Author: Christian Tanzer
 Author-email: tanzer@swing.co.at
 License: BSD License
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: TFL (>=3)
 Provides-Extra: minified
 Requires-Dist: rcssmin ; extra == 'minified'
 Requires-Dist: rjsmin ; extra == 'minified'
 Provides-Extra: minified_debian_slow
 Requires-Dist: cssmin ; extra == 'minified_debian_slow'
```

## Comparing `CHJ-3.8.dist-info/RECORD` & `CHJ-3.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 _CHJ/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
 _CHJ/Media.py,sha256=OG7LOUIGXQ5usaA9AAYVtOTmmYfRVIBI7zFzV6nTN0k,16398
 _CHJ/Parameters.py,sha256=idLnG2MVzwhguwIdDbyzCmiiCyTwf7k7cwm67UpYObQ,14655
 _CHJ/README.rst,sha256=9MqzNE-p3FVi5-YC1gsTsgXbq39b4anaSRbaDiRrvPg,449
-_CHJ/VERSION.py,sha256=KiYr46rtJXBi6xbe4hRpXF4qiVDkNPUewuVClvYGaG4,62
+_CHJ/VERSION.py,sha256=9SWzE5vIomnAHNs_S2yzGRGS2uyp9lEAUIIWLKHojdY,62
 _CHJ/__init__.py,sha256=CQe3NbIXmxPtVDJ9Sy8WzSrhFdtMTOJVOhhPKTCYDPw,809
 _CHJ/setup.cfg,sha256=eKhAFM3IPYhPYp110DyceMV7UVnztKmHZXP_Mz1CuaM,26
-_CHJ/setup.py,sha256=tvsN13DLc8r4Cv6xgVasVGZckYohsc-gTBF0_8Qrgog,3174
+_CHJ/setup.py,sha256=aKfw6RME1lXfu23KCoRMhOkLof478sh_5FYel437c6M,3230
 _CHJ/_CSS/CS.py,sha256=PS4AM2gLzmTZdTG36GOBK9GsDHG0P0G25l3NNBmdkAM,4673
 _CHJ/_CSS/Calc.py,sha256=awJbgK66gijlsF6Ge0fng4ftcavQql52-kXgOoEBHTM,4339
 _CHJ/_CSS/Color.py,sha256=UaoaJ5HwY0VlHNx6ryRZvHqUsK7U-u-wBen-wrbIWqU,6014
 _CHJ/_CSS/Length.py,sha256=l9vtVp5uLq0xY_ye-mtDISgRvK8MCW8OMK54hH87hsk,13618
 _CHJ/_CSS/Media.py,sha256=vJJRNVLaouHJQK9aHBP8eIoopSD5gatl_9Ms_7M1pzw,10544
 _CHJ/_CSS/Property.py,sha256=zfaBgN3F_EGf6aGN9hREO5_wqF1qDn8bqgMRkipq12U,8218
 _CHJ/_CSS/Rule.py,sha256=saLsFyoBhjkrRC4F8t4i7ioyOlRDqsOhk3gFy4SQ_OI,9356
 _CHJ/_CSS/Shape.py,sha256=tNJZYpEvlB0boiD-402oGkzxLt6QOrE_s9Y6bY4yKTY,12539
 _CHJ/_CSS/Style_Sheet.py,sha256=SGIX_PfALWH6THOEVurT7jHAUFFHJJM5SEny7aw6FLo,4007
 _CHJ/_CSS/_TRBL_.py,sha256=_BqOG9tzB6hO_GBrLmmoXSsHRUDenFRSsZ_MyBM2Tnw,2575
 _CHJ/_CSS/__init__.py,sha256=_1xXxTo6GLXpJrCbFJithu9dXz5RhaPT68bBs2WLJi8,896
 _CHJ/_CSS/import_CSS.py,sha256=oppCO0AMz8-OjPCJHZ6yPAd7vb0Xm7JXlOATBAJFvE8,1361
-CHJ-3.8.dist-info/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
-CHJ-3.8.dist-info/METADATA,sha256=SXyWrSM1fN9Iluqs9oLNb7j6ENag9MbVL5SlVZiX85Q,1445
-CHJ-3.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-CHJ-3.8.dist-info/top_level.txt,sha256=WeTgx0w2ZqUHH72QzNUyE_gBUNglwFS5DfZeCb6CKzM,5
-CHJ-3.8.dist-info/RECORD,,
+CHJ-3.9.dist-info/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
+CHJ-3.9.dist-info/METADATA,sha256=vZiWmzdwCkX-9v-TWJvifVevLyTBMeRU5m1CXT_b9rA,1445
+CHJ-3.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+CHJ-3.9.dist-info/top_level.txt,sha256=WeTgx0w2ZqUHH72QzNUyE_gBUNglwFS5DfZeCb6CKzM,5
+CHJ-3.9.dist-info/RECORD,,
```

