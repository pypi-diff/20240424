# Comparing `tmp/onnxsharp-0.0.3-py2.py3-none-any.whl.zip` & `tmp/onnxsharp-0.0.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,28 @@
-Zip file size: 31464 bytes, number of entries: 24
+Zip file size: 32209 bytes, number of entries: 26
 -rw-rw-rw-  2.0 fat      713 b- defN 23-Mar-09 10:06 onnxsharp/__init__.py
 -rw-rw-rw-  2.0 fat     1318 b- defN 23-Mar-09 09:40 onnxsharp/basics.py
+-rw-rw-rw-  2.0 fat      674 b- defN 24-Apr-23 13:05 onnxsharp/command_line.py
 -rw-rw-rw-  2.0 fat    23928 b- defN 24-Mar-05 08:15 onnxsharp/graph.py
 -rw-rw-rw-  2.0 fat    27581 b- defN 23-Mar-09 10:06 onnxsharp/graph_utils.py
 -rw-rw-rw-  2.0 fat     4216 b- defN 24-Jan-11 09:08 onnxsharp/model.py
 -rw-rw-rw-  2.0 fat     8982 b- defN 24-Jan-12 01:33 onnxsharp/node.py
 -rw-rw-rw-  2.0 fat     1445 b- defN 23-Mar-09 07:19 onnxsharp/npy_utils.py
 -rw-rw-rw-  2.0 fat     1081 b- defN 22-Nov-17 11:36 onnxsharp/ort_utils.py
 -rw-rw-rw-  2.0 fat     8659 b- defN 22-Nov-09 05:54 onnxsharp/tensor.py
 -rw-rw-rw-  2.0 fat     2443 b- defN 23-Aug-25 02:11 onnxsharp/topy_sample.py
 -rw-rw-rw-  2.0 fat     3818 b- defN 23-Mar-09 07:19 onnxsharp/torch_utils.py
--rw-rw-rw-  2.0 fat      706 b- defN 24-Apr-23 12:55 onnxsharp-0.0.3.data/scripts/onnx_summarize
--rw-rw-rw-  2.0 fat      462 b- defN 22-Nov-02 12:35 onnxsharp-0.0.3.data/scripts/ort_get_peak_details
--rw-rw-rw-  2.0 fat     5491 b- defN 23-Mar-09 10:06 onnxsharp-0.0.3.data/scripts/ort_get_peak_op_summary
--rw-rw-rw-  2.0 fat      237 b- defN 22-Nov-02 12:35 onnxsharp-0.0.3.data/scripts/ort_get_peak_step
--rw-rw-rw-  2.0 fat      269 b- defN 22-Nov-02 12:35 onnxsharp-0.0.3.data/scripts/ort_get_peak_summary
--rw-rw-rw-  2.0 fat     1911 b- defN 22-Nov-17 11:36 onnxsharp-0.0.3.data/scripts/ort_parse_output_name
--rw-rw-rw-  2.0 fat     2436 b- defN 22-Nov-02 12:35 onnxsharp-0.0.3.data/scripts/ort_parse_peak_summary
--rw-rw-rw-  2.0 fat      256 b- defN 22-Nov-17 11:36 onnxsharp-0.0.3.data/scripts/ort_scan_output_in_order
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-23 12:58 onnxsharp-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1118 b- defN 24-Apr-23 12:58 onnxsharp-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-23 12:58 onnxsharp-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-23 12:58 onnxsharp-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2098 b- defN 24-Apr-23 12:58 onnxsharp-0.0.3.dist-info/RECORD
-24 files, 110846 bytes uncompressed, 28038 bytes compressed:  74.7%
+-rw-rw-rw-  2.0 fat      706 b- defN 24-Apr-23 12:55 onnxsharp-0.0.4.data/scripts/onnx_summarize
+-rw-rw-rw-  2.0 fat      462 b- defN 22-Nov-02 12:35 onnxsharp-0.0.4.data/scripts/ort_get_peak_details
+-rw-rw-rw-  2.0 fat     5491 b- defN 23-Mar-09 10:06 onnxsharp-0.0.4.data/scripts/ort_get_peak_op_summary
+-rw-rw-rw-  2.0 fat      237 b- defN 22-Nov-02 12:35 onnxsharp-0.0.4.data/scripts/ort_get_peak_step
+-rw-rw-rw-  2.0 fat      269 b- defN 22-Nov-02 12:35 onnxsharp-0.0.4.data/scripts/ort_get_peak_summary
+-rw-rw-rw-  2.0 fat     1911 b- defN 22-Nov-17 11:36 onnxsharp-0.0.4.data/scripts/ort_parse_output_name
+-rw-rw-rw-  2.0 fat     2436 b- defN 22-Nov-02 12:35 onnxsharp-0.0.4.data/scripts/ort_parse_peak_summary
+-rw-rw-rw-  2.0 fat      256 b- defN 22-Nov-17 11:36 onnxsharp-0.0.4.data/scripts/ort_scan_output_in_order
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-23 13:07 onnxsharp-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1118 b- defN 24-Apr-23 13:07 onnxsharp-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 24-Apr-23 13:07 onnxsharp-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       78 b- defN 24-Apr-23 13:07 onnxsharp-0.0.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-23 13:07 onnxsharp-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2276 b- defN 24-Apr-23 13:07 onnxsharp-0.0.4.dist-info/RECORD
+26 files, 111776 bytes uncompressed, 28497 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: onnxsharp/__init__.py
 Comment: 
 
 Filename: onnxsharp/basics.py
 Comment: 
 
+Filename: onnxsharp/command_line.py
+Comment: 
+
 Filename: onnxsharp/graph.py
 Comment: 
 
 Filename: onnxsharp/graph_utils.py
 Comment: 
 
 Filename: onnxsharp/model.py
@@ -27,47 +30,50 @@
 
 Filename: onnxsharp/topy_sample.py
 Comment: 
 
 Filename: onnxsharp/torch_utils.py
 Comment: 
 
-Filename: onnxsharp-0.0.3.data/scripts/onnx_summarize
+Filename: onnxsharp-0.0.4.data/scripts/onnx_summarize
+Comment: 
+
+Filename: onnxsharp-0.0.4.data/scripts/ort_get_peak_details
 Comment: 
 
-Filename: onnxsharp-0.0.3.data/scripts/ort_get_peak_details
+Filename: onnxsharp-0.0.4.data/scripts/ort_get_peak_op_summary
 Comment: 
 
-Filename: onnxsharp-0.0.3.data/scripts/ort_get_peak_op_summary
+Filename: onnxsharp-0.0.4.data/scripts/ort_get_peak_step
 Comment: 
 
-Filename: onnxsharp-0.0.3.data/scripts/ort_get_peak_step
+Filename: onnxsharp-0.0.4.data/scripts/ort_get_peak_summary
 Comment: 
 
-Filename: onnxsharp-0.0.3.data/scripts/ort_get_peak_summary
+Filename: onnxsharp-0.0.4.data/scripts/ort_parse_output_name
 Comment: 
 
-Filename: onnxsharp-0.0.3.data/scripts/ort_parse_output_name
+Filename: onnxsharp-0.0.4.data/scripts/ort_parse_peak_summary
 Comment: 
 
-Filename: onnxsharp-0.0.3.data/scripts/ort_parse_peak_summary
+Filename: onnxsharp-0.0.4.data/scripts/ort_scan_output_in_order
 Comment: 
 
-Filename: onnxsharp-0.0.3.data/scripts/ort_scan_output_in_order
+Filename: onnxsharp-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: onnxsharp-0.0.3.dist-info/LICENSE
+Filename: onnxsharp-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: onnxsharp-0.0.3.dist-info/METADATA
+Filename: onnxsharp-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: onnxsharp-0.0.3.dist-info/WHEEL
+Filename: onnxsharp-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: onnxsharp-0.0.3.dist-info/top_level.txt
+Filename: onnxsharp-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: onnxsharp-0.0.3.dist-info/RECORD
+Filename: onnxsharp-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `onnxsharp-0.0.3.data/scripts/onnx_summarize` & `onnxsharp-0.0.4.data/scripts/onnx_summarize`

 * *Files identical despite different names*

## Comparing `onnxsharp-0.0.3.data/scripts/ort_get_peak_op_summary` & `onnxsharp-0.0.4.data/scripts/ort_get_peak_op_summary`

 * *Files identical despite different names*

## Comparing `onnxsharp-0.0.3.data/scripts/ort_parse_output_name` & `onnxsharp-0.0.4.data/scripts/ort_parse_output_name`

 * *Files identical despite different names*

## Comparing `onnxsharp-0.0.3.data/scripts/ort_parse_peak_summary` & `onnxsharp-0.0.4.data/scripts/ort_parse_peak_summary`

 * *Files identical despite different names*

## Comparing `onnxsharp-0.0.3.dist-info/LICENSE` & `onnxsharp-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `onnxsharp-0.0.3.dist-info/METADATA` & `onnxsharp-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxsharp
-Version: 0.0.3
+Version: 0.0.4
 Summary: ONNX Sharp
 Home-page: https://github.com/xuyus/onnx-sharp
 Author: xuyus
 Author-email: 
 License: Apache License v2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `onnxsharp-0.0.3.dist-info/RECORD` & `onnxsharp-0.0.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 onnxsharp/__init__.py,sha256=qXa9Xo_6owPeUAcnGNCsCeFhDNnhwUkTo0IluHJsKZA,713
 onnxsharp/basics.py,sha256=0ZpIZcNNbKqHiUImn3FYz3vE1AhOuYekFjv5F_E26Ys,1318
+onnxsharp/command_line.py,sha256=F7aX8EXEPRXIl2lSLr8J1pTnHNu6JXitf_RHq-jdxxY,674
 onnxsharp/graph.py,sha256=re7QTksEHL4QECBz8tB_z2Iau5-GnhhmuP31Gav4ono,23928
 onnxsharp/graph_utils.py,sha256=XC6UTf-a0YmLQTbws0aQkHgnZ_RfxUU2KwOB6gdzwko,27581
 onnxsharp/model.py,sha256=X1e24TCQenQKaE9aujVzowmEGjRW3wVk2dQZN23qjeA,4216
 onnxsharp/node.py,sha256=jppDDdx-AKeuDRyZGITGAcnUG-NPSPJb9whFVEzKQ_0,8982
 onnxsharp/npy_utils.py,sha256=BgmhzxmEtOf5fL9X8E3FfuwHQnuIl-ch_TzgtCWklPw,1445
 onnxsharp/ort_utils.py,sha256=aKyA5aPxa_ySlxXBrJpCdCrpjoiJMnbaArIZCJpbgB0,1081
 onnxsharp/tensor.py,sha256=iHKIObe0DEY9WNGCMVlSKKbs2jeXZv7AHrs_OUMjrR0,8659
 onnxsharp/topy_sample.py,sha256=hLtdudbzg0DPL24EglPQ_leNv21s8I-dAKmx3tg3UpU,2443
 onnxsharp/torch_utils.py,sha256=VI8tSAw-gIGh_Zn0BthdBpS5g-uI145hrL1ZpxSbeNU,3818
-onnxsharp-0.0.3.data/scripts/onnx_summarize,sha256=1iVJr6BD3wDB132g8VmHjm-NfhWGSh-UlONbeEjrrN8,706
-onnxsharp-0.0.3.data/scripts/ort_get_peak_details,sha256=dyu4V87LWycofXjrVJhYBDgS5KrDFMlZZxHfsidSzsk,462
-onnxsharp-0.0.3.data/scripts/ort_get_peak_op_summary,sha256=BWR9hKaE93cp8lJXZMo2BEHEeMBhUzPYS3DDv_CGpjM,5491
-onnxsharp-0.0.3.data/scripts/ort_get_peak_step,sha256=pjB_RgbFpxaoV6UP2ZyenkoJgKaEULOEedhouHrEcVM,237
-onnxsharp-0.0.3.data/scripts/ort_get_peak_summary,sha256=-jFR5STrbW2owiyXlMfWr63KC71GPHETAM5uaOlju5c,269
-onnxsharp-0.0.3.data/scripts/ort_parse_output_name,sha256=Aw5iWm3nenykAhw2koKrNCb5xupIfOSykEw7d76nCz0,1911
-onnxsharp-0.0.3.data/scripts/ort_parse_peak_summary,sha256=U9xmziK-LBqK7ScLpbkOLlVWnEv0LgRG_qpN5w4qVKE,2436
-onnxsharp-0.0.3.data/scripts/ort_scan_output_in_order,sha256=2t1UGvjatbDVXDMwI1TNwAsVPAlIoJ7QbTf4wCr2HjQ,256
-onnxsharp-0.0.3.dist-info/LICENSE,sha256=SbvpEU5JIU3yzMMkyzrI0dGqHDoJR_lMKGdl6GZHsy4,11558
-onnxsharp-0.0.3.dist-info/METADATA,sha256=TaeISOw_2diAo-SHhxDWS47fXMd-mSo_CSCLvQl2GW8,1118
-onnxsharp-0.0.3.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
-onnxsharp-0.0.3.dist-info/top_level.txt,sha256=hbt5uElu_gcJ_NZYK75bQjYKmLaN0otbjrU1-oByi2s,10
-onnxsharp-0.0.3.dist-info/RECORD,,
+onnxsharp-0.0.4.data/scripts/onnx_summarize,sha256=1iVJr6BD3wDB132g8VmHjm-NfhWGSh-UlONbeEjrrN8,706
+onnxsharp-0.0.4.data/scripts/ort_get_peak_details,sha256=dyu4V87LWycofXjrVJhYBDgS5KrDFMlZZxHfsidSzsk,462
+onnxsharp-0.0.4.data/scripts/ort_get_peak_op_summary,sha256=BWR9hKaE93cp8lJXZMo2BEHEeMBhUzPYS3DDv_CGpjM,5491
+onnxsharp-0.0.4.data/scripts/ort_get_peak_step,sha256=pjB_RgbFpxaoV6UP2ZyenkoJgKaEULOEedhouHrEcVM,237
+onnxsharp-0.0.4.data/scripts/ort_get_peak_summary,sha256=-jFR5STrbW2owiyXlMfWr63KC71GPHETAM5uaOlju5c,269
+onnxsharp-0.0.4.data/scripts/ort_parse_output_name,sha256=Aw5iWm3nenykAhw2koKrNCb5xupIfOSykEw7d76nCz0,1911
+onnxsharp-0.0.4.data/scripts/ort_parse_peak_summary,sha256=U9xmziK-LBqK7ScLpbkOLlVWnEv0LgRG_qpN5w4qVKE,2436
+onnxsharp-0.0.4.data/scripts/ort_scan_output_in_order,sha256=2t1UGvjatbDVXDMwI1TNwAsVPAlIoJ7QbTf4wCr2HjQ,256
+onnxsharp-0.0.4.dist-info/LICENSE,sha256=SbvpEU5JIU3yzMMkyzrI0dGqHDoJR_lMKGdl6GZHsy4,11558
+onnxsharp-0.0.4.dist-info/METADATA,sha256=RwXrlJl9AfkooN9iHnKPVjjq3bNd8Go3mv6H-Pkcdcc,1118
+onnxsharp-0.0.4.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
+onnxsharp-0.0.4.dist-info/entry_points.txt,sha256=2XUKouszOvDzCvbAmJKqR84Zg7eNK42q2OmQXVp4fLM,78
+onnxsharp-0.0.4.dist-info/top_level.txt,sha256=hbt5uElu_gcJ_NZYK75bQjYKmLaN0otbjrU1-oByi2s,10
+onnxsharp-0.0.4.dist-info/RECORD,,
```

