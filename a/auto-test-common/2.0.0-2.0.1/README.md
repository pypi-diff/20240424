# Comparing `tmp/auto-test-common-2.0.0.tar.gz` & `tmp/auto-test-common-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-2.0.0.tar", last modified: Mon Apr 22 00:32:02 2024, max compression
+gzip compressed data, was "auto-test-common-2.0.1.tar", last modified: Wed Apr 24 06:12:41 2024, max compression
```

## Comparing `auto-test-common-2.0.0.tar` & `auto-test-common-2.0.1.tar`

### file list

```diff
@@ -1,75 +1,78 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.096751 auto-test-common-2.0.0/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-22 00:32:02.096876 auto-test-common-2.0.0/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.058120 auto-test-common-2.0.0/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1726 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      653 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-22 00:32:01.000000 auto-test-common-2.0.0/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.058475 auto-test-common-2.0.0/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.0/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.060533 auto-test-common-2.0.0/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.0/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    12431 2024-04-10 07:06:14.000000 auto-test-common-2.0.0/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     7820 2024-03-12 08:21:25.000000 auto-test-common-2.0.0/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    14203 2024-03-27 03:21:56.000000 auto-test-common-2.0.0/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.063182 auto-test-common-2.0.0/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.0/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     7336 2024-04-11 08:58:42.000000 auto-test-common-2.0.0/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.0/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.064138 auto-test-common-2.0.0/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.0/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.0/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.067462 auto-test-common-2.0.0/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.0/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    25952 2024-04-16 09:39:15.000000 auto-test-common-2.0.0/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)    12127 2024-04-11 02:38:06.000000 auto-test-common-2.0.0/common/data/handle_common.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.0/common/data/template_data.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.072388 auto-test-common-2.0.0/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.0/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.0/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.0/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1991 2024-03-28 03:06:03.000000 auto-test-common-2.0.0/common/db/handle_mongo.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.075106 auto-test-common-2.0.0/common/driver/
--rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.0/common/driver/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.0/common/driver/api_page.py
--rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.0/common/driver/ui_page.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.080418 auto-test-common-2.0.0/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4570 2024-03-26 09:07:48.000000 auto-test-common-2.0.0/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.0/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-18 06:49:09.000000 auto-test-common-2.0.0/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.0/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-09 02:10:42.000000 auto-test-common-2.0.0/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.0/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.081365 auto-test-common-2.0.0/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.0/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.0/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.085284 auto-test-common-2.0.0/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.0/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.0/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.0/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.0/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.0/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    17680 2024-03-12 01:23:36.000000 auto-test-common-2.0.0/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-22 00:32:02.095960 auto-test-common-2.0.0/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.0/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1527 2024-03-22 00:22:36.000000 auto-test-common-2.0.0/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5156 2024-03-21 01:50:37.000000 auto-test-common-2.0.0/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-08 01:05:24.000000 auto-test-common-2.0.0/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7770 2024-03-20 05:09:33.000000 auto-test-common-2.0.0/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     5415 2024-03-26 08:31:29.000000 auto-test-common-2.0.0/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-16 09:39:15.000000 auto-test-common-2.0.0/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.0/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.0/common/plugin/my_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.0/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    23046 2024-03-27 01:31:57.000000 auto-test-common-2.0.0/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.0/common/plugin/template_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2090 2024-03-20 05:11:35.000000 auto-test-common-2.0.0/common/plugin/yaml_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2024-04-22 00:32:02.097529 auto-test-common-2.0.0/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1948 2024-03-08 08:28:03.000000 auto-test-common-2.0.0/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.441798 auto-test-common-2.0.1/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-24 06:12:41.441934 auto-test-common-2.0.1/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.409088 auto-test-common-2.0.1/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      628 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1821 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      749 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2024-04-24 06:12:41.000000 auto-test-common-2.0.1/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.409397 auto-test-common-2.0.1/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-2.0.1/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.411258 auto-test-common-2.0.1/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-2.0.1/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5471 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/autotest/assert_function.py
+-rw-r--r--   0 edz        (502) staff       (20)    12844 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     8211 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    14203 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.417272 auto-test-common-2.0.1/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-2.0.1/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     7645 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3808 2023-12-19 05:35:52.000000 auto-test-common-2.0.1/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.418249 auto-test-common-2.0.1/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.1/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2808 2023-08-29 05:34:25.000000 auto-test-common-2.0.1/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.426408 auto-test-common-2.0.1/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-2.0.1/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    25961 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)      426 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/data/eval_data_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)     7933 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/data/faker_handle.py
+-rw-r--r--   0 edz        (502) staff       (20)    12614 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/data/handle_common.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-12 02:50:37.000000 auto-test-common-2.0.1/common/data/template_data.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.429420 auto-test-common-2.0.1/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.1/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-2.0.1/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-2.0.1/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1991 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/db/handle_mongo.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.430460 auto-test-common-2.0.1/common/driver/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2023-06-05 07:58:39.000000 auto-test-common-2.0.1/common/driver/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)      127 2023-06-05 08:02:38.000000 auto-test-common-2.0.1/common/driver/api_page.py
+-rw-r--r--   0 edz        (502) staff       (20)     3037 2023-06-05 08:02:38.000000 auto-test-common-2.0.1/common/driver/ui_page.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.433243 auto-test-common-2.0.1/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     5030 2024-04-24 05:16:27.000000 auto-test-common-2.0.1/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-2.0.1/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    10873 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-2.0.1/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2360 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)      955 2023-06-01 02:02:40.000000 auto-test-common-2.0.1/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.433876 auto-test-common-2.0.1/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-2.0.1/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-2.0.1/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.436114 auto-test-common-2.0.1/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3385 2024-01-10 05:46:42.000000 auto-test-common-2.0.1/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-2.0.1/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-2.0.1/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7734 2023-11-29 00:51:05.000000 auto-test-common-2.0.1/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7268 2023-11-30 01:02:07.000000 auto-test-common-2.0.1/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    17680 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2024-04-24 06:12:41.441485 auto-test-common-2.0.1/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-2.0.1/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1527 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5156 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10554 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7770 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     5415 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13056 2024-04-24 05:10:23.000000 auto-test-common-2.0.1/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-2.0.1/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)       30 2023-06-08 05:24:28.000000 auto-test-common-2.0.1/common/plugin/my_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-2.0.1/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    23046 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     1421 2023-08-23 05:46:04.000000 auto-test-common-2.0.1/common/plugin/template_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2090 2024-04-24 00:46:49.000000 auto-test-common-2.0.1/common/plugin/yaml_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2024-04-24 06:12:41.442641 auto-test-common-2.0.1/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     2099 2024-04-24 05:10:23.000000 auto-test-common-2.0.1/setup.py
```

### Comparing `auto-test-common-2.0.0/PKG-INFO` & `auto-test-common-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.0
+Version: 2.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.0/auto_test_common.egg-info/PKG-INFO` & `auto-test-common-2.0.1/auto_test_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-test-common
-Version: 2.0.0
+Version: 2.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `auto-test-common-2.0.0/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-2.0.1/auto_test_common.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 auto_test_common.egg-info/SOURCES.txt
 auto_test_common.egg-info/dependency_links.txt
 auto_test_common.egg-info/entry_points.txt
 auto_test_common.egg-info/requires.txt
 auto_test_common.egg-info/top_level.txt
 common/__init__.py
 common/autotest/__init__.py
+common/autotest/assert_function.py
 common/autotest/base_requests.py
 common/autotest/handle_allure.py
 common/autotest/handle_assert.py
 common/common/__init__.py
 common/common/api_driver.py
 common/common/constant.py
 common/common/test.py
 common/config/__init__.py
 common/config/config.py
 common/data/__init__.py
 common/data/data_process.py
+common/data/eval_data_handle.py
+common/data/faker_handle.py
 common/data/handle_common.py
 common/data/template_data.py
 common/db/__init__.py
 common/db/handle_db.py
 common/db/handle_db_batch.py
 common/db/handle_mongo.py
 common/db/handle_mysqldb.py
```

### Comparing `auto-test-common-2.0.0/auto_test_common.egg-info/requires.txt` & `auto-test-common-2.0.1/auto_test_common.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 loguru==0.5.1
 PyYAML==5.3.1
 playwright==1.27.1
 requests==2.24.0
 requests-toolbelt==1.0.0
 xlrd==2.0.1
 PyMySQL==0.10.1
+ruamel.yaml==0.18.5
 pytest-rerunfailures==9.1.1
 allure-pytest==2.9.45
-pytest-xdist==2.5.0
+pytest-asyncio==0.23.6
+pytest-mimesis==1.1.0
+pytest-bdd==7.1.2
+faker==21.0.0pytest-xdist==2.5.0
 allure-python-commons==2.9.45
 xlrd==2.0.1
 xlutils==2.0.0
 xlwt==1.3.0
 zipp==3.7.0
 xmltodict==0.13.0
 python-dateutil==2.8.2
```

### Comparing `auto-test-common-2.0.0/common/autotest/base_requests.py` & `auto-test-common-2.0.1/common/autotest/base_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         DataBus.save_init_data()
         case_number = DataProcess.get_key_dic(case, Constant.CASE_NO)
         path = DataProcess.get_key_dic(case, "接口地址")
         if DataProcess.get_key_dic(case, Constant.CASE_DATA_PARAM) != None:
             parametric_key = DataProcess.get_key_dic(case, Constant.CASE_DATA_PARAM)
         else:
             parametric_key = DataProcess.get_key_dic(case, "入参关键字")
-
         if DataProcess.get_key_dic(case, Constant.CASE_DATA_HEADER) != None:
             token = DataProcess.get_key_dic(case, Constant.CASE_DATA_HEADER)
         else:
             token = DataProcess.get_key_dic(case, "token操作")
         if DataProcess.get_key_dic(case, Constant.CASE_DATA_TYPE) != None:
             datatype = DataProcess.get_key_dic(case, Constant.CASE_DATA_TYPE)
         method = DataProcess.get_key_dic(case, Constant.CASE_DATA_METHOD)
@@ -52,15 +51,15 @@
                 data = DataProcess.handle_data(data, False)
         except Exception as e:
             logger.info(f'测试数据：{data} 转换异常:' + repr(e))
         file = DataProcess.handler_files(file_obj)
         desc = f'测试接口详情:{url}'
         # 发送请求
         res = cls.http_request(url=url, method=method, parametric_key=parametric_key,
-                               header=DataProcess.setDictEncode(header), data=data, file=file, desc=desc)
+                               header=header, data=data, file=file, desc=desc)
         try:
             if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
                 MysqlPlatForm.insert_api_data(url, method, header, data, res.elapsed.total_seconds(), res.status_code)
         except:
             logger.warning("保存请求数据异常")
         # 响应后操作
         if token == '写':
@@ -71,15 +70,15 @@
             DataProcess.save_response(case_number, res.json())
         try:
             return res.json(), expect, res
         except:
             return res.text, expect, res
 
     @classmethod
-    def api_exec(self, schemal_key, data=None, header=None, file=None, cookie=None, host: str = 'host', datatype: str='json', step:str='测试接口详情', _replace:int=0) -> object:
+    def api_exec(self, schemal_key, data=None, header=None, file=None, cookie=None, host: str = 'host', datatype: str='json', step:str='测试接口详情', _replace:int=0, assert_data=None) -> object:
         """处理case数据，转换成可用数据发送请求
         :param case: 读取出来的每一行用例内容，可进行解包
         :param env: 环境名称 默认使用config.yaml server下的 dev 后面的基准地址
         return: 响应结果， 预期结果
         """
         DataBus.save_init_data()
         temp = data
@@ -138,28 +137,35 @@
             data = DataProcess.handle_data(variable=data, jsonformat=False, _replace=_replace)
         if 'file' in schemal_data and file is None:
             file = schemal_body['file']
         file_obj = DataProcess.handler_files(file)
         if step == '测试接口详情' and DataProcess.isNotNull(schemal_data['desc']):
             step = '测试接口详情:'+schemal_data['desc']
         res = self.http_request(url=url, method=schemal_data['method'], parametric_key=schemal_data['datatype'],
-                               header=DataProcess.setDictEncode(header), data=data, file=file_obj, cookie=cookie, desc=step)
+                               header=header, data=data, file=file_obj, cookie=cookie, desc=step)
         if 'assert' in schemal_data:
-            if isinstance(temp,dict):
+            if isinstance(temp,dict) and temp is not None:
                 schemal_body = ReadFile.get_yaml_ApiSchemal(schemal_key)
                 assertData = schemal_body['assert']
                 _assert = convert_json_bank(assertData, temp)
+            elif isinstance(assert_data,dict) and assert_data is not  None:
+                schemal_body = ReadFile.get_yaml_ApiSchemal(schemal_key)
+                assertData = schemal_body['assert']
+                _assert = convert_json_bank(assertData, assert_data)
+            elif isinstance(assert_data,str) and DataProcess.isNotNull(assert_data):
+                _assert = assert_data
             else:
                 _assert = schemal_data['assert']
+
             if str(_assert).find('*ResCode') >= 0:
                 assert_response(res, _assert)
             else:
                 if DataProcess.isNotNull(get_system_key(Constant.RESPONSE_CODE)):
                     ex_status_code = get_system_key(Constant.RESPONSE_CODE)
-                    allure_step(f'状态码检查', f'实际状态码: {res.status_code}小于{ex_status_code}')
+                    allure_step(f'返回结果检查【状态码】', f'实际状态码: {res.status_code}小于 预期状态码:{ex_status_code}')
                     assert res.status_code <= int(ex_status_code)
                 assert_response(res, _assert)
         else:
             if DataProcess.isNotNull(get_system_key(Constant.RESPONSE_CODE)):
                 ex_status_code = get_system_key(Constant.RESPONSE_CODE)
                 allure_step(f'状态码检查', f'实际状态码: {res.status_code}小于{ex_status_code}')
                 assert res.status_code <= int(ex_status_code)
```

### Comparing `auto-test-common-2.0.0/common/autotest/handle_allure.py` & `auto-test-common-2.0.1/common/autotest/handle_allure.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,16 @@
     :param content: 附件内容
     """
     logger.info(f'{step}:{content}')
     try:
         with allure.step(step):
             allure.attach(json.dumps(content, ensure_ascii=False, indent=4), step, allure.attachment_type.TEXT)
     except Exception as e:
-        logger.warning(f'{step}：{content} 异常信息'+repr(e))
+        with allure.step(step):
+            allure.attach(content, step, allure.attachment_type.TEXT)
 
 def screenshot(page:Page, desc:str)->None:
     """
     截图
     """
     page.screenshot(timeout=5000, path=TEST_TARGET_RESULTS_PATH)
     #把截图放入到allure
@@ -152,26 +153,39 @@
                 assert_equal(actual, expect)
     except AssertionError:
         raise AssertionError(f'{desc} |- 实际结果: {actual}  预期结果: {expect}')
 
 
 def isNotNull(data):
     try:
-        if isinstance(data, bool):
-            return data
         if data is None:
             return False
-        if isinstance(data, str):
+        elif isinstance(data, bool):
+            return data
+        elif isinstance(data, str):
             _data = data
+        elif isinstance(data, dict):
+            if data.__len__() < 1:
+                return False
+            else:
+                return True
+        elif isinstance(data, list):
+            if data.__len__() < 1:
+                return False
+            else:
+                return True
         else:
             _data = str(data)
         if _data.strip() == '':
             return False
         else:
             return True
     except Exception as e:
-        logger.info('判断数据是否为空异常,数据：'+data)
+        logger.warning('判断数据是否为空异常,数据：'+data)
         return True
 
 
+if __name__ == '__main__':
+    print(isNotNull(None))
+
```

### Comparing `auto-test-common-2.0.0/common/autotest/handle_assert.py` & `auto-test-common-2.0.1/common/autotest/handle_assert.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,24 @@
     except Exception:
         expect_dict = expect_str
     if isinstance(expect_dict,dict):
         index = 0
         for k, v in expect_dict.items():
             # 获取需要断言的实际结果部分
             if str(k).find('*ResCode') != -1:
-                assert_equals(response.status_code, v, f'返回结果【状态码】检查')
+                assert_equals(response.status_code, v, f'返回结果检查【状态码】')
             elif str(k).find('*ResBody') != -1:
-                assert_equals(response.text, v, f'返回结果【返回内容】检查')
+                assert_equals(response.text, v, f'返回结果检查【返回内容】')
             else:
                 try:
                     actual = get_jpath(response.json(), k)
                 except:
                     actual = get_jpath(response.text, k)
                 index += 1
-                assert_equals(actual, v, f'返回结果【{k}】检查')
+                assert_equals(actual, v, f'返回结果检查【{k}】')
 
 def assert_contain_response(response, expect_str: str):
     """ 预期结果实际结果断言方法
     :param res: 实际响应结果
     :param expect_str: 预期响应内容，从excel中读取
     return None
     """
```

### Comparing `auto-test-common-2.0.0/common/common/api_driver.py` & `auto-test-common-2.0.1/common/common/api_driver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import loguru
 import requests
 from common.autotest.handle_allure import allure_api_step, allure_step
 from requests_toolbelt import MultipartEncoder
 from os import path
 import os
 from common.config.config import TEST_FILE_PATH
+import copy
 
 
 class APIDriver(object):
 
     session = None
 
     @classmethod
@@ -29,74 +30,74 @@
         :param file: 文件对象
         :param desc: 自动化测试过程请求描述：打印到Report中
         :param header: 请求头
         :return: 返回res对象
         """
         session = cls.get_session()
         if parametric_key is None:
-            header = cls.getCommontHeader(header)
+            header,header_desc = cls.getCommontHeader(header)
             res = session.request(method=method, url=url, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
-            allure_api_step(desc, url, method, header, '', '', res)
+            allure_api_step(desc, url, method, header_desc, '', '', res)
 
         elif parametric_key == 'params':
-            header = cls.getCommontHeader(header)
+            header,header_desc = cls.getCommontHeader(header)
             res = session.request(method=method, url=url, params=data, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
-            allure_api_step(desc, url, method, header, data, '', res)
+            allure_api_step(desc, url, method, header_desc, data, '', res)
 
         elif parametric_key == 'data':
-            header = cls.getCommontHeader(header)
+            header,header_desc = cls.getCommontHeader(header)
             res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
-            allure_api_step(desc, url, method, header, data, file, res)
+            allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'text':
-            header = cls.getCommontHeader(header)
+            header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'text/plain'
             res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
-            allure_api_step(desc, url, method, header, data, file, res)
+            allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'json':
-            header = cls.getCommontHeader(header)
+            header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/json'
             res = session.request(method=method, url=url, json=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth,verify=False)
-            allure_api_step(desc, url, method, header, data, file, res)
+            allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'xml':
-            header = cls.getCommontHeader(header)
+            header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/xml'
             res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
-            allure_api_step(desc, url, method, header, data, file, res)
+            allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'form':
-            header = cls.getCommontHeader(header)
+            header,header_desc = cls.getCommontHeader(header)
             header['Content-Type'] = 'application/x-www-form-urlencoded'
             try:
                 if isinstance(data, str):
                     from common.data.data_process import DataProcess
                     data = DataProcess.handle_data(data)
             except Exception as e:
                 logger.info(f'测试数据：{data} 转换异常:' + repr(e))
             res = session.request(method=method, url=url, data=data, files=file, headers=header, cookies=cookie,
                                   auth=_auth, verify=False)
-            allure_api_step(desc, url, method, header, data, file, res)
+            allure_api_step(desc, url, method, header_desc, data, file, res)
 
         elif parametric_key == 'form-data':
             if data is not None:
                 data = cls.handleFile(data)
                 m = MultipartEncoder(data)
-                header = cls.getCommontHeader(header)
+                header,header_desc = cls.getCommontHeader(header)
                 header['Content-Type'] = m.content_type
                 res = session.request(method=method, url=url, data=m, headers=header, cookies=cookie,
                                       auth=_auth, verify=False)
-                allure_api_step(desc, url, method, header, data, file, res)
+                allure_api_step(desc, url, method, header_desc, data, file, res)
         else:
             raise ValueError('可选关键字为params, data, xml, json, text, form,form-urlencoded')
         session.close()
         return res
 
     @classmethod
     def getCommontHeader(self, header):
@@ -113,15 +114,18 @@
                 header['Connection'] = 'keep-alive'
             if 'Accept-Encoding' not in header:
                 header['Accept-Encoding'] = 'gzip, deflate, br'
             if 'Accept-Language' not in header:
                 header['Accept-Language'] = 'zh-CN,zh;q=0.9'
             if 'Accept' not in header:
                 header['Accept'] = '*/*'
-        return header
+        header_desc = copy.copy(header)
+        from common.data.data_process import DataProcess
+        header = DataProcess.setDictEncode(header)
+        return header, header_desc
 
     @classmethod
     def handleFile(self,data):
         if isinstance(data,dict):
             for key in data:
                 if isinstance(data[key], str):
                     from common.file.handle_system import adjust_path
```

### Comparing `auto-test-common-2.0.0/common/common/constant.py` & `auto-test-common-2.0.1/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/common/test.py` & `auto-test-common-2.0.1/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/config/config.py` & `auto-test-common-2.0.1/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/data/data_process.py` & `auto-test-common-2.0.1/common/data/data_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,14 @@
         _date = str(_date).strip()
         if len(_date) > 10:
             ts = int(time.mktime(time.strptime(_date, "%Y-%m-%d %H:%M:%S")))
         else:
             ts = int(time.mktime(time.strptime(_date, "%Y-%m-%d")))
         return ts
 
-
     @classmethod
     def check_test_data(self, testdatas:list):
         _testDatas = []
         casename = "00000"
         caseno = "00000"
         try:
             for testdata in testdatas:
@@ -582,15 +581,15 @@
                 allure_step(f'接口返回【{v}】回填【{_key}】', f'回填数据:{_value}')
 
 if __name__ == '__main__':
     # _list=[{'script':'1111[2334]'},{'script':'1122//[2334]'},{'script':'1111[233334]'},{'script':'111/1111'},{'script':'1111'},{'script':'1111'}]
     # list = DataProcess.list_script_removal_byKey(_list,'script')
     from common.plugin.data_bus import DataBus
     DataBus.set_key('3333','')
-    print(DataBus.get_key('3333'))
+    print(DataProcess.objecttodict(DataBus))
```

### Comparing `auto-test-common-2.0.0/common/data/handle_common.py` & `auto-test-common-2.0.1/common/data/handle_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -299,20 +299,43 @@
     from common.data.data_process import DataProcess
     _json = DataProcess.handle_data(_str)
     if _json is None:
         return None
     else:
         return json.dumps(convert_json_dict(_json), ensure_ascii=False)
 
+def objecttodict(obj):
+    """
+     复杂对象转成dict的方法
+    """
+    dict_o = obj.__dict__
+    for key, value in dict_o.items():
+        print(key, type(value))
+        if isinstance(value, (str, int)):  # 不处理str,int的情况
+            pass
+        elif value is None:
+            pass
+        elif isinstance(value, list):  # 处理list的情况
+            valuelist = []
+            for l in value:
+                if isinstance(l, (str, int)):
+                    valuelist.append(l)
+                else:
+                    valuelist.append(objecttodict(l))
+            dict_o[key] = valuelist
+        elif isinstance(value, dict):
+            pass  # 不处理dict的情况
+        else:  # 处理普通对象
+            dict_o[key] = objecttodict(value)
+    return dict_o
+
+
 
 if __name__ == '__main__':
-    content="{'Service': {'Header': {'UsernameToken': {'Username': 'CA129', 'Password': '${Password}'}}, 'Body': {'systemcode': 'CA129', 'filtercondition': '', 'SOAHttpOption': 'GET', 'EsbJsonBody': {}}}}"
-    data= {'Password':'f1021c74-88f6-4b29-811d-ac873bc55115'}
     from common.data.data_process import DataProcess
-    data =convert_json_bank(content, data)
-    print(DataProcess.handle_data(data))
+    print(objecttodict(DataProcess))
```

### Comparing `auto-test-common-2.0.0/common/data/template_data.py` & `auto-test-common-2.0.1/common/data/template_data.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/db/handle_db.py` & `auto-test-common-2.0.1/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/db/handle_db_batch.py` & `auto-test-common-2.0.1/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/db/handle_mongo.py` & `auto-test-common-2.0.1/common/db/handle_mongo.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/db/handle_mysqldb.py` & `auto-test-common-2.0.1/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/db/handle_oracle.py` & `auto-test-common-2.0.1/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/db/handle_sqlserver.py` & `auto-test-common-2.0.1/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/driver/ui_page.py` & `auto-test-common-2.0.1/common/driver/ui_page.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/file/ReadFile.py` & `auto-test-common-2.0.1/common/file/ReadFile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
+
+import loguru
 import yaml
 import xlrd
 from common.config.config import CONFIG_PATH, API_YAML_PATH, CONFIG_YAML_PATH
 from common.data.handle_common import extractor, req_expr
 from common.file.handle_system import adjust_path_data
+from loguru import logger
 
 
 class ReadFile:
 
     @classmethod
     def read_config(cls, file_name, config_path: str = CONFIG_PATH) -> dict:
         """读取配置文件，并且转换成字典
@@ -93,25 +96,36 @@
             value = table.row_values(row)
             value.pop(5)
             data_list.append(list(value))
         return data_list
 
 
 def get_yaml_config(content, is_dict: bool = True, data: dict = None):
-    if is_dict:
-        return eval(req_expr(str(ReadFile.get_yaml_config(content)), data))
-    else:
+    try:
+        if is_dict:
+            return eval(req_expr(str(ReadFile.get_yaml_config(content)), data))
+        else:
+            return req_expr(str(ReadFile.get_yaml_config(content, False)), data)
+    except Exception as e:
         return req_expr(str(ReadFile.get_yaml_config(content, False)), data)
+        logger.warning(f"获取yaml文件参数：{content} 异常信息:{e}")
+
 
 
 def get_yaml_ApiSchemal(content, is_dict: bool = True, data: dict = None):
-    if is_dict:
-        return eval(req_expr(str(ReadFile.get_yaml_ApiSchemal(content)), data))
-    else:
+    try:
+        if is_dict:
+            return eval(req_expr(str(ReadFile.get_yaml_ApiSchemal(content)), data))
+        else:
+            return req_expr(str(ReadFile.get_yaml_config(content, False)), data)
+    except Exception as e:
         return req_expr(str(ReadFile.get_yaml_config(content, False)), data)
+        logger.warning(f"获取yaml文件参数：{content} 异常信息:{e}")
+
+
```

### Comparing `auto-test-common-2.0.0/common/file/handle_excel.py` & `auto-test-common-2.0.1/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/file/handle_file.py` & `auto-test-common-2.0.1/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/file/handle_reques.py` & `auto-test-common-2.0.1/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/file/handle_system.py` & `auto-test-common-2.0.1/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/file/handle_yaml.py` & `auto-test-common-2.0.1/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/mq/handle_rabbit.py` & `auto-test-common-2.0.1/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plat/ATF_platform.py` & `auto-test-common-2.0.1/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plat/jenkin_platform.py` & `auto-test-common-2.0.1/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plat/jira_platform.py` & `auto-test-common-2.0.1/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plat/mysql_platform.py` & `auto-test-common-2.0.1/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plat/service_platform.py` & `auto-test-common-2.0.1/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/allure_plugin.py` & `auto-test-common-2.0.1/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/assert_plugin.py` & `auto-test-common-2.0.1/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/atf_plugin.py` & `auto-test-common-2.0.1/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/data_bus.py` & `auto-test-common-2.0.1/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/data_plugin.py` & `auto-test-common-2.0.1/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/file_plugin.py` & `auto-test-common-2.0.1/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/hooks_plugin.py` & `auto-test-common-2.0.1/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/pytest_playwright.py` & `auto-test-common-2.0.1/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/pytest_plugin.py` & `auto-test-common-2.0.1/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/template_plugin.py` & `auto-test-common-2.0.1/common/plugin/template_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/common/plugin/yaml_plugin.py` & `auto-test-common-2.0.1/common/plugin/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-2.0.0/setup.py` & `auto-test-common-2.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,21 @@
         "loguru==0.5.1",
         "PyYAML==5.3.1",
         "playwright==1.27.1",
         "requests==2.24.0",
         "requests-toolbelt==1.0.0",
         "xlrd==2.0.1",
         "PyMySQL==0.10.1",
+        "ruamel.yaml==0.18.5",
         "pytest-rerunfailures==9.1.1",
         "allure-pytest==2.9.45",
+        "pytest-asyncio==0.23.6",
+        "pytest-mimesis==1.1.0",
+        "pytest-bdd==7.1.2",
+        "faker==21.0.0"
         "pytest-xdist==2.5.0",
         "allure-python-commons==2.9.45",
         "xlrd==2.0.1",
         "xlutils==2.0.0",
         "xlwt==1.3.0",
         "zipp==3.7.0",
         "xmltodict==0.13.0",
```

