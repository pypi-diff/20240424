# Comparing `tmp/ar_ex_sys_worker-1.9.3-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18697 bytes, number of entries: 11
+Zip file size: 18742 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    43711 b- defN 24-Apr-23 11:53 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    44026 b- defN 24-Apr-24 07:49 ar_external_sys_worker/main.py
 -rw-rw-rw-  2.0 fat    22142 b- defN 24-Feb-26 12:35 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    11290 b- defN 24-Apr-23 11:32 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-23 11:57 ar_ex_sys_worker-1.9.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      341 b- defN 24-Apr-23 11:57 ar_ex_sys_worker-1.9.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 11:57 ar_ex_sys_worker-1.9.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-23 11:57 ar_ex_sys_worker-1.9.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      989 b- defN 24-Apr-23 11:57 ar_ex_sys_worker-1.9.3.dist-info/RECORD
-11 files, 80786 bytes uncompressed, 16991 bytes compressed:  79.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      341 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      989 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/RECORD
+11 files, 81101 bytes uncompressed, 17036 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.3.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.9.4.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.3.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.9.4.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.3.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.3.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.3.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -831,50 +831,55 @@
              "photo_out": photo_out},
         "time_in": source["time_start"].strftime("%Y-%m-%d %H:%M:%S"),
         "time_out": source["time_end"].strftime("%Y-%m-%d %H:%M:%S"),
         "video": [],
         }
         if source["external_video"]:
             external_video_info = self.get_video_info(source["external_video"])
-
-            #if external_video_info:
             vid = external_video_info[0]
             photo_obj = None
             if vid["thumb"]:
                 photo_info = self.get_photo_by_id(self.sql_shell, vid["thumb"])
                 if photo_info:
                     photo_obj = self.get_photo_data(photo_info[0]["path"])
+                    #data["photos"]["photo_in"] = photo_obj
             data["video"].append(
                 {"id": str(vid["id"]),
                  "label": "external",
                  "thumb": photo_obj,
                  "extension": vid["extension"],
                  "name": vid["name"]})
         if source["internal_video"]:
             internal_video_info = self.get_video_info(source["internal_video"])
-            #if external_video_info:
             vid = internal_video_info[0]
             photo_obj = None
-            #print("thumb", vid["thumb"])
             if vid["thumb"]:
                 photo_info = self.get_photo_by_id(self.sql_shell, vid["thumb"])
-                #print("PI", photo_info)
                 if photo_info:
                     photo_obj = self.get_photo_data(photo_info[0]["path"])
-                    #print(photo_obj)
             data["video"].append(
                 {"id": str(vid["id"]),
                  "label": "internal",
                  "thumb": photo_obj,
                  "extension": vid["extension"],
                  "name": vid["name"]})
-       # print(data)
         data_json = json.dumps(data)
         return data_json
 
+    def format_file_before_logging(self, data):
+        data = json.loads(data)
+        if data["photos"]["photo_in"]:
+            data["photos"]["photo_in"] = "bytes (deleted from log)"
+        if data["photos"]["photo_out"]:
+            data["photos"]["photo_out"] = "bytes (deleted from log)"
+        for video in data["video"]:
+            if video["thumb"]:
+                video["thumb"] = "bytes (deleted from log)"
+        return str(data).replace("'", '"')
+
 class ASURoutesWorker(mixins.AsuMixin, DataWorker):
     def __init__(self, sql_shell, asu_login, asu_password, **kwargs):
         self.sql_shell = sql_shell
         self.login = asu_login
         self.password = asu_password
         self.headers = self.get_headers()
```

## Comparing `ar_ex_sys_worker-1.9.3.dist-info/LICENSE` & `ar_ex_sys_worker-1.9.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ar_ex_sys_worker-1.9.3.dist-info/RECORD` & `ar_ex_sys_worker-1.9.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ar_external_sys_worker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ar_external_sys_worker/main.py,sha256=sQD6tNa5AuWOZ13qNri0yNdnik385SRDNl0vHQz_UOU,43711
+ar_external_sys_worker/main.py,sha256=0zShCRO0QUPCdMXhPNMB8qSM5tI4-nbLnxJ0j9CgZow,44026
 ar_external_sys_worker/mixins.py,sha256=28uNbnVLwTFu0Goip9ND5jt6QhzweVv_bbOjaQxT-CQ,22142
 ar_external_sys_worker/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ar_external_sys_worker/tests/main_test.py,sha256=WuXyYh_8SJuXiGePXYaYh1ajBLmEYGZzp6AtoOd0VL8,11290
 ar_external_sys_worker/tests/mixins_test.py,sha256=NTPOm74h7bL5ra_acU3AxLgDhn75waGOGKtbkkGSxoc,1107
-ar_ex_sys_worker-1.9.3.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ar_ex_sys_worker-1.9.3.dist-info/METADATA,sha256=oUn4vFxQNtrDBoZwsXxollW1YlFwyom2_h4PB1qRXTQ,341
-ar_ex_sys_worker-1.9.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-ar_ex_sys_worker-1.9.3.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
-ar_ex_sys_worker-1.9.3.dist-info/RECORD,,
+ar_ex_sys_worker-1.9.4.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ar_ex_sys_worker-1.9.4.dist-info/METADATA,sha256=4M7mY5MAtEf94c0UaSpIX4itHKRoiWq678KRXWdZIys,341
+ar_ex_sys_worker-1.9.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+ar_ex_sys_worker-1.9.4.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
+ar_ex_sys_worker-1.9.4.dist-info/RECORD,,
```

