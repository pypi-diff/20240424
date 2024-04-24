# Comparing `tmp/mysql_server_has_gone-2.0.3.tar.gz` & `tmp/mysql_server_has_gone-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_server_has_gone-2.0.3.tar", last modified: Wed Apr 24 06:52:30 2024, max compression
+gzip compressed data, was "mysql_server_has_gone-2.0.4.tar", last modified: Wed Apr 24 07:02:57 2024, max compression
```

## Comparing `mysql_server_has_gone-2.0.3.tar` & `mysql_server_has_gone-2.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 06:52:30.056816 mysql_server_has_gone-2.0.3/
--rw-rw-rw-   0        0        0     1082 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     1090 2024-04-24 06:52:30.055809 mysql_server_has_gone-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      750 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 06:52:30.054014 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/
--rw-rw-rw-   0        0        0     1090 2024-04-24 06:52:29.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-24 06:52:29.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 06:52:29.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-24 06:52:29.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 06:52:30.052797 mysql_server_has_gone-2.0.3/mysql_server_has_gone_away/
--rw-rw-rw-   0        0        0        0 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone_away/__init__.py
--rw-rw-rw-   0        0        0     2491 2024-04-24 06:51:45.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone_away/base.py
--rw-rw-rw-   0        0        0       42 2024-04-24 06:52:30.057819 mysql_server_has_gone-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-04-24 06:47:40.000000 mysql_server_has_gone-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 07:02:57.662831 mysql_server_has_gone-2.0.4/
+-rw-rw-rw-   0        0        0     1082 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1437 2024-04-24 07:02:57.661831 mysql_server_has_gone-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1097 2024-04-24 07:02:46.000000 mysql_server_has_gone-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 07:02:57.660831 mysql_server_has_gone-2.0.4/mysql_server_has_gone.egg-info/
+-rw-rw-rw-   0        0        0     1437 2024-04-24 07:02:57.000000 mysql_server_has_gone-2.0.4/mysql_server_has_gone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-24 07:02:57.000000 mysql_server_has_gone-2.0.4/mysql_server_has_gone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 07:02:57.000000 mysql_server_has_gone-2.0.4/mysql_server_has_gone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-24 07:02:57.000000 mysql_server_has_gone-2.0.4/mysql_server_has_gone.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 07:02:57.659827 mysql_server_has_gone-2.0.4/mysql_server_has_gone_away/
+-rw-rw-rw-   0        0        0        0 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.4/mysql_server_has_gone_away/__init__.py
+-rw-rw-rw-   0        0        0     2491 2024-04-24 06:51:45.000000 mysql_server_has_gone-2.0.4/mysql_server_has_gone_away/base.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 07:02:57.662831 mysql_server_has_gone-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      544 2024-04-24 06:57:27.000000 mysql_server_has_gone-2.0.4/setup.py
```

### Comparing `mysql_server_has_gone-2.0.3/LICENSE` & `mysql_server_has_gone-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_server_has_gone-2.0.3/PKG-INFO` & `mysql_server_has_gone-2.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-Metadata-Version: 2.1
-Name: mysql_server_has_gone
-Version: 2.0.3
-Summary: Django myslq backend that fixes issue with long living connection
-Home-page: https://github.com/maiyajj/MySQL-server-has-gone-away
-Author: maiyajj
-Author-email: 1045373828@qq.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# 基于下面库进行优化，主要适配Django==5.0.3以后的版本。修复原子事务报错的问题
+
+安装：`pip install mysql_server_has_gone`
+因为代码里用到了MySQLdb库，所以需要安装mysqlclient。如果你用到了其他库导致报错，可以github上滴滴我，我会及时修复的。
+
+以下是原始文档：
 
 # MySQL-server-has-gone-away
 
 This repository solves issue where database connection inside of django overlives MySQL database connection timeout specified in `/etc/my.cnf` `wait_timeout = xxxx`. [See this issue](https://stackoverflow.com/questions/26958592/django-after-upgrade-mysql-server-has-gone-away)
 
 
 ## How to use:
 1. For Django 1.x and 2.x use `pip install mysql_server_has_gone_away==1.0.0`
 
-1. For django 3.x use `pip install mysql_server_has_gone_away==2.0.0`
+1. For django 3.x use `pip install mysql_server_has_gone==2.0.0`
 
 1. Put this engine into Django `settings.py`:
 
 ```python
 DATABASES = {
 	'default': {
 		'ENGINE': 'mysql_server_has_gone_away',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mysql_server_has_gone-2.0.3/mysql_server_has_gone_away/base.py` & `mysql_server_has_gone-2.0.4/mysql_server_has_gone_away/base.py`

 * *Files identical despite different names*

### Comparing `mysql_server_has_gone-2.0.3/setup.py` & `mysql_server_has_gone-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mysql_server_has_gone",
-    version="2.0.3",
+    version="2.0.4",
     description="Django myslq backend that fixes issue with long living connection",
     author="maiyajj",
     author_email="1045373828@qq.com",
     license="MIT",
     url="https://github.com/maiyajj/MySQL-server-has-gone-away",
     long_description=long_description,
     packages=find_packages(),
```

