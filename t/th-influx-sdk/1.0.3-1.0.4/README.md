# Comparing `tmp/th-influx-sdk-1.0.3.tar.gz` & `tmp/th-influx-sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th-influx-sdk-1.0.3.tar", last modified: Tue Apr 23 01:28:43 2024, max compression
+gzip compressed data, was "th-influx-sdk-1.0.4.tar", last modified: Wed Apr 24 06:21:40 2024, max compression
```

## Comparing `th-influx-sdk-1.0.3.tar` & `th-influx-sdk-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 01:28:43.624300 th-influx-sdk-1.0.3/
--rw-rw-rw-   0        0        0      300 2024-04-23 01:28:43.622306 th-influx-sdk-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 01:28:43.611364 th-influx-sdk-1.0.3/ThInfluxSDK/
--rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.3/ThInfluxSDK/__init__.py
--rw-rw-rw-   0        0        0    18398 2024-04-23 01:19:12.000000 th-influx-sdk-1.0.3/ThInfluxSDK/influxSDK.py
--rw-rw-rw-   0        0        0       42 2024-04-23 01:28:43.624300 th-influx-sdk-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-23 01:26:03.000000 th-influx-sdk-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 01:28:43.620347 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/
--rw-rw-rw-   0        0        0      300 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-23 01:28:43.000000 th-influx-sdk-1.0.3/th_influx_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 06:21:40.040710 th-influx-sdk-1.0.4/
+-rw-rw-rw-   0        0        0      300 2024-04-24 06:21:40.039757 th-influx-sdk-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 06:21:40.027062 th-influx-sdk-1.0.4/ThInfluxSDK/
+-rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.4/ThInfluxSDK/__init__.py
+-rw-rw-rw-   0        0        0    17760 2024-04-24 06:19:37.000000 th-influx-sdk-1.0.4/ThInfluxSDK/influxSDK.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 06:21:40.040710 th-influx-sdk-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      553 2024-04-24 06:21:35.000000 th-influx-sdk-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:21:40.037692 th-influx-sdk-1.0.4/th_influx_sdk.egg-info/
+-rw-rw-rw-   0        0        0      300 2024-04-24 06:21:39.000000 th-influx-sdk-1.0.4/th_influx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-24 06:21:39.000000 th-influx-sdk-1.0.4/th_influx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 06:21:39.000000 th-influx-sdk-1.0.4/th_influx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-24 06:21:39.000000 th-influx-sdk-1.0.4/th_influx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 06:21:39.000000 th-influx-sdk-1.0.4/th_influx_sdk.egg-info/top_level.txt
```

### Comparing `th-influx-sdk-1.0.3/ThInfluxSDK/influxSDK.py` & `th-influx-sdk-1.0.4/ThInfluxSDK/influxSDK.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,41 +419,26 @@
                 SQLForHisDate += f"and time>='{startTime_temp}' and time<='{endTime_temp}'"
                 time_list = get_time_list(utc_get_time(startTime_temp), utc_get_time(endTime_temp), interval)
             SQLForHisDate += f"group by UUID, time({interval}s) fill(previous)"
             data_map = get_new_data_map(database, tableName, startTime_temp, pointList, influxDB)
             result = influxDB.query(SQLForHisDate, database=database)
 
             result_value_map = OrderedDict()
+            for series in result.raw['series']:
+                result_value_map[series['tags']['UUID']] = series['values']
 
-            # 处理查询结果并构建 result_value_map
-            obj_List_list = []
-            for point in result.get_points():
-                time = point['time']
-                uuid = point['UUID']
-                last = point['last']
-                obj_List = [time, uuid, last]
-                obj_List_list.append(obj_List)
-            # print(json.dumps(obj_List_list))
-            # 根据 uuid 对数据进行排序
-            obj_List_list.sort(key=itemgetter(1))
-
-            # 使用 groupby 将数据按照 uuid 分组
-            grouped_data = groupby(obj_List_list, key=itemgetter(1))
-
-            # 将分组后的数据转换成字典
-            result_value_map = {uuid: list(items) for uuid, items in grouped_data}
             # 遍历时间列表并构建CSV记录
             index = 0
             for time_stamp in time_list:
                 record = [time_stamp]  # 添加时间戳
                 for point in pointList:
                     values_list = result_value_map.get(point)
-                    if values_list and values_list[index][2]:
+                    if values_list and values_list[index][1]:
                         # 假设 values_list 是一个包含时间戳和值的元组列表
-                        record.append(values_list[index][2])
+                        record.append(values_list[index][1])
                     elif point in data_map:
                         record.append(data_map[point])
                     else:
                         record.append('')
 
                         # 写入CSV记录
                 csv_writer.writerow(record)
```

### Comparing `th-influx-sdk-1.0.3/setup.py` & `th-influx-sdk-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name='th-influx-sdk',
-    version='1.0.3',
+    version='1.0.4',
     description='A SDK for influxDb',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='xiongyi',
     author_email='15679191752@163.com',
     packages=find_packages(),
     install_requires=[
```

