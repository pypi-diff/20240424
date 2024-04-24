# Comparing `tmp/pyptt-1.2.8.tar.gz` & `tmp/pyptt-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyptt-1.2.8.tar", last modified: Tue Apr 23 02:38:00 2024, max compression
+gzip compressed data, was "pyptt-1.2.9.tar", last modified: Wed Apr 24 04:54:21 2024, max compression
```

## Comparing `pyptt-1.2.8.tar` & `pyptt-1.2.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.890526 pyptt-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-23 02:37:55.000000 pyptt-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 02:37:55.000000 pyptt-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-23 02:38:00.890526 pyptt-1.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.886526 pyptt-1.2.8/PyPtt/
--rw-r--r--   0 runner    (1001) docker     (127)    32101 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/PTT.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_call_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_change_pw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_del_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_board_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_board_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_bottom_post_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_favourite_board.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_newest_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_post_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_give_money.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_has_new_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_loginout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_mark_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_reply_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_search_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_set_board_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/check_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/connect_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.886526 pyptt-1.2.8/PyPtt/lang/
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/lang/en_US.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/lang/zh_TW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/lib_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    54872 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/screens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.890526 pyptt-1.2.8/PyPtt/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/ssl/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/ssl/key.pem
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.890526 pyptt-1.2.8/PyPtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-23 02:37:55.000000 pyptt-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:38:00.890526 pyptt-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-23 02:37:55.000000 pyptt-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:54:21.575927 pyptt-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-24 04:54:14.000000 pyptt-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 04:54:14.000000 pyptt-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-24 04:54:21.575927 pyptt-1.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:54:21.571927 pyptt-1.2.9/PyPtt/
+-rw-r--r--   0 runner    (1001) docker     (127)    32101 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/PTT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 04:54:21.000000 pyptt-1.2.9/PyPtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_call_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_change_pw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_del_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_board_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_board_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_bottom_post_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_favourite_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_newest_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_post_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_give_money.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_has_new_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_loginout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_mark_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_reply_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_set_board_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/_api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/check_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14410 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/connect_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/lang_en_US.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/lang_zh_TW.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/lib_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54872 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:54:21.571927 pyptt-1.2.9/PyPtt/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/ssl/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/ssl/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-24 04:54:14.000000 pyptt-1.2.9/PyPtt/ssl_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:54:21.571927 pyptt-1.2.9/PyPtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-24 04:54:21.000000 pyptt-1.2.9/PyPtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 04:54:21.000000 pyptt-1.2.9/PyPtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:54:21.000000 pyptt-1.2.9/PyPtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 04:54:21.000000 pyptt-1.2.9/PyPtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 04:54:21.000000 pyptt-1.2.9/PyPtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-24 04:54:14.000000 pyptt-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:54:21.575927 pyptt-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-24 04:54:14.000000 pyptt-1.2.9/setup.py
```

### Comparing `pyptt-1.2.8/LICENSE` & `pyptt-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PKG-INFO` & `pyptt-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.2.8
+Version: 1.2.9
 Summary: PyPtt
 Home-page: https://pyptt.cc/
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `pyptt-1.2.8/PyPtt/PTT.py` & `pyptt-1.2.9/PyPtt/PTT.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_bucket.py` & `pyptt-1.2.9/PyPtt/_api_bucket.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_call_status.py` & `pyptt-1.2.9/PyPtt/_api_call_status.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_change_pw.py` & `pyptt-1.2.9/PyPtt/_api_change_pw.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_comment.py` & `pyptt-1.2.9/PyPtt/_api_comment.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_del_post.py` & `pyptt-1.2.9/PyPtt/_api_del_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_board_info.py` & `pyptt-1.2.9/PyPtt/_api_get_board_info.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_board_list.py` & `pyptt-1.2.9/PyPtt/_api_get_board_list.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_bottom_post_list.py` & `pyptt-1.2.9/PyPtt/_api_get_bottom_post_list.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_favourite_board.py` & `pyptt-1.2.9/PyPtt/_api_get_favourite_board.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_newest_index.py` & `pyptt-1.2.9/PyPtt/_api_get_newest_index.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_post.py` & `pyptt-1.2.9/PyPtt/_api_get_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_post_index.py` & `pyptt-1.2.9/PyPtt/_api_get_post_index.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_time.py` & `pyptt-1.2.9/PyPtt/_api_get_time.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_get_user.py` & `pyptt-1.2.9/PyPtt/_api_get_user.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_give_money.py` & `pyptt-1.2.9/PyPtt/_api_give_money.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_has_new_mail.py` & `pyptt-1.2.9/PyPtt/_api_has_new_mail.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_loginout.py` & `pyptt-1.2.9/PyPtt/_api_loginout.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_mail.py` & `pyptt-1.2.9/PyPtt/_api_mail.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_mark_post.py` & `pyptt-1.2.9/PyPtt/_api_mark_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_post.py` & `pyptt-1.2.9/PyPtt/_api_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_reply_post.py` & `pyptt-1.2.9/PyPtt/_api_reply_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_search_user.py` & `pyptt-1.2.9/PyPtt/_api_search_user.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_set_board_title.py` & `pyptt-1.2.9/PyPtt/_api_set_board_title.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/_api_util.py` & `pyptt-1.2.9/PyPtt/_api_util.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/check_value.py` & `pyptt-1.2.9/PyPtt/check_value.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/command.py` & `pyptt-1.2.9/PyPtt/command.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/config.py` & `pyptt-1.2.9/PyPtt/config.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/connect_core.py` & `pyptt-1.2.9/PyPtt/connect_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,33 @@
 import PyPtt
 from . import command
 from . import data_type
 from . import exceptions
 from . import i18n
 from . import log
 from . import screens
+from . import ssl_config
 
 websockets.http.USER_AGENT += f' PyPtt/{PyPtt.__version__}'
 
-_script_path = os.path.dirname(os.path.abspath(__file__))
+_script_path = os.path.dirname(__file__)
+
+
+def ssl_init():
+    if not os.path.exists(f'{_script_path}/ssl'):
+        os.mkdir(f'{_script_path}/ssl')
+
+    with open(f"{_script_path}/ssl/cert.pem", 'w') as f:
+        f.write(ssl_config.cert)
+
+    with open(f"{_script_path}/ssl/key.pem", 'w') as f:
+        f.write(ssl_config.key)
+
+
+ssl_init()
 
 ssl_context = ssl.create_default_context()
 ssl_context.load_cert_chain(certfile=f"{_script_path}/ssl/cert.pem", keyfile=f"{_script_path}/ssl/key.pem")
 ssl_context.minimum_version = ssl.TLSVersion.TLSv1_2
 
 
 class TargetUnit:
```

### Comparing `pyptt-1.2.8/PyPtt/data_type.py` & `pyptt-1.2.9/PyPtt/data_type.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/exceptions.py` & `pyptt-1.2.9/PyPtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/i18n.py` & `pyptt-1.2.9/PyPtt/i18n.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
 import random
 
-import yaml
-
 from . import __version__
 from . import data_type
 
 locale_pool = {
     data_type.Language.ENGLISH,
     data_type.Language.MANDARIN
 }
 
-_script_path = os.path.dirname(os.path.abspath(__file__))
+_script_path = os.path.dirname(__file__)
 _lang_data = {}
 
 mapping = {
     '{version}': __version__,
 }
 
 
@@ -26,20 +24,22 @@
     return string
 
 
 def init(locale: str, cache: bool = False) -> None:
     if locale not in locale_pool:
         raise ValueError(f'Unknown locale: {locale}')
 
-    language_file = f'{_script_path}/lang/{locale}.yaml'
-    if not os.path.exists(language_file):
-        raise ValueError(f'Unknown locale file: {language_file}')
+    if locale == data_type.Language.ENGLISH:
+        from . import lang_en_US as lang
+    elif locale == data_type.Language.MANDARIN:
+        from . import lang_zh_TW as lang
+    string_data = lang.string_data
 
-    with open(language_file, "r") as f:
-        string_data = yaml.safe_load(f)
+    if string_data is None:
+        raise ValueError(f'Unknown locale: {locale}')
 
     for k, v in string_data.items():
 
         if isinstance(v, list):
             v = random.choice(v)
         elif isinstance(v, str):
             pass
```

### Comparing `pyptt-1.2.8/PyPtt/lib_util.py` & `pyptt-1.2.9/PyPtt/lib_util.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/log.py` & `pyptt-1.2.9/PyPtt/log.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/screens.py` & `pyptt-1.2.9/PyPtt/screens.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/service.py` & `pyptt-1.2.9/PyPtt/service.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt/ssl/cert.pem` & `pyptt-1.2.9/PyPtt/ssl/cert.pem`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/PyPtt.egg-info/PKG-INFO` & `pyptt-1.2.9/PyPtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.2.8
+Version: 1.2.9
 Summary: PyPtt
 Home-page: https://pyptt.cc/
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `pyptt-1.2.8/PyPtt.egg-info/SOURCES.txt` & `pyptt-1.2.9/PyPtt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 PyPtt/check_value.py
 PyPtt/command.py
 PyPtt/config.py
 PyPtt/connect_core.py
 PyPtt/data_type.py
 PyPtt/exceptions.py
 PyPtt/i18n.py
+PyPtt/lang_en_US.py
+PyPtt/lang_zh_TW.py
 PyPtt/lib_util.py
 PyPtt/log.py
 PyPtt/screens.py
 PyPtt/service.py
+PyPtt/ssl_config.py
 PyPtt.egg-info/PKG-INFO
 PyPtt.egg-info/SOURCES.txt
 PyPtt.egg-info/dependency_links.txt
 PyPtt.egg-info/requires.txt
 PyPtt.egg-info/top_level.txt
-PyPtt/lang/en_US.yaml
-PyPtt/lang/zh_TW.yaml
 PyPtt/ssl/cert.pem
 PyPtt/ssl/key.pem
```

### Comparing `pyptt-1.2.8/README.md` & `pyptt-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.8/setup.py` & `pyptt-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,12 +120,11 @@
         'uao',
         'requests',
         'AutoStrEnum',
         'PyYAML',
     ],
     package_data={
         'PyPtt': [
-            'lang/*.yaml',
             'ssl/*.pem',
         ],
     }
 )
```

