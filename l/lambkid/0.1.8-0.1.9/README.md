# Comparing `tmp/lambkid-0.1.8.tar.gz` & `tmp/lambkid-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.1.8.tar", last modified: Tue Apr  9 07:17:10 2024, max compression
+gzip compressed data, was "lambkid-0.1.9.tar", last modified: Tue Apr  9 07:47:44 2024, max compression
```

## Comparing `lambkid-0.1.8.tar` & `lambkid-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.138869 lambkid-0.1.8/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2005 2024-04-09 07:17:10.137903 lambkid-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      628 2024-04-09 07:16:28.000000 lambkid-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.089002 lambkid-0.1.8/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.1.8/docs/cli.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.8/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.8/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.8/docs/sshclient.md
-drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.097978 lambkid-0.1.8/lambkid/
--rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.8/lambkid/__init__.py
--rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.1.8/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.133912 lambkid-0.1.8/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.8/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.8/lambkid/libs/log.py
--rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.1.8/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     6886 2024-04-02 06:59:39.000000 lambkid-0.1.8/lambkid/libs/ssh.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:17:10.135877 lambkid-0.1.8/lambkid.egg-info/
--rw-rw-rw-   0        0        0     2005 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 07:17:09.000000 lambkid-0.1.8/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 07:17:10.138869 lambkid-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1845 2024-04-09 07:16:28.000000 lambkid-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.224520 lambkid-0.1.9/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2005 2024-04-09 07:47:44.223548 lambkid-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-04-09 07:16:28.000000 lambkid-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.169695 lambkid-0.1.9/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.1.9/docs/cli.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.1.9/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.1.9/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.1.9/docs/sshclient.md
+drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.177646 lambkid-0.1.9/lambkid/
+-rw-rw-rw-   0        0        0      113 2024-04-01 07:23:01.000000 lambkid-0.1.9/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.1.9/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.220531 lambkid-0.1.9/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.1.9/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1406 2024-04-07 15:19:33.000000 lambkid-0.1.9/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.1.9/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     6889 2024-04-09 07:46:29.000000 lambkid-0.1.9/lambkid/libs/ssh.py
+drwxrwxrwx   0        0        0        0 2024-04-09 07:47:44.222526 lambkid-0.1.9/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     2005 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 07:47:44.000000 lambkid-0.1.9/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 07:47:44.225518 lambkid-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1845 2024-04-09 07:46:55.000000 lambkid-0.1.9/setup.py
```

### Comparing `lambkid-0.1.8/LICENSE` & `lambkid-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.8/PKG-INFO` & `lambkid-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.8
+Version: 0.1.9
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.1.8/README.md` & `lambkid-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.8/docs/log.md` & `lambkid-0.1.9/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.8/docs/sshclient.md` & `lambkid-0.1.9/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.8/lambkid/cli.py` & `lambkid-0.1.9/lambkid/cli.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.8/lambkid/libs/log.py` & `lambkid-0.1.9/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.8/lambkid/libs/minio_client.py` & `lambkid-0.1.9/lambkid/libs/minio_client.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.1.8/lambkid/libs/ssh.py` & `lambkid-0.1.9/lambkid/libs/ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     @property
     def exit_status_code(self):
         return self.__exit_status_code
 
 
 class SSHClient(object):
     def __init__(self, ip="127.0.0.1", port=22, username="root", password="", keep_alive_interval=60,
-                 connect_timeout=60):
+                 connect_timeout=1200):
         self.__ip = ip
         self.__port = port
         self.__username = username
         self.__password = password
         self.__keep_alive_interval = keep_alive_interval
         self.__connect_timeout = connect_timeout
         self.__ssh = None
@@ -40,30 +40,30 @@
     def ip(self):
         return self.__ip
 
     @property
     def port(self):
         return self.__port
 
-    def wait_for_sshable(self, timeout=120):
+    def wait_for_sshable(self, timeout=600):
         count = 0
         while True:
             count += 1
             if count > (int(timeout / 10)):
                 log.error(f" {self.__ip}:{self.__port} | server {self.__ip} ssh timeout {timeout}s: Error.")
                 return False
             try:
                 if self.__connect():
                     log.info(f" {self.__ip}:{self.__port} | server {self.__ip} can ssh: OK.")
                     return True
             except Exception as e:
                 log.warning(f" {self.__ip}:{self.__port} | server {self.__ip} can not ssh: Error. err msg is {str(e)}")
                 time.sleep(10)
 
-    def exec(self, cmd, timeout=60):
+    def exec(self, cmd, timeout=600):
         log.info(f" {self.__ip}:{self.__port} | begin to run cmd {cmd}, timeout is {timeout}...")
         try:
             if not self.__is_active():
                 self.__reconnect()
             stdin, stdout, stderr = self.__ssh.exec_command(cmd, timeout=timeout)
             exit_status_code = stdout.channel.recv_exit_status()
             output = stdout.read().decode("utf-8")
```

### Comparing `lambkid-0.1.8/lambkid.egg-info/PKG-INFO` & `lambkid-0.1.9/lambkid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.1.8
+Version: 0.1.9
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.1.8/setup.py` & `lambkid-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.1.8",
+    version="0.1.9",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
```

