# Comparing `tmp/hui-tools-0.3.2.tar.gz` & `tmp/hui-tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hui-tools-0.3.2.tar", last modified: Wed Apr 17 04:02:55 2024, max compression
+gzip compressed data, was "hui-tools-0.4.0.tar", last modified: Wed Apr 24 10:47:19 2024, max compression
```

## Comparing `hui-tools-0.3.2.tar` & `hui-tools-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.911946 hui-tools-0.3.2/
--rw-r--r--   0 liuminhui   (501) staff       (20)    11357 2023-07-29 10:14:17.000000 hui-tools-0.3.2/LICENSE
--rw-r--r--   0 liuminhui   (501) staff       (20)    17648 2024-04-17 04:02:55.911662 hui-tools-0.3.2/PKG-INFO
--rw-r--r--   0 liuminhui   (501) staff       (20)    15809 2024-04-15 11:39:36.000000 hui-tools-0.3.2/README.md
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.899506 hui-tools-0.3.2/hui_tools.egg-info/
--rw-r--r--   0 liuminhui   (501) staff       (20)    17648 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/PKG-INFO
--rw-r--r--   0 liuminhui   (501) staff       (20)     1520 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/SOURCES.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/dependency_links.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)      532 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/requires.txt
--rw-r--r--   0 liuminhui   (501) staff       (20)       15 2024-04-17 04:02:55.000000 hui-tools-0.3.2/hui_tools.egg-info/top_level.txt
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.899645 hui-tools-0.3.2/py_tools/
--rw-r--r--   0 liuminhui   (501) staff       (20)        1 2023-09-04 08:25:07.000000 hui-tools-0.3.2/py_tools/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.900761 hui-tools-0.3.2/py_tools/chatbot/
--rw-r--r--   0 liuminhui   (501) staff       (20)      128 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/chatbot/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)    11243 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/chatbot/app_server.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     5238 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/chatbot/chatbot.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     2385 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/chatbot/factory.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.900947 hui-tools-0.3.2/py_tools/connections/
--rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.901289 hui-tools-0.3.2/py_tools/connections/db/
--rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/db/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.902084 hui-tools-0.3.2/py_tools/connections/db/mysql/
--rw-r--r--   0 liuminhui   (501) staff       (20)      215 2024-03-28 15:06:17.000000 hui-tools-0.3.2/py_tools/connections/db/mysql/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)    20121 2024-04-17 03:58:06.000000 hui-tools-0.3.2/py_tools/connections/db/mysql/client.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1722 2024-04-17 03:58:06.000000 hui-tools-0.3.2/py_tools/connections/db/mysql/orm_model.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1452 2024-03-28 01:23:21.000000 hui-tools-0.3.2/py_tools/connections/db/redis_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.902784 hui-tools-0.3.2/py_tools/connections/http/
--rw-r--r--   0 liuminhui   (501) staff       (20)      158 2023-08-10 03:40:34.000000 hui-tools-0.3.2/py_tools/connections/http/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     8809 2023-09-28 06:51:00.000000 hui-tools-0.3.2/py_tools/connections/http/client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.903524 hui-tools-0.3.2/py_tools/connections/mq/
--rw-r--r--   0 liuminhui   (501) staff       (20)      185 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/mq/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      184 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/mq/kafka_client.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      187 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/connections/mq/rabbitmq_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.903913 hui-tools-0.3.2/py_tools/connections/oss/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2024-03-28 01:23:21.000000 hui-tools-0.3.2/py_tools/connections/oss/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1955 2024-03-28 01:23:21.000000 hui-tools-0.3.2/py_tools/connections/oss/minio_client.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.904133 hui-tools-0.3.2/py_tools/constants/
--rw-r--r--   0 liuminhui   (501) staff       (20)      171 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/constants/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.904430 hui-tools-0.3.2/py_tools/data_models/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/data_models/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      270 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/data_models/time.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.905002 hui-tools-0.3.2/py_tools/decorators/
--rw-r--r--   0 liuminhui   (501) staff       (20)      213 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/decorators/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     6380 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/decorators/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     4395 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/decorators/cache.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.906771 hui-tools-0.3.2/py_tools/enums/
--rw-r--r--   0 liuminhui   (501) staff       (20)      334 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/enums/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1699 2023-09-09 15:54:57.000000 hui-tools-0.3.2/py_tools/enums/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1234 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/enums/error.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/enums/feishu.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      452 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/enums/http.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      403 2023-09-09 15:58:16.000000 hui-tools-0.3.2/py_tools/enums/pub_biz.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-09-09 06:12:03.000000 hui-tools-0.3.2/py_tools/enums/time.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.907146 hui-tools-0.3.2/py_tools/exceptions/
--rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/exceptions/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     1141 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/exceptions/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.907367 hui-tools-0.3.2/py_tools/logging/
--rw-r--r--   0 liuminhui   (501) staff       (20)       26 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/logging/__init__.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.907787 hui-tools-0.3.2/py_tools/meta_cls/
--rw-r--r--   0 liuminhui   (501) staff       (20)       35 2023-09-04 07:12:03.000000 hui-tools-0.3.2/py_tools/meta_cls/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      963 2023-09-09 06:35:40.000000 hui-tools-0.3.2/py_tools/meta_cls/base.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.909807 hui-tools-0.3.2/py_tools/utils/
--rw-r--r--   0 liuminhui   (501) staff       (20)      166 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/utils/__init__.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/utils/base.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     5992 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/utils/excel.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-09-09 16:15:14.000000 hui-tools-0.3.2/py_tools/utils/func.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.3.2/py_tools/utils/mask.py
--rw-r--r--   0 liuminhui   (501) staff       (20)      179 2023-09-09 16:16:35.000000 hui-tools-0.3.2/py_tools/utils/serializer.py
--rw-r--r--   0 liuminhui   (501) staff       (20)     6859 2023-09-09 06:33:24.000000 hui-tools-0.3.2/py_tools/utils/time.py
--rw-r--r--   0 liuminhui   (501) staff       (20)       38 2024-04-17 04:02:55.912003 hui-tools-0.3.2/setup.cfg
--rw-r--r--   0 liuminhui   (501) staff       (20)     2289 2024-04-17 04:02:44.000000 hui-tools-0.3.2/setup.py
-drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-17 04:02:55.910281 hui-tools-0.3.2/tests/
--rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.3.2/tests/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.314090 hui-tools-0.4.0/
+-rw-r--r--   0 liuminhui   (501) staff       (20)    11357 2023-07-29 10:14:17.000000 hui-tools-0.4.0/LICENSE
+-rw-r--r--   0 liuminhui   (501) staff       (20)    17724 2024-04-24 10:47:19.313742 hui-tools-0.4.0/PKG-INFO
+-rw-r--r--   0 liuminhui   (501) staff       (20)    15809 2024-04-15 11:39:36.000000 hui-tools-0.4.0/README.md
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.301820 hui-tools-0.4.0/hui_tools.egg-info/
+-rw-r--r--   0 liuminhui   (501) staff       (20)    17724 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/PKG-INFO
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1594 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)      562 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/requires.txt
+-rw-r--r--   0 liuminhui   (501) staff       (20)       15 2024-04-24 10:47:19.000000 hui-tools-0.4.0/hui_tools.egg-info/top_level.txt
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.302026 hui-tools-0.4.0/py_tools/
+-rw-r--r--   0 liuminhui   (501) staff       (20)        1 2023-09-04 08:25:07.000000 hui-tools-0.4.0/py_tools/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.303373 hui-tools-0.4.0/py_tools/chatbot/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      128 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/chatbot/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    11243 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/chatbot/app_server.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5238 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/chatbot/chatbot.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2385 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/chatbot/factory.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.303550 hui-tools-0.4.0/py_tools/connections/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.303909 hui-tools-0.4.0/py_tools/connections/db/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      182 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/db/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.304868 hui-tools-0.4.0/py_tools/connections/db/mysql/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      215 2024-03-28 15:06:17.000000 hui-tools-0.4.0/py_tools/connections/db/mysql/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)    20121 2024-04-17 03:58:06.000000 hui-tools-0.4.0/py_tools/connections/db/mysql/client.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1722 2024-04-17 03:58:06.000000 hui-tools-0.4.0/py_tools/connections/db/mysql/orm_model.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2581 2024-04-24 02:13:05.000000 hui-tools-0.4.0/py_tools/connections/db/redis_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.305331 hui-tools-0.4.0/py_tools/connections/http/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      158 2023-08-10 03:40:34.000000 hui-tools-0.4.0/py_tools/connections/http/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     8809 2023-09-28 06:51:00.000000 hui-tools-0.4.0/py_tools/connections/http/client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.306038 hui-tools-0.4.0/py_tools/connections/mq/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      185 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/mq/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      184 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/mq/kafka_client.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      187 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/connections/mq/rabbitmq_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.306458 hui-tools-0.4.0/py_tools/connections/oss/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2024-03-28 01:23:21.000000 hui-tools-0.4.0/py_tools/connections/oss/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1955 2024-03-28 01:23:21.000000 hui-tools-0.4.0/py_tools/connections/oss/minio_client.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.306690 hui-tools-0.4.0/py_tools/constants/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      171 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/constants/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.307244 hui-tools-0.4.0/py_tools/data_models/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/data_models/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      270 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/data_models/time.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2674 2024-04-24 04:49:33.000000 hui-tools-0.4.0/py_tools/data_models/unit.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.307763 hui-tools-0.4.0/py_tools/decorators/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      213 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/decorators/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     6380 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/decorators/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     4831 2024-04-24 02:14:22.000000 hui-tools-0.4.0/py_tools/decorators/cache.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.309430 hui-tools-0.4.0/py_tools/enums/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      334 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/enums/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2304 2024-04-24 03:43:33.000000 hui-tools-0.4.0/py_tools/enums/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1234 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/enums/error.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/enums/feishu.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      452 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/enums/http.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      486 2024-04-24 03:43:33.000000 hui-tools-0.4.0/py_tools/enums/pub_biz.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      573 2023-09-09 06:12:03.000000 hui-tools-0.4.0/py_tools/enums/time.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.309841 hui-tools-0.4.0/py_tools/exceptions/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/exceptions/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1141 2023-09-09 16:15:14.000000 hui-tools-0.4.0/py_tools/exceptions/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.310107 hui-tools-0.4.0/py_tools/logging/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       26 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/logging/__init__.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.310519 hui-tools-0.4.0/py_tools/meta_cls/
+-rw-r--r--   0 liuminhui   (501) staff       (20)       35 2023-09-04 07:12:03.000000 hui-tools-0.4.0/py_tools/meta_cls/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      963 2023-09-09 06:35:40.000000 hui-tools-0.4.0/py_tools/meta_cls/base.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.312122 hui-tools-0.4.0/py_tools/utils/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      166 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/utils/__init__.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     1067 2024-04-24 10:35:38.000000 hui-tools-0.4.0/py_tools/utils/aio.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      110 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/utils/base.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     5992 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/utils/excel.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      951 2024-04-24 03:52:42.000000 hui-tools-0.4.0/py_tools/utils/func.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      191 2023-07-29 10:14:17.000000 hui-tools-0.4.0/py_tools/utils/mask.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)      179 2023-09-09 16:16:35.000000 hui-tools-0.4.0/py_tools/utils/serializer.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     6538 2024-04-24 02:48:33.000000 hui-tools-0.4.0/py_tools/utils/time.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)     4592 2024-04-24 03:58:59.000000 hui-tools-0.4.0/py_tools/utils/tree.py
+-rw-r--r--   0 liuminhui   (501) staff       (20)       38 2024-04-24 10:47:19.314146 hui-tools-0.4.0/setup.cfg
+-rw-r--r--   0 liuminhui   (501) staff       (20)     2307 2024-04-24 10:45:44.000000 hui-tools-0.4.0/setup.py
+drwxr-xr-x   0 liuminhui   (501) staff       (20)        0 2024-04-24 10:47:19.312263 hui-tools-0.4.0/tests/
+-rw-r--r--   0 liuminhui   (501) staff       (20)      173 2023-07-29 10:14:17.000000 hui-tools-0.4.0/tests/__init__.py
```

### Comparing `hui-tools-0.3.2/LICENSE` & `hui-tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/PKG-INFO` & `hui-tools-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: hui-tools
-Version: 0.3.2
+Version: 0.4.0
 Home-page: https://github.com/HuiDBK/py-tools
 Author: hui
 Author-email: huidbk@163.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru<0.8,>=0.7.0
 Requires-Dist: pydantic<3,>=2.1.1
+Requires-Dist: asgiref==3.8.1
 Provides-Extra: db-orm
 Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "db-orm"
 Requires-Dist: aiomysql==0.2.0; extra == "db-orm"
 Provides-Extra: db-redis
 Requires-Dist: redis>=4.5.4; extra == "db-redis"
 Provides-Extra: minio
 Requires-Dist: minio==7.1.17; extra == "minio"
@@ -28,26 +29,27 @@
 Requires-Dist: requests==2.31.0; extra == "http-client"
 Provides-Extra: time-tools
 Requires-Dist: python-dateutil==2.8.2; extra == "time-tools"
 Provides-Extra: excel-tools
 Requires-Dist: pandas==1.3.5; extra == "excel-tools"
 Requires-Dist: openpyxl==3.0.10; extra == "excel-tools"
 Provides-Extra: all
-Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "all"
-Requires-Dist: requests==2.31.0; extra == "all"
-Requires-Dist: pydantic<3,>=2.1.1; extra == "all"
-Requires-Dist: pandas==1.3.5; extra == "all"
-Requires-Dist: httpx==0.24.1; extra == "all"
-Requires-Dist: openpyxl==3.0.10; extra == "all"
 Requires-Dist: cacheout==0.14.1; extra == "all"
+Requires-Dist: asgiref==3.8.1; extra == "all"
 Requires-Dist: minio==7.1.17; extra == "all"
-Requires-Dist: redis>=4.5.4; extra == "all"
+Requires-Dist: python-dateutil==2.8.2; extra == "all"
 Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
+Requires-Dist: openpyxl==3.0.10; extra == "all"
+Requires-Dist: redis>=4.5.4; extra == "all"
+Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "all"
+Requires-Dist: httpx==0.24.1; extra == "all"
+Requires-Dist: pandas==1.3.5; extra == "all"
 Requires-Dist: aiomysql==0.2.0; extra == "all"
-Requires-Dist: python-dateutil==2.8.2; extra == "all"
+Requires-Dist: pydantic<3,>=2.1.1; extra == "all"
+Requires-Dist: requests==2.31.0; extra == "all"
 
 # Py-Tools
 
 > Py-Tools 是一个实用的 Python 工具集和可复用组件库，旨在简化常见任务，提高 Python 项目的开发效率。
 > 
 > 设计细节请移步到掘金查看：https://juejin.cn/column/7131286129713610766
```

### Comparing `hui-tools-0.3.2/README.md` & `hui-tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/hui_tools.egg-info/PKG-INFO` & `hui-tools-0.4.0/hui_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: hui-tools
-Version: 0.3.2
+Version: 0.4.0
 Home-page: https://github.com/HuiDBK/py-tools
 Author: hui
 Author-email: huidbk@163.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru<0.8,>=0.7.0
 Requires-Dist: pydantic<3,>=2.1.1
+Requires-Dist: asgiref==3.8.1
 Provides-Extra: db-orm
 Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "db-orm"
 Requires-Dist: aiomysql==0.2.0; extra == "db-orm"
 Provides-Extra: db-redis
 Requires-Dist: redis>=4.5.4; extra == "db-redis"
 Provides-Extra: minio
 Requires-Dist: minio==7.1.17; extra == "minio"
@@ -28,26 +29,27 @@
 Requires-Dist: requests==2.31.0; extra == "http-client"
 Provides-Extra: time-tools
 Requires-Dist: python-dateutil==2.8.2; extra == "time-tools"
 Provides-Extra: excel-tools
 Requires-Dist: pandas==1.3.5; extra == "excel-tools"
 Requires-Dist: openpyxl==3.0.10; extra == "excel-tools"
 Provides-Extra: all
-Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "all"
-Requires-Dist: requests==2.31.0; extra == "all"
-Requires-Dist: pydantic<3,>=2.1.1; extra == "all"
-Requires-Dist: pandas==1.3.5; extra == "all"
-Requires-Dist: httpx==0.24.1; extra == "all"
-Requires-Dist: openpyxl==3.0.10; extra == "all"
 Requires-Dist: cacheout==0.14.1; extra == "all"
+Requires-Dist: asgiref==3.8.1; extra == "all"
 Requires-Dist: minio==7.1.17; extra == "all"
-Requires-Dist: redis>=4.5.4; extra == "all"
+Requires-Dist: python-dateutil==2.8.2; extra == "all"
 Requires-Dist: loguru<0.8,>=0.7.0; extra == "all"
+Requires-Dist: openpyxl==3.0.10; extra == "all"
+Requires-Dist: redis>=4.5.4; extra == "all"
+Requires-Dist: sqlalchemy[asyncio]==2.0.20; extra == "all"
+Requires-Dist: httpx==0.24.1; extra == "all"
+Requires-Dist: pandas==1.3.5; extra == "all"
 Requires-Dist: aiomysql==0.2.0; extra == "all"
-Requires-Dist: python-dateutil==2.8.2; extra == "all"
+Requires-Dist: pydantic<3,>=2.1.1; extra == "all"
+Requires-Dist: requests==2.31.0; extra == "all"
 
 # Py-Tools
 
 > Py-Tools 是一个实用的 Python 工具集和可复用组件库，旨在简化常见任务，提高 Python 项目的开发效率。
 > 
 > 设计细节请移步到掘金查看：https://juejin.cn/column/7131286129713610766
```

### Comparing `hui-tools-0.3.2/hui_tools.egg-info/SOURCES.txt` & `hui-tools-0.4.0/hui_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 py_tools/connections/mq/kafka_client.py
 py_tools/connections/mq/rabbitmq_client.py
 py_tools/connections/oss/__init__.py
 py_tools/connections/oss/minio_client.py
 py_tools/constants/__init__.py
 py_tools/data_models/__init__.py
 py_tools/data_models/time.py
+py_tools/data_models/unit.py
 py_tools/decorators/__init__.py
 py_tools/decorators/base.py
 py_tools/decorators/cache.py
 py_tools/enums/__init__.py
 py_tools/enums/base.py
 py_tools/enums/error.py
 py_tools/enums/feishu.py
@@ -39,14 +40,16 @@
 py_tools/enums/time.py
 py_tools/exceptions/__init__.py
 py_tools/exceptions/base.py
 py_tools/logging/__init__.py
 py_tools/meta_cls/__init__.py
 py_tools/meta_cls/base.py
 py_tools/utils/__init__.py
+py_tools/utils/aio.py
 py_tools/utils/base.py
 py_tools/utils/excel.py
 py_tools/utils/func.py
 py_tools/utils/mask.py
 py_tools/utils/serializer.py
 py_tools/utils/time.py
+py_tools/utils/tree.py
 tests/__init__.py
```

### Comparing `hui-tools-0.3.2/hui_tools.egg-info/requires.txt` & `hui-tools-0.4.0/hui_tools.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 loguru<0.8,>=0.7.0
 pydantic<3,>=2.1.1
+asgiref==3.8.1
 
 [all]
-sqlalchemy[asyncio]==2.0.20
-requests==2.31.0
-pydantic<3,>=2.1.1
-pandas==1.3.5
-httpx==0.24.1
-openpyxl==3.0.10
 cacheout==0.14.1
+asgiref==3.8.1
 minio==7.1.17
-redis>=4.5.4
+python-dateutil==2.8.2
 loguru<0.8,>=0.7.0
+openpyxl==3.0.10
+redis>=4.5.4
+sqlalchemy[asyncio]==2.0.20
+httpx==0.24.1
+pandas==1.3.5
 aiomysql==0.2.0
-python-dateutil==2.8.2
+pydantic<3,>=2.1.1
+requests==2.31.0
 
 [chatbot]
 requests==2.31.0
 cacheout==0.14.1
 
 [db-orm]
 sqlalchemy[asyncio]==2.0.20
```

### Comparing `hui-tools-0.3.2/py_tools/chatbot/app_server.py` & `hui-tools-0.4.0/py_tools/chatbot/app_server.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/chatbot/chatbot.py` & `hui-tools-0.4.0/py_tools/chatbot/chatbot.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/chatbot/factory.py` & `hui-tools-0.4.0/py_tools/chatbot/factory.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/connections/db/mysql/client.py` & `hui-tools-0.4.0/py_tools/connections/db/mysql/client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/connections/db/mysql/orm_model.py` & `hui-tools-0.4.0/py_tools/connections/db/mysql/orm_model.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/connections/http/client.py` & `hui-tools-0.4.0/py_tools/connections/http/client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/connections/oss/minio_client.py` & `hui-tools-0.4.0/py_tools/connections/oss/minio_client.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/decorators/base.py` & `hui-tools-0.4.0/py_tools/decorators/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/decorators/cache.py` & `hui-tools-0.4.0/py_tools/decorators/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,145 +3,155 @@
 # @Author: Hui
 # @Desc: { 缓存装饰器模块 }
 # @Date: 2023/05/03 19:23
 import asyncio
 import functools
 import hashlib
 import json
+from datetime import timedelta
+from typing import Union
+
+import cacheout
 from pydantic import BaseModel, Field
-from typing import Type
+from redis import Redis
+from redis import asyncio as aioredis
+
 from py_tools import constants
 
 
 class CacheMeta(BaseModel):
     """缓存元信息"""
 
     key: str = Field(description="缓存的key")
-    ttl: int = Field(description="缓存有效期")
-    cache_type: str = Field(description="缓存的类型（Redis、Memcached等）")
+    ttl: Union[int, timedelta] = Field(description="缓存有效期")
+    cache_client: str = Field(description="缓存的客户端（Redis、Memcached等）")
     data_type: str = Field(description="缓存的数据类型（str、list、hash、set）")
 
 
 class BaseCacheProxy(object):
-    """缓存代理抽象类"""
+    """缓存代理基类"""
 
     def __init__(self, cache_client):
         self.cache_client = cache_client  # 具体的缓存客户端，例如Redis、Memcached等
 
-    def set(self, key, value, ttl):
-        raise NotImplemented
+    def set(self, key: str, value: str, ttl: int):
+        raise NotImplementedError
 
     def get(self, key):
-        raise NotImplemented
+        cache_data = self.cache_client.get(key)
+        return cache_data
 
 
 class RedisCacheProxy(BaseCacheProxy):
-    """redis缓存代理"""
+    """同步redis缓存代理"""
 
-    def set(self, key, value, ttl):
-        value = json.dumps(value)
-        self.cache_client.set(key, value, ttl)
+    def __init__(self, cache_client: Redis):
+        super().__init__(cache_client)
 
-    def get(self, key):
-        cache_data = self.cache_client.get(key)
-        cache_data = json.loads(cache_data)
-        return cache_data
+    def set(self, key, value, ttl):
+        self.cache_client.setex(name=key, value=value, time=ttl)
 
 
 class AsyncRedisCacheProxy(BaseCacheProxy):
-    """异步缓存代理"""
+    """异步Redis缓存代理"""
+
+    def __init__(self, cache_client: aioredis.Redis):
+        super().__init__(cache_client)
 
     async def set(self, key, value, ttl):
-        value = json.dumps(value)
-        await self.cache_client.set(key, value, ttl)
+        await self.cache_client.setex(name=key, value=value, time=ttl)
 
     async def get(self, key):
         cache_data = await self.cache_client.get(key)
-        cache_data = json.loads(cache_data)
         return cache_data
 
 
+class MemoryCacheProxy(BaseCacheProxy):
+    """系统内存缓存代理"""
+
+    def __init__(self, cache_client: cacheout.Cache):
+        super().__init__(cache_client)
+
+    def set(self, key, value, ttl):
+        self.cache_client.set(key=key, value=value, ttl=ttl)
+
+
+MEMORY_PROXY = MemoryCacheProxy(cache_client=cacheout.Cache(maxsize=1024))
+
+
 def cache_json(
-        cache_proxy: Type[BaseCacheProxy],
-        key: str = None,
-        ttl: int = 60,
-        cache_meta: CacheMeta = None,
-        def_key_prefix: str = constants.CACHE_KEY_PREFIX,
+    cache_proxy: BaseCacheProxy = MEMORY_PROXY,
+    key_prefix: str = constants.CACHE_KEY_PREFIX,
+    ttl: Union[int, timedelta] = 60,
 ):
     """
     缓存装饰器（仅支持缓存能够json序列化的数据）
     Args:
-        cache_proxy: 缓存代理对象
-        key: 缓存的key
+        cache_proxy: 缓存代理客户端, 默认系统内存
         ttl: 过期时间 默认60s
-        cache_meta: 缓存元信息
-        def_key_prefix: 默认的key前缀, 再未指定key时使用
+        key_prefix: 默认的key前缀
 
     Returns:
     """
-    if cache_meta:
-        # 有元信息直接覆盖key, ttl
-        key = cache_meta.key
-        ttl = cache_meta.ttl
+    key_prefix = f"{key_prefix}:cache_json"
+    if isinstance(ttl, timedelta):
+        ttl = int(ttl.total_seconds())
 
     def _cache(func):
-
         def _gen_key(*args, **kwargs):
             """生成缓存的key"""
 
-            nonlocal key
-            if not key:
-                # 没有传递key信息，根据函数信息与参数生成
-                # key => 函数所在模块:函数名:函数位置参数:函数关键字参数 进行hash
-                param_args_str = ",".join([str(arg) for arg in args])
-                param_kwargs_str = ",".join(sorted([f"{k}:{v}" for k, v in kwargs.items()]))
-                hash_str = f"{func.__module__}:{func.__name__}:{param_args_str}:{param_kwargs_str}"
-                has_result = hashlib.md5(hash_str.encode()).hexdigest()
-
-                # 根据哈希结果生成key 默认前缀:函数所在模块:函数名:hash
-                key = f"{def_key_prefix}:{func.__module__}:{func.__name__}:{has_result}"
-
-            return key
+            # 没有传递key信息，根据函数信息与参数生成
+            # key => 函数所在模块:函数名:函数位置参数:函数关键字参数 进行hash
+            param_args_str = ",".join([str(arg) for arg in args])
+            param_kwargs_str = ",".join(sorted([f"{k}:{v}" for k, v in kwargs.items()]))
+            hash_str = f"{func.__module__}:{func.__name__}:{param_args_str}:{param_kwargs_str}"
+            hash_ret = hashlib.sha256(hash_str.encode()).hexdigest()
+
+            # 根据哈希结果生成key 默认前缀:函数所在模块:函数名:hash
+            hash_key = f"{key_prefix}:{func.__module__}:{func.__name__}:{hash_ret}"
+            return hash_key
 
         @functools.wraps(func)
         def sync_wrapper(*args, **kwargs):
             """同步处理"""
 
             # 生成缓存的key
-            _key = _gen_key(*args, **kwargs)
+            hash_key = _gen_key(*args, **kwargs)
 
             # 先从缓存获取数据
-            cache_data = cache_proxy.get(_key)
+            cache_data = cache_proxy.get(hash_key)
             if cache_data:
                 # 有直接返回
-                return cache_data
+                print(f"命中缓存: {hash_key}")
+                return json.loads(cache_data)
 
             # 没有，执行函数获取结果
             ret = func(*args, **kwargs)
 
             # 缓存结果
-            cache_proxy.set(key=_key, value=ret, ttl=ttl)
+            cache_proxy.set(key=hash_key, value=json.dumps(ret), ttl=ttl)
             return ret
 
         @functools.wraps(func)
         async def async_wrapper(*args, **kwargs):
             """异步处理"""
 
             # 生成缓存的key
-            _key = _gen_key(*args, **kwargs)
+            hash_key = _gen_key(*args, **kwargs)
 
             # 先从缓存获取数据
-            cache_data = await cache_proxy.get(_key)
+            cache_data = await cache_proxy.get(hash_key)
             if cache_data:
                 # 有直接返回
-                return cache_data
+                return json.loads(cache_data)
 
             # 没有，执行函数获取结果
             ret = await func(*args, **kwargs)
 
             # 缓存结果
-            await cache_proxy.set(key=_key, value=ret, ttl=ttl)
+            await cache_proxy.set(key=hash_key, value=json.dumps(ret), ttl=ttl)
             return ret
 
         return async_wrapper if asyncio.iscoroutinefunction(func) else sync_wrapper
 
     return _cache
```

### Comparing `hui-tools-0.3.2/py_tools/enums/base.py` & `hui-tools-0.4.0/py_tools/enums/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,43 +23,60 @@
         else:
             obj = object.__new__(cls)
         obj._value_ = value
         obj.desc = desc
         return obj
 
     @classmethod
-    def get_members(cls, exclude_enums: list = None, only_value: bool = False) -> list:
+    def get_members(cls, exclude_enums: list = None, only_value: bool = False, only_desc: bool = False) -> list:
         """
         获取枚举的所有成员
         Args:
             exclude_enums: 排除的枚举类列表
-            only_value: 是否只需要成员的值，默认False
+            only_value: 只需要成员的值，默认False
+            only_desc: 只需要成员的desc，默认False
 
         Returns: 枚举成员列表 or 枚举成员值列表
 
         """
         members = list(cls)
         if exclude_enums:
             # 排除指定枚举
             members = [member for member in members if member not in exclude_enums]
 
         if only_value:
             # 只需要成员的值
             members = [member.value for member in members]
+            return members
+
+        if only_desc:
+            # 只需要成员的desc
+            members = [member.desc for member in members]
+            return members
 
         return members
 
     @classmethod
     def get_values(cls, exclude_enums: list = None):
         return cls.get_members(exclude_enums=exclude_enums, only_value=True)
 
     @classmethod
     def get_names(cls):
         return list(cls._member_names_)
 
+    @classmethod
+    def get_desc(cls, exclude_enums: list = None):
+        return cls.get_members(exclude_enums=exclude_enums, only_desc=True)
+
+    @classmethod
+    def get_value_by_desc(cls, enum_desc):
+        members = cls.get_members()
+        member_dic = {member.desc: member.value for member in members}
+        return member_dic.get(enum_desc)
+
 
 class StrEnum(str, BaseEnum):
     """字符串枚举"""
     pass
 
 
 class IntEnum(int, BaseEnum):
```

### Comparing `hui-tools-0.3.2/py_tools/enums/error.py` & `hui-tools-0.4.0/py_tools/enums/error.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/enums/feishu.py` & `hui-tools-0.4.0/py_tools/enums/feishu.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/enums/time.py` & `hui-tools-0.4.0/py_tools/enums/time.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/exceptions/base.py` & `hui-tools-0.4.0/py_tools/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/meta_cls/base.py` & `hui-tools-0.4.0/py_tools/meta_cls/base.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/utils/excel.py` & `hui-tools-0.4.0/py_tools/utils/excel.py`

 * *Files identical despite different names*

### Comparing `hui-tools-0.3.2/py_tools/utils/time.py` & `hui-tools-0.4.0/py_tools/utils/time.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 # -*- coding: utf-8 -*-
 # @Author: Hui
 # @Desc: { 时间工具类模块 }
 # @Date: 2022/11/26 16:08
 
 import time
 from datetime import datetime
-from typing import Type
 
 from dateutil.relativedelta import relativedelta
 
-from py_tools.data_models.time import DateDiff
 from py_tools.meta_cls import SingletonMetaCls
 from py_tools.enums import TimeFormatEnum
 
 
 class TimeUtil(metaclass=SingletonMetaCls):
     """
     时间工具类
@@ -93,32 +91,24 @@
         return datetime.fromtimestamp(timestamp)
 
     @property
     def timestamp(self) -> float:
         """获取 datetime 对象的时间戳"""
         return self.datetime_obj.timestamp()
 
-    def difference_in_detail(self, datetime_obj: datetime):
+    def date_diff(self, datetime_obj: datetime):
         """
         计算两个日期之间的差值详情
         Args:
             datetime_obj: 时间对象
 
         Returns: DateDiff
         """
         delta = relativedelta(self.datetime_obj, datetime_obj)
-
-        return DateDiff(
-            years=abs(delta.years),
-            months=abs(delta.months),
-            days=abs(delta.days),
-            hours=abs(delta.hours),
-            minutes=abs(delta.minutes),
-            seconds=abs(delta.seconds),
-        )
+        return delta
 
     def start_of_week(self) -> datetime:
         """获取本周的开始日期（周一）"""
         return self.datetime_obj - relativedelta(days=self.datetime_obj.weekday())
 
     def end_of_week(self) -> datetime:
         """获取本周的结束日期（周日）"""
```

### Comparing `hui-tools-0.3.2/setup.py` & `hui-tools-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 from functools import reduce
 
 from setuptools import find_packages, setup
 
 
 class PKGManager:
     name = "hui-tools"
-    version = "0.3.2"
+    version = "0.4.0"
     author = "hui"
     author_email = "huidbk@163.com"
 
     @classmethod
     def get_pkg_desc(cls):
         """获取包描述"""
         with open("README.md", "r") as f:
             long_description = f.read()
         return long_description
 
     @classmethod
     def get_install_requires(cls):
         """获取必须安装依赖"""
-        requires = ["loguru>=0.7.0,<0.8", "pydantic>=2.1.1,<3"]
+        requires = ["loguru>=0.7.0,<0.8", "pydantic>=2.1.1,<3", "asgiref==3.8.1"]
         return requires
 
     @classmethod
     def get_extras_require(cls):
         """
         可选的依赖
         """
```

