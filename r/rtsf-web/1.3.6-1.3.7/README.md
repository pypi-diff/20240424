# Comparing `tmp/rtsf-web-1.3.6.tar.gz` & `tmp/rtsf-web-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rtsf-web-1.3.6.tar", last modified: Tue Aug  1 01:39:24 2023, max compression
+gzip compressed data, was "dist\rtsf-web-1.3.7.tar", last modified: Wed Apr 24 06:28:00 2024, max compression
```

## Comparing `rtsf-web-1.3.6.tar` & `rtsf-web-1.3.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/
--rw-rw-rw-   0        0        0    25257 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    21165 2021-11-09 04:23:53.000000 rtsf-web-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      180 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    25257 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       32 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0      926 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/rtsf_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     2877 2023-08-01 01:33:06.000000 rtsf-web-1.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/
--rw-rw-rw-   0        0        0    23527 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/actions.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/chrome/
--rw-rw-rw-   0        0        0     1727 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/chrome/options.py
--rw-rw-rw-   0        0        0      355 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/chrome/webdriver.py
--rw-rw-rw-   0        0        0       37 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/chrome/__init__.py
--rw-rw-rw-   0        0        0     6026 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/cli.py
--rw-rw-rw-   0        0        0     8071 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/driver.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/edge/
--rw-rw-rw-   0        0        0      347 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/edge/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/edge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/firefox/
--rw-rw-rw-   0        0        0     1304 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/firefox/firefox_profile.py
--rw-rw-rw-   0        0        0      359 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/firefox/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/firefox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/ie/
--rw-rw-rw-   0        0        0      339 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/ie/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/ie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/opera/
--rw-rw-rw-   0        0        0      353 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/opera/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/opera/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/remote/
--rw-rw-rw-   0        0        0     3703 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/SeleniumHatch.py
--rw-rw-rw-   0        0        0     2856 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/SeleniumJar.py
--rw-rw-rw-   0        0        0     5917 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/wait_until.py
--rw-rw-rw-   0        0        0      355 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 01:39:24.000000 rtsf-web-1.3.6/webuidriver/safari/
--rw-rw-rw-   0        0        0      357 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/safari/webdriver.py
--rw-rw-rw-   0        0        0        0 2021-11-09 04:19:43.000000 rtsf-web-1.3.6/webuidriver/safari/__init__.py
--rw-rw-rw-   0        0        0      341 2023-08-01 01:33:56.000000 rtsf-web-1.3.6/webuidriver/__about__.py
--rw-rw-rw-   0        0        0      578 2023-08-01 01:31:48.000000 rtsf-web-1.3.6/webuidriver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.561989 rtsf-web-1.3.7/
+-rw-rw-rw-   0        0        0    25257 2024-04-24 06:28:00.560992 rtsf-web-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    21165 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.540089 rtsf-web-1.3.7/rtsf_web.egg-info/
+-rw-rw-rw-   0        0        0    25257 2024-04-24 06:28:00.000000 rtsf-web-1.3.7/rtsf_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2024-04-24 06:28:00.000000 rtsf-web-1.3.7/rtsf_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 06:28:00.000000 rtsf-web-1.3.7/rtsf_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-04-24 06:28:00.000000 rtsf-web-1.3.7/rtsf_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-04-24 06:28:00.000000 rtsf-web-1.3.7/rtsf_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 06:28:00.000000 rtsf-web-1.3.7/rtsf_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 06:28:00.561989 rtsf-web-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2877 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.545437 rtsf-web-1.3.7/webuidriver/
+-rw-rw-rw-   0        0        0      341 2024-04-24 03:08:44.000000 rtsf-web-1.3.7/webuidriver/__about__.py
+-rw-rw-rw-   0        0        0      578 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/__init__.py
+-rw-rw-rw-   0        0        0    23527 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/actions.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.547429 rtsf-web-1.3.7/webuidriver/chrome/
+-rw-rw-rw-   0        0        0       37 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/chrome/__init__.py
+-rw-rw-rw-   0        0        0     2018 2024-04-24 03:07:40.000000 rtsf-web-1.3.7/webuidriver/chrome/options.py
+-rw-rw-rw-   0        0        0      355 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/chrome/webdriver.py
+-rw-rw-rw-   0        0        0     6026 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/cli.py
+-rw-rw-rw-   0        0        0     8071 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/driver.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.549424 rtsf-web-1.3.7/webuidriver/edge/
+-rw-rw-rw-   0        0        0        0 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/edge/__init__.py
+-rw-rw-rw-   0        0        0      347 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/edge/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.551429 rtsf-web-1.3.7/webuidriver/firefox/
+-rw-rw-rw-   0        0        0        0 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/firefox/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/firefox/firefox_profile.py
+-rw-rw-rw-   0        0        0      359 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/firefox/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.552417 rtsf-web-1.3.7/webuidriver/ie/
+-rw-rw-rw-   0        0        0        0 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/ie/__init__.py
+-rw-rw-rw-   0        0        0      339 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/ie/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.553413 rtsf-web-1.3.7/webuidriver/opera/
+-rw-rw-rw-   0        0        0        0 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/opera/__init__.py
+-rw-rw-rw-   0        0        0      353 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/opera/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.558998 rtsf-web-1.3.7/webuidriver/remote/
+-rw-rw-rw-   0        0        0     3703 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/remote/SeleniumHatch.py
+-rw-rw-rw-   0        0        0     2856 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/remote/SeleniumJar.py
+-rw-rw-rw-   0        0        0        0 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/remote/__init__.py
+-rw-rw-rw-   0        0        0     5917 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/remote/wait_until.py
+-rw-rw-rw-   0        0        0      355 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/remote/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:28:00.559994 rtsf-web-1.3.7/webuidriver/safari/
+-rw-rw-rw-   0        0        0        0 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/safari/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-01-10 07:42:35.000000 rtsf-web-1.3.7/webuidriver/safari/webdriver.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rtsf-web-1.3.6/PKG-INFO` & `rtsf-web-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtsf-web
-Version: 1.3.6
+Version: 1.3.7
 Summary: only for web ui test, base on rtsf
 Home-page: https://github.com/RockFeng0/rtsf-web
 Author: 罗科峰
 Author-email: lkf20031988@163.com
 License: MIT
 Description: # rtsf-web
          基于rtsf测试框架和selenium程序框架，关键字驱动Web UI层面，进行自动化的功能测试
```

### Comparing `rtsf-web-1.3.6/README.md` & `rtsf-web-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/rtsf_web.egg-info/PKG-INFO` & `rtsf-web-1.3.7/rtsf_web.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtsf-web
-Version: 1.3.6
+Version: 1.3.7
 Summary: only for web ui test, base on rtsf
 Home-page: https://github.com/RockFeng0/rtsf-web
 Author: 罗科峰
 Author-email: lkf20031988@163.com
 License: MIT
 Description: # rtsf-web
          基于rtsf测试框架和selenium程序框架，关键字驱动Web UI层面，进行自动化的功能测试
```

### Comparing `rtsf-web-1.3.6/rtsf_web.egg-info/SOURCES.txt` & `rtsf-web-1.3.7/rtsf_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/setup.py` & `rtsf-web-1.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/webuidriver/actions.py` & `rtsf-web-1.3.7/webuidriver/actions.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/webuidriver/chrome/options.py` & `rtsf-web-1.3.7/webuidriver/chrome/options.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     NO_IMAGES = "--blink-settings=imagesEnabled=false"  # 禁用图片加载
     INCOGNITO = "--incognito"  # 隐身模式
     DISABLE_GPU = "--disable-gpu"  # 禁用gpu渲染
     FULL_SCREEN = "--start-fullscreen"  # 全屏启动
     KIOSK = "--kiosk"  # 全屏启动，无地址栏
     WINDOW_SIZE = "--window-size=1024,650"  # 置窗口尺寸(宽高)
 
+    # 将给定的（不安全的）起源视为安全的起源。多个来源可以逗号分隔的列表形式提供
+    # 例如： --unsafely-treat-insecure-origin-as-secure=http://example1.com,http://example2.com
+    UNSAFE_AS_SECURE = "--unsafely-treat-insecure-origin-as-secure="
+
 
 class ChromeExperiments(object):
     EXCLUDE_SWITCHES = {
         "name": "excludeSwitches",
         "value": [
             "ignore-certificate-errors",  # 忽略证书错误
             "enable-automation",  # 防止网站识别检测到Selenium爬虫代码
```

### Comparing `rtsf-web-1.3.6/webuidriver/cli.py` & `rtsf-web-1.3.7/webuidriver/cli.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/webuidriver/driver.py` & `rtsf-web-1.3.7/webuidriver/driver.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/webuidriver/firefox/firefox_profile.py` & `rtsf-web-1.3.7/webuidriver/firefox/firefox_profile.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/webuidriver/remote/SeleniumHatch.py` & `rtsf-web-1.3.7/webuidriver/remote/SeleniumHatch.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/webuidriver/remote/SeleniumJar.py` & `rtsf-web-1.3.7/webuidriver/remote/SeleniumJar.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/webuidriver/remote/wait_until.py` & `rtsf-web-1.3.7/webuidriver/remote/wait_until.py`

 * *Files identical despite different names*

### Comparing `rtsf-web-1.3.6/webuidriver/__init__.py` & `rtsf-web-1.3.7/webuidriver/__init__.py`

 * *Files identical despite different names*

