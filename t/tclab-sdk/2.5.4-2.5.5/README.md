# Comparing `tmp/tclab_sdk-2.5.4-py2.py3-none-any.whl.zip` & `tmp/tclab_sdk-2.5.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13102 bytes, number of entries: 7
+Zip file size: 13100 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat    42150 b- defN 24-Mar-23 13:10 tclab/__init__.py
--rw-rw-rw-  2.0 fat    10457 b- defN 24-Mar-23 13:07 tclab/lab.py
--rw-rw-rw-  2.0 fat      703 b- defN 24-Mar-23 13:11 tclab_sdk-2.5.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Mar-23 13:11 tclab_sdk-2.5.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       39 b- defN 24-Mar-23 13:11 tclab_sdk-2.5.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Mar-23 13:11 tclab_sdk-2.5.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      547 b- defN 24-Mar-23 13:11 tclab_sdk-2.5.4.dist-info/RECORD
-7 files, 54012 bytes uncompressed, 12134 bytes compressed:  77.5%
+-rw-rw-rw-  2.0 fat    10458 b- defN 24-Apr-24 12:37 tclab/lab.py
+-rw-rw-rw-  2.0 fat      703 b- defN 24-Apr-24 12:38 tclab_sdk-2.5.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-24 12:38 tclab_sdk-2.5.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-24 12:38 tclab_sdk-2.5.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-24 12:38 tclab_sdk-2.5.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      547 b- defN 24-Apr-24 12:38 tclab_sdk-2.5.5.dist-info/RECORD
+7 files, 54013 bytes uncompressed, 12132 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: tclab/__init__.py
 Comment: 
 
 Filename: tclab/lab.py
 Comment: 
 
-Filename: tclab_sdk-2.5.4.dist-info/METADATA
+Filename: tclab_sdk-2.5.5.dist-info/METADATA
 Comment: 
 
-Filename: tclab_sdk-2.5.4.dist-info/WHEEL
+Filename: tclab_sdk-2.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: tclab_sdk-2.5.4.dist-info/entry_points.txt
+Filename: tclab_sdk-2.5.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: tclab_sdk-2.5.4.dist-info/top_level.txt
+Filename: tclab_sdk-2.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tclab_sdk-2.5.4.dist-info/RECORD
+Filename: tclab_sdk-2.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tclab/lab.py

```diff
@@ -128,15 +128,15 @@
     data=[]
     for i in remove_prefix(dir(parent)):
         data.append({"name":i,"func":eval(f"parent.{i}"),"enter":"tree_attr(Data[Select]['func'])","children":f"tree_func(Data[Select]['func'])"})
         if '_status' in dir(eval(f"parent.{i}")) and "__status" not in dir(eval(f"parent.{i}")):
             if i in Status_Map:
                 data[-1]["status"]=Status_Map[i]
             else:
-                data[-1]["status"]=eval(f"parent.{i}._status(refresh=True)")
+                data[-1]["status"]=eval(f"parent.{i}._status(refresh=False)")
                 eval(f"parent.{i}").__status=data[-1]["status"]
                 Status_Map[i]=data[-1]["status"]
     return data
 
 def tree_attr(parent):
     """获取树形参数结构
```

## Comparing `tclab_sdk-2.5.4.dist-info/METADATA` & `tclab_sdk-2.5.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 2.5.4
+Version: 2.5.5
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,12 +18,12 @@
 Requires-Dist: rich
 Requires-Dist: blessed
 
 # TC Laboratory Central_Management_System Client Module
 
 ## 简介
 
-Tclab中央管理程序Python端SDK V2.5.3 (Beta)
+Tclab中央管理程序Python端SDK V2.5.5 (Beta)
```

## Comparing `tclab_sdk-2.5.4.dist-info/RECORD` & `tclab_sdk-2.5.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 tclab/__init__.py,sha256=5dJxs9FxFBqN9pGX2R0ZR8G0WsEizQqkJZYzM4Cl3tk,42150
-tclab/lab.py,sha256=8NEL_r5QwE-d01_RGrYkZDdSLQSwaLapw9tbG-3lqM4,10457
-tclab_sdk-2.5.4.dist-info/METADATA,sha256=cKpBGK5qbZsTu0QJEduJ1Bk_AqWg5JP3LFetMFMk9_g,703
-tclab_sdk-2.5.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-tclab_sdk-2.5.4.dist-info/entry_points.txt,sha256=5K4SKVjx9Pa2otip47KwDgsSxlfzxmO8QTkbMcwUr54,39
-tclab_sdk-2.5.4.dist-info/top_level.txt,sha256=suFOVgpHLWP5puwKsSZumR0r9m_gMq-5ynwUsBtS1ks,6
-tclab_sdk-2.5.4.dist-info/RECORD,,
+tclab/lab.py,sha256=J9T55wAUGssxi12Yut007iw6AGeU1dvYHHfM2qihk1o,10458
+tclab_sdk-2.5.5.dist-info/METADATA,sha256=TeE9bQMKQp529A8TOa0BFZkjY87JgaKFfRExIbbr7Qw,703
+tclab_sdk-2.5.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+tclab_sdk-2.5.5.dist-info/entry_points.txt,sha256=5K4SKVjx9Pa2otip47KwDgsSxlfzxmO8QTkbMcwUr54,39
+tclab_sdk-2.5.5.dist-info/top_level.txt,sha256=suFOVgpHLWP5puwKsSZumR0r9m_gMq-5ynwUsBtS1ks,6
+tclab_sdk-2.5.5.dist-info/RECORD,,
```

