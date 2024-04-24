# Comparing `tmp/prophet_tools-0.8.tar.gz` & `tmp/prophet_tools-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophet_tools-0.8.tar", last modified: Tue Apr 23 19:48:57 2024, max compression
+gzip compressed data, was "prophet_tools-0.9.tar", last modified: Wed Apr 24 21:50:14 2024, max compression
```

## Comparing `prophet_tools-0.8.tar` & `prophet_tools-0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 19:48:57.376551 prophet_tools-0.8/
--rw-rw-rw-   0        0        0      137 2024-04-23 19:48:57.376551 prophet_tools-0.8/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-09-29 07:18:11.000000 prophet_tools-0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 19:48:57.373551 prophet_tools-0.8/prophet_tools/
--rw-rw-rw-   0        0        0        0 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/__init__.py
--rw-rw-rw-   0        0        0      149 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/auto_import.py
--rw-rw-rw-   0        0        0     1811 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/file_convertors.py
--rw-rw-rw-   0        0        0      268 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/how_to_import.py
--rw-rw-rw-   0        0        0     6879 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/my_functions.py
--rw-rw-rw-   0        0        0      463 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/parsing.py
--rw-rw-rw-   0        0        0     1287 2024-04-23 19:45:43.000000 prophet_tools-0.8/prophet_tools/terminal.py
--rw-rw-rw-   0        0        0     4164 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/всё_подряд.py
-drwxrwxrwx   0        0        0        0 2024-04-23 19:48:57.376551 prophet_tools-0.8/prophet_tools.egg-info/
--rw-rw-rw-   0        0        0      137 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 19:48:57.377553 prophet_tools-0.8/setup.cfg
--rw-rw-rw-   0        0        0      240 2024-04-23 19:46:42.000000 prophet_tools-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:50:14.891113 prophet_tools-0.9/
+-rw-rw-rw-   0        0        0      137 2024-04-24 21:50:14.891113 prophet_tools-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-09-29 07:18:11.000000 prophet_tools-0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 21:50:14.887115 prophet_tools-0.9/prophet_tools/
+-rw-rw-rw-   0        0        0        0 2024-04-23 19:32:58.000000 prophet_tools-0.9/prophet_tools/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-04-23 19:32:58.000000 prophet_tools-0.9/prophet_tools/auto_import.py
+-rw-rw-rw-   0        0        0     1811 2024-04-23 19:32:58.000000 prophet_tools-0.9/prophet_tools/file_convertors.py
+-rw-rw-rw-   0        0        0      268 2024-04-23 19:32:58.000000 prophet_tools-0.9/prophet_tools/how_to_import.py
+-rw-rw-rw-   0        0        0     6970 2024-04-24 21:49:50.000000 prophet_tools-0.9/prophet_tools/my_functions.py
+-rw-rw-rw-   0        0        0      463 2024-04-23 19:32:58.000000 prophet_tools-0.9/prophet_tools/parsing.py
+-rw-rw-rw-   0        0        0     1287 2024-04-23 19:45:43.000000 prophet_tools-0.9/prophet_tools/terminal.py
+-rw-rw-rw-   0        0        0     4164 2024-04-23 19:32:58.000000 prophet_tools-0.9/prophet_tools/всё_подряд.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:50:14.891113 prophet_tools-0.9/prophet_tools.egg-info/
+-rw-rw-rw-   0        0        0      137 2024-04-24 21:50:14.000000 prophet_tools-0.9/prophet_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-04-24 21:50:14.000000 prophet_tools-0.9/prophet_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 21:50:14.000000 prophet_tools-0.9/prophet_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 19:48:57.000000 prophet_tools-0.9/prophet_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-04-24 21:50:14.000000 prophet_tools-0.9/prophet_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 21:50:14.892113 prophet_tools-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      240 2024-04-24 21:50:05.000000 prophet_tools-0.9/setup.py
```

### Comparing `prophet_tools-0.8/prophet_tools/file_convertors.py` & `prophet_tools-0.9/prophet_tools/file_convertors.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.8/prophet_tools/my_functions.py` & `prophet_tools-0.9/prophet_tools/my_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,25 +194,25 @@
 
 def open_folder_in_explorer(folder):
     import os
     folder = folder.replace('/', '\\')
     os.popen(f'explorer {folder}')
 
 def check_in(what, where):
-    if type(what) is str:
+    if type(what) is type(where) is str:
+        return what in where or where in what
+    elif type(what) is str:
         for place in where:
             if what in place:
                 return True
-
-    if type(where) is str:
+    elif type(where) is str:
         for thing in what:
             if thing in where:
                 return True
-
-    if type(what) is type(where) is list:
+    elif type(what) is type(where) is list:
         for thing in what:
             for place in where:
                 if thing in place:
                     return True
 
 if __name__ == '__main__':
     # print(list_of_files(r'C:\Users\Тарасов Никита\YandexDisk\проекты\_Постоянные\Учебный центр\Основы работы на ПК\Дети\1. Word\1. Текст, форматирование, таблицы'))
```

### Comparing `prophet_tools-0.8/prophet_tools/terminal.py` & `prophet_tools-0.9/prophet_tools/terminal.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.8/prophet_tools/всё_подряд.py` & `prophet_tools-0.9/prophet_tools/всё_подряд.py`

 * *Files identical despite different names*

