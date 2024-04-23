# Comparing `tmp/pc-perf-1.1.2.tar.gz` & `tmp/pc-perf-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pc-perf-1.1.2.tar", last modified: Sun Apr 21 15:27:12 2024, max compression
+gzip compressed data, was "pc-perf-1.1.3.tar", last modified: Tue Apr 23 22:42:58 2024, max compression
```

## Comparing `pc-perf-1.1.2.tar` & `pc-perf-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:27:12.320232 pc-perf-1.1.2/
--rw-rw-rw-   0        0        0    35823 2024-04-20 15:52:03.000000 pc-perf-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      943 2024-04-21 15:27:12.319230 pc-perf-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      341 2024-04-20 17:44:37.000000 pc-perf-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 15:27:12.308587 pc-perf-1.1.2/core/
--rw-rw-rw-   0        0        0     2447 2024-04-06 12:27:42.000000 pc-perf-1.1.2/core/monitor.py
--rw-rw-rw-   0        0        0     9574 2024-04-21 07:07:46.000000 pc-perf-1.1.2/core/pc_tools.py
--rw-rw-rw-   0        0        0     6709 2024-04-21 07:37:00.000000 pc-perf-1.1.2/dao.py
--rw-rw-rw-   0        0        0      664 2024-04-21 15:03:50.000000 pc-perf-1.1.2/log.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:27:12.319230 pc-perf-1.1.2/pc_perf.egg-info/
--rw-rw-rw-   0        0        0      943 2024-04-21 15:27:12.000000 pc-perf-1.1.2/pc_perf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-04-21 15:27:12.000000 pc-perf-1.1.2/pc_perf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:27:12.000000 pc-perf-1.1.2/pc_perf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-21 15:27:12.000000 pc-perf-1.1.2/pc_perf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      240 2024-04-21 15:27:12.000000 pc-perf-1.1.2/pc_perf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-04-21 15:27:12.000000 pc-perf-1.1.2/pc_perf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4156 2024-04-21 15:05:37.000000 pc-perf-1.1.2/pc_perf.py
--rw-rw-rw-   0        0        0       42 2024-04-21 15:27:12.320232 pc-perf-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2624 2024-04-21 15:27:10.000000 pc-perf-1.1.2/setup.py
--rw-rw-rw-   0        0        0     1545 2024-04-20 11:36:25.000000 pc-perf-1.1.2/task_handle.py
--rw-rw-rw-   0        0        0     2879 2024-04-21 15:04:24.000000 pc-perf-1.1.2/util.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:42:58.734708 pc-perf-1.1.3/
+-rw-rw-rw-   0        0        0    35823 2024-04-20 15:52:03.000000 pc-perf-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      943 2024-04-23 22:42:58.733709 pc-perf-1.1.3/PKG-INFO
+-rwxrwxrwx   0        0        0   377856 2024-01-28 09:39:06.000000 pc-perf-1.1.3/PresentMon.exe
+-rw-rw-rw-   0        0        0      341 2024-04-20 17:44:37.000000 pc-perf-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 22:42:58.706132 pc-perf-1.1.3/core/
+-rw-rw-rw-   0        0        0     2447 2024-04-06 12:27:42.000000 pc-perf-1.1.3/core/monitor.py
+-rw-rw-rw-   0        0        0     9574 2024-04-21 07:07:46.000000 pc-perf-1.1.3/core/pc_tools.py
+-rw-rw-rw-   0        0        0     6709 2024-04-21 07:37:00.000000 pc-perf-1.1.3/dao.py
+-rw-rw-rw-   0        0        0      664 2024-04-21 15:03:50.000000 pc-perf-1.1.3/log.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:42:58.732708 pc-perf-1.1.3/pc_perf.egg-info/
+-rw-rw-rw-   0        0        0      943 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      240 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-23 22:42:58.000000 pc-perf-1.1.3/pc_perf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4156 2024-04-21 15:05:37.000000 pc-perf-1.1.3/pc_perf.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 22:42:58.734708 pc-perf-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2591 2024-04-23 22:42:38.000000 pc-perf-1.1.3/setup.py
+-rw-rw-rw-   0        0        0     1545 2024-04-20 11:36:25.000000 pc-perf-1.1.3/task_handle.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:42:58.706132 pc-perf-1.1.3/test_result/
+-rw-rw-rw-   0        0        0    30322 2024-04-20 11:36:25.000000 pc-perf-1.1.3/test_result/index.html
+-rw-rw-rw-   0        0        0     2879 2024-04-21 15:04:24.000000 pc-perf-1.1.3/util.py
```

### Comparing `pc-perf-1.1.2/LICENSE` & `pc-perf-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.2/PKG-INFO` & `pc-perf-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pc-perf
-Version: 1.1.2
+Version: 1.1.3
 Summary: pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
 Home-page: https://github.com/15525730080/pc_perf
 Author: 范博洲
 Author-email: 15525730080@163.com
 License: MIT
 Keywords: pc fps cpu memory gpu monitor
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pc-perf-1.1.2/core/monitor.py` & `pc-perf-1.1.3/core/monitor.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.2/core/pc_tools.py` & `pc-perf-1.1.3/core/pc_tools.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.2/dao.py` & `pc-perf-1.1.3/dao.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.2/log.py` & `pc-perf-1.1.3/log.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.2/pc_perf.egg-info/PKG-INFO` & `pc-perf-1.1.3/pc_perf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pc-perf
-Version: 1.1.2
+Version: 1.1.3
 Summary: pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示
 Home-page: https://github.com/15525730080/pc_perf
 Author: 范博洲
 Author-email: 15525730080@163.com
 License: MIT
 Keywords: pc fps cpu memory gpu monitor
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pc-perf-1.1.2/pc_perf.py` & `pc-perf-1.1.3/pc_perf.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.2/setup.py` & `pc-perf-1.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 setup(
     # 包的名称，通常与包的目录名称相同
     name='pc-perf',
 
     # 版本号，遵循语义化版本控制规则
-    version='1.1.2',
+    version='1.1.3',
 
     # 项目简短描述
     description='pc 进程性能测试平台，支持 windows / mac / linux 平台进程cpu、memory、fps（仅支持windows下OpenGL  DirectX 引擎应用）、gpu、thread_num、handle_num 等指标的实时监控和可视化展示',
 
     # 项目的URL，通常是项目主页或源代码仓库
     url='https://github.com/15525730080/pc_perf',
 
@@ -49,15 +49,15 @@
     
     # 包含数据文件，比如配置文件
     include_package_data=True,
 
     # 定义包中非.py文件的内容
     package_data={
         # 如果你的包中有数据文件，可以在这里指定
-        '': ['*.exe', 'test_result/*.html'],  # 举例：包含所有dat和md文件
+        '': ['../*.exe', '../test_result/*.html'],
     },
 
     # 指定Python版本要求
     python_requires='>=3.9',
 
     # # 指定包的入口点，用于命令行工具
     entry_points={
```

### Comparing `pc-perf-1.1.2/task_handle.py` & `pc-perf-1.1.3/task_handle.py`

 * *Files identical despite different names*

### Comparing `pc-perf-1.1.2/util.py` & `pc-perf-1.1.3/util.py`

 * *Files identical despite different names*

