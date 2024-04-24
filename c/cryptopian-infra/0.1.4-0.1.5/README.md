# Comparing `tmp/cryptopian_infra-0.1.4.tar.gz` & `tmp/cryptopian_infra-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptopian_infra-0.1.4.tar", last modified: Wed Apr 17 06:43:19 2024, max compression
+gzip compressed data, was "cryptopian_infra-0.1.5.tar", last modified: Wed Apr 24 02:11:23 2024, max compression
```

## Comparing `cryptopian_infra-0.1.4.tar` & `cryptopian_infra-0.1.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.958770 cryptopian_infra-0.1.4/
--rw-r--r--   0 wuhan      (501) staff       (20)     1063 2022-01-19 16:43:46.000000 cryptopian_infra-0.1.4/LICENSE
--rw-r--r--   0 wuhan      (501) staff       (20)     1218 2024-04-17 06:43:19.958509 cryptopian_infra-0.1.4/PKG-INFO
--rw-r--r--   0 wuhan      (501) staff       (20)      446 2024-03-07 06:40:10.000000 cryptopian_infra-0.1.4/README.md
--rw-r--r--   0 wuhan      (501) staff       (20)      713 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.4/pyproject.toml
--rw-r--r--   0 wuhan      (501) staff       (20)       38 2024-04-17 06:43:19.958966 cryptopian_infra-0.1.4/setup.cfg
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.947057 cryptopian_infra-0.1.4/src/
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.948785 cryptopian_infra-0.1.4/src/cryptopian_infra/
--rw-r--r--   0 wuhan      (501) staff       (20)        0 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/__init__.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.951053 cryptopian_infra-0.1.4/src/cryptopian_infra/alert/
--rw-r--r--   0 wuhan      (501) staff       (20)      112 2024-03-31 08:31:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/alert/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1512 2024-01-15 10:05:02.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/alert/alert.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1819 2024-03-29 08:42:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/alert/alertwrapper.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1221 2024-03-31 08:31:29.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/alert/slackwebhook.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.953470 cryptopian_infra-0.1.4/src/cryptopian_infra/config/
--rw-r--r--   0 wuhan      (501) staff       (20)      364 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/config/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2057 2024-04-12 14:51:39.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/config/apimanager.py
--rw-r--r--   0 wuhan      (501) staff       (20)      872 2023-07-22 01:54:36.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/config/configloader.py
--rw-r--r--   0 wuhan      (501) staff       (20)     4116 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/config/influxdb2factory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2555 2024-01-23 06:24:43.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/config/influxfactory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2297 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/config/mongofactory.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2725 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/config/secretmanagerbase.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2133 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/config/slackwebhookfactory.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.954652 cryptopian_infra-0.1.4/src/cryptopian_infra/infra/
--rw-r--r--   0 wuhan      (501) staff       (20)      145 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/infra/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1403 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/infra/duration.py
--rw-r--r--   0 wuhan      (501) staff       (20)     2112 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/infra/emailclient.py
--rw-r--r--   0 wuhan      (501) staff       (20)      169 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/infra/gracefullystopdocker.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1013 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/infra/stopwatch.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.955027 cryptopian_infra-0.1.4/src/cryptopian_infra/mongo/
--rw-r--r--   0 wuhan      (501) staff       (20)       45 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/mongo/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1591 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/mongo/mongoparameters.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1071 2024-03-29 08:43:35.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/sendalert.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.955953 cryptopian_infra-0.1.4/src/cryptopian_infra/threading/
--rw-r--r--   0 wuhan      (501) staff       (20)       80 2024-03-07 11:38:15.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/threading/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)      421 2024-03-07 12:56:51.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/threading/atomicaccstore.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1303 2024-03-10 04:46:21.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/threading/messagepump.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.957567 cryptopian_infra-0.1.4/src/cryptopian_infra/utils/
--rw-r--r--   0 wuhan      (501) staff       (20)       51 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/utils/__init__.py
--rw-r--r--   0 wuhan      (501) staff       (20)      346 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/utils/asyncutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)      626 2024-03-20 03:40:17.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/utils/datetimeutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)      124 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/utils/dictobj.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1017 2024-04-03 04:36:40.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/utils/dictutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)      133 2024-01-17 10:32:22.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/utils/listutils.py
--rw-r--r--   0 wuhan      (501) staff       (20)     1619 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.4/src/cryptopian_infra/utils/mathutils.py
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.958196 cryptopian_infra-0.1.4/src/cryptopian_infra.egg-info/
--rw-r--r--   0 wuhan      (501) staff       (20)     1218 2024-04-17 06:43:19.000000 cryptopian_infra-0.1.4/src/cryptopian_infra.egg-info/PKG-INFO
--rw-r--r--   0 wuhan      (501) staff       (20)     1579 2024-04-17 06:43:19.000000 cryptopian_infra-0.1.4/src/cryptopian_infra.egg-info/SOURCES.txt
--rw-r--r--   0 wuhan      (501) staff       (20)        1 2024-04-17 06:43:19.000000 cryptopian_infra-0.1.4/src/cryptopian_infra.egg-info/dependency_links.txt
--rw-r--r--   0 wuhan      (501) staff       (20)       91 2024-04-17 06:43:19.000000 cryptopian_infra-0.1.4/src/cryptopian_infra.egg-info/requires.txt
--rw-r--r--   0 wuhan      (501) staff       (20)       17 2024-04-17 06:43:19.000000 cryptopian_infra-0.1.4/src/cryptopian_infra.egg-info/top_level.txt
-drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-17 06:43:19.957758 cryptopian_infra-0.1.4/tests/
--rw-r--r--   0 wuhan      (501) staff       (20)      601 2024-03-06 06:30:32.000000 cryptopian_infra-0.1.4/tests/test_random.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.314020 cryptopian_infra-0.1.5/
+-rw-r--r--   0 wuhan      (501) staff       (20)     1063 2022-01-19 16:43:46.000000 cryptopian_infra-0.1.5/LICENSE
+-rw-r--r--   0 wuhan      (501) staff       (20)     1305 2024-04-24 02:11:23.313759 cryptopian_infra-0.1.5/PKG-INFO
+-rw-r--r--   0 wuhan      (501) staff       (20)      446 2024-03-07 06:40:10.000000 cryptopian_infra-0.1.5/README.md
+-rw-r--r--   0 wuhan      (501) staff       (20)      790 2024-04-24 02:10:54.000000 cryptopian_infra-0.1.5/pyproject.toml
+-rw-r--r--   0 wuhan      (501) staff       (20)       38 2024-04-24 02:11:23.314072 cryptopian_infra-0.1.5/setup.cfg
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.301718 cryptopian_infra-0.1.5/src/
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.303060 cryptopian_infra-0.1.5/src/cryptopian_infra/
+-rw-r--r--   0 wuhan      (501) staff       (20)        0 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/__init__.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.305530 cryptopian_infra-0.1.5/src/cryptopian_infra/alert/
+-rw-r--r--   0 wuhan      (501) staff       (20)      112 2024-03-31 08:31:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/alert/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1512 2024-01-15 10:05:02.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/alert/alert.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1819 2024-03-29 08:42:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/alert/alertwrapper.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1221 2024-03-31 08:31:29.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/alert/slackwebhook.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.307851 cryptopian_infra-0.1.5/src/cryptopian_infra/config/
+-rw-r--r--   0 wuhan      (501) staff       (20)      364 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/config/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2057 2024-04-12 14:51:39.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/config/apimanager.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      872 2023-07-22 01:54:36.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/config/configloader.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     4116 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/config/influxdb2factory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2555 2024-01-23 06:24:43.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/config/influxfactory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2297 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/config/mongofactory.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2725 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/config/secretmanagerbase.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2133 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/config/slackwebhookfactory.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.309709 cryptopian_infra-0.1.5/src/cryptopian_infra/infra/
+-rw-r--r--   0 wuhan      (501) staff       (20)      145 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/infra/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1403 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/infra/duration.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     2112 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/infra/emailclient.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      169 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/infra/gracefullystopdocker.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1013 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/infra/stopwatch.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.310297 cryptopian_infra-0.1.5/src/cryptopian_infra/mongo/
+-rw-r--r--   0 wuhan      (501) staff       (20)       45 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/mongo/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1591 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/mongo/mongoparameters.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1071 2024-03-29 08:43:35.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/sendalert.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.311211 cryptopian_infra-0.1.5/src/cryptopian_infra/threading/
+-rw-r--r--   0 wuhan      (501) staff       (20)       80 2024-03-07 11:38:15.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/threading/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      421 2024-03-07 12:56:51.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/threading/atomicaccstore.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1303 2024-03-10 04:46:21.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/threading/messagepump.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.312837 cryptopian_infra-0.1.5/src/cryptopian_infra/utils/
+-rw-r--r--   0 wuhan      (501) staff       (20)       51 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/utils/__init__.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      346 2023-07-21 11:41:37.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/utils/asyncutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      626 2024-03-20 03:40:17.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/utils/datetimeutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      124 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/utils/dictobj.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1017 2024-04-03 04:36:40.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/utils/dictutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)      133 2024-01-17 10:32:22.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/utils/listutils.py
+-rw-r--r--   0 wuhan      (501) staff       (20)     1619 2024-04-17 06:42:52.000000 cryptopian_infra-0.1.5/src/cryptopian_infra/utils/mathutils.py
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.313426 cryptopian_infra-0.1.5/src/cryptopian_infra.egg-info/
+-rw-r--r--   0 wuhan      (501) staff       (20)     1305 2024-04-24 02:11:23.000000 cryptopian_infra-0.1.5/src/cryptopian_infra.egg-info/PKG-INFO
+-rw-r--r--   0 wuhan      (501) staff       (20)     1579 2024-04-24 02:11:23.000000 cryptopian_infra-0.1.5/src/cryptopian_infra.egg-info/SOURCES.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)        1 2024-04-24 02:11:23.000000 cryptopian_infra-0.1.5/src/cryptopian_infra.egg-info/dependency_links.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)       91 2024-04-24 02:11:23.000000 cryptopian_infra-0.1.5/src/cryptopian_infra.egg-info/requires.txt
+-rw-r--r--   0 wuhan      (501) staff       (20)       17 2024-04-24 02:11:23.000000 cryptopian_infra-0.1.5/src/cryptopian_infra.egg-info/top_level.txt
+drwxr-xr-x   0 wuhan      (501) staff       (20)        0 2024-04-24 02:11:23.312994 cryptopian_infra-0.1.5/tests/
+-rw-r--r--   0 wuhan      (501) staff       (20)      601 2024-03-06 06:30:32.000000 cryptopian_infra-0.1.5/tests/test_random.py
```

### Comparing `cryptopian_infra-0.1.4/LICENSE` & `cryptopian_infra-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/PKG-INFO` & `cryptopian_infra-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: cryptopian_infra
-Version: 0.1.4
+Version: 0.1.5
 Summary: Cryptopian Infrastructure Library
 Author-email: Han Wu <xjohnwu@gmail.com>
+Project-URL: Source, https://github.com/Cryptopian001/cryptopian_infrastructure_python
 Project-URL: Homepage, https://github.com/Cryptopian001/cryptopian_infrastructure_python
 Project-URL: Issues, https://github.com/Cryptopian001/cryptopian_infrastructure_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/alert/alert.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/alert/alert.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/alert/alertwrapper.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/alert/alertwrapper.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/alert/slackwebhook.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/alert/slackwebhook.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/config/apimanager.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/config/apimanager.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/config/configloader.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/config/configloader.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/config/influxdb2factory.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/config/influxdb2factory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/config/influxfactory.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/config/influxfactory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/config/mongofactory.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/config/mongofactory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/config/secretmanagerbase.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/config/secretmanagerbase.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/config/slackwebhookfactory.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/config/slackwebhookfactory.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/infra/duration.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/infra/duration.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/infra/emailclient.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/infra/emailclient.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/infra/stopwatch.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/infra/stopwatch.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/mongo/mongoparameters.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/mongo/mongoparameters.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/sendalert.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/sendalert.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/threading/messagepump.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/threading/messagepump.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/utils/datetimeutils.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/utils/datetimeutils.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/utils/dictutils.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/utils/dictutils.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra/utils/mathutils.py` & `cryptopian_infra-0.1.5/src/cryptopian_infra/utils/mathutils.py`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra.egg-info/PKG-INFO` & `cryptopian_infra-0.1.5/src/cryptopian_infra.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: cryptopian_infra
-Version: 0.1.4
+Version: 0.1.5
 Summary: Cryptopian Infrastructure Library
 Author-email: Han Wu <xjohnwu@gmail.com>
+Project-URL: Source, https://github.com/Cryptopian001/cryptopian_infrastructure_python
 Project-URL: Homepage, https://github.com/Cryptopian001/cryptopian_infrastructure_python
 Project-URL: Issues, https://github.com/Cryptopian001/cryptopian_infrastructure_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `cryptopian_infra-0.1.4/src/cryptopian_infra.egg-info/SOURCES.txt` & `cryptopian_infra-0.1.5/src/cryptopian_infra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptopian_infra-0.1.4/tests/test_random.py` & `cryptopian_infra-0.1.5/tests/test_random.py`

 * *Files identical despite different names*

