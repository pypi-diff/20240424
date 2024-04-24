# Comparing `tmp/ReST_Tapyr-3.8-py2.py3-none-any.whl.zip` & `tmp/ReST_Tapyr-3.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 15912 bytes, number of entries: 20
+Zip file size: 15921 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx     2982 b- defN 22-Jul-02 15:02 _ReST/Directives.py
 -rw-rw-r--  2.0 unx     2468 b- defN 22-Jul-02 15:02 _ReST/HTML_Writer.py
 -rw-rw-r--  2.0 unx     1488 b- defN 16-Oct-12 17:21 _ReST/LICENSE
 -rw-rw-r--  2.0 unx      693 b- defN 22-Jul-02 15:50 _ReST/README.rst
 -rw-rw-r--  2.0 unx     4415 b- defN 22-Jul-02 15:02 _ReST/Roles.py
 -rw-rw-r--  2.0 unx     6109 b- defN 22-Jul-02 15:02 _ReST/To_Html.py
--rw-rw-r--  2.0 unx       62 b- defN 23-May-29 18:58 _ReST/VERSION.py
+-rw-rw-r--  2.0 unx       62 b- defN 24-Apr-24 16:03 _ReST/VERSION.py
 -rw-rw-r--  2.0 unx     1208 b- defN 22-Jul-02 15:02 _ReST/__init__.py
 -rw-rw-r--  2.0 unx       22 b- defN 13-Nov-18 13:49 _ReST/babel.cfg
 -rw-rw-r--  2.0 unx       26 b- defN 16-Oct-12 17:21 _ReST/setup.cfg
--rw-rw-r--  2.0 unx     2665 b- defN 23-May-29 18:39 _ReST/setup.py
+-rw-rw-r--  2.0 unx     2721 b- defN 24-Apr-24 15:45 _ReST/setup.py
 -rw-rw-r--  2.0 unx     1470 b- defN 20-May-20 10:29 _ReST/-I18N/de.po
 -rw-rw-r--  2.0 unx     1404 b- defN 20-May-20 10:29 _ReST/-I18N/en.po
 -rw-rw-r--  2.0 unx     1199 b- defN 20-May-20 10:29 _ReST/-I18N/pt.po
 -rw-rw-r--  2.0 unx     1149 b- defN 20-May-20 10:29 _ReST/-I18N/template.pot
--rw-rw-r--  2.0 unx     1488 b- defN 23-May-29 18:58 ReST_Tapyr-3.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1357 b- defN 23-May-29 18:58 ReST_Tapyr-3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-29 18:58 ReST_Tapyr-3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-May-29 18:58 ReST_Tapyr-3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1489 b- defN 23-May-29 18:58 ReST_Tapyr-3.8.dist-info/RECORD
-20 files, 31810 bytes uncompressed, 13542 bytes compressed:  57.4%
+-rw-rw-r--  2.0 unx     1488 b- defN 24-Apr-24 16:03 ReST_Tapyr-3.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1357 b- defN 24-Apr-24 16:03 ReST_Tapyr-3.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-24 16:03 ReST_Tapyr-3.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-24 16:03 ReST_Tapyr-3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1489 b- defN 24-Apr-24 16:03 ReST_Tapyr-3.9.dist-info/RECORD
+20 files, 31866 bytes uncompressed, 13551 bytes compressed:  57.5%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: _ReST/-I18N/pt.po
 Comment: 
 
 Filename: _ReST/-I18N/template.pot
 Comment: 
 
-Filename: ReST_Tapyr-3.8.dist-info/LICENSE
+Filename: ReST_Tapyr-3.9.dist-info/LICENSE
 Comment: 
 
-Filename: ReST_Tapyr-3.8.dist-info/METADATA
+Filename: ReST_Tapyr-3.9.dist-info/METADATA
 Comment: 
 
-Filename: ReST_Tapyr-3.8.dist-info/WHEEL
+Filename: ReST_Tapyr-3.9.dist-info/WHEEL
 Comment: 
 
-Filename: ReST_Tapyr-3.8.dist-info/top_level.txt
+Filename: ReST_Tapyr-3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ReST_Tapyr-3.8.dist-info/RECORD
+Filename: ReST_Tapyr-3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## _ReST/VERSION.py

```diff
@@ -1,2 +1,2 @@
-__date__    = "2023-05-29T19:42:12+01:00"
-__version__ = "3.8"
+__date__    = "2024-04-24T16:45:19+01:00"
+__version__ = "3.9"
```

## _ReST/setup.py

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
 #    12-Oct-2016 (CT) Creation
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
 
@@ -60,15 +61,15 @@
         [ "Development Status :: 5 - Production/Stable"
         , "License :: OSI Approved :: " + license
         , "Operating System :: OS Independent"
         , "Programming Language :: Python"
         , "Intended Audience :: Developers"
         , "Topic :: Software Development :: Libraries :: Python Modules"
         ]
-    , python_requires      = ">=3.8"
+    , python_requires      = ">=3.9"
     , setup_requires       = ["TFL_STP>=3"]
     , install_requires     = ["TFL>=3", "docutils"]
     , extras_require       = dict ()
     , cmdclass             = dict (test = Test_Command)
     , zip_safe             = False ### no eggs, please
     )
```

## Comparing `ReST_Tapyr-3.8.dist-info/LICENSE` & `ReST_Tapyr-3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ReST_Tapyr-3.8.dist-info/METADATA` & `ReST_Tapyr-3.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ReST-Tapyr
-Version: 3.8
+Version: 3.9
 Summary: Package augmenting docutil's reStructuredText handling.
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
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: TFL (>=3)
 Requires-Dist: docutils
 
 ReST provides classes and functions augmenting docutil's reStructuredText
 handling:
```

## Comparing `ReST_Tapyr-3.8.dist-info/RECORD` & `ReST_Tapyr-3.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 _ReST/Directives.py,sha256=NW-51YxzlYk4tMEb5TJ6mMTKgom9R6nvyNL8UWHt_Mo,2982
 _ReST/HTML_Writer.py,sha256=Ny9Mz6clA_uGYcFQ8R93QHiwcBPE0EYtlhLK92Vo9Dg,2468
 _ReST/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
 _ReST/README.rst,sha256=9ivPhSx_-wL2SKPHTWAK1A05cL9FYh7a5cfpnTbAMjs,693
 _ReST/Roles.py,sha256=PQWdK0cXs_Vu6tggxkWPFK0GShBs7FQ_yiyiP2Ajaos,4415
 _ReST/To_Html.py,sha256=aZi1t_00y3jUMvvbkaZjMvbF7-Q6nXOr1o5gb3yXIHc,6109
-_ReST/VERSION.py,sha256=KiYr46rtJXBi6xbe4hRpXF4qiVDkNPUewuVClvYGaG4,62
+_ReST/VERSION.py,sha256=9SWzE5vIomnAHNs_S2yzGRGS2uyp9lEAUIIWLKHojdY,62
 _ReST/__init__.py,sha256=VjvvODuJc9FsXnd3XKia7dJlJYGRnQqjVboyM3LRMT4,1208
 _ReST/babel.cfg,sha256=erS9tstsRoqErz9ZovM1unBlKentCIdiaEEK6kMsCZE,22
 _ReST/setup.cfg,sha256=eKhAFM3IPYhPYp110DyceMV7UVnztKmHZXP_Mz1CuaM,26
-_ReST/setup.py,sha256=mATGC6v1qbNbnLpeZ-0hGxxHx4skfPPWx4s2YgPRxTU,2665
+_ReST/setup.py,sha256=PNebnbykBnrziS0E398z62aaR52ka1-0RKLL5dCjKgQ,2721
 _ReST/-I18N/de.po,sha256=SEbbRaFkkSvn6qmp27o-sMumyAUhdlGAQ1APNzfZoL4,1470
 _ReST/-I18N/en.po,sha256=n7j3SCWw3dSoMDmp0RNIBV0Y31UzQwyoXKNtKsjLJNg,1404
 _ReST/-I18N/pt.po,sha256=WWgNSA6eWEjvryJAAKJItv5U6dCRKUupzMnBEG6KSKA,1199
 _ReST/-I18N/template.pot,sha256=vHp1jrXG8OsFGUiDDu6Pe70UFRIW5RHmLRg_9gGRS-o,1149
-ReST_Tapyr-3.8.dist-info/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
-ReST_Tapyr-3.8.dist-info/METADATA,sha256=IAD6UnIFkr19BPQy4okBmJqYgtEOVwLSt50TYdw1BcQ,1357
-ReST_Tapyr-3.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-ReST_Tapyr-3.8.dist-info/top_level.txt,sha256=PSu3nQ3-l0Vj0B-8-QGty4BiZ-5p9muPQJbr4Itxc3I,6
-ReST_Tapyr-3.8.dist-info/RECORD,,
+ReST_Tapyr-3.9.dist-info/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
+ReST_Tapyr-3.9.dist-info/METADATA,sha256=GWBw2bqgJMpPKR_DrfhsRTqLOhIJHni7crYN5n5f8CE,1357
+ReST_Tapyr-3.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+ReST_Tapyr-3.9.dist-info/top_level.txt,sha256=PSu3nQ3-l0Vj0B-8-QGty4BiZ-5p9muPQJbr4Itxc3I,6
+ReST_Tapyr-3.9.dist-info/RECORD,,
```

