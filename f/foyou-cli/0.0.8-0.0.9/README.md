# Comparing `tmp/foyou-cli-0.0.8.tar.gz` & `tmp/foyou-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foyou-cli-0.0.8.tar", last modified: Wed Nov  8 09:05:07 2023, max compression
+gzip compressed data, was "foyou-cli-0.0.9.tar", last modified: Sat Nov 11 04:14:00 2023, max compression
```

## Comparing `foyou-cli-0.0.8.tar` & `foyou-cli-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:05:07.468586 foyou-cli-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-11-08 09:05:07.468586 foyou-cli-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 09:05:07.468586 foyou-cli-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:05:07.464586 foyou-cli-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:05:07.468586 foyou-cli-0.0.8/src/foyou_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2023-11-08 09:05:06.000000 foyou-cli-0.0.8/src/foyou_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/src/foyou_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/src/foyou_cli/aliyundrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/src/foyou_cli/ebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-11-08 09:04:59.000000 foyou-cli-0.0.8/src/foyou_cli/wireguard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 09:05:07.468586 foyou-cli-0.0.8/src/foyou_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-11-08 09:05:07.000000 foyou-cli-0.0.8/src/foyou_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-11-08 09:05:07.000000 foyou-cli-0.0.8/src/foyou_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 09:05:07.000000 foyou-cli-0.0.8/src/foyou_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-08 09:05:07.000000 foyou-cli-0.0.8/src/foyou_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-08 09:05:07.000000 foyou-cli-0.0.8/src/foyou_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-08 09:05:07.000000 foyou-cli-0.0.8/src/foyou_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 04:14:00.137322 foyou-cli-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-11-11 04:14:00.137322 foyou-cli-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-11 04:14:00.137322 foyou-cli-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 04:14:00.133321 foyou-cli-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 04:14:00.137322 foyou-cli-0.0.9/src/foyou_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2023-11-11 04:13:59.000000 foyou-cli-0.0.9/src/foyou_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/src/foyou_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/src/foyou_cli/aliyundrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/src/foyou_cli/ebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2023-11-11 04:13:51.000000 foyou-cli-0.0.9/src/foyou_cli/wireguard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 04:14:00.137322 foyou-cli-0.0.9/src/foyou_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-11-11 04:14:00.000000 foyou-cli-0.0.9/src/foyou_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2023-11-11 04:14:00.000000 foyou-cli-0.0.9/src/foyou_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-11 04:14:00.000000 foyou-cli-0.0.9/src/foyou_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-11 04:14:00.000000 foyou-cli-0.0.9/src/foyou_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-11 04:14:00.000000 foyou-cli-0.0.9/src/foyou_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-11 04:14:00.000000 foyou-cli-0.0.9/src/foyou_cli.egg-info/top_level.txt
```

### Comparing `foyou-cli-0.0.8/LICENSE` & `foyou-cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `foyou-cli-0.0.8/PKG-INFO` & `foyou-cli-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foyou-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: python package foyou-cli
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/foyou-cli
 Project-URL: Homepage, https://github.com/foyoux/foyou-cli
 Project-URL: Bug Tracker, https://github.com/foyoux/foyou-cli/issues
 Keywords: foyou-cli
 Classifier: Programming Language :: Python
```

### Comparing `foyou-cli-0.0.8/pyproject.toml` & `foyou-cli-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `foyou-cli-0.0.8/src/foyou_cli/__init__.py` & `foyou-cli-0.0.9/src/foyou_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __title__ = 'foyou-cli'
 __author__ = 'foyoux'
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 __url__ = 'https://github.com/foyoux/foyou-cli'
 __ide__ = 'PyCharm - https://www.jetbrains.com/pycharm/'
 
 import fire
 
 from .aliyundrive import download_by_idm, upload_file
 from .ebook import add_nav_for_epub
```

### Comparing `foyou-cli-0.0.8/src/foyou_cli/aliyundrive.py` & `foyou-cli-0.0.9/src/foyou_cli/aliyundrive.py`

 * *Files identical despite different names*

### Comparing `foyou-cli-0.0.8/src/foyou_cli/ebook.py` & `foyou-cli-0.0.9/src/foyou_cli/ebook.py`

 * *Files identical despite different names*

### Comparing `foyou-cli-0.0.8/src/foyou_cli/wireguard.py` & `foyou-cli-0.0.9/src/foyou_cli/wireguard.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,9 +17,10 @@
         print(i.decode('gb18030'))
         j = i.split()
         if len(j) > 1 and j[1] == b'5':
             idx = j[0].decode()
             print('获取到 WireGuard 网卡索引', idx)
             subprocess.run(f'netsh interface ipv4 set interface {idx} metric={metric}'.split())
             subprocess.run(f'route add 0.0.0.0 mask 128.0.0.0 {gateway}'.split())
+            subprocess.run(f'route add 128.0.0.0 mask 128.0.0.0 {gateway}'.split())
             subprocess.run('ipconfig /flushdns'.split())
             return
```

### Comparing `foyou-cli-0.0.8/src/foyou_cli.egg-info/PKG-INFO` & `foyou-cli-0.0.9/src/foyou_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foyou-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: python package foyou-cli
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/foyou-cli
 Project-URL: Homepage, https://github.com/foyoux/foyou-cli
 Project-URL: Bug Tracker, https://github.com/foyoux/foyou-cli/issues
 Keywords: foyou-cli
 Classifier: Programming Language :: Python
```

