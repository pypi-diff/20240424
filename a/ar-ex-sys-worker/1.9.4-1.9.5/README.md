# Comparing `tmp/ar_ex_sys_worker-1.9.4-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18742 bytes, number of entries: 11
+Zip file size: 18752 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    44026 b- defN 24-Apr-24 07:49 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    44225 b- defN 24-Apr-24 10:59 ar_external_sys_worker/main.py
 -rw-rw-rw-  2.0 fat    22142 b- defN 24-Feb-26 12:35 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    11290 b- defN 24-Apr-23 11:32 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      341 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      989 b- defN 24-Apr-24 08:07 ar_ex_sys_worker-1.9.4.dist-info/RECORD
-11 files, 81101 bytes uncompressed, 17036 bytes compressed:  79.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-24 11:01 ar_ex_sys_worker-1.9.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      341 b- defN 24-Apr-24 11:01 ar_ex_sys_worker-1.9.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-24 11:01 ar_ex_sys_worker-1.9.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-24 11:01 ar_ex_sys_worker-1.9.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      989 b- defN 24-Apr-24 11:01 ar_ex_sys_worker-1.9.5.dist-info/RECORD
+11 files, 81300 bytes uncompressed, 17046 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.4.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.9.5.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.4.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.9.5.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.4.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.4.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.9.4.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -837,29 +837,32 @@
             external_video_info = self.get_video_info(source["external_video"])
             vid = external_video_info[0]
             photo_obj = None
             if vid["thumb"]:
                 photo_info = self.get_photo_by_id(self.sql_shell, vid["thumb"])
                 if photo_info:
                     photo_obj = self.get_photo_data(photo_info[0]["path"])
-                    #data["photos"]["photo_in"] = photo_obj
+                    if photo_obj and not ["photos"]["photo_in"]:
+                        data["photos"]["photo_in"] = photo_obj
             data["video"].append(
                 {"id": str(vid["id"]),
                  "label": "external",
                  "thumb": photo_obj,
                  "extension": vid["extension"],
                  "name": vid["name"]})
         if source["internal_video"]:
             internal_video_info = self.get_video_info(source["internal_video"])
             vid = internal_video_info[0]
             photo_obj = None
             if vid["thumb"]:
                 photo_info = self.get_photo_by_id(self.sql_shell, vid["thumb"])
                 if photo_info:
                     photo_obj = self.get_photo_data(photo_info[0]["path"])
+                    if photo_obj and not ["photos"]["photo_in"]:
+                        data["photos"]["photo_in"] = photo_obj
             data["video"].append(
                 {"id": str(vid["id"]),
                  "label": "internal",
                  "thumb": photo_obj,
                  "extension": vid["extension"],
                  "name": vid["name"]})
         data_json = json.dumps(data)
```

## Comparing `ar_ex_sys_worker-1.9.4.dist-info/LICENSE` & `ar_ex_sys_worker-1.9.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ar_ex_sys_worker-1.9.4.dist-info/RECORD` & `ar_ex_sys_worker-1.9.5.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ar_external_sys_worker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ar_external_sys_worker/main.py,sha256=0zShCRO0QUPCdMXhPNMB8qSM5tI4-nbLnxJ0j9CgZow,44026
+ar_external_sys_worker/main.py,sha256=KOhrajROBu1VMAUuzafWa9B1NeHMm5DwJCmgcGvyn-g,44225
 ar_external_sys_worker/mixins.py,sha256=28uNbnVLwTFu0Goip9ND5jt6QhzweVv_bbOjaQxT-CQ,22142
 ar_external_sys_worker/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ar_external_sys_worker/tests/main_test.py,sha256=WuXyYh_8SJuXiGePXYaYh1ajBLmEYGZzp6AtoOd0VL8,11290
 ar_external_sys_worker/tests/mixins_test.py,sha256=NTPOm74h7bL5ra_acU3AxLgDhn75waGOGKtbkkGSxoc,1107
-ar_ex_sys_worker-1.9.4.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ar_ex_sys_worker-1.9.4.dist-info/METADATA,sha256=4M7mY5MAtEf94c0UaSpIX4itHKRoiWq678KRXWdZIys,341
-ar_ex_sys_worker-1.9.4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-ar_ex_sys_worker-1.9.4.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
-ar_ex_sys_worker-1.9.4.dist-info/RECORD,,
+ar_ex_sys_worker-1.9.5.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ar_ex_sys_worker-1.9.5.dist-info/METADATA,sha256=34BCot19HFCrQjUrMrxgx3nMPi90Tcd-FQ1iNRMAJpo,341
+ar_ex_sys_worker-1.9.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+ar_ex_sys_worker-1.9.5.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
+ar_ex_sys_worker-1.9.5.dist-info/RECORD,,
```

