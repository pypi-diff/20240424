# Comparing `tmp/ATAX-3.8-py2.py3-none-any.whl.zip` & `tmp/ATAX-3.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 35489 bytes, number of entries: 19
+Zip file size: 35501 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx     1488 b- defN 16-Oct-12 17:21 _ATAX/LICENSE
 -rw-rw-r--  2.0 unx      470 b- defN 22-Jul-02 15:50 _ATAX/README.rst
--rw-rw-r--  2.0 unx       62 b- defN 23-May-29 18:58 _ATAX/VERSION.py
+-rw-rw-r--  2.0 unx       62 b- defN 24-Apr-24 16:03 _ATAX/VERSION.py
 -rw-rw-r--  2.0 unx      861 b- defN 22-Jul-02 15:02 _ATAX/__init__.py
 -rw-rw-r--  2.0 unx    64026 b- defN 22-Jul-02 15:02 _ATAX/accounting.py
 -rw-rw-r--  2.0 unx    20701 b- defN 22-Jul-02 15:02 _ATAX/anlagenverzeichnis.py
 -rw-rw-r--  2.0 unx     9024 b- defN 22-Jul-02 15:02 _ATAX/fahrtenbuch.py
 -rw-rw-r--  2.0 unx     3820 b- defN 22-Jul-02 15:02 _ATAX/fahrtenbuch_p.py
 -rw-rw-r--  2.0 unx     5027 b- defN 22-Jul-02 15:02 _ATAX/income_tax_at.py
 -rw-rw-r--  2.0 unx     3420 b- defN 22-Jul-02 15:02 _ATAX/jahresabschluss.py
 -rw-rw-r--  2.0 unx     2437 b- defN 22-Jul-02 15:02 _ATAX/kassabuch.py
 -rw-rw-r--  2.0 unx       26 b- defN 16-Oct-12 17:21 _ATAX/setup.cfg
--rw-rw-r--  2.0 unx     2636 b- defN 23-May-29 18:38 _ATAX/setup.py
+-rw-rw-r--  2.0 unx     2692 b- defN 24-Apr-24 15:45 _ATAX/setup.py
 -rw-rw-r--  2.0 unx     3132 b- defN 22-Jul-02 15:02 _ATAX/umsatzsteuer.py
--rw-rw-r--  2.0 unx     1488 b- defN 23-May-29 18:58 ATAX-3.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1097 b- defN 23-May-29 18:58 ATAX-3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-29 18:58 ATAX-3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-May-29 18:58 ATAX-3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1419 b- defN 23-May-29 18:58 ATAX-3.8.dist-info/RECORD
-19 files, 121250 bytes uncompressed, 33227 bytes compressed:  72.6%
+-rw-rw-r--  2.0 unx     1488 b- defN 24-Apr-24 16:03 ATAX-3.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1097 b- defN 24-Apr-24 16:03 ATAX-3.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-24 16:03 ATAX-3.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-24 16:03 ATAX-3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1419 b- defN 24-Apr-24 16:03 ATAX-3.9.dist-info/RECORD
+19 files, 121306 bytes uncompressed, 33239 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: _ATAX/setup.py
 Comment: 
 
 Filename: _ATAX/umsatzsteuer.py
 Comment: 
 
-Filename: ATAX-3.8.dist-info/LICENSE
+Filename: ATAX-3.9.dist-info/LICENSE
 Comment: 
 
-Filename: ATAX-3.8.dist-info/METADATA
+Filename: ATAX-3.9.dist-info/METADATA
 Comment: 
 
-Filename: ATAX-3.8.dist-info/WHEEL
+Filename: ATAX-3.9.dist-info/WHEEL
 Comment: 
 
-Filename: ATAX-3.8.dist-info/top_level.txt
+Filename: ATAX-3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ATAX-3.8.dist-info/RECORD
+Filename: ATAX-3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## _ATAX/VERSION.py

```diff
@@ -1,2 +1,2 @@
-__date__    = "2023-05-29T19:42:12+01:00"
-__version__ = "3.8"
+__date__    = "2024-04-24T16:45:19+01:00"
+__version__ = "3.9"
```

## _ATAX/setup.py

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
 
@@ -60,15 +61,15 @@
     , classifiers          = \
         [ "Development Status :: 5 - Production/Stable"
         , "License :: OSI Approved :: " + license
         , "Operating System :: OS Independent"
         , "Programming Language :: Python"
         , "Topic :: Office/Business :: Financial :: Accounting"
         ]
-    , python_requires      = ">=3.8"
+    , python_requires      = ">=3.9"
     , setup_requires       = ["TFL_STP>=3"]
     , install_requires     = ["TFL>=3", "CAL>=3"]
     , extras_require       = dict ()
     , cmdclass             = dict (test = Test_Command)
     , zip_safe             = False ### no eggs, please
     )
```

## Comparing `ATAX-3.8.dist-info/LICENSE` & `ATAX-3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ATAX-3.8.dist-info/METADATA` & `ATAX-3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ATAX
-Version: 3.8
+Version: 3.9
 Summary: Package for doing Einnahmen-Ausgabenrechnung according to Austrian tax laws.
 Home-page: https://codeberg.org/tanzer/tapyr
 Author: Christian Tanzer
 Author-email: tanzer@swing.co.at
 License: BSD License
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Office/Business :: Financial :: Accounting
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: TFL (>=3)
 Requires-Dist: CAL (>=3)
 
 ATAX provides classes and functions for doing simple accounting according to
 Austrian tax laws.
```

## Comparing `ATAX-3.8.dist-info/RECORD` & `ATAX-3.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 _ATAX/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
 _ATAX/README.rst,sha256=SLPhXP2bKeU9VHXmJHrgCKvPH3UVOQs-fCarRXNAYW4,470
-_ATAX/VERSION.py,sha256=KiYr46rtJXBi6xbe4hRpXF4qiVDkNPUewuVClvYGaG4,62
+_ATAX/VERSION.py,sha256=9SWzE5vIomnAHNs_S2yzGRGS2uyp9lEAUIIWLKHojdY,62
 _ATAX/__init__.py,sha256=fEdWLYkB5yEHQAokNDnQYQWoWOvbM6NC_b4gJ-dd1dY,861
 _ATAX/accounting.py,sha256=RQGVTxNwzrB1juWAn2VoZu2V-LSLm4dGZ7cmARud0RM,64026
 _ATAX/anlagenverzeichnis.py,sha256=CSWVl9SGALNtt5DMN6RyNaaZsX0GHYuGoPhxMz9dhkE,20701
 _ATAX/fahrtenbuch.py,sha256=wNVgsxEbopFvi2KShpzT2b8mhD9JQcVPrcTVTQcKs2s,9024
 _ATAX/fahrtenbuch_p.py,sha256=xJMBnIMGnSOFtNZAX8CvHCrK4cY8zNA3Ih3KVIpW-Z8,3820
 _ATAX/income_tax_at.py,sha256=FsmaUpPXI6KfQ4hDTvuuusiP4u4eTxG7KZUazRQ0KUU,5027
 _ATAX/jahresabschluss.py,sha256=PQnT8Mqtq54T0AdQ52Jgj7HO3rw1wy_X1_jHBJOmycE,3420
 _ATAX/kassabuch.py,sha256=NUM8m_NHWCSAHbzxP9Ee-qoIvEtXHpNxD35ovbzOSo0,2437
 _ATAX/setup.cfg,sha256=eKhAFM3IPYhPYp110DyceMV7UVnztKmHZXP_Mz1CuaM,26
-_ATAX/setup.py,sha256=44VO3w7qJjDhHVJ00lZm9_15QsTqBaoA0oudtQ9L5xw,2636
+_ATAX/setup.py,sha256=QN48zZ8kUsgchasAd6Ny8zlWCcdwlgCpkT1uKQh9xUw,2692
 _ATAX/umsatzsteuer.py,sha256=9_RRYg58jhC_4FMxGvGTkpykOmj0yOpI01wk28Z19qg,3132
-ATAX-3.8.dist-info/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
-ATAX-3.8.dist-info/METADATA,sha256=iEvkWycDawLQSHm9kLQ2V0RpxTpsD0n36OZPDJLlprw,1097
-ATAX-3.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-ATAX-3.8.dist-info/top_level.txt,sha256=WfXGJuJnhqe6RJCt0rsFmQBwe2pNEF9SHVG1a8p8QlI,6
-ATAX-3.8.dist-info/RECORD,,
+ATAX-3.9.dist-info/LICENSE,sha256=vNT2X-Co_3EnWxE_k0jdK4noRvjPmPKhBQGx6qdL56A,1488
+ATAX-3.9.dist-info/METADATA,sha256=3b_ogf29uA3x1GnYxM2t3VAyzNDjFRbJ8doPQRxrJc0,1097
+ATAX-3.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+ATAX-3.9.dist-info/top_level.txt,sha256=WfXGJuJnhqe6RJCt0rsFmQBwe2pNEF9SHVG1a8p8QlI,6
+ATAX-3.9.dist-info/RECORD,,
```

