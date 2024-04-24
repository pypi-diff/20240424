# Comparing `tmp/lazysdk-0.1.9.tar.gz` & `tmp/lazysdk-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazysdk-0.1.9.tar", last modified: Fri Jun  9 10:27:00 2023, max compression
+gzip compressed data, was "lazysdk-0.1.90.tar", last modified: Wed Apr 24 09:31:29 2024, max compression
```

## Comparing `lazysdk-0.1.9.tar` & `lazysdk-0.1.90.tar`

### file list

```diff
@@ -1,34 +1,47 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 10:27:00.415120 lazysdk-0.1.9/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-09 10:27:00.415009 lazysdk-0.1.9/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      993 2023-02-23 03:14:55.000000 lazysdk-0.1.9/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 10:27:00.414218 lazysdk-0.1.9/lazysdk/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      402 2023-02-23 03:44:47.000000 lazysdk-0.1.9/lazysdk/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-06-06 09:15:38.000000 lazysdk-0.1.9/lazysdk/lazyCrypto.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      555 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazybase64.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6829 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazydict.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyenv.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    13091 2023-02-25 06:33:34.000000 lazysdk-0.1.9/lazysdk/lazyexcel.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    20267 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyfile.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyflask.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      607 2023-02-23 03:41:38.000000 lazysdk-0.1.9/lazysdk/lazyid.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      451 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyip.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    31954 2023-06-09 10:26:14.000000 lazysdk-0.1.9/lazysdk/lazym3u8.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazymd5.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4305 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazypath.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5159 2023-06-07 09:23:18.000000 lazysdk-0.1.9/lazysdk/lazyprocess.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyproxies.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyrandom.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyredis.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2511 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyrequests.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1448 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazytext.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    23199 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazytime.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3783 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazyua.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2023-02-23 03:14:55.000000 lazysdk-0.1.9/lazysdk/lazywebhook.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-06-09 10:27:00.414833 lazysdk-0.1.9/lazysdk.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1369 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      626 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      163 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2023-06-09 10:27:00.000000 lazysdk-0.1.9/lazysdk.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-06-09 10:27:00.415159 lazysdk-0.1.9/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1121 2023-06-09 10:26:14.000000 lazysdk-0.1.9/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-24 09:31:29.453055 lazysdk-0.1.90/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1088 2023-12-14 08:15:44.000000 lazysdk-0.1.90/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-04-24 09:31:29.452845 lazysdk-0.1.90/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1073 2023-12-30 02:37:03.000000 lazysdk-0.1.90/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-24 09:31:29.451857 lazysdk-0.1.90/lazysdk/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      184 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyCrypto.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2797 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazy_id_card.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      669 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazybase64.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      571 2024-02-02 03:54:22.000000 lazysdk-0.1.90/lazysdk/lazycache.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    15383 2023-12-25 11:22:47.000000 lazysdk-0.1.90/lazysdk/lazychromedriver.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      414 2024-02-01 03:07:43.000000 lazysdk-0.1.90/lazysdk/lazydecode.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8883 2024-01-09 11:35:26.000000 lazysdk-0.1.90/lazysdk/lazydict.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyenv.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    15835 2024-02-02 07:00:02.000000 lazysdk-0.1.90/lazysdk/lazyexcel.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    20263 2024-02-04 08:23:46.000000 lazysdk-0.1.90/lazysdk/lazyfile.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyflask.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1867 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyhtml.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1287 2024-01-27 02:46:52.000000 lazysdk-0.1.90/lazysdk/lazyid.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3673 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyinfo.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1364 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyip.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      867 2024-01-18 03:56:02.000000 lazysdk-0.1.90/lazysdk/lazyjson.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      363 2024-04-24 09:30:41.000000 lazysdk-0.1.90/lazysdk/lazylist.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    31937 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazym3u8.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazymd5.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5922 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazypath.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    17702 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyprocess.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyproxies.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1420 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyrandom.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyredis.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3750 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyrequests.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2627 2024-03-22 06:24:43.000000 lazysdk-0.1.90/lazysdk/lazytext.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    26530 2024-02-02 08:29:53.000000 lazysdk-0.1.90/lazysdk/lazytime.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4827 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyua.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1550 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazyurl.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8386 2024-02-05 09:57:19.000000 lazysdk-0.1.90/lazysdk/lazywebhook.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      716 2023-12-14 08:15:44.000000 lazysdk-0.1.90/lazysdk/lazywifi.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      770 2024-03-22 06:19:36.000000 lazysdk-0.1.90/lazysdk/lazyxml.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1683 2023-12-26 07:19:36.000000 lazysdk-0.1.90/lazysdk/showdata.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-24 09:31:29.452586 lazysdk-0.1.90/lazysdk.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      887 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      216 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2024-04-24 09:31:29.000000 lazysdk-0.1.90/lazysdk.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-24 09:31:29.453105 lazysdk-0.1.90/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1208 2024-04-24 09:30:41.000000 lazysdk-0.1.90/setup.py
```

### Comparing `lazysdk-0.1.9/PKG-INFO` & `lazysdk-0.1.90/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-Metadata-Version: 2.1
-Name: lazysdk
-Version: 0.1.9
-Summary: 基于Python的懒人包
-Home-page: https://gitee.com/ZeroSeeker/lazysdk
-Author: ZeroSeeker
-Author-email: zeroseeker@foxmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # lazysdk
 ![](https://img.shields.io/badge/Python-3.8.6-green.svg)
 
 
 #### 介绍
 基于Python3的懒人包
+详细文档见：https://gzcaxecc4u.feishu.cn/docx/EaymdTdIQolphcxgD2jcMsjJn6c
 
 #### 软件架构
 软件架构说明
 - lazysdk.lazyprocess
   - 多进程控制
 
 - lazysdk.lazywebhook
```

### Comparing `lazysdk-0.1.9/lazysdk/lazydict.py` & `lazysdk-0.1.90/lazysdk/lazydict.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding = utf8
 """
 @ Author : ZeroSeeker
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
+import copy
 from collections import OrderedDict
 from urllib import parse
 
 
 def dict_list_ranker_x(dict_list, rank_by_list):
     """
     对dict组成的list按照某个元素重新排序
@@ -73,26 +74,29 @@
 def dict_list_group(list_in, by):
     """
     将dict组成的list按照某个key的值分组，分组后组成新的dict嵌套list
     :param list_in:
     :param by:
     :return:
     """
-    by_list = list()
-    for each_dict in list_in:
-        by_value = each_dict.get(by)
-        by_list.append(by_value)
-    by_set = set(by_list)
-    group_dict = dict()
-    for each_by in by_set:
-        group_dict[each_by] = list()
-    for each_dict in list_in:
-        by_value = each_dict.get(by)
-        group_dict[by_value].extend([each_dict])
-    return group_dict
+    if not list_in:
+        return
+    else:
+        by_list = list()
+        for each_dict in list_in:
+            by_value = each_dict.get(by)
+            by_list.append(by_value)
+        by_set = set(by_list)
+        group_dict = dict()
+        for each_by in by_set:
+            group_dict[each_by] = list()
+        for each_dict in list_in:
+            by_value = each_dict.get(by)
+            group_dict[by_value].extend([each_dict])
+        return group_dict
 
 
 def dict_key_f(in_dict):
     """
     将以驼峰方式命名的dict转换为下划线方式
     """
     out_dict = dict()
@@ -178,38 +182,107 @@
         dict_f = dict_tiler(dict_in=each, connector_str=connector_str)
         list_out.append(dict_f)
     return list_out
 
 
 def list_same_order_dict(
         list_data: list = None,
-        na_value=None
+        na_value=None,
+        keys_sort: list = None
 ) -> list:
     """
     list重排格式化，将单层dict组成的list按照全部key的顺序排序并补充缺失值
     :param list_data: 原始list
     :param na_value: 缺失值的默认值
+    :param keys_sort: 指定顺序,按照指定列的顺序先排，不包含的向后排
     :return list_data_f: 处理后的结果
 
     test data:
         [
             {'a': 1},
             {'b': 2},
             {'b': 2, 'a': 1},
             {'c': 21}
         ]
     """
-    keys = list()
+    keys = list()  # 存储所有的key
     for each_dict in list_data:
-        each_keys = list(each_dict.keys())
+        # 遍历list中的每个dict
+        each_keys = list(each_dict.keys())  # 提取当前dict的所有key
         for each_key in each_keys:
+            # 遍历，得到全量唯一的key
             if each_key in keys:
                 continue
             else:
                 keys.append(each_key)
-    list_data_f = list()
+    keys.sort()  # 先按照升序排序一次
+    if keys_sort:
+        keys_new = copy.deepcopy(keys_sort)  # 先直接拷贝一下排序表
+        for each_key in keys:
+            # 遍历生成的key列表
+            if each_key in keys_new:
+                # 如果遍历的key已存在，将跳过
+                continue
+            else:
+                # 如果遍历的key不已存在，则追加
+                keys_new.append(each_key)
+    else:
+        keys_new = copy.deepcopy(keys)
+    list_data_f = list()  # 存储处理后的数据
     for each_dict in list_data:
         each_dict_order = OrderedDict()  # 有序字典
-        for each_key in keys:
+        for each_key in keys_new:
             each_dict_order[each_key] = each_dict.get(each_key, na_value)
         list_data_f.append(each_dict_order)
     return list_data_f
+
+
+def list_dict_filter(
+        list_in: list,
+        filter_key,
+        filter_value
+):
+    """
+    从[{},{}]中按照某个key-value条件筛选出符合条件的记录
+    """
+    list_out = list(filter(lambda x: x[filter_key] == filter_value, list_in))
+    return list_out
+
+
+def key_max_value(
+        list_in: list,
+        key
+):
+    """
+    求list嵌套的dict中某个key的最大值
+    """
+    max_value = None
+    for each in list_in:
+        key_value = each.get(key)
+        if key_value:
+            if max_value is None or key_value > max_value:
+                max_value = copy.deepcopy(key_value)
+            else:
+                continue
+        else:
+            continue
+    return max_value
+
+
+def key_min_value(
+        list_in: list,
+        key
+):
+    """
+    求list嵌套的dict中某个key的最小值
+    """
+    min_value = None
+    for each in list_in:
+        key_value = each.get(key)
+        if key_value:
+            if min_value is None or key_value < min_value:
+                min_value = copy.deepcopy(key_value)
+            else:
+                continue
+        else:
+            continue
+    return min_value
```

### Comparing `lazysdk-0.1.9/lazysdk/lazyenv.py` & `lazysdk-0.1.90/lazysdk/lazyenv.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.9/lazysdk/lazyexcel.py` & `lazysdk-0.1.90/lazysdk/lazyexcel.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 # coding = utf8
 """
 @ Author : ZeroSeeker
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
+import decimal
+import json
 from collections import OrderedDict
 from . import lazydict
 import openpyxl  # 用于处理.xlsx，文档：https://openpyxl.readthedocs.io/en/stable/
 import datetime
 import xlrd  # 用于处理.xls
 import os
 from .lazypath import path_separator
+from .lazytime import get_format_date
+from .lazytime import get_format_datetime
 
 
 # -------------------------------读取功能区域-------------------------------
 def read_xls(
         file: str,
         sheet_name: str = None,
         date_cols: dict = None,
@@ -92,43 +96,54 @@
         table_data_dict[each_sheet.name] = sheet_data_list  # 将每个sheet的数据组织到table_data_dict里面
     return table_data_dict
 
 
 def read_xlsx(
         file: str,
         sheet_name: str = None,
+        sheet_index: int = None,
         date_cols: dict = None,
         auto_conv_date: bool = False  # 默认格式：'%Y-%m-%d %H:%M:%S'
-) -> dict:
+):
     """
     读取xlsx表格
     :param file: 文件路径
     :param sheet_name: 指定sheet名称，读取指定的sheet
     :param date_cols: 按照既定规则转换时间，例如：{'日期': '%Y-%m-%d','时间': '%H:%M:%S'}，就会将表中对应字段转换为对应格式的字符串
     :param auto_conv_date: 自动转换，会将时间类型的数据自动转换为默认格式的字符串
 
-    :returns: 读取结果字典，字典的第一层key为sheet_name
+    :returns: 读取结果字典，字典的第一层key为sheet_name，如果指定了读取哪个sheet，则只返回值list
 
     cell(a,b).data_type 值类型
     n None
     s string
     d date
     其他暂时未知
     """
     if date_cols is None:
         data_cols_cols = []
     else:
         data_cols_cols = date_cols.keys()
     table_data_dict = OrderedDict()  # 有序字典
-    table_data = openpyxl.load_workbook(file)  # 打开表
-    for each_sheet in table_data.worksheets:  # 遍历所有sheet
-        if sheet_name is None:
+    table_data = openpyxl.load_workbook(file)  # 加载表内容
+    sheets = table_data.worksheets
+    if sheet_name is None and sheet_index is not None:
+        target_sheet = sheets[sheet_index].title
+    elif sheet_name and not sheet_index:
+        target_sheet = sheet_name
+    elif sheet_name and sheet_index:
+        return 'sheet_name和sheet_index不可同时指定'
+    else:
+        target_sheet = None
+
+    for each_sheet in sheets:  # 遍历所有sheet
+        if not target_sheet:
             pass
         else:
-            if each_sheet.title == sheet_name:  # 判断当前的sheet是否是需要获取数据的sheet
+            if each_sheet.title == target_sheet:  # 判断当前的sheet是否是需要获取数据的sheet
                 pass
             else:
                 continue
         row_num = each_sheet.max_row  # 获取行数
         col_num = each_sheet.max_column  # 获取列数
         sheet_data_list = list()
         for each_row in range(1, row_num):  # 遍历每一行
@@ -161,15 +176,18 @@
                     continue  # 去除全空值
                 else:
                     pass
             else:
                 pass
             sheet_data_list.append(each_row_data)  # 将每一行的数据dict组织到当前sheet的数据list中
         table_data_dict[each_sheet.title] = sheet_data_list  # 将每个sheet的数据组织到table_data_dict里面
-    return table_data_dict
+    if target_sheet:
+        return table_data_dict[target_sheet]
+    else:
+        return table_data_dict
 
 
 def read(
         file: str,
         sheet_name: str = None,
         date_cols: dict = None,  # date转换为字符串
         auto_conv_date: bool = False  # 默认格式：'%Y-%m-%d %H:%M:%S'
@@ -207,52 +225,97 @@
 # -------------------------------读取功能区域-------------------------------
 # -------------------------------写入功能区域-------------------------------
 
 
 def save_xlsx(
         file: str,
         value: dict = None,
-        date_cols: dict = None,
-        col_name_dict: dict = None
+        date_cols: list = None,
+        datetime_cols: list = None,
+        num_cols: list = None,
+        col_name_dict: dict = None,
+        col_name_sort: list = None
 ):
     """
     如果输入的value是乱序，将重新排序
     :param file: 文件路径
-    :param value: 需要保存的数据
-    :param date_cols: 按照既定规则转换时间，例如：{'日期': '%Y-%m-%d','时间': '%H:%M:%S'}，就会将表中对应字段转换为对应格式的时间
+    :param value: 需要保存的数据，按照{"sheet名": [数据列表]}的形式
+    :param date_cols: 按照既定规则转换日期，例如：['日期']，就会将表中对应字段转换为对应格式的日期
+    :param datetime_cols: 按照既定规则转换时间，例如：['时间']，就会将表中对应字段转换为对应格式的时间
+    :param num_cols: 数字列列表
     :param col_name_dict: 自定义列名的对照关系，规则为：{'旧名称1':'新名称1', '旧名称2':'新名称2'}
+    :param col_name_sort: 自定义列名排序，将按照列表顺序排，如果不在列表中，将随机
     将输出保存后的文件绝对路径
     """
     if os.path.isabs(file):  # 判断是否为绝对路径
         pass
     else:
         file = os.getcwd() + path_separator + file
     if value is None:
         return
     else:
         wb = openpyxl.Workbook()
-        sheet_index = 0
+        sheet_index = 0  # sheet序号
+
+        if not num_cols:
+            num_cols = []
+        if not date_cols:
+            date_cols = []
+        if not datetime_cols:
+            datetime_cols = []
+
         for sheet_name, sheet_data in value.items():
-            sheet = wb.create_sheet(title=sheet_name, index=sheet_index)
+            # 遍历每个要存储的sheet,sheet_name为sheet的名称，sheet_data为对应sheet的数据
+            sheet = wb.create_sheet(
+                title=sheet_name,
+                index=sheet_index
+            )  # 创建一个sheet
             row_num = 1  # 行序号
             col_num = 1  # 列序号
-            if len(sheet_data) > 0:
+            if sheet_data:
+                # 先按照要求处理数据，处理好数据后统一排序
+
                 # 如果数据是乱序，需要先排序
-                sheet_data_f = lazydict.list_same_order_dict(list_data=sheet_data)
+                sheet_data_f = lazydict.list_same_order_dict(
+                    list_data=sheet_data,
+                    keys_sort=col_name_sort
+                )  # 先对要存储的数据做排序对齐
+
                 if date_cols is not None:
                     for each_sheet_data_f in sheet_data_f:
-                        for date_key, date_f in date_cols.items():
-                            try:
-                                date_value = each_sheet_data_f.get(date_key)
-                                if date_value is not None:
-                                    date_value_f = datetime.datetime.strptime(date_value, date_f)
-                                    each_sheet_data_f[date_key] = date_value_f
-                                else:
+                        # 日期格式化
+                        for date_key in date_cols:
+                            date_value = each_sheet_data_f.get(date_key)
+                            if date_value:
+                                try:
+                                    each_sheet_data_f[date_key] = get_format_date(date_ori=date_value)
+                                except:
+                                    pass
+                            else:
+                                continue
+                        # 时间格式化
+                        for datetime_key in datetime_cols:
+                            datetime_value = each_sheet_data_f.get(datetime_key)
+                            if datetime_value:
+                                try:
+                                    each_sheet_data_f[datetime_key] = get_format_datetime(datetime_ori=datetime_value)
+                                except:
                                     pass
-                            except:
+                            else:
+                                continue
+
+                        # 数字格式化
+                        for each_num_col in num_cols:
+                            date_value = each_sheet_data_f.get(each_num_col)
+                            if date_value:
+                                try:
+                                    each_sheet_data_f[each_num_col] = decimal.Decimal(date_value)
+                                except:
+                                    pass
+                            else:
                                 pass
                 else:
                     pass
                 # 写入标题行
                 for key in sheet_data_f[0]:
                     if col_name_dict is not None and col_name_dict.get(key) is not None:
                         sheet.cell(
@@ -269,18 +332,21 @@
                     col_num += 1
 
                 # 写入数据行
                 row_num += 1
                 for each in sheet_data_f:
                     col_num = 1
                     for key in each:
+                        value = each.get(key)
+                        if isinstance(value, dict) or isinstance(value, list):
+                            value = json.dumps(value, ensure_ascii=False)
                         sheet.cell(
                             row=row_num,
                             column=col_num,
-                            value=each.get(key)
+                            value=value
                         )
                         col_num += 1
                     row_num += 1
             else:
                 continue
             sheet_index += 1
         wb.remove(wb.worksheets[-1])  # 删除最后一个默认的sheet
```

### Comparing `lazysdk-0.1.9/lazysdk/lazyfile.py` & `lazysdk-0.1.90/lazysdk/lazyfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,41 +2,64 @@
 # coding = utf8
 """
 @ Author : ZeroSeeker
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
+import copy
+
 from . import lazypath
 import collections
 import subprocess
 import requests
 import platform
 import datetime
 import openpyxl
 import showlog
 import time
 import xlrd
 import json
 import sys
 import os
+# import zipfile
+from rich.progress import Progress
+from requests import exceptions
 
-
-if platform.system() == 'Windows':
-    path_separator = '\\'
-else:
-    path_separator = '/'
 headers_default = {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:68.0) Gecko/20100101 Firefox/68.0"}
 
 
+def delete(
+        file,
+        postfix: str = None,
+        path: str = None,
+):
+    """
+    删除文件
+    """
+    if path:
+        # 如果指定了路径，就加上路径
+        file_dir = os.path.join(path, file)
+    else:
+        # 如果没指定路径，就直接使用文件名
+        file_dir = file
+
+    if postfix:
+        # 如果指定了后缀名，就加上后缀名
+        file_dir = f'{file}.{postfix}'
+    else:
+        # 如果没指定后缀名，就忽略
+        pass
+    os.remove(file_dir)
+
+
 def get_suffix(
         file_name: str
 ):
-    suffix = file_name.split('.')[-1]  # 获取文件后缀名
-    return suffix
+    return file_name.split('.')[-1]  # 获取文件后缀名
 
 
 def file_rename(
         before_name: str,  # 原名称
         after_name: str  # 重命名名称
 ):
     """
@@ -72,54 +95,59 @@
         suffix_name: str = None,
         headers: dict = None,
         path: str = "download",
         proxies=None,
         size_limit: int = None,
         range_start: int = None,
         range_end: int = None,
+        overwrite: bool = False,
+        verify: bool = True
 ):
     """
     实现文件下载功能，可指定url、文件名、后缀名、请求头、文件保存路径
     :param url:
     :param filename:文件名
     :param suffix_name:后缀名
     :param headers:请求头
     :param path:文件保存路径
     :param proxies:代理
     :param size_limit:尺寸限制
     :param range_start:开始位置
     :param range_end:结束位置
+    :param overwrite: 覆盖
+    :param verify: 验证证书
     :return:
     """
-    if headers is None:
+    if not headers:
         headers_local = headers_default
     else:
         headers_local = headers
 
-    if range_start is None and range_end is None:
+    if not range_start and not range_end:
         range_start = 0
         range_info = None
     elif range_start is not None and range_end is None:
         range_info = 'bytes=%d-' % range_start  # 从这里向后
     elif range_start is None and range_end is not None:
         range_start = 0
         range_info = 'bytes=0-%d' % range_end
     else:
         range_info = 'bytes=%d-%d' % (range_start, range_end)
 
-    if range_info is None:
+    if not range_info:
         pass
     else:
         headers_local['Range'] = range_info
     # 获取文件的基本信息
     response = requests.get(
         url=url,
         headers=headers_local,
         stream=True,
-        proxies=proxies
+        proxies=proxies,
+        verify=verify
     )
     total_length = response.headers.get('content-length')  # 文件大小
     content_type = response.headers.get('content-type')  # 文件类型
     content_disposition = response.headers.get('content-disposition')  # 文件名及类型
     filename_default = 'unknown_' + str(time.time())
     if content_disposition is not None:
         content_dispositions = content_disposition.replace(' ', '').split(';')
@@ -146,84 +174,72 @@
     if path is None:
         path_local = download_file_name
     else:
         if os.path.exists(path):
             pass
         else:
             os.makedirs(path)
-        path_local = path + path_separator + download_file_name
+        path_local = os.path.join(path, download_file_name)
 
-    if range_start is None:
+    if not range_start:
         temp_size = 0  # 已经下载文件大小
     else:
         temp_size = range_start + 0  # 已经下载文件大小
-    chunk_size = 1024  # 分割文件大小，字节B
+    chunk_size = 1024 * 1024  # 分割文件大小，字节B
     total_size = int(total_length)  # 文件总大小
-    total_size_mb = round(total_size / (1024 * 1024), 2)  # 换算到MB的文件大小
+    # total_size_mb = round(total_size / (1024 * 1024), 2)  # 换算到MB的文件大小
     # 添加文件大小控制，跳过下载超大文件
     if size_limit is None:
         pass
     else:
         if total_size > size_limit:
             return
         else:
             pass
 
-    time_start = time.time()  # 获取下载开始时间
     is_finish = False
 
+    if overwrite and os.path.exists(path_local):
+        delete(file=path_local)
+    elif not overwrite and os.path.exists(path_local):
+        # 这里将对已存在的文件名重新命名
+        rename_count = 1
+        while True:
+            download_file_name_rename = f'{download_file_name.split(".")[0]}({rename_count}).{download_file_name.split(".")[1]}'
+            path_local_rename = os.path.join(path, download_file_name_rename)
+            if os.path.exists(path_local_rename):
+                rename_count += 1
+                continue
+            else:
+                break
+        path_local = copy.deepcopy(path_local_rename)
+    else:
+        pass
+
     with open(path_local, "ab") as f:  # wb新建文件，a追加
-        for chunk in response.iter_content(chunk_size=chunk_size):
-            try:
-                temp_time_now = time.time()  # 时间采样
-                time_spend_total = temp_time_now - time_start
-                if time_spend_total == 0:
-                    total_speed = round((temp_size-range_start) / (1024 * 1024) / 0.001, 2)  # 计算速度：MB/s
-                else:
-                    total_speed = round((temp_size-range_start) / (1024 * 1024) / time_spend_total, 2)  # 计算速度：MB/s
-                if not chunk:
-                    if temp_size >= total_size:
-                        is_finish = True
-                    else:
-                        is_finish = False
-                    break
-                else:
-                    temp_size += len(chunk)
-                    f.write(chunk)
-                    f.flush()
-                    done = int(50 * temp_size / total_size)
-                    if total_speed == 0 or time_spend_total == 0:
-                        time_left = 0
-                    else:
-                        time_left = (total_size - temp_size) / total_speed / 1024 / 1024
-                    show_dict = {
-                        'finish_mark': '█' * done,
-                        'not_finish_mark': ' ' * (50 - done),
-                        'total_size': total_size_mb,  # 换算到M
-                        'total_percent': round(100 * temp_size / total_size, 4),
-                        'total_speed': total_speed,
-                        'finish_size': round(temp_size / (1024 * 1024), 2),
-                        'time_spend_total': int(time_spend_total),
-                        'time_left': int(time_left)
-                    }
-                    show_msg = "\r[%(finish_mark)s%(not_finish_mark)s] " \
-                               "总大小:%(total_size)sMB " \
-                               "总进度:%(total_percent)s%% " \
-                               "平均速度:%(total_speed)sMB/s " \
-                               "已下载:%(finish_size)sMB " \
-                               "已耗时 %(time_spend_total)s 秒 " \
-                               "预计剩余 %(time_left)s 秒" % show_dict
-                    sys.stdout.write(show_msg)
-                    sys.stdout.flush()
-                    if temp_size >= total_size:
-                        is_finish = True
+        with Progress() as progress:
+            task = progress.add_task(description="[red]Downloading...", total=total_size)
+            for chunk in response.iter_content(chunk_size=chunk_size):
+                try:
+                    if not chunk:
+                        if temp_size >= total_size:
+                            is_finish = True
+                        else:
+                            is_finish = False
+                        break
                     else:
-                        is_finish = False
-            except:
-                showlog.error('')
+                        f.write(chunk)
+                        f.flush()
+                        progress.update(task, advance=chunk_size)
+                        if temp_size >= total_size:
+                            is_finish = True
+                        else:
+                            is_finish = False
+                except:
+                    showlog.error('')
     print("\n  ==> 文件已全部下载完成，保存位置:", path_local)
     res_dict = {
         'file_dir': path_local,
         'is_finish': is_finish,
         'temp_size': temp_size
     }
     return res_dict
@@ -234,207 +250,153 @@
         filename=None,
         suffix_name=None,
         headers=None,
         path="download",
         proxies=None,
         size_limit=None,
         range_start=None,
-        range_end=None
+        range_end=None,
+        verify: bool = False
 ):
     while True:
-        download_response = download(
-            url=url,
-            filename=filename,
-            suffix_name=suffix_name,
-            headers=headers,
-            path=path,
-            proxies=proxies,
-            size_limit=size_limit,
-            range_start=range_start,
-            range_end=range_end
-        )
-        if download_response.get('is_finish') is True:
-            local_file_dir = download_response.get('file_dir')
-            return local_file_dir
-        else:
-            print(':( 下载中断')
-            range_start = download_response.get('temp_size')
+        try:
+            download_response = download(
+                url=url,
+                filename=filename,
+                suffix_name=suffix_name,
+                headers=headers,
+                path=path,
+                proxies=proxies,
+                size_limit=size_limit,
+                range_start=range_start,
+                range_end=range_end,
+                overwrite=False,
+                verify=verify
+            )
+            if download_response.get('is_finish') is True:
+                local_file_dir = download_response.get('file_dir')
+                return local_file_dir
+            else:
+                print(':( 下载中断')
+                range_start = download_response.get('temp_size')
+                time.sleep(1)
+                print('将继续下载（断点续传）...')
+        except:
+            print(':( 下载中断，将重新下载...')
             time.sleep(1)
-            print('将继续下载（断点续传）...')
 
 
 def read(
-        file_name,
-        postfix="txt",
-        path=None,
-        silence=False
+        file,
+        postfix: str = None,
+        path: str = None,
+        json_auto: bool = False,
+        read_lines: bool = False
 ):
-    try:
-        if postfix == "txt":
-            if path is None:
-                f = open("%s.%s" % (file_name, postfix), encoding='utf-8')
-            else:
-                f = open("%s/%s.%s" % (path, file_name, postfix), encoding='utf-8')
-            res = f.read()
-            return res
-        elif postfix == "json":
-            content_list = list()
-            if path is None:
-                with open("%s.%s" % (file_name, postfix), 'r', encoding='utf-8') as f:
-                    content = f.readlines()
-                    for each in content:
-                        each_json = json.loads(each)
-                        content_list.append(each_json)
-            else:
-                with open("./%s/%s.%s" % (path, file_name, postfix), 'r', encoding='utf-8') as f:
-                    content = f.readlines()
-                    for each in content:
-                        each_json = json.loads(each)
-                        content_list.append(each_json)
-            return content_list
-        else:
-            if path is None:
-                f = open("%s.%s" % (file_name, postfix), encoding='utf-8')
+    """
+    读取文件
+    json_auto：json格式自动转换
+    """
+    if path:
+        # 如果指定了路径，就加上路径
+        file_dir = os.path.join(path, file)
+    else:
+        # 如果没指定路径，就直接使用文件名
+        file_dir = file
+
+    if postfix:
+        # 如果指定了后缀名，就加上后缀名
+        file_dir = f'{file}.{postfix}'
+    else:
+        # 如果没指定后缀名，就忽略
+        pass
+
+    if not os.path.exists(file_dir):
+        return
+
+    if read_lines:
+        with open(file=file_dir, mode='r', encoding='utf-8') as f:
+            content = f.readlines()
+    else:
+        f = open(file=file_dir, mode='r', encoding='utf-8')
+        content = f.read()
+
+    if content:
+        if json_auto:
+            if isinstance(content, str):
+                return json.loads(content)
             else:
-                f = open("%s/%s.%s" % (path, file_name, postfix), encoding='utf-8')
-            res = f.read()
-            return res
-    except Exception as e:
-        if silence is True:
-            pass
+                json_content = list()
+                for each_line in content:
+                    json_content.append(json.loads(each_line))
+                return json_content
         else:
-            showlog.warning(e)
-        return
+            return content
+    else:
+        return content
 
 
-def read_(_source_file):
-    # >>读取数据【方式：一次性全部读取】------------------------------------------------------------
-    data = xlrd.open_workbook(_source_file)  # 打开表
-    res = list()
-    # table = data.sheets()[0]  # 默认使用第一张表格
-    for table in data.sheets():
-        nrows = table.nrows  # 获取行数
-        ncols = table.ncols  # 获取列数
-        for inrows in range(nrows):
-            res_temp = dict()
-            for incols in range(ncols):
-                res_temp.update({table.cell(0, incols).value: table.cell(inrows, incols).value})
-            # print(res_temp)
-            res.append(res_temp)
-    return res
+def save(
+        file,
+        content,
+        suffix: str = None,
+        path: str = None,
+        overwrite: bool = True,
+        encoding: str = 'utf-8'
+) -> str:
+    """
+    保存文件
+    """
+    if path:
+        # 如果指定了路径，就加上路径
+        lazypath.make_path(path)
+        file_dir = os.path.join(path, file)
+    else:
+        # 如果没指定路径，就直接使用文件名
+        file_dir = file
+
+    if suffix:
+        # 如果指定了后缀名，就加上后缀名
+        file_dir = f'{file_dir}.{suffix}'
+    else:
+        # 如果没指定后缀名，就忽略
+        pass
+
+    if overwrite is True:
+        write_mode = "w"  # 覆盖
+    else:
+        write_mode = "a"  # 追加
+
+    f = open(
+        file=file_dir,
+        mode=write_mode,
+        encoding=encoding
+    )
+    f.write(content)
+    f.close()
+    return file_dir
 
 
-def excel_read(source_file):
+def read_(_source_file):
     # >>读取数据【方式：一次性全部读取】------------------------------------------------------------
-    data = xlrd.open_workbook(source_file)  # 打开表
+    data = xlrd.open_workbook(_source_file)  # 打开表
     res = list()
     # table = data.sheets()[0]  # 默认使用第一张表格
     for table in data.sheets():
         nrows = table.nrows  # 获取行数
         ncols = table.ncols  # 获取列数
         for inrows in range(nrows):
             res_temp = dict()
             for incols in range(ncols):
                 res_temp.update({table.cell(0, incols).value: table.cell(inrows, incols).value})
             # print(res_temp)
             res.append(res_temp)
     return res
 
 
-def excel_read_all_table(source_file):
-    try:
-        # >>读取数据【方式：一次性全部读取】------------------------------------------------------------
-        data = xlrd.open_workbook(source_file)  # 打开表
-        res = list()
-        # table = data.sheets()[0]  # 默认使用第一张表格
-        for table in data.sheets():
-            nrows = table.nrows  # 获取行数
-            ncols = table.ncols  # 获取列数
-            for inrows in range(nrows):
-                res_temp = dict()
-                for incols in range(ncols):
-                    res_temp.update({table.cell(0, incols).value: table.cell(inrows, incols).value})
-                # print(res_temp)
-                res.append(res_temp)
-        return res
-    except:
-        return
-
-
-def excel_sheet_dict(source_file):
-    try:
-        # >>读取数据【方式：一次性全部读取】------------------------------------------------------------
-        data = xlrd.open_workbook(source_file)  # 打开表
-        res = dict()
-        for table in data.sheets():
-            table_name = table.name
-            nrows = table.nrows  # 获取行数
-            ncols = table.ncols  # 获取列数
-            res_temp = list()
-            for inrows in range(nrows):
-                data_temp = dict()
-                for incols in range(ncols):
-                    data_temp.update({table.cell(0, incols).value: table.cell(inrows, incols).value})
-                res_temp.append(data_temp)
-            res.update({table_name: res_temp})
-        return res
-    except:
-        return
-
-
-def excel_specify_dict(source_file, sheet_name, _up_data_col_list=None, _col_dict=None):
-    try:
-        col_dict = dict()
-        if _col_dict is not None:
-            temp0 = _col_dict.replace(" ", "").split(",")
-            if temp0 is not None and len(temp0) > 0:
-                for each in temp0:
-                    temp1 = each.split(":")
-                    col_dict.update({temp1[1]: temp1[0]})
-        up_data_col_list = list()
-        if _up_data_col_list is not None:
-            up_data_col_list = _up_data_col_list.replace(" ", "").split(",")
-
-        # >>读取数据【方式：一次性全部读取】------------------------------------------------------------
-        data = xlrd.open_workbook(source_file)  # 打开表
-        res = dict()
-        for table in data.sheets():
-            table_name = table.name
-            if table_name == sheet_name:
-                nrows = table.nrows  # 获取行数
-                ncols = table.ncols  # 获取列数
-                res_temp = list()
-                for inrows in range(nrows):
-                    data_temp = dict()
-                    for incols in range(ncols):
-                        # print(table.cell(0, incols).value)
-                        col_name_ori = table.cell(0, incols).value
-                        if len(col_dict) > 0 and col_dict is not None:
-                            col_name = col_dict.get(col_name_ori)
-                        else:
-                            col_name = col_name_ori
-
-                        if col_name_ori in up_data_col_list:
-                            # print(col_name_ori)
-                            try:
-                                col_value = xlrd.xldate.xldate_as_datetime(table.cell(inrows, incols).value, 0)
-                            except Exception as ex:
-                                # print(ex)
-                                col_value = None
-                        else:
-                            col_value = table.cell(inrows, incols).value
-
-                        data_temp.update({col_name: col_value})
-                    res_temp.append(data_temp)
-                res.update({table_name: res_temp})
-        return res
-    except:
-        return
-
-
 def read_txt(text_name, path=None):
     try:
         if path is None:
             f = open("%s.txt" %text_name, encoding='utf-8')
         else:
             f = open("%s/%s.txt" % (path, text_name), encoding='utf-8')
         res = f.read()
@@ -490,38 +452,14 @@
     def default(self, obj):
         if isinstance(obj, datetime.datetime):
             return obj.strftime("%Y-%m-%d %H:%M:%S")
         else:
             return json.JSONEncoder.default(self, obj)
 
 
-def save(
-        file_name,
-        content,
-        postfix: str = "txt",
-        path=None,
-        overwrite=True
-):
-    """
-    增加自动创建目录功能
-    """
-    if overwrite is True:
-        write_mode = "w"  # 覆盖
-    else:
-        write_mode = "a"  # 追加
-
-    if path is None:
-        f = open("%s.%s" % (file_name, postfix), write_mode, encoding='utf-8')
-    else:
-        lazypath.make_path(path)
-        f = open("%s%s%s.%s" % (path, path_separator, file_name, postfix), write_mode, encoding='utf-8')
-    f.write(content)
-    f.close()
-
-
 def save_list(
         file_name,
         list_data,
         split_by='\n',
         postfix="txt",
         path=None,
         overwrite=False
@@ -529,15 +467,15 @@
     """
     将list按照行存储到文件中，对于datetime类型自动转换为日期时间的格式
     """
     if path is None:
         file_dir = "%s.%s" % (file_name, postfix)
     else:
         lazypath.make_path(path)
-        file_dir = "%s%s%s.%s" % (path, path_separator, file_name, postfix)
+        file_dir = os.path.join(path, f'{file_name}.{postfix}')
 
     if overwrite is True:
 
         write_mode = "w"  # 覆盖
     else:
         write_mode = "a"  # 追加
 
@@ -572,48 +510,178 @@
                 col_num += 1
             row_num += 1
 
         wb.save("%s/%s.xlsx" % (path, table_name))
         showlog.info("导出数据成功！共计%s条数据" % len(data))
 
 
-def save_txt(
-        text_name,
-        content,
-        path=None,
-        overwrite=True):
+def save_bytes(
+        bytes_content: bytes,
+        file: str
+):
     """
-    是否覆写看overwrite参数
-    设置自动创建目录
+    保存bytes为文件
     """
-    if overwrite is True:
-        mode = "w"
-    else:
-        mode = "a"
-
-    if path is None:
-        f = open("%s.txt" % text_name, mode, encoding='utf-8')
-    else:
-        lazypath.make_path(path)
-        f = open("%s%s%s.txt" % (path, path_separator, text_name), mode, encoding='utf-8')
-    f.write(content)
+    with open(file, 'wb') as f:
+        f.write(bytes_content)
     f.close()
+    return os.path.join(sys.path[0], file)
 
 
-def save_sql(
-        file_name,
-        content,
-        path=None
+def get_file_info(file_dir):
+    """
+    获取文件信息
+    """
+    from lazysdk import lazytime
+    file_path = os.path.dirname(file_dir)  # 获取文件路径
+    file_name = os.path.basename(file_dir)  # 获取不含路径信息的文件名
+    file_name_pure, file_suffix = os.path.splitext(file_name)  # 获取不含后缀名的文件名和后缀名
+    return {
+        'name': file_name,  # 获取不含路径信息的文件名
+        'path': file_path,
+        'pure_name': file_name_pure,
+        'suffix': file_suffix,
+        'size': get_file_size(file_dir=file_dir),
+        'create_timestamp': os.path.getctime(file_dir),
+        'create_time': lazytime.get_timestamp2datetime(os.path.getctime(file_dir)),
+        'modified_timestamp': os.path.getmtime(file_dir),
+        'modified_time': lazytime.get_timestamp2datetime(os.path.getmtime(file_dir)),
+    }
+
+
+def zip_file(
+        source_file: str,
+        zip_file: str = None
+) -> str:
+    """
+    压缩文件，此方法只适用于压缩单个文件，不适合压缩文件夹
+    """
+    import zipfile
+    file_path = os.path.dirname(source_file)
+    file_name = os.path.basename(source_file)
+    file_name_pure, file_suffix = os.path.splitext(file_name)
+    if not zip_file:
+        zip_file = os.path.join(file_path, f'{file_name_pure}.zip')
+    my_zip = zipfile.ZipFile(
+        file=zip_file,  # 打开一个对象，也就是目标文件名
+        mode='w'  # 写入模式
+    )
+    my_zip.write(
+        filename=source_file,  # 压缩目标文件路径
+        arcname=os.path.basename(source_file),  # 内部文件名
+        compress_type=zipfile.ZIP_DEFLATED
+    )
+    my_zip.close()
+    return zip_file
+
+
+def zip_path(
+        source_path
+) -> str:
+    """
+    压缩文件夹，并在原来的同级目录输出，返回zip文件路径
+    """
+    import shutil
+    return shutil.make_archive(
+        root_dir=source_path,
+        base_name=source_path,
+        format='zip'
+    )
+
+
+def make_zip(
+        file: str
+) -> str:
+    """
+    创建压缩文件，自动判断源是文件还是路径
+    """
+    if os.path.isdir(file):
+        return zip_path(file)
+    elif os.path.isfile(file):
+        return zip_file(file)
+    else:
+        return ''
+
+
+def unzip(
+        file
+) -> list:
+    """
+    解压文件，会在源文件的同级目录增加一个路径，以存放解压后的文件
+    返回的是一个已解压的所有文件路径的list
+    """
+    import zipfile
+    import locale
+    file_path = os.path.dirname(file)
+    file_name = os.path.basename(file)
+    file_name_pure, file_suffix = os.path.splitext(file_name)
+    encoding = locale.getpreferredencoding()
+    my_zip = zipfile.ZipFile(
+        file=file,
+        mode='r'
+    )
+    unzip_path = os.path.join(file_path, file_name_pure)
+    while True:
+        if os.path.exists(unzip_path):
+            unzip_path = f'{unzip_path}_unpack'
+        else:
+            break
+
+    # 生成一个源文件名对照正确文件名的字典
+    name_dict = dict()
+    for each in my_zip.filelist:
+        each_filename = copy.deepcopy(each.filename)
+        if each_filename[0:8] == '__MACOSX':
+            continue  # 屏蔽mac下的__MACOSX路径
+        else:
+            if each_filename.isascii():
+                pass   # 如果isascii=True，则不改编码
+            else:
+                try:
+                    each_filename = each_filename.encode('437').decode(encoding)  # 尝试使用437编码先解码，再编码
+                except:
+                    pass
+            name_dict[each.filename] = each_filename
+
+    unzip_names = list()
+    for each_name in my_zip.namelist():
+        new_name = name_dict.get(each_name)
+        if new_name:
+            new_name_dir = os.path.join(unzip_path, new_name)
+            extract_name = my_zip.extract(
+                member=each_name,
+                path=unzip_path
+            )
+            if extract_name == new_name_dir:
+                # print(extract_name)
+                pass
+            else:
+                # print(extract_name, '-->', new_name_dir)
+                os.renames(old=extract_name, new=new_name_dir)  # 对乱码文件名重命名
+                if os.path.isfile(new_name_dir):
+                    unzip_names.append(new_name_dir)
+        else:
+            continue
+    return unzip_names
+
+
+def get_stream(
+        url,
+        verify=True,
+        **kwargs
 ):
     """
-    如果文件存在，先清空，再保存
-    :param file_name:
-    :param content:
-    :param path:
-    :return:
+    以流式传输方式发起请求，适用于下载文件时，当文件过大，不会立即下载。
+    当把get函数的stream参数设置成True时，它不会立即开始下载，当你使用iter_content或iter_lines遍历内容或访问内容属性时才开始下载。需要注意一点：文件没有下载之前，它也需要保持连接。
+    iter_content：一块一块的遍历要下载的内容
+    iter_lines：一行一行的遍历要下载的内容
     """
-    if path is None:
-        f = open(file_name, "w", encoding='utf-8')
-    else:
-        f = open("%s%s%s.sql" % (path, path_separator, file_name), "w", encoding='utf-8')
-    f.write(content)
-    f.close()
+    try:
+        response = requests.get(
+            url=url,
+            verify=verify,
+            stream=True,
+            **kwargs
+        )
+    except exceptions.ConnectionError:
+        raise exceptions.ConnectionError(f"Could not reach host. Are you offline?")
+    return response
```

### Comparing `lazysdk-0.1.9/lazysdk/lazyflask.py` & `lazysdk-0.1.90/lazysdk/lazyflask.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.9/lazysdk/lazym3u8.py` & `lazysdk-0.1.90/lazysdk/lazym3u8.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,15 +653,15 @@
     if m3u8_link is None and m3u8_file_path is None:
         print(':( 请传入有效的m3u8地址！')
         return False
 
     if m3u8_file_path is not None:
         print("正在解析m3u8文件...")
         all_content = lazyfile.read(
-            file_name=m3u8_file_path,
+            file=m3u8_file_path,
             postfix=postfix
         )
         m3u8_lines = all_content.split("\n")  # 读取文件里的每一行
     else:
         return False
 
     # 通过判断文件头来确定是否是M3U8文件
@@ -729,17 +729,17 @@
     # -------------------- 获取m3u8内容 --------------------
     if m3u8_url is None:
         if m3u8_file_dir is None:
             if m3u8_content is None:
                 return False
             else:
                 lazyfile.save(
-                    file_name=temp_filename,
+                    file=temp_filename,
                     content=m3u8_content,
-                    postfix="m3u8",
+                    suffix="m3u8",
                     path=video_save_path,
                     overwrite=overwrite
                 )
                 if video_save_path is None:
                     m3u8_file_dir_name = '%s.m3u8' % temp_filename
                 else:
                     m3u8_file_path = r'%s%s%s' % (video_save_path, path_separator, temp_filename)
@@ -747,17 +747,17 @@
         else:
             m3u8_file_dir_name = m3u8_file_dir  # 完整路径
     else:
         try:
             m3u8_file = m3u8_file_maker(m3u8_url=m3u8_url)
             print(':) 获取m3u8内容成功')
             lazyfile.save(
-                file_name=temp_filename,
+                file=temp_filename,
                 content=m3u8_file,
-                postfix="m3u8",
+                suffix="m3u8",
                 path=video_save_path,
                 overwrite=overwrite
             )
             if video_save_path is None:
                 m3u8_file_dir_name = '%s.m3u8' % (temp_filename)
             else:
                 m3u8_file_path = r'%s%s%s' % (video_save_path, path_separator, temp_filename)
```

### Comparing `lazysdk-0.1.9/lazysdk/lazymd5.py` & `lazysdk-0.1.90/lazysdk/lazymd5.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.9/lazysdk/lazyproxies.py` & `lazysdk-0.1.90/lazysdk/lazyproxies.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.9/lazysdk/lazyrandom.py` & `lazysdk-0.1.90/lazysdk/lazyrandom.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # coding = utf8
 """
 @ Author : ZeroSeeker
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
-from numpy import random as np_random
 import string
 import random
 
 
 def random_str(
         str_length: int = 8,
         ascii_lowercase: bool = True,  # 小写字母
@@ -29,23 +28,24 @@
     random_sample = ""
     if ascii_lowercase is True:
         random_sample += string.ascii_lowercase
     if ascii_uppercase is True:
         random_sample += string.ascii_uppercase
     if numbers is True:
         random_sample += string.digits
-    random_sample_list = list(random_sample)
     if repeat:
-        value = ''.join(np_random.choice(
-            a=random_sample_list,
-            size=str_length,
-            replace=True
-        )
-        )  # 可重复采样
+        # 可重复采样
+        value = ''
+        for _ in range(str_length):
+            value += random.sample(
+                random_sample,
+                1
+            )[0]
     else:
+        # 不重复采样
         value = ''.join(
             random.sample(
                 random_sample,
                 str_length
             )
-        )  # 不重复采样
+        )
     return value
```

### Comparing `lazysdk-0.1.9/lazysdk/lazyredis.py` & `lazysdk-0.1.90/lazysdk/lazyredis.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.9/lazysdk/lazytime.py` & `lazysdk-0.1.90/lazysdk/lazytime.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,36 @@
 # coding = utf8
 """
 @ Author : ZeroSeeker
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
+import requests
 import datetime
 import pytz
 import time
 import copy
 import sys
+import re
+
+
+def get_datetime_from_str(
+        string: str
+):
+    """
+    从字符串中识别出时间
+    目前这个模块还不完备
+    """
+    findres = dict()
+    find_datetime = re.findall(pattern=r'(\d\d\d\d-[0-1]\d-[0-3]\d [0-2]\d:[0-5]\d:[0-5]\d)', string=string)
+    findres['datetime'] = find_datetime
+    find_time = re.findall(pattern=r'([0-2]\d:[0-5]\d:[0-5]\d)', string=string)
+    findres['time'] = find_time
+    return findres
 
 
 def get_utc_datetime(
         f: str = '%Y-%m-%dT%H:%M:%SZ'
 ):
     """
     获取utc时间
@@ -91,21 +108,32 @@
         date = str(date_input)
         a1 = date.find(date_delimiter, 0)
         a2 = date.find(date_delimiter, a1 + 1)
         day = int(date[a2 + 1:len(date)])
     return day
 
 
-def get_hour():
+def get_hour(
+        target=None
+) -> int:
     """
     获取当前系统的当前时间：小时数（24小时制）
     :return: 14
     """
-    hour = datetime.datetime.now().hour
-    return hour
+    if not target:
+        return datetime.datetime.now().hour
+    else:
+        if isinstance(target, datetime.datetime):
+            return target.hour
+        elif isinstance(target, str):
+            get_res = get_datetime_from_str(string=target)
+            if get_res.get("time"):
+                return int(get_res.get("time")[0].split(':')[0])
+        else:
+            return -1
 
 
 def get_minute():
     """
     获取当前系统的当前时间：分钟数
     :return: 28
     """
@@ -324,19 +352,29 @@
 ):
     time_array = time.strptime(data, f)
     timestamp = int(time.mktime(time_array))
     return timestamp
 
 
 def get_datetime2date(
-        datetime_str: str
-):
-    datetime_timestamp = get_datetime2timestamp(datetime_str)
-    date_str = get_timestamp2date(datetime_timestamp)
-    return date_str
+        datetime_str,
+        f: str = '%Y-%m-%d'
+) -> str:
+    """
+    datetime->date
+    """
+    temp = copy.deepcopy(datetime_str)  # 复制一份防止发生更改
+    if isinstance(temp, str):
+        datetime_timestamp = get_datetime2timestamp(temp)
+        date_str = get_timestamp2date(datetime_timestamp)
+        return date_str
+    elif isinstance(temp, datetime.datetime):
+        return temp.strftime(f)
+    else:
+        return temp
 
 
 def timestamp_day_num_start(
         num: int = 0
 ):
     """
     换算出相对时间的当日开始时间的时间戳
@@ -578,20 +616,36 @@
         f: str = '%Y年%m月%d日%H时%M分%S秒'
 ):
     time_string_in = date.strftime(f)
     return time_string_in
 
 
 def date_str_list(
-        start_date: str,
-        end_date: str
+        start_date: str = None,
+        end_date: str = None,
+        start_days: int = None,
+        end_days: int = None
 ):
     # 生成起止时间之间的时间序列
-    start_date_f = get_format_date(start_date)
-    end_date_f = get_format_date(end_date)
+    current_day = datetime.date.today()
+
+    if start_date:
+        start_date_f = get_format_date(start_date)
+    elif start_days:
+        start_date_f = current_day + datetime.timedelta(days=start_days)
+    else:
+        start_date_f = current_day
+
+    if end_date:
+        end_date_f = get_format_date(end_date)
+    elif end_days:
+        end_date_f = current_day + datetime.timedelta(days=end_days)
+    else:
+        end_date_f = current_day
+    # print(start_date_f, '-->', end_date_f)
     date_list = list()
     date_list.append(str(start_date_f))
     added_date = start_date_f
     while True:
         added_date = get_add_date(added_date, 1)
         added_date_f = get_format_date(added_date)
         if added_date_f > end_date_f:
@@ -860,7 +914,74 @@
     """
     计算两个日期之间相差的天数
     """
     date1_date = datetime.datetime.strptime(date1, data1_f).date()
     date2_date = datetime.datetime.strptime(date2, data2_f).date()
     days = (date2_date - date1_date).days
     return days
+
+
+def time_limit(
+        end_datetime: str
+):
+    """
+    时间限制
+    截止时间例如：2023-07-01 12:00:00
+    """
+    url = 'http://api.m.taobao.com/rest/api3.do?api=mtop.common.getTimestamp'  # 网络取时
+    res = requests.get(url=url)
+    net_t = res.json()['data']['t']
+    end_date_t = get_datetime2timestamp(end_datetime)
+    if end_date_t * 1000 > int(net_t):
+        seconds_left = end_date_t - int(net_t)/1000
+        print(f'剩余有效时长：{format_seconds(int(seconds_left))}')
+        return
+    else:
+        while True:
+            print('软件已失效，请联系开发者～')
+            time.sleep(1)
+
+
+def wait_hour(
+        hour: int,
+        sleep=0.01
+):
+    """
+    等待 小时整点，如果当前时间是指定的小时，将退出，否则将持续等待
+    hour为0-24的整数
+    sleep为等待检查的间隔时间
+    """
+    while True:
+        if datetime.datetime.now().hour == hour:
+            break
+        else:
+            time.sleep(sleep)
+
+
+def get_weekday():
+    """
+    获取当前时间的星期序列，星期1为1，星期日为7
+    """
+    return datetime.datetime.now().weekday() + 1
+
+
+def get_recent_days_date(
+        num_start: int = -1,
+        num_end: int = 0
+) -> list:
+    """
+    获取指定前推天数的日期列表
+    """
+    return date_str_list(
+        start_date=get_date_string(days=num_start),
+        end_date=get_date_string(days=num_end)
+    )
+
+
+def network_timestamp():
+    """
+    获取网络时间，精确到毫秒
+    """
+    url = 'https://api.m.taobao.com/rest/api3.do?api=mtop.common.getTimestamp'  # 淘宝网络取时
+    res = requests.get(url=url)
+    net_t = res.json()['data']['t']  # 精确到毫秒的时间戳
+    return int(net_t)
```

### Comparing `lazysdk-0.1.9/lazysdk/lazyua.py` & `lazysdk-0.1.90/lazysdk/lazyua.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 @ Author : ZeroSeeker
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
 from ua_parser import user_agent_parser
+from user_agents import parse
 ua_match_ignore_values = ['Other', None]
 
 
 def dict_values_match(
         dict_a: dict,
         dict_b: dict,
         ignore_values: list = None  # 忽略值，例如：['Other', None]
@@ -115,7 +116,39 @@
         for each_match_res in match_res:
             count_all += each_match_res.get('count_all')
             count_match += each_match_res.get('count_match')
         if count_all == 0:
             return 0
         else:
             return count_match/count_all
+
+
+def ua_match(
+        ua1: str,
+        ua2: str,
+        match_os: bool = True,
+        match_device: bool = True
+):
+    """
+    按照os和device匹配信息，匹配成功返回True，匹配失败返回False
+    """
+    user_agent1 = parse(ua1)
+    user_agent2 = parse(ua2)
+    user_agent1_os = user_agent1.os
+    user_agent1_device = user_agent1.device
+    user_agent2_os = user_agent2.os
+    user_agent2_device = user_agent2.device
+    if match_os and match_device:
+        user_agent1_str = str(user_agent1_os) + str(user_agent1_device)
+        user_agent2_str = str(user_agent2_os) + str(user_agent2_device)
+    elif match_os and not match_device:
+        user_agent1_str = str(user_agent1_os)
+        user_agent2_str = str(user_agent2_os)
+    elif not match_os and match_device:
+        user_agent1_str = str(user_agent1_device)
+        user_agent2_str = str(user_agent2_device)
+    else:
+        return False
+    if user_agent1_str == user_agent2_str:
+        return True
+    else:
+        return False
```

### Comparing `lazysdk-0.1.9/lazysdk/lazywebhook.py` & `lazysdk-0.1.90/lazysdk/lazywebhook.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.9/lazysdk.egg-info/SOURCES.txt` & `lazysdk-0.1.90/lazysdk.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,42 @@
+LICENSE
 README.md
 setup.py
 lazysdk/__init__.py
 lazysdk/lazyCrypto.py
+lazysdk/lazy_id_card.py
 lazysdk/lazybase64.py
+lazysdk/lazycache.py
+lazysdk/lazychromedriver.py
+lazysdk/lazydecode.py
 lazysdk/lazydict.py
 lazysdk/lazyenv.py
 lazysdk/lazyexcel.py
 lazysdk/lazyfile.py
 lazysdk/lazyflask.py
+lazysdk/lazyhtml.py
 lazysdk/lazyid.py
+lazysdk/lazyinfo.py
 lazysdk/lazyip.py
+lazysdk/lazyjson.py
+lazysdk/lazylist.py
 lazysdk/lazym3u8.py
 lazysdk/lazymd5.py
 lazysdk/lazypath.py
 lazysdk/lazyprocess.py
 lazysdk/lazyproxies.py
 lazysdk/lazyrandom.py
 lazysdk/lazyredis.py
 lazysdk/lazyrequests.py
 lazysdk/lazytext.py
 lazysdk/lazytime.py
 lazysdk/lazyua.py
+lazysdk/lazyurl.py
 lazysdk/lazywebhook.py
+lazysdk/lazywifi.py
+lazysdk/lazyxml.py
+lazysdk/showdata.py
 lazysdk.egg-info/PKG-INFO
 lazysdk.egg-info/SOURCES.txt
 lazysdk.egg-info/dependency_links.txt
 lazysdk.egg-info/requires.txt
 lazysdk.egg-info/top_level.txt
```

### Comparing `lazysdk-0.1.9/setup.py` & `lazysdk-0.1.90/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,34 +9,37 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazysdk",
-    version="0.1.9",
+    version="0.1.90",
     description="基于Python的懒人包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazysdk",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'showlog>=0.0.6',
-        'requests==2.27.1',
+        'requests>=2.31.0',
         'envx>=1.0.1',
         'pytz==2022.1',
-        'redis==4.1.0',
         'ua_parser==0.10.0',
         'openpyxl==3.0.9',
         'xlrd==2.0.1',
-        'numpy==1.22.0',
         'm3u8==3.5.0',
-        'pycryptodome==3.10.1'
+        'pycryptodome==3.10.1',
+        'filetype==1.2.0',
+        'netifaces==0.11.0',
+        'user_agents==2.2.0',
+        'rich>=13.5.2',
+        'urllib3==1.23'
     ]
 )
```

