# Comparing `tmp/movoid_robotframework-1.3.2.tar.gz` & `tmp/movoid_robotframework-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework-1.3.2.tar", last modified: Sat Apr 20 15:08:25 2024, max compression
+gzip compressed data, was "movoid_robotframework-1.4.0.tar", last modified: Wed Apr 24 14:03:12 2024, max compression
```

## Comparing `movoid_robotframework-1.3.2.tar` & `movoid_robotframework-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:25.146665 movoid_robotframework-1.3.2/
--rw-rw-rw-   0        0        0      282 2024-04-20 15:08:25.145658 movoid_robotframework-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:25.136682 movoid_robotframework-1.3.2/RobotFrameworkBasic/
--rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:25.139284 movoid_robotframework-1.3.2/RobotFrameworkBasic/action/
--rw-rw-rw-   0        0        0      220 2024-02-20 17:40:03.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/action/__init__.py
--rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/action/calculate.py
--rw-rw-rw-   0        0        0     3715 2024-02-20 09:25:58.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/common.py
--rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/decorator.py
--rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/error.py
--rw-rw-rw-   0        0        0      260 2024-02-20 17:40:03.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/main.py
--rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.3.2/RobotFrameworkBasic/version.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:08:25.144652 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/
--rw-rw-rw-   0        0        0      282 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-20 15:08:25.000000 movoid_robotframework-1.3.2/movoid_robotframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:08:25.146665 movoid_robotframework-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      550 2024-04-20 15:07:13.000000 movoid_robotframework-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:03:12.981059 movoid_robotframework-1.4.0/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2024-04-24 14:03:12.979885 movoid_robotframework-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 14:03:12.966046 movoid_robotframework-1.4.0/RobotFrameworkBasic/
+-rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:03:12.969123 movoid_robotframework-1.4.0/RobotFrameworkBasic/action/
+-rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/action/__init__.py
+-rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/action/calculate.py
+-rw-rw-rw-   0        0        0     5494 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/action/config.py
+-rw-rw-rw-   0        0        0     4476 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/common.py
+-rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/decorator.py
+-rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/error.py
+-rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/main.py
+-rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.0/RobotFrameworkBasic/version.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:03:12.978876 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-24 14:03:12.000000 movoid_robotframework-1.4.0/movoid_robotframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:03:12.981059 movoid_robotframework-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      558 2024-04-24 13:51:26.000000 movoid_robotframework-1.4.0/setup.py
```

### Comparing `movoid_robotframework-1.3.2/RobotFrameworkBasic/action/calculate.py` & `movoid_robotframework-1.4.0/RobotFrameworkBasic/action/calculate.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.3.2/RobotFrameworkBasic/common.py` & `movoid_robotframework-1.4.0/RobotFrameworkBasic/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -104,7 +104,25 @@
         :param value: value to be set
         :return: None
         """
         ori_dict[key] = value
 
     def always_true(self):
         return True
+
+    @robot_log_keyword
+    def get_suite_case_str(self, join_str: str = '-', suite: bool = True, case: bool = True):
+        """
+        获取当前的suit、case的名称
+        :param join_str: suite和case的连接字符串，默认为-
+        :param suite: 是否显示suite名
+        :param case: 是否显示case名，如果不是case内，即使True也不显示
+        :return: 连接好的字符串
+        """
+        sc_list = []
+        if suite:
+            sc_list.append(self.get_robot_variable('SUITE NAME'))
+        if case:
+            temp = self.get_robot_variable('TEST NAME')
+            if temp is not None:
+                sc_list.append(self.get_robot_variable('TEST NAME'))
+        return join_str.join(sc_list)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `movoid_robotframework-1.3.2/RobotFrameworkBasic/decorator.py` & `movoid_robotframework-1.4.0/RobotFrameworkBasic/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.3.2/RobotFrameworkBasic/version.py` & `movoid_robotframework-1.4.0/RobotFrameworkBasic/version.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.3.2/setup.py` & `movoid_robotframework-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework',
-    version='1.3.2',
+    version='1.4.0',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['robotframework',
+    install_requires=['robotframework>=6.0,<8',
                       'movoid_function'
                       ],
 )
```

