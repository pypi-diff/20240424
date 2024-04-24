# Comparing `tmp/hebill-1.2.3.tar.gz` & `tmp/hebill-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hebill-1.2.3.tar", last modified: Wed Apr 24 03:23:46 2024, max compression
+gzip compressed data, was "hebill-1.2.4.tar", last modified: Wed Apr 24 03:55:27 2024, max compression
```

## Comparing `hebill-1.2.3.tar` & `hebill-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,296 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 03:23:46.547122 hebill-1.2.3/
--rw-rw-rw-   0        0        0      924 2024-04-24 03:23:46.547122 hebill-1.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 03:23:46.540605 hebill-1.2.3/hebill/
--rw-rw-rw-   0        0        0      341 2024-04-24 03:12:13.000000 hebill-1.2.3/hebill/__init__.py
--rw-rw-rw-   0        0        0      267 2024-04-24 03:23:45.000000 hebill-1.2.3/hebill/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:23:46.544605 hebill-1.2.3/hebill.egg-info/
--rw-rw-rw-   0        0        0      924 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-24 03:23:46.000000 hebill-1.2.3/hebill.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      592 2024-04-24 03:23:45.000000 hebill-1.2.3/pack_upload_setup.py
--rw-rw-rw-   0        0        0       42 2024-04-24 03:23:46.547122 hebill-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.352720 hebill-1.2.4/
+-rw-rw-rw-   0        0        0      924 2024-04-24 03:55:27.351720 hebill-1.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.181171 hebill-1.2.4/hebill/
+-rw-rw-rw-   0        0        0      341 2024-04-24 03:12:13.000000 hebill-1.2.4/hebill/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-04-24 03:46:52.000000 hebill-1.2.4/hebill/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.188692 hebill-1.2.4/hebill/dimensions/
+-rw-rw-rw-   0        0        0       30 2024-04-12 00:54:52.000000 hebill-1.2.4/hebill/dimensions/__init__.py
+-rw-rw-rw-   0        0        0     1707 2024-04-12 04:30:14.000000 hebill-1.2.4/hebill/dimensions/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.193026 hebill-1.2.4/hebill/dir/
+-rw-rw-rw-   0        0        0       23 2024-04-08 01:00:04.000000 hebill-1.2.4/hebill/dir/__init__.py
+-rw-rw-rw-   0        0        0     2224 2024-04-09 00:29:06.000000 hebill-1.2.4/hebill/dir/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.199528 hebill-1.2.4/hebill/excel/
+-rw-rw-rw-   0        0        0       25 2024-04-12 01:05:37.000000 hebill-1.2.4/hebill/excel/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-12 00:54:52.000000 hebill-1.2.4/hebill/excel/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.200539 hebill-1.2.4/hebill/file/
+-rw-rw-rw-   0        0        0       24 2024-04-05 01:59:44.000000 hebill-1.2.4/hebill/file/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-04-08 01:57:47.000000 hebill-1.2.4/hebill/file/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.202052 hebill-1.2.4/hebill/html/
+-rw-rw-rw-   0        0        0       95 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.203063 hebill-1.2.4/hebill/html/components/
+-rw-rw-rw-   0        0        0       60 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/components/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.204063 hebill-1.2.4/hebill/html/components/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:20.000000 hebill-1.2.4/hebill/html/components/html/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.205062 hebill-1.2.4/hebill/html/components/html/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:07.000000 hebill-1.2.4/hebill/html/components/html/body/__init__.py
+-rw-rw-rw-   0        0        0      100 2024-04-05 08:05:17.000000 hebill-1.2.4/hebill/html/components/html/body/core.py
+-rw-rw-rw-   0        0        0      424 2024-04-05 08:03:11.000000 hebill-1.2.4/hebill/html/components/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.207590 hebill-1.2.4/hebill/html/components/html/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:02.000000 hebill-1.2.4/hebill/html/components/html/head/__init__.py
+-rw-rw-rw-   0        0        0      551 2024-04-05 08:05:17.000000 hebill-1.2.4/hebill/html/components/html/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.208598 hebill-1.2.4/hebill/html/components/html/head/title/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.4/hebill/html/components/html/head/title/__init__.py
+-rw-rw-rw-   0        0        0      106 2024-04-05 08:05:17.000000 hebill-1.2.4/hebill/html/components/html/head/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.210597 hebill-1.2.4/hebill/html/components/html/libraries/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:36.000000 hebill-1.2.4/hebill/html/components/html/libraries/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-04-05 08:05:17.000000 hebill-1.2.4/hebill/html/components/html/libraries/libraries.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.211597 hebill-1.2.4/hebill/html/components/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:11:14.000000 hebill-1.2.4/hebill/html/components/table/__init__.py
+-rw-rw-rw-   0        0        0      673 2024-04-05 08:08:29.000000 hebill-1.2.4/hebill/html/components/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.213208 hebill-1.2.4/hebill/html/components/table/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:13:04.000000 hebill-1.2.4/hebill/html/components/table/tbody/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:15:50.000000 hebill-1.2.4/hebill/html/components/table/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.214216 hebill-1.2.4/hebill/html/components/table/tbody/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.4/hebill/html/components/table/tbody/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.4/hebill/html/components/table/tbody/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.215217 hebill-1.2.4/hebill/html/components/table/tbody/tr/td/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.4/hebill/html/components/table/tbody/tr/td/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.4/hebill/html/components/table/tbody/tr/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.216217 hebill-1.2.4/hebill/html/components/table/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:12:57.000000 hebill-1.2.4/hebill/html/components/table/thead/__init__.py
+-rw-rw-rw-   0        0        0      565 2024-04-05 08:11:22.000000 hebill-1.2.4/hebill/html/components/table/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.217217 hebill-1.2.4/hebill/html/components/table/thead/tr/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.4/hebill/html/components/table/thead/tr/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-05 08:15:50.000000 hebill-1.2.4/hebill/html/components/table/thead/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.218217 hebill-1.2.4/hebill/html/components/table/thead/tr/th/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.4/hebill/html/components/table/thead/tr/th/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-04-05 08:15:50.000000 hebill-1.2.4/hebill/html/components/table/thead/tr/th/core.py
+-rw-rw-rw-   0        0        0      966 2024-04-05 07:58:22.000000 hebill-1.2.4/hebill/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.219219 hebill-1.2.4/hebill/html/nodes/
+-rw-rw-rw-   0        0        0      186 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.220219 hebill-1.2.4/hebill/html/nodes/code/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:22.000000 hebill-1.2.4/hebill/html/nodes/code/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-05 08:03:49.000000 hebill-1.2.4/hebill/html/nodes/code/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.222218 hebill-1.2.4/hebill/html/nodes/comment/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:28.000000 hebill-1.2.4/hebill/html/nodes/comment/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-04-05 08:05:37.000000 hebill-1.2.4/hebill/html/nodes/comment/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.223218 hebill-1.2.4/hebill/html/nodes/content/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:33.000000 hebill-1.2.4/hebill/html/nodes/content/__init__.py
+-rw-rw-rw-   0        0        0      357 2024-04-05 08:07:50.000000 hebill-1.2.4/hebill/html/nodes/content/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.224344 hebill-1.2.4/hebill/html/nodes/group/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:49.000000 hebill-1.2.4/hebill/html/nodes/group/__init__.py
+-rw-rw-rw-   0        0        0      738 2024-04-05 08:07:50.000000 hebill-1.2.4/hebill/html/nodes/group/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.225855 hebill-1.2.4/hebill/html/nodes/group/create/
+-rw-rw-rw-   0        0        0        0 2024-03-09 00:40:03.000000 hebill-1.2.4/hebill/html/nodes/group/create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.227868 hebill-1.2.4/hebill/html/nodes/group/create/components/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:31.000000 hebill-1.2.4/hebill/html/nodes/group/create/components/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-04-05 07:56:53.000000 hebill-1.2.4/hebill/html/nodes/group/create/components/core.py
+-rw-rw-rw-   0        0        0      752 2024-04-05 07:56:53.000000 hebill-1.2.4/hebill/html/nodes/group/create/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.228869 hebill-1.2.4/hebill/html/nodes/group/create/nodes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:50:37.000000 hebill-1.2.4/hebill/html/nodes/group/create/nodes/__init__.py
+-rw-rw-rw-   0        0        0      648 2024-04-05 07:56:53.000000 hebill-1.2.4/hebill/html/nodes/group/create/nodes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.231869 hebill-1.2.4/hebill/html/nodes/group/create/tags/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:51:13.000000 hebill-1.2.4/hebill/html/nodes/group/create/tags/__init__.py
+-rw-rw-rw-   0        0        0     2518 2024-04-05 07:56:53.000000 hebill-1.2.4/hebill/html/nodes/group/create/tags/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.233055 hebill-1.2.4/hebill/html/nodes/node/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:54.000000 hebill-1.2.4/hebill/html/nodes/node/__init__.py
+-rw-rw-rw-   0        0        0     1104 2024-04-05 08:07:50.000000 hebill-1.2.4/hebill/html/nodes/node/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.235056 hebill-1.2.4/hebill/html/nodes/tag/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:07:58.000000 hebill-1.2.4/hebill/html/nodes/tag/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.237052 hebill-1.2.4/hebill/html/nodes/tag/attributes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:38.000000 hebill-1.2.4/hebill/html/nodes/tag/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.239054 hebill-1.2.4/hebill/html/nodes/tag/attributes/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:09:52.000000 hebill-1.2.4/hebill/html/nodes/tag/attributes/classes/__init__.py
+-rw-rw-rw-   0        0        0      707 2024-03-09 00:40:03.000000 hebill-1.2.4/hebill/html/nodes/tag/attributes/classes/core.py
+-rw-rw-rw-   0        0        0     1524 2024-04-05 08:11:22.000000 hebill-1.2.4/hebill/html/nodes/tag/attributes/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.242108 hebill-1.2.4/hebill/html/nodes/tag/attributes/styles/
+-rw-rw-rw-   0        0        0        0 2024-04-05 08:10:01.000000 hebill-1.2.4/hebill/html/nodes/tag/attributes/styles/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-03-09 00:40:03.000000 hebill-1.2.4/hebill/html/nodes/tag/attributes/styles/core.py
+-rw-rw-rw-   0        0        0     1130 2024-04-05 08:11:22.000000 hebill-1.2.4/hebill/html/nodes/tag/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.242108 hebill-1.2.4/hebill/html/tags/
+-rw-rw-rw-   0        0        0      617 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.244118 hebill-1.2.4/hebill/html/tags/a/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:21.000000 hebill-1.2.4/hebill/html/tags/a/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/a/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.245118 hebill-1.2.4/hebill/html/tags/body/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:29.000000 hebill-1.2.4/hebill/html/tags/body/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/body/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.246117 hebill-1.2.4/hebill/html/tags/div/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:35.000000 hebill-1.2.4/hebill/html/tags/div/__init__.py
+-rw-rw-rw-   0        0        0      213 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/div/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.247231 hebill-1.2.4/hebill/html/tags/h1/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.4/hebill/html/tags/h1/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/h1/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.248242 hebill-1.2.4/hebill/html/tags/h2/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.4/hebill/html/tags/h2/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/h2/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.249241 hebill-1.2.4/hebill/html/tags/h3/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.4/hebill/html/tags/h3/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/h3/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.250239 hebill-1.2.4/hebill/html/tags/h4/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.4/hebill/html/tags/h4/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/h4/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.252240 hebill-1.2.4/hebill/html/tags/h5/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.4/hebill/html/tags/h5/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/h5/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.253241 hebill-1.2.4/hebill/html/tags/h6/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:02:49.000000 hebill-1.2.4/hebill/html/tags/h6/__init__.py
+-rw-rw-rw-   0        0        0      211 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/h6/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.254529 hebill-1.2.4/hebill/html/tags/head/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:23.000000 hebill-1.2.4/hebill/html/tags/head/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/head/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.255722 hebill-1.2.4/hebill/html/tags/html/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:34.000000 hebill-1.2.4/hebill/html/tags/html/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/html/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.257232 hebill-1.2.4/hebill/html/tags/input_text/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:04:58.000000 hebill-1.2.4/hebill/html/tags/input_text/__init__.py
+-rw-rw-rw-   0        0        0      487 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/input_text/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.259779 hebill-1.2.4/hebill/html/tags/link/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:05.000000 hebill-1.2.4/hebill/html/tags/link/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/link/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.260789 hebill-1.2.4/hebill/html/tags/script/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:27.000000 hebill-1.2.4/hebill/html/tags/script/__init__.py
+-rw-rw-rw-   0        0        0      215 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/script/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.261787 hebill-1.2.4/hebill/html/tags/span/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:32.000000 hebill-1.2.4/hebill/html/tags/span/__init__.py
+-rw-rw-rw-   0        0        0      256 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/span/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.263253 hebill-1.2.4/hebill/html/tags/table/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:37.000000 hebill-1.2.4/hebill/html/tags/table/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.264375 hebill-1.2.4/hebill/html/tags/tbody/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:49.000000 hebill-1.2.4/hebill/html/tags/tbody/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/tbody/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.265385 hebill-1.2.4/hebill/html/tags/td/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:05:59.000000 hebill-1.2.4/hebill/html/tags/td/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/td/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.266385 hebill-1.2.4/hebill/html/tags/th/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:04.000000 hebill-1.2.4/hebill/html/tags/th/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/th/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.267796 hebill-1.2.4/hebill/html/tags/thead/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:10.000000 hebill-1.2.4/hebill/html/tags/thead/__init__.py
+-rw-rw-rw-   0        0        0      125 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/thead/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.269133 hebill-1.2.4/hebill/html/tags/title/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:16.000000 hebill-1.2.4/hebill/html/tags/title/__init__.py
+-rw-rw-rw-   0        0        0      376 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/title/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.271145 hebill-1.2.4/hebill/html/tags/tr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 03:06:21.000000 hebill-1.2.4/hebill/html/tags/tr/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-04-05 03:31:08.000000 hebill-1.2.4/hebill/html/tags/tr/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.274149 hebill-1.2.4/hebill/image/
+-rw-rw-rw-   0        0        0      653 2024-04-09 01:17:04.000000 hebill-1.2.4/hebill/image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.278730 hebill-1.2.4/hebill/image/png/
+-rw-rw-rw-   0        0        0        0 2024-04-05 04:11:13.000000 hebill-1.2.4/hebill/image/png/__init__.py
+-rw-rw-rw-   0        0        0    60832 2024-04-12 00:49:55.000000 hebill-1.2.4/hebill/image/png/constants.py
+-rw-rw-rw-   0        0        0     5804 2024-04-06 01:07:24.000000 hebill-1.2.4/hebill/image/png/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.280743 hebill-1.2.4/hebill/math/
+-rw-rw-rw-   0        0        0       52 2024-04-16 07:28:38.000000 hebill-1.2.4/hebill/math/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-04-18 07:17:06.000000 hebill-1.2.4/hebill/math/ring_volume_weight.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.285195 hebill-1.2.4/hebill/mysql/
+-rw-rw-rw-   0        0        0       76 2024-04-19 11:39:48.000000 hebill-1.2.4/hebill/mysql/__init__.py
+-rw-rw-rw-   0        0        0       79 2024-03-22 03:00:14.000000 hebill-1.2.4/hebill/mysql/constants.py
+-rw-rw-rw-   0        0        0     3772 2024-04-05 02:36:51.000000 hebill-1.2.4/hebill/mysql/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.290719 hebill-1.2.4/hebill/mysql/features/
+-rw-rw-rw-   0        0        0      146 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/features/__init__.py
+-rw-rw-rw-   0        0        0      847 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/features/table_describe_data.py
+-rw-rw-rw-   0        0        0     1028 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/features/table_index_data.py
+-rw-rw-rw-   0        0        0     1423 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/features/table_status_data.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.290719 hebill-1.2.4/hebill/mysql/plugins/
+-rw-rw-rw-   0        0        0      134 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.292168 hebill-1.2.4/hebill/mysql/plugins/columns/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:25.000000 hebill-1.2.4/hebill/mysql/plugins/columns/__init__.py
+-rw-rw-rw-   0        0        0      583 2024-03-22 12:26:14.000000 hebill-1.2.4/hebill/mysql/plugins/columns/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.293473 hebill-1.2.4/hebill/mysql/plugins/limits/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:33.000000 hebill-1.2.4/hebill/mysql/plugins/limits/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-03-22 12:26:14.000000 hebill-1.2.4/hebill/mysql/plugins/limits/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.294677 hebill-1.2.4/hebill/mysql/plugins/orders/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:49:41.000000 hebill-1.2.4/hebill/mysql/plugins/orders/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-22 12:26:14.000000 hebill-1.2.4/hebill/mysql/plugins/orders/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.298069 hebill-1.2.4/hebill/mysql/plugins/wheres/
+-rw-rw-rw-   0        0        0        0 2024-04-05 02:35:12.000000 hebill-1.2.4/hebill/mysql/plugins/wheres/__init__.py
+-rw-rw-rw-   0        0        0     3174 2024-04-05 02:36:51.000000 hebill-1.2.4/hebill/mysql/plugins/wheres/condition.py
+-rw-rw-rw-   0        0        0     2635 2024-03-22 15:25:59.000000 hebill-1.2.4/hebill/mysql/plugins/wheres/conditions.py
+-rw-rw-rw-   0        0        0      206 2024-04-05 02:36:51.000000 hebill-1.2.4/hebill/mysql/plugins/wheres/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.299581 hebill-1.2.4/hebill/mysql/table/
+-rw-rw-rw-   0        0        0       25 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/table/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.301965 hebill-1.2.4/hebill/mysql/table/column/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:18:02.000000 hebill-1.2.4/hebill/mysql/table/column/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/table/column/core.py
+-rw-rw-rw-   0        0        0     7332 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/table/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.305363 hebill-1.2.4/hebill/mysql/table/data/
+-rw-rw-rw-   0        0        0        0 2024-03-22 00:21:17.000000 hebill-1.2.4/hebill/mysql/table/data/__init__.py
+-rw-rw-rw-   0        0        0      568 2024-03-22 03:43:57.000000 hebill-1.2.4/hebill/mysql/table/data/core.py
+-rw-rw-rw-   0        0        0     1710 2024-03-22 11:35:59.000000 hebill-1.2.4/hebill/mysql/table/data/drop.py
+-rw-rw-rw-   0        0        0     1564 2024-02-27 01:58:04.000000 hebill-1.2.4/hebill/mysql/table/data/insert.py
+-rw-rw-rw-   0        0        0     2041 2024-03-22 11:35:59.000000 hebill-1.2.4/hebill/mysql/table/data/search.py
+-rw-rw-rw-   0        0        0      722 2024-04-05 03:00:49.000000 hebill-1.2.4/hebill/mysql/table/data/update.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.307661 hebill-1.2.4/hebill/numeric/
+-rw-rw-rw-   0        0        0       27 2024-04-09 02:38:00.000000 hebill-1.2.4/hebill/numeric/__init__.py
+-rw-rw-rw-   0        0        0     1127 2024-04-10 07:14:07.000000 hebill-1.2.4/hebill/numeric/constants.py
+-rw-rw-rw-   0        0        0    14209 2024-04-11 00:11:08.000000 hebill-1.2.4/hebill/numeric/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.309661 hebill-1.2.4/hebill/pdf/
+-rw-rw-rw-   0        0        0      465 2024-04-19 11:23:54.000000 hebill-1.2.4/hebill/pdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.310795 hebill-1.2.4/hebill/pdf/component/
+-rw-rw-rw-   0        0        0        0 2024-03-19 08:57:35.000000 hebill-1.2.4/hebill/pdf/component/__init__.py
+-rw-rw-rw-   0        0        0     2485 2024-04-09 02:04:40.000000 hebill-1.2.4/hebill/pdf/component/core.py
+-rw-rw-rw-   0        0        0     1121 2024-03-20 08:39:59.000000 hebill-1.2.4/hebill/pdf/constants.py
+-rw-rw-rw-   0        0        0     8799 2024-04-19 11:39:48.000000 hebill-1.2.4/hebill/pdf/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.314800 hebill-1.2.4/hebill/pdf/features/
+-rw-rw-rw-   0        0        0        0 2024-04-09 01:59:41.000000 hebill-1.2.4/hebill/pdf/features/__init__.py
+-rw-rw-rw-   0        0        0      441 2024-04-09 02:04:40.000000 hebill-1.2.4/hebill/pdf/features/configs.py
+-rw-rw-rw-   0        0        0     1419 2024-04-09 02:04:40.000000 hebill-1.2.4/hebill/pdf/features/document_configs.py
+-rw-rw-rw-   0        0        0     1382 2024-04-09 02:04:40.000000 hebill-1.2.4/hebill/pdf/features/page_configs.py
+-rw-rw-rw-   0        0        0     4891 2024-04-09 02:04:40.000000 hebill-1.2.4/hebill/pdf/features/styles.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.318135 hebill-1.2.4/hebill/pdf/library/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:28.000000 hebill-1.2.4/hebill/pdf/library/__init__.py
+-rw-rw-rw-   0        0        0     8548 2024-03-19 00:59:10.000000 hebill-1.2.4/hebill/pdf/library/configs_selector_color.py
+-rw-rw-rw-   0        0        0      826 2024-03-19 16:42:53.000000 hebill-1.2.4/hebill/pdf/library/configs_selector_font.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.330937 hebill-1.2.4/hebill/pdf/page/
+-rw-rw-rw-   0        0        0        0 2024-03-19 01:10:08.000000 hebill-1.2.4/hebill/pdf/page/__init__.py
+-rw-rw-rw-   0        0        0      886 2024-04-09 02:04:40.000000 hebill-1.2.4/hebill/pdf/page/_draw_.py
+-rw-rw-rw-   0        0        0      382 2024-03-20 07:59:42.000000 hebill-1.2.4/hebill/pdf/page/_draw_line.py
+-rw-rw-rw-   0        0        0      462 2024-03-20 07:59:42.000000 hebill-1.2.4/hebill/pdf/page/_draw_shape.py
+-rw-rw-rw-   0        0        0      447 2024-03-20 07:59:42.000000 hebill-1.2.4/hebill/pdf/page/_draw_text.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 02:04:40.000000 hebill-1.2.4/hebill/pdf/page/core.py
+-rw-rw-rw-   0        0        0      413 2024-03-20 00:39:33.000000 hebill-1.2.4/hebill/pdf/page/draw_circle.py
+-rw-rw-rw-   0        0        0      465 2024-03-20 00:39:33.000000 hebill-1.2.4/hebill/pdf/page/draw_ellipse.py
+-rw-rw-rw-   0        0        0     1047 2024-03-20 08:33:48.000000 hebill-1.2.4/hebill/pdf/page/draw_grids.py
+-rw-rw-rw-   0        0        0      457 2024-03-20 00:39:33.000000 hebill-1.2.4/hebill/pdf/page/draw_line.py
+-rw-rw-rw-   0        0        0     1528 2024-03-20 07:59:42.000000 hebill-1.2.4/hebill/pdf/page/draw_path.py
+-rw-rw-rw-   0        0        0      726 2024-03-20 04:01:39.000000 hebill-1.2.4/hebill/pdf/page/draw_rect.py
+-rw-rw-rw-   0        0        0      668 2024-03-21 15:41:19.000000 hebill-1.2.4/hebill/pdf/page/draw_string.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.334454 hebill-1.2.4/hebill/pypi/
+-rw-rw-rw-   0        0        0       24 2024-04-05 13:22:37.000000 hebill-1.2.4/hebill/pypi/__init__.py
+-rw-rw-rw-   0        0        0     8933 2024-04-24 03:54:15.000000 hebill-1.2.4/hebill/pypi/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.336454 hebill-1.2.4/hebill/string/
+-rw-rw-rw-   0        0        0       26 2024-04-10 02:30:43.000000 hebill-1.2.4/hebill/string/__init__.py
+-rw-rw-rw-   0        0        0     1571 2024-04-19 11:39:48.000000 hebill-1.2.4/hebill/string/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.337453 hebill-1.2.4/hebill/sys/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.4/hebill/sys/__init__.py
+-rw-rw-rw-   0        0        0      626 2024-04-19 14:39:39.000000 hebill-1.2.4/hebill/sys/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.338456 hebill-1.2.4/hebill/url/
+-rw-rw-rw-   0        0        0       23 2024-04-05 01:59:44.000000 hebill-1.2.4/hebill/url/__init__.py
+-rw-rw-rw-   0        0        0      317 2024-04-05 01:34:58.000000 hebill-1.2.4/hebill/url/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.340454 hebill-1.2.4/hebill/webserver/
+-rw-rw-rw-   0        0        0       57 2024-04-19 11:39:48.000000 hebill-1.2.4/hebill/webserver/__init__.py
+-rw-rw-rw-   0        0        0     1508 2024-04-19 11:41:02.000000 hebill-1.2.4/hebill/webserver/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.341454 hebill-1.2.4/hebill/webserver/features/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:18.000000 hebill-1.2.4/hebill/webserver/features/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.342455 hebill-1.2.4/hebill/webserver/features/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:55.000000 hebill-1.2.4/hebill/webserver/features/client/__init__.py
+-rw-rw-rw-   0        0        0      143 2024-04-03 02:21:39.000000 hebill-1.2.4/hebill/webserver/features/client/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.343963 hebill-1.2.4/hebill/webserver/features/request/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:21.000000 hebill-1.2.4/hebill/webserver/features/request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.344973 hebill-1.2.4/hebill/webserver/features/request/cookie/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:27:33.000000 hebill-1.2.4/hebill/webserver/features/request/cookie/__init__.py
+-rw-rw-rw-   0        0        0      205 2024-04-03 03:01:28.000000 hebill-1.2.4/hebill/webserver/features/request/cookie/core.py
+-rw-rw-rw-   0        0        0      587 2024-04-03 07:11:58.000000 hebill-1.2.4/hebill/webserver/features/request/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.345974 hebill-1.2.4/hebill/webserver/features/request/get/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:55.000000 hebill-1.2.4/hebill/webserver/features/request/get/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-03 08:50:01.000000 hebill-1.2.4/hebill/webserver/features/request/get/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.346972 hebill-1.2.4/hebill/webserver/features/request/headers/
+-rw-rw-rw-   0        0        0        0 2024-04-03 07:07:38.000000 hebill-1.2.4/hebill/webserver/features/request/headers/__init__.py
+-rw-rw-rw-   0        0        0      219 2024-04-03 08:50:01.000000 hebill-1.2.4/hebill/webserver/features/request/headers/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.347972 hebill-1.2.4/hebill/webserver/features/request/post/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:09:59.000000 hebill-1.2.4/hebill/webserver/features/request/post/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-04-03 02:21:39.000000 hebill-1.2.4/hebill/webserver/features/request/post/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.349202 hebill-1.2.4/hebill/webserver/features/website/
+-rw-rw-rw-   0        0        0        0 2024-04-03 02:05:11.000000 hebill-1.2.4/hebill/webserver/features/website/__init__.py
+-rw-rw-rw-   0        0        0      479 2024-04-03 03:01:28.000000 hebill-1.2.4/hebill/webserver/features/website/core.py
+-rw-rw-rw-   0        0        0     2503 2024-04-19 11:39:48.000000 hebill-1.2.4/hebill/webserver/handle.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:55:27.350711 hebill-1.2.4/hebill.egg-info/
+-rw-rw-rw-   0        0        0      924 2024-04-24 03:55:26.000000 hebill-1.2.4/hebill.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7080 2024-04-24 03:55:27.000000 hebill-1.2.4/hebill.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:55:26.000000 hebill-1.2.4/hebill.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-24 03:55:26.000000 hebill-1.2.4/hebill.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 03:55:26.000000 hebill-1.2.4/hebill.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      595 2024-04-24 03:55:26.000000 hebill-1.2.4/pack_upload_setup.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:55:27.352720 hebill-1.2.4/setup.cfg
```

### Comparing `hebill-1.2.3/PKG-INFO` & `hebill-1.2.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hebill
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python Hebill
 Requires-Python: >=3.12
 Description-Content-Type: text/plain
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: wxpython==4.2.1
```

### Comparing `hebill-1.2.3/hebill.egg-info/PKG-INFO` & `hebill-1.2.4/hebill.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hebill
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python Hebill
 Requires-Python: >=3.12
 Description-Content-Type: text/plain
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: wxpython==4.2.1
```

### Comparing `hebill-1.2.3/pack_upload_setup.py` & `hebill-1.2.4/pack_upload_setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
-from setuptools import setup
+from setuptools import setup, find_packages
 setup(
     name='hebill',
-    version='1.2.3',
+    version='1.2.4',
     description='Python Hebill',
     long_description=open(r'D:\SDK\GitHub\python_hebill\hebill\README.MD', encoding='utf-8').read(),
     long_description_content_type='text/plain',
-    packages=[
-        'hebill',
-    ],
+    packages=find_packages(),
     install_requires=[
         'psutil==5.9.8',
         'pillow==10.3.0',
         'requests==2.31.0',
         'wxpython==4.2.1',
         'reportlab==4.1.0',
         'PyMySQL==1.1.0',
```

