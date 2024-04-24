# Comparing `tmp/ncmlistdownloader-1.0.1.240422a1.tar.gz` & `tmp/ncmlistdownloader-1.0.1.240424a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.1.240422a1.tar", last modified: Mon Apr 22 14:58:37 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.1.240424a1.tar", last modified: Wed Apr 24 15:01:15 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.1.240422a1.tar` & `ncmlistdownloader-1.0.1.240424a1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.657003 ncmlistdownloader-1.0.1.240422a1/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/LICENSE
--rw-rw-rw-   0        0        0     1399 2024-04-22 14:58:37.653470 ncmlistdownloader-1.0.1.240422a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.602011 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1263 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.627464 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     1628 2024-04-22 14:56:18.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0      649 2024-04-22 14:58:10.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/common.py
--rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/find_from_id.py
--rw-rw-rw-   0        0        0      990 2024-04-22 14:57:54.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.637429 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2859 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2184 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.639424 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.643414 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.647403 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.650395 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     7481 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:58:37.652469 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1399 2024-04-22 14:58:37.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-04-22 14:58:37.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 14:58:37.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-22 14:58:37.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-22 14:58:37.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-22 14:58:37.000000 ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 14:58:37.657965 ncmlistdownloader-1.0.1.240422a1/setup.cfg
--rw-rw-rw-   0        0        0     1758 2024-04-22 14:58:02.000000 ncmlistdownloader-1.0.1.240422a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.175533 ncmlistdownloader-1.0.1.240424a1/
+-rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/LICENSE
+-rw-rw-rw-   0        0        0     1399 2024-04-24 15:01:15.175533 ncmlistdownloader-1.0.1.240424a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.120699 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1263 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.146867 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     1628 2024-04-22 14:56:18.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0      649 2024-04-22 14:58:10.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/common.py
+-rw-rw-rw-   0        0        0     1353 2024-04-24 15:00:22.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/download.py
+-rw-rw-rw-   0        0        0     2501 2024-04-22 14:56:53.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1048 2024-04-24 15:00:39.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.157960 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2859 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2184 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.162941 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.164234 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.167780 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2323 2024-04-22 14:49:08.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.171762 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     8163 2024-04-24 15:00:54.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:01:15.174753 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1399 2024-04-24 15:01:15.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-04-24 15:01:15.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:01:15.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-24 15:01:15.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-24 15:01:15.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-24 15:01:15.000000 ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:01:15.175533 ncmlistdownloader-1.0.1.240424a1/setup.cfg
+-rw-rw-rw-   0        0        0     1758 2024-04-24 15:00:44.000000 ncmlistdownloader-1.0.1.240424a1/setup.py
```

### Comparing `ncmlistdownloader-1.0.1.240422a1/LICENSE` & `ncmlistdownloader-1.0.1.240424a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/PKG-INFO` & `ncmlistdownloader-1.0.1.240424a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.240422a1
+Version: 1.0.1.240424a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/__init__.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/common.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/find_from_id.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/cmd/json_io.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/cmd/json_io.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 '''
 ncmlistdownloader/cmd/json_io.py
-Core.Ver.1.0.1.240422a1
+Core.Ver.1.0.1.240424a1
 Author: CooooldWind_
 '''
 
 from ncmlistdownloader.song import *
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.cmd.common import *
 
 def json_save_list(pl: Playlist):
     path = str(input_func(notice = "Input the file's page"))
     d = {
-        'type': 'downloading_list',
+        'type': 'downloading_list_ncmld',
         'global_config': GLOBAL_CONFIG_MODEL,
         'track': [],
     }
     t = []
     for i in pl.track:
         t.append({
             'type': 'song',
             'info': {
                 'title': i.title,
                 'artist': i.artist,
                 'album': i.album,
                 'id': i.id,
+                'pic_url': i.url_info['album_pic']
             },
             'global': True,
             'downloading_config': GLOBAL_CONFIG_MODEL,
         })
     d['track'] = t
     with open(path, 'w+', encoding = 'utf-8') as file:
         json.dump(d, file, ensure_ascii = False, sort_keys = True)
```

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader/song/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/song/__init__.py
-Core.Ver.1.0.0.240412a2
+Core.Ver.1.0.0.240424a1
 Author: CooooldWind_
 '''
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
@@ -190,15 +190,17 @@
         往文件里面写入歌曲信息
         ----------
         参数: 
         1. `filename`: 文件名，字符串，仅mp3/flac格式
         '''
         filename_ready = self.get_formated_filename('mp3')
         if filename == 'No filename':
-            filename = self.filename_info['song']
+            if self.filename_info.get('song') == None:
+                filename = filename_ready
+            else: filename = self.filename_info['song']
         attribute_write(filename = filename, info = self.processed_info)
 
     def cover_write(self, filename = 'No filename', cover_filename = 'No cover_filename'):
         '''
         专辑封面写入
         ----------
         参数: 
@@ -214,8 +216,23 @@
     def lyric_write(self, filename = 'No filename', lyric_filename = 'No lyric_filename'):
         if filename == 'No filename':
             filename = self.filename_info['song']
         if lyric_filename == 'No lyric_filename':
             lyric_filename = self.filename_info['lyric']
         lyric_write(filename = filename, lyric_filename = lyric_filename)
 
-    
+    def auto_run(self, d = None):
+        if d['song_download'] == True:
+            self.song_download()
+        if d['cover_download'] == True:
+            self.cover_download()
+        if d['lyric_download'] == True:
+            self.lyric_get()
+        if d['attribute_write'] == True:
+            self.attribute_write()
+        if d['cover_write'] == True:
+            self.cover_write()
+        if d['lyric_write'] == True:
+            self.lyric_write()
+
+    def multi_run(self, d = None):
+        threading.Thread(target = self.auto_run, args = (d,)).start()
```

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.1.240422a1
+Version: 1.0.1.240424a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.1.240422a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.1.240424a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
 ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
 ncmlistdownloader.egg-info/top_level.txt
 ncmlistdownloader/cmd/__init__.py
 ncmlistdownloader/cmd/common.py
+ncmlistdownloader/cmd/download.py
 ncmlistdownloader/cmd/find_from_id.py
 ncmlistdownloader/cmd/json_io.py
 ncmlistdownloader/common/__init__.py
 ncmlistdownloader/common/encode_sec_key.py
 ncmlistdownloader/common/global_args.py
 ncmlistdownloader/common/thread_test.py
 ncmlistdownloader/downloader/__init__.py
```

### Comparing `ncmlistdownloader-1.0.1.240422a1/setup.py` & `ncmlistdownloader-1.0.1.240424a1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.1.240422a1",
+    version = "1.0.1.240424a1",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

