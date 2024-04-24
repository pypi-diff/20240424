# Comparing `tmp/kappamodules-0.1.7.tar.gz` & `tmp/kappamodules-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappamodules-0.1.7.tar", last modified: Sat Dec 30 21:44:19 2023, max compression
+gzip compressed data, was "kappamodules-0.1.8.tar", last modified: Sun Dec 31 01:31:06 2023, max compression
```

## Comparing `kappamodules-0.1.7.tar` & `kappamodules-0.1.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.713291 kappamodules-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-30 21:42:44.000000 kappamodules-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-12-30 21:44:19.713291 kappamodules-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-30 21:42:44.000000 kappamodules-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.701291 kappamodules-0.1.7/kappamodules/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-30 21:44:06.000000 kappamodules-0.1.7/kappamodules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.705291 kappamodules-0.1.7/kappamodules/attention/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/attention/dot_product_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/attention/dot_product_attention_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/attention/linear_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/attention/perceiver_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.705291 kappamodules-0.1.7/kappamodules/diffaug/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/diffaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/diffaug/gaussian_blur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.705291 kappamodules-0.1.7/kappamodules/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/functional/patchify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/functional/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.705291 kappamodules-0.1.7/kappamodules/init/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/init/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.705291 kappamodules-0.1.7/kappamodules/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/continuous_sincos_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/paramless_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/regular_grid_sincos_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/residual.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/rms_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/layers/weight_norm_linear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.709291 kappamodules-0.1.7/kappamodules/losses/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/losses/l1_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/losses/mse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.709291 kappamodules-0.1.7/kappamodules/modulation/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/modulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/modulation/dit.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/modulation/film.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/modulation/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/modulation/timestep_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.709291 kappamodules-0.1.7/kappamodules/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/ssl/contrastive_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/ssl/contrastive_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/ssl/dino_projector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.709291 kappamodules-0.1.7/kappamodules/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/transformer/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/transformer/perceiver_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/transformer/postnorm_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.709291 kappamodules-0.1.7/kappamodules/unet/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/unet/unet_denoising_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.709291 kappamodules-0.1.7/kappamodules/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/utils/mode_to_ctor.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/utils/param_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/utils/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/utils/tensor_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.713291 kappamodules-0.1.7/kappamodules/vit/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/dit_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/vit_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/vit_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/vit_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/vit_class_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/vit_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/vit_patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/vit_pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-12-30 21:42:44.000000 kappamodules-0.1.7/kappamodules/vit/vit_seperate_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-30 21:44:19.713291 kappamodules-0.1.7/kappamodules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-12-30 21:44:19.000000 kappamodules-0.1.7/kappamodules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-12-30 21:44:19.000000 kappamodules-0.1.7/kappamodules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-30 21:44:19.000000 kappamodules-0.1.7/kappamodules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-30 21:44:19.000000 kappamodules-0.1.7/kappamodules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-30 21:44:19.000000 kappamodules-0.1.7/kappamodules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-30 21:42:44.000000 kappamodules-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-30 21:44:19.713291 kappamodules-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.301346 kappamodules-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-31 01:29:27.000000 kappamodules-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2023-12-31 01:31:06.301346 kappamodules-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-31 01:29:27.000000 kappamodules-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.289346 kappamodules-0.1.8/kappamodules/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-31 01:30:52.000000 kappamodules-0.1.8/kappamodules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.289346 kappamodules-0.1.8/kappamodules/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/attention/dot_product_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/attention/dot_product_attention_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/attention/linear_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/attention/perceiver_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.289346 kappamodules-0.1.8/kappamodules/diffaug/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/diffaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/diffaug/gaussian_blur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.293346 kappamodules-0.1.8/kappamodules/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/functional/patchify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/functional/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.293346 kappamodules-0.1.8/kappamodules/init/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/init/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.293346 kappamodules-0.1.8/kappamodules/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/continuous_sincos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/paramless_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/regular_grid_sincos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/rms_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/layers/weight_norm_linear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.293346 kappamodules-0.1.8/kappamodules/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/losses/l1_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/losses/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.293346 kappamodules-0.1.8/kappamodules/modulation/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/modulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/modulation/dit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/modulation/film.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/modulation/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/modulation/timestep_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.297346 kappamodules-0.1.8/kappamodules/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/ssl/contrastive_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/ssl/contrastive_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/ssl/dino_projector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.297346 kappamodules-0.1.8/kappamodules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/transformer/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/transformer/perceiver_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/transformer/postnorm_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.297346 kappamodules-0.1.8/kappamodules/unet/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/unet/unet_denoising_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.297346 kappamodules-0.1.8/kappamodules/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/utils/mode_to_ctor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/utils/param_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/utils/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/utils/tensor_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.301346 kappamodules-0.1.8/kappamodules/vit/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/dit_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/vit_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/vit_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/vit_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/vit_class_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/vit_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/vit_patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/vit_pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-12-31 01:29:27.000000 kappamodules-0.1.8/kappamodules/vit/vit_seperate_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 01:31:06.301346 kappamodules-0.1.8/kappamodules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2023-12-31 01:31:06.000000 kappamodules-0.1.8/kappamodules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-12-31 01:31:06.000000 kappamodules-0.1.8/kappamodules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 01:31:06.000000 kappamodules-0.1.8/kappamodules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-31 01:31:06.000000 kappamodules-0.1.8/kappamodules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-31 01:31:06.000000 kappamodules-0.1.8/kappamodules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-31 01:29:27.000000 kappamodules-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2023-12-31 01:31:06.301346 kappamodules-0.1.8/setup.cfg
```

### Comparing `kappamodules-0.1.7/LICENSE` & `kappamodules-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/PKG-INFO` & `kappamodules-0.1.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappamodules
-Version: 0.1.7
+Version: 0.1.8
 Summary: efficient building blocks for pytorch models
 Home-page: https://github.com/BenediktAlkin/KappaModules
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaModules
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaModules/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappamodules-0.1.7/kappamodules/attention/dot_product_attention.py` & `kappamodules-0.1.8/kappamodules/attention/dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/attention/dot_product_attention_slow.py` & `kappamodules-0.1.8/kappamodules/attention/dot_product_attention_slow.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/attention/linear_attention.py` & `kappamodules-0.1.8/kappamodules/attention/linear_attention.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/attention/perceiver_attention.py` & `kappamodules-0.1.8/kappamodules/attention/perceiver_attention.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/diffaug/gaussian_blur.py` & `kappamodules-0.1.8/kappamodules/diffaug/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/functional/patchify.py` & `kappamodules-0.1.8/kappamodules/functional/patchify.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/functional/pos_embed.py` & `kappamodules-0.1.8/kappamodules/functional/pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/init/functional.py` & `kappamodules-0.1.8/kappamodules/init/functional.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/layers/continuous_sincos_embed.py` & `kappamodules-0.1.8/kappamodules/layers/continuous_sincos_embed.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,17 @@
         self.dim = dim
         self.ndim = ndim
         # if dim is not cleanly divisible -> cut away trailing dimensions
         self.ndim_padding = dim % ndim
         dim_per_ndim = (dim - self.ndim_padding) // ndim
         self.sincos_padding = dim_per_ndim % 2
         self.max_wavelength = max_wavelength
-        self.padding = self.ndim_padding + self.sincos_padding * 2
+        self.padding = self.ndim_padding + self.sincos_padding * ndim
         effective_dim_per_wave = (self.dim - self.padding) // ndim
+        assert effective_dim_per_wave > 0
         self.register_buffer(
             "omega",
             1. / max_wavelength ** (torch.arange(0, effective_dim_per_wave, 2, dtype=dtype) / effective_dim_per_wave),
         )
 
     def forward(self, coords):
         out_dtype = coords.dtype
@@ -33,7 +34,13 @@
         else:
             raise NotImplementedError
         emb = emb.to(out_dtype)
         if self.padding > 0:
             padding = torch.zeros(*emb.shape[:-1], self.padding, device=emb.device, dtype=emb.dtype)
             emb = torch.concat([emb, padding], dim=-1)
         return emb
+
+    def __str__(self):
+        return repr(self)
+
+    def __repr__(self):
+        return f"{type(self).__name__}(dim={self.dim})"
```

### Comparing `kappamodules-0.1.7/kappamodules/layers/drop_path.py` & `kappamodules-0.1.8/kappamodules/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/layers/identity.py` & `kappamodules-0.1.8/kappamodules/layers/identity.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/layers/paramless_batchnorm.py` & `kappamodules-0.1.8/kappamodules/layers/paramless_batchnorm.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/layers/regular_grid_sincos_embed.py` & `kappamodules-0.1.8/kappamodules/layers/regular_grid_sincos_embed.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/layers/residual.py` & `kappamodules-0.1.8/kappamodules/layers/residual.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/layers/weight_norm_linear.py` & `kappamodules-0.1.8/kappamodules/layers/weight_norm_linear.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/modulation/dit.py` & `kappamodules-0.1.8/kappamodules/modulation/dit.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/modulation/film.py` & `kappamodules-0.1.8/kappamodules/modulation/film.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/modulation/timestep_embed.py` & `kappamodules-0.1.8/kappamodules/modulation/timestep_embed.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/ssl/contrastive_predictor.py` & `kappamodules-0.1.8/kappamodules/ssl/contrastive_predictor.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/ssl/contrastive_projector.py` & `kappamodules-0.1.8/kappamodules/ssl/contrastive_projector.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/ssl/dino_projector.py` & `kappamodules-0.1.8/kappamodules/ssl/dino_projector.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/transformer/mlp.py` & `kappamodules-0.1.8/kappamodules/transformer/mlp.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/transformer/perceiver_block.py` & `kappamodules-0.1.8/kappamodules/transformer/perceiver_block.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/transformer/postnorm_block.py` & `kappamodules-0.1.8/kappamodules/transformer/postnorm_block.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/unet/unet_denoising_diffusion.py` & `kappamodules-0.1.8/kappamodules/unet/unet_denoising_diffusion.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/utils/mode_to_ctor.py` & `kappamodules-0.1.8/kappamodules/utils/mode_to_ctor.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/utils/param_checking.py` & `kappamodules-0.1.8/kappamodules/utils/param_checking.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/utils/tensor_cache.py` & `kappamodules-0.1.8/kappamodules/utils/tensor_cache.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/dit_block.py` & `kappamodules-0.1.8/kappamodules/vit/dit_block.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/vit_batchnorm.py` & `kappamodules-0.1.8/kappamodules/vit/vit_batchnorm.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/vit_block.py` & `kappamodules-0.1.8/kappamodules/vit/vit_block.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/vit_blocks.py` & `kappamodules-0.1.8/kappamodules/vit/vit_blocks.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/vit_class_tokens.py` & `kappamodules-0.1.8/kappamodules/vit/vit_class_tokens.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/vit_mlp.py` & `kappamodules-0.1.8/kappamodules/vit/vit_mlp.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/vit_patch_embed.py` & `kappamodules-0.1.8/kappamodules/vit/vit_patch_embed.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/vit_pos_embed.py` & `kappamodules-0.1.8/kappamodules/vit/vit_pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules/vit/vit_seperate_norm.py` & `kappamodules-0.1.8/kappamodules/vit/vit_seperate_norm.py`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/kappamodules.egg-info/PKG-INFO` & `kappamodules-0.1.8/kappamodules.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappamodules
-Version: 0.1.7
+Version: 0.1.8
 Summary: efficient building blocks for pytorch models
 Home-page: https://github.com/BenediktAlkin/KappaModules
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaModules
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaModules/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kappamodules-0.1.7/kappamodules.egg-info/SOURCES.txt` & `kappamodules-0.1.8/kappamodules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kappamodules-0.1.7/setup.cfg` & `kappamodules-0.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.1.7
+version = 0.1.8
 name = kappamodules
 description = efficient building blocks for pytorch models
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaModules
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaModules
```

