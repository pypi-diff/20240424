# Comparing `tmp/ldjcourse-0.0.7.8.tar.gz` & `tmp/ldjcourse-0.0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ldjcourse-0.0.7.8.tar", last modified: Mon Apr 22 13:25:44 2024, max compression
+gzip compressed data, was "dist\ldjcourse-0.0.7.9.tar", last modified: Mon Apr 22 13:36:55 2024, max compression
```

## Comparing `ldjcourse-0.0.7.8.tar` & `ldjcourse-0.0.7.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 13:25:44.450794 ldjcourse-0.0.7.8/
--rw-rw-rw-   0        0        0      168 2024-04-22 13:25:44.443651 ldjcourse-0.0.7.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 13:25:44.342480 ldjcourse-0.0.7.8/ldjcourse/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.7.8/ldjcourse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:25:44.372697 ldjcourse-0.0.7.8/ldjcourse/pandas/
--rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.7.8/ldjcourse/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:25:44.420070 ldjcourse-0.0.7.8/ldjcourse/pandas/v1_1/
--rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.7.8/ldjcourse/pandas/v1_1/__init__.py
--rw-rw-rw-   0        0        0     1145 2024-04-21 15:59:16.000000 ldjcourse-0.0.7.8/ldjcourse/pandas/v1_1/api.py
--rw-rw-rw-   0        0        0     3497 2024-04-22 13:25:42.000000 ldjcourse-0.0.7.8/ldjcourse/pandas/v1_1/data.py
--rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.7.8/ldjcourse/pandas/v1_1/setting.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:25:44.435743 ldjcourse-0.0.7.8/ldjcourse.egg-info/
--rw-rw-rw-   0        0        0      168 2024-04-22 13:25:44.000000 ldjcourse-0.0.7.8/ldjcourse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-22 13:25:44.000000 ldjcourse-0.0.7.8/ldjcourse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 13:25:44.000000 ldjcourse-0.0.7.8/ldjcourse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-22 13:25:44.000000 ldjcourse-0.0.7.8/ldjcourse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 13:25:44.451765 ldjcourse-0.0.7.8/setup.cfg
--rw-rw-rw-   0        0        0      584 2024-04-22 13:25:42.000000 ldjcourse-0.0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 13:36:55.214674 ldjcourse-0.0.7.9/
+-rw-rw-rw-   0        0        0      168 2024-04-22 13:36:55.207862 ldjcourse-0.0.7.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 13:36:55.120235 ldjcourse-0.0.7.9/ldjcourse/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:24:13.000000 ldjcourse-0.0.7.9/ldjcourse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 13:36:55.150092 ldjcourse-0.0.7.9/ldjcourse/pandas/
+-rw-rw-rw-   0        0        0        0 2024-04-20 04:41:18.000000 ldjcourse-0.0.7.9/ldjcourse/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 13:36:55.186555 ldjcourse-0.0.7.9/ldjcourse/pandas/v1_1/
+-rw-rw-rw-   0        0        0        0 2024-04-06 11:25:30.000000 ldjcourse-0.0.7.9/ldjcourse/pandas/v1_1/__init__.py
+-rw-rw-rw-   0        0        0     1145 2024-04-21 15:59:16.000000 ldjcourse-0.0.7.9/ldjcourse/pandas/v1_1/api.py
+-rw-rw-rw-   0        0        0     3497 2024-04-22 13:36:53.000000 ldjcourse-0.0.7.9/ldjcourse/pandas/v1_1/data.py
+-rw-rw-rw-   0        0        0       22 2024-04-20 04:51:34.000000 ldjcourse-0.0.7.9/ldjcourse/pandas/v1_1/setting.py
+drwxrwxrwx   0        0        0        0 2024-04-22 13:36:55.199586 ldjcourse-0.0.7.9/ldjcourse.egg-info/
+-rw-rw-rw-   0        0        0      168 2024-04-22 13:36:54.000000 ldjcourse-0.0.7.9/ldjcourse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-22 13:36:54.000000 ldjcourse-0.0.7.9/ldjcourse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 13:36:54.000000 ldjcourse-0.0.7.9/ldjcourse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-22 13:36:54.000000 ldjcourse-0.0.7.9/ldjcourse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 13:36:55.215520 ldjcourse-0.0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0      584 2024-04-22 13:36:53.000000 ldjcourse-0.0.7.9/setup.py
```

### Comparing `ldjcourse-0.0.7.8/ldjcourse/pandas/v1_1/api.py` & `ldjcourse-0.0.7.9/ldjcourse/pandas/v1_1/api.py`

 * *Files identical despite different names*

### Comparing `ldjcourse-0.0.7.8/ldjcourse/pandas/v1_1/data.py` & `ldjcourse-0.0.7.9/ldjcourse/pandas/v1_1/data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -49,20 +49,20 @@
 
 def data3():
     # 定义行索引
     index = ['01', '02', '03']
 
     # 定义多级列索引
     columns = [
-        ('var1', 'before', 2),
         ('var1', 'before', 1),
+        ('var1', 'before', 2),
         ('var1', 'post', 1),
         ('var1', 'post', 2),
-        ('var2', 'before', 2),
         ('var2', 'before', 1),
+        ('var2', 'before', 2),
         ('var2', 'post', 1),
         ('var2', 'post', 2),
     ]
     names = ['var', 'stage1', 'stage2']
     columns = pd.MultiIndex.from_tuples(columns, names=names)
 
     # 定义数据
```

### Comparing `ldjcourse-0.0.7.8/setup.py` & `ldjcourse-0.0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7.8'
+VERSION = '0.0.7.9'
 
 setup(
     name='ldjcourse',
     version=VERSION,
     author='元蓝先生',
     description='B站：元蓝先生 https://space.bilibili.com/3546564903569609',
     license='MIT',
```

