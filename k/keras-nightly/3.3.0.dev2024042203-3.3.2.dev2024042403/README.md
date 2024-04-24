# Comparing `tmp/keras_nightly-3.3.0.dev2024042203.tar.gz` & `tmp/keras_nightly-3.3.2.dev2024042403.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.0.dev2024042203.tar", last modified: Mon Apr 22 03:21:35 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.2.dev2024042403.tar", last modified: Wed Apr 24 03:21:30 2024, max compression
```

## Comparing `keras_nightly-3.3.0.dev2024042203.tar` & `keras_nightly-3.3.2.dev2024042403.tar`

### file list

```diff
@@ -1,921 +1,697 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.896886 keras_nightly-3.3.0.dev2024042203/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-22 03:21:35.896886 keras_nightly-3.3.0.dev2024042203/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.748887 keras_nightly-3.3.0.dev2024042203/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/activation_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/attention_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/base_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/conv_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/core_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/merge_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/normalization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/pooling_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/regularization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/reshaping_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/layer_benchmark/rnn_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/benchmarks/model_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/model_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/model_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/model_benchmark/bert_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/model_benchmark/image_classification_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/benchmarks/torch_ctl_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/torch_ctl_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/torch_ctl_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.752887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.756887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.760887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.764887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.768887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.772887 keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.776887 keras_nightly-3.3.0.dev2024042203/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/activations/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.780887 keras_nightly-3.3.0.dev2024042203/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/applications_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/imagenet_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.780887 keras_nightly-3.3.0.dev2024042203/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.784886 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/backend_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/compute_output_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/dtypes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/global_state_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/keras_tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/stateless_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/variables_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.788886 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/distribution_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26120 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30709 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.792887 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18006 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28024 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.796887 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26595 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    77416 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/optimizer_distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/saved_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.796887 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    47357 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.800886 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.804886 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/backup_and_restore_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/csv_logger_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/early_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/lambda_callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/learning_rate_scheduler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/model_checkpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/reduce_lr_on_plateau_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/remote_monitor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/swap_ema_weights_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/tensorboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/terminate_on_nan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.804886 keras_nightly-3.3.0.dev2024042203/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/constraints/constraints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.808886 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.808886 keras_nightly-3.3.0.dev2024042203/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/distribution/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/distribution/distribution_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.808886 keras_nightly-3.3.0.dev2024042203/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/dtype_policies/dtype_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/dtype_policies/dtype_policy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.808886 keras_nightly-3.3.0.dev2024042203/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/export/export_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/export/export_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.812886 keras_nightly-3.3.0.dev2024042203/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/initializers/constant_initializers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/initializers/random_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/initializers/random_initializers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.812886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.812886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/activation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/elu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/leaky_relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/prelu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/softmax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.816886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/additive_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/grouped_query_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/multi_head_attention_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.820886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv_transpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/depthwise_conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/separable_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/separable_conv_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.824886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24999 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    41835 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    31411 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/einsum_dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/identity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/input_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/lambda_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/masking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    63788 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.824886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/merging_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.828886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/batch_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/group_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/layer_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/spectral_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/unit_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/unit_normalization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.832886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_max_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/max_pooling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.840886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/audio_preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/category_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/center_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/discretization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/feature_space_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/hashed_crossing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/hashing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/index_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/integer_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_brightness_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_contrast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_flip_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_rotation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_translation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_zoom_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/rescaling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/resizing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/string_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/text_vectorization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.844886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/activity_regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/alpha_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/gaussian_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/gaussian_noise_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/spatial_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/spatial_dropout_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.848886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/flatten_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/permute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/repeat_vector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/reshape_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding3d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.852886 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/bidirectional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/dropout_rnn_cell_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/gru_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/simple_rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/stacked_rnn_cells_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/time_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/time_distributed_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.852886 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.856886 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.856886 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/json_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/legacy_h5_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.856886 keras_nightly-3.3.0.dev2024042203/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/losses/loss_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/losses/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/losses/losses_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.860886 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/accuracy_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/confusion_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/f_score_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/hinge_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/iou_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/metric_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/probabilistic_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/reduction_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/metrics/regression_metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.864886 keras_nightly-3.3.0.dev2024042203/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/cloning_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/functional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    24695 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/sequential_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/variable_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/models/variable_mapping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.868886 keras_nightly-3.3.0.dev2024042203/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/core_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/function_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    31485 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    19959 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/linalg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/math_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    64046 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    83662 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/nn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   194898 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)   284656 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/numpy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/operation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/operation_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/symbolic_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/ops/symbolic_arguments_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.876886 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adadelta_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adafactor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adagrad_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adamax_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adamw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/ftrl_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/lion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/loss_scale_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/nadam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/optimizer_sparse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/rmsprop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.876886 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/schedules/learning_rate_schedule_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/sgd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.876886 keras_nightly-3.3.0.dev2024042203/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/quantizers/quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/quantizers/quantizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.876886 keras_nightly-3.3.0.dev2024042203/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/random/random_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/random/seed_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/random/seed_generator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.876886 keras_nightly-3.3.0.dev2024042203/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/regularizers/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/regularizers/regularizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.880886 keras_nightly-3.3.0.dev2024042203/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/object_registration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/saving_api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/saving_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/serialization_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/saving/serialization_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.880886 keras_nightly-3.3.0.dev2024042203/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/testing/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/testing/test_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.880886 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/compile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/compile_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.884886 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/array_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/generator_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/epoch_iterator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    51439 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/trainers/trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.884886 keras_nightly-3.3.0.dev2024042203/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/tree/tree_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/tree/tree_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.896886 keras_nightly-3.3.0.dev2024042203/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/audio_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/code_stats_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/dtype_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/file_utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/image_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/io_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/jax_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/naming_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/numerical_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/rng_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/sequence_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/summary_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/text_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/timeseries_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/torch_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/keras/src/utils/tracking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-22 03:21:33.000000 keras_nightly-3.3.0.dev2024042203/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 03:21:35.896886 keras_nightly-3.3.0.dev2024042203/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-22 03:21:35.000000 keras_nightly-3.3.0.dev2024042203/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-22 03:21:35.000000 keras_nightly-3.3.0.dev2024042203/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 03:21:35.000000 keras_nightly-3.3.0.dev2024042203/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 03:21:35.000000 keras_nightly-3.3.0.dev2024042203/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 03:21:35.000000 keras_nightly-3.3.0.dev2024042203/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-22 03:20:11.000000 keras_nightly-3.3.0.dev2024042203/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-22 03:21:35.896886 keras_nightly-3.3.0.dev2024042203/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-22 03:21:33.000000 keras_nightly-3.3.0.dev2024042203/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.300445 keras_nightly-3.3.2.dev2024042403/
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-24 03:21:30.300445 keras_nightly-3.3.2.dev2024042403/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.200445 keras_nightly-3.3.2.dev2024042403/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.200445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.200445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.200445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.200445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.200445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-24 03:21:28.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.204445 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-24 03:21:28.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-24 03:21:28.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.208444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 03:21:28.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 03:21:28.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-24 03:21:27.000000 keras_nightly-3.3.2.dev2024042403/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.212444 keras_nightly-3.3.2.dev2024042403/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.216445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.220445 keras_nightly-3.3.2.dev2024042403/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.224444 keras_nightly-3.3.2.dev2024042403/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.228445 keras_nightly-3.3.2.dev2024042403/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.228445 keras_nightly-3.3.2.dev2024042403/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.232445 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.236445 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26214 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30833 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.236445 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18006 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28098 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.240445 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26595 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77771 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.244445 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24278 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47434 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.244445 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.248445 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.248445 keras_nightly-3.3.2.dev2024042403/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.252445 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.252445 keras_nightly-3.3.2.dev2024042403/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.252445 keras_nightly-3.3.2.dev2024042403/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.252445 keras_nightly-3.3.2.dev2024042403/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.252445 keras_nightly-3.3.2.dev2024042403/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.252445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.256445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.256445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.260445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.260445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25345 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42181 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63788 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.260445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.264445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.264445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.272445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.272445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.276445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.276445 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.276445 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.280445 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.280445 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.280445 keras_nightly-3.3.2.dev2024042403/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.284445 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.284445 keras_nightly-3.3.2.dev2024042403/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.288445 keras_nightly-3.3.2.dev2024042403/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64046 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195627 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.288445 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.288445 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.288445 keras_nightly-3.3.2.dev2024042403/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.288445 keras_nightly-3.3.2.dev2024042403/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.292445 keras_nightly-3.3.2.dev2024042403/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.292445 keras_nightly-3.3.2.dev2024042403/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.292445 keras_nightly-3.3.2.dev2024042403/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.292445 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25940 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.296445 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.296445 keras_nightly-3.3.2.dev2024042403/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/tree/tree_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.300445 keras_nightly-3.3.2.dev2024042403/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-04-24 03:19:53.000000 keras_nightly-3.3.2.dev2024042403/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-24 03:21:28.000000 keras_nightly-3.3.2.dev2024042403/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:21:30.300445 keras_nightly-3.3.2.dev2024042403/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-24 03:21:30.000000 keras_nightly-3.3.2.dev2024042403/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20384 2024-04-24 03:21:30.000000 keras_nightly-3.3.2.dev2024042403/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 03:21:30.000000 keras_nightly-3.3.2.dev2024042403/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 03:21:30.000000 keras_nightly-3.3.2.dev2024042403/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 03:21:30.000000 keras_nightly-3.3.2.dev2024042403/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 03:21:30.300445 keras_nightly-3.3.2.dev2024042403/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-24 03:21:28.000000 keras_nightly-3.3.2.dev2024042403/setup.py
```

### Comparing `keras_nightly-3.3.0.dev2024042203/PKG-INFO` & `keras_nightly-3.3.2.dev2024042403/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.0.dev2024042203
+Version: 3.3.2.dev2024042403
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: namex
 Requires-Dist: h5py
 Requires-Dist: optree
 Requires-Dist: ml-dtypes
```

### Comparing `keras_nightly-3.3.0.dev2024042203/README.md` & `keras_nightly-3.3.2.dev2024042403/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-from keras.api import _tf_keras
+
 from keras.api import activations
 from keras.api import applications
 from keras.api import backend
 from keras.api import callbacks
 from keras.api import config
 from keras.api import constraints
 from keras.api import datasets
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
 from keras.api import activations
 from keras.api import applications
-from keras.api import backend
 from keras.api import callbacks
 from keras.api import config
 from keras.api import constraints
 from keras.api import datasets
 from keras.api import distribution
 from keras.api import dtype_policies
 from keras.api import export
 from keras.api import initializers
-from keras.api import layers
 from keras.api import legacy
-from keras.api import losses
-from keras.api import metrics
 from keras.api import mixed_precision
 from keras.api import models
 from keras.api import ops
 from keras.api import optimizers
-from keras.api import preprocessing
 from keras.api import quantizers
 from keras.api import random
 from keras.api import regularizers
-from keras.api import saving
 from keras.api import tree
 from keras.api import utils
+from keras._tf_keras.keras import backend
+from keras._tf_keras.keras import layers
+from keras._tf_keras.keras import losses
+from keras._tf_keras.keras import metrics
+from keras._tf_keras.keras import preprocessing
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.exports import Variable
 from keras.src.backend.exports import device
 from keras.src.backend.exports import name_scope
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import FloatDTypePolicy
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/activations/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/applications/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/backend/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-from keras.src.backend.common.dtypes import result_type
-from keras.src.backend.common.global_state import clear_session
-from keras.src.backend.common.keras_tensor import is_keras_tensor
-from keras.src.backend.common.variables import is_float_dtype
-from keras.src.backend.common.variables import is_int_dtype
-from keras.src.backend.common.variables import standardize_dtype
-from keras.src.backend.config import backend
-from keras.src.backend.config import epsilon
-from keras.src.backend.config import floatx
-from keras.src.backend.config import image_data_format
-from keras.src.backend.config import set_epsilon
-from keras.src.backend.config import set_floatx
-from keras.src.backend.config import set_image_data_format
-from keras.src.utils.naming import get_uid
+from keras.src.backend.jax import core
+from keras.src.backend.jax import distribution_lib
+from keras.src.backend.jax import image
+from keras.src.backend.jax import linalg
+from keras.src.backend.jax import math
+from keras.src.backend.jax import nn
+from keras.src.backend.jax import numpy
+from keras.src.backend.jax import random
+from keras.src.backend.jax.core import SUPPORTS_SPARSE_TENSORS
+from keras.src.backend.jax.core import Variable
+from keras.src.backend.jax.core import cast
+from keras.src.backend.jax.core import compute_output_spec
+from keras.src.backend.jax.core import cond
+from keras.src.backend.jax.core import convert_to_numpy
+from keras.src.backend.jax.core import convert_to_tensor
+from keras.src.backend.jax.core import device_scope
+from keras.src.backend.jax.core import is_tensor
+from keras.src.backend.jax.core import scatter
+from keras.src.backend.jax.core import shape
+from keras.src.backend.jax.core import stop_gradient
+from keras.src.backend.jax.core import vectorized_map
+from keras.src.backend.jax.rnn import cudnn_ok
+from keras.src.backend.jax.rnn import gru
+from keras.src.backend.jax.rnn import lstm
+from keras.src.backend.jax.rnn import rnn
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/config/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/constraints/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/distribution/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/initializers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/layers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/layers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,14 @@
 from keras.src.layers.preprocessing.rescaling import Rescaling
 from keras.src.layers.preprocessing.resizing import Resizing
 from keras.src.layers.preprocessing.string_lookup import StringLookup
 from keras.src.layers.preprocessing.text_vectorization import TextVectorization
 from keras.src.layers.regularization.activity_regularization import (
     ActivityRegularization,
 )
-from keras.src.layers.regularization.alpha_dropout import AlphaDropout
 from keras.src.layers.regularization.dropout import Dropout
 from keras.src.layers.regularization.gaussian_dropout import GaussianDropout
 from keras.src.layers.regularization.gaussian_noise import GaussianNoise
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout1D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout2D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout3D
 from keras.src.layers.reshaping.cropping1d import Cropping1D
@@ -186,10 +185,14 @@
 from keras.src.layers.rnn.lstm import LSTM
 from keras.src.layers.rnn.lstm import LSTMCell
 from keras.src.layers.rnn.rnn import RNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.layers.rnn.time_distributed import TimeDistributed
+from keras.src.legacy.layers import AlphaDropout
+from keras.src.legacy.layers import RandomHeight
+from keras.src.legacy.layers import RandomWidth
+from keras.src.legacy.layers import ThresholdedReLU
 from keras.src.utils.jax_layer import FlaxLayer
 from keras.src.utils.jax_layer import JaxLayer
 from keras.src.utils.torch_utils import TorchModuleWrapper
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/losses/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/losses/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
+from keras.src.legacy.losses import Reduction
 from keras.src.losses import deserialize
 from keras.src.losses import get
 from keras.src.losses import serialize
 from keras.src.losses.loss import Loss
 from keras.src.losses.losses import CTC
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
@@ -34,17 +35,23 @@
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
 from keras.src.losses.losses import dice
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
-from keras.src.losses.losses import kl_divergence
-from keras.src.losses.losses import log_cosh
-from keras.src.losses.losses import mean_absolute_error
-from keras.src.losses.losses import mean_absolute_percentage_error
-from keras.src.losses.losses import mean_squared_error
-from keras.src.losses.losses import mean_squared_logarithmic_error
+from keras.src.losses.losses import kl_divergence as KLD
+from keras.src.losses.losses import kl_divergence as kld
+from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
+from keras.src.losses.losses import log_cosh as logcosh
+from keras.src.losses.losses import mean_absolute_error as MAE
+from keras.src.losses.losses import mean_absolute_error as mae
+from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
+from keras.src.losses.losses import mean_absolute_percentage_error as mape
+from keras.src.losses.losses import mean_squared_error as MSE
+from keras.src.losses.losses import mean_squared_error as mse
+from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
+from keras.src.losses.losses import mean_squared_logarithmic_error as msle
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
 from keras.src.losses.losses import tversky
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/metrics/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,26 @@
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
-from keras.src.losses.losses import kl_divergence
-from keras.src.losses.losses import log_cosh
-from keras.src.losses.losses import mean_absolute_error
-from keras.src.losses.losses import mean_absolute_percentage_error
-from keras.src.losses.losses import mean_squared_error
-from keras.src.losses.losses import mean_squared_logarithmic_error
+from keras.src.losses.losses import kl_divergence as KLD
+from keras.src.losses.losses import kl_divergence as kld
+from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
+from keras.src.losses.losses import log_cosh as logcosh
+from keras.src.losses.losses import mean_absolute_error as MAE
+from keras.src.losses.losses import mean_absolute_error as mae
+from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
+from keras.src.losses.losses import mean_absolute_percentage_error as mape
+from keras.src.losses.losses import mean_squared_error as MSE
+from keras.src.losses.losses import mean_squared_error as mse
+from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
+from keras.src.losses.losses import mean_squared_logarithmic_error as msle
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
 from keras.src.metrics import deserialize
 from keras.src.metrics import get
 from keras.src.metrics import serialize
 from keras.src.metrics.accuracy_metrics import Accuracy
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/ops/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/random/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/saving/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/tree/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/api/utils/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/activations/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/activations/activations.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/api_export.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/convnext.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/densenet.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/nasnet.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/resnet.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/vgg16.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/vgg19.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/applications/xception.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/common/variables.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/config.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/exports.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from keras.src.backend.jax import core
-from keras.src.backend.jax import distribution_lib
-from keras.src.backend.jax import image
-from keras.src.backend.jax import linalg
-from keras.src.backend.jax import math
-from keras.src.backend.jax import nn
-from keras.src.backend.jax import numpy
-from keras.src.backend.jax import random
-from keras.src.backend.jax.core import SUPPORTS_SPARSE_TENSORS
-from keras.src.backend.jax.core import Variable
-from keras.src.backend.jax.core import cast
-from keras.src.backend.jax.core import compute_output_spec
-from keras.src.backend.jax.core import cond
-from keras.src.backend.jax.core import convert_to_numpy
-from keras.src.backend.jax.core import convert_to_tensor
-from keras.src.backend.jax.core import device_scope
-from keras.src.backend.jax.core import is_tensor
-from keras.src.backend.jax.core import scatter
-from keras.src.backend.jax.core import shape
-from keras.src.backend.jax.core import stop_gradient
-from keras.src.backend.jax.core import vectorized_map
-from keras.src.backend.jax.rnn import cudnn_ok
-from keras.src.backend.jax.rnn import gru
-from keras.src.backend.jax.rnn import lstm
-from keras.src.backend.jax.rnn import rnn
+from keras.src.backend.tensorflow import core
+from keras.src.backend.tensorflow import distribution_lib
+from keras.src.backend.tensorflow import image
+from keras.src.backend.tensorflow import linalg
+from keras.src.backend.tensorflow import math
+from keras.src.backend.tensorflow import nn
+from keras.src.backend.tensorflow import numpy
+from keras.src.backend.tensorflow import random
+from keras.src.backend.tensorflow import tensorboard
+from keras.src.backend.tensorflow.core import SUPPORTS_SPARSE_TENSORS
+from keras.src.backend.tensorflow.core import Variable
+from keras.src.backend.tensorflow.core import cast
+from keras.src.backend.tensorflow.core import compute_output_spec
+from keras.src.backend.tensorflow.core import cond
+from keras.src.backend.tensorflow.core import convert_to_numpy
+from keras.src.backend.tensorflow.core import convert_to_tensor
+from keras.src.backend.tensorflow.core import device_scope
+from keras.src.backend.tensorflow.core import is_tensor
+from keras.src.backend.tensorflow.core import name_scope
+from keras.src.backend.tensorflow.core import scatter
+from keras.src.backend.tensorflow.core import shape
+from keras.src.backend.tensorflow.core import stop_gradient
+from keras.src.backend.tensorflow.core import vectorized_map
+from keras.src.backend.tensorflow.rnn import cudnn_ok
+from keras.src.backend.tensorflow.rnn import gru
+from keras.src.backend.tensorflow.rnn import lstm
+from keras.src.backend.tensorflow.rnn import rnn
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/core.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/image.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/math.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,15 +778,16 @@
         paths, unique_inverse = jnp.unique(
             paths,
             return_inverse=True,
             size=2 * num_classes * beam_width,
             axis=0,
             fill_value=_pad,
         )
-        unique_inverse = jnp.squeeze(unique_inverse, axis=1)
+        if len(unique_inverse.shape) >= 2:
+            unique_inverse = jnp.squeeze(unique_inverse, axis=1)
 
         emit_scores = jnp.where(masked, -jnp.inf, scores)
         mask_scores = jnp.where(masked, scores, -jnp.inf)
 
         emit_scores = _merge_scores(unique_inverse, emit_scores)
         mask_scores = _merge_scores(unique_inverse, mask_scores)
 
@@ -838,15 +839,16 @@
         paths, unique_inverse = jnp.unique(
             paths,
             return_inverse=True,
             size=2 * num_classes * beam_width,
             axis=0,
             fill_value=_pad,
         )
-        unique_inverse = jnp.squeeze(unique_inverse, axis=1)
+        if len(unique_inverse.shape) >= 2:
+            unique_inverse = jnp.squeeze(unique_inverse, axis=1)
         scores = _merge_scores(unique_inverse, scores)
 
         top_indices = jnp.argsort(scores)[-top_paths:][::-1]
         paths = paths[top_indices]
         scores = scores[top_indices]
 
         return paths, scores
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1019,16 +1019,18 @@
     return jnp.vdot(x1, x2)
 
 
 def vstack(xs):
     return jnp.vstack(xs)
 
 
-def vectorize(pyfunc):
-    return jnp.vectorize(pyfunc)
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    if excluded is None:
+        excluded = set()
+    return jnp.vectorize(pyfunc, excluded=excluded, signature=signature)
 
 
 def where(condition, x1, x2):
     return jnp.where(condition, x1, x2)
 
 
 @sparse.elementwise_division
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/random.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -933,16 +933,16 @@
         dtype = dtypes.result_type(*dtype_set)
         xs = tree.map_structure(
             lambda x: convert_to_tensor(x).astype(dtype), xs
         )
     return np.vstack(xs)
 
 
-def vectorize(pyfunc):
-    return np.vectorize(pyfunc)
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    return np.vectorize(pyfunc, excluded=excluded, signature=signature)
 
 
 def where(condition, x1, x2):
     if x1 is not None and x2 is not None:
         if not isinstance(x1, (int, float)):
             x1 = convert_to_tensor(x1)
         if not isinstance(x2, (int, float)):
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from keras.src import tree
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
+from keras.src.backend.common.backend_utils import vectorize_impl
 from keras.src.backend.tensorflow import sparse
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
 
 
 @sparse.elementwise_binary_union(tf.sparse.add)
 def add(x1, x2):
@@ -2152,22 +2153,33 @@
     dtype_set = set([getattr(x, "dtype", type(x)) for x in xs])
     if len(dtype_set) > 1:
         dtype = dtypes.result_type(*dtype_set)
         xs = tree.map_structure(lambda x: convert_to_tensor(x, dtype), xs)
     return tf.concat(xs, axis=0)
 
 
-def vectorize(pyfunc):
-    @functools.wraps(pyfunc)
+def _vmap_fn(fn, in_axes=0):
+    if in_axes != 0:
+        raise ValueError(
+            "Not supported with `vectorize()` with the TensorFlow backend."
+        )
+
+    @functools.wraps(fn)
     def wrapped(x):
-        return tf.vectorized_map(pyfunc, x)
+        return tf.vectorized_map(fn, x)
 
     return wrapped
 
 
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    return vectorize_impl(
+        pyfunc, _vmap_fn, excluded=excluded, signature=signature
+    )
+
+
 def where(condition, x1, x2):
     condition = tf.cast(condition, "bool")
     if x1 is not None and x2 is not None:
         if not isinstance(x1, (int, float)):
             x1 = convert_to_tensor(x1)
         if not isinstance(x2, (int, float)):
             x2 = convert_to_tensor(x2)
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/core.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/image.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/math.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import builtins
-import functools
 import math
 
 import torch
 
 from keras.src.backend import KerasTensor
 from keras.src.backend import config
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
+from keras.src.backend.common.backend_utils import vectorize_impl
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.backend.torch.core import cast
 from keras.src.backend.torch.core import convert_to_tensor
 from keras.src.backend.torch.core import get_device
 from keras.src.backend.torch.core import is_tensor
 from keras.src.backend.torch.core import to_torch_dtype
 
@@ -1409,20 +1409,18 @@
 
 
 def vstack(xs):
     xs = [convert_to_tensor(x) for x in xs]
     return torch.vstack(xs)
 
 
-def vectorize(pyfunc):
-    @functools.wraps(pyfunc)
-    def wrapped(x):
-        return torch.vmap(pyfunc, x)
-
-    return wrapped
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    return vectorize_impl(
+        pyfunc, torch.vmap, excluded=excluded, signature=signature
+    )
 
 
 def where(condition, x1, x2):
     condition = convert_to_tensor(condition, dtype=bool)
     if x1 is not None and x2 is not None:
         x1 = convert_to_tensor(x1)
         x2 = convert_to_tensor(x2)
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/random.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/callback.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/history.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/reduce_lr_on_plateau_test.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adadelta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-import pytest
-
-from keras.src import callbacks
-from keras.src import layers
-from keras.src import optimizers
-from keras.src import testing
-from keras.src.models import Sequential
-from keras.src.testing import test_utils
-from keras.src.utils import io_utils
-from keras.src.utils import numerical_utils
-
-
-class ReduceLROnPlateauTest(testing.TestCase):
-    def setUp(self):
-        (x_train, y_train), (x_test, y_test) = test_utils.get_test_data(
-            train_samples=10,
-            test_samples=10,
-            input_shape=(3,),
-            num_classes=2,
-        )
-        y_test = numerical_utils.to_categorical(y_test)
-        y_train = numerical_utils.to_categorical(y_train)
-
-        model = Sequential([layers.Dense(5), layers.Dense(2)])
-
-        model.compile(
-            loss="mse",
-            optimizer=optimizers.Adam(0.1),
-        )
-
-        self.model = model
-        self.x_train = x_train
-        self.x_test = x_test
-        self.y_train = y_train
-        self.y_test = y_test
-
-    @pytest.mark.requires_trainable_backend
-    def test_reduces_lr_with_model_fit(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1, factor=0.1, monitor="val_loss", min_delta=100
-        )
-
-        self.model.fit(
-            self.x_train,
-            self.y_train,
-            validation_data=(self.x_test, self.y_test),
-            callbacks=[reduce_lr],
-            epochs=2,
-        )
-
-        self.assertEqual(self.model.optimizer.learning_rate.value, 0.01)
-
-    @pytest.mark.requires_trainable_backend
-    def test_throws_when_optimizer_has_schedule(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1, factor=0.1, monitor="val_loss", min_delta=100
-        )
+from keras.src import ops
+from keras.src.api_export import keras_export
+from keras.src.optimizers import optimizer
+
+
+@keras_export(["keras.optimizers.Adadelta"])
+class Adadelta(optimizer.Optimizer):
+    """Optimizer that implements the Adadelta algorithm.
+
+    Adadelta optimization is a stochastic gradient descent method that is based
+    on adaptive learning rate per dimension to address two drawbacks:
+
+    - The continual decay of learning rates throughout training.
+    - The need for a manually selected global learning rate.
+
+    Adadelta is a more robust extension of Adagrad that adapts learning rates
+    based on a moving window of gradient updates, instead of accumulating all
+    past gradients. This way, Adadelta continues learning even when many updates
+    have been done. Compared to Adagrad, in the original version of Adadelta you
+    don't have to set an initial learning rate. In this version, the initial
+    learning rate can be set, as in most other Keras optimizers.
+
+    Args:
+        learning_rate: A float, a
+            `keras.optimizers.schedules.LearningRateSchedule` instance, or
+            a callable that takes no arguments and returns the actual value to
+            use. The learning rate. Defaults to `0.001`. Note that `Adadelta`
+            tends to benefit from higher initial learning rate values compared
+            to other optimizers. To match the exact form in the original paper,
+            use 1.0.
+        rho: A floating point value. The decay rate. Defaults to `0.95`.
+        epsilon: Small floating point value for maintaining numerical stability.
+        {{base_optimizer_keyword_args}}
+
+    Reference:
+
+    - [Zeiler, 2012](http://arxiv.org/abs/1212.5701)
+    """
+
+    def __init__(
+        self,
+        learning_rate=0.001,
+        rho=0.95,
+        epsilon=1e-7,
+        weight_decay=None,
+        clipnorm=None,
+        clipvalue=None,
+        global_clipnorm=None,
+        use_ema=False,
+        ema_momentum=0.99,
+        ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
+        name="adadelta",
+        **kwargs,
+    ):
+        super().__init__(
+            learning_rate=learning_rate,
+            weight_decay=weight_decay,
+            clipnorm=clipnorm,
+            clipvalue=clipvalue,
+            global_clipnorm=global_clipnorm,
+            use_ema=use_ema,
+            ema_momentum=ema_momentum,
+            ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
+            name=name,
+            **kwargs,
+        )
+        self.rho = rho
+        self.epsilon = epsilon
+
+    def build(self, var_list):
+        if self.built:
+            return
+        super().build(var_list)
+        self._accumulated_grads = []
+        self._accumulated_delta_vars = []
+        for var in var_list:
+            self._accumulated_grads.append(
+                self.add_variable_from_reference(var, "accumulated_grad")
+            )
+            self._accumulated_delta_vars.append(
+                self.add_variable_from_reference(var, "accumulated_delta_var")
+            )
 
-        self.model.compile(
-            loss="mse",
-            optimizer=optimizers.Adam(
-                optimizers.schedules.PolynomialDecay(
-                    initial_learning_rate=0.1, decay_steps=10
-                )
+    def update_step(self, grad, variable, learning_rate):
+        """Update step given gradient and the associated model variable."""
+        lr = ops.cast(learning_rate, variable.dtype)
+        grad = ops.cast(grad, variable.dtype)
+
+        rho = self.rho
+        accumulated_grad = self._accumulated_grads[
+            self._get_variable_index(variable)
+        ]
+        accumulated_delta_var = self._accumulated_delta_vars[
+            self._get_variable_index(variable)
+        ]
+
+        def rms(x):
+            return ops.sqrt(ops.add(x, self.epsilon))
+
+        self.assign(
+            accumulated_grad,
+            ops.add(
+                rho * accumulated_grad, ops.multiply(1 - rho, ops.square(grad))
             ),
         )
-
-        with self.assertRaisesRegex(
-            TypeError,
-            "This optimizer was created with a `LearningRateSchedule`",
-        ):
-            self.model.fit(
-                self.x_train,
-                self.y_train,
-                validation_data=(self.x_test, self.y_test),
-                callbacks=[reduce_lr],
-                epochs=2,
+        delta_var = ops.negative(
+            ops.divide(
+                ops.multiply(rms(accumulated_delta_var), grad),
+                rms(accumulated_grad),
             )
-
-    @pytest.mark.requires_trainable_backend
-    def test_verbose_logging(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1, factor=0.1, monitor="val_loss", min_delta=100, verbose=1
         )
-        io_utils.disable_interactive_logging()
-        io_utils.set_logging_verbosity("INFO")
-
-        with self.assertLogs() as logs:
-            self.model.fit(
-                self.x_train,
-                self.y_train,
-                validation_data=(self.x_test, self.y_test),
-                callbacks=[reduce_lr],
-                epochs=2,
-            )
-            expected_log = "ReduceLROnPlateau reducing learning rate to 0.01"
-            self.assertTrue(any(expected_log in log for log in logs.output))
-
-    @pytest.mark.requires_trainable_backend
-    def test_honors_min_lr(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1,
-            factor=0.1,
-            monitor="val_loss",
-            min_delta=10,
-            min_lr=0.005,
-        )
-
-        self.model.fit(
-            self.x_train,
-            self.y_train,
-            validation_data=(self.x_test, self.y_test),
-            callbacks=[reduce_lr],
-            epochs=4,
+        self.assign(
+            accumulated_delta_var,
+            ops.add(
+                ops.multiply(rho, accumulated_delta_var),
+                ops.multiply(1 - rho, ops.square(delta_var)),
+            ),
         )
+        self.assign_add(variable, ops.multiply(lr, delta_var))
 
-        self.assertEqual(self.model.optimizer.learning_rate.value, 0.005)
+    def get_config(self):
+        config = super().get_config()
 
-    @pytest.mark.requires_trainable_backend
-    def test_cooldown(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1,
-            factor=0.1,
-            monitor="val_loss",
-            min_delta=100,
-            cooldown=2,
+        config.update(
+            {
+                "rho": self.rho,
+                "epsilon": self.epsilon,
+            }
         )
+        return config
 
-        self.model.fit(
-            self.x_train,
-            self.y_train,
-            validation_data=(self.x_test, self.y_test),
-            callbacks=[reduce_lr],
-            epochs=4,
-        )
 
-        # With a cooldown of 2 epochs, we should only reduce the LR every other
-        # epoch, so after 4 epochs we will have reduced 2 times.
-        self.assertAllClose(self.model.optimizer.learning_rate.value, 0.001)
+Adadelta.__doc__ = Adadelta.__doc__.replace(
+    "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
+)
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/constraints/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/constraints/constraints.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/cifar.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/imdb.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/imdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,16 @@
             [w if (skip_top <= w < num_words) else oov_char for w in x]
             for x in xs
         ]
     else:
         xs = [[w for w in x if skip_top <= w < num_words] for x in xs]
 
     idx = len(x_train)
-    x_train, y_train = xs[:idx], labels[:idx]
-    x_test, y_test = xs[idx:], labels[idx:]
+    x_train, y_train = np.array(xs[:idx], dtype="object"), labels[:idx]
+    x_test, y_test = np.array(xs[idx:], dtype="object"), labels[idx:]
     return (x_train, y_train), (x_test, y_test)
 
 
 @keras_export("keras.datasets.imdb.get_word_index")
 def get_word_index(path="imdb_word_index.json"):
     """Retrieves a dict mapping words to their index in the IMDB dataset.
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/mnist.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/datasets/reuters.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/distribution/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/dtype_policies/dtype_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,14 +289,19 @@
         valid_policies = [
             f"{mode}_from_{policy}"
             for mode in ("float8")
             for policy in valid_float_policies
         ]
         return valid_policies
 
+    def get_config(self):
+        config = super().get_config()
+        config.update({"amax_history_length": self.amax_history_length})
+        return config
+
 
 @keras_export(
     [
         "keras.config.set_dtype_policy",
         "keras.mixed_precision.set_dtype_policy",  # Legacy
         "keras.mixed_precision.set_global_policy",  # Legacy
     ]
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/export/export_lib.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/initializers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/initializers/initializer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/base_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,27 +303,31 @@
         self.lora_enabled = True
         self.lora_rank = rank
 
     def save_own_variables(self, store):
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
-        store["0"] = self.kernel
+        target_variables = [self.kernel]
         if self.use_bias:
-            store["1"] = self.bias
+            target_variables.append(self.bias)
+        for i, variable in enumerate(target_variables):
+            store[str(i)] = variable
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
-        self._kernel.assign(store["0"])
+        target_variables = [self._kernel]
         if self.use_bias:
-            self.bias.assign(store["1"])
+            target_variables.append(self.bias)
+        for i, variable in enumerate(target_variables):
+            variable.assign(store[str(i)])
         if self.lora_enabled:
             self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
             self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
 
     def get_config(self):
         config = super().get_config()
         config.update(
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/dense.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/dense.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,59 +198,63 @@
     def save_own_variables(self, store):
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         kernel_value, kernel_scale = self._get_kernel_with_merged_lora()
-        store["0"] = kernel_value
+        target_variables = [kernel_value]
         if self.use_bias:
-            store["1"] = self.bias
+            target_variables.append(self.bias)
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             mode = self.dtype_policy.quantization_mode
             if mode == "int8":
-                store["2"] = kernel_scale
+                target_variables.append(kernel_scale)
             elif mode == "float8":
-                store["2"] = self.inputs_scale
-                store["3"] = self.inputs_amax_history
-                store["4"] = self.kernel_scale
-                store["5"] = self.kernel_amax_history
-                store["6"] = self.outputs_grad_scale
-                store["7"] = self.outputs_grad_amax_history
+                target_variables.append(self.inputs_scale)
+                target_variables.append(self.inputs_amax_history)
+                target_variables.append(self.kernel_scale)
+                target_variables.append(self.kernel_amax_history)
+                target_variables.append(self.outputs_grad_scale)
+                target_variables.append(self.outputs_grad_amax_history)
             else:
                 raise NotImplementedError(
                     self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
                 )
+        for i, variable in enumerate(target_variables):
+            store[str(i)] = variable
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
-        self._kernel.assign(store["0"])
+        target_variables = [self._kernel]
         if self.use_bias:
-            self.bias.assign(store["1"])
+            target_variables.append(self.bias)
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             mode = self.dtype_policy.quantization_mode
             if mode == "int8":
-                self.kernel_scale.assign(store["2"])
+                target_variables.append(self.kernel_scale)
             elif mode == "float8":
-                self.inputs_scale.assign(store["2"])
-                self.inputs_amax_history.assign(store["3"])
-                self.kernel_scale.assign(store["4"])
-                self.kernel_amax_history.assign(store["5"])
-                self.outputs_grad_scale.assign(store["6"])
-                self.outputs_grad_amax_history.assign(store["7"])
+                target_variables.append(self.inputs_scale)
+                target_variables.append(self.inputs_amax_history)
+                target_variables.append(self.kernel_scale)
+                target_variables.append(self.kernel_amax_history)
+                target_variables.append(self.outputs_grad_scale)
+                target_variables.append(self.outputs_grad_amax_history)
             else:
                 raise NotImplementedError(
                     self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
                 )
+        for i, variable in enumerate(target_variables):
+            variable.assign(store[str(i)])
         if self.lora_enabled:
             self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
             self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
 
     def get_config(self):
         base_config = super().get_config()
         config = {
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/dense_test.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/testing/test_case.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,734 +1,689 @@
-import os
+import json
+import shutil
+import tempfile
+import unittest
 
 import numpy as np
-import pytest
-from absl.testing import parameterized
 
 from keras.src import backend
-from keras.src import constraints
-from keras.src import layers
-from keras.src import models
+from keras.src import distribution
 from keras.src import ops
-from keras.src import optimizers
-from keras.src import random
-from keras.src import saving
-from keras.src import testing
-from keras.src.backend.common import keras_tensor
-from keras.src.export import export_lib
-
-
-class DenseTest(testing.TestCase, parameterized.TestCase):
-    @pytest.mark.requires_trainable_backend
-    def test_dense_basics(self):
-        # 2D case, no bias.
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 4,
-                "activation": "relu",
-                "kernel_initializer": "random_uniform",
-                "bias_initializer": "ones",
-                "use_bias": False,
-            },
-            input_shape=(2, 3),
-            expected_output_shape=(2, 4),
-            expected_num_trainable_weights=1,
-            expected_num_non_trainable_weights=0,
-            expected_num_seed_generators=0,
-            expected_num_losses=0,
-            supports_masking=True,
-        )
-        # 3D case, some regularizers.
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 5,
-                "activation": "sigmoid",
-                "kernel_regularizer": "l2",
-                "bias_regularizer": "l2",
-            },
-            input_shape=(2, 3, 4),
-            expected_output_shape=(2, 3, 5),
-            expected_num_trainable_weights=2,
-            expected_num_non_trainable_weights=0,
-            expected_num_seed_generators=0,
-            expected_num_losses=2,  # we have 2 regularizers.
-            supports_masking=True,
-        )
-
-    def test_dense_correctness(self):
-        # With bias and activation.
-        layer = layers.Dense(units=2, activation="relu")
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-                np.array([5.0, -6.0]),
-            ]
-        )
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        self.assertAllClose(layer(inputs), [[10.0, 0.0]])
-
-        # Just a kernel matmul.
-        layer = layers.Dense(units=2, use_bias=False)
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-            ]
-        )
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        self.assertEqual(layer.bias, None)
-        self.assertAllClose(layer(inputs), [[5.0, -6.0]])
-
-    def test_dense_errors(self):
-        with self.assertRaisesRegex(ValueError, "incompatible with the layer"):
-            layer = layers.Dense(units=2, activation="relu")
-            layer(keras_tensor.KerasTensor((1, 2)))
-            layer(keras_tensor.KerasTensor((1, 3)))
-
-    @pytest.mark.skipif(
-        not backend.SUPPORTS_SPARSE_TENSORS,
-        reason="Backend does not support sparse tensors.",
-    )
-    def test_dense_sparse(self):
-        import tensorflow as tf
-
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 4,
-            },
-            input_shape=(2, 3),
-            input_sparse=True,
-            expected_output_shape=(2, 4),
-            expected_num_trainable_weights=2,
-            expected_num_non_trainable_weights=0,
-            expected_num_seed_generators=0,
-            expected_num_losses=0,
-        )
-
-        inputs = 4 * backend.random.uniform((10, 10))
-        inputs = tf.sparse.from_dense(tf.nn.dropout(inputs, 0.8))
-
-        inputs = np.random.random((10, 10)).astype("float32")
-        inputs = np.multiply(inputs, inputs >= 0.8)
-
-        if backend.backend() == "tensorflow":
+from keras.src import tree
+from keras.src import utils
+from keras.src.backend.common import is_float_dtype
+from keras.src.backend.common import standardize_dtype
+from keras.src.backend.common.global_state import clear_session
+from keras.src.backend.common.keras_tensor import KerasTensor
+from keras.src.models import Model
+from keras.src.utils import traceback_utils
+
+
+class TestCase(unittest.TestCase):
+    maxDiff = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def setUp(self):
+        # clear global state so that test cases are independent
+        # required for the jit enabled torch tests since dynamo has
+        # a global cache for guards, compiled fn, etc
+        clear_session(free_memory=False)
+        if traceback_utils.is_traceback_filtering_enabled():
+            traceback_utils.disable_traceback_filtering()
+
+    def get_temp_dir(self):
+        temp_dir = tempfile.mkdtemp()
+        self.addCleanup(lambda: shutil.rmtree(temp_dir))
+        return temp_dir
+
+    def assertAllClose(self, x1, x2, atol=1e-6, rtol=1e-6, msg=None):
+        if not isinstance(x1, np.ndarray):
+            x1 = backend.convert_to_numpy(x1)
+        if not isinstance(x2, np.ndarray):
+            x2 = backend.convert_to_numpy(x2)
+        np.testing.assert_allclose(x1, x2, atol=atol, rtol=rtol)
+
+    def assertNotAllClose(self, x1, x2, atol=1e-6, rtol=1e-6, msg=None):
+        try:
+            self.assertAllClose(x1, x2, atol=atol, rtol=rtol, msg=msg)
+        except AssertionError:
+            return
+        msg = msg or ""
+        raise AssertionError(
+            f"The two values are close at all elements. \n"
+            f"{msg}.\n"
+            f"Values: {x1}"
+        )
+
+    def assertAlmostEqual(self, x1, x2, decimal=3, msg=None):
+        if not isinstance(x1, np.ndarray):
+            x1 = backend.convert_to_numpy(x1)
+        if not isinstance(x2, np.ndarray):
+            x2 = backend.convert_to_numpy(x2)
+        np.testing.assert_almost_equal(x1, x2, decimal=decimal)
+
+    def assertAllEqual(self, x1, x2, msg=None):
+        self.assertEqual(len(x1), len(x2), msg=msg)
+        for e1, e2 in zip(x1, x2):
+            if isinstance(e1, (list, tuple)) or isinstance(e2, (list, tuple)):
+                self.assertAllEqual(e1, e2, msg=msg)
+            else:
+                e1 = backend.convert_to_numpy(e1)
+                e2 = backend.convert_to_numpy(e2)
+                self.assertEqual(e1, e2, msg=msg)
+
+    def assertLen(self, iterable, expected_len, msg=None):
+        self.assertEqual(len(iterable), expected_len, msg=msg)
+
+    def assertSparse(self, x, sparse=True):
+        if isinstance(x, KerasTensor):
+            self.assertEqual(x.sparse, sparse)
+        elif backend.backend() == "tensorflow":
             import tensorflow as tf
 
-            inputs = tf.sparse.from_dense(inputs)
+            if sparse:
+                self.assertIsInstance(x, tf.SparseTensor)
+            else:
+                self.assertNotIsInstance(x, tf.SparseTensor)
         elif backend.backend() == "jax":
             import jax.experimental.sparse as jax_sparse
 
-            inputs = jax_sparse.BCOO.fromdense(inputs)
+            if sparse:
+                self.assertIsInstance(x, jax_sparse.JAXSparse)
+            else:
+                self.assertNotIsInstance(x, jax_sparse.JAXSparse)
         else:
-            self.fail(f"Sparse is unsupported with backend {backend.backend()}")
-
-        layer = layers.Dense(units=10)
-        outputs = layer(inputs)
-
-        # Verify the computation is the same as if it had been a dense tensor
-        expected_outputs = ops.add(
-            ops.matmul(
-                backend.convert_to_tensor(inputs, sparse=False), layer.kernel
-            ),
-            layer.bias,
-        )
-        self.assertAllClose(outputs, expected_outputs)
+            self.assertFalse(
+                sparse,
+                f"Backend {backend.backend()} does not support sparse tensors",
+            )
+
+    def run_class_serialization_test(self, instance, custom_objects=None):
+        from keras.src.saving import custom_object_scope
+        from keras.src.saving import deserialize_keras_object
+        from keras.src.saving import serialize_keras_object
+
+        # get_config roundtrip
+        cls = instance.__class__
+        config = instance.get_config()
+        config_json = json.dumps(config, sort_keys=True, indent=4)
+        ref_dir = dir(instance)[:]
+        with custom_object_scope(custom_objects):
+            revived_instance = cls.from_config(config)
+        revived_config = revived_instance.get_config()
+        revived_config_json = json.dumps(
+            revived_config, sort_keys=True, indent=4
+        )
+        self.assertEqual(config_json, revived_config_json)
+        self.assertEqual(set(ref_dir), set(dir(revived_instance)))
+
+        # serialization roundtrip
+        serialized = serialize_keras_object(instance)
+        serialized_json = json.dumps(serialized, sort_keys=True, indent=4)
+        with custom_object_scope(custom_objects):
+            revived_instance = deserialize_keras_object(
+                json.loads(serialized_json)
+            )
+        revived_config = revived_instance.get_config()
+        revived_config_json = json.dumps(
+            revived_config, sort_keys=True, indent=4
+        )
+        self.assertEqual(config_json, revived_config_json)
+        new_dir = dir(revived_instance)[:]
+        for lst in [ref_dir, new_dir]:
+            if "__annotations__" in lst:
+                lst.remove("__annotations__")
+        self.assertEqual(set(ref_dir), set(new_dir))
+        return revived_instance
+
+    def run_layer_test(
+        self,
+        layer_cls,
+        init_kwargs,
+        input_shape=None,
+        input_dtype=None,
+        input_sparse=False,
+        input_data=None,
+        call_kwargs=None,
+        expected_output_shape=None,
+        expected_output_dtype=None,
+        expected_output_sparse=False,
+        expected_output=None,
+        expected_num_trainable_weights=None,
+        expected_num_non_trainable_weights=None,
+        expected_num_non_trainable_variables=None,
+        expected_num_seed_generators=None,
+        expected_num_losses=None,
+        supports_masking=None,
+        expected_mask_shape=None,
+        custom_objects=None,
+        run_training_check=True,
+        run_mixed_precision_check=True,
+    ):
+        """Run basic checks on a layer.
 
-        # Verify the gradient is sparse
-        if backend.backend() == "tensorflow":
-            import tensorflow as tf
+        Args:
+            layer_cls: The class of the layer to test.
+            init_kwargs: Dict of arguments to be used to
+                instantiate the layer.
+            input_shape: Shape tuple (or list/dict of shape tuples)
+                to call the layer on.
+            input_dtype: Corresponding input dtype.
+            input_sparse: Whether the input is a sparse tensor (this requires
+                the backend to support sparse tensors).
+            input_data: Tensor (or list/dict of tensors)
+                to call the layer on.
+            call_kwargs: Dict of arguments to use when calling the
+                layer (does not include the first input tensor argument)
+            expected_output_shape: Shape tuple
+                (or list/dict of shape tuples)
+                expected as output.
+            expected_output_dtype: dtype expected as output.
+            expected_output_sparse: Whether the output is expected to be sparse
+                (this requires the backend to support sparse tensors).
+            expected_output: Expected output tensor -- only
+                to be specified if input_data is provided.
+            expected_num_trainable_weights: Expected number
+                of trainable weights of the layer once built.
+            expected_num_non_trainable_weights: Expected number
+                of non-trainable weights of the layer once built.
+            expected_num_seed_generators: Expected number of
+                SeedGenerators objects of the layer once built.
+            expected_num_losses: Expected number of loss tensors
+                produced when calling the layer.
+            supports_masking: If True, will check that the layer
+                supports masking.
+            expected_mask_shape: Expected mask shape tuple
+                returned by compute_mask() (only supports 1 shape).
+            custom_objects: Dict of any custom objects to be
+                considered during deserialization.
+            run_training_check: Whether to attempt to train the layer
+                (if an input shape or input data was provided).
+            run_mixed_precision_check: Whether to test the layer with a mixed
+                precision dtype policy.
+        """
+        if input_shape is not None and input_data is not None:
+            raise ValueError(
+                "input_shape and input_data cannot be passed "
+                "at the same time."
+            )
+        if expected_output_shape is not None and expected_output is not None:
+            raise ValueError(
+                "expected_output_shape and expected_output cannot be passed "
+                "at the same time."
+            )
+        if expected_output is not None and input_data is None:
+            raise ValueError(
+                "In order to use expected_output, input_data must be provided."
+            )
+        if expected_mask_shape is not None and supports_masking is not True:
+            raise ValueError(
+                "In order to use expected_mask_shape, supports_masking "
+                "must be True."
+            )
+
+        init_kwargs = init_kwargs or {}
+        call_kwargs = call_kwargs or {}
+
+        if input_shape is not None and input_dtype is not None:
+            if isinstance(input_shape, tuple) and is_shape_tuple(
+                input_shape[0]
+            ):
+                self.assertIsInstance(input_dtype, tuple)
+                self.assertEqual(
+                    len(input_shape),
+                    len(input_dtype),
+                    msg="The number of input shapes and dtypes does not match",
+                )
+            elif isinstance(input_shape, dict):
+                self.assertIsInstance(input_dtype, dict)
+                self.assertEqual(
+                    set(input_shape.keys()),
+                    set(input_dtype.keys()),
+                    msg="The number of input shapes and dtypes does not match",
+                )
+            elif isinstance(input_shape, list):
+                self.assertIsInstance(input_dtype, list)
+                self.assertEqual(
+                    len(input_shape),
+                    len(input_dtype),
+                    msg="The number of input shapes and dtypes does not match",
+                )
+            elif not isinstance(input_shape, tuple):
+                raise ValueError("The type of input_shape is not supported")
+        if input_shape is not None and input_dtype is None:
+            input_dtype = tree.map_shape_structure(
+                lambda _: "float32", input_shape
+            )
+
+        # Serialization test.
+        layer = layer_cls(**init_kwargs)
+        self.run_class_serialization_test(layer, custom_objects)
+
+        # Basic masking test.
+        if supports_masking is not None:
+            self.assertEqual(
+                layer.supports_masking,
+                supports_masking,
+                msg="Unexpected supports_masking value",
+            )
+
+        def run_build_asserts(layer):
+            self.assertTrue(layer.built)
+            if expected_num_trainable_weights is not None:
+                self.assertLen(
+                    layer.trainable_weights,
+                    expected_num_trainable_weights,
+                    msg="Unexpected number of trainable_weights",
+                )
+            if expected_num_non_trainable_weights is not None:
+                self.assertLen(
+                    layer.non_trainable_weights,
+                    expected_num_non_trainable_weights,
+                    msg="Unexpected number of non_trainable_weights",
+                )
+            if expected_num_non_trainable_variables is not None:
+                self.assertLen(
+                    layer.non_trainable_variables,
+                    expected_num_non_trainable_variables,
+                    msg="Unexpected number of non_trainable_variables",
+                )
+            if expected_num_seed_generators is not None:
+                self.assertLen(
+                    get_seed_generators(layer),
+                    expected_num_seed_generators,
+                    msg="Unexpected number of seed_generators",
+                )
+            if (
+                backend.backend() == "torch"
+                and expected_num_trainable_weights is not None
+                and expected_num_non_trainable_weights is not None
+                and expected_num_seed_generators is not None
+            ):
+                self.assertLen(
+                    layer.torch_params,
+                    expected_num_trainable_weights
+                    + expected_num_non_trainable_weights
+                    + expected_num_seed_generators,
+                    msg="Unexpected number of torch_params",
+                )
 
-            with tf.GradientTape() as g:
-                outputs = layer(inputs)
+        def run_output_asserts(layer, output, eager=False):
+            if expected_output_shape is not None:
+                if isinstance(expected_output_shape, tuple) and is_shape_tuple(
+                    expected_output_shape[0]
+                ):
+                    self.assertIsInstance(output, tuple)
+                    self.assertEqual(
+                        len(output),
+                        len(expected_output_shape),
+                        msg="Unexpected number of outputs",
+                    )
+                    output_shape = tuple(v.shape for v in output)
+                    self.assertEqual(
+                        expected_output_shape,
+                        output_shape,
+                        msg="Unexpected output shape",
+                    )
+                elif isinstance(expected_output_shape, tuple):
+                    self.assertEqual(
+                        expected_output_shape,
+                        output.shape,
+                        msg="Unexpected output shape",
+                    )
+                elif isinstance(expected_output_shape, dict):
+                    self.assertIsInstance(output, dict)
+                    self.assertEqual(
+                        set(output.keys()),
+                        set(expected_output_shape.keys()),
+                        msg="Unexpected output dict keys",
+                    )
+                    output_shape = {k: v.shape for k, v in output.items()}
+                    self.assertEqual(
+                        expected_output_shape,
+                        output_shape,
+                        msg="Unexpected output shape",
+                    )
+                elif isinstance(expected_output_shape, list):
+                    self.assertIsInstance(output, list)
+                    self.assertEqual(
+                        len(output),
+                        len(expected_output_shape),
+                        msg="Unexpected number of outputs",
+                    )
+                    output_shape = [v.shape for v in output]
+                    self.assertEqual(
+                        expected_output_shape,
+                        output_shape,
+                        msg="Unexpected output shape",
+                    )
+                else:
+                    raise ValueError(
+                        "The type of expected_output_shape is not supported"
+                    )
+            if expected_output_dtype is not None:
+                if isinstance(expected_output_dtype, tuple):
+                    self.assertIsInstance(output, tuple)
+                    self.assertEqual(
+                        len(output),
+                        len(expected_output_dtype),
+                        msg="Unexpected number of outputs",
+                    )
+                    output_dtype = tuple(
+                        backend.standardize_dtype(v.dtype) for v in output
+                    )
+                    self.assertEqual(
+                        expected_output_dtype,
+                        output_dtype,
+                        msg="Unexpected output dtype",
+                    )
+                elif isinstance(expected_output_dtype, dict):
+                    self.assertIsInstance(output, dict)
+                    self.assertEqual(
+                        set(output.keys()),
+                        set(expected_output_dtype.keys()),
+                        msg="Unexpected output dict keys",
+                    )
+                    output_dtype = {
+                        k: backend.standardize_dtype(v.dtype)
+                        for k, v in output.items()
+                    }
+                    self.assertEqual(
+                        expected_output_dtype,
+                        output_dtype,
+                        msg="Unexpected output dtype",
+                    )
+                elif isinstance(expected_output_dtype, list):
+                    self.assertIsInstance(output, list)
+                    self.assertEqual(
+                        len(output),
+                        len(expected_output_dtype),
+                        msg="Unexpected number of outputs",
+                    )
+                    output_dtype = [
+                        backend.standardize_dtype(v.dtype) for v in output
+                    ]
+                    self.assertEqual(
+                        expected_output_dtype,
+                        output_dtype,
+                        msg="Unexpected output dtype",
+                    )
+                else:
+                    output_dtype = tree.flatten(output)[0].dtype
+                    self.assertEqual(
+                        expected_output_dtype,
+                        backend.standardize_dtype(output_dtype),
+                        msg="Unexpected output dtype",
+                    )
+            if expected_output_sparse:
+                for x in tree.flatten(output):
+                    self.assertSparse(x)
+            if eager:
+                if expected_output is not None:
+                    self.assertEqual(type(expected_output), type(output))
+                    for ref_v, v in zip(
+                        tree.flatten(expected_output), tree.flatten(output)
+                    ):
+                        self.assertAllClose(
+                            ref_v, v, msg="Unexpected output value"
+                        )
+                if expected_num_losses is not None:
+                    self.assertLen(layer.losses, expected_num_losses)
+
+        def run_training_step(layer, input_data, output_data):
+            class TestModel(Model):
+                def __init__(self, layer):
+                    super().__init__()
+                    self.layer = layer
+
+                def call(self, x, training=False):
+                    return self.layer(x, training=training)
+
+            model = TestModel(layer)
+
+            data = (input_data, output_data)
+            if backend.backend() == "torch":
+                data = tree.map_structure(backend.convert_to_numpy, data)
+
+            def data_generator():
+                while True:
+                    yield data
+
+            # test the "default" path for each backend by setting
+            # jit_compile="auto".
+            # for tensorflow and jax backends auto is jitted
+            # Note that tensorflow cannot be jitted with sparse tensors
+            # for torch backend auto is eager
+            #
+            # NB: for torch, jit_compile=True turns on torchdynamo
+            #  which may not always succeed in tracing depending
+            #  on the model. Run your program with these env vars
+            #  to get debug traces of dynamo:
+            #    TORCH_LOGS="+dynamo"
+            #    TORCHDYNAMO_VERBOSE=1
+            #    TORCHDYNAMO_REPORT_GUARD_FAILURES=1
+            jit_compile = "auto"
+            if backend.backend() == "tensorflow" and input_sparse:
+                jit_compile = False
+            model.compile(optimizer="sgd", loss="mse", jit_compile=jit_compile)
+            model.fit(data_generator(), steps_per_epoch=1, verbose=0)
+
+        # Build test.
+        if input_data is not None or input_shape is not None:
+            if input_shape is None:
+                build_shape = tree.map_structure(
+                    lambda x: ops.shape(x), input_data
+                )
+            else:
+                build_shape = input_shape
+            layer = layer_cls(**init_kwargs)
+            if isinstance(build_shape, dict):
+                layer.build(**build_shape)
+            else:
+                layer.build(build_shape)
+            run_build_asserts(layer)
+
+            # Symbolic call test.
+            if input_shape is None:
+                keras_tensor_inputs = tree.map_structure(
+                    lambda x: create_keras_tensors(
+                        ops.shape(x), x.dtype, input_sparse
+                    ),
+                    input_data,
+                )
+            else:
+                keras_tensor_inputs = create_keras_tensors(
+                    input_shape, input_dtype, input_sparse
+                )
+            layer = layer_cls(**init_kwargs)
+            if isinstance(keras_tensor_inputs, dict):
+                keras_tensor_outputs = layer(
+                    **keras_tensor_inputs, **call_kwargs
+                )
+            else:
+                keras_tensor_outputs = layer(keras_tensor_inputs, **call_kwargs)
+            run_build_asserts(layer)
+            run_output_asserts(layer, keras_tensor_outputs, eager=False)
+
+            if expected_mask_shape is not None:
+                output_mask = layer.compute_mask(keras_tensor_inputs)
+                self.assertEqual(expected_mask_shape, output_mask.shape)
+
+        # Eager call test and compiled training test.
+        if input_data is not None or input_shape is not None:
+            if input_data is None:
+                input_data = create_eager_tensors(
+                    input_shape, input_dtype, input_sparse
+                )
+            layer = layer_cls(**init_kwargs)
+            if isinstance(input_data, dict):
+                output_data = layer(**input_data, **call_kwargs)
+            else:
+                output_data = layer(input_data, **call_kwargs)
+            run_output_asserts(layer, output_data, eager=True)
+
+            if run_training_check:
+                run_training_step(layer, input_data, output_data)
+
+            # Never test mixed precision on torch CPU. Torch lacks support.
+            if run_mixed_precision_check and backend.backend() == "torch":
+                import torch
+
+                run_mixed_precision_check = torch.cuda.is_available()
+
+            if run_mixed_precision_check:
+                layer = layer_cls(**{**init_kwargs, "dtype": "mixed_float16"})
+                input_spec = tree.map_structure(
+                    lambda spec: KerasTensor(
+                        spec.shape,
+                        dtype=(
+                            layer.compute_dtype
+                            if layer.autocast
+                            and backend.is_float_dtype(spec.dtype)
+                            else spec.dtype
+                        ),
+                    ),
+                    keras_tensor_inputs,
+                )
+                if isinstance(input_data, dict):
+                    output_data = layer(**input_data, **call_kwargs)
+                    output_spec = layer.compute_output_spec(**input_spec)
+                else:
+                    output_data = layer(input_data, **call_kwargs)
+                    output_spec = layer.compute_output_spec(input_spec)
+                for tensor, spec in zip(
+                    tree.flatten(output_data), tree.flatten(output_spec)
+                ):
+                    dtype = standardize_dtype(tensor.dtype)
+                    self.assertEqual(dtype, spec.dtype)
+                for weight in layer.weights:
+                    dtype = standardize_dtype(weight.dtype)
+                    if is_float_dtype(dtype):
+                        self.assertEqual(dtype, "float32")
 
-            self.assertIsInstance(
-                g.gradient(outputs, layer.kernel), tf.IndexedSlices
-            )
 
-    def test_dense_no_activation(self):
-        layer = layers.Dense(units=2, use_bias=False, activation=None)
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-            ]
-        )
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        self.assertEqual(layer.bias, None)
-        self.assertAllClose(layer(inputs), [[5.0, -6.0]])
+def tensorflow_uses_gpu():
+    return backend.backend() == "tensorflow" and uses_gpu()
 
-    def test_dense_without_activation_set(self):
-        layer = layers.Dense(units=2, use_bias=False)
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-            ]
-        )
-        layer.activation = None
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        self.assertEqual(layer.bias, None)
-        self.assertAllClose(layer(inputs), [[5.0, -6.0]])
 
-    def test_dense_with_activation(self):
-        layer = layers.Dense(units=2, use_bias=False, activation="relu")
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-            ]
-        )
+def jax_uses_gpu():
+    return backend.backend() == "jax" and uses_gpu()
 
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        output = layer(inputs)
-        expected_output = np.array([[5.0, 0.0]])
-        self.assertAllClose(output, expected_output)
-
-    def test_dense_constraints(self):
-        layer = layers.Dense(units=2, kernel_constraint="non_neg")
-        layer.build((None, 2))
-        self.assertIsInstance(layer.kernel.constraint, constraints.NonNeg)
-        layer = layers.Dense(units=2, bias_constraint="non_neg")
-        layer.build((None, 2))
-        self.assertIsInstance(layer.bias.constraint, constraints.NonNeg)
-
-    @pytest.mark.requires_trainable_backend
-    def test_enable_lora(self):
-        layer = layers.Dense(units=16)
-        layer.build((None, 8))
-        layer.enable_lora(4)
-        self.assertLen(layer.trainable_weights, 3)
-        self.assertLen(layer.non_trainable_weights, 1)
-        if backend.backend() == "torch":
-            self.assertLen(layer.torch_params, 4)
-        # Try eager call
-        x = np.random.random((64, 8))
-        y = np.random.random((64, 16))
-        _ = layer(x[:2])
-
-        init_lora_a_kernel_value = layer.lora_kernel_a.numpy()
-        init_lora_b_kernel_value = layer.lora_kernel_b.numpy()
-
-        # Try calling fit()
-        model = models.Sequential(
-            [
-                layer,
-            ]
-        )
-        model.compile(optimizer="sgd", loss="mse")
-        model.fit(x, y)
 
-        final_lora_a_kernel_value = layer.lora_kernel_a.numpy()
-        final_lora_b_kernel_value = layer.lora_kernel_b.numpy()
-        diff_a = np.max(
-            np.abs(init_lora_a_kernel_value - final_lora_a_kernel_value)
-        )
-        diff_b = np.max(
-            np.abs(init_lora_b_kernel_value - final_lora_b_kernel_value)
-        )
-        self.assertGreater(diff_a, 0.0)
-        self.assertGreater(diff_b, 0.0)
+def torch_uses_gpu():
+    return backend.backend() == "torch" and uses_gpu()
 
-        # Try saving and reloading the model
-        temp_filepath = os.path.join(self.get_temp_dir(), "lora_model.keras")
-        model.save(temp_filepath)
-
-        new_model = saving.load_model(temp_filepath)
-        self.assertTrue(new_model.layers[0].lora_enabled)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-        # Try saving and reloading the model's weights only
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "lora_model.weights.h5"
-        )
-        model.save_weights(temp_filepath)
 
-        # Load the file into a fresh, non-lora model
-        new_model = models.Sequential(
-            [
-                layers.Dense(units=16),
-            ]
-        )
-        new_model.build((None, 8))
-        new_model.load_weights(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-        # Try loading a normal checkpoint into a lora model
-        new_model.save_weights(temp_filepath)
-        model.load_weights(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-    @pytest.mark.requires_trainable_backend
-    def test_lora_weight_name(self):
-
-        class MyModel(models.Model):
-            def __init__(self):
-                super().__init__(name="mymodel")
-                self.dense = layers.Dense(16, name="dense")
-
-            def build(self, input_shape):
-                self.dense.build(input_shape)
-
-            def call(self, x):
-                return self.dense(x)
-
-        model = MyModel()
-        model.build((None, 8))
-        model.dense.enable_lora(4)
-        self.assertEqual(
-            model.dense.lora_kernel_a.path, "mymodel/dense/lora_kernel_a"
-        )
+def uses_gpu():
+    # Condition used to skip tests when using the GPU
+    devices = distribution.list_devices()
+    if any(d.startswith("gpu") for d in devices):
+        return True
+    return False
 
-    @pytest.mark.requires_trainable_backend
-    def test_lora_rank_argument(self):
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 5,
-                "activation": "sigmoid",
-                "kernel_regularizer": "l2",
-                "lora_rank": 2,
-            },
-            input_shape=(2, 3, 4),
-            expected_output_shape=(2, 3, 5),
-            expected_num_trainable_weights=3,
-            expected_num_non_trainable_weights=1,
-            expected_num_seed_generators=0,
-            expected_num_losses=2,  # we have 2 regularizers.
-            supports_masking=True,
-        )
 
-    def test_enable_lora_with_kernel_constraint(self):
-        layer = layers.Dense(units=2, kernel_constraint="max_norm")
-        with self.assertRaisesRegex(
-            ValueError, "incompatible with kernel constraints"
-        ):
-            layer.enable_lora(rank=2)
-
-    def test_enable_lora_on_unbuilt_layer(self):
-        layer = layers.Dense(units=2)
-        with self.assertRaisesRegex(
-            ValueError, "Cannot enable lora on a layer that isn't yet built"
-        ):
-            layer.enable_lora(rank=2)
-
-    def test_enable_lora_when_already_enabled(self):
-        layer = layers.Dense(units=2)
-        layer.build((None, 2))
-        layer.enable_lora(rank=2)
-        with self.assertRaisesRegex(ValueError, "lora is already enabled"):
-            layer.enable_lora(rank=2)
-
-    """Test quantization-related (int8 and float8) methods"""
-
-    @pytest.mark.skipif(
-        backend.backend() == "numpy",
-        reason=f"{backend.backend()} does not support ops.custom_gradient.",
+def create_keras_tensors(input_shape, dtype, sparse):
+    if isinstance(input_shape, dict):
+        return {
+            utils.removesuffix(k, "_shape"): KerasTensor(
+                v, dtype=dtype[k], sparse=sparse
+            )
+            for k, v in input_shape.items()
+        }
+    return map_shape_dtype_structure(
+        lambda shape, dt: KerasTensor(shape, dtype=dt, sparse=sparse),
+        input_shape,
+        dtype,
     )
-    def test_quantize_int8(self):
-        layer = layers.Dense(units=16)
-        layer.build((None, 8))
-        x = np.random.random((2, 8))
-        y_float = layer(x)
-        layer.quantize("int8")
-
-        # Verify weights dtype
-        self.assertEqual(backend.standardize_dtype(layer._kernel.dtype), "int8")
-        self.assertEqual(
-            backend.standardize_dtype(layer.kernel_scale.dtype),
-            layer.variable_dtype,
-        )
-
-        # Try eager call and verify output correctness
-        y_quantized = layer(x)
-        mse = ops.mean(ops.square(y_float - y_quantized))
-        self.assertLess(mse, 1e-3)  # A weak correctness test
-
-        # Try saving and reloading the model
-        model = models.Sequential([layer])
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_model.keras"
-        )
-        model.save(temp_filepath)
-        new_model = saving.load_model(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-        # Try saving and reloading the model's weights only
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_model.weights.h5"
-        )
-        model.save_weights(temp_filepath)
-
-        # Try lora
-        layer = layers.Dense(units=16)
-        layer.build((None, 8))
-        layer.enable_lora(4)
-        layer.quantize("int8")
-        x = np.random.random((2, 8))
-        _ = layer(x)
-
-        # Try building with quantized dtype policy
-        layer = layers.Dense(units=16, dtype="int8_from_mixed_bfloat16")
-        layer.build((None, 8))
-        self.assertEqual(backend.standardize_dtype(layer._kernel.dtype), "int8")
-        self.assertEqual(
-            backend.standardize_dtype(layer.kernel_scale.dtype), "float32"
-        )
 
-    @parameterized.named_parameters(
-        ("int8", "int8"),
-        ("float8", "float8"),
-    )
-    def test_quantize_on_unbuilt_layer(self, mode):
-        layer = layers.Dense(units=2)
-        with self.assertRaisesRegex(
-            ValueError, "Cannot quantize a layer that isn't yet built."
-        ):
-            layer.quantize(mode)
-
-    @parameterized.named_parameters(
-        ("int8", "int8"),
-        ("float8", "float8"),
-    )
-    def test_quantize_on_subclass(self, mode):
-        class MyDense(layers.Dense):
-            pass
-
-        layer = MyDense(units=16)
-        layer.build((None, 8))
-        with self.assertRaises(NotImplementedError):
-            layer.quantize(mode)
-
-    @parameterized.named_parameters(
-        ("int8", "int8"),
-        ("float8", "float8"),
-    )
-    def test_quantize_when_already_quantized(self, mode):
-        layer = layers.Dense(units=2)
-        layer.build((None, 2))
-        layer.quantize(mode)
-        for m in ["int8", "float8"]:
-            with self.assertRaisesRegex(
-                ValueError, "is already quantized with dtype_policy="
-            ):
-                layer.quantize(m)
 
-    @parameterized.named_parameters(
-        ("int8", "int8_from_float32"),
-        ("float8", "float8_from_float32"),
-    )
-    def test_quantize_when_already_quantized_using_dtype_argument(self, mode):
-        layer = layers.Dense(units=2, dtype=mode)
-        layer.build((None, 2))
-        for m in ["int8", "float8"]:
-            with self.assertRaisesRegex(
-                ValueError, "is already quantized with dtype_policy="
-            ):
-                layer.quantize(m)
+def create_eager_tensors(input_shape, dtype, sparse):
+    from keras.src.backend import random
 
-    @parameterized.named_parameters(
-        ("int8", "int8_from_float32", 3),
-        ("float8", "float8_from_float32", 8),
-    )
-    def test_quantize_by_setting_dtype_policy(
-        self, policy, expected_num_variables
+    if set(tree.flatten(dtype)).difference(
+        ["float16", "float32", "float64", "int16", "int32", "int64"]
     ):
-        layer = layers.Dense(units=2)
-        layer.build((None, 2))
-        layer.dtype_policy = policy
-        self.assertLen(layer.variables, expected_num_variables)
-
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_int8_dtype_argument(self):
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 5,
-                "dtype": "int8_from_mixed_bfloat16",
-            },
-            input_shape=(2, 3, 4),
-            expected_output_shape=(2, 3, 5),
-            expected_num_trainable_weights=1,
-            expected_num_non_trainable_weights=2,
-            expected_num_seed_generators=0,
-            expected_num_losses=0,
-            supports_masking=True,
+        raise ValueError(
+            "dtype must be a standard float or int dtype. "
+            f"Received: dtype={dtype}"
         )
 
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_int8_when_lora_enabled(self):
-        # Note that saving and loading with lora_enabled and quantized are
-        # lossy, so we use a weak correctness test for model outputs (atol=0.5).
-        config = dict(units=16)
-        layer = layers.Dense(**config)
-        layer.build((None, 8))
-        layer.enable_lora(4)
-        layer.quantize("int8")
-        self.assertLen(layer.trainable_weights, 3)
-        self.assertLen(layer.non_trainable_weights, 2)
-        if backend.backend() == "torch":
-            self.assertLen(layer.torch_params, 5)
-
-        # Try calling fit()
-        init_lora_a_kernel_value = layer.lora_kernel_a.numpy()
-        init_lora_b_kernel_value = layer.lora_kernel_b.numpy()
-        x = np.random.random((64, 8))
-        y = np.random.random((64, 16))
-        model = models.Sequential([layer])
-        model.compile(optimizer="sgd", loss="mse")
-        model.fit(x, y, epochs=2)
-
-        final_lora_a_kernel_value = layer.lora_kernel_a.numpy()
-        final_lora_b_kernel_value = layer.lora_kernel_b.numpy()
-        diff_a = np.max(
-            np.abs(init_lora_a_kernel_value - final_lora_a_kernel_value)
-        )
-        diff_b = np.max(
-            np.abs(init_lora_b_kernel_value - final_lora_b_kernel_value)
-        )
-        self.assertGreater(diff_a, 0.0)
-        self.assertGreater(diff_b, 0.0)
-
-        # Try saving and reloading the model
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_lora_model.keras"
-        )
-        model.save(temp_filepath)
-        new_model = saving.load_model(temp_filepath)
-        self.assertTrue(new_model.layers[0].lora_enabled)
-        self.assertAllClose(model.predict(x), new_model.predict(x), atol=0.5)
-
-        # Try saving and reloading the model's weights only
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_lora_model.weights.h5"
-        )
-        model.save_weights(temp_filepath)
-        new_model = models.Sequential([layers.Dense(**config)])
-        new_model.build((None, 8))
-        new_model.quantize("int8")
-        new_model.load_weights(temp_filepath)
-        self.assertFalse(new_model.layers[0].lora_enabled)
-        self.assertAllClose(model.predict(x), new_model.predict(x), atol=0.5)
-
-        # Try loading a normal checkpoint into a lora model
-        new_model.save_weights(temp_filepath)
-        model.load_weights(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x), atol=0.5)
-
-        # Test export and TFSMLayer reloading when using tensorflow backend
+    if sparse:
         if backend.backend() == "tensorflow":
             import tensorflow as tf
 
-            temp_filepath = os.path.join(self.get_temp_dir(), "exported_model")
-            ref_input = tf.random.normal((2, 8))
-            ref_output = model(ref_input)
-            export_lib.export_model(model, temp_filepath)
-            reloaded_layer = export_lib.TFSMLayer(temp_filepath)
-            self.assertAllClose(
-                reloaded_layer(ref_input), ref_output, atol=1e-7
-            )
-            self.assertLen(reloaded_layer.weights, len(model.weights))
-            self.assertLen(
-                reloaded_layer.trainable_weights, len(model.trainable_weights)
-            )
-            self.assertLen(
-                reloaded_layer.non_trainable_weights,
-                len(model.non_trainable_weights),
-            )
-
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_float8_dtype_argument(self):
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 5,
-                "dtype": "float8_from_mixed_bfloat16",
-            },
-            input_shape=(2, 3, 4),
-            expected_output_shape=(2, 3, 5),
-            expected_num_trainable_weights=8,
-            expected_num_non_trainable_weights=0,
-            expected_num_seed_generators=0,
-            expected_num_losses=0,
-            supports_masking=True,
-        )
+            def create_fn(shape, dt):
+                rng = np.random.default_rng(0)
+                x = (4 * rng.standard_normal(shape)).astype(dt)
+                x = np.multiply(x, rng.random(shape) < 0.7)
+                return tf.sparse.from_dense(x)
 
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_float8(self):
-        import ml_dtypes
-
-        from keras.src import quantizers
-
-        layer = layers.Dense(units=32)
-        layer.build((None, 16))
-        layer.quantize("float8")
-        optimizer = optimizers.AdamW(learning_rate=0.1)
-        optimizer.build(layer.trainable_variables)
-
-        def loss_fn(x, dy):
-            y = layer(x, training=True)
-            loss = y * ops.cast(dy, y.dtype)
-            return ops.sum(loss)
+        elif backend.backend() == "jax":
+            import jax.experimental.sparse as jax_sparse
 
-        if backend.backend() == "tensorflow":
-            import tensorflow as tf
+            def create_fn(shape, dt):
+                rng = np.random.default_rng(0)
+                x = (4 * rng.standard_normal(shape)).astype(dt)
+                x = np.multiply(x, rng.random(shape) < 0.7)
+                return jax_sparse.BCOO.fromdense(x, n_batch=1)
 
-            @tf.function(jit_compile=True)
-            def train_one_step(x, dy):
-                with tf.GradientTape() as tape:
-                    loss = loss_fn(x, dy)
-                grads = tape.gradient(loss, layer.trainable_variables)
-                optimizer.apply(grads, layer.trainable_variables)
+        else:
+            raise ValueError(
+                f"Sparse is unsupported with backend {backend.backend()}"
+            )
 
-        elif backend.backend() == "jax":
-            import jax
+    else:
 
-            def stateless_loss_fn(trainable_variables, x, dy):
-                y = layer.stateless_call(trainable_variables, [], x)[0]
-                loss = y * ops.cast(dy, y.dtype)
-                return ops.sum(loss)
-
-            grad_fn = jax.jit(jax.grad(stateless_loss_fn))
-
-            def train_one_step(x, dy):
-                trainable_variables = [
-                    v.value for v in layer.trainable_variables
-                ]
-                optimizer_variables = [v.value for v in optimizer.variables]
-                grads = grad_fn(trainable_variables, x, dy)
-                trainable_variables, optimizer_variables = (
-                    optimizer.stateless_apply(
-                        optimizer_variables, grads, trainable_variables
-                    )
-                )
-                for variable, value in zip(
-                    layer.trainable_variables, trainable_variables
-                ):
-                    variable.assign(value)
-                for variable, value in zip(
-                    optimizer.variables, optimizer_variables
-                ):
-                    variable.assign(value)
+        def create_fn(shape, dt):
+            return ops.cast(
+                random.uniform(shape, dtype="float32") * 3, dtype=dt
+            )
 
-        elif backend.backend() == "torch":
+    if isinstance(input_shape, dict):
+        return {
+            utils.removesuffix(k, "_shape"): create_fn(v, dtype[k])
+            for k, v in input_shape.items()
+        }
+    return map_shape_dtype_structure(create_fn, input_shape, dtype)
 
-            def train_one_step(x, dy):
-                layer.zero_grad()
-                loss = loss_fn(x, dy)
-                loss.backward()
-                grads = [v.value.grad for v in layer.trainable_variables]
-                optimizer.apply(grads, layer.trainable_variables)
-
-        scale_x, amax_history_x = ops.ones(()), ops.zeros((1024,))
-        scale_k, amax_history_k = ops.ones(()), ops.zeros((1024,))
-        scale_g, amax_history_g = ops.ones(()), ops.zeros((1024,))
-        e4m3_max = ops.cast(
-            float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
-        )
-        e5m2_max = ops.cast(
-            float(ml_dtypes.finfo("float8_e5m2").max), "float32"
-        )
 
-        for _ in range(3):
-            x = random.normal((16, 16), dtype="float32")
-            g = random.normal((16, 32), dtype="float32")
-            k = ops.convert_to_tensor(layer._kernel)
-
-            # Manually compute the expected amax history and scaling factors.
-            amax_from_history_x = ops.max(amax_history_x)
-            amax_from_history_k = ops.max(amax_history_k)
-            amax_from_history_g = ops.max(amax_history_g)
-            scale_x = quantizers.compute_float8_scale(
-                amax_from_history_x, scale_x, e4m3_max
-            )
-            scale_k = quantizers.compute_float8_scale(
-                amax_from_history_k, scale_k, e4m3_max
-            )
-            scale_g = quantizers.compute_float8_scale(
-                amax_from_history_g, scale_g, e5m2_max
-            )
-            amax_history_x = quantizers.compute_float8_amax_history(
-                x, amax_history_x
-            )
-            amax_history_k = quantizers.compute_float8_amax_history(
-                k, amax_history_k
-            )
-            amax_history_g = quantizers.compute_float8_amax_history(
-                g, amax_history_g
-            )
-
-            train_one_step(x, g)
-
-            self.assertAllClose(layer.inputs_amax_history, amax_history_x)
-            self.assertAllClose(layer.kernel_amax_history, amax_history_k)
-            self.assertAllClose(layer.outputs_grad_amax_history, amax_history_g)
-            self.assertAllClose(layer.inputs_scale, scale_x)
-            self.assertAllClose(layer.kernel_scale, scale_k)
-            self.assertAllClose(layer.outputs_grad_scale, scale_g)
-
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_float8_fitting(self):
-        config = dict(units=16)
-        layer = layers.Dense(**config)
-        layer.build((None, 8))
-        layer.quantize("float8")
-        self.assertLen(layer.trainable_weights, 8)
-        self.assertLen(layer.non_trainable_weights, 0)
-
-        # Try calling fit()
-        x = np.random.random((64, 8))
-        y = np.random.random((64, 16))
-        model = models.Sequential([layer])
-        model.compile(optimizer="sgd", loss="mse")
-        model.fit(x, y, epochs=2)
-
-        # Try saving and reloading the model
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_float8_model.keras"
-        )
-        model.save(temp_filepath)
-        new_model = saving.load_model(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-        # Try saving and reloading the model's weights only
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_float8_model.weights.h5"
+def is_shape_tuple(x):
+    return isinstance(x, (list, tuple)) and all(
+        isinstance(e, (int, type(None))) for e in x
+    )
+
+
+def map_shape_dtype_structure(fn, shape, dtype):
+    """Variant of tree.map_structure that operates on shape tuples."""
+    if is_shape_tuple(shape):
+        return fn(tuple(shape), dtype)
+    if isinstance(shape, list):
+        return [
+            map_shape_dtype_structure(fn, s, d) for s, d in zip(shape, dtype)
+        ]
+    if isinstance(shape, tuple):
+        return tuple(
+            map_shape_dtype_structure(fn, s, d) for s, d in zip(shape, dtype)
+        )
+    if isinstance(shape, dict):
+        return {
+            k: map_shape_dtype_structure(fn, v, dtype[k])
+            for k, v in shape.items()
+        }
+    else:
+        raise ValueError(
+            f"Cannot map function to unknown objects {shape} and {dtype}"
         )
-        model.save_weights(temp_filepath)
-        new_model = models.Sequential([layers.Dense(**config)])
-        new_model.build((None, 8))
-        new_model.quantize("float8")
-        new_model.load_weights(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
 
-        # Test export and TFSMLayer reloading when using tensorflow backend
-        if backend.backend() == "tensorflow":
-            import tensorflow as tf
 
-            temp_filepath = os.path.join(self.get_temp_dir(), "exported_model")
-            ref_input = tf.random.normal((2, 8))
-            ref_output = model(ref_input)
-            export_lib.export_model(model, temp_filepath)
-            reloaded_layer = export_lib.TFSMLayer(temp_filepath)
-            self.assertAllClose(reloaded_layer(ref_input), ref_output)
-            self.assertLen(reloaded_layer.weights, len(model.weights))
-            self.assertLen(
-                reloaded_layer.trainable_weights, len(model.trainable_weights)
-            )
-            self.assertLen(
-                reloaded_layer.non_trainable_weights,
-                len(model.non_trainable_weights),
-            )
+def get_seed_generators(layer):
+    """Get a List of all seed generators in the layer recursively."""
+    seed_generators = []
+    seen_ids = set()
+    for sublayer in layer._flatten_layers(True, True):
+        for sg in sublayer._seed_generators:
+            if id(sg) not in seen_ids:
+                seed_generators.append(sg)
+                seen_ids.add(id(sg))
+    return seed_generators
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/einsum_dense.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,59 +253,63 @@
     def save_own_variables(self, store):
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         kernel_value, kernel_scale = self._get_kernel_with_merged_lora()
-        store["0"] = kernel_value
+        target_variables = [kernel_value]
         if self.bias is not None:
-            store["1"] = self.bias
+            target_variables.append(self.bias)
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             mode = self.dtype_policy.quantization_mode
             if mode == "int8":
-                store["2"] = kernel_scale
+                target_variables.append(kernel_scale)
             elif mode == "float8":
-                store["2"] = self.inputs_scale
-                store["3"] = self.inputs_amax_history
-                store["4"] = self.kernel_scale
-                store["5"] = self.kernel_amax_history
-                store["6"] = self.outputs_grad_scale
-                store["7"] = self.outputs_grad_amax_history
+                target_variables.append(self.inputs_scale)
+                target_variables.append(self.inputs_amax_history)
+                target_variables.append(self.kernel_scale)
+                target_variables.append(self.kernel_amax_history)
+                target_variables.append(self.outputs_grad_scale)
+                target_variables.append(self.outputs_grad_amax_history)
             else:
                 raise NotImplementedError(
                     self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
                 )
+        for i, variable in enumerate(target_variables):
+            store[str(i)] = variable
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
-        self._kernel.assign(store["0"])
+        target_variables = [self._kernel]
         if self.bias is not None:
-            self.bias.assign(store["1"])
+            target_variables.append(self.bias)
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             mode = self.dtype_policy.quantization_mode
             if mode == "int8":
-                self.kernel_scale.assign(store["2"])
+                target_variables.append(self.kernel_scale)
             elif mode == "float8":
-                self.inputs_scale.assign(store["2"])
-                self.inputs_amax_history.assign(store["3"])
-                self.kernel_scale.assign(store["4"])
-                self.kernel_amax_history.assign(store["5"])
-                self.outputs_grad_scale.assign(store["6"])
-                self.outputs_grad_amax_history.assign(store["7"])
+                target_variables.append(self.inputs_scale)
+                target_variables.append(self.inputs_amax_history)
+                target_variables.append(self.kernel_scale)
+                target_variables.append(self.kernel_amax_history)
+                target_variables.append(self.outputs_grad_scale)
+                target_variables.append(self.outputs_grad_amax_history)
             else:
                 raise NotImplementedError(
                     self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
                 )
+        for i, variable in enumerate(target_variables):
+            variable.assign(store[str(i)])
         if self.lora_enabled:
             self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
             self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
 
     def get_config(self):
         base_config = super().get_config()
         config = {
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,41 +195,45 @@
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         embeddings_value, embeddings_scale = (
             self._get_embeddings_with_merged_lora()
         )
-        store["0"] = embeddings_value
+        target_variables = [embeddings_value]
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             mode = self.dtype_policy.quantization_mode
             if mode == "int8":
-                store["1"] = embeddings_scale
+                target_variables.append(embeddings_scale)
             else:
                 raise NotImplementedError(
                     self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
                 )
+        for i, variable in enumerate(target_variables):
+            store[str(i)] = variable
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
-        self._embeddings.assign(store["0"])
+        target_variables = [self._embeddings]
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             mode = self.dtype_policy.quantization_mode
             if mode == "int8":
-                self.embeddings_scale.assign(store["1"])
+                target_variables.append(self.embeddings_scale)
             else:
                 raise NotImplementedError(
                     self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
                 )
+        for i, variable in enumerate(target_variables):
+            variable.assign(store[str(i)])
         if self.lora_enabled:
             self.lora_embeddings_a.assign(
                 ops.zeros(self.lora_embeddings_a.shape)
             )
             self.lora_embeddings_b.assign(
                 ops.zeros(self.lora_embeddings_b.shape)
             )
@@ -307,25 +311,27 @@
             )
 
     def _int8_build(
         self,
         embeddings_initializer="zeros",
         embeddings_scale_initializer="ones",
     ):
-        self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
         self._embeddings = self.add_weight(
             name="embeddings",
             shape=(self.input_dim, self.output_dim),
             initializer=embeddings_initializer,
             dtype="int8",
             trainable=False,
         )
+        # We choose to reduce the axis of `output_dim` because, typically,
+        # `input_dim` is larger than `output_dim`. This reduces quantization
+        # error.
         self.embeddings_scale = self.add_weight(
             name="embeddings_scale",
-            shape=(self.output_dim,),
+            shape=(self.input_dim,),
             initializer=embeddings_scale_initializer,
             trainable=False,
         )
         self._is_quantized = True
 
     def quantized_call(self, inputs):
         if self.dtype_policy.quantization_mode == "int8":
@@ -337,19 +343,20 @@
             )
 
     def _int8_call(self, inputs):
         # We cannot update quantized self._embeddings, so the custom gradient is
         # not needed
         if backend.standardize_dtype(inputs.dtype) not in ("int32", "int64"):
             inputs = ops.cast(inputs, "int32")
+        embeddings_scale = ops.take(self.embeddings_scale, inputs, axis=0)
         outputs = ops.take(self._embeddings, inputs, axis=0)
         # De-scale outputs
-        outputs = ops.cast(outputs, self.compute_dtype)
         outputs = ops.divide(
-            outputs, ops.expand_dims(self.embeddings_scale, axis=0)
+            ops.cast(outputs, dtype=self.compute_dtype),
+            ops.expand_dims(embeddings_scale, axis=-1),
         )
         if self.lora_enabled:
             lora_outputs = ops.take(self.lora_embeddings_a, inputs, axis=0)
             lora_outputs = ops.matmul(lora_outputs, self.lora_embeddings_b)
             outputs = ops.add(outputs, lora_outputs)
         return outputs
 
@@ -371,22 +378,20 @@
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
             # We set the internal `self._dtype_policy` instead of using the
             # setter to avoid double `quantize` call
             self._dtype_policy = dtype_policies.get(quantized_dtype)
 
         self._tracker.unlock()
         if mode == "int8":
-            # Configure `self.inputs_quantizer`
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
             # Quantize `self._embeddings` to int8 and compute corresponding
             # scale
             embeddings_value, embeddings_scale = quantizers.abs_max_quantize(
-                self._embeddings, axis=0
+                self._embeddings, axis=-1
             )
-            embeddings_scale = ops.squeeze(embeddings_scale, axis=0)
+            embeddings_scale = ops.squeeze(embeddings_scale, axis=-1)
             self._untrack_variable(self._embeddings)
             del self._embeddings
             # Utilize a lambda expression as an initializer to prevent adding a
             # large constant to the computation graph.
             self._int8_build(
                 lambda shape, dtype: embeddings_value,
                 lambda shape, dtype: embeddings_scale,
@@ -404,19 +409,19 @@
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             embeddings_value = self._embeddings
             embeddings_scale = self.embeddings_scale
             if self.lora_enabled:
                 # Dequantize & quantize to merge lora weights into embeddings
                 # Note that this is a lossy compression
                 embeddings_value = ops.divide(
-                    embeddings_value, embeddings_scale
+                    embeddings_value, ops.expand_dims(embeddings_scale, axis=-1)
                 )
                 embeddings_value = ops.add(
                     embeddings_value,
                     ops.matmul(self.lora_embeddings_a, self.lora_embeddings_b),
                 )
                 embeddings_value, embeddings_scale = (
-                    quantizers.abs_max_quantize(embeddings_value, axis=0)
+                    quantizers.abs_max_quantize(embeddings_value, axis=-1)
                 )
-                embeddings_scale = ops.squeeze(embeddings_scale, axis=0)
+                embeddings_scale = ops.squeeze(embeddings_scale, axis=-1)
             return embeddings_value, embeddings_scale
         return self.embeddings, None
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/identity.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/masking.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/input_spec.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/layer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/add.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/average.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/backend.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/layers.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/losses.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/losses/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/losses/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,16 +131,16 @@
 @keras_export("keras.losses.deserialize")
 def deserialize(name, custom_objects=None):
     """Deserializes a serialized loss class/function instance.
 
     Args:
         name: Loss configuration.
         custom_objects: Optional dictionary mapping names (strings) to custom
-          objects (classes and functions) to be considered during
-          deserialization.
+            objects (classes and functions) to be considered during
+            deserialization.
 
     Returns:
         A Keras `Loss` instance or a loss function.
     """
     return serialization_lib.deserialize_keras_object(
         name,
         module_objects=ALL_OBJECTS_DICT,
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/losses/loss.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/losses/losses.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/metric.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/models/cloning.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/models/functional.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/models/model.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/models/sequential.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/core.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/function.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/image.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/linalg.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/math.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/nn.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/node.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/numpy.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -5412,40 +5412,53 @@
     """
     if any_symbolic_tensors((x1, x2)):
         return Vdot().symbolic_call(x1, x2)
     return backend.numpy.vdot(x1, x2)
 
 
 @keras_export(["keras.ops.vectorize", "keras.ops.numpy.vectorize"])
-def vectorize(pyfunc):
+def vectorize(pyfunc, *, excluded=None, signature=None):
     """Turn a function into a vectorized function.
 
     Example:
 
     ```python
     def myfunc(a, b):
         return a + b
 
     vfunc = np.vectorize(myfunc)
     y = vfunc([1, 2, 3, 4], 2)  # Returns Tensor([3, 4, 5, 6])
     ```
 
     Args:
         pyfunc: Callable of a single tensor argument.
+        excluded: Optional set of integers representing
+            positional arguments for which the function
+            will not be vectorized.
+            These will be passed directly to `pyfunc` unmodified.
+        signature: Optional generalized universal function signature,
+            e.g., `"(m,n),(n)->(m)"` for vectorized
+            matrix-vector multiplication. If provided,
+            `pyfunc` will be called with (and expected to return)
+            arrays with shapes given by the size of corresponding
+            core dimensions. By default, `pyfunc` is assumed
+            to take scalars tensors as input and output.
 
     Returns:
         A new function that applies `pyfunc` to every element
         of its input along axis 0 (the batch axis).
     """
     if not callable(pyfunc):
         raise ValueError(
             "Expected argument `pyfunc` to be a callable. "
             f"Received: pyfunc={pyfunc}"
         )
-    return backend.numpy.vectorize(pyfunc)
+    return backend.numpy.vectorize(
+        pyfunc, excluded=excluded, signature=signature
+    )
 
 
 class Vstack(Operation):
     def call(self, xs):
         return backend.numpy.vstack(xs)
 
     def compute_output_spec(self, xs):
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/operation.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adamax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,139 +1,156 @@
 from keras.src import ops
 from keras.src.api_export import keras_export
 from keras.src.optimizers import optimizer
 
 
-@keras_export(["keras.optimizers.Adadelta"])
-class Adadelta(optimizer.Optimizer):
-    """Optimizer that implements the Adadelta algorithm.
-
-    Adadelta optimization is a stochastic gradient descent method that is based
-    on adaptive learning rate per dimension to address two drawbacks:
-
-    - The continual decay of learning rates throughout training.
-    - The need for a manually selected global learning rate.
-
-    Adadelta is a more robust extension of Adagrad that adapts learning rates
-    based on a moving window of gradient updates, instead of accumulating all
-    past gradients. This way, Adadelta continues learning even when many updates
-    have been done. Compared to Adagrad, in the original version of Adadelta you
-    don't have to set an initial learning rate. In this version, the initial
-    learning rate can be set, as in most other Keras optimizers.
+@keras_export(["keras.optimizers.Adamax"])
+class Adamax(optimizer.Optimizer):
+    """Optimizer that implements the Adamax algorithm.
+
+    Adamax, a variant of Adam based on the infinity norm, is a first-order
+    gradient-based optimization method. Due to its capability of adjusting the
+    learning rate based on data characteristics, it is suited to learn
+    time-variant process, e.g., speech data with dynamically changed noise
+    conditions. Default parameters follow those provided in the paper (see
+    references below).
+
+    Initialization:
+
+    ```python
+    m = 0  # Initialize initial 1st moment vector
+    u = 0  # Initialize the exponentially weighted infinity norm
+    t = 0  # Initialize timestep
+    ```
+
+    The update rule for parameter `w` with gradient `g` is described at the end
+    of section 7.1 of the paper (see the referenece section):
+
+    ```python
+    t += 1
+    m = beta1 * m + (1 - beta) * g
+    u = max(beta2 * u, abs(g))
+    current_lr = learning_rate / (1 - beta1 ** t)
+    w = w - current_lr * m / (u + epsilon)
+    ```
 
     Args:
         learning_rate: A float, a
             `keras.optimizers.schedules.LearningRateSchedule` instance, or
             a callable that takes no arguments and returns the actual value to
-            use. The learning rate. Defaults to `0.001`. Note that `Adadelta`
-            tends to benefit from higher initial learning rate values compared
-            to other optimizers. To match the exact form in the original paper,
-            use 1.0.
-        rho: A floating point value. The decay rate. Defaults to `0.95`.
-        epsilon: Small floating point value for maintaining numerical stability.
-        {{base_optimizer_keyword_args}}
+            use. The learning rate. Defaults to `0.001`.
+        beta_1: A float value or a constant float tensor. The exponential decay
+            rate for the 1st moment estimates.
+        beta_2: A float value or a constant float tensor. The exponential decay
+            rate for the exponentially weighted infinity norm.
+        epsilon: A small constant for numerical stability.
+            {{base_optimizer_keyword_args}}
 
     Reference:
 
-    - [Zeiler, 2012](http://arxiv.org/abs/1212.5701)
+    - [Kingma et al., 2014](http://arxiv.org/abs/1412.6980)
     """
 
     def __init__(
         self,
         learning_rate=0.001,
-        rho=0.95,
+        beta_1=0.9,
+        beta_2=0.999,
         epsilon=1e-7,
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
         loss_scale_factor=None,
         gradient_accumulation_steps=None,
-        name="adadelta",
+        name="adamax",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
+            name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
             loss_scale_factor=loss_scale_factor,
             gradient_accumulation_steps=gradient_accumulation_steps,
-            name=name,
             **kwargs,
         )
-        self.rho = rho
+        self.beta_1 = beta_1
+        self.beta_2 = beta_2
         self.epsilon = epsilon
 
     def build(self, var_list):
+        """Initialize optimizer variables.
+
+        Adamax optimizer has 2 types of variables: momentums (denoted as m),
+        exponentially weighted infinity norm (denoted as u).
+
+        Args:
+            var_list: list of model variables to build Adamax variables on.
+        """
         if self.built:
             return
         super().build(var_list)
-        self._accumulated_grads = []
-        self._accumulated_delta_vars = []
+        self._m = []
+        self._u = []
         for var in var_list:
-            self._accumulated_grads.append(
-                self.add_variable_from_reference(var, "accumulated_grad")
+            self._m.append(
+                self.add_variable_from_reference(
+                    reference_variable=var, name="momentum"
+                )
             )
-            self._accumulated_delta_vars.append(
-                self.add_variable_from_reference(var, "accumulated_delta_var")
+            self._u.append(
+                self.add_variable_from_reference(
+                    reference_variable=var, name="norm"
+                )
             )
 
-    def update_step(self, grad, variable, learning_rate):
+    def update_step(self, gradient, variable, learning_rate):
         """Update step given gradient and the associated model variable."""
         lr = ops.cast(learning_rate, variable.dtype)
-        grad = ops.cast(grad, variable.dtype)
-
-        rho = self.rho
-        accumulated_grad = self._accumulated_grads[
-            self._get_variable_index(variable)
-        ]
-        accumulated_delta_var = self._accumulated_delta_vars[
-            self._get_variable_index(variable)
-        ]
+        gradient = ops.cast(gradient, variable.dtype)
+        local_step = ops.cast(self.iterations + 1, variable.dtype)
+        beta_1_power = ops.power(
+            ops.cast(self.beta_1, variable.dtype), local_step
+        )
 
-        def rms(x):
-            return ops.sqrt(ops.add(x, self.epsilon))
+        m = self._m[self._get_variable_index(variable)]
+        u = self._u[self._get_variable_index(variable)]
 
+        self.assign_add(
+            m, ops.multiply(ops.subtract(gradient, m), (1 - self.beta_1))
+        )
         self.assign(
-            accumulated_grad,
-            ops.add(
-                rho * accumulated_grad, ops.multiply(1 - rho, ops.square(grad))
-            ),
+            u, ops.maximum(ops.multiply(self.beta_2, u), ops.abs(gradient))
         )
-        delta_var = ops.negative(
+        self.assign_sub(
+            variable,
             ops.divide(
-                ops.multiply(rms(accumulated_delta_var), grad),
-                rms(accumulated_grad),
-            )
-        )
-        self.assign(
-            accumulated_delta_var,
-            ops.add(
-                ops.multiply(rho, accumulated_delta_var),
-                ops.multiply(1 - rho, ops.square(delta_var)),
+                ops.multiply(lr, m),
+                ops.multiply((1 - beta_1_power), ops.add(u, self.epsilon)),
             ),
         )
-        self.assign_add(variable, ops.multiply(lr, delta_var))
 
     def get_config(self):
         config = super().get_config()
 
         config.update(
             {
-                "rho": self.rho,
+                "beta_1": self.beta_1,
+                "beta_2": self.beta_2,
                 "epsilon": self.epsilon,
             }
         )
         return config
 
 
-Adadelta.__doc__ = Adadelta.__doc__.replace(
+Adamax.__doc__ = Adamax.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adam.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/lion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,65 @@
 from keras.src import ops
 from keras.src.api_export import keras_export
 from keras.src.optimizers import optimizer
 
 
-@keras_export(["keras.optimizers.Adamax"])
-class Adamax(optimizer.Optimizer):
-    """Optimizer that implements the Adamax algorithm.
-
-    Adamax, a variant of Adam based on the infinity norm, is a first-order
-    gradient-based optimization method. Due to its capability of adjusting the
-    learning rate based on data characteristics, it is suited to learn
-    time-variant process, e.g., speech data with dynamically changed noise
-    conditions. Default parameters follow those provided in the paper (see
-    references below).
-
-    Initialization:
-
-    ```python
-    m = 0  # Initialize initial 1st moment vector
-    u = 0  # Initialize the exponentially weighted infinity norm
-    t = 0  # Initialize timestep
-    ```
-
-    The update rule for parameter `w` with gradient `g` is described at the end
-    of section 7.1 of the paper (see the referenece section):
-
-    ```python
-    t += 1
-    m = beta1 * m + (1 - beta) * g
-    u = max(beta2 * u, abs(g))
-    current_lr = learning_rate / (1 - beta1 ** t)
-    w = w - current_lr * m / (u + epsilon)
-    ```
+@keras_export(["keras.optimizers.Lion"])
+class Lion(optimizer.Optimizer):
+    """Optimizer that implements the Lion algorithm.
+
+    The Lion optimizer is a stochastic-gradient-descent method that uses the
+    sign operator to control the magnitude of the update, unlike other adaptive
+    optimizers such as Adam that rely on second-order moments. This make
+    Lion more memory-efficient as it only keeps track of the momentum. According
+    to the authors (see reference), its performance gain over Adam grows with
+    the batch size. Because the update of Lion is produced through the sign
+    operation, resulting in a larger norm, a suitable learning rate for Lion is
+    typically 3-10x smaller than that for AdamW. The weight decay for Lion
+    should be in turn 3-10x larger than that for AdamW to maintain a
+    similar strength (lr * wd).
 
     Args:
         learning_rate: A float, a
             `keras.optimizers.schedules.LearningRateSchedule` instance, or
             a callable that takes no arguments and returns the actual value to
             use. The learning rate. Defaults to `0.001`.
-        beta_1: A float value or a constant float tensor. The exponential decay
-            rate for the 1st moment estimates.
-        beta_2: A float value or a constant float tensor. The exponential decay
-            rate for the exponentially weighted infinity norm.
-        epsilon: A small constant for numerical stability.
-            {{base_optimizer_keyword_args}}
+        beta_1: A float value or a constant float tensor, or a callable
+            that takes no arguments and returns the actual value to use. The
+            rate to combine the current gradient and the 1st moment estimate.
+            Defaults to `0.9`.
+        beta_2: A float value or a constant float tensor, or a callable
+            that takes no arguments and returns the actual value to use. The
+            exponential decay rate for the 1st moment estimate. Defaults to
+            `0.99`.
+        {{base_optimizer_keyword_args}}
+
+    References:
+
+    - [Chen et al., 2023](http://arxiv.org/abs/2302.06675)
+    - [Authors' implementation](
+        http://github.com/google/automl/tree/master/lion)
 
-    Reference:
-
-    - [Kingma et al., 2014](http://arxiv.org/abs/1412.6980)
     """
 
     def __init__(
         self,
         learning_rate=0.001,
         beta_1=0.9,
-        beta_2=0.999,
-        epsilon=1e-7,
+        beta_2=0.99,
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
         loss_scale_factor=None,
         gradient_accumulation_steps=None,
-        name="adamax",
+        name="lion",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
@@ -80,77 +70,73 @@
             ema_overwrite_frequency=ema_overwrite_frequency,
             loss_scale_factor=loss_scale_factor,
             gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
         self.beta_1 = beta_1
         self.beta_2 = beta_2
-        self.epsilon = epsilon
+        if beta_1 <= 0 or beta_1 > 1:
+            raise ValueError(
+                "Argument `beta_1` must be in the [0, 1] range. Otherwise, the "
+                f"optimizer degenerates to SignSGD. Received: beta_1={beta_1}."
+            )
 
     def build(self, var_list):
         """Initialize optimizer variables.
 
-        Adamax optimizer has 2 types of variables: momentums (denoted as m),
-        exponentially weighted infinity norm (denoted as u).
+        Lion optimizer has one variable `momentums`.
 
         Args:
-            var_list: list of model variables to build Adamax variables on.
+            var_list: list of model variables to build Lion variables on.
         """
         if self.built:
             return
         super().build(var_list)
-        self._m = []
-        self._u = []
+        self._momentums = []
         for var in var_list:
-            self._m.append(
+            self._momentums.append(
                 self.add_variable_from_reference(
                     reference_variable=var, name="momentum"
                 )
             )
-            self._u.append(
-                self.add_variable_from_reference(
-                    reference_variable=var, name="norm"
-                )
-            )
 
     def update_step(self, gradient, variable, learning_rate):
         """Update step given gradient and the associated model variable."""
         lr = ops.cast(learning_rate, variable.dtype)
         gradient = ops.cast(gradient, variable.dtype)
-        local_step = ops.cast(self.iterations + 1, variable.dtype)
-        beta_1_power = ops.power(
-            ops.cast(self.beta_1, variable.dtype), local_step
-        )
-
-        m = self._m[self._get_variable_index(variable)]
-        u = self._u[self._get_variable_index(variable)]
+        beta_1 = ops.cast(self.beta_1, variable.dtype)
+        beta_2 = ops.cast(self.beta_2, variable.dtype)
+        m = self._momentums[self._get_variable_index(variable)]
 
-        self.assign_add(
-            m, ops.multiply(ops.subtract(gradient, m), (1 - self.beta_1))
-        )
-        self.assign(
-            u, ops.maximum(ops.multiply(self.beta_2, u), ops.abs(gradient))
-        )
         self.assign_sub(
             variable,
-            ops.divide(
-                ops.multiply(lr, m),
-                ops.multiply((1 - beta_1_power), ops.add(u, self.epsilon)),
+            ops.multiply(
+                lr,
+                ops.sign(
+                    ops.add(
+                        ops.multiply(m, beta_1),
+                        ops.multiply(gradient, (1.0 - beta_1)),
+                    )
+                ),
+            ),
+        )
+        self.assign(
+            m,
+            ops.add(
+                ops.multiply(m, beta_2), ops.multiply(gradient, (1.0 - beta_2))
             ),
         )
 
     def get_config(self):
         config = super().get_config()
-
         config.update(
             {
                 "beta_1": self.beta_1,
                 "beta_2": self.beta_2,
-                "epsilon": self.epsilon,
             }
         )
         return config
 
 
-Adamax.__doc__ = Adamax.__doc__.replace(
+Lion.__doc__ = Lion.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/random/random.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/random/seed_generator.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/saving/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/saving/object_registration.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/saving/saving_api.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/testing/test_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/compile_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,18 +409,22 @@
     def __init__(
         self,
         loss,
         loss_weights=None,
         reduction="sum_over_batch_size",
         output_names=None,
     ):
-        if loss_weights and not isinstance(loss_weights, (list, tuple, dict)):
+        if loss_weights and not isinstance(
+            loss_weights, (list, tuple, dict, float)
+        ):
             raise ValueError(
-                "Expected `loss_weights` argument to be a list, tuple, or "
-                f"dict. Received instead: loss_weights={loss_weights} "
+                "Expected `loss_weights` argument to be a float "
+                "(single output case) or a list, tuple, or "
+                "dict (multiple output case). "
+                f"Received instead: loss_weights={loss_weights} "
                 f"of type {type(loss_weights)}"
             )
         self._user_loss = loss
         self._user_loss_weights = loss_weights
         self.built = False
         self.output_names = output_names
         super().__init__(name="compile_loss", reduction=reduction)
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/trainers/trainer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/tree/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/tree/tree_api.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/__init__.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/code_stats.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/file_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/image_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/io_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/module_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/naming.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/progbar.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/python_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras/src/utils/tracking.py` & `keras_nightly-3.3.2.dev2024042403/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024042203/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.2.dev2024042403/keras_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.0.dev2024042203
+Version: 3.3.2.dev2024042403
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: namex
 Requires-Dist: h5py
 Requires-Dist: optree
 Requires-Dist: ml-dtypes
```

### Comparing `keras_nightly-3.3.0.dev2024042203/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.2.dev2024042403/keras_nightly.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,75 @@
-LICENSE
 README.md
-pyproject.toml
-setup.cfg
 setup.py
-benchmarks/__init__.py
-benchmarks/layer_benchmark/__init__.py
-benchmarks/layer_benchmark/activation_benchmark.py
-benchmarks/layer_benchmark/attention_benchmark.py
-benchmarks/layer_benchmark/base_benchmark.py
-benchmarks/layer_benchmark/conv_benchmark.py
-benchmarks/layer_benchmark/core_benchmark.py
-benchmarks/layer_benchmark/merge_benchmark.py
-benchmarks/layer_benchmark/normalization_benchmark.py
-benchmarks/layer_benchmark/pooling_benchmark.py
-benchmarks/layer_benchmark/regularization_benchmark.py
-benchmarks/layer_benchmark/reshaping_benchmark.py
-benchmarks/layer_benchmark/rnn_benchmark.py
-benchmarks/model_benchmark/__init__.py
-benchmarks/model_benchmark/benchmark_utils.py
-benchmarks/model_benchmark/bert_benchmark.py
-benchmarks/model_benchmark/image_classification_benchmark.py
-benchmarks/torch_ctl_benchmark/__init__.py
-benchmarks/torch_ctl_benchmark/benchmark_utils.py
-benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
-benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
 keras/__init__.py
+keras/_tf_keras/__init__.py
+keras/_tf_keras/keras/__init__.py
+keras/_tf_keras/keras/activations/__init__.py
+keras/_tf_keras/keras/applications/__init__.py
+keras/_tf_keras/keras/applications/convnext/__init__.py
+keras/_tf_keras/keras/applications/densenet/__init__.py
+keras/_tf_keras/keras/applications/efficientnet/__init__.py
+keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+keras/_tf_keras/keras/applications/inception_v3/__init__.py
+keras/_tf_keras/keras/applications/mobilenet/__init__.py
+keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+keras/_tf_keras/keras/applications/nasnet/__init__.py
+keras/_tf_keras/keras/applications/resnet/__init__.py
+keras/_tf_keras/keras/applications/resnet50/__init__.py
+keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+keras/_tf_keras/keras/applications/vgg16/__init__.py
+keras/_tf_keras/keras/applications/vgg19/__init__.py
+keras/_tf_keras/keras/applications/xception/__init__.py
+keras/_tf_keras/keras/backend/__init__.py
+keras/_tf_keras/keras/callbacks/__init__.py
+keras/_tf_keras/keras/config/__init__.py
+keras/_tf_keras/keras/constraints/__init__.py
+keras/_tf_keras/keras/datasets/__init__.py
+keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+keras/_tf_keras/keras/datasets/california_housing/__init__.py
+keras/_tf_keras/keras/datasets/cifar10/__init__.py
+keras/_tf_keras/keras/datasets/cifar100/__init__.py
+keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+keras/_tf_keras/keras/datasets/imdb/__init__.py
+keras/_tf_keras/keras/datasets/mnist/__init__.py
+keras/_tf_keras/keras/datasets/reuters/__init__.py
+keras/_tf_keras/keras/distribution/__init__.py
+keras/_tf_keras/keras/dtype_policies/__init__.py
+keras/_tf_keras/keras/export/__init__.py
+keras/_tf_keras/keras/initializers/__init__.py
+keras/_tf_keras/keras/layers/__init__.py
+keras/_tf_keras/keras/legacy/__init__.py
+keras/_tf_keras/keras/legacy/saving/__init__.py
+keras/_tf_keras/keras/losses/__init__.py
+keras/_tf_keras/keras/metrics/__init__.py
+keras/_tf_keras/keras/mixed_precision/__init__.py
+keras/_tf_keras/keras/models/__init__.py
+keras/_tf_keras/keras/ops/__init__.py
+keras/_tf_keras/keras/ops/image/__init__.py
+keras/_tf_keras/keras/ops/linalg/__init__.py
+keras/_tf_keras/keras/ops/nn/__init__.py
+keras/_tf_keras/keras/ops/numpy/__init__.py
+keras/_tf_keras/keras/optimizers/__init__.py
+keras/_tf_keras/keras/optimizers/legacy/__init__.py
+keras/_tf_keras/keras/optimizers/schedules/__init__.py
+keras/_tf_keras/keras/preprocessing/__init__.py
+keras/_tf_keras/keras/preprocessing/image/__init__.py
+keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+keras/_tf_keras/keras/preprocessing/text/__init__.py
+keras/_tf_keras/keras/quantizers/__init__.py
+keras/_tf_keras/keras/random/__init__.py
+keras/_tf_keras/keras/regularizers/__init__.py
+keras/_tf_keras/keras/saving/__init__.py
+keras/_tf_keras/keras/tree/__init__.py
+keras/_tf_keras/keras/utils/__init__.py
+keras/_tf_keras/keras/utils/legacy/__init__.py
 keras/api/__init__.py
-keras/api/_tf_keras/__init__.py
-keras/api/_tf_keras/keras/__init__.py
-keras/api/_tf_keras/keras/activations/__init__.py
-keras/api/_tf_keras/keras/applications/__init__.py
-keras/api/_tf_keras/keras/applications/convnext/__init__.py
-keras/api/_tf_keras/keras/applications/densenet/__init__.py
-keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
-keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
-keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
-keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
-keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-keras/api/_tf_keras/keras/applications/nasnet/__init__.py
-keras/api/_tf_keras/keras/applications/resnet/__init__.py
-keras/api/_tf_keras/keras/applications/resnet50/__init__.py
-keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
-keras/api/_tf_keras/keras/applications/vgg16/__init__.py
-keras/api/_tf_keras/keras/applications/vgg19/__init__.py
-keras/api/_tf_keras/keras/applications/xception/__init__.py
-keras/api/_tf_keras/keras/backend/__init__.py
-keras/api/_tf_keras/keras/callbacks/__init__.py
-keras/api/_tf_keras/keras/config/__init__.py
-keras/api/_tf_keras/keras/constraints/__init__.py
-keras/api/_tf_keras/keras/datasets/__init__.py
-keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
-keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
-keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
-keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
-keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-keras/api/_tf_keras/keras/datasets/imdb/__init__.py
-keras/api/_tf_keras/keras/datasets/mnist/__init__.py
-keras/api/_tf_keras/keras/datasets/reuters/__init__.py
-keras/api/_tf_keras/keras/distribution/__init__.py
-keras/api/_tf_keras/keras/dtype_policies/__init__.py
-keras/api/_tf_keras/keras/export/__init__.py
-keras/api/_tf_keras/keras/initializers/__init__.py
-keras/api/_tf_keras/keras/layers/__init__.py
-keras/api/_tf_keras/keras/legacy/__init__.py
-keras/api/_tf_keras/keras/legacy/saving/__init__.py
-keras/api/_tf_keras/keras/losses/__init__.py
-keras/api/_tf_keras/keras/metrics/__init__.py
-keras/api/_tf_keras/keras/mixed_precision/__init__.py
-keras/api/_tf_keras/keras/models/__init__.py
-keras/api/_tf_keras/keras/ops/__init__.py
-keras/api/_tf_keras/keras/ops/image/__init__.py
-keras/api/_tf_keras/keras/ops/linalg/__init__.py
-keras/api/_tf_keras/keras/ops/nn/__init__.py
-keras/api/_tf_keras/keras/ops/numpy/__init__.py
-keras/api/_tf_keras/keras/optimizers/__init__.py
-keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
-keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
-keras/api/_tf_keras/keras/preprocessing/__init__.py
-keras/api/_tf_keras/keras/preprocessing/image/__init__.py
-keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
-keras/api/_tf_keras/keras/quantizers/__init__.py
-keras/api/_tf_keras/keras/random/__init__.py
-keras/api/_tf_keras/keras/regularizers/__init__.py
-keras/api/_tf_keras/keras/saving/__init__.py
-keras/api/_tf_keras/keras/tree/__init__.py
-keras/api/_tf_keras/keras/utils/__init__.py
-keras/api/_tf_keras/keras/utils/legacy/__init__.py
 keras/api/activations/__init__.py
 keras/api/applications/__init__.py
 keras/api/applications/convnext/__init__.py
 keras/api/applications/densenet/__init__.py
 keras/api/applications/efficientnet/__init__.py
 keras/api/applications/efficientnet_v2/__init__.py
 keras/api/applications/imagenet_utils/__init__.py
@@ -151,23 +128,20 @@
 keras/api/utils/__init__.py
 keras/api/utils/legacy/__init__.py
 keras/src/__init__.py
 keras/src/api_export.py
 keras/src/version.py
 keras/src/activations/__init__.py
 keras/src/activations/activations.py
-keras/src/activations/activations_test.py
 keras/src/applications/__init__.py
-keras/src/applications/applications_test.py
 keras/src/applications/convnext.py
 keras/src/applications/densenet.py
 keras/src/applications/efficientnet.py
 keras/src/applications/efficientnet_v2.py
 keras/src/applications/imagenet_utils.py
-keras/src/applications/imagenet_utils_test.py
 keras/src/applications/inception_resnet_v2.py
 keras/src/applications/inception_v3.py
 keras/src/applications/mobilenet.py
 keras/src/applications/mobilenet_v2.py
 keras/src/applications/mobilenet_v3.py
 keras/src/applications/nasnet.py
 keras/src/applications/resnet.py
@@ -176,32 +150,23 @@
 keras/src/applications/vgg19.py
 keras/src/applications/xception.py
 keras/src/backend/__init__.py
 keras/src/backend/config.py
 keras/src/backend/exports.py
 keras/src/backend/common/__init__.py
 keras/src/backend/common/backend_utils.py
-keras/src/backend/common/backend_utils_test.py
-keras/src/backend/common/compute_output_spec_test.py
 keras/src/backend/common/dtypes.py
-keras/src/backend/common/dtypes_test.py
 keras/src/backend/common/global_state.py
-keras/src/backend/common/global_state_test.py
 keras/src/backend/common/keras_tensor.py
-keras/src/backend/common/keras_tensor_test.py
 keras/src/backend/common/name_scope.py
-keras/src/backend/common/name_scope_test.py
 keras/src/backend/common/stateless_scope.py
-keras/src/backend/common/stateless_scope_test.py
 keras/src/backend/common/variables.py
-keras/src/backend/common/variables_test.py
 keras/src/backend/jax/__init__.py
 keras/src/backend/jax/core.py
 keras/src/backend/jax/distribution_lib.py
-keras/src/backend/jax/distribution_lib_test.py
 keras/src/backend/jax/image.py
 keras/src/backend/jax/layer.py
 keras/src/backend/jax/linalg.py
 keras/src/backend/jax/math.py
 keras/src/backend/jax/nn.py
 keras/src/backend/jax/numpy.py
 keras/src/backend/jax/optimizer.py
@@ -218,28 +183,24 @@
 keras/src/backend/numpy/nn.py
 keras/src/backend/numpy/numpy.py
 keras/src/backend/numpy/random.py
 keras/src/backend/numpy/rnn.py
 keras/src/backend/numpy/trainer.py
 keras/src/backend/tensorflow/__init__.py
 keras/src/backend/tensorflow/core.py
-keras/src/backend/tensorflow/distribute_test.py
 keras/src/backend/tensorflow/distribution_lib.py
 keras/src/backend/tensorflow/image.py
 keras/src/backend/tensorflow/layer.py
 keras/src/backend/tensorflow/linalg.py
 keras/src/backend/tensorflow/math.py
-keras/src/backend/tensorflow/name_scope_test.py
 keras/src/backend/tensorflow/nn.py
 keras/src/backend/tensorflow/numpy.py
 keras/src/backend/tensorflow/optimizer.py
-keras/src/backend/tensorflow/optimizer_distribute_test.py
 keras/src/backend/tensorflow/random.py
 keras/src/backend/tensorflow/rnn.py
-keras/src/backend/tensorflow/saved_model_test.py
 keras/src/backend/tensorflow/sparse.py
 keras/src/backend/tensorflow/tensorboard.py
 keras/src/backend/tensorflow/trackable.py
 keras/src/backend/tensorflow/trainer.py
 keras/src/backend/torch/__init__.py
 keras/src/backend/torch/core.py
 keras/src/backend/torch/image.py
@@ -261,481 +222,298 @@
 keras/src/backend/torch/optimizers/torch_nadam.py
 keras/src/backend/torch/optimizers/torch_optimizer.py
 keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
 keras/src/backend/torch/optimizers/torch_rmsprop.py
 keras/src/backend/torch/optimizers/torch_sgd.py
 keras/src/callbacks/__init__.py
 keras/src/callbacks/backup_and_restore.py
-keras/src/callbacks/backup_and_restore_test.py
 keras/src/callbacks/callback.py
 keras/src/callbacks/callback_list.py
-keras/src/callbacks/callback_test.py
 keras/src/callbacks/csv_logger.py
-keras/src/callbacks/csv_logger_test.py
 keras/src/callbacks/early_stopping.py
-keras/src/callbacks/early_stopping_test.py
 keras/src/callbacks/history.py
 keras/src/callbacks/lambda_callback.py
-keras/src/callbacks/lambda_callback_test.py
 keras/src/callbacks/learning_rate_scheduler.py
-keras/src/callbacks/learning_rate_scheduler_test.py
 keras/src/callbacks/model_checkpoint.py
-keras/src/callbacks/model_checkpoint_test.py
 keras/src/callbacks/progbar_logger.py
 keras/src/callbacks/reduce_lr_on_plateau.py
-keras/src/callbacks/reduce_lr_on_plateau_test.py
 keras/src/callbacks/remote_monitor.py
-keras/src/callbacks/remote_monitor_test.py
 keras/src/callbacks/swap_ema_weights.py
-keras/src/callbacks/swap_ema_weights_test.py
 keras/src/callbacks/tensorboard.py
-keras/src/callbacks/tensorboard_test.py
 keras/src/callbacks/terminate_on_nan.py
-keras/src/callbacks/terminate_on_nan_test.py
 keras/src/constraints/__init__.py
 keras/src/constraints/constraints.py
-keras/src/constraints/constraints_test.py
 keras/src/datasets/__init__.py
 keras/src/datasets/boston_housing.py
 keras/src/datasets/california_housing.py
 keras/src/datasets/cifar.py
 keras/src/datasets/cifar10.py
 keras/src/datasets/cifar100.py
 keras/src/datasets/fashion_mnist.py
 keras/src/datasets/imdb.py
 keras/src/datasets/mnist.py
 keras/src/datasets/reuters.py
 keras/src/distribution/__init__.py
 keras/src/distribution/distribution_lib.py
-keras/src/distribution/distribution_lib_test.py
 keras/src/dtype_policies/__init__.py
 keras/src/dtype_policies/dtype_policy.py
-keras/src/dtype_policies/dtype_policy_test.py
 keras/src/export/__init__.py
 keras/src/export/export_lib.py
-keras/src/export/export_lib_test.py
 keras/src/initializers/__init__.py
 keras/src/initializers/constant_initializers.py
-keras/src/initializers/constant_initializers_test.py
 keras/src/initializers/initializer.py
 keras/src/initializers/random_initializers.py
-keras/src/initializers/random_initializers_test.py
 keras/src/layers/__init__.py
 keras/src/layers/input_spec.py
 keras/src/layers/layer.py
-keras/src/layers/layer_test.py
 keras/src/layers/activations/__init__.py
 keras/src/layers/activations/activation.py
-keras/src/layers/activations/activation_test.py
 keras/src/layers/activations/elu.py
-keras/src/layers/activations/elu_test.py
 keras/src/layers/activations/leaky_relu.py
-keras/src/layers/activations/leaky_relu_test.py
 keras/src/layers/activations/prelu.py
-keras/src/layers/activations/prelu_test.py
 keras/src/layers/activations/relu.py
-keras/src/layers/activations/relu_test.py
 keras/src/layers/activations/softmax.py
-keras/src/layers/activations/softmax_test.py
 keras/src/layers/attention/__init__.py
 keras/src/layers/attention/additive_attention.py
-keras/src/layers/attention/additive_attention_test.py
 keras/src/layers/attention/attention.py
-keras/src/layers/attention/attention_test.py
 keras/src/layers/attention/grouped_query_attention.py
-keras/src/layers/attention/grouped_query_attention_test.py
 keras/src/layers/attention/multi_head_attention.py
-keras/src/layers/attention/multi_head_attention_test.py
 keras/src/layers/convolutional/__init__.py
 keras/src/layers/convolutional/base_conv.py
 keras/src/layers/convolutional/base_conv_transpose.py
 keras/src/layers/convolutional/base_depthwise_conv.py
 keras/src/layers/convolutional/base_separable_conv.py
 keras/src/layers/convolutional/conv1d.py
 keras/src/layers/convolutional/conv1d_transpose.py
 keras/src/layers/convolutional/conv2d.py
 keras/src/layers/convolutional/conv2d_transpose.py
 keras/src/layers/convolutional/conv3d.py
 keras/src/layers/convolutional/conv3d_transpose.py
-keras/src/layers/convolutional/conv_test.py
-keras/src/layers/convolutional/conv_transpose_test.py
 keras/src/layers/convolutional/depthwise_conv1d.py
 keras/src/layers/convolutional/depthwise_conv2d.py
-keras/src/layers/convolutional/depthwise_conv_test.py
 keras/src/layers/convolutional/separable_conv1d.py
 keras/src/layers/convolutional/separable_conv2d.py
-keras/src/layers/convolutional/separable_conv_test.py
 keras/src/layers/core/__init__.py
 keras/src/layers/core/dense.py
-keras/src/layers/core/dense_test.py
 keras/src/layers/core/einsum_dense.py
-keras/src/layers/core/einsum_dense_test.py
 keras/src/layers/core/embedding.py
-keras/src/layers/core/embedding_test.py
 keras/src/layers/core/identity.py
-keras/src/layers/core/identity_test.py
 keras/src/layers/core/input_layer.py
-keras/src/layers/core/input_layer_test.py
 keras/src/layers/core/lambda_layer.py
-keras/src/layers/core/lambda_layer_test.py
 keras/src/layers/core/masking.py
-keras/src/layers/core/masking_test.py
 keras/src/layers/core/wrapper.py
-keras/src/layers/core/wrapper_test.py
 keras/src/layers/merging/__init__.py
 keras/src/layers/merging/add.py
 keras/src/layers/merging/average.py
 keras/src/layers/merging/base_merge.py
 keras/src/layers/merging/concatenate.py
 keras/src/layers/merging/dot.py
 keras/src/layers/merging/maximum.py
-keras/src/layers/merging/merging_test.py
 keras/src/layers/merging/minimum.py
 keras/src/layers/merging/multiply.py
 keras/src/layers/merging/subtract.py
 keras/src/layers/normalization/__init__.py
 keras/src/layers/normalization/batch_normalization.py
-keras/src/layers/normalization/batch_normalization_test.py
 keras/src/layers/normalization/group_normalization.py
-keras/src/layers/normalization/group_normalization_test.py
 keras/src/layers/normalization/layer_normalization.py
-keras/src/layers/normalization/layer_normalization_test.py
 keras/src/layers/normalization/spectral_normalization.py
-keras/src/layers/normalization/spectral_normalization_test.py
 keras/src/layers/normalization/unit_normalization.py
-keras/src/layers/normalization/unit_normalization_test.py
 keras/src/layers/pooling/__init__.py
 keras/src/layers/pooling/average_pooling1d.py
 keras/src/layers/pooling/average_pooling2d.py
 keras/src/layers/pooling/average_pooling3d.py
-keras/src/layers/pooling/average_pooling_test.py
 keras/src/layers/pooling/base_global_pooling.py
 keras/src/layers/pooling/base_pooling.py
 keras/src/layers/pooling/global_average_pooling1d.py
 keras/src/layers/pooling/global_average_pooling2d.py
 keras/src/layers/pooling/global_average_pooling3d.py
-keras/src/layers/pooling/global_average_pooling_test.py
 keras/src/layers/pooling/global_max_pooling1d.py
 keras/src/layers/pooling/global_max_pooling2d.py
 keras/src/layers/pooling/global_max_pooling3d.py
-keras/src/layers/pooling/global_max_pooling_test.py
 keras/src/layers/pooling/max_pooling1d.py
 keras/src/layers/pooling/max_pooling2d.py
 keras/src/layers/pooling/max_pooling3d.py
-keras/src/layers/pooling/max_pooling_test.py
 keras/src/layers/preprocessing/__init__.py
 keras/src/layers/preprocessing/audio_preprocessing.py
-keras/src/layers/preprocessing/audio_preprocessing_test.py
 keras/src/layers/preprocessing/category_encoding.py
-keras/src/layers/preprocessing/category_encoding_test.py
 keras/src/layers/preprocessing/center_crop.py
-keras/src/layers/preprocessing/center_crop_test.py
 keras/src/layers/preprocessing/discretization.py
-keras/src/layers/preprocessing/discretization_test.py
 keras/src/layers/preprocessing/feature_space.py
-keras/src/layers/preprocessing/feature_space_test.py
 keras/src/layers/preprocessing/hashed_crossing.py
-keras/src/layers/preprocessing/hashed_crossing_test.py
 keras/src/layers/preprocessing/hashing.py
-keras/src/layers/preprocessing/hashing_test.py
 keras/src/layers/preprocessing/index_lookup.py
-keras/src/layers/preprocessing/index_lookup_test.py
 keras/src/layers/preprocessing/integer_lookup.py
-keras/src/layers/preprocessing/integer_lookup_test.py
 keras/src/layers/preprocessing/normalization.py
-keras/src/layers/preprocessing/normalization_test.py
 keras/src/layers/preprocessing/random_brightness.py
-keras/src/layers/preprocessing/random_brightness_test.py
 keras/src/layers/preprocessing/random_contrast.py
-keras/src/layers/preprocessing/random_contrast_test.py
 keras/src/layers/preprocessing/random_crop.py
-keras/src/layers/preprocessing/random_crop_test.py
 keras/src/layers/preprocessing/random_flip.py
-keras/src/layers/preprocessing/random_flip_test.py
 keras/src/layers/preprocessing/random_rotation.py
-keras/src/layers/preprocessing/random_rotation_test.py
 keras/src/layers/preprocessing/random_translation.py
-keras/src/layers/preprocessing/random_translation_test.py
 keras/src/layers/preprocessing/random_zoom.py
-keras/src/layers/preprocessing/random_zoom_test.py
 keras/src/layers/preprocessing/rescaling.py
-keras/src/layers/preprocessing/rescaling_test.py
 keras/src/layers/preprocessing/resizing.py
-keras/src/layers/preprocessing/resizing_test.py
 keras/src/layers/preprocessing/string_lookup.py
-keras/src/layers/preprocessing/string_lookup_test.py
 keras/src/layers/preprocessing/text_vectorization.py
-keras/src/layers/preprocessing/text_vectorization_test.py
 keras/src/layers/preprocessing/tf_data_layer.py
 keras/src/layers/regularization/__init__.py
 keras/src/layers/regularization/activity_regularization.py
-keras/src/layers/regularization/activity_regularization_test.py
 keras/src/layers/regularization/alpha_dropout.py
-keras/src/layers/regularization/alpha_dropout_test.py
 keras/src/layers/regularization/dropout.py
-keras/src/layers/regularization/dropout_test.py
 keras/src/layers/regularization/gaussian_dropout.py
-keras/src/layers/regularization/gaussian_dropout_test.py
 keras/src/layers/regularization/gaussian_noise.py
-keras/src/layers/regularization/gaussian_noise_test.py
 keras/src/layers/regularization/spatial_dropout.py
-keras/src/layers/regularization/spatial_dropout_test.py
 keras/src/layers/reshaping/__init__.py
 keras/src/layers/reshaping/cropping1d.py
-keras/src/layers/reshaping/cropping1d_test.py
 keras/src/layers/reshaping/cropping2d.py
-keras/src/layers/reshaping/cropping2d_test.py
 keras/src/layers/reshaping/cropping3d.py
-keras/src/layers/reshaping/cropping3d_test.py
 keras/src/layers/reshaping/flatten.py
-keras/src/layers/reshaping/flatten_test.py
 keras/src/layers/reshaping/permute.py
-keras/src/layers/reshaping/permute_test.py
 keras/src/layers/reshaping/repeat_vector.py
-keras/src/layers/reshaping/repeat_vector_test.py
 keras/src/layers/reshaping/reshape.py
-keras/src/layers/reshaping/reshape_test.py
 keras/src/layers/reshaping/up_sampling1d.py
-keras/src/layers/reshaping/up_sampling1d_test.py
 keras/src/layers/reshaping/up_sampling2d.py
-keras/src/layers/reshaping/up_sampling2d_test.py
 keras/src/layers/reshaping/up_sampling3d.py
-keras/src/layers/reshaping/up_sampling3d_test.py
 keras/src/layers/reshaping/zero_padding1d.py
-keras/src/layers/reshaping/zero_padding1d_test.py
 keras/src/layers/reshaping/zero_padding2d.py
-keras/src/layers/reshaping/zero_padding2d_test.py
 keras/src/layers/reshaping/zero_padding3d.py
-keras/src/layers/reshaping/zero_padding3d_test.py
 keras/src/layers/rnn/__init__.py
 keras/src/layers/rnn/bidirectional.py
-keras/src/layers/rnn/bidirectional_test.py
 keras/src/layers/rnn/conv_lstm.py
 keras/src/layers/rnn/conv_lstm1d.py
-keras/src/layers/rnn/conv_lstm1d_test.py
 keras/src/layers/rnn/conv_lstm2d.py
-keras/src/layers/rnn/conv_lstm2d_test.py
 keras/src/layers/rnn/conv_lstm3d.py
-keras/src/layers/rnn/conv_lstm3d_test.py
-keras/src/layers/rnn/conv_lstm_test.py
 keras/src/layers/rnn/dropout_rnn_cell.py
-keras/src/layers/rnn/dropout_rnn_cell_test.py
 keras/src/layers/rnn/gru.py
-keras/src/layers/rnn/gru_test.py
 keras/src/layers/rnn/lstm.py
-keras/src/layers/rnn/lstm_test.py
 keras/src/layers/rnn/rnn.py
-keras/src/layers/rnn/rnn_test.py
 keras/src/layers/rnn/simple_rnn.py
-keras/src/layers/rnn/simple_rnn_test.py
 keras/src/layers/rnn/stacked_rnn_cells.py
-keras/src/layers/rnn/stacked_rnn_cells_test.py
 keras/src/layers/rnn/time_distributed.py
-keras/src/layers/rnn/time_distributed_test.py
 keras/src/legacy/__init__.py
 keras/src/legacy/backend.py
 keras/src/legacy/layers.py
 keras/src/legacy/losses.py
 keras/src/legacy/preprocessing/__init__.py
 keras/src/legacy/preprocessing/image.py
 keras/src/legacy/preprocessing/sequence.py
 keras/src/legacy/preprocessing/text.py
 keras/src/legacy/saving/__init__.py
 keras/src/legacy/saving/json_utils.py
-keras/src/legacy/saving/json_utils_test.py
 keras/src/legacy/saving/legacy_h5_format.py
-keras/src/legacy/saving/legacy_h5_format_test.py
 keras/src/legacy/saving/saving_options.py
 keras/src/legacy/saving/saving_utils.py
 keras/src/legacy/saving/serialization.py
 keras/src/losses/__init__.py
 keras/src/losses/loss.py
-keras/src/losses/loss_test.py
 keras/src/losses/losses.py
-keras/src/losses/losses_test.py
 keras/src/metrics/__init__.py
 keras/src/metrics/accuracy_metrics.py
-keras/src/metrics/accuracy_metrics_test.py
 keras/src/metrics/confusion_metrics.py
-keras/src/metrics/confusion_metrics_test.py
 keras/src/metrics/f_score_metrics.py
-keras/src/metrics/f_score_metrics_test.py
 keras/src/metrics/hinge_metrics.py
-keras/src/metrics/hinge_metrics_test.py
 keras/src/metrics/iou_metrics.py
-keras/src/metrics/iou_metrics_test.py
 keras/src/metrics/metric.py
-keras/src/metrics/metric_test.py
 keras/src/metrics/metrics_utils.py
 keras/src/metrics/probabilistic_metrics.py
-keras/src/metrics/probabilistic_metrics_test.py
 keras/src/metrics/reduction_metrics.py
-keras/src/metrics/reduction_metrics_test.py
 keras/src/metrics/regression_metrics.py
-keras/src/metrics/regression_metrics_test.py
 keras/src/models/__init__.py
 keras/src/models/cloning.py
-keras/src/models/cloning_test.py
 keras/src/models/functional.py
-keras/src/models/functional_test.py
 keras/src/models/model.py
-keras/src/models/model_test.py
 keras/src/models/sequential.py
-keras/src/models/sequential_test.py
 keras/src/models/variable_mapping.py
-keras/src/models/variable_mapping_test.py
 keras/src/ops/__init__.py
 keras/src/ops/core.py
-keras/src/ops/core_test.py
 keras/src/ops/function.py
-keras/src/ops/function_test.py
 keras/src/ops/image.py
-keras/src/ops/image_test.py
 keras/src/ops/linalg.py
-keras/src/ops/linalg_test.py
 keras/src/ops/math.py
-keras/src/ops/math_test.py
 keras/src/ops/nn.py
-keras/src/ops/nn_test.py
 keras/src/ops/node.py
-keras/src/ops/node_test.py
 keras/src/ops/numpy.py
-keras/src/ops/numpy_test.py
 keras/src/ops/operation.py
-keras/src/ops/operation_test.py
 keras/src/ops/operation_utils.py
-keras/src/ops/operation_utils_test.py
 keras/src/ops/symbolic_arguments.py
-keras/src/ops/symbolic_arguments_test.py
 keras/src/optimizers/__init__.py
 keras/src/optimizers/adadelta.py
-keras/src/optimizers/adadelta_test.py
 keras/src/optimizers/adafactor.py
-keras/src/optimizers/adafactor_test.py
 keras/src/optimizers/adagrad.py
-keras/src/optimizers/adagrad_test.py
 keras/src/optimizers/adam.py
-keras/src/optimizers/adam_test.py
 keras/src/optimizers/adamax.py
-keras/src/optimizers/adamax_test.py
 keras/src/optimizers/adamw.py
-keras/src/optimizers/adamw_test.py
 keras/src/optimizers/base_optimizer.py
 keras/src/optimizers/ftrl.py
-keras/src/optimizers/ftrl_test.py
 keras/src/optimizers/lion.py
-keras/src/optimizers/lion_test.py
 keras/src/optimizers/loss_scale_optimizer.py
-keras/src/optimizers/loss_scale_optimizer_test.py
 keras/src/optimizers/nadam.py
-keras/src/optimizers/nadam_test.py
 keras/src/optimizers/optimizer.py
-keras/src/optimizers/optimizer_sparse_test.py
-keras/src/optimizers/optimizer_test.py
 keras/src/optimizers/rmsprop.py
-keras/src/optimizers/rmsprop_test.py
 keras/src/optimizers/sgd.py
-keras/src/optimizers/sgd_test.py
 keras/src/optimizers/schedules/__init__.py
 keras/src/optimizers/schedules/learning_rate_schedule.py
-keras/src/optimizers/schedules/learning_rate_schedule_test.py
 keras/src/quantizers/__init__.py
 keras/src/quantizers/quantizers.py
-keras/src/quantizers/quantizers_test.py
 keras/src/random/__init__.py
 keras/src/random/random.py
-keras/src/random/random_test.py
 keras/src/random/seed_generator.py
-keras/src/random/seed_generator_test.py
 keras/src/regularizers/__init__.py
 keras/src/regularizers/regularizers.py
-keras/src/regularizers/regularizers_test.py
 keras/src/saving/__init__.py
 keras/src/saving/object_registration.py
-keras/src/saving/object_registration_test.py
 keras/src/saving/saving_api.py
-keras/src/saving/saving_api_test.py
 keras/src/saving/saving_lib.py
-keras/src/saving/saving_lib_test.py
 keras/src/saving/serialization_lib.py
-keras/src/saving/serialization_lib_test.py
 keras/src/testing/__init__.py
 keras/src/testing/test_case.py
 keras/src/testing/test_utils.py
-keras/src/testing/test_utils_test.py
 keras/src/trainers/__init__.py
 keras/src/trainers/compile_utils.py
-keras/src/trainers/compile_utils_test.py
 keras/src/trainers/epoch_iterator.py
-keras/src/trainers/epoch_iterator_test.py
 keras/src/trainers/trainer.py
-keras/src/trainers/trainer_test.py
 keras/src/trainers/data_adapters/__init__.py
 keras/src/trainers/data_adapters/array_data_adapter.py
-keras/src/trainers/data_adapters/array_data_adapter_test.py
 keras/src/trainers/data_adapters/array_slicing.py
 keras/src/trainers/data_adapters/data_adapter.py
 keras/src/trainers/data_adapters/data_adapter_utils.py
 keras/src/trainers/data_adapters/generator_data_adapter.py
-keras/src/trainers/data_adapters/generator_data_adapter_test.py
 keras/src/trainers/data_adapters/py_dataset_adapter.py
-keras/src/trainers/data_adapters/py_dataset_adapter_test.py
 keras/src/trainers/data_adapters/tf_dataset_adapter.py
-keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
 keras/src/trainers/data_adapters/torch_data_loader_adapter.py
-keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
 keras/src/tree/__init__.py
 keras/src/tree/dmtree_impl.py
 keras/src/tree/optree_impl.py
 keras/src/tree/tree_api.py
-keras/src/tree/tree_test.py
 keras/src/utils/__init__.py
 keras/src/utils/argument_validation.py
 keras/src/utils/audio_dataset_utils.py
-keras/src/utils/audio_dataset_utils_test.py
 keras/src/utils/backend_utils.py
 keras/src/utils/code_stats.py
-keras/src/utils/code_stats_test.py
 keras/src/utils/dataset_utils.py
-keras/src/utils/dataset_utils_test.py
 keras/src/utils/dtype_utils.py
-keras/src/utils/dtype_utils_test.py
 keras/src/utils/file_utils.py
-keras/src/utils/file_utils_test.py
 keras/src/utils/image_dataset_utils.py
-keras/src/utils/image_dataset_utils_test.py
 keras/src/utils/image_utils.py
 keras/src/utils/io_utils.py
-keras/src/utils/io_utils_test.py
 keras/src/utils/jax_layer.py
-keras/src/utils/jax_layer_test.py
 keras/src/utils/jax_utils.py
 keras/src/utils/model_visualization.py
 keras/src/utils/module_utils.py
 keras/src/utils/naming.py
-keras/src/utils/naming_test.py
 keras/src/utils/numerical_utils.py
-keras/src/utils/numerical_utils_test.py
 keras/src/utils/progbar.py
 keras/src/utils/python_utils.py
-keras/src/utils/python_utils_test.py
 keras/src/utils/rng_utils.py
-keras/src/utils/rng_utils_test.py
 keras/src/utils/sequence_utils.py
-keras/src/utils/sequence_utils_test.py
 keras/src/utils/summary_utils.py
-keras/src/utils/summary_utils_test.py
 keras/src/utils/text_dataset_utils.py
-keras/src/utils/text_dataset_utils_test.py
 keras/src/utils/tf_utils.py
 keras/src/utils/timeseries_dataset_utils.py
-keras/src/utils/timeseries_dataset_utils_test.py
 keras/src/utils/torch_utils.py
-keras/src/utils/torch_utils_test.py
 keras/src/utils/traceback_utils.py
 keras/src/utils/tracking.py
-keras/src/utils/tracking_test.py
 keras_nightly.egg-info/PKG-INFO
 keras_nightly.egg-info/SOURCES.txt
 keras_nightly.egg-info/dependency_links.txt
 keras_nightly.egg-info/requires.txt
 keras_nightly.egg-info/top_level.txt
```

### Comparing `keras_nightly-3.3.0.dev2024042203/setup.py` & `keras_nightly-3.3.2.dev2024042403/setup.py`

 * *Files identical despite different names*

