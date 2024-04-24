# Comparing `tmp/zoltraak-0.1.5.tar.gz` & `tmp/zoltraak-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoltraak-0.1.5.tar", last modified: Wed Apr 24 07:08:35 2024, max compression
+gzip compressed data, was "zoltraak-0.1.6.tar", last modified: Wed Apr 24 07:09:53 2024, max compression
```

## Comparing `zoltraak-0.1.5.tar` & `zoltraak-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,46 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:08:35.447187 zoltraak-0.1.5/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:08:35.447034 zoltraak-0.1.5/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.5/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 07:08:35.447350 zoltraak-0.1.5/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      426 2024-04-24 07:08:27.000000 zoltraak-0.1.5/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:08:35.445167 zoltraak-0.1.5/zoltraak/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.5/zoltraak/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5713 2024-04-24 06:17:03.000000 zoltraak-0.1.5/zoltraak/cli.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.5/zoltraak/converter.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:08:35.446706 zoltraak-0.1.5/zoltraak/llms/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1065 2024-04-21 23:52:43.000000 zoltraak-0.1.5/zoltraak/llms/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      946 2024-04-16 05:55:37.000000 zoltraak-0.1.5/zoltraak/llms/claude.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    10617 2024-04-24 06:37:12.000000 zoltraak-0.1.5/zoltraak/md_generator.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:08:35.446047 zoltraak-0.1.5/zoltraak.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:08:35.000000 zoltraak-0.1.5/zoltraak.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      345 2024-04-24 07:08:35.000000 zoltraak-0.1.5/zoltraak.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 07:08:35.000000 zoltraak-0.1.5/zoltraak.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 07:08:35.000000 zoltraak-0.1.5/zoltraak.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        7 2024-04-24 07:08:35.000000 zoltraak-0.1.5/zoltraak.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 07:08:35.000000 zoltraak-0.1.5/zoltraak.egg-info/top_level.txt
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.616243 zoltraak-0.1.6/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:09:53.616113 zoltraak-0.1.6/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    50235 2024-04-24 03:41:33.000000 zoltraak-0.1.6/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-04-24 07:09:53.616278 zoltraak-0.1.6/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      425 2024-04-24 07:09:50.000000 zoltraak-0.1.6/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.608419 zoltraak-0.1.6/zoltraak/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-15 18:33:00.000000 zoltraak-0.1.6/zoltraak/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5713 2024-04-24 06:17:03.000000 zoltraak-0.1.6/zoltraak/cli.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    17101 2024-04-24 03:11:27.000000 zoltraak-0.1.6/zoltraak/converter.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.609593 zoltraak-0.1.6/zoltraak/llms/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1065 2024-04-21 23:52:43.000000 zoltraak-0.1.6/zoltraak/llms/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      946 2024-04-16 05:55:37.000000 zoltraak-0.1.6/zoltraak/llms/claude.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    10617 2024-04-24 06:37:12.000000 zoltraak-0.1.6/zoltraak/md_generator.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.607086 zoltraak-0.1.6/zoltraak/setting/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.609879 zoltraak-0.1.6/zoltraak/setting/architect/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      183 2024-04-24 03:01:15.000000 zoltraak-0.1.6/zoltraak/setting/architect/architect.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.614374 zoltraak-0.1.6/zoltraak/setting/compiler/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     7114 2024-04-22 10:16:30.000000 zoltraak-0.1.6/zoltraak/setting/compiler/biz_consult copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3766 2024-04-22 10:21:52.000000 zoltraak-0.1.6/zoltraak/setting/compiler/biz_consult.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1093 2024-04-22 00:24:25.000000 zoltraak-0.1.6/zoltraak/setting/compiler/dev_akirapp.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       69 2024-04-22 23:55:14.000000 zoltraak-0.1.6/zoltraak/setting/compiler/dev_front.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1463 2024-04-22 00:24:12.000000 zoltraak-0.1.6/zoltraak/setting/compiler/dev_func.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2302 2024-04-22 10:10:26.000000 zoltraak-0.1.6/zoltraak/setting/compiler/dev_obj.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1413 2024-04-22 00:43:30.000000 zoltraak-0.1.6/zoltraak/setting/compiler/dev_obj_lisp.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2759 2024-04-22 00:47:40.000000 zoltraak-0.1.6/zoltraak/setting/compiler/dev_obj_lisp_g.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2221 2024-04-22 00:56:55.000000 zoltraak-0.1.6/zoltraak/setting/compiler/dev_obj_lisp_g_base64.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      100 2024-04-21 22:59:42.000000 zoltraak-0.1.6/zoltraak/setting/compiler/encode_lisp.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      447 2024-04-22 16:38:24.000000 zoltraak-0.1.6/zoltraak/setting/compiler/general_def.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3832 2024-04-21 23:02:20.000000 zoltraak-0.1.6/zoltraak/setting/compiler/general_reqdef.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      772 2024-04-24 02:39:26.000000 zoltraak-0.1.6/zoltraak/setting/compiler/ref_create_directory.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.614634 zoltraak-0.1.6/zoltraak/setting/developer/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 03:16:20.000000 zoltraak-0.1.6/zoltraak/setting/developer/dev_python.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.614724 zoltraak-0.1.6/zoltraak/setting/encryption/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      432 2024-04-21 18:24:02.000000 zoltraak-0.1.6/zoltraak/setting/encryption/emoji.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.615354 zoltraak-0.1.6/zoltraak/setting/formatter/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      118 2024-04-21 18:10:10.000000 zoltraak-0.1.6/zoltraak/setting/formatter/md_comment.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      193 2024-04-21 18:04:36.000000 zoltraak-0.1.6/zoltraak/setting/formatter/py_comment.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.615693 zoltraak-0.1.6/zoltraak/setting/interpretspec/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4799 2024-04-21 18:35:46.000000 zoltraak-0.1.6/zoltraak/setting/interpretspec/hirokichi.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-04-24 07:09:53.609155 zoltraak-0.1.6/zoltraak.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       52 2024-04-24 07:09:53.000000 zoltraak-0.1.6/zoltraak.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1144 2024-04-24 07:09:53.000000 zoltraak-0.1.6/zoltraak.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-04-24 07:09:53.000000 zoltraak-0.1.6/zoltraak.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-04-24 07:09:53.000000 zoltraak-0.1.6/zoltraak.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        7 2024-04-24 07:09:53.000000 zoltraak-0.1.6/zoltraak.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        9 2024-04-24 07:09:53.000000 zoltraak-0.1.6/zoltraak.egg-info/top_level.txt
```

### Comparing `zoltraak-0.1.5/README.md` & `zoltraak-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.5/zoltraak/cli.py` & `zoltraak-0.1.6/zoltraak/cli.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.5/zoltraak/converter.py` & `zoltraak-0.1.6/zoltraak/converter.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.5/zoltraak/llms/claude.py` & `zoltraak-0.1.6/zoltraak/llms/claude.py`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.5/zoltraak/llms/claude.txt` & `zoltraak-0.1.6/zoltraak/llms/claude.txt`

 * *Files identical despite different names*

### Comparing `zoltraak-0.1.5/zoltraak/md_generator.py` & `zoltraak-0.1.6/zoltraak/md_generator.py`

 * *Files identical despite different names*

