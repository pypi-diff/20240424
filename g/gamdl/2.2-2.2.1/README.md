# Comparing `tmp/gamdl-2.2.tar.gz` & `tmp/gamdl-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.2.tar` & `gamdl-2.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       17 2024-04-23 03:51:01.997233 gamdl-2.2/.github/FUNDING.yml
--rw-r--r--   0        0        0     1137 2024-04-23 03:51:01.997233 gamdl-2.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-23 03:51:01.997233 gamdl-2.2/.gitignore
--rw-r--r--   0        0        0    12217 2024-04-23 03:51:02.001234 gamdl-2.2/README.md
--rw-r--r--   0        0        0       20 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/__main__.py
--rw-r--r--   0        0        0     8853 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26863 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/cli.py
--rw-r--r--   0        0        0     5570 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/constants.py
--rw-r--r--   0        0        0    16173 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader.py
--rw-r--r--   0        0        0    10482 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2202 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader_post.py
--rw-r--r--   0        0        0    14146 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3922 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      797 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/models.py
--rw-r--r--   0        0        0      593 2024-04-23 03:51:02.001234 gamdl-2.2/pyproject.toml
--rw-r--r--   0        0        0       56 2024-04-23 03:51:02.001234 gamdl-2.2/requirements.txt
--rw-r--r--   0        0        0    12723 1970-01-01 00:00:00.000000 gamdl-2.2/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-24 17:07:05.501882 gamdl-2.2.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1137 2024-04-24 17:07:05.501882 gamdl-2.2.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-24 17:07:05.501882 gamdl-2.2.1/.gitignore
+-rw-r--r--   0        0        0    12217 2024-04-24 17:07:05.501882 gamdl-2.2.1/README.md
+-rw-r--r--   0        0        0       22 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/__main__.py
+-rw-r--r--   0        0        0     8853 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26863 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/cli.py
+-rw-r--r--   0        0        0     5570 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/constants.py
+-rw-r--r--   0        0        0    16173 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/downloader.py
+-rw-r--r--   0        0        0    10474 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2202 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    14146 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3882 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      797 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-24 17:07:05.501882 gamdl-2.2.1/gamdl/models.py
+-rw-r--r--   0        0        0      593 2024-04-24 17:07:05.501882 gamdl-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-04-24 17:07:05.501882 gamdl-2.2.1/requirements.txt
+-rw-r--r--   0        0        0    12725 1970-01-01 00:00:00.000000 gamdl-2.2.1/PKG-INFO
```

### Comparing `gamdl-2.2/.github/workflows/main.yml` & `gamdl-2.2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/README.md` & `gamdl-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/apple_music_api.py` & `gamdl-2.2.1/gamdl/apple_music_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/cli.py` & `gamdl-2.2.1/gamdl/cli.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/constants.py` & `gamdl-2.2.1/gamdl/constants.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/downloader.py` & `gamdl-2.2.1/gamdl/downloader.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/downloader_music_video.py` & `gamdl-2.2.1/gamdl/downloader_music_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .constants import MUSIC_VIDEO_CODEC_MAP
 from .downloader import Downloader
 from .enums import MusicVideoCodec, RemuxMode
 from .models import StreamInfo
 
 
 class DownloaderMusicVideo:
-    MP4_FORMAT_CODECS = ["hvc1", "ec-3"]
+    MP4_FORMAT_CODECS = ["hvc1", "audio-atmos", "audio-ec3"]
 
     def __init__(
         self,
         downloader: Downloader,
         codec: MusicVideoCodec = MusicVideoCodec.H264,
     ):
         self.downloader = downloader
@@ -102,14 +102,15 @@
     ) -> dict:
         choices = [
             Choice(
                 name=playlist["group_id"],
                 value=playlist,
             )
             for playlist in playlists
+            if playlist.get("uri")
         ]
         selected = inquirer.select(
             message="Select which audio codec to download:",
             choices=choices,
         ).execute()
         return selected
 
@@ -138,17 +139,15 @@
     def get_stream_info_audio(self, m3u8_master_data: dict) -> StreamInfo:
         stream_info = StreamInfo()
         if self.codec != MusicVideoCodec.ASK:
             playlist = self.get_playlist_audio(m3u8_master_data["media"])
         else:
             playlist = self.get_playlist_audio_from_user(m3u8_master_data["media"])
         stream_info.stream_url = playlist["uri"]
-        stream_info.codec = re.search(r"_([^_]+)\.m3u8", stream_info.stream_url).group(
-            1
-        )
+        stream_info.codec = playlist["group_id"]
         m3u8_data = m3u8.load(stream_info.stream_url).data
         stream_info.pssh = self.get_pssh(m3u8_data)
         return stream_info
 
     def get_music_video_id_alt(self, metadata: dict) -> str:
         return metadata["attributes"]["url"].split("/")[-1].split("?")[0]
```

### Comparing `gamdl-2.2/gamdl/downloader_post.py` & `gamdl-2.2.1/gamdl/downloader_post.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/downloader_song.py` & `gamdl-2.2.1/gamdl/downloader_song.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/downloader_song_legacy.py` & `gamdl-2.2.1/gamdl/downloader_song_legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
     def decrypt(
         self,
         encrypted_path: Path,
         decrypted_path: Path,
         decryption_key: str,
     ):
-        self.fix_key_id(encrypted_path)
         subprocess.run(
             [
                 self.downloader.mp4decrypt_path_full,
                 encrypted_path,
                 "--key",
                 f"1:{decryption_key}",
                 decrypted_path,
```

### Comparing `gamdl-2.2/gamdl/enums.py` & `gamdl-2.2.1/gamdl/enums.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/hardcoded_wvd.py` & `gamdl-2.2.1/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/gamdl/itunes_api.py` & `gamdl-2.2.1/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/pyproject.toml` & `gamdl-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gamdl-2.2/PKG-INFO` & `gamdl-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.2
+Version: 2.2.1
 Summary: A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts.
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
 Requires-Dist: inquirerpy
```

