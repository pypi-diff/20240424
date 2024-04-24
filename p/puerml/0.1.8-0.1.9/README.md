# Comparing `tmp/puerml-0.1.8.tar.gz` & `tmp/puerml-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puerml-0.1.8.tar", last modified: Tue Apr 23 13:09:40 2024, max compression
+gzip compressed data, was "puerml-0.1.9.tar", last modified: Tue Apr 23 13:39:58 2024, max compression
```

## Comparing `puerml-0.1.8.tar` & `puerml-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:09:40.546100 puerml-0.1.8/
--rw-r--r--   0 Alexander   (502) staff       (20)     1070 2024-04-22 09:02:31.000000 puerml-0.1.8/LICENSE
--rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-23 13:09:40.545655 puerml-0.1.8/PKG-INFO
--rw-r--r--   0 Alexander   (502) staff       (20)        4 2024-04-22 09:02:31.000000 puerml-0.1.8/README.md
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:09:40.534250 puerml-0.1.8/puerml/
--rw-r--r--   0 Alexander   (502) staff       (20)       51 2024-04-22 09:37:20.000000 puerml-0.1.8/puerml/__init__.py
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:09:40.543258 puerml-0.1.8/puerml/library/
--rw-r--r--   0 Alexander   (502) staff       (20)      179 2024-04-23 12:52:56.000000 puerml-0.1.8/puerml/library/__init__.py
--rw-r--r--   0 Alexander   (502) staff       (20)      850 2024-04-22 09:10:49.000000 puerml-0.1.8/puerml/library/benchmark.py
--rw-r--r--   0 Alexander   (502) staff       (20)     8390 2024-04-22 09:10:49.000000 puerml-0.1.8/puerml/library/data_frame.py
--rw-r--r--   0 Alexander   (502) staff       (20)      655 2024-04-23 12:52:56.000000 puerml-0.1.8/puerml/library/decorators.py
--rw-r--r--   0 Alexander   (502) staff       (20)     2217 2024-04-23 12:52:56.000000 puerml-0.1.8/puerml/library/git.py
--rw-r--r--   0 Alexander   (502) staff       (20)     2318 2024-04-23 12:52:56.000000 puerml-0.1.8/puerml/library/jsonl.py
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:09:40.536937 puerml-0.1.8/puerml.egg-info/
--rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-23 13:09:40.000000 puerml-0.1.8/puerml.egg-info/PKG-INFO
--rw-r--r--   0 Alexander   (502) staff       (20)      324 2024-04-23 13:09:40.000000 puerml-0.1.8/puerml.egg-info/SOURCES.txt
--rw-r--r--   0 Alexander   (502) staff       (20)        1 2024-04-23 13:09:40.000000 puerml-0.1.8/puerml.egg-info/dependency_links.txt
--rw-r--r--   0 Alexander   (502) staff       (20)        7 2024-04-23 13:09:40.000000 puerml-0.1.8/puerml.egg-info/top_level.txt
--rw-r--r--   0 Alexander   (502) staff       (20)       38 2024-04-23 13:09:40.546254 puerml-0.1.8/setup.cfg
--rw-r--r--   0 Alexander   (502) staff       (20)      149 2024-04-23 13:09:39.000000 puerml-0.1.8/setup.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:39:58.419737 puerml-0.1.9/
+-rw-r--r--   0 Alexander   (502) staff       (20)     1070 2024-04-22 09:02:31.000000 puerml-0.1.9/LICENSE
+-rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-23 13:39:58.419242 puerml-0.1.9/PKG-INFO
+-rw-r--r--   0 Alexander   (502) staff       (20)        4 2024-04-22 09:02:31.000000 puerml-0.1.9/README.md
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:39:58.409886 puerml-0.1.9/puerml/
+-rw-r--r--   0 Alexander   (502) staff       (20)       51 2024-04-22 09:37:20.000000 puerml-0.1.9/puerml/__init__.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:39:58.418073 puerml-0.1.9/puerml/library/
+-rw-r--r--   0 Alexander   (502) staff       (20)      179 2024-04-23 12:52:56.000000 puerml-0.1.9/puerml/library/__init__.py
+-rw-r--r--   0 Alexander   (502) staff       (20)      850 2024-04-22 09:10:49.000000 puerml-0.1.9/puerml/library/benchmark.py
+-rw-r--r--   0 Alexander   (502) staff       (20)     8567 2024-04-23 13:39:52.000000 puerml-0.1.9/puerml/library/data_frame.py
+-rw-r--r--   0 Alexander   (502) staff       (20)      655 2024-04-23 12:52:56.000000 puerml-0.1.9/puerml/library/decorators.py
+-rw-r--r--   0 Alexander   (502) staff       (20)     2217 2024-04-23 12:52:56.000000 puerml-0.1.9/puerml/library/git.py
+-rw-r--r--   0 Alexander   (502) staff       (20)     2318 2024-04-23 12:52:56.000000 puerml-0.1.9/puerml/library/jsonl.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:39:58.412321 puerml-0.1.9/puerml.egg-info/
+-rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-23 13:39:58.000000 puerml-0.1.9/puerml.egg-info/PKG-INFO
+-rw-r--r--   0 Alexander   (502) staff       (20)      324 2024-04-23 13:39:58.000000 puerml-0.1.9/puerml.egg-info/SOURCES.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)        1 2024-04-23 13:39:58.000000 puerml-0.1.9/puerml.egg-info/dependency_links.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)        7 2024-04-23 13:39:58.000000 puerml-0.1.9/puerml.egg-info/top_level.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)       38 2024-04-23 13:39:58.419941 puerml-0.1.9/setup.cfg
+-rw-r--r--   0 Alexander   (502) staff       (20)      149 2024-04-23 13:39:57.000000 puerml-0.1.9/setup.py
```

### Comparing `puerml-0.1.8/LICENSE` & `puerml-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `puerml-0.1.8/puerml/library/benchmark.py` & `puerml-0.1.9/puerml/library/benchmark.py`

 * *Files identical despite different names*

### Comparing `puerml-0.1.8/puerml/library/data_frame.py` & `puerml-0.1.9/puerml/library/data_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 
 	@staticmethod
 	def open(file_path, delimiter=None, encoding='utf-8'):
 		df = DataFrame()
 		df.append_file(file_path, delimiter, encoding)
 		return df
 		
+	@staticmethod
+	def from_string(s, delimiter='\t'):
+		rows   = [line.strip().split(delimiter) for line in s.split('\n')]
+		header = rows.pop(0)
+		return DataFrame(header, rows)
 
 	######################################################
 			
 	def __init__(self, header=None, rows=None):
 		self.id      = DataFrame._id
 		self.rows    = []
 		self.header  = None
```

### Comparing `puerml-0.1.8/puerml/library/decorators.py` & `puerml-0.1.9/puerml/library/decorators.py`

 * *Files identical despite different names*

### Comparing `puerml-0.1.8/puerml/library/git.py` & `puerml-0.1.9/puerml/library/git.py`

 * *Files identical despite different names*

### Comparing `puerml-0.1.8/puerml/library/jsonl.py` & `puerml-0.1.9/puerml/library/jsonl.py`

 * *Files identical despite different names*

