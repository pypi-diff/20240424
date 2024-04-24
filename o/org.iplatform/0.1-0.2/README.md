# Comparing `tmp/org.iplatform-0.1-py3-none-any.whl.zip` & `tmp/org.iplatform-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 21255 bytes, number of entries: 40
+Zip file size: 21257 bytes, number of entries: 40
 -rw-rw-rw-  2.0 fat     1529 b- defN 24-Apr-21 10:51 org/iplatform/common/entities/asset/Asset.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 09:53 org/iplatform/common/entities/asset/__init__.py
 -rw-rw-rw-  2.0 fat      530 b- defN 24-Apr-21 09:13 org/iplatform/common/entities/coordinate/Coordinate.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 09:53 org/iplatform/common/entities/coordinate/__init__.py
 -rw-rw-rw-  2.0 fat     3631 b- defN 24-Apr-22 06:25 org/iplatform/common/entities/device/Device.py
 -rw-rw-rw-  2.0 fat      269 b- defN 24-Apr-21 06:37 org/iplatform/common/entities/device/DeviceType.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 09:53 org/iplatform/common/entities/device/__init__.py
@@ -30,13 +30,13 @@
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 09:53 org/iplatform/common/entities/protocol/__init__.py
 -rw-rw-rw-  2.0 fat      133 b- defN 24-Apr-21 10:54 org/iplatform/common/entities/relation/Relation.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 09:53 org/iplatform/common/entities/relation/__init__.py
 -rw-rw-rw-  2.0 fat     2742 b- defN 24-Apr-21 01:46 org/iplatform/common/entities/role/Role.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 09:53 org/iplatform/common/entities/role/__init__.py
 -rw-rw-rw-  2.0 fat     7088 b- defN 24-Apr-22 05:22 org/iplatform/common/entities/user/User.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-23 09:53 org/iplatform/common/entities/user/__init__.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-24 08:32 org.iplatform-0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9494 b- defN 24-Apr-24 08:32 org.iplatform-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 08:32 org.iplatform-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-Apr-24 08:32 org.iplatform-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4123 b- defN 24-Apr-24 08:32 org.iplatform-0.1.dist-info/RECORD
-40 files, 48017 bytes uncompressed, 14289 bytes compressed:  70.2%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-24 08:33 org.iplatform-0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9494 b- defN 24-Apr-24 08:33 org.iplatform-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 08:33 org.iplatform-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-Apr-24 08:33 org.iplatform-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     4123 b- defN 24-Apr-24 08:33 org.iplatform-0.2.dist-info/RECORD
+40 files, 48017 bytes uncompressed, 14291 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -99,23 +99,23 @@
 
 Filename: org/iplatform/common/entities/user/User.py
 Comment: 
 
 Filename: org/iplatform/common/entities/user/__init__.py
 Comment: 
 
-Filename: org.iplatform-0.1.dist-info/LICENSE
+Filename: org.iplatform-0.2.dist-info/LICENSE
 Comment: 
 
-Filename: org.iplatform-0.1.dist-info/METADATA
+Filename: org.iplatform-0.2.dist-info/METADATA
 Comment: 
 
-Filename: org.iplatform-0.1.dist-info/WHEEL
+Filename: org.iplatform-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: org.iplatform-0.1.dist-info/top_level.txt
+Filename: org.iplatform-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: org.iplatform-0.1.dist-info/RECORD
+Filename: org.iplatform-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `org.iplatform-0.1.dist-info/LICENSE` & `org.iplatform-0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `org.iplatform-0.1.dist-info/METADATA` & `org.iplatform-0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: org.iplatform
-Version: 0.1
+Version: 0.2
 Summary: A common package for iplatform
 Author-email: Anthony Tony <author@example.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

## Comparing `org.iplatform-0.1.dist-info/RECORD` & `org.iplatform-0.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 org/iplatform/common/entities/protocol/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 org/iplatform/common/entities/relation/Relation.py,sha256=WtpWDMyMaxOQ7anHBKgqM-isV13Rvv3W-XW4yNL94uc,133
 org/iplatform/common/entities/relation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 org/iplatform/common/entities/role/Role.py,sha256=O4rmyT2eLTGh5aR5CnnPcsqz2nTtqA2jk8Ku1PFYJ4U,2742
 org/iplatform/common/entities/role/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 org/iplatform/common/entities/user/User.py,sha256=-LBwRKzwW2Xk6DgE_65-ZBUS5QWmFNK71ZPSd_fEltg,7088
 org/iplatform/common/entities/user/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-org.iplatform-0.1.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-org.iplatform-0.1.dist-info/METADATA,sha256=B4f16GAvIEBvVd-x3k4GgWIwb6HvdQ71n11qnHhh8Is,9494
-org.iplatform-0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-org.iplatform-0.1.dist-info/top_level.txt,sha256=Y-Q3pQ6MMlBKzHVfq3nXGvODPPpbfj5OBXrcr17O02w,4
-org.iplatform-0.1.dist-info/RECORD,,
+org.iplatform-0.2.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+org.iplatform-0.2.dist-info/METADATA,sha256=eJOm678d3c2KvUK2eZqoiGoyNe_eEWvdj2GkKY8uT0Q,9494
+org.iplatform-0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+org.iplatform-0.2.dist-info/top_level.txt,sha256=Y-Q3pQ6MMlBKzHVfq3nXGvODPPpbfj5OBXrcr17O02w,4
+org.iplatform-0.2.dist-info/RECORD,,
```

