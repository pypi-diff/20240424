# Comparing `tmp/mmcv-2.0.1.tar.gz` & `tmp/mmcv-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmcv-2.0.1.tar", last modified: Thu Jun 29 07:28:50 2023, max compression
+gzip compressed data, was "dist/mmcv-2.1.0.tar", last modified: Tue Oct 17 11:30:44 2023, max compression
```

## Comparing `mmcv-2.0.1.tar` & `mmcv-2.1.0.tar`

### file list

```diff
@@ -1,565 +1,570 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-29 07:28:43.000000 mmcv-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-29 07:28:43.000000 mmcv-2.0.1/LICENSES.md
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-29 07:28:43.000000 mmcv-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-29 07:28:50.000000 mmcv-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-29 07:28:43.000000 mmcv-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    37139 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/cnn/rfsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/rfsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/rfsearch/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/rfsearch/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/rfsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    28189 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21048 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6429 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/active_rotated_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/bezier_align.py
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/bias_act.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/box_iou_quadri.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)    10564 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/chamfer_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/conv2d_gradfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/convex_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    17255 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/spconv/
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/spconv/indice.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    11437 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/mlu/
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/mps/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSDevice.h
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSLibrary.h
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSLibrary.mm
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSStream.h
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/parrots_cpp_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/parrots_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/pytorch_cuda_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/pytorch_device_registry.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/pytorch_npu_helper.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h
--rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/prettyprint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_launch.h
--rw-r--r--   0 runner    (1001) docker     (123)    37579 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/ball_query._parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/ball_query.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/ball_query_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/border_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/border_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/border_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_naive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/contour_expand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/contour_expand_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/convex_iou.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/convex_iou_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/correlation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/correlation_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/correlation_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)    84444 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/cudabind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21266 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_conv_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/focal_loss.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/focal_loss_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/gather_points.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/gather_points_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/gather_points_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/group_points.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/group_points_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/group_points_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/info.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/iou3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/iou3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/iou3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/knn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/knn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/knn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/min_area_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/min_area_polygons_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/ms_deform_attn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/nms_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/nms_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/nms_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/pixel_group_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/prroi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/psamask_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/psamask_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_pool_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/sync_bn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/sync_bn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/three_interpolate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/three_nn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/three_nn_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/three_nn_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/tin_shift.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/tin_shift_pytorch.h
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/upfirdn2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/voxelization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/voxelization_parrots.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/parrots/voxelization_pytorch.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/assign_score_withk.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/ball_query.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/bezier_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/bias_act.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/border_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/carafe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/carafe_naive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/chamfer_distance.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     3290 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/contour_expand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/convex_iou.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/correlation.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18378 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20255 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4806 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17468 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    99744 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    83983 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu
--rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    21266 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/deform_conv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/focal_loss.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/gather_points.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/group_points.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/info.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/iou3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/knn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/masked_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/min_area_polygons.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    10375 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mps/
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/nms_quadri.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/nms_rotated.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1110 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/pixel_group.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/points_in_boxes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/points_in_polygons.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/prroi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/psamask.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    55203 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/pybind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/roi_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/roi_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/scatter_points.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/spconv_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/spconv_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/sync_bn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/three_interpolate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/three_nn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/tin_shift.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/upfirdn2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/csrc/pytorch/voxelization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17467 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/diff_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/filtered_lrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8143 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/min_area_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)    14424 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/points_in_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/prroi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/riroi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/rotated_feature_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/sparse_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/sparse_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/sparse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/sparse_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/sparse_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/sparse_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/three_nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2426 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    17765 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/transforms/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/transforms/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/transforms/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)    57971 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/transforms/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24709 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/transforms/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/utils/device_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-29 07:28:43.000000 mmcv-2.0.1/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 07:28:50.000000 mmcv-2.0.1/mmcv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 07:28:43.000000 mmcv-2.0.1/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-29 07:28:50.000000 mmcv-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    20584 2023-06-29 07:28:43.000000 mmcv-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:28:50.000000 mmcv-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-29 07:28:43.000000 mmcv-2.0.1/tests/test_arraymisc.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-29 07:28:43.000000 mmcv-2.0.1/tests/test_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2023-10-17 11:30:39.000000 mmcv-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-17 11:30:39.000000 mmcv-2.1.0/LICENSES.md
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-10-17 11:30:39.000000 mmcv-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-17 11:30:44.000000 mmcv-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2023-10-17 11:30:39.000000 mmcv-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37139 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/cnn/rfsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/rfsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/rfsearch/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/rfsearch/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/rfsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23248 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28189 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6724 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/active_rotated_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/bezier_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14058 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/bias_act.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/box_iou_quadri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/chamfer_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/conv2d_gradfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/convex_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/correlation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    12955 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    12524 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23369 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    33575 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/spconv/
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/spconv/indice.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    11437 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/mlu/
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/mps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSDevice.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSLibrary.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSLibrary.mm
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSStream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/parrots_cpp_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/parrots_cuda_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/pytorch_cuda_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/pytorch_device_registry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/pytorch_npu_helper.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/prettyprint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14014 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_launch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37649 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/ball_query._parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/ball_query.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/ball_query_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/border_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/border_align_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/border_align_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_naive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/contour_expand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/contour_expand_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/convex_iou.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/convex_iou_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/correlation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/correlation_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/correlation_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    84444 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/cudabind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21266 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_conv_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/focal_loss.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/focal_loss_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/gather_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/gather_points_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/gather_points_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/group_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/group_points_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/group_points_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/info.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/iou3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/iou3d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/iou3d_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/knn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/knn_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/knn_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/min_area_polygons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/min_area_polygons_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/ms_deform_attn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/nms.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/nms_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/nms_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/nms_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/pixel_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/pixel_group_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/prroi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/psamask.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/psamask_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/psamask_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_pool_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/sync_bn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/sync_bn_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/three_interpolate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/three_nn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/three_nn_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/three_nn_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/tin_shift.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/tin_shift_pytorch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/upfirdn2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/voxelization.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/voxelization_parrots.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/parrots/voxelization_pytorch.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/assign_score_withk.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/ball_query.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/bezier_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/bias_act.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/border_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/carafe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/carafe_naive.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/chamfer_distance.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3290 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/contour_expand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/convex_iou.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/correlation.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17454 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18378 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20255 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4806 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/psamask.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18587 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17468 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    99744 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    83984 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    18325 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    19211 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     6631 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    22064 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    30436 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    11432 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    21266 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/deform_conv.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/focal_loss.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/gather_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/group_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/info.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/iou3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/knn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/masked_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/min_area_polygons.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/diff_iou_rotated_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10375 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11780 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/scatter_points_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20040 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18472 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mps/
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/nms.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/nms_quadri.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/nms_rotated.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/box_iou_rotated_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/group_points_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/points_in_polygons_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/pixel_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/points_in_boxes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/points_in_polygons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/prroi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/psamask.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    55203 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/pybind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/roi_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/roi_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/scatter_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/spconv_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/spconv_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/sync_bn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/three_interpolate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/three_nn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/tin_shift.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/upfirdn2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/csrc/pytorch/voxelization.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20328 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/diff_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/filtered_lrelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10686 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8143 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/min_area_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17158 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19306 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/points_in_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/prroi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/riroi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/rotated_feature_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14049 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/sparse_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/sparse_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/sparse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/sparse_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/sparse_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/sparse_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/three_nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2426 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17765 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/transforms/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/transforms/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57971 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/transforms/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24709 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/transforms/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/utils/device_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-10-17 11:30:39.000000 mmcv-2.1.0/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-17 11:30:43.000000 mmcv-2.1.0/mmcv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2023-10-17 11:30:44.000000 mmcv-2.1.0/mmcv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 11:30:43.000000 mmcv-2.1.0/mmcv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 11:30:43.000000 mmcv-2.1.0/mmcv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-17 11:30:43.000000 mmcv-2.1.0/mmcv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-17 11:30:43.000000 mmcv-2.1.0/mmcv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-17 11:30:39.000000 mmcv-2.1.0/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-17 11:30:44.000000 mmcv-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    21203 2023-10-17 11:30:39.000000 mmcv-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:30:44.000000 mmcv-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-10-17 11:30:39.000000 mmcv-2.1.0/tests/test_arraymisc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2023-10-17 11:30:39.000000 mmcv-2.1.0/tests/test_visualization.py
```

### Comparing `mmcv-2.0.1/LICENSE` & `mmcv-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/LICENSES.md` & `mmcv-2.1.0/LICENSES.md`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/PKG-INFO` & `mmcv-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcv
-Version: 2.0.1
+Version: 2.1.0
 Summary: OpenMMLab Computer Vision Foundation
 Home-page: https://github.com/open-mmlab/mmcv
 Author: MMCV Contributors
 Author-email: openmmlab@gmail.com
 Keywords: computer vision
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mmcv-2.0.1/README.md` & `mmcv-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/arraymisc/quantization.py` & `mmcv-2.1.0/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/__init__.py` & `mmcv-2.1.0/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/alexnet.py` & `mmcv-2.1.0/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/__init__.py` & `mmcv-2.1.0/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/activation.py` & `mmcv-2.1.0/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/context_block.py` & `mmcv-2.1.0/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/conv.py` & `mmcv-2.1.0/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `mmcv-2.1.0/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/conv_module.py` & `mmcv-2.1.0/mmcv/cnn/bricks/conv_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 
 from .activation import build_activation_layer
 from .conv import build_conv_layer
 from .norm import build_norm_layer
 from .padding import build_padding_layer
 
 
-def fast_conv_bn_eval_forward(bn: _BatchNorm, conv: nn.modules.conv._ConvNd,
-                              x: torch.Tensor):
+def efficient_conv_bn_eval_forward(bn: _BatchNorm,
+                                   conv: nn.modules.conv._ConvNd,
+                                   x: torch.Tensor):
     """
     Implementation based on https://arxiv.org/abs/2305.11624
     "Tune-Mode ConvBN Blocks For Efficient Transfer Learning"
     It leverages the associative law between convolution and affine transform,
     i.e., normalize (weight conv feature) = (normalize weight) conv feature.
     It works for Eval mode of ConvBN blocks during validation, and can be used
     for training as well. It reduces memory and computation cost.
@@ -111,17 +112,17 @@
             instead. Currently, we support ['zeros', 'circular'] with official
             implementation and ['reflect'] with our own implementation.
             Default: 'zeros'.
         order (tuple[str]): The order of conv/norm/activation layers. It is a
             sequence of "conv", "norm" and "act". Common examples are
             ("conv", "norm", "act") and ("act", "conv", "norm").
             Default: ('conv', 'norm', 'act').
-        fast_conv_bn_eval (bool): Whether use fast conv when the consecutive
-            bn is in eval mode (either training or testing), as proposed in
-            https://arxiv.org/abs/2305.11624 . Default: False.
+        efficient_conv_bn_eval (bool): Whether use efficient conv when the
+            consecutive bn is in eval mode (either training or testing), as
+            proposed in https://arxiv.org/abs/2305.11624 . Default: `False`.
     """
 
     _abbr_ = 'conv_block'
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
@@ -134,15 +135,15 @@
                  conv_cfg: Optional[Dict] = None,
                  norm_cfg: Optional[Dict] = None,
                  act_cfg: Optional[Dict] = dict(type='ReLU'),
                  inplace: bool = True,
                  with_spectral_norm: bool = False,
                  padding_mode: str = 'zeros',
                  order: tuple = ('conv', 'norm', 'act'),
-                 fast_conv_bn_eval: bool = False):
+                 efficient_conv_bn_eval: bool = False):
         super().__init__()
         assert conv_cfg is None or isinstance(conv_cfg, dict)
         assert norm_cfg is None or isinstance(norm_cfg, dict)
         assert act_cfg is None or isinstance(act_cfg, dict)
         official_padding_mode = ['zeros', 'circular']
         self.conv_cfg = conv_cfg
         self.norm_cfg = norm_cfg
@@ -205,15 +206,15 @@
             if self.with_bias:
                 if isinstance(norm, (_BatchNorm, _InstanceNorm)):
                     warnings.warn(
                         'Unnecessary conv bias before batch/instance norm')
         else:
             self.norm_name = None  # type: ignore
 
-        self.turn_on_fast_conv_bn_eval(fast_conv_bn_eval)
+        self.turn_on_efficient_conv_bn_eval(efficient_conv_bn_eval)
 
         # build activation layer
         if self.with_activation:
             act_cfg_ = act_cfg.copy()  # type: ignore
             # nn.Tanh has no 'inplace' argument
             if act_cfg_['type'] not in [
                     'Tanh', 'PReLU', 'Sigmoid', 'HSigmoid', 'Swish', 'GELU'
@@ -259,49 +260,50 @@
         layer_index = 0
         while layer_index < len(self.order):
             layer = self.order[layer_index]
             if layer == 'conv':
                 if self.with_explicit_padding:
                     x = self.padding_layer(x)
                 # if the next operation is norm and we have a norm layer in
-                # eval mode and we have enabled fast_conv_bn_eval for the conv
-                # operator, then activate the optimized forward and skip the
-                # next norm operator since it has been fused
+                # eval mode and we have enabled `efficient_conv_bn_eval` for
+                # the conv operator, then activate the optimized forward and
+                # skip the next norm operator since it has been fused
                 if layer_index + 1 < len(self.order) and \
                         self.order[layer_index + 1] == 'norm' and norm and \
                         self.with_norm and not self.norm.training and \
-                        self.fast_conv_bn_eval_forward is not None:
-                    self.conv.forward = partial(self.fast_conv_bn_eval_forward,
-                                                self.norm, self.conv)
+                        self.efficient_conv_bn_eval_forward is not None:
+                    self.conv.forward = partial(
+                        self.efficient_conv_bn_eval_forward, self.norm,
+                        self.conv)
                     layer_index += 1
                     x = self.conv(x)
                     del self.conv.forward
                 else:
                     x = self.conv(x)
             elif layer == 'norm' and norm and self.with_norm:
                 x = self.norm(x)
             elif layer == 'act' and activate and self.with_activation:
                 x = self.activate(x)
             layer_index += 1
         return x
 
-    def turn_on_fast_conv_bn_eval(self, fast_conv_bn_eval=True):
-        # fast_conv_bn_eval works for conv + bn
+    def turn_on_efficient_conv_bn_eval(self, efficient_conv_bn_eval=True):
+        # efficient_conv_bn_eval works for conv + bn
         # with `track_running_stats` option
-        if fast_conv_bn_eval and self.norm \
+        if efficient_conv_bn_eval and self.norm \
                             and isinstance(self.norm, _BatchNorm) \
                             and self.norm.track_running_stats:
-            self.fast_conv_bn_eval_forward = fast_conv_bn_eval_forward
+            self.efficient_conv_bn_eval_forward = efficient_conv_bn_eval_forward  # noqa: E501
         else:
-            self.fast_conv_bn_eval_forward = None  # type: ignore
+            self.efficient_conv_bn_eval_forward = None  # type: ignore
 
     @staticmethod
     def create_from_conv_bn(conv: torch.nn.modules.conv._ConvNd,
                             bn: torch.nn.modules.batchnorm._BatchNorm,
-                            fast_conv_bn_eval=True) -> 'ConvModule':
+                            efficient_conv_bn_eval=True) -> 'ConvModule':
         """Create a ConvModule from a conv and a bn module."""
         self = ConvModule.__new__(ConvModule)
         super(ConvModule, self).__init__()
 
         self.conv_cfg = None
         self.norm_cfg = None
         self.act_cfg = None
@@ -327,10 +329,10 @@
         self.output_padding = self.conv.output_padding
         self.groups = self.conv.groups
 
         # build normalization layers
         self.norm_name, norm = 'bn', bn
         self.add_module(self.norm_name, norm)
 
-        self.turn_on_fast_conv_bn_eval(fast_conv_bn_eval)
+        self.turn_on_efficient_conv_bn_eval(efficient_conv_bn_eval)
 
         return self
```

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/conv_ws.py` & `mmcv-2.1.0/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `mmcv-2.1.0/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/drop.py` & `mmcv-2.1.0/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/generalized_attention.py` & `mmcv-2.1.0/mmcv/cnn/bricks/generalized_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 
         if self.spatial_range >= 0:
             cur_local_constraint_map = \
                 self.local_constraint_map[:h, :w, :h_kv, :w_kv].\
                 contiguous().\
                 view(1, 1, h*w, h_kv*w_kv)
 
-            energy = energy.masked_fill_(cur_local_constraint_map,
+            energy = energy.masked_fill_(cur_local_constraint_map.bool(),
                                          float('-inf'))
 
         attention = F.softmax(energy, 3)
 
         proj_value = self.value_conv(x_kv)
         proj_value_reshape = proj_value.\
             view((n, num_heads, self.v_dim, h_kv * w_kv)).\
```

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/hsigmoid.py` & `mmcv-2.1.0/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/hswish.py` & `mmcv-2.1.0/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/non_local.py` & `mmcv-2.1.0/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/norm.py` & `mmcv-2.1.0/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/padding.py` & `mmcv-2.1.0/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/plugin.py` & `mmcv-2.1.0/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/scale.py` & `mmcv-2.1.0/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/transformer.py` & `mmcv-2.1.0/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/upsample.py` & `mmcv-2.1.0/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/bricks/wrappers.py` & `mmcv-2.1.0/mmcv/cnn/bricks/wrappers.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return NewEmptyTensorOp.apply(grad, shape), None
 
 
 @MODELS.register_module('Conv', force=True)
 class Conv2d(nn.Conv2d):
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-        if x.numel() == 0 and obsolete_torch_version(TORCH_VERSION, (1, 4)):
+        if obsolete_torch_version(TORCH_VERSION, (1, 4)) and x.numel() == 0:
             out_shape = [x.shape[0], self.out_channels]
             for i, k, p, s, d in zip(x.shape[-2:], self.kernel_size,
                                      self.padding, self.stride, self.dilation):
                 o = (i + 2 * p - (d * (k - 1) + 1)) // s + 1
                 out_shape.append(o)
             empty = NewEmptyTensorOp.apply(x, out_shape)
             if self.training:
@@ -58,15 +58,15 @@
         return super().forward(x)
 
 
 @MODELS.register_module('Conv3d', force=True)
 class Conv3d(nn.Conv3d):
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-        if x.numel() == 0 and obsolete_torch_version(TORCH_VERSION, (1, 4)):
+        if obsolete_torch_version(TORCH_VERSION, (1, 4)) and x.numel() == 0:
             out_shape = [x.shape[0], self.out_channels]
             for i, k, p, s, d in zip(x.shape[-3:], self.kernel_size,
                                      self.padding, self.stride, self.dilation):
                 o = (i + 2 * p - (d * (k - 1) + 1)) // s + 1
                 out_shape.append(o)
             empty = NewEmptyTensorOp.apply(x, out_shape)
             if self.training:
@@ -80,15 +80,15 @@
 
 
 @MODELS.register_module()
 @MODELS.register_module('deconv')
 class ConvTranspose2d(nn.ConvTranspose2d):
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-        if x.numel() == 0 and obsolete_torch_version(TORCH_VERSION, (1, 4)):
+        if obsolete_torch_version(TORCH_VERSION, (1, 4)) and x.numel() == 0:
             out_shape = [x.shape[0], self.out_channels]
             for i, k, p, s, d, op in zip(x.shape[-2:], self.kernel_size,
                                          self.padding, self.stride,
                                          self.dilation, self.output_padding):
                 out_shape.append((i - 1) * s - 2 * p + (d * (k - 1) + 1) + op)
             empty = NewEmptyTensorOp.apply(x, out_shape)
             if self.training:
@@ -102,15 +102,15 @@
 
 
 @MODELS.register_module()
 @MODELS.register_module('deconv3d')
 class ConvTranspose3d(nn.ConvTranspose3d):
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-        if x.numel() == 0 and obsolete_torch_version(TORCH_VERSION, (1, 4)):
+        if obsolete_torch_version(TORCH_VERSION, (1, 4)) and x.numel() == 0:
             out_shape = [x.shape[0], self.out_channels]
             for i, k, p, s, d, op in zip(x.shape[-3:], self.kernel_size,
                                          self.padding, self.stride,
                                          self.dilation, self.output_padding):
                 out_shape.append((i - 1) * s - 2 * p + (d * (k - 1) + 1) + op)
             empty = NewEmptyTensorOp.apply(x, out_shape)
             if self.training:
@@ -123,15 +123,15 @@
         return super().forward(x)
 
 
 class MaxPool2d(nn.MaxPool2d):
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         # PyTorch 1.9 does not support empty tensor inference yet
-        if x.numel() == 0 and obsolete_torch_version(TORCH_VERSION, (1, 9)):
+        if obsolete_torch_version(TORCH_VERSION, (1, 9)) and x.numel() == 0:
             out_shape = list(x.shape[:2])
             for i, k, p, s, d in zip(x.shape[-2:], _pair(self.kernel_size),
                                      _pair(self.padding), _pair(self.stride),
                                      _pair(self.dilation)):
                 o = (i + 2 * p - (d * (k - 1) + 1)) / s + 1
                 o = math.ceil(o) if self.ceil_mode else math.floor(o)
                 out_shape.append(o)
@@ -141,15 +141,15 @@
         return super().forward(x)
 
 
 class MaxPool3d(nn.MaxPool3d):
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         # PyTorch 1.9 does not support empty tensor inference yet
-        if x.numel() == 0 and obsolete_torch_version(TORCH_VERSION, (1, 9)):
+        if obsolete_torch_version(TORCH_VERSION, (1, 9)) and x.numel() == 0:
             out_shape = list(x.shape[:2])
             for i, k, p, s, d in zip(x.shape[-3:], _triple(self.kernel_size),
                                      _triple(self.padding),
                                      _triple(self.stride),
                                      _triple(self.dilation)):
                 o = (i + 2 * p - (d * (k - 1) + 1)) / s + 1
                 o = math.ceil(o) if self.ceil_mode else math.floor(o)
@@ -160,15 +160,15 @@
         return super().forward(x)
 
 
 class Linear(torch.nn.Linear):
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         # empty tensor forward of Linear layer is supported in Pytorch 1.6
-        if x.numel() == 0 and obsolete_torch_version(TORCH_VERSION, (1, 5)):
+        if obsolete_torch_version(TORCH_VERSION, (1, 5)) and x.numel() == 0:
             out_shape = [x.shape[0], self.out_features]
             empty = NewEmptyTensorOp.apply(x, out_shape)
             if self.training:
                 # produce dummy gradient to avoid DDP warning.
                 dummy = sum(x.view(-1)[0] for x in self.parameters()) * 0.0
                 return empty + dummy
             else:
```

### Comparing `mmcv-2.0.1/mmcv/cnn/resnet.py` & `mmcv-2.1.0/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/rfsearch/operator.py` & `mmcv-2.1.0/mmcv/cnn/rfsearch/operator.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/rfsearch/search.py` & `mmcv-2.1.0/mmcv/cnn/rfsearch/search.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/rfsearch/utils.py` & `mmcv-2.1.0/mmcv/cnn/rfsearch/utils.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/utils/flops_counter.py` & `mmcv-2.1.0/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/utils/fuse_conv_bn.py` & `mmcv-2.1.0/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/cnn/vgg.py` & `mmcv-2.1.0/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/image/__init__.py` & `mmcv-2.1.0/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/image/colorspace.py` & `mmcv-2.1.0/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/image/geometric.py` & `mmcv-2.1.0/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/image/io.py` & `mmcv-2.1.0/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/image/misc.py` & `mmcv-2.1.0/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/image/photometric.py` & `mmcv-2.1.0/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/__init__.py` & `mmcv-2.1.0/mmcv/ops/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+from mmcv.utils import IS_MLU_AVAILABLE
 from .active_rotated_filter import active_rotated_filter
 from .assign_score_withk import assign_score_withk
 from .ball_query import ball_query
 from .bbox import bbox_overlaps
 from .bezier_align import BezierAlign, bezier_align
 from .bias_act import bias_act
 from .border_align import BorderAlign, border_align
@@ -105,7 +106,13 @@
     'SparseConvTensor', 'scatter_nd', 'points_in_boxes_part',
     'points_in_boxes_cpu', 'points_in_boxes_all', 'points_in_polygons',
     'min_area_polygons', 'active_rotated_filter', 'convex_iou', 'convex_giou',
     'diff_iou_rotated_2d', 'diff_iou_rotated_3d', 'chamfer_distance',
     'PrRoIPool', 'prroi_pool', 'bias_act', 'filtered_lrelu', 'conv2d',
     'conv_transpose2d', 'filter2d', 'upsample2d', 'BezierAlign', 'bezier_align'
 ]
+
+if IS_MLU_AVAILABLE:
+    from .deform_conv import DeformConv2dPack_MLU  # noqa:F401
+    from .modulated_deform_conv import \
+        ModulatedDeformConv2dPack_MLU  # noqa:F401
+    __all__.extend(['ModulatedDeformConv2dPack_MLU', 'DeformConv2dPack_MLU'])
```

### Comparing `mmcv-2.0.1/mmcv/ops/active_rotated_filter.py` & `mmcv-2.1.0/mmcv/ops/active_rotated_filter.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/assign_score_withk.py` & `mmcv-2.1.0/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/ball_query.py` & `mmcv-2.1.0/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/bbox.py` & `mmcv-2.1.0/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/bezier_align.py` & `mmcv-2.1.0/mmcv/ops/bezier_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/bias_act.py` & `mmcv-2.1.0/mmcv/ops/bias_act.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/border_align.py` & `mmcv-2.1.0/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/box_iou_quadri.py` & `mmcv-2.1.0/mmcv/ops/box_iou_quadri.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/box_iou_rotated.py` & `mmcv-2.1.0/mmcv/ops/box_iou_rotated.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,19 @@
         else:
             ious = bboxes1.new_zeros(rows * cols)
     if not clockwise:
         flip_mat = bboxes1.new_ones(bboxes1.shape[-1])
         flip_mat[-1] = -1
         bboxes1 = bboxes1 * flip_mat
         bboxes2 = bboxes2 * flip_mat
+    if bboxes1.device.type == 'npu':
+        scale_mat = bboxes1.new_ones(bboxes1.shape[-1])
+        scale_mat[-1] = 1.0 / 0.01745329252
+        bboxes1 = bboxes1 * scale_mat
+        bboxes2 = bboxes2 * scale_mat
     bboxes1 = bboxes1.contiguous()
     bboxes2 = bboxes2.contiguous()
     ext_module.box_iou_rotated(
         bboxes1, bboxes2, ious, mode_flag=mode_flag, aligned=aligned)
     if not aligned:
         ious = ious.view(rows, cols)
     return ious
```

### Comparing `mmcv-2.0.1/mmcv/ops/carafe.py` & `mmcv-2.1.0/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/cc_attention.py` & `mmcv-2.1.0/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/chamfer_distance.py` & `mmcv-2.1.0/mmcv/ops/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/contour_expand.py` & `mmcv-2.1.0/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/conv2d_gradfix.py` & `mmcv-2.1.0/mmcv/ops/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/convex_iou.py` & `mmcv-2.1.0/mmcv/ops/convex_iou.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/corner_pool.py` & `mmcv-2.1.0/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/correlation.py` & `mmcv-2.1.0/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp` & `mmcv-2.1.0/mmcv/ops/csrc/common/box_iou_rotated_utils.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/active_rotated_filter_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/assign_score_withk_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/ball_query_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/bbox_overlaps_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/bezier_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/border_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/box_iou_quadri_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/box_iou_rotated_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/carafe_cuda_kernel.cuh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 // Copyright (c) OpenMMLab. All rights reserved
 #ifndef CARAFE_CUDA_KERNEL_CUH
 #define CARAFE_CUDA_KERNEL_CUH
 
+#include <ATen/cuda/DeviceUtils.cuh>
+
 #ifdef MMCV_USE_PARROTS
 #include "parrots_cuda_helper.hpp"
 #else
 #include "pytorch_cuda_helper.hpp"
 #endif
 
 #ifdef MMCV_WITH_HIP
@@ -52,15 +54,16 @@
   return val;
 }
 
 template <>
 __device__ __forceinline__ phalf warpReduceSum(phalf val) {
   for (int offset = WARP_SIZE / 2; offset > 0; offset /= 2)
 #ifdef MMCV_WITH_HIP
-    __PHALF(val) += __shfl_down(val, offset);
+    // Using PyTorch's macro for half support
+    __PHALF(val) += WARP_SHFL_DOWN(val, offset);
 #else
     __PHALF(val) +=
         __shfl_down_sync(FULL_MASK, __PHALF(val).operator __half(), offset);
 #endif
   return val;
 }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/carafe_naive_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/chamfer_distance_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/common_cuda_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/convex_iou_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/correlation_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/deform_conv_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/deform_roi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/diff_iou_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/furthest_point_sample_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/gather_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/group_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/iou3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/knn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/masked_conv2d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/min_area_polygons_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/modulated_deform_conv_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/ms_deform_attn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/nms_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/nms_quadri_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/nms_rotated_cuda.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/parrots_cudawarpfunction.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/points_in_boxes_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/points_in_polygons_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/prroi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/psamask_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/riroi_align_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roi_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roi_align_rotated_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roi_pool_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roiaware_pool3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/roipoint_pool3d_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/rotated_feature_align_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/scatter_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/sigmoid_focal_loss_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/softmax_focal_loss_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/spconv/indice.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/spconv/indice.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/spconv/reordering.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/stack_ball_query_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/stack_group_points_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/sync_bn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/three_interpolate_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/three_nn_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/tin_shift_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/cuda/voxelization_cuda_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp` & `mmcv-2.1.0/mmcv/ops/csrc/common/mlu/common_mlu_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSDevice.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSDevice.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSLibrary.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSLibrary.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSLibrary.mm` & `mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSLibrary.mm`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSStream.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSStream.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/mps/MPSUtils.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/mps/MPSUtils.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/parrots_cpp_helper.hpp` & `mmcv-2.1.0/mmcv/ops/csrc/common/parrots_cpp_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/parrots_cuda_helper.hpp` & `mmcv-2.1.0/mmcv/ops/csrc/common/parrots_cuda_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp` & `mmcv-2.1.0/mmcv/ops/csrc/common/pytorch_cpp_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/pytorch_device_registry.hpp` & `mmcv-2.1.0/mmcv/ops/csrc/common/pytorch_device_registry.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp` & `mmcv-2.1.0/mmcv/ops/csrc/common/pytorch_mlu_helper.hpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/paramsgrid.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/prettyprint.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/prettyprint.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/pybind11_utils.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/geometry.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/indice.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/maxpool.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/mp_helper.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/point2voxel.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/spconv/reordering.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/helper_kernel.cuh`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h` & `mmcv-2.1.0/mmcv/ops/csrc/common/utils/spconv/tensorview/tensorview.h`

 * *Files 0% similar despite different names*

```diff
@@ -315,16 +315,17 @@
 
 template <size_t MaxDim = TV_MAX_DIM>
 struct ShapeBase : public SimpleVector<int, MaxDim> {
   TV_HOST_DEVICE_INLINE ShapeBase() : SimpleVector<int, MaxDim>(){};
   TV_HOST_DEVICE_INLINE ShapeBase(std::initializer_list<int> shape)
       : SimpleVector<int, MaxDim>(shape) {}
 
-  template <typename scalar_t, template <class...> class Container>
-  ShapeBase(Container<scalar_t> shape) : SimpleVector<int, MaxDim>(shape) {}
+  // TODO: find out why this template can no be used on windows
+  // template <typename scalar_t, template <class...> class Container>
+  // ShapeBase(Container<scalar_t> shape) : SimpleVector<int, MaxDim>(shape) {}
   TV_HOST_DEVICE_INLINE ShapeBase(const ShapeBase<MaxDim> &shape)
       : SimpleVector<int, MaxDim>(shape) {}
   ShapeBase(const std::vector<int> &arr) : SimpleVector<int, MaxDim>(arr) {}
 
   ShapeBase<MaxDim> &operator=(const ShapeBase<MaxDim> &shape) = default;
   TV_HOST_DEVICE_INLINE ShapeBase<MaxDim> subshape(int start, int end) const {
 #ifdef TV_DEBUG
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/active_rotated_filter_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/assign_score_withk_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/ball_query._parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/ball_query._parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/ball_query.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/ball_query.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/bbox_overlaps_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/border_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/border_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/border_align_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/border_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/border_align_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/border_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/box_iou_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_naive.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_naive.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_naive_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_naive_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/carafe_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/carafe_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/chamfer_distance_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/contour_expand.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/contour_expand.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/contour_expand_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/convex_iou.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/convex_iou.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/convex_iou_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/correlation.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/correlation.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/correlation_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/correlation_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/correlation_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/correlation_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/cudabind.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/cudabind.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_conv.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_conv_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_conv_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_conv_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/deform_roi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/diff_iou_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/focal_loss.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/focal_loss.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/focal_loss_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/focal_loss_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/focal_loss_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/furthest_point_sample_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/fused_bias_leakyrelu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/fused_bias_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/gather_points.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/gather_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/gather_points_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/gather_points_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/gather_points_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/gather_points_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/group_points.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/group_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/group_points_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/group_points_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/group_points_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/group_points_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/info.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/info.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/iou3d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/iou3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/iou3d_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/iou3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/iou3d_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/iou3d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/knn.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/knn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/knn_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/knn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/masked_conv2d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/min_area_polygons_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/modulated_deform_conv_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/ms_deform_attn.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/ms_deform_attn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/ms_deform_attn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/nms.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/nms.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/nms_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/nms_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/nms_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/nms_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/nms_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/nms_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/pixel_group.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/pixel_group_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_boxes_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/points_in_polygons_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/prroi_pool.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/prroi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/prroi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/prroi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/psamask.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/psamask_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/psamask_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/psamask_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/psamask_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/riroi_align_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_align_rotated_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_pool.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_pool_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roi_pool_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roi_pool_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roiaware_pool3d_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/roipoint_pool3d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/rotated_feature_align_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/sync_bn.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/sync_bn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/sync_bn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/sync_bn_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/sync_bn_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/three_interpolate.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/three_interpolate.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/three_interpolate_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/three_interpolate_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/three_nn.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/three_nn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/three_nn_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/three_nn_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/tin_shift.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/tin_shift.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/tin_shift_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/upfirdn2d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/upfirdn2d_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/voxelization.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/voxelization.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/voxelization_parrots.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/voxelization_parrots.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/parrots/voxelization_pytorch.h` & `mmcv-2.1.0/mmcv/ops/csrc/parrots/voxelization_pytorch.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/assign_score_withk.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/assign_score_withk.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/ball_query.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/ball_query.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/bbox_overlaps.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 #ifdef MMCV_WITH_DIOPI
 #include <diopi/diopirt.h>
 #include <diopi/functions.h>
 #include <diopi/functions_mmcv.h>
 
+#include "csrc_dipu/base/basedef.h"
 #include "csrc_dipu/diopirt/diopirt_impl.h"
 
 using dipu::diopi_helper::toDiopiScalar;
 using dipu::diopi_helper::toDiopiTensorHandle;
 #endif
 
 void bbox_overlaps_impl(const Tensor bboxes1, const Tensor bboxes2, Tensor ious,
@@ -29,15 +30,17 @@
     bbox_overlaps_impl(bboxes1, bboxes2, ious, mode, aligned, offset);
     return;
   }
   diopiContext ctx(dipu::getCurrentDIPUStream().rawstream());
   diopiContextHandle_t ch = &ctx;
   auto bboxes2_p = toDiopiTensorHandle(bboxes2);
   auto ious_p = toDiopiTensorHandle(ious);
-  if (reinterpret_cast<void *>(diopiBboxOverlapsMmcv) != nullptr) {
+  bool is_mock_cuda = bboxes1.device().type() == dipu::DIPU_DEVICE_TYPE;
+  if (is_mock_cuda &&
+      reinterpret_cast<void *>(diopiBboxOverlapsMmcv) != nullptr) {
     auto ret = diopiBboxOverlapsMmcv(ch, ious_p, bboxes1_p, bboxes2_p, mode,
                                      offset, aligned);
     if (ret == diopiSuccess) return;
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op bbox_overlaps";
   auto bboxes1_cpu = bboxes1.cpu();
   auto bboxes2_cpu = bboxes2.cpu();
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/bezier_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/bezier_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/bias_act.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/bias_act.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/border_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/border_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/box_iou_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/carafe.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/carafe.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/carafe_naive.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/carafe_naive.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/chamfer_distance.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/chamfer_distance.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/contour_expand.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/contour_expand.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/convex_iou.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/convex_iou.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/correlation.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/correlation.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/active_rotated_filter.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/bbox_overlaps_cpu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/bezier_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/box_iou_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/box_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/modulated_deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/nms_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/psamask.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/roi_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_indice.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_maxpool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/sparse_reordering.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cpu/voxelization.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/active_rotated_filter_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/assign_score_withk_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/ball_query_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/bbox_overlaps_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/bezier_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/bias_act_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/border_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/box_iou_quadri_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/box_iou_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/carafe_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/carafe_naive_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/chamfer_distance_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/convex_iou.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/correlation_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/cudabind.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/deform_conv_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/deform_roi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/diff_iou_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/filtered_lrelu.cu`

 * *Files 0% similar despite different names*

```diff
@@ -1674,15 +1674,15 @@
               "b must be a vector with the same number of channels as x");
   TORCH_CHECK(up >= 1 && down >= 1, "up and down must be at least 1");
 
   // Figure out how much shared memory is available on the device.
   int maxSharedBytes = 0;
 #ifdef MMCV_WITH_HIP
   cudaDeviceGetAttribute(&maxSharedBytes,
-                         hipDeviceAttributeSharedMemPerBlockOptin,
+                         hipDeviceAttributeMaxSharedMemoryPerBlock,
                          x.device().index());
 #else
   AT_CUDA_CHECK(cudaDeviceGetAttribute(&maxSharedBytes,
                                        cudaDevAttrMaxSharedMemoryPerBlockOptin,
                                        x.device().index()));
 #endif
   int sharedKB = maxSharedBytes >> 10;
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/focal_loss_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/furthest_point_sample_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/fused_bias_leakyrelu_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/fused_spconv_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/gather_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/group_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/iou3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/knn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/masked_conv2d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/min_area_polygons.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/modulated_deform_conv_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/ms_deform_attn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_quadri_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/nms_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/points_in_boxes_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/points_in_polygons_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/prroi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/psamask_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/riroi_align_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_align_rotated_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roi_pool_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roiaware_pool3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/roipoint_pool3d_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/rotated_feature_align_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/scatter_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_indice.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_maxpool.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_pool_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sparse_reordering.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/spconv_ops_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/stack_ball_query_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/stack_group_points_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/sync_bn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/three_interpolate_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/three_nn_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/tin_shift_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/deform_conv.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/deform_roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/diff_iou_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/filtered_lrelu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/focal_loss.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/focal_loss.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/furthest_point_sample.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/fused_bias_leakyrelu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/fused_spconv_ops.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/gather_points.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/gather_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/group_points.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/group_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/info.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/info.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/iou3d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/iou3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/knn.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/knn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/masked_conv2d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/masked_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,17 @@
   auto xyz_impl = torch_mlu::getMluTensorImpl(xyz_contiguous);
   auto idx_impl = torch_mlu::getMluTensorImpl(idx_contiguous);
   auto new_xyz_ptr = new_xyz_impl->cnnlMalloc();
   auto xyz_ptr = xyz_impl->cnnlMalloc();
   auto idx_ptr = idx_impl->cnnlMalloc();
 
   auto handle = mluOpGetCurrentHandle();
-  mluOpBallQuery(handle, new_xyz_desc.desc(), new_xyz_ptr, xyz_desc.desc(),
-                 xyz_ptr, min_radius, max_radius, nsample, idx_desc.desc(),
-                 idx_ptr);
+  TORCH_MLUOP_CHECK(mluOpBallQuery(
+      handle, new_xyz_desc.desc(), new_xyz_ptr, xyz_desc.desc(), xyz_ptr,
+      min_radius, max_radius, nsample, idx_desc.desc(), idx_ptr));
 }
 
 void ball_query_forward_impl(int b, int n, int m, float min_radius,
                              float max_radius, int nsample,
                              const Tensor new_xyz, const Tensor xyz,
                              Tensor idx);
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,17 @@
   auto ious_impl = torch_mlu::getMluTensorImpl(ious_contiguous);
 
   auto boxes1_ptr = boxes1_impl->cnnlMalloc();
   auto boxes2_ptr = boxes2_impl->cnnlMalloc();
   auto ious_ptr = ious_impl->cnnlMalloc();
 
   CNLOG(INFO) << "Call mluOpBoxIouRotated().";
-  mluOpBoxIouRotated(handle, mode_flag, aligned, boxes1_desc.desc(), boxes1_ptr,
-                     boxes2_desc.desc(), boxes2_ptr, ious_desc.desc(),
-                     ious_ptr);
+  TORCH_MLUOP_CHECK(mluOpBoxIouRotated(
+      handle, mode_flag, aligned, boxes1_desc.desc(), boxes1_ptr,
+      boxes2_desc.desc(), boxes2_ptr, ious_desc.desc(), ious_ptr));
 }
 
 void box_iou_rotated_mlu(const Tensor boxes1, const Tensor boxes2, Tensor ious,
                          const int mode_flag, const bool aligned) {
   BoxIouRotatedMLUKernelLauncher(boxes1, boxes2, ious, mode_flag, aligned);
 }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -67,23 +67,23 @@
   auto mask_ptr = mask_impl->cnnlMalloc();
   auto output_impl = torch_mlu::getMluTensorImpl(routput_);
   auto output_ptr = output_impl->cnnlMalloc();
 
   // set op descriptor
   auto handle = mluOpGetCurrentHandle();
   mluOpCarafeDescriptor_t carafe_desc;
-  mluOpCreateCarafeDescriptor(&carafe_desc);
-  mluOpSetCarafeDescriptor(carafe_desc, input.dim(), kernel_size, group_size,
-                           scale_factor);
+  TORCH_MLUOP_CHECK(mluOpCreateCarafeDescriptor(&carafe_desc));
+  TORCH_MLUOP_CHECK(mluOpSetCarafeDescriptor(
+      carafe_desc, input.dim(), kernel_size, group_size, scale_factor));
   // launch kernel
-  mluOpCarafeForward(handle, carafe_desc, input_desc.desc(), input_ptr,
-                     mask_desc.desc(), mask_ptr, output_desc.desc(),
-                     output_ptr);
+  TORCH_MLUOP_CHECK(mluOpCarafeForward(handle, carafe_desc, input_desc.desc(),
+                                       input_ptr, mask_desc.desc(), mask_ptr,
+                                       output_desc.desc(), output_ptr));
   // destroy op descriptor
-  mluOpDestroyCarafeDescriptor(carafe_desc);
+  TORCH_MLUOP_CHECK(mluOpDestroyCarafeDescriptor(carafe_desc));
 
   // copy output from NHWC back into NCHW
   rinput.copy_(rinput_);
   output.copy_(routput_);
 }
 
 void CARAFEBackwardMLUKernelLauncher(
@@ -155,24 +155,25 @@
   auto grad_input_ptr = grad_input_impl->cnnlMalloc();
   auto grad_mask_impl = torch_mlu::getMluTensorImpl(rgrad_mask_);
   auto grad_mask_ptr = grad_mask_impl->cnnlMalloc();
 
   // set op descriptor
   auto handle = mluOpGetCurrentHandle();
   mluOpCarafeDescriptor_t carafe_desc;
-  mluOpCreateCarafeDescriptor(&carafe_desc);
-  mluOpSetCarafeDescriptor(carafe_desc, grad_output.dim(), kernel_size,
-                           group_size, scale_factor);
+  TORCH_MLUOP_CHECK(mluOpCreateCarafeDescriptor(&carafe_desc));
+  TORCH_MLUOP_CHECK(mluOpSetCarafeDescriptor(
+      carafe_desc, grad_output.dim(), kernel_size, group_size, scale_factor));
   // launch kernel
-  mluOpCarafeBackward(handle, carafe_desc, input_desc.desc(), input_ptr,
-                      mask_desc.desc(), mask_ptr, grad_output_desc.desc(),
-                      grad_output_ptr, grad_input_desc.desc(), grad_input_ptr,
-                      grad_mask_desc.desc(), grad_mask_ptr);
+  TORCH_MLUOP_CHECK(mluOpCarafeBackward(
+      handle, carafe_desc, input_desc.desc(), input_ptr, mask_desc.desc(),
+      mask_ptr, grad_output_desc.desc(), grad_output_ptr,
+      grad_input_desc.desc(), grad_input_ptr, grad_mask_desc.desc(),
+      grad_mask_ptr));
   // destroy op descriptor
-  mluOpDestroyCarafeDescriptor(carafe_desc);
+  TORCH_MLUOP_CHECK(mluOpDestroyCarafeDescriptor(carafe_desc));
 
   // copy output from NHWC back into NCHW
   grad_input.copy_(rgrad_input_);
   grad_mask.copy_(rgrad_mask_);
 }
 
 void carafe_forward_mlu(Tensor features, Tensor masks, Tensor rfeatures,
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,18 @@
   auto rois_impl = torch_mlu::getMluTensorImpl(rois_contiguous);
   auto rois_ptr = rois_impl->cnnlMalloc();
   auto output_impl = torch_mlu::getMluTensorImpl(output_contiguous);
   auto output_ptr = output_impl->cnnlMalloc();
 
   // get compute handle
   auto handle = mluOpGetCurrentHandle();
-  mluOpDeformRoiPoolForward(
+  TORCH_MLUOP_CHECK(mluOpDeformRoiPoolForward(
       handle, input_desc.desc(), input_ptr, rois_desc.desc(), rois_ptr,
       offset_real_desc, offset_ptr, pooled_height, pooled_width, spatial_scale,
-      sampling_ratio, gamma, output_desc.desc(), output_ptr);
+      sampling_ratio, gamma, output_desc.desc(), output_ptr));
 
   output.copy_(output_contiguous);
 }
 
 void DeformRoIPoolBackwardMLUKernelLauncher(
     Tensor grad_output, Tensor input, Tensor rois, Tensor offset,
     Tensor grad_input, Tensor grad_offset, int pooled_height, int pooled_width,
@@ -109,20 +109,20 @@
     grad_offset_real_desc = grad_offset_desc.desc();
     auto grad_offset_impl = torch_mlu::getMluTensorImpl(grad_offset_contiguous);
     grad_offset_ptr = grad_offset_impl->cnnlMalloc();
   }
 
   // get compute handle
   auto handle = mluOpGetCurrentHandle();
-  mluOpDeformRoiPoolBackward(
+  TORCH_MLUOP_CHECK(mluOpDeformRoiPoolBackward(
       handle, grad_output_desc.desc(), grad_output_ptr, input_desc.desc(),
       input_ptr, rois_desc.desc(), rois_ptr, offset_real_desc, offset_ptr,
       pooled_height, pooled_width, spatial_scale, sampling_ratio, gamma,
       grad_input_desc.desc(), grad_input_ptr, grad_offset_real_desc,
-      grad_offset_ptr);
+      grad_offset_ptr));
   grad_input.copy_(grad_input_);
 }
 
 void deform_roi_pool_forward_mlu(Tensor input, Tensor rois, Tensor offset,
                                  Tensor output, int pooled_height,
                                  int pooled_width, float spatial_scale,
                                  int sampling_ratio, float gamma) {
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,16 @@
   MluOpTensorDescriptor boxes_desc, output_desc;
   boxes_desc.set(boxes_);
   output_desc.set(output);
 
   // workspace
   size_t workspace_size = 0;
   auto handle = mluOpGetCurrentHandle();
-  mluOpGetNmsWorkspaceSize(handle, boxes_desc.desc(), NULL, &workspace_size);
+  TORCH_MLUOP_CHECK(mluOpGetNmsWorkspaceSize(handle, boxes_desc.desc(), NULL,
+                                             &workspace_size));
   auto workspace = at::empty(workspace_size, boxes.options().dtype(at::kByte));
 
   // get compute queue
   auto boxes_impl = torch_mlu::getMluTensorImpl(boxes_);
   auto boxes_ptr = boxes_impl->cnnlMalloc();
   auto workspace_impl = torch_mlu::getMluTensorImpl(workspace);
   auto workspace_ptr = workspace_impl->cnnlMalloc();
@@ -52,24 +53,24 @@
   const float soft_nms_sigma = 0.0;
   const float confidence_threshold = 0.0;
   const int input_layout = 0;
   const bool pad_to_max_output_size = false;
   const int max_output_size = input_box_num;
   const float offset = 0.0;
 
-  mluOpCreateNmsDescriptor(&nms_desc);
-  mluOpSetNmsDescriptor(nms_desc, box_mode, output_mode, algo, method_mode,
-                        iou_threshold, soft_nms_sigma, max_output_size,
-                        confidence_threshold, offset, input_layout,
-                        pad_to_max_output_size);
-
-  mluOpNms(handle, nms_desc, boxes_desc.desc(), boxes_ptr, NULL, NULL,
-           workspace_ptr, workspace_size, output_desc.desc(), output_ptr,
-           output_size_ptr);
-  mluOpDestroyNmsDescriptor(nms_desc);
+  TORCH_MLUOP_CHECK(mluOpCreateNmsDescriptor(&nms_desc));
+  TORCH_MLUOP_CHECK(mluOpSetNmsDescriptor(
+      nms_desc, box_mode, output_mode, algo, method_mode, iou_threshold,
+      soft_nms_sigma, max_output_size, confidence_threshold, offset,
+      input_layout, pad_to_max_output_size));
+
+  TORCH_MLUOP_CHECK(mluOpNms(handle, nms_desc, boxes_desc.desc(), boxes_ptr,
+                             NULL, NULL, workspace_ptr, workspace_size,
+                             output_desc.desc(), output_ptr, output_size_ptr));
+  TORCH_MLUOP_CHECK(mluOpDestroyNmsDescriptor(nms_desc));
 }
 
 void iou3d_nms3d_forward_mlu(const Tensor boxes, Tensor &keep, Tensor &keep_num,
                              float nms_overlap_thresh) {
   IoU3DNMS3DMLUKernelLauncher(boxes, keep, keep_num, nms_overlap_thresh);
 }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,27 @@
       break;
     default:
       layout = MLUOP_LAYOUT_ARRAY;
   }
   return layout;
 }
 
+mluOpReduceMode_t getMluOpReduceMode(const reduce_t reduce_type) {
+  const std::map<reduce_t, mluOpReduceMode_t> mapping_type = {
+      {reduce_t::MAX, MLUOP_REDUCE_DMAX},
+      {reduce_t::SUM, MLUOP_REDUCE_DSUM},
+      {reduce_t::MEAN, MLUOP_REDUCE_DMEAN}};
+  if (mapping_type.find(reduce_type) != mapping_type.end()) {
+    return mapping_type.find(reduce_type)->second;
+  } else {
+    TORCH_CHECK(false, "Unsupported reduce type: ", to_string(reduce_type));
+    return MLUOP_REDUCE_DSUM;
+  }
+}
+
 void MluOpTensorDescriptor::set(Tensor t) {
   mluOpDataType_t data_type = getMluOpDataType(t.dtype());
   mluOpTensorLayout_t layout = getMluOpSuggestLayout(t);
   int t_dim = t.dim();
   std::vector<int> dim_array;
   if (t_dim == 0) {
     dim_array.push_back(
@@ -106,15 +119,16 @@
 }
 
 void MluOpTensorDescriptor::set_desc(const at::Tensor& t,
                                      mluOpTensorLayout_t layout,
                                      mluOpDataType_t dtype,
                                      std::vector<int>& dims) {
   int dimNb = dims.size();
-  mluOpSetTensorDescriptor(desc_, layout, dtype, dimNb, dims.data());
+  TORCH_MLUOP_CHECK(
+      mluOpSetTensorDescriptor(desc_, layout, dtype, dimNb, dims.data()));
 }
 
 // Handles
 std::once_flag mmcv_mluop_init_flag;
 std::mutex mmcv_mluop_mutex;
 static std::vector<MluOpHandle> mmcv_mluop_handles;
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,14 @@
  * TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
  * SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  *************************************************************************/
 #include "mlu_common_helper.h"
 #include "pytorch_device_registry.hpp"
 #include "pytorch_mlu_helper.hpp"
 
-/*************************************************************************
- * This MACRO contains operations of simple tensor to mlu-tensor.
- * _contiguous, _desc, _impl, _ptr will be automatically generated in
- * this MACRO.
- *************************************************************************/
-#define INITIAL_MLU_PARAM_WITH_TENSOR(NAME)                         \
-  auto NAME##_contigous = torch_mlu::cnnl::ops::cnnl_contiguous(    \
-      NAME, NAME.suggest_memory_format());                          \
-  MluOpTensorDescriptor NAME##_desc;                                \
-  NAME##_desc.set(NAME##_contigous);                                \
-  auto NAME##_impl = torch_mlu::getMluTensorImpl(NAME##_contigous); \
-  auto NAME##_ptr = NAME##_impl->cnnlMalloc();
-
 Tensor MsDeformAttnForwardLauncher(const Tensor& value,
                                    const Tensor& spatial_shapes,
                                    const Tensor& level_start_index,
                                    const Tensor& sampling_loc,
                                    const Tensor& attn_weight,
                                    const int im2col_step) {
   auto handle = mluOpGetCurrentHandle();
@@ -44,20 +31,20 @@
   INITIAL_MLU_PARAM_WITH_TENSOR(output);
   INITIAL_MLU_PARAM_WITH_TENSOR(value);
   INITIAL_MLU_PARAM_WITH_TENSOR(spatial_shapes_int);
   INITIAL_MLU_PARAM_WITH_TENSOR(level_start_index_int);
   INITIAL_MLU_PARAM_WITH_TENSOR(sampling_loc);
   INITIAL_MLU_PARAM_WITH_TENSOR(attn_weight);
 
-  mluOpMsDeformAttnForward(
+  TORCH_MLUOP_CHECK(mluOpMsDeformAttnForward(
       handle, value_desc.desc(), value_ptr, spatial_shapes_int_desc.desc(),
       spatial_shapes_int_ptr, level_start_index_int_desc.desc(),
       level_start_index_int_ptr, sampling_loc_desc.desc(), sampling_loc_ptr,
       attn_weight_desc.desc(), attn_weight_ptr, im2col_step, output_desc.desc(),
-      output_ptr);
+      output_ptr));
 
   output = output.view({batch_size, num_queries, num_heads * channels});
   return output;
 }
 
 void MsDeformAttnBackwardLauncher(
     const Tensor& value, const Tensor& spatial_shapes,
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -30,16 +30,16 @@
   boxes_desc.set(boxes_);
   scores_desc.set(scores_);
   output_desc.set(output);
 
   // workspace
   size_t workspace_size = 0;
   auto handle = mluOpGetCurrentHandle();
-  mluOpGetNmsWorkspaceSize(handle, boxes_desc.desc(), scores_desc.desc(),
-                           &workspace_size);
+  TORCH_MLUOP_CHECK(mluOpGetNmsWorkspaceSize(
+      handle, boxes_desc.desc(), scores_desc.desc(), &workspace_size));
   auto workspace = at::empty(workspace_size, boxes.options().dtype(at::kByte));
 
   // get compute queue
   auto boxes_impl = torch_mlu::getMluTensorImpl(boxes_);
   auto boxes_ptr = boxes_impl->cnnlMalloc();
   auto scores_impl = torch_mlu::getMluTensorImpl(scores_);
   auto scores_ptr = scores_impl->cnnlMalloc();
@@ -58,24 +58,25 @@
   const mluOpNmsMethodMode_t method_mode = (mluOpNmsMethodMode_t)0;
   const float soft_nms_sigma = 0.0;
   const float confidence_threshold = 0.0;
   const int input_layout = 0;
   const bool pad_to_max_output_size = false;
   const int max_output_size = max_output_boxes;
 
-  mluOpCreateNmsDescriptor(&nms_desc);
-  mluOpSetNmsDescriptor(nms_desc, box_mode, output_mode, algo, method_mode,
-                        iou_threshold, soft_nms_sigma, max_output_size,
-                        confidence_threshold, (float)offset, input_layout,
-                        pad_to_max_output_size);
-
-  mluOpNms(handle, nms_desc, boxes_desc.desc(), boxes_ptr, scores_desc.desc(),
-           scores_ptr, workspace_ptr, workspace_size, output_desc.desc(),
-           output_ptr, output_size_ptr);
-  mluOpDestroyNmsDescriptor(nms_desc);
+  TORCH_MLUOP_CHECK(mluOpCreateNmsDescriptor(&nms_desc));
+  TORCH_MLUOP_CHECK(mluOpSetNmsDescriptor(
+      nms_desc, box_mode, output_mode, algo, method_mode, iou_threshold,
+      soft_nms_sigma, max_output_size, confidence_threshold, (float)offset,
+      input_layout, pad_to_max_output_size));
+
+  TORCH_MLUOP_CHECK(mluOpNms(handle, nms_desc, boxes_desc.desc(), boxes_ptr,
+                             scores_desc.desc(), scores_ptr, workspace_ptr,
+                             workspace_size, output_desc.desc(), output_ptr,
+                             output_size_ptr));
+  TORCH_MLUOP_CHECK(mluOpDestroyNmsDescriptor(nms_desc));
   int output_num = *static_cast<int *>(output_size.cpu().data_ptr());
   auto ret = output.to(boxes.options().dtype(at::kLong));
   return ret.slice(0, 0, output_num);
 }
 
 Tensor nms_mlu(Tensor boxes, Tensor scores, float iou_threshold, int offset) {
   return NMSMLUKernelLauncher(boxes, scores, iou_threshold, offset);
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/nms_rotated_mlu.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -26,28 +26,30 @@
   boxes_desc.set(boxes_);
   scores_desc.set(scores_);
   output_desc.set(output);
 
   // workspace
   size_t workspace_size = 0;
   auto handle = mluOpGetCurrentHandle();
-  mluOpGetNmsRotatedWorkspaceSize(handle, boxes_desc.desc(), &workspace_size);
+  TORCH_MLUOP_CHECK(mluOpGetNmsRotatedWorkspaceSize(handle, boxes_desc.desc(),
+                                                    &workspace_size));
   auto workspace = at::empty(workspace_size, boxes.options().dtype(at::kByte));
 
   auto boxes_impl = torch_mlu::getMluTensorImpl(boxes_);
   auto boxes_ptr = boxes_impl->cnnlMalloc();
   auto scores_impl = torch_mlu::getMluTensorImpl(scores_);
   auto scores_ptr = scores_impl->cnnlMalloc();
   auto workspace_impl = torch_mlu::getMluTensorImpl(workspace);
   auto workspace_ptr = workspace_impl->cnnlMalloc();
   auto output_impl = torch_mlu::getMluTensorImpl(output);
   auto output_ptr = output_impl->cnnlMalloc();
   auto output_size_impl = torch_mlu::getMluTensorImpl(output_size);
   auto output_size_ptr = output_size_impl->cnnlMalloc();
 
-  mluOpNmsRotated(handle, iou_threshold, boxes_desc.desc(), boxes_ptr,
-                  scores_desc.desc(), scores_ptr, workspace_ptr, workspace_size,
-                  output_desc.desc(), output_ptr, (int *)output_size_ptr);
+  TORCH_MLUOP_CHECK(mluOpNmsRotated(
+      handle, iou_threshold, boxes_desc.desc(), boxes_ptr, scores_desc.desc(),
+      scores_ptr, workspace_ptr, workspace_size, output_desc.desc(), output_ptr,
+      (int *)output_size_ptr));
   int output_num = *static_cast<int *>(output_size.cpu().data_ptr());
   auto ret = output.to(boxes.options().dtype(at::kLong));
   return ret.slice(0, 0, output_num);
 }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
   auto handle = mluOpGetCurrentHandle();
   auto x_impl = torch_mlu::getMluTensorImpl(x_tensor);
   auto x_ptr = x_impl->cnnlMalloc();
   auto y_impl = torch_mlu::getMluTensorImpl(y_tmp);
   auto y_ptr = y_impl->cnnlMalloc();
 
-  mluOpPsamaskForward(handle, psa_type, x_desc.desc(), x_ptr, h_mask, w_mask,
-                      y_desc.desc(), y_ptr);
+  TORCH_MLUOP_CHECK(mluOpPsamaskForward(handle, psa_type, x_desc.desc(), x_ptr,
+                                        h_mask, w_mask, y_desc.desc(), y_ptr));
 
   y.copy_(y_tmp);
 }
 
 void PSAMaskBackwardMLUKernelLauncher(const int psa_type, const Tensor dy,
                                       Tensor dx, const int num_,
                                       const int h_feature, const int w_feature,
@@ -63,16 +63,17 @@
 
   // get ptr of tensors
   auto dx_impl = torch_mlu::getMluTensorImpl(dx_tmp);
   auto dx_ptr = dx_impl->cnnlMalloc();
   auto dy_impl = torch_mlu::getMluTensorImpl(dy_tensor);
   auto dy_ptr = dy_impl->cnnlMalloc();
 
-  mluOpPsamaskBackward(handle, psa_type, dy_desc.desc(), dy_ptr, h_mask, w_mask,
-                       dx_tmp_desc.desc(), dx_ptr);
+  TORCH_MLUOP_CHECK(mluOpPsamaskBackward(handle, psa_type, dy_desc.desc(),
+                                         dy_ptr, h_mask, w_mask,
+                                         dx_tmp_desc.desc(), dx_ptr));
 
   dx.copy_(dx_tmp);
 }
 
 void psamask_forward_mlu(const int psa_type, const Tensor input, Tensor output,
                          const int num_, const int h_feature,
                          const int w_feature, const int h_mask,
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -44,43 +44,43 @@
 
   // get the mlu ptr
   auto self_ptr = self_impl->cnnlMalloc();
   auto rois_ptr = rois_impl->cnnlMalloc();
   auto output_ptr = output_impl->cnnlMalloc();
 
   mluOpRoiAlignForwardDescriptor_t roialign_desc;
-  mluOpCreateRoiAlignForwardDescriptor(&roialign_desc);
-  mluOpSetRoiAlignForwardDescriptor_v2(roialign_desc, aligned_height,
-                                       aligned_width, sampling_ratio,
-                                       spatial_scale, pool_mode, aligned);
+  TORCH_MLUOP_CHECK(mluOpCreateRoiAlignForwardDescriptor(&roialign_desc));
+  TORCH_MLUOP_CHECK(mluOpSetRoiAlignForwardDescriptor_v2(
+      roialign_desc, aligned_height, aligned_width, sampling_ratio,
+      spatial_scale, pool_mode, aligned));
 
   auto handle = mluOpGetCurrentHandle();
   if (pool_mode == 0) {
     auto argmax_y_contiguous =
         torch_mlu::cnnl::ops::cnnl_contiguous(argmax_y, memory_format);
     auto argmax_x_contiguous =
         torch_mlu::cnnl::ops::cnnl_contiguous(argmax_x, memory_format);
     auto argmax_x_impl = torch_mlu::getMluTensorImpl(argmax_x_contiguous);
     auto argmax_y_impl = torch_mlu::getMluTensorImpl(argmax_y_contiguous);
     auto argmax_x_ptr = argmax_x_impl->cnnlMalloc();
     auto argmax_y_ptr = argmax_y_impl->cnnlMalloc();
     argmax_y_desc.set_with_layout(argmax_x_contiguous, MLUOP_LAYOUT_NHWC);
     argmax_x_desc.set_with_layout(argmax_x_contiguous, MLUOP_LAYOUT_NHWC);
-    mluOpRoiAlignForward_v2(handle, roialign_desc, input_desc.desc(), self_ptr,
-                            rois_desc.desc(), rois_ptr, output_desc.desc(),
-                            output_ptr, argmax_x_desc.desc(), argmax_x_ptr,
-                            argmax_y_desc.desc(), argmax_y_ptr);
+    TORCH_MLUOP_CHECK(mluOpRoiAlignForward_v2(
+        handle, roialign_desc, input_desc.desc(), self_ptr, rois_desc.desc(),
+        rois_ptr, output_desc.desc(), output_ptr, argmax_x_desc.desc(),
+        argmax_x_ptr, argmax_y_desc.desc(), argmax_y_ptr));
     argmax_x.copy_(argmax_x_contiguous);
     argmax_y.copy_(argmax_y_contiguous);
   } else {
-    mluOpRoiAlignForward_v2(handle, roialign_desc, input_desc.desc(), self_ptr,
-                            rois_desc.desc(), rois_ptr, output_desc.desc(),
-                            output_ptr, NULL, NULL, NULL, NULL);
+    TORCH_MLUOP_CHECK(mluOpRoiAlignForward_v2(
+        handle, roialign_desc, input_desc.desc(), self_ptr, rois_desc.desc(),
+        rois_ptr, output_desc.desc(), output_ptr, NULL, NULL, NULL, NULL));
   }
-  mluOpDestroyRoiAlignForwardDescriptor(roialign_desc);
+  TORCH_MLUOP_CHECK(mluOpDestroyRoiAlignForwardDescriptor(roialign_desc));
   output.copy_(output_contiguous);
 }
 
 void ROIAlignBackwardMLUKernelLauncher(Tensor grad, Tensor rois,
                                        Tensor argmax_y, Tensor argmax_x,
                                        Tensor grad_input, int aligned_height,
                                        int aligned_width, float spatial_scale,
@@ -132,24 +132,24 @@
         torch_mlu::cnnl::ops::cnnl_contiguous(argmax_x, memory_format);
     auto argmax_x_impl = torch_mlu::getMluTensorImpl(argmax_x_contiguous);
     auto argmax_y_impl = torch_mlu::getMluTensorImpl(argmax_y_contiguous);
     auto argmax_x_ptr = argmax_x_impl->cnnlMalloc();
     auto argmax_y_ptr = argmax_y_impl->cnnlMalloc();
     argmax_y_desc.set_with_layout(argmax_x_contiguous, MLUOP_LAYOUT_NHWC);
     argmax_x_desc.set_with_layout(argmax_x_contiguous, MLUOP_LAYOUT_NHWC);
-    mluOpRoiAlignBackward_v2(handle, grads_desc.desc(), grad_ptr,
-                             rois_desc.desc(), rois_ptr, argmax_y_desc.desc(),
-                             argmax_x_ptr, argmax_y_desc.desc(), argmax_y_ptr,
-                             spatial_scale, sampling_ratio, aligned, pool_mode,
-                             grad_input_desc.desc(), grad_input_ptr);
+    TORCH_MLUOP_CHECK(mluOpRoiAlignBackward_v2(
+        handle, grads_desc.desc(), grad_ptr, rois_desc.desc(), rois_ptr,
+        argmax_y_desc.desc(), argmax_x_ptr, argmax_y_desc.desc(), argmax_y_ptr,
+        spatial_scale, sampling_ratio, aligned, pool_mode,
+        grad_input_desc.desc(), grad_input_ptr));
   } else {
-    mluOpRoiAlignBackward_v2(handle, grads_desc.desc(), grad_ptr,
-                             rois_desc.desc(), rois_ptr, NULL, NULL, NULL, NULL,
-                             spatial_scale, sampling_ratio, aligned, pool_mode,
-                             grad_input_desc.desc(), grad_input_ptr);
+    TORCH_MLUOP_CHECK(mluOpRoiAlignBackward_v2(
+        handle, grads_desc.desc(), grad_ptr, rois_desc.desc(), rois_ptr, NULL,
+        NULL, NULL, NULL, spatial_scale, sampling_ratio, aligned, pool_mode,
+        grad_input_desc.desc(), grad_input_ptr));
   }
   grad_input.copy_(grad_input_);
 }
 
 void roi_align_forward_mlu(Tensor input, Tensor rois, Tensor output,
                            Tensor argmax_y, Tensor argmax_x, int aligned_height,
                            int aligned_width, float spatial_scale,
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
   auto rois_impl = torch_mlu::getMluTensorImpl(rois_contiguous);
   auto rois_ptr = rois_impl->cnnlMalloc();
   auto output_impl = torch_mlu::getMluTensorImpl(output_contiguous);
   auto output_ptr = output_impl->cnnlMalloc();
 
   // get compute handle
   auto handle = mluOpGetCurrentHandle();
-  mluOpRoiAlignRotatedForward(
+  TORCH_MLUOP_CHECK(mluOpRoiAlignRotatedForward(
       handle, input_desc.desc(), input_ptr, rois_desc.desc(), rois_ptr,
       pooled_height, pooled_width, sampling_ratio, spatial_scale, aligned,
-      clockwise, output_desc.desc(), output_ptr);
+      clockwise, output_desc.desc(), output_ptr));
 
   output.copy_(output_contiguous);
 }
 
 void ROIAlignRotatedBackwardMLUKernelLauncher(
     Tensor top_grad, Tensor rois, Tensor bottom_grad, int pooled_height,
     int pooled_width, float spatial_scale, int sampling_ratio, bool aligned,
@@ -72,18 +72,18 @@
   MluOpTensorDescriptor top_grad_desc, rois_desc, bottom_grad_desc;
   top_grad_desc.set_with_layout(top_grad_, MLUOP_LAYOUT_NHWC);
   rois_desc.set(rois_contiguous);
   bottom_grad_desc.set_with_layout(bottom_grad_, MLUOP_LAYOUT_NHWC);
 
   // get compute handle
   auto handle = mluOpGetCurrentHandle();
-  mluOpRoiAlignRotatedBackward(
+  TORCH_MLUOP_CHECK(mluOpRoiAlignRotatedBackward(
       handle, top_grad_desc.desc(), top_grad_ptr, rois_desc.desc(), rois_ptr,
       pooled_height, pooled_width, sampling_ratio, spatial_scale, aligned,
-      clockwise, bottom_grad_desc.desc(), bottom_grad_ptr);
+      clockwise, bottom_grad_desc.desc(), bottom_grad_ptr));
   bottom_grad.copy_(bottom_grad_);
 }
 
 void roi_align_rotated_forward_mlu(Tensor input, Tensor rois, Tensor output,
                                    int aligned_height, int aligned_width,
                                    float spatial_scale, int sampling_ratio,
                                    bool aligned, bool clockwise) {
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
   pts_feature_desc.set(pts_feature_contiguous);
   argmax_desc.set(argmax_contiguous);
   pts_idx_of_voxels_desc.set(pts_idx_of_voxels_contiguous);
   pooled_features_desc.set(pooled_features_contiguous);
 
   // allocate extra space for workspace
   size_t workspace_size = 0;
-  mluOpGetRoiawarePool3dForwardWorkspaceSize(
+  TORCH_MLUOP_CHECK(mluOpGetRoiawarePool3dForwardWorkspaceSize(
       handle, rois_desc.desc(), pts_desc.desc(), pts_feature_desc.desc(),
-      &workspace_size);
+      &workspace_size));
 
   auto workspace = at::empty(workspace_size, rois.options().dtype(at::kByte));
   auto workspace_impl = torch_mlu::getMluTensorImpl(workspace);
   auto workspace_ptr = workspace_impl->cnnlMalloc();
 
   auto rois_impl = torch_mlu::getMluTensorImpl(rois_contiguous);
   auto pts_impl = torch_mlu::getMluTensorImpl(pts_contiguous);
@@ -65,21 +65,21 @@
   auto pts_ptr = pts_impl->cnnlMalloc();
   auto pts_feature_ptr = pts_feature_impl->cnnlMalloc();
   auto argmax_ptr = argmax_impl->cnnlMalloc();
   auto pts_idx_of_voxels_ptr = pts_idx_of_voxels_impl->cnnlMalloc();
   auto pooled_features_ptr = pooled_features_impl->cnnlMalloc();
 
   CNLOG(INFO) << "Call mluOpRoiawarePool3dForward().";
-  mluOpRoiawarePool3dForward(
+  TORCH_MLUOP_CHECK(mluOpRoiawarePool3dForward(
       handle, pool_method, boxes_num, pts_num, channels, rois_desc.desc(),
       rois_ptr, pts_desc.desc(), pts_ptr, pts_feature_desc.desc(),
       pts_feature_ptr, workspace_ptr, workspace_size, max_pts_each_voxel, out_x,
       out_y, out_z, argmax_desc.desc(), argmax_ptr,
       pts_idx_of_voxels_desc.desc(), pts_idx_of_voxels_ptr,
-      pooled_features_desc.desc(), pooled_features_ptr);
+      pooled_features_desc.desc(), pooled_features_ptr));
 }
 
 void roiaware_pool3d_forward_mlu(int boxes_num, int pts_num, int channels,
                                  int max_pts_each_voxel, int out_x, int out_y,
                                  int out_z, const Tensor rois, const Tensor pts,
                                  const Tensor pts_feature, Tensor argmax,
                                  Tensor pts_idx_of_voxels,
@@ -131,19 +131,19 @@
 
   auto pts_idx_of_voxels_ptr = pts_idx_of_voxels_impl->cnnlMalloc();
   auto argmax_ptr = argmax_impl->cnnlMalloc();
   auto grad_out_ptr = grad_out_impl->cnnlMalloc();
   auto grad_in_ptr = grad_in_impl->cnnlMalloc();
 
   CNLOG(INFO) << "Call mluOpRoiawarePool3dBackward().";
-  mluOpRoiawarePool3dBackward(
+  TORCH_MLUOP_CHECK(mluOpRoiawarePool3dBackward(
       handle, pool_method, boxes_num, out_x, out_y, out_z, channels,
       max_pts_each_voxel, pts_idx_of_voxels_desc.desc(), pts_idx_of_voxels_ptr,
       argmax_desc.desc(), argmax_ptr, grad_out_desc.desc(), grad_out_ptr,
-      grad_in_desc.desc(), grad_in_ptr);
+      grad_in_desc.desc(), grad_in_ptr));
 }
 
 void roiaware_pool3d_backward_mlu(int boxes_num, int out_x, int out_y,
                                   int out_z, int channels,
                                   int max_pts_each_voxel,
                                   const Tensor pts_idx_of_voxels,
                                   const Tensor argmax, const Tensor grad_out,
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -5,40 +5,15 @@
  * OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
  * MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
  * IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
  * CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
  * TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
  * SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
  *************************************************************************/
-#include "pytorch_device_registry.hpp"
-#include "pytorch_mlu_helper.hpp"
-
-void KernelRoiPointPool3dForward(cnrtDim3_t k_dim, cnrtFunctionType_t k_type,
-                                 cnrtQueue_t queue, const cnrtDataType_t d_type,
-                                 const int batch_size, const int pts_num,
-                                 const int boxes_num, const int feature_in_len,
-                                 const int sampled_pts_num, const void *xyz,
-                                 const void *boxes3d, const void *pts_feature,
-                                 void *pooled_features, int *pooled_empty_flag);
-
-void KernelRoiPointPool3dLargeBoxesNumForward(
-    cnrtDim3_t k_dim, cnrtFunctionType_t k_type, cnrtQueue_t queue,
-    const cnrtDataType_t d_type, const int batch_size, const int pts_num,
-    const int boxes_num, const int feature_in_len, const int sampled_pts_num,
-    const void *xyz, const void *boxes3d, const void *pts_feature,
-    void *pooled_features, int *pooled_empty_flag);
-
-// policy function
-static void policyFuncForward(cnrtDim3_t *k_dim, cnrtFunctionType_t *k_type) {
-  // start U1 task, occupy all available clusters
-  k_dim->x = torch_mlu::getDeviceAttr(cnrtAttrMcorePerCluster);
-  k_dim->y = torch_mlu::getDeviceAttr(cnrtAttrClusterCount);
-  k_dim->z = 1;
-  *k_type = CNRT_FUNC_TYPE_UNION1;
-}
+#include "mlu_common_helper.h"
 
 void RoIPointPool3dForwardMLUKernelLauncher(
     int batch_size, int pts_num, int boxes_num, int feature_in_len,
     int sampled_pts_num, const Tensor xyz, const Tensor boxes3d,
     const Tensor pts_feature, Tensor pooled_features,
     Tensor pooled_empty_flag) {
   // check datatype
@@ -94,58 +69,67 @@
   TORCH_CHECK(boxes3d.numel() < max_input_size,
               "boxes3d element num should be less than 2^31, got ",
               boxes3d.numel(), ".");
   TORCH_CHECK(pts_feature.numel() < max_input_size,
               "pts_feature element num should be less than 2^31, got ",
               pts_feature.numel(), ".");
 
-  // calculate task dimension
-  cnrtDim3_t k_dim;
-  cnrtFunctionType_t k_type;
-  policyFuncForward(&k_dim, &k_type);
-
-  // get compute queue
-  auto queue = torch_mlu::getCurQueue();
+  // set contiguous
+  auto xyz_contiguous =
+      torch_mlu::cnnl::ops::cnnl_contiguous(xyz, xyz.suggest_memory_format());
+  auto pts_feature_contiguous = torch_mlu::cnnl::ops::cnnl_contiguous(
+      pts_feature, pts_feature.suggest_memory_format());
+  auto boxes3d_contiguous = torch_mlu::cnnl::ops::cnnl_contiguous(
+      boxes3d, boxes3d.suggest_memory_format());
+  auto pooled_features_contiguous = torch_mlu::cnnl::ops::cnnl_contiguous(
+      pooled_features, pooled_features.suggest_memory_format());
+  auto pooled_empty_flag_contiguous = torch_mlu::cnnl::ops::cnnl_contiguous(
+      pooled_empty_flag, pooled_empty_flag.suggest_memory_format());
 
   // get ptr of tensors
-  // transpose points [B, N ,3] -> [3, B, N]
-  auto xyz_ = xyz.permute({2, 0, 1}).contiguous();
-  auto xyz_impl = torch_mlu::getMluTensorImpl(xyz_);
+  auto xyz_impl = torch_mlu::getMluTensorImpl(xyz_contiguous);
   auto xyz_ptr = xyz_impl->cnnlMalloc();
-  // transpose point_features [B, N, C] -> [B, C, N]
-  auto pts_feature_ = pts_feature.permute({0, 2, 1}).contiguous();
-  auto pts_feature_impl = torch_mlu::getMluTensorImpl(pts_feature_);
+  auto pts_feature_impl = torch_mlu::getMluTensorImpl(pts_feature_contiguous);
   auto pts_feature_ptr = pts_feature_impl->cnnlMalloc();
-  auto boxes3d_impl = torch_mlu::getMluTensorImpl(boxes3d);
+  auto boxes3d_impl = torch_mlu::getMluTensorImpl(boxes3d_contiguous);
   auto boxes3d_ptr = boxes3d_impl->cnnlMalloc();
-  auto pooled_features_impl = torch_mlu::getMluTensorImpl(pooled_features);
+  auto pooled_features_impl =
+      torch_mlu::getMluTensorImpl(pooled_features_contiguous);
   auto pooled_features_ptr = pooled_features_impl->cnnlMalloc();
-  auto pooled_empty_flag_impl = torch_mlu::getMluTensorImpl(pooled_empty_flag);
+  auto pooled_empty_flag_impl =
+      torch_mlu::getMluTensorImpl(pooled_empty_flag_contiguous);
   auto pooled_empty_flag_ptr = pooled_empty_flag_impl->cnnlMalloc();
 
-  // get compute dtype of input
-  cnrtDataType_t data_type = torch_mlu::toCnrtDtype(xyz_.dtype());
-
-  // launch kernel
-  if (boxes_num <= 10240) {
-    CNLOG(INFO) << "Launch Kernel MLUKernelRoiPointPool3dForward<<<" << k_dim.x
-                << ", " << k_dim.y << ", " << k_dim.z << ">>>";
-    KernelRoiPointPool3dForward(
-        k_dim, k_type, queue, data_type, batch_size, pts_num, boxes_num,
-        feature_in_len, sampled_pts_num, xyz_ptr, boxes3d_ptr, pts_feature_ptr,
-        pooled_features_ptr, (int *)pooled_empty_flag_ptr);
-  } else {
-    CNLOG(INFO)
-        << "Launch Kernel MLUKernelRoiPointPool3dLargeBoxesNumForward<<<"
-        << k_dim.x << ", " << k_dim.y << ", " << k_dim.z << ">>>";
-    KernelRoiPointPool3dLargeBoxesNumForward(
-        k_dim, k_type, queue, data_type, batch_size, pts_num, boxes_num,
-        feature_in_len, sampled_pts_num, xyz_ptr, boxes3d_ptr, pts_feature_ptr,
-        pooled_features_ptr, (int *)pooled_empty_flag_ptr);
-  }
+  // create tensor descriptors
+  MluOpTensorDescriptor xyz_desc, pts_feature_desc, boxes3d_desc,
+      pooled_features_desc, pooled_empty_flag_desc;
+  xyz_desc.set(xyz_contiguous);
+  pts_feature_desc.set(pts_feature_contiguous);
+  boxes3d_desc.set(boxes3d_contiguous);
+  pooled_features_desc.set(pooled_features_contiguous);
+  pooled_empty_flag_desc.set(pooled_empty_flag_contiguous);
+
+  // get workspace
+  size_t workspace_size = 0;
+  auto handle = mluOpGetCurrentHandle();
+  TORCH_MLUOP_CHECK(mluOpGetRoiPointPool3dWorkspaceSize(
+      handle, batch_size, pts_num, boxes_num, feature_in_len, sampled_pts_num,
+      xyz_desc.desc(), pts_feature_desc.desc(), boxes3d_desc.desc(),
+      pooled_features_desc.desc(), pooled_empty_flag_desc.desc(),
+      &workspace_size));
+
+  auto workspace = at::empty(workspace_size, xyz.options().dtype(at::kByte));
+  auto workspace_impl = torch_mlu::getMluTensorImpl(workspace);
+  auto workspace_ptr = workspace_impl->cnnlMalloc();
+  TORCH_MLUOP_CHECK(mluOpRoiPointPool3d(
+      handle, batch_size, pts_num, boxes_num, feature_in_len, sampled_pts_num,
+      xyz_desc.desc(), xyz_ptr, pts_feature_desc.desc(), pts_feature_ptr,
+      boxes3d_desc.desc(), boxes3d_ptr, workspace_ptr, workspace_size,
+      pooled_features_desc.desc(), pooled_features_ptr,
+      pooled_empty_flag_desc.desc(), (int *)pooled_empty_flag_ptr));
 }
 
 void roipoint_pool3d_forward_mlu(int batch_size, int pts_num, int boxes_num,
                                  int feature_in_len, int sampled_pts_num,
                                  const Tensor xyz, const Tensor boxes3d,
                                  const Tensor pts_feature,
                                  Tensor pooled_features,
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
   auto best_bboxes_impl = torch_mlu::getMluTensorImpl(best_bboxes_contiguous);
   auto best_bboxes_ptr = best_bboxes_impl->cnnlMalloc();
   auto output_impl = torch_mlu::getMluTensorImpl(output_contiguous);
   auto output_ptr = output_impl->cnnlMalloc();
 
   // get compute handle
   auto handle = mluOpGetCurrentHandle();
-  mluOpRotatedFeatureAlignForward(
+  TORCH_MLUOP_CHECK(mluOpRotatedFeatureAlignForward(
       handle, features_desc.desc(), features_ptr, best_bboxes_desc.desc(),
-      best_bboxes_ptr, spatial_scale, points, output_desc.desc(), output_ptr);
+      best_bboxes_ptr, spatial_scale, points, output_desc.desc(), output_ptr));
 
   output.copy_(output_contiguous);
 }
 
 void RotatedFeatureAlignBackwardMLUKernelLauncher(const Tensor top_grad,
                                                   const Tensor best_bboxes,
                                                   const float spatial_scale,
@@ -72,18 +72,18 @@
   MluOpTensorDescriptor top_grad_desc, best_bboxes_desc, bottom_grad_desc;
   top_grad_desc.set_with_layout(top_grad_, MLUOP_LAYOUT_NHWC);
   best_bboxes_desc.set(best_bboxes_contiguous);
   bottom_grad_desc.set_with_layout(bottom_grad_, MLUOP_LAYOUT_NHWC);
 
   // get compute handle
   auto handle = mluOpGetCurrentHandle();
-  mluOpRotatedFeatureAlignBackward(handle, top_grad_desc.desc(), top_grad_ptr,
-                                   best_bboxes_desc.desc(), best_bboxes_ptr,
-                                   spatial_scale, points,
-                                   bottom_grad_desc.desc(), bottom_grad_ptr);
+  TORCH_MLUOP_CHECK(mluOpRotatedFeatureAlignBackward(
+      handle, top_grad_desc.desc(), top_grad_ptr, best_bboxes_desc.desc(),
+      best_bboxes_ptr, spatial_scale, points, bottom_grad_desc.desc(),
+      bottom_grad_ptr));
   bottom_grad.copy_(bottom_grad_);
 }
 
 void rotated_feature_align_forward_mlu(const Tensor features,
                                        const Tensor best_bboxes,
                                        const float spatial_scale,
                                        const int points, Tensor output) {
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -82,39 +82,39 @@
   indiceNum_desc.set(indiceNum_contiguous);
   out_indices_desc.set(out_indices_contiguous);
   {
     mluOpTensorLayout_t layout = MLUOP_LAYOUT_ARRAY;
     mluOpDataType_t dtype = MLUOP_DTYPE_INT32;
     std::vector<int> dims;
     dims = {numAct, coorDim + 1};
-    mluOpSetTensorDescriptor(indices_desc.desc(), layout, dtype, dims.size(),
-                             dims.data());
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        indices_desc.desc(), layout, dtype, dims.size(), dims.data()));
     dims = {kernelVolume, 2, numAct};
-    mluOpSetTensorDescriptor(indicePairs_desc.desc(), layout, dtype,
-                             dims.size(), dims.data());
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        indicePairs_desc.desc(), layout, dtype, dims.size(), dims.data()));
     dims = {kernelVolume};
-    mluOpSetTensorDescriptor(indiceNum_desc.desc(), layout, dtype, dims.size(),
-                             dims.data());
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        indiceNum_desc.desc(), layout, dtype, dims.size(), dims.data()));
     dims = {out_size, coorDim + 1};
-    mluOpSetTensorDescriptor(out_indices_desc.desc(), layout, dtype,
-                             dims.size(), dims.data());
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        out_indices_desc.desc(), layout, dtype, dims.size(), dims.data()));
   }
 
   mluOpSparseConvolutionDescriptor_t sparse_conv_desc;
-  mluOpCreateSparseConvolutionDescriptor(&sparse_conv_desc);
-  mluOpSetSparseConvolutionDescriptor(
+  TORCH_MLUOP_CHECK(mluOpCreateSparseConvolutionDescriptor(&sparse_conv_desc));
+  TORCH_MLUOP_CHECK(mluOpSetSparseConvolutionDescriptor(
       sparse_conv_desc, NDim + 2, batch, padding32.data(), stride32.data(),
       dilation32.data(), input_space.data(), filter_space.data(),
-      output_space.data(), sub_m, transpose, 0);
+      output_space.data(), sub_m, transpose, 0));
 
   auto handle = mluOpGetCurrentHandle();
   size_t workspace_size = 0;
-  mluOpGetIndicePairsWorkspaceSize(
+  TORCH_MLUOP_CHECK(mluOpGetIndicePairsWorkspaceSize(
       handle, sparse_conv_desc, indices_desc.desc(), indicePairs_desc.desc(),
-      out_indices_desc.desc(), indiceNum_desc.desc(), &workspace_size);
+      out_indices_desc.desc(), indiceNum_desc.desc(), &workspace_size));
   auto indice_workspace_size =
       at::empty(workspace_size, indices.options().dtype(at::kByte));
 
   auto indices_impl = torch_mlu::getMluTensorImpl(indices_contiguous);
   auto out_indices_impl = torch_mlu::getMluTensorImpl(out_indices_contiguous);
   auto indicePairs_impl = torch_mlu::getMluTensorImpl(indicePairs_contiguous);
   auto indiceNum_impl = torch_mlu::getMluTensorImpl(indiceNum_contiguous);
@@ -123,22 +123,23 @@
 
   auto indices_ptr = indices_impl->cnnlMalloc();
   auto out_indices_ptr = out_indices_impl->cnnlMalloc();
   auto indicePairs_ptr = indicePairs_impl->cnnlMalloc();
   auto indiceNum_ptr = indiceNum_impl->cnnlMalloc();
   auto indice_workspace_ptr = indice_workspace_impl->cnnlMalloc();
 
-  mluOpGetIndicePairs(handle, sparse_conv_desc, indices_desc.desc(),
-                      indices_ptr, indice_workspace_ptr, workspace_size,
-                      indicePairs_desc.desc(), indicePairs_ptr,
-                      out_indices_desc.desc(), out_indices_ptr,
-                      indiceNum_desc.desc(), indiceNum_ptr);
+  TORCH_MLUOP_CHECK(mluOpGetIndicePairs(
+      handle, sparse_conv_desc, indices_desc.desc(), indices_ptr,
+      indice_workspace_ptr, workspace_size, indicePairs_desc.desc(),
+      indicePairs_ptr, out_indices_desc.desc(), out_indices_ptr,
+      indiceNum_desc.desc(), indiceNum_ptr));
   int num_act_out = 0;
-  mluOpGetSparseConvolutionNumActOut(sparse_conv_desc, &num_act_out);
-  mluOpDestroySparseConvolutionDescriptor(sparse_conv_desc);
+  TORCH_MLUOP_CHECK(
+      mluOpGetSparseConvolutionNumActOut(sparse_conv_desc, &num_act_out));
+  TORCH_MLUOP_CHECK(mluOpDestroySparseConvolutionDescriptor(sparse_conv_desc));
   if (!sub_m) {
     return {out_indices.slice(0, 0, num_act_out), indicePairs, indiceNum};
   } else {
     return {indices, indicePairs, indiceNum};
   }
 }
 
@@ -175,41 +176,44 @@
   {
     mluOpTensorLayout_t layout;
     mluOpDataType_t dtype;
     int dim;
     int dims[8];
 
     // features_desc
-    mluOpGetTensorDescriptor(features_desc.desc(), &layout, &dtype, &dim, dims);
-    mluOpSetTensorDescriptor(features_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype,
-                             dim, dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(features_desc.desc(), &layout,
+                                               &dtype, &dim, dims));
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        features_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
 
     // filters_desc
-    mluOpGetTensorDescriptor(filters_desc.desc(), &layout, &dtype, &dim, dims);
-    mluOpSetTensorDescriptor(filters_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype,
-                             dim, dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(filters_desc.desc(), &layout,
+                                               &dtype, &dim, dims));
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        filters_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
 
     // indice_pairs_desc
-    mluOpGetTensorDescriptor(indice_pairs_desc.desc(), &layout, &dtype, &dim,
-                             dims);
-    mluOpSetTensorDescriptor(indice_pairs_desc.desc(), MLUOP_LAYOUT_ARRAY,
-                             dtype, dim, dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(indice_pairs_desc.desc(),
+                                               &layout, &dtype, &dim, dims));
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        indice_pairs_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
 
     // output_desc
-    mluOpGetTensorDescriptor(output_desc.desc(), &layout, &dtype, &dim, dims);
-    mluOpSetTensorDescriptor(output_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim,
-                             dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(output_desc.desc(), &layout,
+                                               &dtype, &dim, dims));
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        output_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
   }
 
   auto handle = mluOpGetCurrentHandle();
   size_t workspace_size = 0;
-  mluOpGetIndiceConvolutionForwardWorkspaceSize(
+  TORCH_MLUOP_CHECK(mluOpGetIndiceConvolutionForwardWorkspaceSize(
       handle, features_desc.desc(), filters_desc.desc(),
       indice_pairs_desc.desc(), output_desc.desc(), indice_num, numActOut,
-      _inverse, _subM, &workspace_size);
+      _inverse, _subM, &workspace_size));
 
   auto workspace =
       at::empty(workspace_size, features.options().dtype(at::kByte));
 
   auto features_impl = torch_mlu::getMluTensorImpl(features_contiguous);
   auto filters_impl = torch_mlu::getMluTensorImpl(filters_contiguous);
   auto indice_pairs_impl = torch_mlu::getMluTensorImpl(indice_pairs_contiguous);
@@ -219,19 +223,19 @@
   auto filters_ptr = filters_impl->cnnlMalloc();
   auto indice_pairs_ptr = indice_pairs_impl->cnnlMalloc();
   auto workspace_ptr = workspace_impl->cnnlMalloc();
 
   //  outputs
   auto output_impl = torch_mlu::getMluTensorImpl(output);
   auto output_ptr = output_impl->cnnlMalloc();
-  mluOpIndiceConvolutionForward(
+  TORCH_MLUOP_CHECK(mluOpIndiceConvolutionForward(
       handle, features_desc.desc(), features_ptr, filters_desc.desc(),
       filters_ptr, indice_pairs_desc.desc(), indice_pairs_ptr, indice_num,
       numActOut, _inverse, _subM, workspace_ptr, workspace_size,
-      output_desc.desc(), output_ptr);
+      output_desc.desc(), output_ptr));
 
   return output;
 }
 
 std::vector<torch::Tensor> IndiceConvBackwardMLUKernelLauncher(
     torch::Tensor features, torch::Tensor filters, torch::Tensor outGrad,
     torch::Tensor indicePairs, torch::Tensor indiceNum, int64_t _inverse,
@@ -286,59 +290,61 @@
   {
     mluOpTensorLayout_t layout;
     mluOpDataType_t dtype;
     int dim;
     int dims[8];
 
     // features_desc
-    mluOpGetTensorDescriptor(features_desc.desc(), &layout, &dtype, &dim, dims);
-    mluOpSetTensorDescriptor(features_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype,
-                             dim, dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(features_desc.desc(), &layout,
+                                               &dtype, &dim, dims));
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        features_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
 
     // filters_desc
-    mluOpGetTensorDescriptor(filters_desc.desc(), &layout, &dtype, &dim, dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(filters_desc.desc(), &layout,
+                                               &dtype, &dim, dims));
     if (dim == 4) {
-      mluOpSetTensorDescriptor(filters_desc.desc(), MLUOP_LAYOUT_HWCN, dtype,
-                               dim, dims);
+      TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+          filters_desc.desc(), MLUOP_LAYOUT_HWCN, dtype, dim, dims));
     } else {
-      mluOpSetTensorDescriptor(filters_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype,
-                               dim, dims);
+      TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+          filters_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
     }
 
     // output_grad_desc
-    mluOpGetTensorDescriptor(output_grad_desc.desc(), &layout, &dtype, &dim,
-                             dims);
-    mluOpSetTensorDescriptor(output_grad_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype,
-                             dim, dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(output_grad_desc.desc(), &layout,
+                                               &dtype, &dim, dims));
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        output_grad_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
 
     // indice_pairs_desc
-    mluOpGetTensorDescriptor(indice_pairs_desc.desc(), &layout, &dtype, &dim,
-                             dims);
-    mluOpSetTensorDescriptor(indice_pairs_desc.desc(), MLUOP_LAYOUT_ARRAY,
-                             dtype, dim, dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(indice_pairs_desc.desc(),
+                                               &layout, &dtype, &dim, dims));
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        indice_pairs_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
 
     // input_grad_desc
-    mluOpGetTensorDescriptor(input_grad_desc.desc(), &layout, &dtype, &dim,
-                             dims);
-    mluOpSetTensorDescriptor(input_grad_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype,
-                             dim, dims);
+    TORCH_MLUOP_CHECK(mluOpGetTensorDescriptor(input_grad_desc.desc(), &layout,
+                                               &dtype, &dim, dims));
+    TORCH_MLUOP_CHECK(mluOpSetTensorDescriptor(
+        input_grad_desc.desc(), MLUOP_LAYOUT_ARRAY, dtype, dim, dims));
   }
 
   auto handle = mluOpGetCurrentHandle();
   size_t data_workspace_size = 0;
   mluOpGetIndiceConvolutionBackwardDataWorkspaceSize(
       handle, output_grad_desc.desc(), filters_desc.desc(),
       indice_pairs_desc.desc(), input_grad_desc.desc(), indice_num, _inverse,
       &data_workspace_size);
 
   size_t filters_workspace_size = 0;
-  mluOpGetIndiceConvolutionBackwardFilterWorkspaceSize(
+  TORCH_MLUOP_CHECK(mluOpGetIndiceConvolutionBackwardFilterWorkspaceSize(
       handle, features_desc.desc(), output_grad_desc.desc(),
       indice_pairs_desc.desc(), filters_grad_desc.desc(), indice_num, _inverse,
-      _subM, &filters_workspace_size);
+      _subM, &filters_workspace_size));
 
   auto indice_convbpdata_workspace =
       at::empty(data_workspace_size, features.options().dtype(at::kByte));
   auto indice_convbpfilter_workspace =
       at::empty(filters_workspace_size, filters.options().dtype(at::kByte));
 
   auto features_impl = torch_mlu::getMluTensorImpl(features_contiguous);
@@ -361,25 +367,25 @@
 
   // outputs
   auto input_grad_impl = torch_mlu::getMluTensorImpl(input_grad);
   auto input_grad_ptr = input_grad_impl->cnnlMalloc();
   auto filters_grad_impl = torch_mlu::getMluTensorImpl(filters_grad);
   auto filters_grad_ptr = filters_grad_impl->cnnlMalloc();
 
-  mluOpIndiceConvolutionBackwardData(
+  TORCH_MLUOP_CHECK(mluOpIndiceConvolutionBackwardData(
       handle, output_grad_desc.desc(), output_grad_ptr, filters_desc.desc(),
       filters_ptr, indice_pairs_desc.desc(), indice_pairs_ptr, indice_num,
       _inverse, _subM, indice_convbpdata_workspace_ptr, data_workspace_size,
-      input_grad_desc.desc(), input_grad_ptr);
+      input_grad_desc.desc(), input_grad_ptr));
 
-  mluOpIndiceConvolutionBackwardFilter(
+  TORCH_MLUOP_CHECK(mluOpIndiceConvolutionBackwardFilter(
       handle, features_desc.desc(), features_ptr, output_grad_desc.desc(),
       output_grad_ptr, indice_pairs_desc.desc(), indice_pairs_ptr, indice_num,
       _inverse, _subM, indice_convbpfilter_workspace_ptr,
-      filters_workspace_size, filters_grad_desc.desc(), filters_grad_ptr);
+      filters_workspace_size, filters_grad_desc.desc(), filters_grad_ptr));
 
   std::vector<torch::Tensor> result;
   result.push_back(input_grad);
   result.push_back(filters_grad);
   return result;
 }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -26,34 +26,34 @@
   unknown_desc.set(unknown_contiguous);
   known_desc.set(known_contiguous);
   dist2_desc.set(dist2_contiguous);
   idx_desc.set(idx_contiguous);
 
   auto handle = mluOpGetCurrentHandle();
   size_t workspace_size = 0;
-  mluOpGetThreeNNForwardWorkspaceSize(handle, known_desc.desc(),
-                                      &workspace_size);
+  TORCH_MLUOP_CHECK(mluOpGetThreeNNForwardWorkspaceSize(
+      handle, known_desc.desc(), &workspace_size));
   auto known_workspace =
       at::empty(workspace_size, known.options().dtype(at::kByte));
 
   auto unknown_impl = torch_mlu::getMluTensorImpl(unknown_contiguous);
   auto known_impl = torch_mlu::getMluTensorImpl(known_contiguous);
   auto dist2_impl = torch_mlu::getMluTensorImpl(dist2_contiguous);
   auto idx_impl = torch_mlu::getMluTensorImpl(idx_contiguous);
   auto workspace_impl = torch_mlu::getMluTensorImpl(known_workspace);
   auto unknown_ptr = unknown_impl->cnnlMalloc();
   auto known_ptr = known_impl->cnnlMalloc();
   auto dist2_ptr = dist2_impl->cnnlMalloc();
   auto idx_ptr = idx_impl->cnnlMalloc();
   auto workspace_ptr = workspace_impl->cnnlMalloc();
 
-  mluOpThreeNNForward(handle, unknown_desc.desc(), unknown_ptr,
-                      known_desc.desc(), known_ptr, workspace_ptr,
-                      workspace_size, dist2_desc.desc(), dist2_ptr,
-                      idx_desc.desc(), idx_ptr);
+  TORCH_MLUOP_CHECK(mluOpThreeNNForward(
+      handle, unknown_desc.desc(), unknown_ptr, known_desc.desc(), known_ptr,
+      workspace_ptr, workspace_size, dist2_desc.desc(), dist2_ptr,
+      idx_desc.desc(), idx_ptr));
 }
 
 void three_nn_forward_mlu(int b, int n, int m, const Tensor unknown,
                           const Tensor known, Tensor dist2, Tensor idx) {
   ThreeNNMLUKernelLauncher(b, n, m, unknown, known, dist2, idx);
 }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -49,31 +49,31 @@
   INITIAL_MLU_PARAM_WITH_TENSOR(coors_range_tensor);
 
   auto voxel_num_tensor = at::empty({1}, points.options().dtype(torch::kInt32));
   INITIAL_MLU_PARAM_WITH_TENSOR(voxel_num_tensor);
 
   size_t workspace_size;
   auto handle = mluOpGetCurrentHandle();
-  mluOpGetVoxelizationWorkspaceSize(
+  TORCH_MLUOP_CHECK(mluOpGetVoxelizationWorkspaceSize(
       handle, points_desc.desc(), voxel_size_tensor_desc.desc(),
       coors_range_tensor_desc.desc(), max_points, max_voxels, NDim, true,
       voxels_desc.desc(), coors_desc.desc(), num_points_per_voxel_desc.desc(),
-      voxel_num_tensor_desc.desc(), &workspace_size);
+      voxel_num_tensor_desc.desc(), &workspace_size));
   auto workspace_tensor =
       at::empty(workspace_size, points.options().dtype(at::kByte));
   INITIAL_MLU_PARAM_WITH_TENSOR(workspace_tensor);
 
-  mluOpVoxelization(handle, points_desc.desc(), points_ptr,
-                    voxel_size_tensor_desc.desc(), voxel_size_tensor_ptr,
-                    coors_range_tensor_desc.desc(), coors_range_tensor_ptr,
-                    max_points, max_voxels, NDim, true, workspace_tensor_ptr,
-                    workspace_size, voxels_desc.desc(), voxels_ptr,
-                    coors_desc.desc(), coors_ptr,
-                    num_points_per_voxel_desc.desc(), num_points_per_voxel_ptr,
-                    voxel_num_tensor_desc.desc(), voxel_num_tensor_ptr);
+  TORCH_MLUOP_CHECK(mluOpVoxelization(
+      handle, points_desc.desc(), points_ptr, voxel_size_tensor_desc.desc(),
+      voxel_size_tensor_ptr, coors_range_tensor_desc.desc(),
+      coors_range_tensor_ptr, max_points, max_voxels, NDim, true,
+      workspace_tensor_ptr, workspace_size, voxels_desc.desc(), voxels_ptr,
+      coors_desc.desc(), coors_ptr, num_points_per_voxel_desc.desc(),
+      num_points_per_voxel_ptr, voxel_num_tensor_desc.desc(),
+      voxel_num_tensor_ptr));
   auto voxel_num_cpu = voxel_num_tensor.to(at::kCPU);
   int voxel_num_int = voxel_num_cpu.data_ptr<int>()[0];
   return voxel_num_int;
 }
 
 int hard_voxelize_forward_mlu(const at::Tensor &points, at::Tensor &voxels,
                               at::Tensor &coors,
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/modulated_deform_conv.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/ms_deform_attn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/nms.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/nms.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 #ifdef MMCV_WITH_DIOPI
 #include <diopi/diopirt.h>
 #include <diopi/functions.h>
 #include <diopi/functions_mmcv.h>
 
+#include "csrc_dipu/base/basedef.h"
 #include "csrc_dipu/diopirt/diopirt_impl.h"
 
 using dipu::diopi_helper::toDiopiScalar;
 using dipu::diopi_helper::toDiopiTensorHandle;
 #endif
 
 Tensor nms_impl(Tensor boxes, Tensor scores, float iou_threshold, int offset) {
@@ -38,15 +39,16 @@
   }
   diopiContext ctx(dipu::getCurrentDIPUStream().rawstream());
   diopiContextHandle_t ch = &ctx;
   Tensor out;
   auto outp = toDiopiTensorHandle(out);
   diopiTensorHandle_t* outhandle = &outp;
   auto scores_p = toDiopiTensorHandle(scores);
-  if (reinterpret_cast<void*>(diopiNmsMmcv) != nullptr) {
+  bool is_mock_cuda = boxes.device().type() == dipu::DIPU_DEVICE_TYPE;
+  if (is_mock_cuda && reinterpret_cast<void*>(diopiNmsMmcv) != nullptr) {
     auto ret =
         diopiNmsMmcv(ch, outhandle, boxes_p, scores_p, iou_threshold, offset);
     if (ret == diopiSuccess) {
       auto tensorhandle = reinterpret_cast<Tensor*>(*outhandle);
       return *tensorhandle;
     }
   }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/nms_quadri.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/nms_quadri.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/nms_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/nms_rotated.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,21 @@
   if (dets.device().is_cuda()) {
 #ifdef MMCV_WITH_CUDA
     return nms_rotated_cuda(dets, scores, order, dets_sorted.contiguous(),
                             iou_threshold, multi_label);
 #else
     AT_ERROR("Not compiled with GPU support");
 #endif
+#ifdef MMCV_WITH_XLA
   } else if (dets.device().type() == at::kXLA) {
-#ifdef MMCV_WITH_NPU
     return nms_rotated_npu(dets, scores, labels, iou_threshold);
-#else
-    AT_ERROR("Not compiled with NPU support");
+#endif
+#ifdef MMCV_WITH_KPRIVATE
+  } else if (dets.device().type() == at::kPrivateUse1) {
+    return nms_rotated_npu(dets, scores, labels, iou_threshold);
 #endif
 #ifdef MMCV_WITH_MLU
   } else if (dets.device().type() == at::kMLU) {
     return nms_rotated_mlu(dets, scores, iou_threshold);
 #endif
   }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -16,36 +16,36 @@
   at::Tensor bboxesFP32 = bboxes2;
   at::Tensor gtboxesFP32 = bboxes1;
   if (bboxes2.size(0) < bboxes1.size(0)) {
     swap_flag = true;
     bboxesFP32 = bboxes1;
     gtboxesFP32 = bboxes2;
   }
-  if (bboxes2.scalar_type() != at::ScalarType::Float) {
-    bboxesFP32 = NPUNativeFunctions::npu_dtype_cast(bboxesFP32, at::kFloat);
-    gtboxesFP32 = NPUNativeFunctions::npu_dtype_cast(gtboxesFP32, at::kFloat);
+  if (bboxes2.scalar_type() != at::kFloat) {
+    bboxesFP32 = bboxesFP32.to(at::kFloat);
+    gtboxesFP32 = gtboxesFP32.to(at::kFloat);
   }
   c10::SmallVector<int64_t, SIZE> iousSize = {gtboxesFP32.size(0),
                                               bboxesFP32.size(0)};
   if (aligned) {
     iousSize = {gtboxesFP32.size(0), 1};
   }
-  at::Tensor iousFP32 = OpPreparation::ApplyTensor(bboxesFP32, iousSize);
+  at::Tensor iousFP32 = at::empty(iousSize, bboxesFP32.options());
   bboxesFP32 = aligned ? bboxesFP32.transpose(0, 1) : bboxesFP32;
   gtboxesFP32 = aligned ? gtboxesFP32.transpose(0, 1) : gtboxesFP32;
   OpCommand cmd;
   cmd.Name("Iou")
       .Input(bboxesFP32)
       .Input(gtboxesFP32)
       .Output(iousFP32)
       .Attr("mode", modeStr)
       .Attr("eps", (float)offset)
       .Attr("aligned", aligned)
       .Run();
-  if (bboxes2.scalar_type() != at::ScalarType::Float) {
-    iousFP32 = NPUNativeFunctions::npu_dtype_cast(iousFP32, at::kHalf);
+  if (bboxes2.scalar_type() != at::kFloat) {
+    iousFP32 = iousFP32.to(at::kHalf);
   }
   iousFP32 = swap_flag ? iousFP32.transpose(0, 1) : iousFP32;
   ious.copy_(iousFP32);
 }
 
 REGISTER_NPU_IMPL(bbox_overlaps_impl, bbox_overlaps_npu);
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -8,23 +8,21 @@
   int64_t n_class = input.size(1);
   at::Tensor target_y = at::ones_like(input);
   if (n_class == 1) {
     target_y = at::reshape(target, input.sizes());
     target_y = at::mul(target_y, -1.0);
     target_y = at::add(target_y, 1.0);
   } else {
-    target_y = at_npu::native::NPUNativeFunctions::one_hot(target, n_class);
+    target_y = at::one_hot(target, n_class);
   }
-  target_y =
-      at_npu::native::NPUNativeFunctions::npu_dtype_cast(target_y, at::kInt);
+  target_y = target_y.to(at::kInt);
   int64_t weight_size = weight.size(0);
   at::Tensor weight_y = at::ones_like(input);
   if (weight_size > 0) {
-    weight_y = at_npu::native::NPUNativeFunctions::npu_broadcast(weight,
-                                                                 input.sizes());
+    weight_y = at::broadcast_to(weight, input.sizes());
   }
   OpCommand cmd;
   string reduction = "none";
   cmd.Name("SigmoidFocalLoss")
       .Input(input)
       .Input(target_y)
       .Input(weight_y)
@@ -42,26 +40,24 @@
                                      Tensor grad_input, float gamma,
                                      float alpha) {
   int64_t n_class = input.size(1);
   at::Tensor target_y = at::ones_like(input);
   if (n_class == 1) {
     target_y = at::reshape(target, input.sizes());
   } else {
-    target_y = at_npu::native::NPUNativeFunctions::one_hot(target, n_class);
+    target_y = at::one_hot(target, n_class);
     target_y = at::mul(target_y, -1.0);
     target_y = at::add(target_y, 1.0);
   }
-  target_y =
-      at_npu::native::NPUNativeFunctions::npu_dtype_cast(target_y, at::kInt);
+  target_y = target_y.to(at::kInt);
   at::Tensor grad_up = at::ones_like(input);
   int64_t weight_size = weight.size(0);
   at::Tensor weight_y = at::ones_like(input);
   if (weight_size > 0) {
-    weight_y = at_npu::native::NPUNativeFunctions::npu_broadcast(weight,
-                                                                 input.sizes());
+    weight_y = at::broadcast_to(weight, input.sizes());
   }
   OpCommand cmd;
   string reduction = "none";
   cmd.Name("SigmoidFocalLossGrad")
       .Input(input)
       .Input(target_y)
       .Input(grad_up)
@@ -76,23 +72,20 @@
 void sigmoid_focal_loss_backward_impl(Tensor input, Tensor target,
                                       Tensor weight, Tensor grad_input,
                                       float gamma, float alpha);
 
 void softmax_focal_loss_forward_npu(Tensor input, Tensor target, Tensor weight,
                                     Tensor output, float gamma, float alpha) {
   int64_t n_class = input.size(1);
-  at::Tensor target_y =
-      at_npu::native::NPUNativeFunctions::one_hot(target, n_class);
-  target_y =
-      at_npu::native::NPUNativeFunctions::npu_dtype_cast(target_y, at::kInt);
+  at::Tensor target_y = at::one_hot(target, n_class);
+  target_y = target_y.to(at::kInt);
   int64_t weight_size = weight.size(0);
   at::Tensor weight_y = at::ones_like(input);
   if (weight_size > 0) {
-    weight_y = at_npu::native::NPUNativeFunctions::npu_broadcast(weight,
-                                                                 input.sizes());
+    weight_y = at::broadcast_to(weight, input.sizes());
   }
   at::Tensor op_output = at::ones_like(input);
   OpCommand cmd;
   string reduction = "none";
   cmd.Name("SoftmaxFocalLoss")
       .Input(input)
       .Input(target_y)
@@ -103,36 +96,32 @@
       .Attr("reduction", reduction)
       .Run();
   int64_t n_batch = input.size(0);
   c10::SmallVector<int64_t, 2> offsets = {0, 0};
   c10::SmallVector<int64_t, 2> sizes = {n_batch, 1};
   at::IntArrayRef offset = at::IntArrayRef(offsets);
   at::IntArrayRef size = at::IntArrayRef(sizes);
-  at_npu::native::NPUNativeFunctions::npu_slice_out(op_output, offset, size,
-                                                    output);
+  at_npu::native::custom_ops::npu_slice_out(op_output, offset, size, output);
 }
 
 void softmax_focal_loss_forward_impl(Tensor input, Tensor target, Tensor weight,
                                      Tensor grad_input, float gamma,
                                      float alpha);
 
 void softmax_focal_loss_backward_npu(Tensor input, Tensor target, Tensor weight,
                                      Tensor buff, Tensor grad_input,
                                      float gamma, float alpha) {
   int64_t n_class = input.size(1);
-  at::Tensor target_y =
-      at_npu::native::NPUNativeFunctions::one_hot(target, n_class);
-  target_y =
-      at_npu::native::NPUNativeFunctions::npu_dtype_cast(target_y, at::kInt);
+  at::Tensor target_y = at::one_hot(target, n_class);
+  target_y = target_y.to(at::kInt);
   at::Tensor grad_up = at::ones_like(input);
   int64_t weight_size = weight.size(0);
   at::Tensor weight_y = at::ones_like(input);
   if (weight_size > 0) {
-    weight_y = at_npu::native::NPUNativeFunctions::npu_broadcast(weight,
-                                                                 input.sizes());
+    weight_y = at::broadcast_to(weight, input.sizes());
   }
   OpCommand cmd;
   string reduction = "none";
   cmd.Name("SoftmaxFocalLossGrad")
       .Input(input)
       .Input(target_y)
       .Input(grad_up)
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,17 @@
       for (int i = 0; i < input_length; i++) {
         if (i != 1) {
           input_size_tmp[i] = 1;
         }
       }
     }
     at::Tensor bias_tmp = at::reshape(bias, input_size_tmp);
-    at::Tensor bias_ = at_npu::native::NPUNativeFunctions::npu_broadcast(
-        bias_tmp, input.sizes());
+    // at::Tensor bias_ = at_npu::native::NPUNativeFunctions::npu_broadcast(
+    //     bias_tmp, input.sizes());
+    at::Tensor bias_ = at::broadcast_to(bias_tmp, input.sizes());
     OpCommand cmd;
     cmd.Name("FusedBiasLeakyRelu")
         .Input(input)
         .Input(bias_)
         .Output(py)
         .Attr("scale", scale)
         .Attr("negative_slope", alpha)
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/points_in_polygons_npu.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #include "pytorch_npu_helper.hpp"
 
 using namespace NPU_NAME_SPACE;
 using namespace std;
 
-void gather_points_forward_npu(int b, int c, int n, int npoints,
-                               const Tensor points, const Tensor idx,
-                               Tensor out) {
-  // b, c, n, and npoints do not need to be passed into gatherv2,
-  // b, c, n, and npoints are calculated inside the operator
-  // gatherv2 operator in ascend needs to set axis to 2, batch_dims is 1
-  c10::SmallVector<int64_t, N> axis = {2};
-  int64_t batch_dims = 1;
+constexpr int32_t MAX_POLYGONS_BATCH = 2800;
 
+void points_in_polygons_npu(const Tensor points, Tensor polygons, Tensor output,
+                            const int rows, const int cols) {
+  TORCH_CHECK(
+      (polygons.sizes()[0] <= MAX_POLYGONS_BATCH),
+      "The batch of polygons tensor must be less than MAX_POLYGONS_BATCH");
+  at::Tensor trans_polygons = polygons.transpose(0, 1);
   OpCommand cmd;
-  cmd.Name("GatherV2")
-      .Input(points)
-      .Input(idx)
-      .Input(axis)
-      .Output(out)
-      .Attr("batch_dims", batch_dims)
+  at::Tensor new_trans_polygons = NpuUtils::format_contiguous(trans_polygons);
+  cmd.Name("PointsInPolygons")
+      .Input(points, (string) "points")
+      .Input(new_trans_polygons, (string) "polygons")
+      .Output(output)
       .Run();
 }
 
-void gather_points_forward_impl(int b, int c, int n, int npoints,
-                                const Tensor points, const Tensor idx,
-                                Tensor out);
+void points_in_polygons_forward_impl(const Tensor points, Tensor polygons,
+                                     Tensor output, const int rows,
+                                     const int cols);
 
-REGISTER_NPU_IMPL(gather_points_forward_impl, gather_points_forward_npu);
+REGISTER_NPU_IMPL(points_in_polygons_forward_impl, points_in_polygons_npu);
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/nms_npu.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -3,43 +3,38 @@
 using namespace NPU_NAME_SPACE;
 using namespace std;
 
 Tensor nms_npu(Tensor boxes, Tensor scores, float iou_threshold, int offset) {
   TORCH_CHECK((boxes.scalar_type() == at::ScalarType::Float),
               "The type of boxes tensor passed in nms_npu should be float");
   int64_t offset_64 = offset;
-  at::Tensor iou_threshold_y = at_npu::native::OpPreparation::ApplyTensor(
-                                   {}, boxes.options().dtype(at::kFloat), boxes)
-                                   .fill_(iou_threshold);
+  at::Tensor iou_threshold_y =
+      at::empty({}, boxes.options().dtype(at::kFloat)).fill_(iou_threshold);
   at::Tensor scores_threshold_y =
-      at_npu::native::OpPreparation::ApplyTensor(
-          {}, boxes.options().dtype(at::kFloat), boxes)
-          .fill_(0);
-  at::Tensor max_outputsize_y = at_npu::native::OpPreparation::ApplyTensor(
-                                    {}, boxes.options().dtype(at::kInt), boxes)
-                                    .fill_(boxes.size(0));
+      at::empty({}, boxes.options().dtype(at::kFloat)).fill_(0);
+  at::Tensor max_outputsize_y =
+      at::empty({}, boxes.options().dtype(at::kInt)).fill_(boxes.size(0));
+
   c10::SmallVector<int64_t, SIZE> outputsize = {boxes.size(0)};
-  at::Tensor output = at_npu::native::OpPreparation::ApplyTensor(
-                          outputsize, boxes.options().dtype(at::kInt), boxes)
-                          .fill_(-1);
+  at::Tensor output =
+      at::empty(outputsize, boxes.options().dtype(at::kInt)).fill_(-1);
   OpCommand cmd;
   cmd.Name("NonMaxSuppressionV3")
       .Input(boxes)
       .Input(scores)
       .Input(max_outputsize_y)
       .Input(iou_threshold_y)
       .Input(scores_threshold_y)
       .Attr("offset", offset_64)
       .Output(output)
       .Run();
   auto outputsizeBool = at::gt(output, -1);
-  auto outputsizeInt = outputsizeBool.to(at::ScalarType::Int);
-  auto countLen = at::sum(outputsizeInt, at::ScalarType::Int);
+  auto outputsizeInt = outputsizeBool.to(at::kInt);
+  auto countLen = at::sum(outputsizeInt, at::kInt);
   at::Tensor actual_output = output.slice(0, 0, countLen.item().toLong());
-  actual_output = at_npu::native::NPUNativeFunctions::npu_dtype_cast(
-      actual_output, at::kLong);
+  actual_output = actual_output.to(at::kLong);
   return actual_output;
 }
 
 Tensor nms_impl(Tensor boxes, Tensor scores, float iou_threshold, int offset);
 
 REGISTER_NPU_IMPL(nms_impl, nms_npu);
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 using namespace NPU_NAME_SPACE;
 
 Tensor nms_rotated_npu(const Tensor dets, const Tensor scores,
                        const Tensor labels, const float iou_threshold) {
   auto originDtype = dets.scalar_type();
   at::Tensor detsCast = dets;
   at::Tensor scoresCast = scores;
-  if (originDtype != at::ScalarType::Float) {
-    detsCast = NPUNativeFunctions::npu_dtype_cast(dets, at::kFloat);
-    scoresCast = NPUNativeFunctions::npu_dtype_cast(scores, at::kFloat);
+  if (originDtype != at::kFloat) {
+    detsCast = detsCast.to(at::kFloat);
+    scoresCast = scoresCast.to(at::kFloat);
   }
   c10::SmallVector<int64_t, SIZE> selectedIndexSize = {dets.size(0)};
-  at::Tensor selectedBox = OpPreparation::ApplyTensor(dets);
-  at::Tensor selectedIndex = OpPreparation::ApplyTensor(
-      selectedIndexSize, dets.options().dtype(at::kInt), dets);
+
+  at::Tensor selectedBox = at::empty_like(dets);
+  at::Tensor selectedIndex =
+      at::empty(selectedIndexSize, dets.options().dtype(at::kInt));
 
   c10::SmallVector<int64_t, N> output_sync_idx = {0, 1};
   OpCommand cmd;
   cmd.Sync(output_sync_idx)
       .Name("RotatedNMS")
       .Input(detsCast)
       .Input(scoresCast)
       .Input(labels)
       .Output(selectedBox)
       .Output(selectedIndex)
       .Attr("iou_threshold", (float)iou_threshold)
       .Run();
-  selectedIndex = NPUNativeFunctions::npu_dtype_cast(selectedIndex, at::kLong);
+  selectedIndex = selectedIndex.to(at::kLong);
   return selectedIndex;
 }
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 using namespace NPU_NAME_SPACE;
 using namespace std;
 
 void roi_align_forward_npu(Tensor input, Tensor rois, Tensor output,
                            Tensor argmax_y, Tensor argmax_x, int aligned_height,
                            int aligned_width, float spatial_scale,
                            int sampling_ratio, int pool_mode, bool aligned) {
+  int64_t roi_end_mode = 2;
   if (!aligned) {
     LOG(WARNING) << "The [aligned] attr in roi_align op is false";
+    roi_end_mode = 0;
   }
   int64_t aligned_height_64 = aligned_height;
   int64_t aligned_width_64 = aligned_width;
   int64_t sampling_ratio_64 = sampling_ratio;
-  int64_t roi_end_mode = 0;
   OpCommand cmd;
   cmd.Name("ROIAlign")
       .Input(input)
       .Input(rois)
       .Output(output)
       .Attr("spatial_scale", spatial_scale)
       .Attr("pooled_height", aligned_height_64)
@@ -31,17 +32,21 @@
                             Tensor argmax_x, Tensor grad_input,
                             int aligned_height, int aligned_width,
                             float spatial_scale, int sampling_ratio,
                             int pool_mode, bool aligned) {
   int64_t aligned_height_64 = aligned_height;
   int64_t aligned_width_64 = aligned_width;
   int64_t sampling_ratio_64 = sampling_ratio;
-  int64_t roi_end_mode = 0;
+  int64_t roi_end_mode = 2;
+  if (!aligned) {
+    LOG(WARNING) << "The [aligned] attr in roi_align_grad op is false";
+    roi_end_mode = 0;
+  }
   c10::SmallVector<int64_t, SIZE> xdiff_shape =
-      at_npu::native::array_to_small_vector(grad_input.sizes());
+      array_to_small_vector(grad_input.sizes());
   OpCommand cmd;
   cmd.Name("ROIAlignGrad")
       .Input(grad_output)
       .Input(rois)
       .Output(grad_input)
       .Attr("xdiff_shape", xdiff_shape)
       .Attr("pooled_width", aligned_width_64)
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 void roi_pool_forward_npu(Tensor input, Tensor rois, Tensor output,
                           Tensor argmax, int pooled_height, int pooled_width,
                           float spatial_scale) {
   int64_t pooled_height_64 = pooled_height;
   int64_t pooled_width_64 = pooled_width;
   int64_t pooled_channel = 1;
-  at::Tensor roi_actual_num = at_npu::native::OpPreparation::ApplyTensor(
-      {}, rois.options().dtype(at::kInt), rois);
+  at::Tensor roi_actual_num =
+      at::empty_like(rois, rois.options().dtype(at::kInt));
   if (input.sizes()[1] % 16 == 0) {
     OpCommand cmd;
     cmd.Name("RoiPoolingWithArgMax")
         .Input(input)
         .Input(rois)
         .Input(roi_actual_num)
         .Output(output)
@@ -46,16 +46,16 @@
 
 void roi_pool_backward_npu(Tensor grad_output, Tensor rois, Tensor argmax,
                            Tensor grad_input, int pooled_height,
                            int pooled_width, float spatial_scale) {
   int64_t pooled_height_64 = pooled_height;
   int64_t pooled_width_64 = pooled_width;
   int64_t pooled_channel = 1;
-  at::Tensor roi_actual_num = at_npu::native::OpPreparation::ApplyTensor(
-      {}, rois.options().dtype(at::kInt), rois);
+  at::Tensor roi_actual_num =
+      at::empty_like(rois, rois.options().dtype(at::kInt));
   at::Tensor x = at::ones_like(grad_input);
   OpCommand cmd;
   cmd.Name("RoiPoolingGradWithArgMax")
       .Input(grad_output)
       .Input(x)
       .Input(rois)
       .Input(roi_actual_num)
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 int hard_voxelize_forward_npu(const at::Tensor &points, at::Tensor &voxels,
                               at::Tensor &coors,
                               at::Tensor &num_points_per_voxel,
                               const std::vector<float> voxel_size,
                               const std::vector<float> coors_range,
                               const int max_points, const int max_voxels,
                               const int NDim = 3) {
-  at::Tensor voxel_num_tmp = OpPreparation::ApplyTensor(points, {1});
-  at::Tensor voxel_num = at_npu::native::NPUNativeFunctions::npu_dtype_cast(
-      voxel_num_tmp, at::kInt);
+  at::Tensor voxel_num_tmp = at::empty({1}, points.options());
+  at::Tensor voxel_num = voxel_num_tmp.to(at::kInt);
 
   at::Tensor voxel_size_cpu = at::from_blob(
       const_cast<float *>(voxel_size.data()), {3}, dtype(at::kFloat));
   at::Tensor voxel_size_npu = voxel_size_cpu.to(points.device());
 
   at::Tensor coors_range_cpu = at::from_blob(
       const_cast<float *>(coors_range.data()), {6}, dtype(at::kFloat));
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/pixel_group.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/pixel_group.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/points_in_boxes.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/points_in_boxes.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/points_in_polygons.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/points_in_polygons.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/prroi_pool.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/prroi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/psamask.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/psamask.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/pybind.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/pybind.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/riroi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/roi_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/roi_align.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include "pytorch_cpp_helper.hpp"
 #include "pytorch_device_registry.hpp"
 #ifdef MMCV_WITH_DIOPI
 #include <diopi/diopirt.h>
 #include <diopi/functions.h>
 #include <diopi/functions_mmcv.h>
 
+#include "csrc_dipu/base/basedef.h"
 #include "csrc_dipu/diopirt/diopirt_impl.h"
 
 using dipu::diopi_helper::toDiopiScalar;
 using dipu::diopi_helper::toDiopiTensorHandle;
 #endif
 
 void roi_align_forward_impl(Tensor input, Tensor rois, Tensor output,
@@ -49,15 +50,16 @@
   }
   diopiContext ctx(dipu::getCurrentDIPUStream().rawstream());
   diopiContextHandle_t ch = &ctx;
   auto rois_p = toDiopiTensorHandle(rois);
   auto out_p = toDiopiTensorHandle(output);
   auto argmax_y_p = toDiopiTensorHandle(argmax_y);
   auto argmax_x_p = toDiopiTensorHandle(argmax_x);
-  if (reinterpret_cast<void*>(diopiRoiAlignMmcv) != nullptr) {
+  bool is_mock_cuda = input.device().type() == dipu::DIPU_DEVICE_TYPE;
+  if (is_mock_cuda && reinterpret_cast<void *>(diopiRoiAlignMmcv) != nullptr) {
     auto ret = diopiRoiAlignMmcv(
         ch, out_p, argmax_y_p, argmax_x_p, input_p, rois_p, aligned_height,
         aligned_width, sampling_ratio, pool_mode, spatial_scale, aligned);
     if (ret == diopiSuccess) return;
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op roi_align_forward";
   auto input_cpu = input.cpu();
@@ -87,15 +89,17 @@
   }
   auto rois_ = toDiopiTensorHandle(rois);
   auto argmax_y_ = toDiopiTensorHandle(argmax_y);
   auto argmax_x_ = toDiopiTensorHandle(argmax_x);
   auto grad_input_ = toDiopiTensorHandle(grad_input);
   diopiContext ctx(dipu::getCurrentDIPUStream().rawstream());
   diopiContextHandle_t ch = &ctx;
-  if (reinterpret_cast<void*>(diopiRoiAlignBackwardMmcv) != nullptr) {
+  bool is_mock_cuda = grad_output.device().type() == dipu::DIPU_DEVICE_TYPE;
+  if (is_mock_cuda &&
+      reinterpret_cast<void *>(diopiRoiAlignBackwardMmcv) != nullptr) {
     auto ret = diopiRoiAlignBackwardMmcv(ch, grad_input_, grad_output_, rois_,
                                          argmax_y_, argmax_x_, aligned_height,
                                          aligned_width, sampling_ratio,
                                          pool_mode, spatial_scale, aligned);
     if (ret == diopiSuccess) return;
   }
   LOG(WARNING) << "Fallback to cpu: mmcv ext op roi_align_backward";
```

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/roi_align_rotated.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/roi_pool.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/roi_pool.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/roiaware_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/roipoint_pool3d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/rotated_feature_align.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/scatter_points.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/scatter_points.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/sparse_pool_ops.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/spconv_ops.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/spconv_ops.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/spconv_utils.h` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/spconv_utils.h`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/sync_bn.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/sync_bn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/three_interpolate.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/three_interpolate.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/three_nn.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/three_nn.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/tin_shift.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/tin_shift.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/upfirdn2d.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/csrc/pytorch/voxelization.cpp` & `mmcv-2.1.0/mmcv/ops/csrc/pytorch/voxelization.cpp`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/deform_conv.py` & `mmcv-2.1.0/mmcv/ops/deform_conv.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from mmengine.registry import MODELS
 from mmengine.utils import deprecated_api_warning
 from torch import Tensor
 from torch.autograd import Function
 from torch.autograd.function import once_differentiable
 from torch.nn.modules.utils import _pair, _single
 
+from mmcv.utils import IS_MLU_AVAILABLE
 from ..utils import ext_loader
 from .modulated_deform_conv import ModulatedDeformConv2dFunction
 
 ext_module = ext_loader.load_ext('_ext', [
     'deform_conv_forward', 'deform_conv_backward_input',
     'deform_conv_backward_parameters'
 ])
@@ -434,7 +435,67 @@
                 f'DeformConv2dPack {prefix.rstrip(".")} is upgraded to '
                 'version 2.',
                 logger='current')
 
         super()._load_from_state_dict(state_dict, prefix, local_metadata,
                                       strict, missing_keys, unexpected_keys,
                                       error_msgs)
+
+
+if IS_MLU_AVAILABLE:
+    import torchvision
+    from mmengine.utils import digit_version
+    from torchvision.ops import deform_conv2d as tv_deform_conv2d
+
+    @MODELS.register_module('DCN', force=True)
+    class DeformConv2dPack_MLU(DeformConv2d):
+        """This class is the DCN implementation of the MLU device. The MLU
+        backend support of the operator has been implemented in torchvision.
+        The mmcv registration mechanism is used for multiplexing here. The
+        torchvision implementation of DCN is called.
+        Args:
+            in_channels (int): Same as nn.Conv2d.
+            out_channels (int): Same as nn.Conv2d.
+            kernel_size (int or tuple[int]): Same as nn.Conv2d.
+            stride (int): Same as nn.Conv2d, while tuple is not supported.
+            padding (int): Same as nn.Conv2d, while tuple is not supported.
+            dilation (int): Same as nn.Conv2d, while tuple is not supported.
+            groups (int): Same as nn.Conv2d.
+            bias (bool or str): If specified as `auto`, it will be decided by
+                the norm_cfg. Bias will be set as True if norm_cfg is None,
+                otherwise False.
+            im2col_step (int): Number of samples processed by
+                im2col_cuda_kernel per call. It will work when ``batch_size``
+                > ``im2col_step``, but ``batch_size`` must be divisible by
+                ``im2col_step``. Default: 32. `New in version 1.7.2.
+                Currently not supported on MLU devices.`
+        """
+
+        def __init__(self, *args, **kwargs):
+            assert digit_version(torchvision.__version__) >= digit_version(
+                '0.10.0a0'), 'the version of torchvision should be >= 0.10.0'
+            super().__init__(*args, **kwargs)
+
+            self.conv_offset = nn.Conv2d(
+                self.in_channels,
+                self.deform_groups * 2 * self.kernel_size[0] *
+                self.kernel_size[1],
+                kernel_size=self.kernel_size,
+                stride=_pair(self.stride),
+                padding=_pair(self.padding),
+                dilation=_pair(self.dilation),
+                bias=True)
+            self.init_offset()
+
+        def init_offset(self):
+            self.conv_offset.weight.data.zero_()
+            self.conv_offset.bias.data.zero_()
+
+        def forward(self, x: Tensor) -> Tensor:  # type: ignore
+            cur_im2col_step = min(self.im2col_step, x.size(0))
+            assert (x.size(0) % cur_im2col_step
+                    ) == 0, 'batch size must be divisible by im2col_step'
+            offset = self.conv_offset(x)
+            x = x.type_as(offset)
+            weight = self.weight.type_as(x)
+            return tv_deform_conv2d(x, offset, weight, None, self.stride,
+                                    self.padding, self.dilation)
```

### Comparing `mmcv-2.0.1/mmcv/ops/deform_roi_pool.py` & `mmcv-2.1.0/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/deprecated_wrappers.py` & `mmcv-2.1.0/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/diff_iou_rotated.py` & `mmcv-2.1.0/mmcv/ops/diff_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/filtered_lrelu.py` & `mmcv-2.1.0/mmcv/ops/filtered_lrelu.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/focal_loss.py` & `mmcv-2.1.0/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/furthest_point_sample.py` & `mmcv-2.1.0/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/fused_bias_leakyrelu.py` & `mmcv-2.1.0/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/gather_points.py` & `mmcv-2.1.0/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/group_points.py` & `mmcv-2.1.0/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/info.py` & `mmcv-2.1.0/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/iou3d.py` & `mmcv-2.1.0/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/knn.py` & `mmcv-2.1.0/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/masked_conv.py` & `mmcv-2.1.0/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/merge_cells.py` & `mmcv-2.1.0/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/min_area_polygons.py` & `mmcv-2.1.0/mmcv/ops/min_area_polygons.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/modulated_deform_conv.py` & `mmcv-2.1.0/mmcv/ops/modulated_deform_conv.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from mmengine.logging import print_log
 from mmengine.registry import MODELS
 from mmengine.utils import deprecated_api_warning
 from torch.autograd import Function
 from torch.autograd.function import once_differentiable
 from torch.nn.modules.utils import _pair, _single
 
+from mmcv.utils import IS_MLU_AVAILABLE
 from ..utils import ext_loader
 
 ext_module = ext_loader.load_ext(
     '_ext',
     ['modulated_deform_conv_forward', 'modulated_deform_conv_backward'])
 
 
@@ -53,15 +54,16 @@
         _, _, kernel_h, kernel_w = weight.shape
         conv2d_bias = bias if len(bias) > 0 else None
         sort_index_fp, sort_index_bp = \
             ModulatedDeformConv2dFunction._calculate_sort_index(
                 kernel_w, kernel_h, ctx.deform_groups)
         select_offset = offset.index_select(1, sort_index_fp)
         offset_all = torch.cat([select_offset, mask], dim=1)
-        output, offset_out = torch.npu_deformable_conv2d(
+        import torch_npu
+        output, offset_out = torch_npu.npu_deformable_conv2d(
             input_tensor,
             weight,
             offset_all,
             conv2d_bias,
             kernel_size=[kernel_w, kernel_h],
             stride=[1, 1, ctx.stride[0], ctx.stride[1]],
             padding=[
@@ -354,7 +356,72 @@
                 f'ModulatedDeformConvPack {prefix.rstrip(".")} is upgraded to '
                 'version 2.',
                 logger='current')
 
         super()._load_from_state_dict(state_dict, prefix, local_metadata,
                                       strict, missing_keys, unexpected_keys,
                                       error_msgs)
+
+
+if IS_MLU_AVAILABLE:
+    import torchvision
+    from mmengine.utils import digit_version
+    from torchvision.ops import deform_conv2d as tv_deform_conv2d
+
+    @MODELS.register_module('DCNv2', force=True)
+    class ModulatedDeformConv2dPack_MLU(ModulatedDeformConv2d):
+        """This class is the DCNv2 implementation of the MLU device.
+
+        The MLU backend support of the operator has been implemented
+        in torchvision. The mmcv registration mechanism is used for
+        multiplexing here. The torchvision implementation of DCNv2 is called.
+        Args:
+            in_channels (int): Same as nn.Conv2d.
+            out_channels (int): Same as nn.Conv2d.
+            kernel_size (int or tuple[int]): Same as nn.Conv2d.
+            stride (int): Same as nn.Conv2d, while tuple is not supported.
+            padding (int): Same as nn.Conv2d, while tuple is not supported.
+            dilation (int): Same as nn.Conv2d, while tuple is not supported.
+            groups (int): Same as nn.Conv2d.
+            bias (bool or str): If specified as `auto`, it will be decided by
+                the norm_cfg. Bias will be set as True if norm_cfg is None,
+                otherwise False.
+        """
+
+        def __init__(self, *args, **kwargs):
+            assert digit_version(torchvision.__version__) >= digit_version(
+                '0.10.0a0'), 'the version of torchvision should be >= 0.10.0'
+            super().__init__(*args, **kwargs)
+            self.conv_offset = nn.Conv2d(
+                self.in_channels,
+                self.deform_groups * 3 * self.kernel_size[0] *
+                self.kernel_size[1],
+                kernel_size=self.kernel_size,
+                stride=self.stride,
+                padding=self.padding,
+                dilation=self.dilation,
+                bias=True)
+            self.init_weights()
+
+        def init_weights(self):
+            super().init_weights()
+            if hasattr(self, 'conv_offset'):
+                self.conv_offset.weight.data.zero_()
+                self.conv_offset.bias.data.zero_()
+
+        def forward(self, x):
+            out = self.conv_offset(x)
+            o1, o2, mask = torch.chunk(out, 3, dim=1)
+            offset = torch.cat((o1, o2), dim=1)
+            mask = torch.sigmoid(mask)
+            x = x.type_as(offset)
+            weight = self.weight.type_as(x)
+            mask = mask.type_as(x)
+            return tv_deform_conv2d(
+                x,
+                offset,
+                weight,
+                bias=self.bias,
+                stride=self.stride,
+                padding=self.padding,
+                dilation=self.dilation,
+                mask=mask)
```

### Comparing `mmcv-2.0.1/mmcv/ops/multi_scale_deform_attn.py` & `mmcv-2.1.0/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/nms.py` & `mmcv-2.1.0/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/pixel_group.py` & `mmcv-2.1.0/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/point_sample.py` & `mmcv-2.1.0/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/points_in_boxes.py` & `mmcv-2.1.0/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/points_in_polygons.py` & `mmcv-2.1.0/mmcv/ops/points_in_polygons.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,12 +27,15 @@
     """
     assert points.shape[1] == 2, \
         'points dimension should be 2, ' \
         f'but got unexpected shape {points.shape[1]}'
     assert polygons.shape[1] == 8, \
         'polygons dimension should be 8, ' \
         f'but got unexpected shape {polygons.shape[1]}'
-    output = torch.full([points.shape[0], polygons.shape[0]],
-                        0.).cuda().float()
+    output = torch.zeros(
+        points.shape[0],
+        polygons.shape[0],
+        dtype=torch.float32,
+        device=points.device)
     ext_module.points_in_polygons_forward(points.contiguous(),
                                           polygons.contiguous(), output)
     return output
```

### Comparing `mmcv-2.0.1/mmcv/ops/points_sampler.py` & `mmcv-2.1.0/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/prroi_pool.py` & `mmcv-2.1.0/mmcv/ops/prroi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/psa_mask.py` & `mmcv-2.1.0/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/riroi_align_rotated.py` & `mmcv-2.1.0/mmcv/ops/riroi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/roi_align.py` & `mmcv-2.1.0/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/roi_align_rotated.py` & `mmcv-2.1.0/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/roi_pool.py` & `mmcv-2.1.0/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/roiaware_pool3d.py` & `mmcv-2.1.0/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/roipoint_pool3d.py` & `mmcv-2.1.0/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/rotated_feature_align.py` & `mmcv-2.1.0/mmcv/ops/rotated_feature_align.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/saconv.py` & `mmcv-2.1.0/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/scatter_points.py` & `mmcv-2.1.0/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/sparse_conv.py` & `mmcv-2.1.0/mmcv/ops/sparse_conv.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/sparse_functional.py` & `mmcv-2.1.0/mmcv/ops/sparse_functional.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/sparse_modules.py` & `mmcv-2.1.0/mmcv/ops/sparse_modules.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/sparse_ops.py` & `mmcv-2.1.0/mmcv/ops/sparse_ops.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/sparse_pool.py` & `mmcv-2.1.0/mmcv/ops/sparse_pool.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/sparse_structure.py` & `mmcv-2.1.0/mmcv/ops/sparse_structure.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/sync_bn.py` & `mmcv-2.1.0/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/three_interpolate.py` & `mmcv-2.1.0/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/three_nn.py` & `mmcv-2.1.0/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/tin_shift.py` & `mmcv-2.1.0/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/upfirdn2d.py` & `mmcv-2.1.0/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/ops/voxelize.py` & `mmcv-2.1.0/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/transforms/__init__.py` & `mmcv-2.1.0/mmcv/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/transforms/base.py` & `mmcv-2.1.0/mmcv/transforms/base.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/transforms/formatting.py` & `mmcv-2.1.0/mmcv/transforms/formatting.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/transforms/loading.py` & `mmcv-2.1.0/mmcv/transforms/loading.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/transforms/processing.py` & `mmcv-2.1.0/mmcv/transforms/processing.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/transforms/utils.py` & `mmcv-2.1.0/mmcv/transforms/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
+import copy
 import functools
 import inspect
 import weakref
 from collections import defaultdict
 from collections.abc import Iterable
 from contextlib import contextmanager
 from typing import Callable, Union
@@ -76,15 +77,18 @@
             if hasattr(instance, '_cache'):
                 del instance._cache
             # Return function output
             return self.func(instance, *args, **kwargs)
 
     def __get__(self, obj, cls):
         self.instance_ref = weakref.ref(obj)
-        return self
+        # Return a copy to avoid multiple transform instances sharing
+        # one `cache_randomness` instance, which may cause data races
+        # in multithreading cases.
+        return copy.copy(self)
 
 
 def avoid_cache_randomness(cls):
     """Decorator that marks a data transform class (subclass of
     :class:`BaseTransform`) prohibited from caching randomness. With this
     decorator, errors will be raised in following cases:
```

### Comparing `mmcv-2.0.1/mmcv/transforms/wrappers.py` & `mmcv-2.1.0/mmcv/transforms/wrappers.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/utils/env.py` & `mmcv-2.1.0/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/utils/ext_loader.py` & `mmcv-2.1.0/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/utils/parrots_jit.py` & `mmcv-2.1.0/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/version.py` & `mmcv-2.1.0/mmcv/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '2.0.1'
+__version__ = '2.1.0'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `mmcv-2.0.1/mmcv/video/__init__.py` & `mmcv-2.1.0/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/video/io.py` & `mmcv-2.1.0/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/video/optflow.py` & `mmcv-2.1.0/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/video/processing.py` & `mmcv-2.1.0/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/visualization/color.py` & `mmcv-2.1.0/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/visualization/image.py` & `mmcv-2.1.0/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv/visualization/optflow.py` & `mmcv-2.1.0/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/mmcv.egg-info/PKG-INFO` & `mmcv-2.1.0/mmcv.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcv
-Version: 2.0.1
+Version: 2.1.0
 Summary: OpenMMLab Computer Vision Foundation
 Home-page: https://github.com/open-mmlab/mmcv
 Author: MMCV Contributors
 Author-email: openmmlab@gmail.com
 Keywords: computer vision
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mmcv-2.0.1/mmcv.egg-info/SOURCES.txt` & `mmcv-2.1.0/mmcv.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -469,14 +469,15 @@
 mmcv/ops/csrc/pytorch/cuda/upfirdn2d_kernel.cu
 mmcv/ops/csrc/pytorch/cuda/voxelization_cuda.cu
 mmcv/ops/csrc/pytorch/mlu/ball_query_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/bbox_overlaps_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/box_iou_rotated.cpp
 mmcv/ops/csrc/pytorch/mlu/carafe_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/deform_roi_pool_mlu.cpp
+mmcv/ops/csrc/pytorch/mlu/diff_iou_rotated_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/focal_loss_sigmoid_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/iou3d_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/masked_conv2d_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.cpp
 mmcv/ops/csrc/pytorch/mlu/mlu_common_helper.h
 mmcv/ops/csrc/pytorch/mlu/ms_deform_attn_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/nms_mlu.cpp
@@ -484,27 +485,31 @@
 mmcv/ops/csrc/pytorch/mlu/psamask_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roi_align_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roi_align_rotated_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roi_pool_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roiaware_pool3d_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/roipoint_pool3d_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/rotated_feature_align_mlu.cpp
+mmcv/ops/csrc/pytorch/mlu/scatter_points_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/sparse_conv_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/three_nn_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/tin_shift_mlu.cpp
 mmcv/ops/csrc/pytorch/mlu/voxelization_mlu.cpp
 mmcv/ops/csrc/pytorch/mps/bbox_overlaps_mps.mm
 mmcv/ops/csrc/pytorch/npu/active_rotated_filter_npu.cpp
 mmcv/ops/csrc/pytorch/npu/bbox_overlaps_npu.cpp
+mmcv/ops/csrc/pytorch/npu/box_iou_rotated_npu.cpp
 mmcv/ops/csrc/pytorch/npu/deform_roi_pool.cpp
 mmcv/ops/csrc/pytorch/npu/focal_loss_npu.cpp
 mmcv/ops/csrc/pytorch/npu/fused_bias_leakyrelu_npu.cpp
 mmcv/ops/csrc/pytorch/npu/gather_points_npu.cpp
+mmcv/ops/csrc/pytorch/npu/group_points_npu.cpp
 mmcv/ops/csrc/pytorch/npu/nms_npu.cpp
 mmcv/ops/csrc/pytorch/npu/nms_rotated_npu.cpp
+mmcv/ops/csrc/pytorch/npu/points_in_polygons_npu.cpp
 mmcv/ops/csrc/pytorch/npu/psa_mask_npu.cpp
 mmcv/ops/csrc/pytorch/npu/roi_align_npu.cpp
 mmcv/ops/csrc/pytorch/npu/roi_pool_npu.cpp
 mmcv/ops/csrc/pytorch/npu/voxelization_npu.cpp
 mmcv/transforms/__init__.py
 mmcv/transforms/base.py
 mmcv/transforms/builder.py
```

### Comparing `mmcv-2.0.1/setup.cfg` & `mmcv-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/setup.py` & `mmcv-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,21 +197,23 @@
         # to cxx, users also need to pass an empty list to PyTorch.
         # Since PyTorch1.8.0, it has a default value so users do not need
         # to pass an empty list anymore.
         # More details at https://github.com/pytorch/pytorch/pull/45956
         extra_compile_args = {'cxx': []}
 
         if platform.system() != 'Windows':
-            extra_compile_args['cxx'] = ['-std=c++14']
+            if parse_version(torch.__version__) <= parse_version('1.12.1'):
+                extra_compile_args['cxx'] = ['-std=c++14']
+            else:
+                extra_compile_args['cxx'] = ['-std=c++17']
         else:
-            # TODO: In Windows, C++17 is chosen to compile extensions in
-            # PyTorch2.0 , but a compile error will be reported.
-            # As a temporary solution, force the use of C++14.
-            if parse_version(torch.__version__) >= parse_version('2.0.0'):
+            if parse_version(torch.__version__) <= parse_version('1.12.1'):
                 extra_compile_args['cxx'] = ['/std:c++14']
+            else:
+                extra_compile_args['cxx'] = ['/std:c++17']
 
         include_dirs = []
         library_dirs = []
         libraries = []
 
         extra_objects = []
         extra_link_args = []
@@ -378,26 +380,32 @@
             extra_compile_args['cxx'] = ['-Wall', '-std=c++17']
             extra_compile_args['cxx'] += [
                 '-framework', 'Metal', '-framework', 'Foundation'
             ]
             extra_compile_args['cxx'] += ['-ObjC++']
             # src
             op_files = glob.glob('./mmcv/ops/csrc/pytorch/*.cpp') + \
-                glob.glob('./mmcv/ops/csrc/pytorch/cpu/*.cpp') + \
-                glob.glob('./mmcv/ops/csrc/common/mps/*.mm') + \
-                glob.glob('./mmcv/ops/csrc/pytorch/mps/*.mm')
+                glob.glob('./mmcv/ops/csrc/pytorch/cpu/*.cpp')
+            # TODO: support mps ops on torch>=2.1.0
+            if parse_version(torch.__version__) < parse_version('2.1.0'):
+                op_files += glob.glob('./mmcv/ops/csrc/common/mps/*.mm') + \
+                    glob.glob('./mmcv/ops/csrc/pytorch/mps/*.mm')
             extension = CppExtension
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common'))
             include_dirs.append(os.path.abspath('./mmcv/ops/csrc/common/mps'))
         elif (os.getenv('FORCE_NPU', '0') == '1'):
             print(f'Compiling {ext_name} only with CPU and NPU')
             try:
                 from torch_npu.utils.cpp_extension import NpuExtension
                 define_macros += [('MMCV_WITH_NPU', None)]
                 extension = NpuExtension
+                if parse_version(torch.__version__) <= parse_version('2.0.0'):
+                    define_macros += [('MMCV_WITH_XLA', None)]
+                if parse_version(torch.__version__) > parse_version('2.0.0'):
+                    define_macros += [('MMCV_WITH_KPRIVATE', None)]
             except Exception:
                 raise ImportError('can not find any torch_npu')
             # src
             op_files = glob.glob('./mmcv/ops/csrc/pytorch/*.cpp') + \
                 glob.glob('./mmcv/ops/csrc/pytorch/cpu/*.cpp') + \
                 glob.glob('./mmcv/ops/csrc/common/npu/*.cpp') + \
                 glob.glob('./mmcv/ops/csrc/pytorch/npu/*.cpp')
@@ -414,15 +422,18 @@
         # c++14 features, the argument ['std=c++14'] must be added here.
         # However, in the windows environment, some standard libraries
         # will depend on c++17 or higher. In fact, for the windows
         # environment, the compiler will choose the appropriate compiler
         # to compile those cpp files, so there is no need to add the
         # argument
         if 'nvcc' in extra_compile_args and platform.system() != 'Windows':
-            extra_compile_args['nvcc'] += ['-std=c++14']
+            if parse_version(torch.__version__) <= parse_version('1.12.1'):
+                extra_compile_args['nvcc'] += ['-std=c++14']
+            else:
+                extra_compile_args['nvcc'] += ['-std=c++17']
 
         ext_ops = extension(
             name=ext_name,
             sources=op_files,
             include_dirs=include_dirs,
             define_macros=define_macros,
             extra_objects=extra_objects,
```

### Comparing `mmcv-2.0.1/tests/test_arraymisc.py` & `mmcv-2.1.0/tests/test_arraymisc.py`

 * *Files identical despite different names*

### Comparing `mmcv-2.0.1/tests/test_visualization.py` & `mmcv-2.1.0/tests/test_visualization.py`

 * *Files identical despite different names*

