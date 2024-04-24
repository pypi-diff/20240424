# Comparing `tmp/mysql_server_has_gone-2.0.2.tar.gz` & `tmp/mysql_server_has_gone-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_server_has_gone-2.0.2.tar", last modified: Tue Apr 23 01:46:41 2024, max compression
+gzip compressed data, was "mysql_server_has_gone-2.0.3.tar", last modified: Wed Apr 24 06:52:30 2024, max compression
```

## Comparing `mysql_server_has_gone-2.0.2.tar` & `mysql_server_has_gone-2.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 01:46:41.805828 mysql_server_has_gone-2.0.2/
--rw-rw-rw-   0        0        0     1082 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     1090 2024-04-23 01:46:41.805297 mysql_server_has_gone-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      750 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 01:46:41.804272 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/
--rw-rw-rw-   0        0        0     1090 2024-04-23 01:46:41.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-23 01:46:41.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 01:46:41.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-23 01:46:41.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 01:46:41.803151 mysql_server_has_gone-2.0.2/mysql_server_has_gone_away/
--rw-rw-rw-   0        0        0        0 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone_away/__init__.py
--rw-rw-rw-   0        0        0     1973 2024-04-23 01:44:06.000000 mysql_server_has_gone-2.0.2/mysql_server_has_gone_away/base.py
--rw-rw-rw-   0        0        0       42 2024-04-23 01:46:41.805828 mysql_server_has_gone-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      544 2024-04-23 01:46:38.000000 mysql_server_has_gone-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 06:52:30.056816 mysql_server_has_gone-2.0.3/
+-rw-rw-rw-   0        0        0     1082 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1090 2024-04-24 06:52:30.055809 mysql_server_has_gone-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 06:52:30.054014 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/
+-rw-rw-rw-   0        0        0     1090 2024-04-24 06:52:29.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-24 06:52:29.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 06:52:29.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-24 06:52:29.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 06:52:30.052797 mysql_server_has_gone-2.0.3/mysql_server_has_gone_away/
+-rw-rw-rw-   0        0        0        0 2024-04-11 06:21:33.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone_away/__init__.py
+-rw-rw-rw-   0        0        0     2491 2024-04-24 06:51:45.000000 mysql_server_has_gone-2.0.3/mysql_server_has_gone_away/base.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 06:52:30.057819 mysql_server_has_gone-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      544 2024-04-24 06:47:40.000000 mysql_server_has_gone-2.0.3/setup.py
```

### Comparing `mysql_server_has_gone-2.0.2/LICENSE` & `mysql_server_has_gone-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_server_has_gone-2.0.2/PKG-INFO` & `mysql_server_has_gone-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_server_has_gone
-Version: 2.0.2
+Version: 2.0.3
 Summary: Django myslq backend that fixes issue with long living connection
 Home-page: https://github.com/maiyajj/MySQL-server-has-gone-away
 Author: maiyajj
 Author-email: 1045373828@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysql_server_has_gone-2.0.2/README.md` & `mysql_server_has_gone-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mysql_server_has_gone-2.0.2/mysql_server_has_gone.egg-info/PKG-INFO` & `mysql_server_has_gone-2.0.3/mysql_server_has_gone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_server_has_gone
-Version: 2.0.2
+Version: 2.0.3
 Summary: Django myslq backend that fixes issue with long living connection
 Home-page: https://github.com/maiyajj/MySQL-server-has-gone-away
 Author: maiyajj
 Author-email: 1045373828@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mysql_server_has_gone-2.0.2/mysql_server_has_gone_away/base.py` & `mysql_server_has_gone-2.0.3/mysql_server_has_gone_away/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 https://stackoverflow.com/a/60894948/3872976
 """
 
 import logging
 
 from django.db import IntegrityError, InterfaceError, OperationalError
 from django.db.backends.mysql import base
+from django.db.utils import OperationalError as DjangoOperationalError
+from MySQLdb import OperationalError as MySQLOperationalError
 from retry import retry
 
 logger = logging.getLogger("mysql_server_has_gone_away")
 
 
 def check_mysql_gone_away(db_wrapper):
     def decorate(f):
-        @retry(tries=3)
+        @retry(tries=5)
         def wrapper(self, query, args=None):
             try:
                 return f(self, query, args)
-            except (OperationalError, InterfaceError) as e:
+            except (OperationalError, DjangoOperationalError, MySQLOperationalError, InterfaceError) as e:
                 logger.error(f"MySQL server has gone away. Rerunning query: {query}; Error: {e}")
                 if (
                     "MySQL server has gone away" in str(e)
                     or "Server has gone away" in str(e)
                     or "Lost connection to MySQL server during query" in str(e)
+                    or "The client was disconnected by the server because of inactivity" in str(e)
                 ):
                     db_wrapper.connection.close()
                     db_wrapper.connect()
                     self.cursor = db_wrapper.connection.cursor()
                     return f(self, query, args)
                 # Map some error codes to IntegrityError, since they seem to be
                 # misclassified and Django would prefer the more logical place.
@@ -51,7 +54,13 @@
 
             @check_mysql_gone_away(self)
             def executemany(self, query, args):
                 return self.cursor.executemany(query, args)
 
         cursor = self.connection.cursor()
         return CursorWrapper(cursor)
+
+    def _set_autocommit(self, autocommit):
+        try:
+            super()._set_autocommit(autocommit)
+        except (DjangoOperationalError, MySQLOperationalError) as e:
+            logger.error(f"DatabaseWrapper Error: {e}")
```

### Comparing `mysql_server_has_gone-2.0.2/setup.py` & `mysql_server_has_gone-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mysql_server_has_gone",
-    version="2.0.2",
+    version="2.0.3",
     description="Django myslq backend that fixes issue with long living connection",
     author="maiyajj",
     author_email="1045373828@qq.com",
     license="MIT",
     url="https://github.com/maiyajj/MySQL-server-has-gone-away",
     long_description=long_description,
     packages=find_packages(),
```

