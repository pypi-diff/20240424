# Comparing `tmp/zhousf-lib-1.5.2.tar.gz` & `tmp/zhousf-lib-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-1.5.2.tar", last modified: Mon Apr  1 08:27:40 2024, max compression
+gzip compressed data, was "zhousf-lib-1.5.3.tar", last modified: Wed Apr 24 03:01:08 2024, max compression
```

## Comparing `zhousf-lib-1.5.2.tar` & `zhousf-lib-1.5.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.509719 zhousf-lib-1.5.2/
--rw-rw-rw-   0        0        0     1086 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     3232 2024-04-01 08:27:40.508719 zhousf-lib-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 08:27:40.509719 zhousf-lib-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     4535 2024-04-01 08:27:36.000000 zhousf-lib-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.305940 zhousf-lib-1.5.2/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     3232 2024-04-01 08:27:40.000000 zhousf-lib-1.5.2/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3912 2024-04-01 08:27:40.000000 zhousf-lib-1.5.2/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 08:27:40.000000 zhousf-lib-1.5.2/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-01 08:27:40.000000 zhousf-lib-1.5.2/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.307964 zhousf-lib-1.5.2/zhousflib/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.308963 zhousf-lib-1.5.2/zhousflib/ann/
--rw-rw-rw-   0        0        0     6638 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ann/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.311943 zhousf-lib-1.5.2/zhousflib/ann/onnx/
--rw-rw-rw-   0        0        0     3170 2024-03-25 07:18:11.000000 zhousf-lib-1.5.2/zhousflib/ann/onnx/__init__.py
--rw-rw-rw-   0        0        0     6855 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ann/onnx/onnx_to_trt.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.314940 zhousf-lib-1.5.2/zhousflib/ann/tensorrt/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ann/tensorrt/__init__.py
--rw-rw-rw-   0        0        0     5990 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ann/tensorrt/tensorrt_infer.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.318968 zhousf-lib-1.5.2/zhousflib/ann/torch/
--rw-rw-rw-   0        0        0     1251 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ann/torch/__init__.py
--rw-rw-rw-   0        0        0     6881 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ann/torch/torch_to_onnx.py
--rw-rw-rw-   0        0        0     5934 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ann/torch/torch_to_script.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.319968 zhousf-lib-1.5.2/zhousflib/ann/transformers/
--rw-rw-rw-   0        0        0     1709 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ann/transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.324970 zhousf-lib-1.5.2/zhousflib/database/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/database/__init__.py
--rw-rw-rw-   0        0        0     2678 2024-03-18 06:19:35.000000 zhousf-lib-1.5.2/zhousflib/database/lmdb_master.py
--rw-rw-rw-   0        0        0     2841 2024-03-25 07:58:00.000000 zhousf-lib-1.5.2/zhousflib/database/tinydb_master.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.326973 zhousf-lib-1.5.2/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.328967 zhousf-lib-1.5.2/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     4897 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.338578 zhousf-lib-1.5.2/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0     1416 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8259 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5499 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6641 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     4946 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.351615 zhousf-lib-1.5.2/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0      981 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     1276 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_bbox_update.py
--rw-rw-rw-   0        0        0     3906 2024-03-25 07:25:55.000000 zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8093 2024-03-25 07:25:54.000000 zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9624 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0    10464 2024-03-25 07:25:54.000000 zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_convert_uiex.py
--rw-rw-rw-   0        0        0     3832 2024-03-25 07:25:54.000000 zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_dataset_clip.py
--rw-rw-rw-   0        0        0     1674 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/labelme/shape_convert.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.354614 zhousf-lib-1.5.2/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2958 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.359639 zhousf-lib-1.5.2/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      504 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.364643 zhousf-lib-1.5.2/zhousflib/file/
--rw-rw-rw-   0        0        0     1230 2024-01-30 02:48:23.000000 zhousf-lib-1.5.2/zhousflib/file/__init__.py
--rw-rw-rw-   0        0        0     3250 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/file/delete_file.py
--rw-rw-rw-   0        0        0     4725 2024-04-01 06:46:05.000000 zhousf-lib-1.5.2/zhousflib/file/download.py
--rw-rw-rw-   0        0        0     3227 2024-04-01 06:46:05.000000 zhousf-lib-1.5.2/zhousflib/file/zip_util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.380772 zhousf-lib-1.5.2/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      765 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.393817 zhousf-lib-1.5.2/zhousflib/image/
--rw-rw-rw-   0        0        0     1159 2024-04-01 06:55:42.000000 zhousf-lib-1.5.2/zhousflib/image/__init__.py
--rw-rw-rw-   0        0        0     5599 2024-01-30 02:48:23.000000 zhousf-lib-1.5.2/zhousflib/image/cv.py
--rw-rw-rw-   0        0        0     6818 2024-04-01 06:55:42.000000 zhousf-lib-1.5.2/zhousflib/image/cv_util.py
--rw-rw-rw-   0        0        0     8570 2024-03-25 07:25:55.000000 zhousf-lib-1.5.2/zhousflib/image/img_util.py
--rw-rw-rw-   0        0        0     5768 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/image/nms_util.py
--rw-rw-rw-   0        0        0     8569 2024-03-25 07:25:55.000000 zhousf-lib-1.5.2/zhousflib/image/op.py
--rw-rw-rw-   0        0        0     4228 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/image/pil_util.py
--rw-rw-rw-   0        0        0    10277 2024-03-07 06:30:39.000000 zhousf-lib-1.5.2/zhousflib/image/similarity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.394939 zhousf-lib-1.5.2/zhousflib/infer_framework/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.408302 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/__init__.py
--rw-rw-rw-   0        0        0      851 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend.py
--rw-rw-rw-   0        0        0     3594 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_http.py
--rw-rw-rw-   0        0        0     3685 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_onnx.py
--rw-rw-rw-   0        0        0      612 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_original.py
--rw-rw-rw-   0        0        0     3152 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_tensorrt.py
--rw-rw-rw-   0        0        0     2661 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_torch_script.py
--rw-rw-rw-   0        0        0     7080 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/fast_infer.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.411706 zhousf-lib-1.5.2/zhousflib/infer_framework/triton/
--rw-rw-rw-   0        0        0     3124 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/triton/__init__.py
--rw-rw-rw-   0        0        0    12167 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/infer_framework/triton/client_http.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.414782 zhousf-lib-1.5.2/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1525 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.418987 zhousf-lib-1.5.2/zhousflib/metrics/
--rw-rw-rw-   0        0        0       76 2024-02-29 06:32:37.000000 zhousf-lib-1.5.2/zhousflib/metrics/__init__.py
--rw-rw-rw-   0        0        0     3429 2024-03-25 07:21:21.000000 zhousf-lib-1.5.2/zhousflib/metrics/f_score.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.431761 zhousf-lib-1.5.2/zhousflib/ml/
--rw-rw-rw-   0        0        0       99 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ml/__init__.py
--rw-rw-rw-   0        0        0     4515 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ml/feature_vector.py
--rw-rw-rw-   0        0        0     8568 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ml/model_base.py
--rw-rw-rw-   0        0        0     2923 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ml/model_cluster.py
--rw-rw-rw-   0        0        0    10995 2024-01-31 01:40:34.000000 zhousf-lib-1.5.2/zhousflib/ml/model_gbdt.py
--rw-rw-rw-   0        0        0     7630 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/ml/model_lr.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.439175 zhousf-lib-1.5.2/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     4839 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     6180 2024-04-01 06:42:29.000000 zhousf-lib-1.5.2/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.445234 zhousf-lib-1.5.2/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1847 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1465 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.450234 zhousf-lib-1.5.2/zhousflib/so/
--rw-rw-rw-   0        0        0       85 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/so/__init__.py
--rw-rw-rw-   0        0        0     3840 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/so/project_to_so.py
--rw-rw-rw-   0        0        0      286 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/so/py_to_so.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.454233 zhousf-lib-1.5.2/zhousflib/text/
--rw-rw-rw-   0        0        0       87 2024-01-31 01:12:08.000000 zhousf-lib-1.5.2/zhousflib/text/__init__.py
--rw-rw-rw-   0        0        0     3141 2024-02-29 06:26:47.000000 zhousf-lib-1.5.2/zhousflib/text/similarity.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.462254 zhousf-lib-1.5.2/zhousflib/thread/
--rw-rw-rw-   0        0        0       60 2024-04-01 07:09:10.000000 zhousf-lib-1.5.2/zhousflib/thread/__init__.py
--rw-rw-rw-   0        0        0     2319 2024-03-19 06:25:39.000000 zhousf-lib-1.5.2/zhousflib/thread/thread_util.py
--rw-rw-rw-   0        0        0      829 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/thread/threadpool_util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.466235 zhousf-lib-1.5.2/zhousflib/time/
--rw-rw-rw-   0        0        0     1159 2024-03-25 07:19:09.000000 zhousf-lib-1.5.2/zhousflib/time/__init__.py
--rw-rw-rw-   0        0        0     4671 2024-03-25 07:18:11.000000 zhousf-lib-1.5.2/zhousflib/time/time_util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.496643 zhousf-lib-1.5.2/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0     2161 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/char_util.py
--rw-rw-rw-   0        0        0     2703 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/dict_util.py
--rw-rw-rw-   0        0        0     2195 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0    13480 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0     4919 2024-02-29 02:35:31.000000 zhousf-lib-1.5.2/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1481 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/math_util.py
--rw-rw-rw-   0        0        0     1358 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3526 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      527 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/random_util.py
--rw-rw-rw-   0        0        0     4692 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     5122 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/util/string_util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:27:40.506677 zhousf-lib-1.5.2/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     4246 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/web/config.py
--rw-rw-rw-   0        0        0     1200 2024-03-21 07:56:35.000000 zhousf-lib-1.5.2/zhousflib/web/fast_api.py
--rw-rw-rw-   0        0        0     3107 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     4497 2024-03-25 07:18:11.000000 zhousf-lib-1.5.2/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2024-01-23 07:44:48.000000 zhousf-lib-1.5.2/zhousflib/web/response.py
--rw-rw-rw-   0        0        0     6913 2024-04-01 08:27:11.000000 zhousf-lib-1.5.2/zhousflib/web/web.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.434537 zhousf-lib-1.5.3/
+-rw-rw-rw-   0        0        0     1086 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     3232 2024-04-24 03:01:08.433537 zhousf-lib-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2338 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:01:08.435537 zhousf-lib-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     4535 2024-04-24 02:58:49.000000 zhousf-lib-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.230592 zhousf-lib-1.5.3/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     3232 2024-04-24 03:01:08.000000 zhousf-lib-1.5.3/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3912 2024-04-24 03:01:08.000000 zhousf-lib-1.5.3/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:01:08.000000 zhousf-lib-1.5.3/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 03:01:08.000000 zhousf-lib-1.5.3/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.232149 zhousf-lib-1.5.3/zhousflib/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.234184 zhousf-lib-1.5.3/zhousflib/ann/
+-rw-rw-rw-   0        0        0     6638 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ann/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.237184 zhousf-lib-1.5.3/zhousflib/ann/onnx/
+-rw-rw-rw-   0        0        0     3170 2024-03-25 07:18:11.000000 zhousf-lib-1.5.3/zhousflib/ann/onnx/__init__.py
+-rw-rw-rw-   0        0        0     6855 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ann/onnx/onnx_to_trt.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.239177 zhousf-lib-1.5.3/zhousflib/ann/tensorrt/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ann/tensorrt/__init__.py
+-rw-rw-rw-   0        0        0     5990 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ann/tensorrt/tensorrt_infer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.243193 zhousf-lib-1.5.3/zhousflib/ann/torch/
+-rw-rw-rw-   0        0        0     1251 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ann/torch/__init__.py
+-rw-rw-rw-   0        0        0     6881 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ann/torch/torch_to_onnx.py
+-rw-rw-rw-   0        0        0     5934 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ann/torch/torch_to_script.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.245184 zhousf-lib-1.5.3/zhousflib/ann/transformers/
+-rw-rw-rw-   0        0        0     1709 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ann/transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.249814 zhousf-lib-1.5.3/zhousflib/database/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/database/__init__.py
+-rw-rw-rw-   0        0        0     2630 2024-04-24 02:58:49.000000 zhousf-lib-1.5.3/zhousflib/database/lmdb_master.py
+-rw-rw-rw-   0        0        0     2860 2024-04-24 02:55:52.000000 zhousf-lib-1.5.3/zhousflib/database/tinydb_master.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.251850 zhousf-lib-1.5.3/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.254849 zhousf-lib-1.5.3/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     4897 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.263851 zhousf-lib-1.5.3/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0     1416 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8259 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5499 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6641 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     4946 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.276820 zhousf-lib-1.5.3/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0      981 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     1276 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_bbox_update.py
+-rw-rw-rw-   0        0        0     3906 2024-03-25 07:25:55.000000 zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8093 2024-03-25 07:25:54.000000 zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9624 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0    10464 2024-03-25 07:25:54.000000 zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_convert_uiex.py
+-rw-rw-rw-   0        0        0     3832 2024-03-25 07:25:54.000000 zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_dataset_clip.py
+-rw-rw-rw-   0        0        0     1674 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/labelme/shape_convert.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.279818 zhousf-lib-1.5.3/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2958 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.284819 zhousf-lib-1.5.3/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      504 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.290850 zhousf-lib-1.5.3/zhousflib/file/
+-rw-rw-rw-   0        0        0     1230 2024-01-30 02:48:23.000000 zhousf-lib-1.5.3/zhousflib/file/__init__.py
+-rw-rw-rw-   0        0        0     3250 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/file/delete_file.py
+-rw-rw-rw-   0        0        0     4725 2024-04-01 06:46:05.000000 zhousf-lib-1.5.3/zhousflib/file/download.py
+-rw-rw-rw-   0        0        0     3227 2024-04-01 06:46:05.000000 zhousf-lib-1.5.3/zhousflib/file/zip_util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.308454 zhousf-lib-1.5.3/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      765 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.320431 zhousf-lib-1.5.3/zhousflib/image/
+-rw-rw-rw-   0        0        0     1159 2024-04-01 06:55:42.000000 zhousf-lib-1.5.3/zhousflib/image/__init__.py
+-rw-rw-rw-   0        0        0     5599 2024-01-30 02:48:23.000000 zhousf-lib-1.5.3/zhousflib/image/cv.py
+-rw-rw-rw-   0        0        0     6818 2024-04-01 06:55:42.000000 zhousf-lib-1.5.3/zhousflib/image/cv_util.py
+-rw-rw-rw-   0        0        0     8570 2024-03-25 07:25:55.000000 zhousf-lib-1.5.3/zhousflib/image/img_util.py
+-rw-rw-rw-   0        0        0     5768 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/image/nms_util.py
+-rw-rw-rw-   0        0        0     8569 2024-03-25 07:25:55.000000 zhousf-lib-1.5.3/zhousflib/image/op.py
+-rw-rw-rw-   0        0        0     4228 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/image/pil_util.py
+-rw-rw-rw-   0        0        0    10277 2024-03-07 06:30:39.000000 zhousf-lib-1.5.3/zhousflib/image/similarity.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.321431 zhousf-lib-1.5.3/zhousflib/infer_framework/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.335432 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/__init__.py
+-rw-rw-rw-   0        0        0      851 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend.py
+-rw-rw-rw-   0        0        0     3594 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_http.py
+-rw-rw-rw-   0        0        0     3685 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_onnx.py
+-rw-rw-rw-   0        0        0      612 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_original.py
+-rw-rw-rw-   0        0        0     3152 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_tensorrt.py
+-rw-rw-rw-   0        0        0     2661 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_torch_script.py
+-rw-rw-rw-   0        0        0     7080 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/fast_infer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.338431 zhousf-lib-1.5.3/zhousflib/infer_framework/triton/
+-rw-rw-rw-   0        0        0     3124 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/triton/__init__.py
+-rw-rw-rw-   0        0        0    12167 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/infer_framework/triton/client_http.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.341432 zhousf-lib-1.5.3/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1525 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.345431 zhousf-lib-1.5.3/zhousflib/metrics/
+-rw-rw-rw-   0        0        0       76 2024-02-29 06:32:37.000000 zhousf-lib-1.5.3/zhousflib/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3429 2024-03-25 07:21:21.000000 zhousf-lib-1.5.3/zhousflib/metrics/f_score.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.356007 zhousf-lib-1.5.3/zhousflib/ml/
+-rw-rw-rw-   0        0        0       99 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ml/__init__.py
+-rw-rw-rw-   0        0        0     4515 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ml/feature_vector.py
+-rw-rw-rw-   0        0        0     8568 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ml/model_base.py
+-rw-rw-rw-   0        0        0     2923 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ml/model_cluster.py
+-rw-rw-rw-   0        0        0    10995 2024-01-31 01:40:34.000000 zhousf-lib-1.5.3/zhousflib/ml/model_gbdt.py
+-rw-rw-rw-   0        0        0     7630 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/ml/model_lr.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.361007 zhousf-lib-1.5.3/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4839 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     6180 2024-04-01 06:42:29.000000 zhousf-lib-1.5.3/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.368008 zhousf-lib-1.5.3/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1847 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1465 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.373007 zhousf-lib-1.5.3/zhousflib/so/
+-rw-rw-rw-   0        0        0       85 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/so/__init__.py
+-rw-rw-rw-   0        0        0     3840 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/so/project_to_so.py
+-rw-rw-rw-   0        0        0      286 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/so/py_to_so.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.377007 zhousf-lib-1.5.3/zhousflib/text/
+-rw-rw-rw-   0        0        0       87 2024-01-31 01:12:08.000000 zhousf-lib-1.5.3/zhousflib/text/__init__.py
+-rw-rw-rw-   0        0        0     3141 2024-02-29 06:26:47.000000 zhousf-lib-1.5.3/zhousflib/text/similarity.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.382007 zhousf-lib-1.5.3/zhousflib/thread/
+-rw-rw-rw-   0        0        0       60 2024-04-01 07:09:10.000000 zhousf-lib-1.5.3/zhousflib/thread/__init__.py
+-rw-rw-rw-   0        0        0     2318 2024-04-08 01:21:36.000000 zhousf-lib-1.5.3/zhousflib/thread/thread_util.py
+-rw-rw-rw-   0        0        0      829 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/thread/threadpool_util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.386007 zhousf-lib-1.5.3/zhousflib/time/
+-rw-rw-rw-   0        0        0     1159 2024-03-25 07:19:09.000000 zhousf-lib-1.5.3/zhousflib/time/__init__.py
+-rw-rw-rw-   0        0        0     4671 2024-03-25 07:18:11.000000 zhousf-lib-1.5.3/zhousflib/time/time_util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.415538 zhousf-lib-1.5.3/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0     2161 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/char_util.py
+-rw-rw-rw-   0        0        0     2703 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/dict_util.py
+-rw-rw-rw-   0        0        0     2195 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0    13480 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0     4919 2024-02-29 02:35:31.000000 zhousf-lib-1.5.3/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1481 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/math_util.py
+-rw-rw-rw-   0        0        0     1358 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3526 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      527 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/random_util.py
+-rw-rw-rw-   0        0        0     4692 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     5122 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/util/string_util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:01:08.431537 zhousf-lib-1.5.3/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     4246 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/web/config.py
+-rw-rw-rw-   0        0        0     1200 2024-03-21 07:56:35.000000 zhousf-lib-1.5.3/zhousflib/web/fast_api.py
+-rw-rw-rw-   0        0        0     3107 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     4497 2024-03-25 07:18:11.000000 zhousf-lib-1.5.3/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2024-01-23 07:44:48.000000 zhousf-lib-1.5.3/zhousflib/web/response.py
+-rw-rw-rw-   0        0        0     6913 2024-04-01 08:27:11.000000 zhousf-lib-1.5.3/zhousflib/web/web.py
```

### Comparing `zhousf-lib-1.5.2/LICENSE` & `zhousf-lib-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/PKG-INFO` & `zhousf-lib-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 1.5.2
+Version: 1.5.3
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-1.5.2/README.md` & `zhousf-lib-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/setup.py` & `zhousf-lib-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '1.5.2'
+VERSION = '1.5.3'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-1.5.2/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-1.5.3/zhousf_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 1.5.2
+Version: 1.5.3
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-1.5.2/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-1.5.3/zhousf_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ann/__init__.py` & `zhousf-lib-1.5.3/zhousflib/ann/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ann/onnx/__init__.py` & `zhousf-lib-1.5.3/zhousflib/ann/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ann/onnx/onnx_to_trt.py` & `zhousf-lib-1.5.3/zhousflib/ann/onnx/onnx_to_trt.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ann/tensorrt/tensorrt_infer.py` & `zhousf-lib-1.5.3/zhousflib/ann/tensorrt/tensorrt_infer.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ann/torch/__init__.py` & `zhousf-lib-1.5.3/zhousflib/ann/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ann/torch/torch_to_onnx.py` & `zhousf-lib-1.5.3/zhousflib/ann/torch/torch_to_onnx.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ann/torch/torch_to_script.py` & `zhousf-lib-1.5.3/zhousflib/ann/torch/torch_to_script.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ann/transformers/__init__.py` & `zhousf-lib-1.5.3/zhousflib/ann/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/database/lmdb_master.py` & `zhousf-lib-1.5.3/zhousflib/database/lmdb_master.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Author  : zhousf
 # @Function: lmdb (Lightning Memory-Mapped Database) 快如闪电的内存映射数据库
-# pip install lmdb
+# 支持多进程
+"""
+pip install lmdb
+"""
 from pathlib import Path
 
 import pickle
 import lmdb
 
 """
 实例化数据库
@@ -40,18 +43,16 @@
         """
         插入数据
         :param key:
         :param value:
         :return:
         """
         txn = self.env.begin(write=True)
-        res = txn.get(str(key).encode())
-        if res is None:
-            txn.put(str(key).encode(), pickle.dumps(value))
-            txn.commit()
+        txn.put(str(key).encode(), pickle.dumps(value))
+        txn.commit()
 
     def delete(self, key: str):
         """
         删除
         :param key:
         :return:
         """
```

### Comparing `zhousf-lib-1.5.2/zhousflib/database/tinydb_master.py` & `zhousf-lib-1.5.3/zhousflib/database/tinydb_master.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # @Author  : zhousf
-# @Function:
+# @Function: 不支持多进程
 """
 pip install tinydb
 """
 from pathlib import Path
 from tinydb import TinyDB, Query
 from tinydb.table import Document
 from typing import (
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-1.5.3/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/coco/__init__.py` & `zhousf-lib-1.5.3/zhousflib/datasets/coco/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-1.5.3/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/labelme/__init__.py` & `zhousf-lib-1.5.3/zhousflib/datasets/labelme/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_bbox_update.py` & `zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_convert_uiex.py` & `zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_convert_uiex.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-1.5.3/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/labelme/shape_convert.py` & `zhousf-lib-1.5.3/zhousflib/datasets/labelme/shape_convert.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-1.5.3/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-1.5.3/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/file/__init__.py` & `zhousf-lib-1.5.3/zhousflib/file/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/file/delete_file.py` & `zhousf-lib-1.5.3/zhousflib/file/delete_file.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/file/download.py` & `zhousf-lib-1.5.3/zhousflib/file/download.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/file/zip_util.py` & `zhousf-lib-1.5.3/zhousflib/file/zip_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/font/SimSun.ttf` & `zhousf-lib-1.5.3/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/font/Symbola.ttf` & `zhousf-lib-1.5.3/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/font/__init__.py` & `zhousf-lib-1.5.3/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/image/__init__.py` & `zhousf-lib-1.5.3/zhousflib/image/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/image/cv.py` & `zhousf-lib-1.5.3/zhousflib/image/cv.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/image/cv_util.py` & `zhousf-lib-1.5.3/zhousflib/image/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/image/img_util.py` & `zhousf-lib-1.5.3/zhousflib/image/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/image/nms_util.py` & `zhousf-lib-1.5.3/zhousflib/image/nms_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/image/op.py` & `zhousf-lib-1.5.3/zhousflib/image/op.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/image/pil_util.py` & `zhousf-lib-1.5.3/zhousflib/image/pil_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/image/similarity.py` & `zhousf-lib-1.5.3/zhousflib/image/similarity.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_http.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_http.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_onnx.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_onnx.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_original.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_original.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_tensorrt.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_tensorrt.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/backend_torch_script.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/backend_torch_script.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/fast_infer/fast_infer.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/fast_infer/fast_infer.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/triton/__init__.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/infer_framework/triton/client_http.py` & `zhousf-lib-1.5.3/zhousflib/infer_framework/triton/client_http.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/locust/locust_demo.py` & `zhousf-lib-1.5.3/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/metrics/f_score.py` & `zhousf-lib-1.5.3/zhousflib/metrics/f_score.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ml/feature_vector.py` & `zhousf-lib-1.5.3/zhousflib/ml/feature_vector.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ml/model_base.py` & `zhousf-lib-1.5.3/zhousflib/ml/model_base.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ml/model_cluster.py` & `zhousf-lib-1.5.3/zhousflib/ml/model_cluster.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ml/model_gbdt.py` & `zhousf-lib-1.5.3/zhousflib/ml/model_gbdt.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/ml/model_lr.py` & `zhousf-lib-1.5.3/zhousflib/ml/model_lr.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-1.5.3/zhousflib/pandas/openpyxl_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/pandas/pandas_util.py` & `zhousf-lib-1.5.3/zhousflib/pandas/pandas_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/pdf/export_image.py` & `zhousf-lib-1.5.3/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-1.5.3/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/so/project_to_so.py` & `zhousf-lib-1.5.3/zhousflib/so/project_to_so.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/text/similarity.py` & `zhousf-lib-1.5.3/zhousflib/text/similarity.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/thread/thread_util.py` & `zhousf-lib-1.5.3/zhousflib/thread/thread_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,42 +46,42 @@
         print("{0}: {1}".format(thread_name, func_arg))
         counter -= 1
     return thread_name
 
 
 def test_sync():
     """
-    异步
+    同步
     """
-    thread_1 = MultiThread(name="thread_1", func=my_func, func_arg="dddd1", thread_lock=None)
-    thread_2 = MultiThread(name="thread_2", func=my_func, func_arg="32333", thread_lock=None)
+    thread_lock = threading.Lock()
+    thread_1 = MultiThread(name="thread_1", func=my_func, thread_lock=thread_lock)
+    thread_2 = MultiThread(name="thread_2", func=my_func, thread_lock=thread_lock)
     thread_1.start()
-    thread_1.join()
     thread_2.start()
-    thread_2.join()
     # 等待所有线程完成
     threads = [thread_1, thread_2]
     for t in threads:
-        print(t.get_result())
+        t.join()
     print("Exiting Main Thread")
 
 
 def test_async():
     """
-    同步
+    异步
     """
-    thread_lock = threading.Lock()
-    thread_1 = MultiThread(name="thread_1", func=my_func, thread_lock=thread_lock)
-    thread_2 = MultiThread(name="thread_2", func=my_func, thread_lock=thread_lock)
+    thread_1 = MultiThread(name="thread_1", func=my_func, func_arg="dddd1", thread_lock=None)
+    thread_2 = MultiThread(name="thread_2", func=my_func, func_arg="32333", thread_lock=None)
     thread_1.start()
     thread_2.start()
     # 等待所有线程完成
     threads = [thread_1, thread_2]
     for t in threads:
         t.join()
+    for t in threads:
+        print(t.get_result())
     print("Exiting Main Thread")
 
 
 if __name__ == "__main__":
     test_async()
     # test_sync()
     pass
```

### Comparing `zhousf-lib-1.5.2/zhousflib/thread/threadpool_util.py` & `zhousf-lib-1.5.3/zhousflib/thread/threadpool_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/time/__init__.py` & `zhousf-lib-1.5.3/zhousflib/time/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/time/time_util.py` & `zhousf-lib-1.5.3/zhousflib/time/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/calculater_util.py` & `zhousf-lib-1.5.3/zhousflib/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/char_util.py` & `zhousf-lib-1.5.3/zhousflib/util/char_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/dict_util.py` & `zhousf-lib-1.5.3/zhousflib/util/dict_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/encrypt_util.py` & `zhousf-lib-1.5.3/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/iou_util.py` & `zhousf-lib-1.5.3/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/json_util.py` & `zhousf-lib-1.5.3/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/list_util.py` & `zhousf-lib-1.5.3/zhousflib/util/list_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/math_util.py` & `zhousf-lib-1.5.3/zhousflib/util/math_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/permission_util.py` & `zhousf-lib-1.5.3/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/poly_util.py` & `zhousf-lib-1.5.3/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/random_util.py` & `zhousf-lib-1.5.3/zhousflib/util/random_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/re_util.py` & `zhousf-lib-1.5.3/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/singleton.py` & `zhousf-lib-1.5.3/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/util/string_util.py` & `zhousf-lib-1.5.3/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/web/config.py` & `zhousf-lib-1.5.3/zhousflib/web/config.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/web/fast_api.py` & `zhousf-lib-1.5.3/zhousflib/web/fast_api.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/web/log_util.py` & `zhousf-lib-1.5.3/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/web/logger.py` & `zhousf-lib-1.5.3/zhousflib/web/logger.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/web/response.py` & `zhousf-lib-1.5.3/zhousflib/web/response.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.2/zhousflib/web/web.py` & `zhousf-lib-1.5.3/zhousflib/web/web.py`

 * *Files identical despite different names*

