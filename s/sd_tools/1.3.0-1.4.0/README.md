# Comparing `tmp/sd_tools-1.3.0.tar.gz` & `tmp/sd_tools-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_tools-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sd_tools-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sd_tools-1.3.0.tar` & `sd_tools-1.4.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
--rw-r--r--   0        0        0       62 2024-03-20 12:27:39.732811 sd_tools-1.3.0/.gitignore
--rw-r--r--   0        0        0     1066 2024-03-13 13:59:00.328247 sd_tools-1.3.0/LICENSE
--rw-r--r--   0        0        0     7742 2024-03-27 12:12:35.675073 sd_tools-1.3.0/README.md
--rw-r--r--   0        0        0     1067 2024-03-27 12:15:38.191299 sd_tools-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       66 2024-03-13 13:59:00.331410 sd_tools-1.3.0/pyrightconfig.json
--rw-r--r--   0        0        0        0 2024-03-14 11:59:50.653597 sd_tools-1.3.0/src/sd_tools/__init__.py
--rw-r--r--   0        0        0     1224 2024-03-27 02:09:58.110511 sd_tools-1.3.0/src/sd_tools/misc.py
--rw-r--r--   0        0        0     2003 2024-03-27 12:14:11.338055 sd_tools-1.3.0/src/sd_tools/plugins/base.py
--rw-r--r--   0        0        0     1855 2024-03-20 02:37:31.819560 sd_tools-1.3.0/src/sd_tools/plugins/canny.py
--rw-r--r--   0        0        0      401 2024-03-14 06:20:33.776026 sd_tools-1.3.0/src/sd_tools/plugins/cfg.py
--rw-r--r--   0        0        0      244 2024-03-14 06:40:40.391656 sd_tools-1.3.0/src/sd_tools/plugins/debug.py
--rw-r--r--   0        0        0     1319 2024-03-14 06:40:40.352819 sd_tools-1.3.0/src/sd_tools/plugins/depth.py
--rw-r--r--   0        0        0      459 2024-03-14 06:40:40.395319 sd_tools-1.3.0/src/sd_tools/plugins/device.py
--rw-r--r--   0        0        0      460 2024-03-24 04:09:01.813371 sd_tools-1.3.0/src/sd_tools/plugins/dpo.py
--rw-r--r--   0        0        0     1755 2024-03-22 08:49:17.470727 sd_tools-1.3.0/src/sd_tools/plugins/http/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 06:14:55.106370 sd_tools-1.3.0/src/sd_tools/plugins/http/assets/dom.js
--rw-r--r--   0        0        0      344 2024-03-27 02:35:53.522855 sd_tools-1.3.0/src/sd_tools/plugins/http/assets/index.css
--rw-r--r--   0        0        0     7592 2024-03-27 09:00:42.269603 sd_tools-1.3.0/src/sd_tools/plugins/http/assets/index.html
--rw-r--r--   0        0        0     3397 2024-03-22 07:50:25.752370 sd_tools-1.3.0/src/sd_tools/plugins/http/assets/index.js
--rw-r--r--   0        0        0     2848 2024-03-25 02:14:33.353431 sd_tools-1.3.0/src/sd_tools/plugins/http/http.py
--rw-r--r--   0        0        0      692 2024-03-16 02:41:10.652555 sd_tools-1.3.0/src/sd_tools/plugins/image.py
--rw-r--r--   0        0        0     2457 2024-03-16 03:46:17.495924 sd_tools-1.3.0/src/sd_tools/plugins/inpainting.py
--rw-r--r--   0        0        0     3030 2024-03-15 06:51:01.708178 sd_tools-1.3.0/src/sd_tools/plugins/instantid.py
--rw-r--r--   0        0        0    20798 2024-03-13 13:59:00.332472 sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/attention_processor.py
--rw-r--r--   0        0        0    17070 2024-03-13 13:59:00.332579 sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/attention_processor_faceid.py
--rw-r--r--   0        0        0    17226 2024-03-20 12:27:39.739221 sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/ip_adapter.py
--rw-r--r--   0        0        0    22087 2024-03-15 06:28:27.306922 sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/ip_adapter_faceid.py
--rw-r--r--   0        0        0    21634 2024-03-17 08:01:00.583128 sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/ip_adapter_faceid_separate.py
--rw-r--r--   0        0        0     5059 2024-03-13 13:59:00.332902 sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/resampler.py
--rw-r--r--   0        0        0     2831 2024-03-13 13:59:00.332994 sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/utils.py
--rw-r--r--   0        0        0     1526 2024-03-20 12:11:59.416590 sd_tools-1.3.0/src/sd_tools/plugins/ip_composition.py
--rw-r--r--   0        0        0     1533 2024-03-20 12:27:39.739604 sd_tools-1.3.0/src/sd_tools/plugins/ip_composition_xl.py
--rw-r--r--   0        0        0      765 2024-03-17 02:05:40.016028 sd_tools-1.3.0/src/sd_tools/plugins/ipa.py
--rw-r--r--   0        0        0     1604 2024-03-17 05:43:08.698284 sd_tools-1.3.0/src/sd_tools/plugins/ipa_faceid.py
--rw-r--r--   0        0        0     2161 2024-03-15 06:02:45.860113 sd_tools-1.3.0/src/sd_tools/plugins/ipa_faceid_plus.py
--rw-r--r--   0        0        0     1969 2024-03-17 08:00:09.256096 sd_tools-1.3.0/src/sd_tools/plugins/ipa_faceid_portrait.py
--rw-r--r--   0        0        0     2201 2024-03-17 04:01:53.203275 sd_tools-1.3.0/src/sd_tools/plugins/ipa_plus.py
--rw-r--r--   0        0        0    19054 2024-03-21 10:34:31.685732 sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/__init__.py
--rw-r--r--   0        0        0    11187 2024-03-21 01:42:22.419170 sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/attention_sharing.py
--rw-r--r--   0        0        0      397 2024-03-21 01:42:22.419271 sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/enums.py
--rw-r--r--   0        0        0    11967 2024-03-21 01:42:22.419362 sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/models.py
--rw-r--r--   0        0        0     3185 2024-03-21 01:42:22.419449 sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/utils.py
--rw-r--r--   0        0        0      650 2024-03-17 04:23:18.302633 sd_tools-1.3.0/src/sd_tools/plugins/lcm.py
--rw-r--r--   0        0        0     1746 2024-03-15 06:30:59.313872 sd_tools-1.3.0/src/sd_tools/plugins/lightning.py
--rw-r--r--   0        0        0      778 2024-03-20 08:03:36.666890 sd_tools-1.3.0/src/sd_tools/plugins/lora.py
--rw-r--r--   0        0        0      551 2024-03-17 03:54:21.945070 sd_tools-1.3.0/src/sd_tools/plugins/model.py
--rw-r--r--   0        0        0      489 2024-03-16 02:06:36.963210 sd_tools-1.3.0/src/sd_tools/plugins/modelXL.py
--rw-r--r--   0        0        0      399 2024-03-17 03:45:38.145127 sd_tools-1.3.0/src/sd_tools/plugins/offline.py
--rw-r--r--   0        0        0      995 2024-03-20 05:57:58.633564 sd_tools-1.3.0/src/sd_tools/plugins/output.py
--rw-r--r--   0        0        0     1527 2024-03-15 05:18:15.440399 sd_tools-1.3.0/src/sd_tools/plugins/photo_maker.py
--rw-r--r--   0        0        0      701 2024-03-26 11:35:22.155512 sd_tools-1.3.0/src/sd_tools/plugins/pipe.py
--rw-r--r--   0        0        0    41018 2024-03-13 13:59:00.333812 sd_tools-1.3.0/src/sd_tools/plugins/pipeline_stable_diffusion_xl_instantid.py
--rw-r--r--   0        0        0     1773 2024-03-20 12:27:39.733090 sd_tools-1.3.0/src/sd_tools/plugins/pix2pix/__init__.py
--rw-r--r--   0        0        0     1923 2024-03-20 12:27:39.733324 sd_tools-1.3.0/src/sd_tools/plugins/pix2pix/model.py
--rw-r--r--   0        0        0     8079 2024-03-20 12:27:39.733545 sd_tools-1.3.0/src/sd_tools/plugins/pix2pix/pix2pix_turbo.py
--rw-r--r--   0        0        0     1784 2024-03-14 06:40:40.355607 sd_tools-1.3.0/src/sd_tools/plugins/pose.py
--rw-r--r--   0        0        0      923 2024-03-16 02:17:20.864538 sd_tools-1.3.0/src/sd_tools/plugins/prompt.py
--rw-r--r--   0        0        0      864 2024-03-14 02:21:39.697871 sd_tools-1.3.0/src/sd_tools/plugins/res_adapter.py
--rw-r--r--   0        0        0     2183 2024-03-16 04:59:14.396579 sd_tools-1.3.0/src/sd_tools/plugins/run.py
--rw-r--r--   0        0        0      584 2024-03-16 01:29:12.525848 sd_tools-1.3.0/src/sd_tools/plugins/safetensor.py
--rw-r--r--   0        0        0     1648 2024-03-24 09:16:25.270006 sd_tools-1.3.0/src/sd_tools/plugins/scheduler.py
--rw-r--r--   0        0        0      417 2024-03-14 02:49:42.682570 sd_tools-1.3.0/src/sd_tools/plugins/seed.py
--rw-r--r--   0        0        0      937 2024-03-17 03:59:31.494227 sd_tools-1.3.0/src/sd_tools/plugins/size.py
--rw-r--r--   0        0        0      467 2024-03-16 00:52:49.602175 sd_tools-1.3.0/src/sd_tools/plugins/steps.py
--rw-r--r--   0        0        0      615 2024-03-13 13:59:00.334611 sd_tools-1.3.0/src/sd_tools/plugins/tcd.py
--rw-r--r--   0        0        0     2159 2024-03-20 12:27:39.733673 sd_tools-1.3.0/src/sd_tools/plugins/utils.py
--rw-r--r--   0        0        0      562 2024-03-24 02:00:45.604124 sd_tools-1.3.0/src/sd_tools/plugins/wrong.py
--rw-r--r--   0        0        0      591 2024-03-27 01:31:44.292219 sd_tools-1.3.0/src/sd_tools/plugins/yoso.py
--rw-r--r--   0        0        0     2591 2024-03-27 01:45:09.311032 sd_tools-1.3.0/src/sd_tools/sd.py
--rw-r--r--   0        0        0     3196 2024-03-24 04:09:38.232342 sd_tools-1.3.0/src/sd_tools/sdxl.py
--rw-r--r--   0        0        0      128 2024-03-27 02:43:29.057940 sd_tools-1.3.0/tailwind.config.js
--rw-r--r--   0        0        0      814 2024-03-15 06:37:01.430389 sd_tools-1.3.0/test.py
--rw-r--r--   0        0        0    63588 2024-03-15 05:06:34.040124 sd_tools-1.3.0/test/ghibli/kazetachinu022.webp
--rw-r--r--   0        0        0    72868 2024-03-15 05:06:33.984328 sd_tools-1.3.0/test/ghibli/kazetachinu023.webp
--rw-r--r--   0        0        0    74852 2024-03-15 05:06:34.098337 sd_tools-1.3.0/test/ghibli/kazetachinu024.webp
--rw-r--r--   0        0        0    81834 2024-03-15 05:06:33.696935 sd_tools-1.3.0/test/ghibli/kazetachinu028.webp
--rw-r--r--   0        0        0    54982 2024-03-15 05:06:33.805085 sd_tools-1.3.0/test/ghibli/kazetachinu043.webp
--rw-r--r--   0        0        0    57434 2024-03-15 05:06:33.928397 sd_tools-1.3.0/test/ghibli/kazetachinu047.webp
--rw-r--r--   0        0        0    53568 2024-03-15 05:06:33.751835 sd_tools-1.3.0/test/ghibli/kazetachinu048.webp
--rw-r--r--   0        0        0   118666 2024-03-15 05:06:33.870865 sd_tools-1.3.0/test/ghibli/kazetachinu050.webp
--rw-r--r--   0        0        0   417414 2024-03-17 04:29:44.684835 sd_tools-1.3.0/test/tesla.webp
--rw-r--r--   0        0        0     8639 1970-01-01 00:00:00.000000 sd_tools-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       62 2024-03-20 12:27:39.732811 sd_tools-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1066 2024-03-13 13:59:00.328247 sd_tools-1.4.0/LICENSE
+-rw-r--r--   0        0        0     7753 2024-04-24 12:29:24.902311 sd_tools-1.4.0/README.md
+-rw-r--r--   0        0        0     1102 2024-04-24 12:29:50.192654 sd_tools-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-03-13 13:59:00.331410 sd_tools-1.4.0/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2024-03-14 11:59:50.653597 sd_tools-1.4.0/src/sd_tools/__init__.py
+-rw-r--r--   0        0        0     1796 2024-04-01 09:24:34.609141 sd_tools-1.4.0/src/sd_tools/misc.py
+-rw-r--r--   0        0        0     2003 2024-03-27 12:14:11.338055 sd_tools-1.4.0/src/sd_tools/plugins/base.py
+-rw-r--r--   0        0        0     1855 2024-03-20 02:37:31.819560 sd_tools-1.4.0/src/sd_tools/plugins/canny.py
+-rw-r--r--   0        0        0      401 2024-03-14 06:20:33.776026 sd_tools-1.4.0/src/sd_tools/plugins/cfg.py
+-rw-r--r--   0        0        0      244 2024-03-14 06:40:40.391656 sd_tools-1.4.0/src/sd_tools/plugins/debug.py
+-rw-r--r--   0        0        0     1319 2024-03-14 06:40:40.352819 sd_tools-1.4.0/src/sd_tools/plugins/depth.py
+-rw-r--r--   0        0        0      459 2024-03-14 06:40:40.395319 sd_tools-1.4.0/src/sd_tools/plugins/device.py
+-rw-r--r--   0        0        0      460 2024-03-24 04:09:01.813371 sd_tools-1.4.0/src/sd_tools/plugins/dpo.py
+-rw-r--r--   0        0        0     1755 2024-03-22 08:49:17.470727 sd_tools-1.4.0/src/sd_tools/plugins/http/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 06:14:55.106370 sd_tools-1.4.0/src/sd_tools/plugins/http/assets/dom.js
+-rw-r--r--   0        0        0      344 2024-03-27 02:35:53.522855 sd_tools-1.4.0/src/sd_tools/plugins/http/assets/index.css
+-rw-r--r--   0        0        0     7592 2024-03-27 09:00:42.269603 sd_tools-1.4.0/src/sd_tools/plugins/http/assets/index.html
+-rw-r--r--   0        0        0     3397 2024-03-22 07:50:25.752370 sd_tools-1.4.0/src/sd_tools/plugins/http/assets/index.js
+-rw-r--r--   0        0        0     2848 2024-03-25 02:14:33.353431 sd_tools-1.4.0/src/sd_tools/plugins/http/http.py
+-rw-r--r--   0        0        0      949 2024-04-24 11:35:48.347473 sd_tools-1.4.0/src/sd_tools/plugins/hyper.py
+-rw-r--r--   0        0        0      692 2024-03-16 02:41:10.652555 sd_tools-1.4.0/src/sd_tools/plugins/image.py
+-rw-r--r--   0        0        0     2457 2024-03-16 03:46:17.495924 sd_tools-1.4.0/src/sd_tools/plugins/inpainting.py
+-rw-r--r--   0        0        0     3030 2024-03-15 06:51:01.708178 sd_tools-1.4.0/src/sd_tools/plugins/instantid.py
+-rw-r--r--   0        0        0    20798 2024-03-13 13:59:00.332472 sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/attention_processor.py
+-rw-r--r--   0        0        0    17070 2024-03-13 13:59:00.332579 sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/attention_processor_faceid.py
+-rw-r--r--   0        0        0    17226 2024-03-20 12:27:39.739221 sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/ip_adapter.py
+-rw-r--r--   0        0        0    22087 2024-03-15 06:28:27.306922 sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/ip_adapter_faceid.py
+-rw-r--r--   0        0        0    21634 2024-03-17 08:01:00.583128 sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/ip_adapter_faceid_separate.py
+-rw-r--r--   0        0        0     5059 2024-03-13 13:59:00.332902 sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/resampler.py
+-rw-r--r--   0        0        0     2831 2024-03-13 13:59:00.332994 sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/utils.py
+-rw-r--r--   0        0        0     1526 2024-03-20 12:11:59.416590 sd_tools-1.4.0/src/sd_tools/plugins/ip_composition.py
+-rw-r--r--   0        0        0     1533 2024-03-20 12:27:39.739604 sd_tools-1.4.0/src/sd_tools/plugins/ip_composition_xl.py
+-rw-r--r--   0        0        0      765 2024-03-17 02:05:40.016028 sd_tools-1.4.0/src/sd_tools/plugins/ipa.py
+-rw-r--r--   0        0        0     1604 2024-03-17 05:43:08.698284 sd_tools-1.4.0/src/sd_tools/plugins/ipa_faceid.py
+-rw-r--r--   0        0        0     2161 2024-03-15 06:02:45.860113 sd_tools-1.4.0/src/sd_tools/plugins/ipa_faceid_plus.py
+-rw-r--r--   0        0        0     1969 2024-03-17 08:00:09.256096 sd_tools-1.4.0/src/sd_tools/plugins/ipa_faceid_portrait.py
+-rw-r--r--   0        0        0     2201 2024-03-17 04:01:53.203275 sd_tools-1.4.0/src/sd_tools/plugins/ipa_plus.py
+-rw-r--r--   0        0        0    19054 2024-03-21 10:34:31.685732 sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/__init__.py
+-rw-r--r--   0        0        0    11187 2024-03-21 01:42:22.419170 sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/attention_sharing.py
+-rw-r--r--   0        0        0      397 2024-03-21 01:42:22.419271 sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/enums.py
+-rw-r--r--   0        0        0    11967 2024-03-21 01:42:22.419362 sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/models.py
+-rw-r--r--   0        0        0     3185 2024-03-21 01:42:22.419449 sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/utils.py
+-rw-r--r--   0        0        0      650 2024-03-17 04:23:18.302633 sd_tools-1.4.0/src/sd_tools/plugins/lcm.py
+-rw-r--r--   0        0        0     1746 2024-03-15 06:30:59.313872 sd_tools-1.4.0/src/sd_tools/plugins/lightning.py
+-rw-r--r--   0        0        0      778 2024-03-20 08:03:36.666890 sd_tools-1.4.0/src/sd_tools/plugins/lora.py
+-rw-r--r--   0        0        0      551 2024-03-17 03:54:21.945070 sd_tools-1.4.0/src/sd_tools/plugins/model.py
+-rw-r--r--   0        0        0      489 2024-03-16 02:06:36.963210 sd_tools-1.4.0/src/sd_tools/plugins/modelXL.py
+-rw-r--r--   0        0        0      399 2024-03-17 03:45:38.145127 sd_tools-1.4.0/src/sd_tools/plugins/offline.py
+-rw-r--r--   0        0        0      995 2024-03-20 05:57:58.633564 sd_tools-1.4.0/src/sd_tools/plugins/output.py
+-rw-r--r--   0        0        0     1527 2024-03-15 05:18:15.440399 sd_tools-1.4.0/src/sd_tools/plugins/photo_maker.py
+-rw-r--r--   0        0        0      701 2024-03-26 11:35:22.155512 sd_tools-1.4.0/src/sd_tools/plugins/pipe.py
+-rw-r--r--   0        0        0    41018 2024-03-13 13:59:00.333812 sd_tools-1.4.0/src/sd_tools/plugins/pipeline_stable_diffusion_xl_instantid.py
+-rw-r--r--   0        0        0     1773 2024-03-20 12:27:39.733090 sd_tools-1.4.0/src/sd_tools/plugins/pix2pix/__init__.py
+-rw-r--r--   0        0        0     1923 2024-03-20 12:27:39.733324 sd_tools-1.4.0/src/sd_tools/plugins/pix2pix/model.py
+-rw-r--r--   0        0        0     8079 2024-03-20 12:27:39.733545 sd_tools-1.4.0/src/sd_tools/plugins/pix2pix/pix2pix_turbo.py
+-rw-r--r--   0        0        0     1784 2024-03-14 06:40:40.355607 sd_tools-1.4.0/src/sd_tools/plugins/pose.py
+-rw-r--r--   0        0        0      923 2024-03-16 02:17:20.864538 sd_tools-1.4.0/src/sd_tools/plugins/prompt.py
+-rw-r--r--   0        0        0      864 2024-03-14 02:21:39.697871 sd_tools-1.4.0/src/sd_tools/plugins/res_adapter.py
+-rw-r--r--   0        0        0     2183 2024-03-16 04:59:14.396579 sd_tools-1.4.0/src/sd_tools/plugins/run.py
+-rw-r--r--   0        0        0      584 2024-03-16 01:29:12.525848 sd_tools-1.4.0/src/sd_tools/plugins/safetensor.py
+-rw-r--r--   0        0        0     1648 2024-03-24 09:16:25.270006 sd_tools-1.4.0/src/sd_tools/plugins/scheduler.py
+-rw-r--r--   0        0        0      417 2024-03-14 02:49:42.682570 sd_tools-1.4.0/src/sd_tools/plugins/seed.py
+-rw-r--r--   0        0        0      937 2024-03-17 03:59:31.494227 sd_tools-1.4.0/src/sd_tools/plugins/size.py
+-rw-r--r--   0        0        0      467 2024-03-16 00:52:49.602175 sd_tools-1.4.0/src/sd_tools/plugins/steps.py
+-rw-r--r--   0        0        0      615 2024-03-13 13:59:00.334611 sd_tools-1.4.0/src/sd_tools/plugins/tcd.py
+-rw-r--r--   0        0        0     2159 2024-03-20 12:27:39.733673 sd_tools-1.4.0/src/sd_tools/plugins/utils.py
+-rw-r--r--   0        0        0      562 2024-03-24 02:00:45.604124 sd_tools-1.4.0/src/sd_tools/plugins/wrong.py
+-rw-r--r--   0        0        0      591 2024-03-27 01:31:44.292219 sd_tools-1.4.0/src/sd_tools/plugins/yoso.py
+-rw-r--r--   0        0        0     2591 2024-03-29 06:08:14.851736 sd_tools-1.4.0/src/sd_tools/sd.py
+-rw-r--r--   0        0        0     3261 2024-04-24 11:22:46.008117 sd_tools-1.4.0/src/sd_tools/sdxl.py
+-rw-r--r--   0        0        0      128 2024-03-27 02:43:29.057940 sd_tools-1.4.0/tailwind.config.js
+-rw-r--r--   0        0        0      814 2024-03-15 06:37:01.430389 sd_tools-1.4.0/test.py
+-rw-r--r--   0        0        0    63588 2024-03-15 05:06:34.040124 sd_tools-1.4.0/test/ghibli/kazetachinu022.webp
+-rw-r--r--   0        0        0    72868 2024-03-15 05:06:33.984328 sd_tools-1.4.0/test/ghibli/kazetachinu023.webp
+-rw-r--r--   0        0        0    74852 2024-03-15 05:06:34.098337 sd_tools-1.4.0/test/ghibli/kazetachinu024.webp
+-rw-r--r--   0        0        0    81834 2024-03-15 05:06:33.696935 sd_tools-1.4.0/test/ghibli/kazetachinu028.webp
+-rw-r--r--   0        0        0    54982 2024-03-15 05:06:33.805085 sd_tools-1.4.0/test/ghibli/kazetachinu043.webp
+-rw-r--r--   0        0        0    57434 2024-03-15 05:06:33.928397 sd_tools-1.4.0/test/ghibli/kazetachinu047.webp
+-rw-r--r--   0        0        0    53568 2024-03-15 05:06:33.751835 sd_tools-1.4.0/test/ghibli/kazetachinu048.webp
+-rw-r--r--   0        0        0   118666 2024-03-15 05:06:33.870865 sd_tools-1.4.0/test/ghibli/kazetachinu050.webp
+-rw-r--r--   0        0        0   417414 2024-03-17 04:29:44.684835 sd_tools-1.4.0/test/tesla.webp
+-rw-r--r--   0        0        0     8650 1970-01-01 00:00:00.000000 sd_tools-1.4.0/PKG-INFO
```

### Comparing `sd_tools-1.3.0/LICENSE` & `sd_tools-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/README.md` & `sd_tools-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
  --steps 8 \
  --size 1024x576 \
  --loras ./lora1.safetensors ./lora2.safetensors:0.8 \
 ```
 
 ### Speed Up Generation
 
-Using `--lcm`, `--tcd` or `--lightning` to speed up generation, not necessary for turbo/lightning models:
+Using `--lcm`, `--tcd`, `--hyper` or `--lightning` to speed up generation, not necessary for turbo/lightning models:
 
 ```shell
 sdxl 'locomotive' \
  --model SG161222/RealVisXL_V4.0 \
  --steps 4 \
  --size 1024x576 \
  --tcd 1 \
```

### Comparing `sd_tools-1.3.0/pyproject.toml` & `sd_tools-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sd_tools"
-version = "1.3.0"
+version = "1.4.0"
 authors = [{ name = "Feng Zhou", email = "zf.pascal@gmail.com" }]
 description = "command line tool for stable diffusion"
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -32,10 +32,11 @@
 
 [project.urls]
 Home = "https://github.com/zweifisch/sd-cli"
 
 [project.scripts]
 sdxl = "sd_tools.sdxl:main"
 sd = "sd_tools.sd:main"
-pt2st = "sd_tools.misc:pt2st"
-st-inspect = "sd_tools.misc:st_inspect"
-sd-to-fp16 = "sd_tools.misc:to_fp16"
+sd-pt2st = "sd_tools.misc:pt2st"
+sd-inspect = "sd_tools.misc:st_inspect"
+sd-2fp16 = "sd_tools.misc:to_fp16"
+sd-path = "sd_tools.misc:hf_path"
```

### Comparing `sd_tools-1.3.0/src/sd_tools/misc.py` & `sd_tools-1.4.0/src/sd_tools/misc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from huggingface_hub.repocard import hf_hub_download
 import torch
 import json
 import struct
 from argparse import ArgumentParser
 from safetensors.torch import save_file
 import operator as op
 from functools import reduce
@@ -14,18 +15,24 @@
     args = parser.parse_args()
 
     save_file(torch.load(args.input), args.output)
 
 def st_inspect():
 
     parser = ArgumentParser('safetensor inspect')
-    parser.add_argument('file', type=str)
+    parser.add_argument('--file', type=str)
+    parser.add_argument('--hf', type=str)
     args = parser.parse_args()
 
-    with open(args.file, 'rb') as f:
+    path = args.file
+    if args.hf:
+        ns, project, filename = args.hf.split('/', 2)
+        path = hf_hub_download(repo_id=f"{ns}/{project}", filename=filename, local_files_only=True)
+
+    with open(path, 'rb') as f:
         files = json.loads(f.read(struct.unpack('<Q', f.read(8))[0]).decode())
         for k, v in files.items():
             if not v.get('shape'): continue
             print(k, reduce(op.mul, v['shape'], 1), 'x'.join(map(str, v['shape'])))
 
 def to_fp16():
 
@@ -34,7 +41,16 @@
     parser.add_argument('output', type=str)
     args = parser.parse_args()
 
     from diffusers import AutoPipelineForText2Image
     pipe = AutoPipelineForText2Image.from_pretrained(args.model, torch_dtype=torch.float16)
 
     pipe.save_pretrained(args.output, variant='fp16')
+
+def hf_path():
+
+    parser = ArgumentParser('get hf cache path')
+    parser.add_argument('file', type=str)
+    args = parser.parse_args()
+
+    ns, project, filename = args.file.split('/', 2)
+    print(hf_hub_download(repo_id=f"{ns}/{project}", filename=filename, local_files_only=True))
```

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/base.py` & `sd_tools-1.4.0/src/sd_tools/plugins/base.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/canny.py` & `sd_tools-1.4.0/src/sd_tools/plugins/canny.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/depth.py` & `sd_tools-1.4.0/src/sd_tools/plugins/depth.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/http/__init__.py` & `sd_tools-1.4.0/src/sd_tools/plugins/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/http/assets/index.html` & `sd_tools-1.4.0/src/sd_tools/plugins/http/assets/index.html`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/http/assets/index.js` & `sd_tools-1.4.0/src/sd_tools/plugins/http/assets/index.js`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/http/http.py` & `sd_tools-1.4.0/src/sd_tools/plugins/http/http.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/image.py` & `sd_tools-1.4.0/src/sd_tools/plugins/image.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/inpainting.py` & `sd_tools-1.4.0/src/sd_tools/plugins/inpainting.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/instantid.py` & `sd_tools-1.4.0/src/sd_tools/plugins/instantid.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/attention_processor.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/attention_processor.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/attention_processor_faceid.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/attention_processor_faceid.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/ip_adapter.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/ip_adapter.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/ip_adapter_faceid.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/ip_adapter_faceid.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/ip_adapter_faceid_separate.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/ip_adapter_faceid_separate.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/resampler.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/resampler.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_adapter/utils.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_adapter/utils.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_composition.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_composition.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ip_composition_xl.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ip_composition_xl.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ipa.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ipa.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ipa_faceid.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ipa_faceid.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ipa_faceid_plus.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ipa_faceid_plus.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ipa_faceid_portrait.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ipa_faceid_portrait.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/ipa_plus.py` & `sd_tools-1.4.0/src/sd_tools/plugins/ipa_plus.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/__init__.py` & `sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/attention_sharing.py` & `sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/attention_sharing.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/models.py` & `sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/models.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/layerdiffusion/utils.py` & `sd_tools-1.4.0/src/sd_tools/plugins/layerdiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/lcm.py` & `sd_tools-1.4.0/src/sd_tools/plugins/lcm.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/lightning.py` & `sd_tools-1.4.0/src/sd_tools/plugins/lightning.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/lora.py` & `sd_tools-1.4.0/src/sd_tools/plugins/lora.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/model.py` & `sd_tools-1.4.0/src/sd_tools/plugins/model.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/output.py` & `sd_tools-1.4.0/src/sd_tools/plugins/output.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/photo_maker.py` & `sd_tools-1.4.0/src/sd_tools/plugins/photo_maker.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/pipe.py` & `sd_tools-1.4.0/src/sd_tools/plugins/pipe.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/pipeline_stable_diffusion_xl_instantid.py` & `sd_tools-1.4.0/src/sd_tools/plugins/pipeline_stable_diffusion_xl_instantid.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/pix2pix/__init__.py` & `sd_tools-1.4.0/src/sd_tools/plugins/pix2pix/__init__.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/pix2pix/model.py` & `sd_tools-1.4.0/src/sd_tools/plugins/pix2pix/model.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/pix2pix/pix2pix_turbo.py` & `sd_tools-1.4.0/src/sd_tools/plugins/pix2pix/pix2pix_turbo.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/pose.py` & `sd_tools-1.4.0/src/sd_tools/plugins/pose.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/prompt.py` & `sd_tools-1.4.0/src/sd_tools/plugins/prompt.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/res_adapter.py` & `sd_tools-1.4.0/src/sd_tools/plugins/res_adapter.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/run.py` & `sd_tools-1.4.0/src/sd_tools/plugins/run.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/safetensor.py` & `sd_tools-1.4.0/src/sd_tools/plugins/safetensor.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/scheduler.py` & `sd_tools-1.4.0/src/sd_tools/plugins/scheduler.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/size.py` & `sd_tools-1.4.0/src/sd_tools/plugins/size.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/tcd.py` & `sd_tools-1.4.0/src/sd_tools/plugins/tcd.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/utils.py` & `sd_tools-1.4.0/src/sd_tools/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/wrong.py` & `sd_tools-1.4.0/src/sd_tools/plugins/wrong.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/plugins/yoso.py` & `sd_tools-1.4.0/src/sd_tools/plugins/yoso.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/sd.py` & `sd_tools-1.4.0/src/sd_tools/sd.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/src/sd_tools/sdxl.py` & `sd_tools-1.4.0/src/sd_tools/sdxl.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from argparse import RawTextHelpFormatter
 
 from sd_tools.plugins.safetensor import PluginSafetensor
 
 from .plugins.debug import PluginDebug
 from .plugins.base import Context, PipeOptions, PipelineOptions
 from .plugins.lightning import PluginLightning
+from .plugins.hyper import PluginHyper
 from .plugins.photo_maker import PluginPhotoMaker
 from .plugins.cfg import PluginCFG
 from .plugins.size import PluginSize
 from .plugins.prompt import PluginPrompt
 from .plugins.wrong import PluginWrong
 from .plugins.modelXL import PluginModelXL
 from .plugins.pipe import PluginPipe
@@ -68,14 +69,15 @@
         PluginSteps(ctx),
         PluginSeed(ctx),
         PluginWrong(ctx),
         PluginDPO(ctx),
         PluginTCD(ctx),
         PluginLCM(ctx),
         PluginLightning(ctx),
+        PluginHyper(ctx),
         PluginOutput(ctx),
         PluginCanny(ctx),
         PluginPose(ctx),
         PluginDepth(ctx),
         PluginPhotoMaker(ctx),
         # PluginIPAdaptor(ctx),
         PluginIPAdaptorPlus(ctx),
```

### Comparing `sd_tools-1.3.0/test.py` & `sd_tools-1.4.0/test.py`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/ghibli/kazetachinu022.webp` & `sd_tools-1.4.0/test/ghibli/kazetachinu022.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/ghibli/kazetachinu023.webp` & `sd_tools-1.4.0/test/ghibli/kazetachinu023.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/ghibli/kazetachinu024.webp` & `sd_tools-1.4.0/test/ghibli/kazetachinu024.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/ghibli/kazetachinu028.webp` & `sd_tools-1.4.0/test/ghibli/kazetachinu028.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/ghibli/kazetachinu043.webp` & `sd_tools-1.4.0/test/ghibli/kazetachinu043.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/ghibli/kazetachinu047.webp` & `sd_tools-1.4.0/test/ghibli/kazetachinu047.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/ghibli/kazetachinu048.webp` & `sd_tools-1.4.0/test/ghibli/kazetachinu048.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/ghibli/kazetachinu050.webp` & `sd_tools-1.4.0/test/ghibli/kazetachinu050.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/test/tesla.webp` & `sd_tools-1.4.0/test/tesla.webp`

 * *Files identical despite different names*

### Comparing `sd_tools-1.3.0/PKG-INFO` & `sd_tools-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd_tools
-Version: 1.3.0
+Version: 1.4.0
 Summary: command line tool for stable diffusion
 Author-email: Feng Zhou <zf.pascal@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -137,15 +137,15 @@
  --steps 8 \
  --size 1024x576 \
  --loras ./lora1.safetensors ./lora2.safetensors:0.8 \
 ```
 
 ### Speed Up Generation
 
-Using `--lcm`, `--tcd` or `--lightning` to speed up generation, not necessary for turbo/lightning models:
+Using `--lcm`, `--tcd`, `--hyper` or `--lightning` to speed up generation, not necessary for turbo/lightning models:
 
 ```shell
 sdxl 'locomotive' \
  --model SG161222/RealVisXL_V4.0 \
  --steps 4 \
  --size 1024x576 \
  --tcd 1 \
```

