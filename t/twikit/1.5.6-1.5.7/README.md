# Comparing `tmp/twikit-1.5.6.tar.gz` & `tmp/twikit-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.5.6.tar", last modified: Tue Apr 23 16:28:58 2024, max compression
+gzip compressed data, was "twikit-1.5.7.tar", last modified: Wed Apr 24 16:53:59 2024, max compression
```

## Comparing `twikit-1.5.6.tar` & `twikit-1.5.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 16:28:58.595224 twikit-1.5.6/
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.6/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-23 16:28:58.592231 twikit-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 16:28:58.595224 twikit-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:28:58.508456 twikit-1.5.6/twikit/
--rw-rw-rw-   0        0        0      658 2024-04-23 16:10:56.000000 twikit-1.5.6/twikit/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-04-23 16:10:15.000000 twikit-1.5.6/twikit/bookmark.py
--rw-rw-rw-   0        0        0   142561 2024-04-23 16:24:09.000000 twikit-1.5.6/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.6/twikit/community.py
--rw-rw-rw-   0        0        0     2666 2024-04-22 14:20:57.000000 twikit-1.5.6/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.6/twikit/group.py
--rw-rw-rw-   0        0        0     2095 2024-04-23 16:02:50.000000 twikit-1.5.6/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.6/twikit/notification.py
--rw-rw-rw-   0        0        0        0 2024-04-23 16:07:38.000000 twikit-1.5.6/twikit/py.typed
--rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/trend.py
--rw-rw-rw-   0        0        0    22843 2024-04-23 15:35:16.000000 twikit-1.5.6/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:28:58.589239 twikit-1.5.6/twikit/twikit_async/
--rw-rw-rw-   0        0        0      610 2024-04-23 16:10:47.000000 twikit-1.5.6/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-04-23 16:10:22.000000 twikit-1.5.6/twikit/twikit_async/bookmark.py
--rw-rw-rw-   0        0        0   144937 2024-04-23 15:33:35.000000 twikit-1.5.6/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.6/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.6/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    22724 2024-04-23 15:36:30.000000 twikit-1.5.6/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-04-16 15:30:17.000000 twikit-1.5.6/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.6/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.6/twikit/user.py
--rw-rw-rw-   0        0        0    30070 2024-04-22 14:10:16.000000 twikit-1.5.6/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:28:58.533388 twikit-1.5.6/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-23 16:28:58.000000 twikit-1.5.6/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      857 2024-04-23 16:28:58.000000 twikit-1.5.6/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:28:58.000000 twikit-1.5.6/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-23 16:28:58.000000 twikit-1.5.6/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 16:28:58.000000 twikit-1.5.6/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 16:53:59.978966 twikit-1.5.7/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.5.7/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-24 16:53:59.975973 twikit-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.5.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:53:59.978966 twikit-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:53:59.899179 twikit-1.5.7/twikit/
+-rw-rw-rw-   0        0        0      658 2024-04-24 16:49:51.000000 twikit-1.5.7/twikit/__init__.py
+-rw-rw-rw-   0        0        0     1686 2024-04-23 16:10:15.000000 twikit-1.5.7/twikit/bookmark.py
+-rw-rw-rw-   0        0        0   142787 2024-04-24 16:49:04.000000 twikit-1.5.7/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-04-15 14:41:30.000000 twikit-1.5.7/twikit/community.py
+-rw-rw-rw-   0        0        0     2666 2024-04-22 14:20:57.000000 twikit-1.5.7/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.5.7/twikit/group.py
+-rw-rw-rw-   0        0        0     2095 2024-04-23 16:02:50.000000 twikit-1.5.7/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 14:30:38.000000 twikit-1.5.7/twikit/notification.py
+-rw-rw-rw-   0        0        0        0 2024-04-23 16:07:38.000000 twikit-1.5.7/twikit/py.typed
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/trend.py
+-rw-rw-rw-   0        0        0    22891 2024-04-24 16:28:18.000000 twikit-1.5.7/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:53:59.972981 twikit-1.5.7/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      610 2024-04-23 16:10:47.000000 twikit-1.5.7/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0     1758 2024-04-23 16:10:22.000000 twikit-1.5.7/twikit/twikit_async/bookmark.py
+-rw-rw-rw-   0        0        0   145199 2024-04-24 16:49:39.000000 twikit-1.5.7/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-04-15 14:48:23.000000 twikit-1.5.7/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2137 2024-04-14 11:11:58.000000 twikit-1.5.7/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    22772 2024-04-24 16:29:28.000000 twikit-1.5.7/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-04-16 15:30:17.000000 twikit-1.5.7/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.5.7/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-04-16 15:30:25.000000 twikit-1.5.7/twikit/user.py
+-rw-rw-rw-   0        0        0    30253 2024-04-24 16:45:39.000000 twikit-1.5.7/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:53:59.917130 twikit-1.5.7/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 16:53:59.000000 twikit-1.5.7/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.5.6/LICENSE` & `twikit-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/PKG-INFO` & `twikit-1.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.6
+Version: 1.5.7
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.6/README.md` & `twikit-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/setup.py` & `twikit-1.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/__init__.py` & `twikit-1.5.7/twikit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========================
 Twikit Twitter API Wrapper
 ==========================
 
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.5.6'
+__version__ = '1.5.7'
 
 from .bookmark import BookmarkFolder
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
 from .group import Group, GroupMessage
```

### Comparing `twikit-1.5.6/twikit/bookmark.py` & `twikit-1.5.7/twikit/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/client.py` & `twikit-1.5.7/twikit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,14 +160,15 @@
         --------
         >>> client.login(
         ...     auth_info_1='example_user',
         ...     auth_info_2='email@example.com',
         ...     password='00000000'
         ... )
         """
+        self.http.client.cookies.clear()
         guest_token = self._get_guest_token()
         headers = self._base_headers | {
             'x-guest-token': guest_token
         }
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
 
@@ -1428,15 +1429,15 @@
             else:
                 if tweet is None:
                     reply_to.append(tweet_object)
                 else:
                     replies = []
                     sr_cursor = None
                     show_replies = None
-                    # Reply to reply
+
                     for reply in entry['content']['items'][1:]:
                         if 'tweetcomposer' in reply['entryId']:
                             continue
                         if 'tweet' in find_dict(reply, 'result'):
                             reply = reply['tweet']
                         if 'tweet' in reply.get('entryId'):
                             rpl_data = find_dict(reply, 'result')[0]
@@ -1457,14 +1458,18 @@
                     tweet_object.replies = Result(
                         replies,
                         show_replies,
                         sr_cursor
                     )
                     replies_list.append(tweet_object)
 
+                    display_type = find_dict(entry, 'tweetDisplayType', True)
+                    if display_type and display_type[0] == 'SelfThread':
+                        tweet.thread = [tweet_object, *replies]
+
         if entries[-1]['entryId'].startswith('cursor'):
             # if has more replies
             reply_next_cursor = entries[-1]['content']['itemContent']['value']
             _fetch_more_replies = partial(self._get_more_replies,
                                           tweet_id, reply_next_cursor)
         else:
             reply_next_cursor = None
```

### Comparing `twikit-1.5.6/twikit/community.py` & `twikit-1.5.7/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/errors.py` & `twikit-1.5.7/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/group.py` & `twikit-1.5.7/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/http.py` & `twikit-1.5.7/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/list.py` & `twikit-1.5.7/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/message.py` & `twikit-1.5.7/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/notification.py` & `twikit-1.5.7/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/trend.py` & `twikit-1.5.7/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/tweet.py` & `twikit-1.5.7/twikit/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         self._client = client
         self._data = data
         self.user = user
 
         self.replies: Result[Tweet] | None = None
         self.reply_to: list[Tweet] | None = None
         self.related_tweets: list[Tweet] | None = None
+        self.thread: list[Tweet] | None = None
 
         self.id: str = data['rest_id']
 
         legacy = data['legacy']
         self.created_at: str = legacy['created_at']
         self.text: str = legacy['full_text']
```

### Comparing `twikit-1.5.6/twikit/twikit_async/__init__.py` & `twikit-1.5.7/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/bookmark.py` & `twikit-1.5.7/twikit/twikit_async/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/client.py` & `twikit-1.5.7/twikit/twikit_async/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
         --------
         >>> await client.login(
         ...     auth_info_1='example_user',
         ...     auth_info_2='email@example.com',
         ...     password='00000000'
         ... )
         """
+        self.http.client.cookies.clear()
         guest_token = await self._get_guest_token()
         headers = self._base_headers | {
             'x-guest-token': guest_token
         }
         headers.pop('X-Twitter-Active-User')
         headers.pop('X-Twitter-Auth-Type')
 
@@ -1474,14 +1475,18 @@
                     tweet_object.replies = Result(
                         replies,
                         show_replies,
                         sr_cursor
                     )
                     replies_list.append(tweet_object)
 
+                    display_type = find_dict(entry, 'tweetDisplayType', True)
+                    if display_type and display_type[0] == 'SelfThread':
+                        tweet.thread = [tweet_object, *replies]
+
         if entries[-1]['entryId'].startswith('cursor'):
             # if has more replies
             reply_next_cursor = entries[-1]['content']['itemContent']['value']
             _fetch_more_replies = partial(self._get_more_replies,
                                           tweet_id, reply_next_cursor)
         else:
             reply_next_cursor = None
```

### Comparing `twikit-1.5.6/twikit/twikit_async/community.py` & `twikit-1.5.7/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/errors.py` & `twikit-1.5.7/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/group.py` & `twikit-1.5.7/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/http.py` & `twikit-1.5.7/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/list.py` & `twikit-1.5.7/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/message.py` & `twikit-1.5.7/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/notification.py` & `twikit-1.5.7/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/trend.py` & `twikit-1.5.7/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/tweet.py` & `twikit-1.5.7/twikit/twikit_async/tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         self._client = client
         self._data = data
         self.user = user
 
         self.replies: Result[Tweet] | None = None
         self.reply_to: list[Tweet] | None = None
         self.related_tweets: list[Tweet] | None = None
+        self.thread: list[Tweet] | None = None
 
         self.id: str = data['rest_id']
 
         legacy = data['legacy']
         self.created_at: str = legacy['created_at']
         self.text: str = legacy['full_text']
```

### Comparing `twikit-1.5.6/twikit/twikit_async/user.py` & `twikit-1.5.7/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/twikit_async/utils.py` & `twikit-1.5.7/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/user.py` & `twikit-1.5.7/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.5.6/twikit/utils.py` & `twikit-1.5.7/twikit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,25 +397,32 @@
     @property
     def task_id(self) -> str | None:
         if self.response is None:
             return None
         return self.response['subtasks'][0]['subtask_id']
 
 
-def find_dict(obj: list | dict, key: str | int) -> list[Any]:
+def find_dict(
+    obj: list | dict, key: str | int, find_one: bool = False
+) -> list[Any]:
     """
     Retrieves elements from a nested dictionary.
     """
     results = []
     if isinstance(obj, dict):
         if key in obj:
             results.append(obj.get(key))
+            if find_one:
+                return results
     if isinstance(obj, (list, dict)):
         for elem in (obj if isinstance(obj, list) else obj.values()):
-            results += find_dict(elem, key)
+            r = find_dict(elem, key, find_one)
+            results += r
+            if r and find_one:
+                return results
     return results
 
 
 def get_query_id(url: str) -> str:
     """
     Extracts the identifier from a URL.
```

### Comparing `twikit-1.5.6/twikit.egg-info/PKG-INFO` & `twikit-1.5.7/twikit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.5.6
+Version: 1.5.7
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.5.6/twikit.egg-info/SOURCES.txt` & `twikit-1.5.7/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

