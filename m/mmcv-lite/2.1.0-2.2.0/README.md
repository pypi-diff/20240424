# Comparing `tmp/mmcv-lite-2.1.0.tar.gz` & `tmp/mmcv-lite-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmcv-lite-2.1.0.tar", last modified: Tue Oct 17 11:30:38 2023, max compression
+gzip compressed data, was "dist/mmcv-lite-2.2.0.tar", last modified: Wed Apr 24 14:24:21 2024, max compression
```

## Comparing `mmcv-lite-2.1.0.tar` & `mmcv-lite-2.2.0.tar`

### file list

```diff
@@ -1,570 +1,580 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/LICENSES.md
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (127)    16063 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (127)    37139 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/cnn/rfsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/rfsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/rfsearch/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/rfsearch/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/rfsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23248 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    28189 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6724 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/active_rotated_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/bezier_align.py
--rw-r--r--   0 runner    (1001) docker     (127)    14058 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/bias_act.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/box_iou_quadri.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/chamfer_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/conv2d_gradfix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/convex_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/
--rw-r--r--   0 runner    (1001) docker     (127)    12955 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    12524 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23369 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    15470 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    12932 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    33575 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/spconv/
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/spconv/indice.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    11437 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/mlu/
--rw-r--r--   0 runner    (1001) docker     (127)    10647 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSDevice.h
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSLibrary.h
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSLibrary.mm
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSStream.h
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/parrots_cpp_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/parrots_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_device_registry.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_npu_helper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/prettyprint.h
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h
--rw-r--r--   0 runner    (1001) docker     (127)    14014 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_launch.h
--rw-r--r--   0 runner    (1001) docker     (127)    37649 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ball_query._parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ball_query.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ball_query_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/border_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/border_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/border_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_naive.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      750 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/contour_expand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/contour_expand_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/convex_iou.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/convex_iou_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/correlation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/correlation_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/correlation_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)    84444 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/cudabind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    21266 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_conv_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/focal_loss.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/focal_loss_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/gather_points.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/gather_points_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/gather_points_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/group_points.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/group_points_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/group_points_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/info.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/iou3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/iou3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/iou3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/knn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/knn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/knn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/min_area_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/min_area_polygons_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)    10725 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ms_deform_attn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/nms_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/nms_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/nms_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/pixel_group_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/prroi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/psamask_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/psamask_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      619 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/sync_bn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/sync_bn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_interpolate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_nn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_nn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_nn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/tin_shift.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/tin_shift_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/upfirdn2d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/voxelization.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/voxelization_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/voxelization_pytorch.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/assign_score_withk.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/ball_query.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/bezier_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/bias_act.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/border_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/carafe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/carafe_naive.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/chamfer_distance.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     3290 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/contour_expand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/convex_iou.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/correlation.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17454 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18378 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20255 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18587 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17468 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9196 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)    99744 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)    83984 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)    18325 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu
--rw-r--r--   0 runner    (1001) docker     (127)    19211 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu
--rw-r--r--   0 runner    (1001) docker     (127)    22064 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)    30436 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)    11432 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)    21266 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/focal_loss.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/gather_points.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/group_points.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/info.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/iou3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/knn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/masked_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/min_area_polygons.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/diff_iou_rotated_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    10375 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11780 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/scatter_points_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20040 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18472 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mps/
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/nms_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/nms_rotated.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/box_iou_rotated_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/group_points_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/points_in_polygons_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/points_in_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/prroi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    55203 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/pybind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/scatter_points.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/spconv_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/spconv_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/sync_bn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/three_interpolate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/three_nn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/tin_shift.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/upfirdn2d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/voxelization.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20328 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/diff_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)    17614 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/filtered_lrelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10686 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8143 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/min_area_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)    17158 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (127)    19306 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/points_in_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/prroi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/riroi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8324 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/rotated_feature_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    14049 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/sparse_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/sparse_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/sparse_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/sparse_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/sparse_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/sparse_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/three_nn.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2426 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)    17765 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/transforms/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/transforms/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)    57971 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/transforms/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24709 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/transforms/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/utils/device_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21786 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/mmcv_lite.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    21203 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:38.000000 mmcv-lite-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/tests/test_arraymisc.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-10-17 11:30:35.000000 mmcv-lite-2.1.0/tests/test_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/LICENSES.md
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37139 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/cnn/rfsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/rfsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/rfsearch/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/rfsearch/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/rfsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23248 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6724 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/active_rotated_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/bezier_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/bias_act.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/box_iou_quadri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/chamfer_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/conv2d_gradfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/convex_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/correlation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    12955 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23369 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    33575 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/spconv/
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/spconv/indice.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/mlu/
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSDevice.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSLibrary.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSLibrary.mm
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSStream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/parrots_cpp_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/parrots_cuda_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_cuda_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_device_registry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_npu_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_npu_util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/prettyprint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/tensorview/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_launch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37649 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/active_rotated_filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/active_rotated_filter_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/assign_score_withk.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ball_query._parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ball_query.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ball_query_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/bbox_overlaps.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/bbox_overlaps_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/border_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/border_align_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/border_align_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/box_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_naive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/chamfer_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/contour_expand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/contour_expand_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/convex_iou.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/convex_iou_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/correlation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/correlation_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/correlation_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    84444 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/cudabind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21266 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_conv_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/diff_iou_rotated_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/focal_loss.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/focal_loss_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/furthest_point_sample.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/gather_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/gather_points_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/gather_points_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/group_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/group_points_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/group_points_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/info.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/iou3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/iou3d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/iou3d_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/knn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/knn_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/knn_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/masked_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/min_area_polygons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/min_area_polygons_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ms_deform_attn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/nms.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/nms_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/nms_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/nms_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/pixel_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/pixel_group_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_boxes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_polygons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_polygons_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/prroi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/psamask.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/psamask_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/psamask_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_pool_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roipoint_pool3d_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/rotated_feature_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/sync_bn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/sync_bn_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_interpolate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_nn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_nn_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_nn_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/tin_shift.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/tin_shift_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/upfirdn2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/voxelization.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/voxelization_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/voxelization_pytorch.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/assign_score_withk.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/ball_query.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/bezier_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/bias_act.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/border_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/carafe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/carafe_naive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/chamfer_distance.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3290 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/contour_expand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/convex_iou.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/correlation.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18378 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20255 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/nms.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/psamask.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18587 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    99744 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    83984 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    18325 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    19211 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    22064 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    30436 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    11432 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    21266 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/focal_loss.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/gather_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/group_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/info.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/iou3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/knn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/masked_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/min_area_polygons.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/diff_iou_rotated_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10375 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11780 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/scatter_points_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20040 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mps/
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/nms.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/nms_quadri.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/nms_rotated.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/ball_query_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/box_iou_rotated_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/chamfer_distance_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/common_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/group_points_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/ms_deform_attn_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/points_in_polygons_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/roi_align_rotated_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/rotated_feature_align_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/stack_ball_query_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/stack_group_points_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/three_interpolate_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/pixel_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/points_in_boxes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/points_in_polygons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/prroi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/psamask.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    55203 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/pybind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roi_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/scatter_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/spconv_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/spconv_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/sync_bn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/three_interpolate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/three_nn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/tin_shift.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/upfirdn2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/voxelization.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/diff_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/filtered_lrelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8143 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/min_area_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17187 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16856 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19306 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/points_in_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/prroi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/riroi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/rotated_feature_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/sparse_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/sparse_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/sparse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/sparse_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/sparse_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/sparse_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/three_nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2426 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17765 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/transforms/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/transforms/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57971 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/transforms/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24709 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/transforms/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/utils/device_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22277 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv_lite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/mmcv_lite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    21722 2024-04-24 14:24:20.000000 mmcv-lite-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:24:21.000000 mmcv-lite-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/tests/test_arraymisc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 14:24:14.000000 mmcv-lite-2.2.0/tests/test_visualization.py
```

### Comparing `mmcv-lite-2.1.0/LICENSE` & `mmcv-lite-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/LICENSES.md` & `mmcv-lite-2.2.0/LICENSES.md`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/PKG-INFO` & `mmcv-lite-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcv-lite
-Version: 2.1.0
+Version: 2.2.0
 Summary: OpenMMLab Computer Vision Foundation
 Home-page: https://github.com/open-mmlab/mmcv
 Author: MMCV Contributors
 Author-email: openmmlab@gmail.com
 Keywords: computer vision
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mmcv-lite-2.1.0/README.md` & `mmcv-lite-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/arraymisc/quantization.py` & `mmcv-lite-2.2.0/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/__init__.py` & `mmcv-lite-2.2.0/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/alexnet.py` & `mmcv-lite-2.2.0/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/__init__.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/activation.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/context_block.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/conv.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/conv_module.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/conv_ws.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/drop.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/generalized_attention.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/hsigmoid.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/hswish.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/non_local.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/norm.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/padding.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/plugin.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/scale.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/transformer.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/upsample.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/bricks/wrappers.py` & `mmcv-lite-2.2.0/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/resnet.py` & `mmcv-lite-2.2.0/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/rfsearch/operator.py` & `mmcv-lite-2.2.0/mmcv/cnn/rfsearch/operator.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/rfsearch/search.py` & `mmcv-lite-2.2.0/mmcv/cnn/rfsearch/search.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/rfsearch/utils.py` & `mmcv-lite-2.2.0/mmcv/cnn/rfsearch/utils.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/utils/flops_counter.py` & `mmcv-lite-2.2.0/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/utils/fuse_conv_bn.py` & `mmcv-lite-2.2.0/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/cnn/vgg.py` & `mmcv-lite-2.2.0/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/image/__init__.py` & `mmcv-lite-2.2.0/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/image/colorspace.py` & `mmcv-lite-2.2.0/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/image/geometric.py` & `mmcv-lite-2.2.0/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/image/io.py` & `mmcv-lite-2.2.0/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/image/misc.py` & `mmcv-lite-2.2.0/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/image/photometric.py` & `mmcv-lite-2.2.0/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/__init__.py` & `mmcv-lite-2.2.0/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/active_rotated_filter.py` & `mmcv-lite-2.2.0/mmcv/ops/active_rotated_filter.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/assign_score_withk.py` & `mmcv-lite-2.2.0/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/ball_query.py` & `mmcv-lite-2.2.0/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/bbox.py` & `mmcv-lite-2.2.0/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/bezier_align.py` & `mmcv-lite-2.2.0/mmcv/ops/bezier_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/bias_act.py` & `mmcv-lite-2.2.0/mmcv/ops/bias_act.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/border_align.py` & `mmcv-lite-2.2.0/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/box_iou_quadri.py` & `mmcv-lite-2.2.0/mmcv/ops/box_iou_quadri.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/box_iou_rotated.py` & `mmcv-lite-2.2.0/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/carafe.py` & `mmcv-lite-2.2.0/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/cc_attention.py` & `mmcv-lite-2.2.0/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/chamfer_distance.py` & `mmcv-lite-2.2.0/mmcv/ops/chamfer_distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         """
         batch_size, n, _ = xyz1.size()
         _, m, _ = xyz2.size()
         device = xyz1.device
         xyz1 = xyz1.contiguous()
         xyz2 = xyz2.contiguous()
 
-        dist1 = torch.zeros(batch_size, n).to(device)
-        dist2 = torch.zeros(batch_size, m).to(device)
+        dist1 = torch.zeros(batch_size, n).type(xyz1.dtype).to(device)
+        dist2 = torch.zeros(batch_size, m).type(xyz2.dtype).to(device)
         idx1 = torch.zeros(batch_size, n).type(torch.IntTensor).to(device)
         idx2 = torch.zeros(batch_size, m).type(torch.IntTensor).to(device)
 
         ext_module.chamfer_distance_forward(xyz1, xyz2, dist1, dist2, idx1,
                                             idx2)
         ctx.save_for_backward(xyz1, xyz2, idx1, idx2)
         return dist1, dist2, idx1, idx2
@@ -77,16 +77,16 @@
             - grad_xyz2 (Tensor):Gradient of the point set with shape \
                 (B, N, 2).
         """
         xyz1, xyz2, idx1, idx2 = ctx.saved_tensors
         device = grad_dist1.device
         grad_dist1 = grad_dist1.contiguous()
         grad_dist2 = grad_dist2.contiguous()
-        grad_xyz1 = torch.zeros(xyz1.size()).to(device)
-        grad_xyz2 = torch.zeros(xyz2.size()).to(device)
+        grad_xyz1 = torch.zeros(xyz1.size()).type(xyz1.dtype).to(device)
+        grad_xyz2 = torch.zeros(xyz2.size()).type(xyz2.dtype).to(device)
 
         ext_module.chamfer_distance_backward(xyz1, xyz2, idx1, idx2,
                                              grad_dist1, grad_dist2, grad_xyz1,
                                              grad_xyz2)
         return grad_xyz1, grad_xyz2
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/contour_expand.py` & `mmcv-lite-2.2.0/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/conv2d_gradfix.py` & `mmcv-lite-2.2.0/mmcv/ops/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/convex_iou.py` & `mmcv-lite-2.2.0/mmcv/ops/convex_iou.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/corner_pool.py` & `mmcv-lite-2.2.0/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/correlation.py` & `mmcv-lite-2.2.0/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/spconv/indice.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/spconv/indice.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSDevice.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSDevice.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSLibrary.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSLibrary.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSLibrary.mm` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSLibrary.mm`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSStream.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSStream.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/mps/MPSUtils.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/mps/MPSUtils.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/parrots_cpp_helper.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/parrots_cpp_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/parrots_cuda_helper.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/parrots_cuda_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_device_registry.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_device_registry.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/pytorch_npu_helper.hpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/pytorch_npu_helper.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,20 @@
  * See the License for the specific language governing permissions and
  * limitations under the License.
  ******************************************************************************/
 
 #ifndef PYTORCH_NPU_HELPER_HPP_
 #define PYTORCH_NPU_HELPER_HPP_
 
-#include <torch_npu/csrc/aten/CustomFunctions.h>
 #include <torch_npu/csrc/framework/utils/CalcuOpUtil.h>
 #include <torch_npu/csrc/framework/utils/OpAdapter.h>
 
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
+#include "pytorch_npu_util.hpp"
 
 #define NPU_NAME_SPACE at_npu::native
 
 #ifdef MMCV_WITH_XLA
 #define REGISTER_NPU_IMPL(key, value) REGISTER_DEVICE_IMPL(key, XLA, value)
 #else
 #define REGISTER_NPU_IMPL(key, value) \
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/prettyprint.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/prettyprint.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/assign_score_withk.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ball_query._parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ball_query._parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ball_query.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ball_query.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/bbox_overlaps.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/border_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/border_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/border_align_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/border_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/border_align_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/border_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_naive.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_naive.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/carafe_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/carafe_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/chamfer_distance.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/contour_expand.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/contour_expand.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/convex_iou.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/convex_iou.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/correlation.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/correlation.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/correlation_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/correlation_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/correlation_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/correlation_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/cudabind.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/cudabind.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_conv.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_conv_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_conv_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/focal_loss.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/focal_loss.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/focal_loss_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/focal_loss_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/furthest_point_sample.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/gather_points.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/gather_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/gather_points_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/gather_points_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/gather_points_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/gather_points_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/group_points.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/group_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/group_points_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/group_points_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/group_points_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/group_points_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/info.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/info.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/iou3d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/iou3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/iou3d_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/iou3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/iou3d_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/iou3d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/knn.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/knn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/knn_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/knn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/masked_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ms_deform_attn.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ms_deform_attn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/nms.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/nms.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/nms_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/nms_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/nms_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/nms_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/nms_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/nms_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/pixel_group.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_polygons.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/prroi_pool.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/prroi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/psamask.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/psamask_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/psamask_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/psamask_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/psamask_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_pool.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roi_pool_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/sync_bn.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/sync_bn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/sync_bn_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/sync_bn_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_interpolate.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_interpolate.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_nn.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_nn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/three_nn_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/three_nn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/tin_shift.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/tin_shift.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/upfirdn2d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/voxelization.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/voxelization.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/voxelization_parrots.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/voxelization_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/parrots/voxelization_pytorch.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/parrots/voxelization_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/assign_score_withk.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/assign_score_withk.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/ball_query.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/ball_query.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/bezier_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/bezier_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/bias_act.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/bias_act.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/border_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/border_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/carafe.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/carafe.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/carafe_naive.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/carafe_naive.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/chamfer_distance.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/chamfer_distance.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/contour_expand.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/contour_expand.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/convex_iou.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/convex_iou.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/correlation.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/correlation.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/nms.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/psamask.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/deform_conv.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/focal_loss.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/focal_loss.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 // Copyright (c) OpenMMLab. All rights reserved
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 #ifdef MMCV_WITH_DIOPI
 #include <diopi/diopirt.h>
 #include <diopi/functions.h>
 #include <diopi/functions_mmcv.h>
+#include <torch/csrc/utils/pybind.h>
 
 #include "csrc_dipu/diopirt/diopirt_impl.h"
+#include "csrc_dipu/runtime/device/deviceapis.h"
+#include "csrc_dipu/utils/helpfunc.hpp"
 
+using dipu::VENDOR_TYPE;
 using dipu::diopi_helper::toDiopiScalar;
 using dipu::diopi_helper::toDiopiTensorHandle;
 #endif
 
 void sigmoid_focal_loss_forward_impl(Tensor input, Tensor target, Tensor weight,
                                      Tensor output, float gamma, float alpha) {
   DISPATCH_DEVICE_IMPL(sigmoid_focal_loss_forward_impl, input, target, weight,
@@ -53,17 +57,24 @@
   }
   diopiContext ctx(dipu::getCurrentDIPUStream().rawstream());
   diopiContextHandle_t ch = &ctx;
   auto target_p = toDiopiTensorHandle(target);
   auto weight_p = toDiopiTensorHandle(weight);
   auto output_p = toDiopiTensorHandle(output);
   if (reinterpret_cast<void *>(diopiSigmoidFocalLossMmcv) != nullptr) {
-    auto ret = diopiSigmoidFocalLossMmcv(ch, output_p, input_p, target_p,
-                                         weight_p, gamma, alpha);
-    if (ret == diopiSuccess) return;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret = diopiSigmoidFocalLossMmcv(ch, output_p, input_p, target_p,
+                                           weight_p, gamma, alpha);
+      if (ret == diopiSuccess) return;
+    } else {
+      auto ret = diopiSigmoidFocalLossMmcv(ch, output_p, input_p, target_p,
+                                           weight_p, gamma, alpha);
+      if (ret == diopiSuccess) return;
+    }
   }
   LOG(WARNING)
       << "Fallback to cpu: mmcv ext op sigmoid_focal_loss_forward_impl";
   auto input_cpu = input.cpu();
   auto target_cpu = target.cpu();
   auto weight_cpu = weight.cpu();
   auto output_cpu = output.cpu();
@@ -86,17 +97,24 @@
   }
   diopiContext ctx(dipu::getCurrentDIPUStream().rawstream());
   diopiContextHandle_t ch = &ctx;
   auto target_p = toDiopiTensorHandle(target);
   auto weight_p = toDiopiTensorHandle(weight);
   auto grad_input_p = toDiopiTensorHandle(grad_input);
   if (reinterpret_cast<void *>(diopiSigmoidFocalLossBackwardMmcv) != nullptr) {
-    auto ret = diopiSigmoidFocalLossBackwardMmcv(
-        ch, grad_input_p, input_p, target_p, weight_p, gamma, alpha);
-    if (ret == diopiSuccess) return;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret = diopiSigmoidFocalLossBackwardMmcv(
+          ch, grad_input_p, input_p, target_p, weight_p, gamma, alpha);
+      if (ret == diopiSuccess) return;
+    } else {
+      auto ret = diopiSigmoidFocalLossBackwardMmcv(
+          ch, grad_input_p, input_p, target_p, weight_p, gamma, alpha);
+      if (ret == diopiSuccess) return;
+    }
   }
   LOG(WARNING)
       << "Fallback to cpu: mmcv ext op sigmoid_focal_loss_forward_impl";
   auto input_cpu = input.cpu();
   auto target_cpu = target.cpu();
   auto weight_cpu = weight.cpu();
   auto grad_input_cpu = grad_input.cpu();
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/gather_points.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/gather_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/group_points.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/group_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/info.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/info.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/iou3d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/iou3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/knn.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/knn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/masked_conv2d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/masked_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/diff_iou_rotated_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/diff_iou_rotated_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/scatter_points_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/scatter_points_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 // Copyright (c) OpenMMLab. All rights reserved
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 #ifdef MMCV_WITH_DIOPI
 #include <diopi/diopirt.h>
 #include <diopi/functions.h>
 #include <diopi/functions_mmcv.h>
+#include <torch/csrc/utils/pybind.h>
 
 #include "csrc_dipu/diopirt/diopirt_impl.h"
+#include "csrc_dipu/runtime/device/deviceapis.h"
+#include "csrc_dipu/utils/helpfunc.hpp"
 
+using dipu::VENDOR_TYPE;
 using dipu::diopi_helper::toDiopiScalar;
 using dipu::diopi_helper::toDiopiTensorHandle;
 #endif
 
 void modulated_deformable_im2col_impl(
     const Tensor data_im, const Tensor data_offset, const Tensor data_mask,
     const int batch_size, const int channels, const int height_im,
@@ -269,19 +273,28 @@
   auto bias_p = toDiopiTensorHandle(bias);
   auto ones_p = toDiopiTensorHandle(ones);
   auto offset_p = toDiopiTensorHandle(offset);
   auto mask_p = toDiopiTensorHandle(mask);
   auto output_p = toDiopiTensorHandle(output);
   auto columns_p = toDiopiTensorHandle(columns);
   if (reinterpret_cast<void*>(diopiModulatedDeformConvMmcv) != nullptr) {
-    auto ret = diopiModulatedDeformConvMmcv(
-        ch, output_p, columns_p, ones_p, input_p, weight_p, bias_p, offset_p,
-        mask_p, kernel_h, kernel_w, stride_h, stride_w, pad_h, pad_w,
-        dilation_h, dilation_w, group, deformable_group, with_bias);
-    if (ret == diopiSuccess) return;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret = diopiModulatedDeformConvMmcv(
+          ch, output_p, columns_p, ones_p, input_p, weight_p, bias_p, offset_p,
+          mask_p, kernel_h, kernel_w, stride_h, stride_w, pad_h, pad_w,
+          dilation_h, dilation_w, group, deformable_group, with_bias);
+      if (ret == diopiSuccess) return;
+    } else {
+      auto ret = diopiModulatedDeformConvMmcv(
+          ch, output_p, columns_p, ones_p, input_p, weight_p, bias_p, offset_p,
+          mask_p, kernel_h, kernel_w, stride_h, stride_w, pad_h, pad_w,
+          dilation_h, dilation_w, group, deformable_group, with_bias);
+      if (ret == diopiSuccess) return;
+    }
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op modulated_deform_conv_forward";
   auto input_cpu = input.cpu();
   auto weight_cpu = weight.cpu();
   auto bias_cpu = bias.cpu();
   auto ones_cpu = ones.cpu();
   auto offset_cpu = offset.cpu();
@@ -327,20 +340,32 @@
   auto grad_bias_p = toDiopiTensorHandle(grad_bias);
   auto grad_offset_p = toDiopiTensorHandle(grad_offset);
   auto grad_mask_p = toDiopiTensorHandle(grad_mask);
   auto grad_output_p = toDiopiTensorHandle(grad_output);
 
   if (reinterpret_cast<void*>(diopiModulatedDeformConvBackwardMmcv) !=
       nullptr) {
-    auto ret = diopiModulatedDeformConvBackwardMmcv(
-        ch, grad_input_p, grad_weight_p, grad_bias_p, grad_offset_p,
-        grad_mask_p, input_p, weight_p, bias_p, ones_p, offset_p, mask_p,
-        columns_p, grad_output_p, kernel_h, kernel_w, stride_h, stride_w, pad_h,
-        pad_w, dilation_h, dilation_w, group, deformable_group, with_bias);
-    if (ret == diopiSuccess) return;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret = diopiModulatedDeformConvBackwardMmcv(
+          ch, grad_input_p, grad_weight_p, grad_bias_p, grad_offset_p,
+          grad_mask_p, input_p, weight_p, bias_p, ones_p, offset_p, mask_p,
+          columns_p, grad_output_p, kernel_h, kernel_w, stride_h, stride_w,
+          pad_h, pad_w, dilation_h, dilation_w, group, deformable_group,
+          with_bias);
+      if (ret == diopiSuccess) return;
+    } else {
+      auto ret = diopiModulatedDeformConvBackwardMmcv(
+          ch, grad_input_p, grad_weight_p, grad_bias_p, grad_offset_p,
+          grad_mask_p, input_p, weight_p, bias_p, ones_p, offset_p, mask_p,
+          columns_p, grad_output_p, kernel_h, kernel_w, stride_h, stride_w,
+          pad_h, pad_w, dilation_h, dilation_w, group, deformable_group,
+          with_bias);
+      if (ret == diopiSuccess) return;
+    }
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op modulated_deform_conv_forward";
   auto input_cpu = input.cpu();
   auto weight_cpu = weight.cpu();
   auto bias_cpu = bias.cpu();
   auto ones_cpu = ones.cpu();
   auto offset_cpu = offset.cpu();
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/nms.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/nms.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 // Copyright (c) OpenMMLab. All rights reserved
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 #ifdef MMCV_WITH_DIOPI
 #include <diopi/diopirt.h>
 #include <diopi/functions.h>
 #include <diopi/functions_mmcv.h>
+#include <torch/csrc/utils/pybind.h>
 
 #include "csrc_dipu/base/basedef.h"
 #include "csrc_dipu/diopirt/diopirt_impl.h"
+#include "csrc_dipu/runtime/device/deviceapis.h"
+#include "csrc_dipu/utils/helpfunc.hpp"
 
+using dipu::VENDOR_TYPE;
 using dipu::diopi_helper::toDiopiScalar;
 using dipu::diopi_helper::toDiopiTensorHandle;
 #endif
 
 Tensor nms_impl(Tensor boxes, Tensor scores, float iou_threshold, int offset) {
   return DISPATCH_DEVICE_IMPL(nms_impl, boxes, scores, iou_threshold, offset);
 }
@@ -41,19 +45,29 @@
   diopiContextHandle_t ch = &ctx;
   Tensor out;
   auto outp = toDiopiTensorHandle(out);
   diopiTensorHandle_t* outhandle = &outp;
   auto scores_p = toDiopiTensorHandle(scores);
   bool is_mock_cuda = boxes.device().type() == dipu::DIPU_DEVICE_TYPE;
   if (is_mock_cuda && reinterpret_cast<void*>(diopiNmsMmcv) != nullptr) {
-    auto ret =
-        diopiNmsMmcv(ch, outhandle, boxes_p, scores_p, iou_threshold, offset);
-    if (ret == diopiSuccess) {
-      auto tensorhandle = reinterpret_cast<Tensor*>(*outhandle);
-      return *tensorhandle;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret =
+          diopiNmsMmcv(ch, outhandle, boxes_p, scores_p, iou_threshold, offset);
+      if (ret == diopiSuccess) {
+        auto tensorhandle = reinterpret_cast<Tensor*>(*outhandle);
+        return *tensorhandle;
+      }
+    } else {
+      auto ret =
+          diopiNmsMmcv(ch, outhandle, boxes_p, scores_p, iou_threshold, offset);
+      if (ret == diopiSuccess) {
+        auto tensorhandle = reinterpret_cast<Tensor*>(*outhandle);
+        return *tensorhandle;
+      }
     }
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op nms";
   auto boxes_cpu = boxes.cpu();
   auto scores_cpu = scores.cpu();
   return nms_impl(boxes_cpu, scores_cpu, iou_threshold, offset);
 }
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/nms_quadri.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/nms_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/nms_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/nms_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/box_iou_rotated_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/box_iou_rotated_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #include "pytorch_npu_helper.hpp"
-
 using namespace NPU_NAME_SPACE;
 using namespace std;
 
 void sigmoid_focal_loss_forward_npu(Tensor input, Tensor target, Tensor weight,
                                     Tensor output, float gamma, float alpha) {
   int64_t n_class = input.size(1);
   at::Tensor target_y = at::ones_like(input);
@@ -96,15 +95,30 @@
       .Attr("reduction", reduction)
       .Run();
   int64_t n_batch = input.size(0);
   c10::SmallVector<int64_t, 2> offsets = {0, 0};
   c10::SmallVector<int64_t, 2> sizes = {n_batch, 1};
   at::IntArrayRef offset = at::IntArrayRef(offsets);
   at::IntArrayRef size = at::IntArrayRef(sizes);
-  at_npu::native::custom_ops::npu_slice_out(op_output, offset, size, output);
+  at::IntArrayRef size_array = at::IntArrayRef(sizes);
+  c10::SmallVector<int64_t, 8> offsetVec;
+  for (uint64_t i = 0; i < offset.size(); i++) {
+    offsetVec.emplace_back(offset[i]);
+  }
+  c10::SmallVector<int64_t, 8> sizeVec;
+  for (uint64_t i = 0; i < size_array.size(); i++) {
+    sizeVec.emplace_back(size_array[i]);
+  }
+  OpCommand cmd2;
+  cmd2.Name("Slice")
+      .Input(op_output)
+      .Input(offsetVec)
+      .Input(sizeVec)
+      .Output(output)
+      .Run();
 }
 
 void softmax_focal_loss_forward_impl(Tensor input, Tensor target, Tensor weight,
                                      Tensor grad_input, float gamma,
                                      float alpha);
 
 void softmax_focal_loss_backward_npu(Tensor input, Tensor target, Tensor weight,
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
                                 float alpha, float scale) {
   at::Tensor py = at::empty_like(input);
   // forward
   if (grad == 0) {
     auto input_size = input.sizes();
     int input_length = input_size.size();
     c10::SmallVector<int64_t, SIZE> input_size_tmp;
-    input_size_tmp = array_to_small_vector(input_size);
+    for (uint64_t i = 0; i < input_size.size(); i++) {
+      input_size_tmp.emplace_back(input_size[i]);
+    }
     if (input_length > 1) {
       for (int i = 0; i < input_length; i++) {
         if (i != 1) {
           input_size_tmp[i] = 1;
         }
       }
     }
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,19 @@
   if (idx.scalar_type() != at::ScalarType::Int) {
     indices = idx.to(at::kInt);
   }
   if (idx.dim() == 0) {
     indices.unsqueeze_(0);
   }
   int64_t dim = 0;
-  at::SmallVector<int64_t, N> pad_size = array_to_small_vector(idx.sizes());
+  auto shape = idx.sizes();
+  c10::SmallVector<int64_t, 8> pad_size;
+  for (uint64_t i = 0; i < shape.size(); i++) {
+    pad_size.emplace_back(shape[i]);
+  }
   at::Tensor trans_grad_points = grad_points.transpose(1, 2).contiguous();
   at::Tensor grad_points_view = trans_grad_points.view(
       {trans_grad_points.sizes()[0] * trans_grad_points.sizes()[1],
        trans_grad_points.sizes()[2]});
   at::Tensor trans_grad_out = grad_out.transpose(1, 2).contiguous();
   trans_grad_out = trans_grad_out.view(
       {trans_grad_out.sizes()[0] * trans_grad_out.sizes()[1],
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/group_points_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/group_points_npu.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -16,29 +16,29 @@
   index = index.to(points.device());
   index = index.view({-1, 1, 1});
   index = at::mul(index, n);
   at::Tensor indices = at::add(index, idx);
   indices = indices.view({-1});
 
   at::Tensor trans_features = points.transpose(1, 2);
-  at::Tensor features = NpuUtils::format_contiguous(trans_features);
+  at::Tensor features = trans_features.contiguous();
   features = features.view({b * n, c});
 
   OpCommand cmd;
   cmd.Name("GatherV2")
       .Input(features)
       .Input(indices)
       .Input(axis)
       .Output(out)
       .Attr("batch_dims", batch_dims)
       .Run();
 
   at::Tensor output =
       out.view({b, npoints, nsample, c}).transpose(1, 3).transpose(2, 3);
-  at::Tensor res = NpuUtils::format_contiguous(output);
+  at::Tensor res = output.contiguous();
   out.copy_(res);
 }
 
 void group_points_forward_impl(int b, int c, int n, int npoints, int nsample,
                                const Tensor points, const Tensor idx,
                                Tensor out);
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/points_in_polygons_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/points_in_polygons_npu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 void points_in_polygons_npu(const Tensor points, Tensor polygons, Tensor output,
                             const int rows, const int cols) {
   TORCH_CHECK(
       (polygons.sizes()[0] <= MAX_POLYGONS_BATCH),
       "The batch of polygons tensor must be less than MAX_POLYGONS_BATCH");
   at::Tensor trans_polygons = polygons.transpose(0, 1);
   OpCommand cmd;
-  at::Tensor new_trans_polygons = NpuUtils::format_contiguous(trans_polygons);
+  at::Tensor new_trans_polygons = trans_polygons.contiguous();
   cmd.Name("PointsInPolygons")
       .Input(points, (string) "points")
       .Input(new_trans_polygons, (string) "polygons")
       .Output(output)
       .Run();
 }
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -37,16 +37,19 @@
   int64_t aligned_width_64 = aligned_width;
   int64_t sampling_ratio_64 = sampling_ratio;
   int64_t roi_end_mode = 2;
   if (!aligned) {
     LOG(WARNING) << "The [aligned] attr in roi_align_grad op is false";
     roi_end_mode = 0;
   }
-  c10::SmallVector<int64_t, SIZE> xdiff_shape =
-      array_to_small_vector(grad_input.sizes());
+  auto shape = grad_input.sizes();
+  c10::SmallVector<int64_t, SIZE> xdiff_shape;
+  for (uint64_t i = 0; i < shape.size(); i++) {
+    xdiff_shape.emplace_back(shape[i]);
+  }
   OpCommand cmd;
   cmd.Name("ROIAlignGrad")
       .Input(grad_output)
       .Input(rois)
       .Output(grad_input)
       .Attr("xdiff_shape", xdiff_shape)
       .Attr("pooled_width", aligned_width_64)
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/pixel_group.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/points_in_boxes.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/points_in_polygons.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/points_in_polygons.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/prroi_pool.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/prroi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/psamask.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/pybind.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/pybind.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roi_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roi_align.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 // Copyright (c) OpenMMLab. All rights reserved
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 #ifdef MMCV_WITH_DIOPI
 #include <diopi/diopirt.h>
 #include <diopi/functions.h>
 #include <diopi/functions_mmcv.h>
+#include <torch/csrc/utils/pybind.h>
 
 #include "csrc_dipu/base/basedef.h"
 #include "csrc_dipu/diopirt/diopirt_impl.h"
+#include "csrc_dipu/runtime/device/deviceapis.h"
+#include "csrc_dipu/utils/helpfunc.hpp"
 
+using dipu::VENDOR_TYPE;
 using dipu::diopi_helper::toDiopiScalar;
 using dipu::diopi_helper::toDiopiTensorHandle;
 #endif
 
 void roi_align_forward_impl(Tensor input, Tensor rois, Tensor output,
                             Tensor argmax_y, Tensor argmax_x,
                             int aligned_height, int aligned_width,
@@ -52,18 +56,26 @@
   diopiContextHandle_t ch = &ctx;
   auto rois_p = toDiopiTensorHandle(rois);
   auto out_p = toDiopiTensorHandle(output);
   auto argmax_y_p = toDiopiTensorHandle(argmax_y);
   auto argmax_x_p = toDiopiTensorHandle(argmax_x);
   bool is_mock_cuda = input.device().type() == dipu::DIPU_DEVICE_TYPE;
   if (is_mock_cuda && reinterpret_cast<void *>(diopiRoiAlignMmcv) != nullptr) {
-    auto ret = diopiRoiAlignMmcv(
-        ch, out_p, argmax_y_p, argmax_x_p, input_p, rois_p, aligned_height,
-        aligned_width, sampling_ratio, pool_mode, spatial_scale, aligned);
-    if (ret == diopiSuccess) return;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret = diopiRoiAlignMmcv(
+          ch, out_p, argmax_y_p, argmax_x_p, input_p, rois_p, aligned_height,
+          aligned_width, sampling_ratio, pool_mode, spatial_scale, aligned);
+      if (ret == diopiSuccess) return;
+    } else {
+      auto ret = diopiRoiAlignMmcv(
+          ch, out_p, argmax_y_p, argmax_x_p, input_p, rois_p, aligned_height,
+          aligned_width, sampling_ratio, pool_mode, spatial_scale, aligned);
+      if (ret == diopiSuccess) return;
+    }
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op roi_align_forward";
   auto input_cpu = input.cpu();
   auto rois_cpu = rois.cpu();
   auto out_cpu = output.cpu();
   auto argmax_y_cpu = argmax_y.cpu();
   auto argmax_x_cpu = argmax_x.cpu();
@@ -92,19 +104,28 @@
   auto argmax_x_ = toDiopiTensorHandle(argmax_x);
   auto grad_input_ = toDiopiTensorHandle(grad_input);
   diopiContext ctx(dipu::getCurrentDIPUStream().rawstream());
   diopiContextHandle_t ch = &ctx;
   bool is_mock_cuda = grad_output.device().type() == dipu::DIPU_DEVICE_TYPE;
   if (is_mock_cuda &&
       reinterpret_cast<void *>(diopiRoiAlignBackwardMmcv) != nullptr) {
-    auto ret = diopiRoiAlignBackwardMmcv(ch, grad_input_, grad_output_, rois_,
-                                         argmax_y_, argmax_x_, aligned_height,
-                                         aligned_width, sampling_ratio,
-                                         pool_mode, spatial_scale, aligned);
-    if (ret == diopiSuccess) return;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret = diopiRoiAlignBackwardMmcv(ch, grad_input_, grad_output_, rois_,
+                                           argmax_y_, argmax_x_, aligned_height,
+                                           aligned_width, sampling_ratio,
+                                           pool_mode, spatial_scale, aligned);
+      if (ret == diopiSuccess) return;
+    } else {
+      auto ret = diopiRoiAlignBackwardMmcv(ch, grad_input_, grad_output_, rois_,
+                                           argmax_y_, argmax_x_, aligned_height,
+                                           aligned_width, sampling_ratio,
+                                           pool_mode, spatial_scale, aligned);
+      if (ret == diopiSuccess) return;
+    }
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op roi_align_backward";
   auto grad_output_cpu = grad_output.cpu();
   auto rois_cpu = rois.cpu();
   auto argmax_y_cpu = argmax_y.cpu();
   auto argmax_x_cpu = argmax_x.cpu();
   auto grad_input_cpu = grad_input.cpu();
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roi_pool.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/scatter_points.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/scatter_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/spconv_ops.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/spconv_ops.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/spconv_utils.h` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/spconv_utils.h`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/sync_bn.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/sync_bn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/three_interpolate.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/three_interpolate.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/three_nn.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/three_nn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/tin_shift.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/tin_shift.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/upfirdn2d.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/csrc/pytorch/voxelization.cpp` & `mmcv-lite-2.2.0/mmcv/ops/csrc/pytorch/voxelization.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 // Copyright (c) OpenMMLab. All rights reserved.
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 #ifdef MMCV_WITH_DIOPI
 #include <diopi/diopirt.h>
 #include <diopi/functions.h>
 #include <diopi/functions_mmcv.h>
+#include <torch/csrc/utils/pybind.h>
 
 #include "csrc_dipu/diopirt/diopirt_impl.h"
+#include "csrc_dipu/runtime/device/deviceapis.h"
+#include "csrc_dipu/utils/helpfunc.hpp"
 
+using dipu::VENDOR_TYPE;
 using dipu::diopi_helper::toDiopiScalar;
 using dipu::diopi_helper::toDiopiTensorHandle;
 #endif
 
 int hard_voxelize_forward_impl(const at::Tensor &points, at::Tensor &voxels,
                                at::Tensor &coors,
                                at::Tensor &num_points_per_voxel,
@@ -80,19 +84,28 @@
   auto voxel_size_p = toDiopiTensorHandle(voxel_size);
   auto coors_range_p = toDiopiTensorHandle(coors_range);
   auto voxels_p = toDiopiTensorHandle(voxels);
   auto coors_p = toDiopiTensorHandle(coors);
   auto num_points_per_voxel_p = toDiopiTensorHandle(num_points_per_voxel);
   auto voxel_num_p = toDiopiTensorHandle(voxel_num);
   if (reinterpret_cast<void *>(diopiHardVoxelizeMmcv) != nullptr) {
-    auto ret = diopiHardVoxelizeMmcv(
-        ch, voxels_p, coors_p, num_points_per_voxel_p, voxel_num_p, points_p,
-        voxel_size_p, coors_range_p, max_points, max_voxels, NDim,
-        deterministic);
-    if (ret == diopiSuccess) return;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret = diopiHardVoxelizeMmcv(
+          ch, voxels_p, coors_p, num_points_per_voxel_p, voxel_num_p, points_p,
+          voxel_size_p, coors_range_p, max_points, max_voxels, NDim,
+          deterministic);
+      if (ret == diopiSuccess) return;
+    } else {
+      auto ret = diopiHardVoxelizeMmcv(
+          ch, voxels_p, coors_p, num_points_per_voxel_p, voxel_num_p, points_p,
+          voxel_size_p, coors_range_p, max_points, max_voxels, NDim,
+          deterministic);
+      if (ret == diopiSuccess) return;
+    }
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op hard_voxelize_forward";
   auto points_cpu = points.cpu();
   auto voxel_size_cpu = voxel_size.cpu();
   auto coors_range_cpu = coors_range.cpu();
   auto voxels_cpu = voxels.cpu();
   auto coors_cpu = coors.cpu();
@@ -142,17 +155,24 @@
   }
   diopiContext ctx(dipu::getCurrentDIPUStream().rawstream());
   diopiContextHandle_t ch = &ctx;
   auto voxel_size_p = toDiopiTensorHandle(voxel_size);
   auto coors_range_p = toDiopiTensorHandle(coors_range);
   auto coors_p = toDiopiTensorHandle(coors);
   if (reinterpret_cast<void *>(diopiDynamicVoxelizeMmcv) != nullptr) {
-    auto ret = diopiDynamicVoxelizeMmcv(ch, coors_p, points_p, voxel_size_p,
-                                        coors_range_p, NDim);
-    if (ret == diopiSuccess) return;
+    if (strcmp(dipu::VendorTypeToStr(VENDOR_TYPE), "NPU") == 0) {
+      pybind11::gil_scoped_release no_gil;
+      auto ret = diopiDynamicVoxelizeMmcv(ch, coors_p, points_p, voxel_size_p,
+                                          coors_range_p, NDim);
+      if (ret == diopiSuccess) return;
+    } else {
+      auto ret = diopiDynamicVoxelizeMmcv(ch, coors_p, points_p, voxel_size_p,
+                                          coors_range_p, NDim);
+      if (ret == diopiSuccess) return;
+    }
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op dynamic_voxelize_forward";
   auto points_cpu = points.cpu();
   auto voxel_size_cpu = voxel_size.cpu();
   auto coors_range_cpu = coors_range.cpu();
   auto coors_cpu = coors.cpu();
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/deform_conv.py` & `mmcv-lite-2.2.0/mmcv/ops/deform_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,18 +47,19 @@
             groups_i=groups,
             deform_groups_i=deform_groups,
             bias_i=bias,
             im2col_step_i=im2col_step)
 
     @staticmethod
     def _npu_backward(ctx, grad_output):
+        import torch_npu
         input_tensor, weight, offset_out, offset_all, sort_index_for_npu_bp = \
             ctx.saved_tensors
         grad_input, grad_weight, grad_offset_all, grad_bias = \
-            torch.npu_deformable_conv2dbk(
+            torch_npu.npu_deformable_conv2dbk(
                 input_tensor, grad_output, offset_out, weight, offset_all,
                 kernel_size=[weight.shape[3], weight.shape[2]],
                 stride=[1, 1, ctx.stride[0], ctx.stride[1]],
                 padding=[ctx.padding[0], ctx.padding[0], ctx.padding[1],
                          ctx.padding[1]],
                 dilation=[1, 1, ctx.dilation[0], ctx.dilation[1]],
                 groups=ctx.groups, deformable_groups=ctx.deform_groups,
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/deform_roi_pool.py` & `mmcv-lite-2.2.0/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/deprecated_wrappers.py` & `mmcv-lite-2.2.0/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/diff_iou_rotated.py` & `mmcv-lite-2.2.0/mmcv/ops/diff_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/filtered_lrelu.py` & `mmcv-lite-2.2.0/mmcv/ops/filtered_lrelu.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/focal_loss.py` & `mmcv-lite-2.2.0/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/furthest_point_sample.py` & `mmcv-lite-2.2.0/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/fused_bias_leakyrelu.py` & `mmcv-lite-2.2.0/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/gather_points.py` & `mmcv-lite-2.2.0/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/group_points.py` & `mmcv-lite-2.2.0/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/info.py` & `mmcv-lite-2.2.0/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/iou3d.py` & `mmcv-lite-2.2.0/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/knn.py` & `mmcv-lite-2.2.0/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/masked_conv.py` & `mmcv-lite-2.2.0/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/merge_cells.py` & `mmcv-lite-2.2.0/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/min_area_polygons.py` & `mmcv-lite-2.2.0/mmcv/ops/min_area_polygons.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/modulated_deform_conv.py` & `mmcv-lite-2.2.0/mmcv/ops/modulated_deform_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,17 @@
                                   sort_index_bp)
         return output
 
     @staticmethod
     def _npu_backward(ctx, grad_output):
         input_tensor, weight, offset_out, offset_all, sort_index_bp = \
             ctx.saved_tensors
+        import torch_npu
         grad_input, grad_weight, grad_offset_all, grad_bias = \
-            torch.npu_deformable_conv2dbk(
+            torch_npu.npu_deformable_conv2dbk(
                 input_tensor, grad_output, offset_out, weight, offset_all,
                 kernel_size=[weight.shape[3], weight.shape[2]],
                 stride=[1, 1, ctx.stride[0], ctx.stride[1]],
                 padding=[ctx.padding[0], ctx.padding[0], ctx.padding[1],
                          ctx.padding[1]],
                 dilation=[1, 1, ctx.dilation[0], ctx.dilation[1]],
                 groups=ctx.groups, deformable_groups=ctx.deform_groups,
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/multi_scale_deform_attn.py` & `mmcv-lite-2.2.0/mmcv/ops/multi_scale_deform_attn.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from mmengine.model import BaseModule, constant_init, xavier_init
 from mmengine.registry import MODELS
 from mmengine.utils import deprecated_api_warning
 from torch.autograd.function import Function, once_differentiable
 
-from mmcv.utils import IS_CUDA_AVAILABLE, IS_MLU_AVAILABLE
+from mmcv.utils import IS_CUDA_AVAILABLE, IS_MLU_AVAILABLE, IS_NPU_AVAILABLE
 from ..utils import ext_loader
 
 ext_module = ext_loader.load_ext(
     '_ext', ['ms_deform_attn_backward', 'ms_deform_attn_forward'])
 
 
 class MultiScaleDeformableAttnFunction(Function):
@@ -80,15 +80,15 @@
 
         Args:
             grad_output (torch.Tensor): Gradient of output tensor of forward.
 
         Returns:
             tuple[Tensor]: Gradient of input tensors in forward.
         """
-        value, value_spatial_shapes, value_level_start_index,\
+        value, value_spatial_shapes, value_level_start_index, \
             sampling_locations, attention_weights = ctx.saved_tensors
         grad_value = torch.zeros_like(value)
         grad_sampling_loc = torch.zeros_like(sampling_locations)
         grad_attn_weight = torch.zeros_like(attention_weights)
 
         ext_module.ms_deform_attn_backward(
             value,
@@ -360,15 +360,16 @@
                 * reference_points[:, :, None, :, None, 2:] \
                 * 0.5
         else:
             raise ValueError(
                 f'Last dim of reference_points must be'
                 f' 2 or 4, but get {reference_points.shape[-1]} instead.')
         if ((IS_CUDA_AVAILABLE and value.is_cuda)
-                or (IS_MLU_AVAILABLE and value.is_mlu)):
+                or (IS_MLU_AVAILABLE and value.is_mlu)
+                or (IS_NPU_AVAILABLE and value.device.type == 'npu')):
             output = MultiScaleDeformableAttnFunction.apply(
                 value, spatial_shapes, level_start_index, sampling_locations,
                 attention_weights, self.im2col_step)
         else:
             output = multi_scale_deformable_attn_pytorch(
                 value, spatial_shapes, sampling_locations, attention_weights)
```

### Comparing `mmcv-lite-2.1.0/mmcv/ops/nms.py` & `mmcv-lite-2.2.0/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/pixel_group.py` & `mmcv-lite-2.2.0/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/point_sample.py` & `mmcv-lite-2.2.0/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/points_in_boxes.py` & `mmcv-lite-2.2.0/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/points_in_polygons.py` & `mmcv-lite-2.2.0/mmcv/ops/points_in_polygons.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/points_sampler.py` & `mmcv-lite-2.2.0/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/prroi_pool.py` & `mmcv-lite-2.2.0/mmcv/ops/prroi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/psa_mask.py` & `mmcv-lite-2.2.0/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/riroi_align_rotated.py` & `mmcv-lite-2.2.0/mmcv/ops/riroi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/roi_align.py` & `mmcv-lite-2.2.0/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/roi_align_rotated.py` & `mmcv-lite-2.2.0/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/roi_pool.py` & `mmcv-lite-2.2.0/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/roiaware_pool3d.py` & `mmcv-lite-2.2.0/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/roipoint_pool3d.py` & `mmcv-lite-2.2.0/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/rotated_feature_align.py` & `mmcv-lite-2.2.0/mmcv/ops/rotated_feature_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/saconv.py` & `mmcv-lite-2.2.0/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/scatter_points.py` & `mmcv-lite-2.2.0/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/sparse_conv.py` & `mmcv-lite-2.2.0/mmcv/ops/sparse_conv.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/sparse_functional.py` & `mmcv-lite-2.2.0/mmcv/ops/sparse_functional.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/sparse_modules.py` & `mmcv-lite-2.2.0/mmcv/ops/sparse_modules.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/sparse_ops.py` & `mmcv-lite-2.2.0/mmcv/ops/sparse_ops.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/sparse_pool.py` & `mmcv-lite-2.2.0/mmcv/ops/sparse_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/sparse_structure.py` & `mmcv-lite-2.2.0/mmcv/ops/sparse_structure.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/sync_bn.py` & `mmcv-lite-2.2.0/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/three_interpolate.py` & `mmcv-lite-2.2.0/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/three_nn.py` & `mmcv-lite-2.2.0/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/tin_shift.py` & `mmcv-lite-2.2.0/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/upfirdn2d.py` & `mmcv-lite-2.2.0/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/ops/voxelize.py` & `mmcv-lite-2.2.0/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/transforms/__init__.py` & `mmcv-lite-2.2.0/mmcv/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/transforms/base.py` & `mmcv-lite-2.2.0/mmcv/transforms/base.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/transforms/formatting.py` & `mmcv-lite-2.2.0/mmcv/transforms/formatting.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/transforms/loading.py` & `mmcv-lite-2.2.0/mmcv/transforms/loading.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/transforms/processing.py` & `mmcv-lite-2.2.0/mmcv/transforms/processing.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/transforms/utils.py` & `mmcv-lite-2.2.0/mmcv/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/transforms/wrappers.py` & `mmcv-lite-2.2.0/mmcv/transforms/wrappers.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/utils/env.py` & `mmcv-lite-2.2.0/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/utils/ext_loader.py` & `mmcv-lite-2.2.0/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/utils/parrots_jit.py` & `mmcv-lite-2.2.0/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/version.py` & `mmcv-lite-2.2.0/mmcv/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '2.1.0'
+__version__ = '2.2.0'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `mmcv-lite-2.1.0/mmcv/video/__init__.py` & `mmcv-lite-2.2.0/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/video/io.py` & `mmcv-lite-2.2.0/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/video/optflow.py` & `mmcv-lite-2.2.0/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/video/processing.py` & `mmcv-lite-2.2.0/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/visualization/color.py` & `mmcv-lite-2.2.0/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/visualization/image.py` & `mmcv-lite-2.2.0/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv/visualization/optflow.py` & `mmcv-lite-2.2.0/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/mmcv_lite.egg-info/PKG-INFO` & `mmcv-lite-2.2.0/mmcv_lite.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcv-lite
-Version: 2.1.0
+Version: 2.2.0
 Summary: OpenMMLab Computer Vision Foundation
 Home-page: https://github.com/open-mmlab/mmcv
 Author: MMCV Contributors
 Author-email: openmmlab@gmail.com
 Keywords: computer vision
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mmcv-lite-2.1.0/mmcv_lite.egg-info/SOURCES.txt` & `mmcv-lite-2.2.0/mmcv_lite.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 mmcv/ops/csrc/common/parrots_cpp_helper.hpp
 mmcv/ops/csrc/common/parrots_cuda_helper.hpp
 mmcv/ops/csrc/common/pytorch_cpp_helper.hpp
 mmcv/ops/csrc/common/pytorch_cuda_helper.hpp
 mmcv/ops/csrc/common/pytorch_device_registry.hpp
 mmcv/ops/csrc/common/pytorch_mlu_helper.hpp
 mmcv/ops/csrc/common/pytorch_npu_helper.hpp
+mmcv/ops/csrc/common/pytorch_npu_util.hpp
 mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh
 mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh
@@ -486,27 +487,36 @@
 mmcv/ops/csrc/pytorch/mlu/scatter_points_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp
 mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
 mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp
+mmcv/ops/csrc/pytorch/npu/ball_query_npu.cpp
 mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp
 mmcv/ops/csrc/pytorch/npu/box_iou_rotated_npu.cpp
+mmcv/ops/csrc/pytorch/npu/chamfer_distance_npu.cpp
+mmcv/ops/csrc/pytorch/npu/common_util.h
 mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
 mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
 mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
 mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp
 mmcv/ops/csrc/pytorch/npu/group_points_npu.cpp
+mmcv/ops/csrc/pytorch/npu/ms_deform_attn_npu.cpp
 mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
 mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp
 mmcv/ops/csrc/pytorch/npu/points_in_polygons_npu.cpp
 mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
 mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp
+mmcv/ops/csrc/pytorch/npu/roi_align_rotated_npu.cpp
 mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
+mmcv/ops/csrc/pytorch/npu/rotated_feature_align_npu.cpp
+mmcv/ops/csrc/pytorch/npu/stack_ball_query_npu.cpp
+mmcv/ops/csrc/pytorch/npu/stack_group_points_npu.cpp
+mmcv/ops/csrc/pytorch/npu/three_interpolate_npu.cpp
 mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp
 mmcv/transforms/__init__.py
 mmcv/transforms/base.py
 mmcv/transforms/builder.py
 mmcv/transforms/formatting.py
 mmcv/transforms/loading.py
 mmcv/transforms/processing.py
```

### Comparing `mmcv-lite-2.1.0/setup.cfg` & `mmcv-lite-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/setup.py` & `mmcv-lite-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,18 +240,20 @@
             extension = CppExtension
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common'))
             dipu_root = os.getenv('DIPU_ROOT')
             diopi_path = os.getenv('DIOPI_PATH')
             dipu_path = os.getenv('DIPU_PATH')
             vendor_include_dirs = os.getenv('VENDOR_INCLUDE_DIRS')
             nccl_include_dirs = os.getenv('NCCL_INCLUDE_DIRS')
+            pytorch_dir = os.getenv('PYTORCH_DIR')
             include_dirs.append(dipu_root)
             include_dirs.append(diopi_path + '/include')
             include_dirs.append(dipu_path + '/dist/include')
             include_dirs.append(vendor_include_dirs)
+            include_dirs.append(pytorch_dir + 'torch/include')
             if nccl_include_dirs:
                 include_dirs.append(nccl_include_dirs)
             library_dirs += [dipu_root]
             libraries += ['torch_dipu']
         elif is_rocm_pytorch or torch.cuda.is_available() or os.getenv(
                 'FORCE_CUDA', '0') == '1':
             if is_rocm_pytorch:
@@ -391,20 +393,30 @@
                     glob.glob('./mmcv/ops/csrc/pytorch/mps/*.mm')
             extension = CppExtension
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common'))
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common/mps'))
         elif (os.getenv('FORCE_NPU', '0') == '1'):
             print(f'Compiling {ext_name} only with CPU and NPU')
             try:
+                import importlib
+
                 from torch_npu.utils.cpp_extension import NpuExtension
+                extra_compile_args['cxx'] += [
+                    '-D__FILENAME__=\"$$(notdir $$(abspath $$<))\"'
+                ]
+                extra_compile_args['cxx'] += [
+                    '-I' + importlib.util.find_spec(
+                        'torch_npu').submodule_search_locations[0] +
+                    '/include/third_party/acl/inc'
+                ]
                 define_macros += [('MMCV_WITH_NPU', None)]
                 extension = NpuExtension
-                if parse_version(torch.__version__) <= parse_version('2.0.0'):
+                if parse_version(torch.__version__) < parse_version('2.1.0'):
                     define_macros += [('MMCV_WITH_XLA', None)]
-                if parse_version(torch.__version__) > parse_version('2.0.0'):
+                if parse_version(torch.__version__) >= parse_version('2.1.0'):
                     define_macros += [('MMCV_WITH_KPRIVATE', None)]
             except Exception:
                 raise ImportError('can not find any torch_npu')
             # src
             op_files = glob.glob('./mmcv/ops/csrc/pytorch/*.cpp') + \
                 glob.glob('./mmcv/ops/csrc/pytorch/cpu/*.cpp') + \
                 glob.glob('./mmcv/ops/csrc/common/npu/*.cpp') + \
```

### Comparing `mmcv-lite-2.1.0/tests/test_arraymisc.py` & `mmcv-lite-2.2.0/tests/test_arraymisc.py`

 * *Files identical despite different names*

### Comparing `mmcv-lite-2.1.0/tests/test_visualization.py` & `mmcv-lite-2.2.0/tests/test_visualization.py`

 * *Files identical despite different names*

