# Comparing `tmp/tools_hjh-2.6.2.tar.gz` & `tmp/tools_hjh-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.6.2.tar", last modified: Mon Apr 22 04:50:05 2024, max compression
+gzip compressed data, was "dist\tools_hjh-2.6.3.tar", last modified: Wed Apr 24 01:51:43 2024, max compression
```

## Comparing `tools_hjh-2.6.2.tar` & `tools_hjh-2.6.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 04:50:05.000000 tools_hjh-2.6.2/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.2/LICENSE
--rw-rw-rw-   0        0        0      207 2024-04-22 04:50:05.000000 tools_hjh-2.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 04:50:05.000000 tools_hjh-2.6.2/setup.cfg
--rw-rw-rw-   0        0        0      417 2024-02-19 08:41:24.000000 tools_hjh-2.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 04:50:04.000000 tools_hjh-2.6.2/tools_hjh/
--rw-rw-rw-   0        0        0     3720 2024-03-13 07:44:26.000000 tools_hjh-2.6.2/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.2/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     6029 2024-04-22 03:27:09.000000 tools_hjh-2.6.2/tools_hjh/Fanyi.py
--rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.2/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.2/tools_hjh/HTTPRequest2.py
--rw-rw-rw-   0        0        0     9183 2024-03-13 12:45:59.000000 tools_hjh-2.6.2/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.2/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.2/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    44796 2024-04-22 02:39:49.000000 tools_hjh-2.6.2/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.2/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     2092 2024-03-13 06:16:36.000000 tools_hjh-2.6.2/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     7061 2024-04-22 01:45:38.000000 tools_hjh-2.6.2/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      539 2024-01-30 07:55:42.000000 tools_hjh-2.6.2/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 04:50:05.000000 tools_hjh-2.6.2/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-22 04:50:03.000000 tools_hjh-2.6.2/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-04-22 04:50:02.000000 tools_hjh-2.6.2/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-04-22 04:50:03.000000 tools_hjh-2.6.2/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      498 2024-04-22 04:50:03.000000 tools_hjh-2.6.2/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2024-04-22 04:50:03.000000 tools_hjh-2.6.2/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 01:51:43.000000 tools_hjh-2.6.3/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.3/LICENSE
+-rw-rw-rw-   0        0        0      207 2024-04-24 01:51:43.000000 tools_hjh-2.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 01:51:43.000000 tools_hjh-2.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      417 2024-04-24 01:51:25.000000 tools_hjh-2.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:51:42.000000 tools_hjh-2.6.3/tools_hjh/
+-rw-rw-rw-   0        0        0     4066 2024-04-22 08:48:58.000000 tools_hjh-2.6.3/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.3/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.3/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.3/tools_hjh/HTTPRequest2.py
+-rw-rw-rw-   0        0        0     9183 2024-03-13 12:45:59.000000 tools_hjh-2.6.3/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.3/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.3/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    46268 2024-04-24 01:40:14.000000 tools_hjh-2.6.3/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.3/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     2092 2024-03-13 06:16:36.000000 tools_hjh-2.6.3/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     7061 2024-04-22 05:04:03.000000 tools_hjh-2.6.3/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      539 2024-01-30 07:55:42.000000 tools_hjh-2.6.3/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:51:43.000000 tools_hjh-2.6.3/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      479 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.6.2/tools_hjh/Chrome.py` & `tools_hjh-2.6.3/tools_hjh/Chrome.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,24 +25,31 @@
 class Chrome():
     """ 使用浏览器解析url，返回源码
         __init__.param：
             chrome_path: chrome.exe路径
             chromedriver_path: chromedriver.exe路径
     """
 
-    def __init__(self, chrome_path, chromedriver_path, is_hidden=False, is_display_picture=True):
+    def __init__(self, chrome_path, chromedriver_path, is_hidden=False, is_display_picture=True, headers=None):
         chrome_options = Options()
+        # chrome_options.add_argument("--single-process")
+        # chrome_options.add_argument("--disable-site-isolation-trials")
+
         if is_hidden:
             chrome_options.add_argument("--headless")
         chrome_options.binary_location = chrome_path
         if not is_display_picture:
             chrome_options.add_experimental_option('prefs', {'profile.managed_default_content_settings.images': 2})
+        if headers is not None:
+            for key, value in headers.items():
+                header = key + "=" + value
+                chrome_options.add_argument(header)
         self.chrome = webdriver.Chrome(chromedriver_path, options=chrome_options)
         self.status = 0  # 未被占用
-        
+    
     def set_cookies(self, cookies, cookie_domian):
         self.get(cookie_domian)
         for cookie in cookies:
             self.chrome.add_cookie(cookie)
         
     def close(self):
         self.chrome.quit()
@@ -56,20 +63,20 @@
     
     def get_status(self):
         return self.status
 
 
 class ChromePool():
 
-    def __init__(self, maxSize, chrome_path, chromedriver_path, is_hidden=False, is_display_picture=True, cache=False):
+    def __init__(self, maxSize, chrome_path, chromedriver_path, is_hidden=False, is_display_picture=True, cache=False, headers=None):
         self.cache = cache
         self.maxSize = maxSize
         self.pool = []
         for _ in range(0, maxSize):
-            self.pool.append(Chrome(chrome_path, chromedriver_path, is_hidden, is_display_picture))
+            self.pool.append(Chrome(chrome_path, chromedriver_path, is_hidden, is_display_picture, headers))
         self.openSize = 0
         
     def set_cookies(self, cookies, cookie_domian):
 
         def set_one(chrome, cookies, cookie_domian):
             chrome.set_cookies(cookies, cookie_domian)
```

### Comparing `tools_hjh-2.6.2/tools_hjh/DBConn.py` & `tools_hjh-2.6.3/tools_hjh/DBConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/HTTPRequest.py` & `tools_hjh-2.6.3/tools_hjh/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/HTTPRequest2.py` & `tools_hjh-2.6.3/tools_hjh/HTTPRequest2.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/HTTPTools.py` & `tools_hjh-2.6.3/tools_hjh/HTTPTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/Log.py` & `tools_hjh-2.6.3/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/MemoryDB.py` & `tools_hjh-2.6.3/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/OracleTools.py` & `tools_hjh-2.6.3/tools_hjh/OracleTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding:utf-8
 from tools_hjh.DBConn import DBConn
 from tools_hjh.MemoryDB import MemoryDB
 from tools_hjh.Tools import line_merge_align, locatdate, merge_spaces, analysis_hosts, locattime
 from tools_hjh import Tools
+import math
     
 
 def main():
     rows = []
     for idx in range(0, 10):
         row = (idx, idx, idx)
         rows.append(row)
@@ -14,15 +15,45 @@
     num = testDB.insert('t1', rows, 'c1')
     print(num)
     testDB.close()
 
 
 class OracleTools:
     """ 用于Oracle的工具类 """
-    
+
+    @staticmethod
+    def insert_not_exists_by_dblink(ora_conn, src_link, username, table):
+        """通过dblink补充某个表中唯一键缺少的记录"""
+        mess = OracleTools.desc(ora_conn, username, table)
+        cols_list = None
+        cols_num = math.inf
+        for line in mess.split('\n'):
+            if line.startswith('index') and line.endswith('unique'):
+                cols_ = line.split('(')[1].split(')')[0]
+                cols_num_ = len(cols_.split(', '))
+                if cols_num_ < cols_num:
+                    cols_num = cols_num_
+                    cols_list = cols_.split(', ')
+        if cols_list == None:
+            cols_list = []
+            for line in mess.split('\n'):
+                if line.startswith('column'):
+                    col = line.split(' ')[1]
+                    cols_list.append(col)
+        left_sql = ''
+        right_sql = ''
+        for col in cols_list:
+            left_sql = left_sql + 't.' + col + '||'
+            right_sql = right_sql + 't2.' + col + '||'
+        where_sql = left_sql[0:-2] + ' = ' + right_sql[0:-2]
+        
+        sql = 'insert into {username}.{table} \nselect * from {username}.{table}@{src_link} t where not exists(select 1 from {username}.{table} t2 where {where_sql})'
+        sql = sql.replace('{username}', username).replace('{table}', table).replace('{src_link}', src_link).replace('{where_sql}', where_sql)
+        return sql
+
     @staticmethod
     def desc(ora_conn, username, table, simple_mode=True):
         """得到表结构，包括索引、约束和默认值情况"""
         username = username.upper()
         table = table.upper()
         mess = 'table: ' + table.lower() + '\n'
```

### Comparing `tools_hjh-2.6.2/tools_hjh/SSHConn.py` & `tools_hjh-2.6.3/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/ThreadPool.py` & `tools_hjh-2.6.3/tools_hjh/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/Tools.py` & `tools_hjh-2.6.3/tools_hjh/Tools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.2/tools_hjh/__init__.py` & `tools_hjh-2.6.3/tools_hjh/__init__.py`

 * *Files identical despite different names*

