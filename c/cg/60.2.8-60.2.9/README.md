# Comparing `tmp/cg-60.2.8-py3-none-any.whl.zip` & `tmp/cg-60.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1341,12 +1341,12 @@
 -rw-r--r--  2.0 unx     2920 b- defN 80-Jan-01 00:00 tests/utils/test_commands.py
 -rw-r--r--  2.0 unx      953 b- defN 80-Jan-01 00:00 tests/utils/test_date.py
 -rw-r--r--  2.0 unx     1508 b- defN 80-Jan-01 00:00 tests/utils/test_dict.py
 -rw-r--r--  2.0 unx     7154 b- defN 80-Jan-01 00:00 tests/utils/test_dispatcher.py
 -rw-r--r--  2.0 unx     4100 b- defN 80-Jan-01 00:00 tests/utils/test_files.py
 -rw-r--r--  2.0 unx     1170 b- defN 80-Jan-01 00:00 tests/utils/test_time.py
 -rw-r--r--  2.0 unx     2366 b- defN 80-Jan-01 00:00 tests/utils/test_utils.py
--rw-r--r--  2.0 unx     4369 b- defN 80-Jan-01 00:00 cg-60.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cg-60.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 cg-60.2.8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx   143819 b- defN 16-Jan-01 00:00 cg-60.2.8.dist-info/RECORD
+-rw-r--r--  2.0 unx     4369 b- defN 80-Jan-01 00:00 cg-60.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cg-60.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 cg-60.2.9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx   143819 b- defN 16-Jan-01 00:00 cg-60.2.9.dist-info/RECORD
 1350 files, 9467394 bytes uncompressed, 3155548 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -4032,20 +4032,20 @@
 
 Filename: tests/utils/test_time.py
 Comment: 
 
 Filename: tests/utils/test_utils.py
 Comment: 
 
-Filename: cg-60.2.8.dist-info/METADATA
+Filename: cg-60.2.9.dist-info/METADATA
 Comment: 
 
-Filename: cg-60.2.8.dist-info/WHEEL
+Filename: cg-60.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: cg-60.2.8.dist-info/entry_points.txt
+Filename: cg-60.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: cg-60.2.8.dist-info/RECORD
+Filename: cg-60.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cg/__init__.py

```diff
@@ -1,2 +1,2 @@
 __title__ = "cg"
-__version__ = "60.2.8"
+__version__ = "60.2.9"
```

## cg/constants/archiving.py

```diff
@@ -1,10 +1,10 @@
 from enum import StrEnum
 
-DEFAULT_SPRING_ARCHIVE_COUNT = 200
+DEFAULT_SPRING_ARCHIVE_COUNT = 100
 
 
 class ArchiveLocations(StrEnum):
     """Archive locations for the different customers' Spring files."""
 
     KAROLINSKA_BUCKET: str = "karolinska_bucket"
```

## Comparing `cg-60.2.8.dist-info/METADATA` & `cg-60.2.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 60.2.8
+Version: 60.2.9
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `cg-60.2.8.dist-info/RECORD` & `cg-60.2.9.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 README.md,sha256=0uxO6Rbd31UOHgU5U0z3DRRIS5K7gbyEVR8ixxSQC7g,2686
-cg/__init__.py,sha256=nXIl5wp_-9GjpMZo-OYk8WhlIpxkGc_HrlmELw19tXo,40
+cg/__init__.py,sha256=LBZoeJa9qu4lk2iKmyMNZfhFoYa2e5IhK3K11JYYEBk,40
 cg/apps/__init__.py,sha256=pYf0vxo4iYQqURzFRYzqpOCdV8Cm9MWx0GHvJOz0EMg,315
 cg/apps/coverage/__init__.py,sha256=dJtsmNf8tODE2-VEomMIoYA7ugLYZAk_upsfOQCZeF8,27
 cg/apps/coverage/api.py,sha256=e_ozC3QeNKoEfpjjMaL-XjeBLtz-JySWccrtw0E9mLM,2940
 cg/apps/crunchy/__init__.py,sha256=wqpS8FrCNUnMTeaVxhw0Plq7gv0DGTVojGIyJlEUPeU,56
 cg/apps/crunchy/crunchy.py,sha256=3HN-zKE1Io4xcM8scb1RV1F6JH6Q0FYWn1CwOiHUvXI,12783
 cg/apps/crunchy/files.py,sha256=ojRzyEE2EhNg0TMfxduvZU6gL9fasef8m61J0GegMUo,4502
 cg/apps/crunchy/models.py,sha256=MOSMFmZ3u1ShUAIy2t229VUsE-5RCo1Z3ZBCZWIdAgM,430
@@ -174,15 +174,15 @@
 cg/clients/arnold/exceptions.py,sha256=w9J9TLie5tcgqzaO0L3lrF3OlowtjzkeGR4R7quXzko,384
 cg/clients/janus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cg/clients/janus/api.py,sha256=v6kcmG93rYyU-CUVOhngcHvjgIFvQardxxUURBztr6w,1246
 cg/clients/janus/dto/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cg/clients/janus/dto/create_qc_metrics_request.py,sha256=5eb_EwjGtI5nB8vmXTDcYul2bUjc_iSn4CKIS8T9Trs,503
 cg/clients/janus/exceptions.py,sha256=WQQNefE5azCLRXpU2xw6S2cylGd73eaFUHqrDRkjN-A,420
 cg/constants/__init__.py,sha256=IIb1rsu93s1-s6PwR-mIaiSCy4T6YnazFc7HcV6qMBo,937
-cg/constants/archiving.py,sha256=LzxfDdJ0spg67veMQetZ0y3d-K55YxJBFfl3boACU3k,253
+cg/constants/archiving.py,sha256=osJHg_JlIvOSswP7n45NXOESBO9PVXitcDz1MsP9OVY,253
 cg/constants/backup.py,sha256=uN1KtX1sbkajBFNt7PBqUn1MEhpi6A03iWxjYfC5SFw,35
 cg/constants/bcl_convert_metrics.py,sha256=fwiBuPaCrJfyQyP6Zjqo5Nxm_Kl5Wl-M2WjEkX8g8Gw,769
 cg/constants/compression.py,sha256=hY8Ws7r0uFhDD10GDYjTN1nFeKWnekRGlOpM14g-yZ4,469
 cg/constants/constants.py,sha256=aVckay_dzf0Z7L5OYEJkTxIs-I9dakZ8QwIaPrfVg_s,6570
 cg/constants/delivery.py,sha256=gw36ANDanevg2-rHxw7zAng9NJNmouTkWMhHwBYPeWY,6033
 cg/constants/demultiplexing.py,sha256=Ci_OI9crJqthOZh0gEBvpIl8bun0k3szJHia5nurP-E,8916
 cg/constants/encryption.py,sha256=1YzIsYHl144-yuZvr9VD_i3CrQLOXIb9qpySWzRMo8E,1422
@@ -1340,11 +1340,11 @@
 tests/utils/test_commands.py,sha256=pMg3T6cbpfcAwnhdD_arLpBdrKdCZ4rYoE77Eo0zjXM,2920
 tests/utils/test_date.py,sha256=M3YZA8w7MAIzWKiPnvDqmBnjfDZLwipWhGuXDjbdycI,953
 tests/utils/test_dict.py,sha256=7rEQT_dxBBZdP4mNXs9ajrUlayUTHN4G8f_W4ykKHWY,1508
 tests/utils/test_dispatcher.py,sha256=ZiFROV7PfQcLCbFDXztoqyDUGrdW6H6aIh6JDwl_6lQ,7154
 tests/utils/test_files.py,sha256=XOXV9ZJlCSBN6XSLGyJtVbgix8GmK6ddiVsGosyETgM,4100
 tests/utils/test_time.py,sha256=jHimmt6I7O-2CrYi7WHq-YY91ywEad1yjbKN3d4HP5w,1170
 tests/utils/test_utils.py,sha256=QbEJxl0zynOVgQ82qudzMG6YLoFdIDXNtiYtIz-KN8U,2366
-cg-60.2.8.dist-info/METADATA,sha256=XdD-B2XHk2TA2B8OKuLK5Jd-7-HerVUJ-Ka9qALmsmU,4369
-cg-60.2.8.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-cg-60.2.8.dist-info/entry_points.txt,sha256=q5f47YQQGltzK_xnIq1mDopRXXEItr85Xe1BCtG-Wts,39
-cg-60.2.8.dist-info/RECORD,,
+cg-60.2.9.dist-info/METADATA,sha256=2-v0S7fmnBPyqPMsxSYauGWB3u6qB11Wdxpiozf_cYg,4369
+cg-60.2.9.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+cg-60.2.9.dist-info/entry_points.txt,sha256=q5f47YQQGltzK_xnIq1mDopRXXEItr85Xe1BCtG-Wts,39
+cg-60.2.9.dist-info/RECORD,,
```

