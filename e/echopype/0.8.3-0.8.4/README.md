# Comparing `tmp/echopype-0.8.3.tar.gz` & `tmp/echopype-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echopype-0.8.3.tar", last modified: Mon Dec 25 19:11:58 2023, max compression
+gzip compressed data, was "echopype-0.8.4.tar", last modified: Wed Apr 24 17:45:35 2024, max compression
```

## Comparing `echopype-0.8.3.tar` & `echopype-0.8.4.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-25 19:11:54.000000 echopype-0.8.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2023-12-25 19:11:54.000000 echopype-0.8.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-25 19:11:54.000000 echopype-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-25 19:11:54.000000 echopype-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-25 19:11:58.763023 echopype-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2023-12-25 19:11:54.000000 echopype-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-25 19:11:58.000000 echopype-0.8.3/_echopype_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.755023 echopype-0.8.3/echopype/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.755023 echopype-0.8.3/echopype/calibrate/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21887 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/cal_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/calibrate_azfp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/calibrate_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24233 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/calibrate_ek.py
--rw-r--r--   0 runner    (1001) docker     (127)    19532 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10347 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/ek80_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14142 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/env_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/env_params_old.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/calibrate/range.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.755023 echopype-0.8.3/echopype/clean/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/clean/noise_est.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.759023 echopype-0.8.3/echopype/commongrid/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/commongrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/commongrid/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/commongrid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.759023 echopype-0.8.3/echopype/consolidate/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/consolidate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15742 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/consolidate/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/consolidate/split_beam_angle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.759023 echopype-0.8.3/echopype/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44472 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/ad2cp_fields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16885 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    72040 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/parse_ad2cp.py
--rw-r--r--   0 runner    (1001) docker     (127)    19612 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/parse_azfp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26133 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/parse_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/parse_ek60.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/parse_ek80.py
--rw-r--r--   0 runner    (1001) docker     (127)    24355 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/set_groups_ad2cp.py
--rw-r--r--   0 runner    (1001) docker     (127)    35922 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/set_groups_azfp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12963 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/set_groups_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31501 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/set_groups_ek60.py
--rw-r--r--   0 runner    (1001) docker     (127)    55076 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/set_groups_ek80.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.759023 echopype-0.8.3/echopype/convert/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/utils/ek_date_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    21214 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/utils/ek_raw_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    66310 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/utils/ek_raw_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/convert/utils/ek_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.759023 echopype-0.8.3/echopype/echodata/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36975 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.759023 echopype-0.8.3/echopype/echodata/convention/
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/convention/1.0.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/convention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/convention/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/convention/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25555 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/echodata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.759023 echopype-0.8.3/echopype/echodata/sensor_ep_version_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/sensor_ep_version_mapping/ep_version_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    39212 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/sensor_ep_version_mapping/v05x_to_v06x.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/simrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/utils_platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/echodata/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.751023 echopype-0.8.3/echopype/echodata/widgets/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/echodata/widgets/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/widgets/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/echodata/widgets/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/widgets/static/html/icons-svg-inline.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/echodata/widgets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/widgets/templates/echodata.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/widgets/templates/style.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/echodata/widgets/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21013 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/mask/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/mask/freq_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/metrics/summary_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/qc/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/qc/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/utils/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/utils/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    16905 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/utils/prov.py
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/utils/uwa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.763023 echopype-0.8.3/echopype/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/visualize/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/visualize/cm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2023-12-25 19:11:54.000000 echopype-0.8.3/echopype/visualize/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 19:11:58.755023 echopype-0.8.3/echopype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-25 19:11:58.000000 echopype-0.8.3/echopype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2023-12-25 19:11:58.000000 echopype-0.8.3/echopype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 19:11:58.000000 echopype-0.8.3/echopype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-12-25 19:11:58.000000 echopype-0.8.3/echopype.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-25 19:11:58.000000 echopype-0.8.3/echopype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-12-25 19:11:54.000000 echopype-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-25 19:11:54.000000 echopype-0.8.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-12-25 19:11:54.000000 echopype-0.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-25 19:11:58.763023 echopype-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-25 19:11:54.000000 echopype-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.009311 echopype-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 17:45:30.000000 echopype-0.8.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-24 17:45:30.000000 echopype-0.8.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 17:45:30.000000 echopype-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-24 17:45:30.000000 echopype-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-24 17:45:35.009311 echopype-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-24 17:45:30.000000 echopype-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 17:45:34.000000 echopype-0.8.4/_echopype_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:34.997310 echopype-0.8.4/echopype/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.001311 echopype-0.8.4/echopype/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21881 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/cal_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/calibrate_azfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/calibrate_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24445 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/calibrate_ek.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19532 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/ek80_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14232 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/env_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/env_params_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/calibrate/range.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.001311 echopype-0.8.4/echopype/clean/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/clean/noise_est.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.001311 echopype-0.8.4/echopype/commongrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/commongrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/commongrid/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18993 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/commongrid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.001311 echopype-0.8.4/echopype/consolidate/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/consolidate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/consolidate/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/consolidate/split_beam_angle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.001311 echopype-0.8.4/echopype/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44472 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/ad2cp_fields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72040 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/parse_ad2cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/parse_azfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26133 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/parse_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/parse_ek60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/parse_ek80.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24411 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/set_groups_ad2cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35408 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/set_groups_azfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/set_groups_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31501 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/set_groups_ek60.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55132 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/set_groups_ek80.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.001311 echopype-0.8.4/echopype/convert/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/utils/ek_date_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/utils/ek_raw_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66310 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/utils/ek_raw_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/convert/utils/ek_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/echodata/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37063 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/echodata/convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/convention/1.0.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/convention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/convention/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/convention/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25559 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/echodata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/echodata/sensor_ep_version_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/sensor_ep_version_mapping/ep_version_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39228 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/sensor_ep_version_mapping/v05x_to_v06x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/simrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/utils_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/echodata/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:34.997310 echopype-0.8.4/echopype/echodata/widgets/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/echodata/widgets/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/widgets/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/echodata/widgets/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/widgets/static/html/icons-svg-inline.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/echodata/widgets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/widgets/templates/echodata.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/widgets/templates/style.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/echodata/widgets/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24734 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/mask/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/mask/freq_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/metrics/summary_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/qc/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.005311 echopype-0.8.4/echopype/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/utils/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/utils/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16906 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/utils/prov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/utils/uwa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:35.009311 echopype-0.8.4/echopype/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/visualize/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/visualize/cm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-24 17:45:30.000000 echopype-0.8.4/echopype/visualize/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:45:34.997310 echopype-0.8.4/echopype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-24 17:45:34.000000 echopype-0.8.4/echopype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-24 17:45:34.000000 echopype-0.8.4/echopype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:45:34.000000 echopype-0.8.4/echopype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 17:45:34.000000 echopype-0.8.4/echopype.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 17:45:34.000000 echopype-0.8.4/echopype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-24 17:45:30.000000 echopype-0.8.4/gsoc_contrib_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 17:45:30.000000 echopype-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-24 17:45:30.000000 echopype-0.8.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 17:45:30.000000 echopype-0.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 17:45:35.009311 echopype-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 17:45:30.000000 echopype-0.8.4/setup.py
```

### Comparing `echopype-0.8.3/CITATION.cff` & `echopype-0.8.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/LICENSE` & `echopype-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/PKG-INFO` & `echopype-0.8.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: echopype
-Version: 0.8.3
-Summary: Enhancing the interoperability and scalability in analyzing ocean sonar data
-Home-page: https://github.com/OSOceanAcoustics/echopype
-Author: Wu-Jung Lee
-Author-email: leewujung@gmail.com
-Maintainer: Wu-Jung Lee
-Maintainer-email: leewujung@gmail.com
-License: Apache License, Version 2.0
-Platform: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: plot
-License-File: LICENSE
-
 <div align="center">
   <img src="https://raw.githubusercontent.com/OSOceanAcoustics/echopype/master/docs/source/_static/echopype_logo_banner.png" width="400">
 </div>
 
 # Echopype
 
 <div>
@@ -64,55 +38,99 @@
   </a>
 
   <a href="https://anaconda.org/conda-forge/echopype">
     <img src="https://img.shields.io/conda/vn/conda-forge/echopype.svg"/>
   </a>
 </div>
 
+[![ssec](https://img.shields.io/badge/SSEC-Project-purple?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA0AAAAOCAQAAABedl5ZAAAACXBIWXMAAAHKAAABygHMtnUxAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAMNJREFUGBltwcEqwwEcAOAfc1F2sNsOTqSlNUopSv5jW1YzHHYY/6YtLa1Jy4mbl3Bz8QIeyKM4fMaUxr4vZnEpjWnmLMSYCysxTcddhF25+EvJia5hhCudULAePyRalvUteXIfBgYxJufRuaKuprKsbDjVUrUj40FNQ11PTzEmrCmrevPhRcVQai8m1PRVvOPZgX2JttWYsGhD3atbHWcyUqX4oqDtJkJiJHUYv+R1JbaNHJmP/+Q1HLu2GbNoSm3Ft0+Y1YMdPSTSwQAAAABJRU5ErkJggg==&style=plastic)](https://escience.washington.edu/echopype/)
+
 Echopype is a package built to enable interoperability and scalability in ocean sonar data processing. These data are widely used for obtaining information about the distribution and abundance of marine animals, such as fish and krill. Our ability to collect large volumes of sonar data from a variety of ocean platforms has grown significantly in the last decade. However, most of the new data remain under-utilized. echopype aims to address the root cause of this problem - the lack of interoperable data format and scalable analysis workflows that adapt well with increasing data volume - by providing open-source tools as entry points for scientists to make discovery using these new data.
 
 Watch the [echopype talk](https://www.youtube.com/watch?v=qboH7MyHrpU)
 at SciPy 2019 for background, discussions and a quick demo!
 
+
 ## Documentation
 
 Learn more about echopype in the official documentation at https://echopype.readthedocs.io. Check out executable examples in the companion repository https://github.com/OSOceanAcoustics/echopype-examples.
 
 
 ## Contributing
 
 You can find information about how to contribute to echopype at our [Contributing Page](https://echopype.readthedocs.io/en/latest/contributing.html).
 
+## <img src="docs/source/images/GSoC-logo-horizontal.svg" alt="Google Summer of Code logo" width="300" style="padding-right: 50px; vertical-align: middle">
+
+In collaboration with the [Integrated Ocean Observing System (IOOS)](https://ioos.noaa.gov/), the Echopype team aims to recruit talented [Google Summer of Code (GSoC)](https://summerofcode.withgoogle.com/)
+participants to help us upgrade the robustness and scalability of the Echopype package.
+
+If you are a GSoC 2024 contributor, please head over to [GSoC contributor's guide](gsoc_contrib_guide.md) to get more information specific to the program.
+
+
 
 ## Echopype doesn't run on your data?
 
 Please report any bugs by [creating issues on GitHub](https://medium.com/nyc-planning-digital/writing-a-proper-github-issue-97427d62a20f).
 
 [Pull requests](https://jarednielsen.com/learn-git-fork-pull-request/) are always welcome!
 
 
-Contributors
-------------
+## Contributors
 
 [![Contributors](https://contrib.rocks/image?repo=OSOceanAcoustics/echopype)](https://github.com/OSOceanAcoustics/echopype/graphs/contributors)
 
-Wu-Jung Lee ([@leewujung](https://github.com/leewujung)) founded the echopype project in 2018. It is currently led by Wu-Jung Lee and Emilio Mayorga ([@emiliom](https://github.com/emiliom)), who are primary developers together with Landung "Don" Setiawan ([@lsetiawan](https://github.com/lsetiawan)), and previously Brandon Reyes ([@b-reyes](https://github.com/b-reyes)), Kavin Nguyen ([@ngkavin](https://github.com/ngkavin)) and Imran Majeed ([@imranmaj](https://github.com/imranmaj)). Valentina Staneva ([@valentina-s](https://github.com/valentina-s)) is also part of the development team.
+Wu-Jung Lee ([@leewujung](https://github.com/leewujung))
+founded the echopype project in 2018 and continue to be the primary contributor
+together with Praneeth Ratna([@praneethratna](https://github.com/praneethratna)).
+Emilio Mayorga ([@emiliom](https://github.com/emiliom)),
+Landung "Don" Setiawan ([@lsetiawan](https://github.com/lsetiawan)),
+Brandon Reyes ([@b-reyes](https://github.com/b-reyes)),
+Kavin Nguyen ([@ngkavin](https://github.com/ngkavin))
+and Imran Majeed ([@imranmaj](https://github.com/imranmaj))
+have contributed significantly to the code.
+Valentina Staneva ([@valentina-s](https://github.com/valentina-s)) is also part of the development team.
+
+A complete list of direct contributors is on our [GitHub Contributors Page](https://github.com/OSOceanAcoustics/echopype/graphs/contributors).
+
 
-Other contributors are listed in [echopype documentation](https://echopype.readthedocs.io).
+## Acknowledgement
 
 We thank Dave Billenness of ASL Environmental Sciences for
-providing the AZFP Matlab Toolbox as reference for our
-development of AZFP support in echopype.
-We also thank Rick Towler ([@rhtowler](https://github.com/rhtowler))
+providing the AZFP Matlab Toolbox as reference for developing
+support for the AZFP echosounder,
+and Rick Towler ([@rhtowler](https://github.com/rhtowler))
 of the NOAA Alaska Fisheries Science Center
 for providing low-level file parsing routines for
 Simrad EK60 and EK80 echosounders.
 
+We also thank funding support from
+the National Science Foundation and NOAA Ocean Exploration,
+and software engineering support from
+the University of Washington Scientific Software Engineering Center (SSEC),
+as part of the Schmidt Futures Virtual Institute for Scientific Software (VISS) in 2023.
+
+<div>
+  <a href="https://oceanexplorer.noaa.gov/news/oer-updates/2021/fy21-ffo-schedule.html">
+    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/79/NOAA_logo.svg/936px-NOAA_logo.svg.png" alt="NOAA_logo" width="120">
+  </a>
+
+  <a href="https://www.nsf.gov/awardsearch/showAward?AWD_ID=1849930&HistoricalAwards=false">
+    <img src="https://upload.wikimedia.org/wikipedia/commons/7/7e/NSF_logo.png" alt="NSF_logo" width="120">
+  </a>
+
+  <a href="https://escience.washington.edu/software-engineering/ssec/">
+    <img src="https://avatars.githubusercontent.com/u/122321194?s=200&v=4" alt="SSEC_logo" width="120">
+  </a>
+</div>
+
+
+
+
+
 ## License
 
 Echopype is licensed under the open source [Apache 2.0 license](https://opensource.org/licenses/Apache-2.0).
 
 ---------------
 
-Copyright (c) 2018-2023, Echopype Developers.
-
-
+Copyright (c) 2018-2024, Echopype Developers.
```

#### html2text {}

```diff
@@ -1,62 +1,67 @@
-Metadata-Version: 2.1 Name: echopype Version: 0.8.3 Summary: Enhancing the
-interoperability and scalability in analyzing ocean sonar data Home-page:
-https://github.com/OSOceanAcoustics/echopype Author: Wu-Jung Lee Author-email:
-leewujung@gmail.com Maintainer: Wu-Jung Lee Maintainer-email:
-leewujung@gmail.com License: Apache License, Version 2.0 Platform: OS
-Independent Classifier: Development Status :: 4 - Beta Classifier: Environment
-:: Console Classifier: Intended Audience :: Science/Research Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Topic :: Scientific/Engineering Requires-Python: >=3.9 Description-Content-
-Type: text/markdown Provides-Extra: plot License-File: LICENSE
    [https://raw.githubusercontent.com/OSOceanAcoustics/echopype/master/docs/
                    source/_static/echopype_logo_banner.png]
 # Echopype
 _[_D_O_I_]_[_G_i_t_H_u_b_ _L_i_c_e_n_s_e_]
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_O_S_O_c_e_a_n_A_c_o_u_s_t_i_c_s_/_e_c_h_o_p_y_p_e_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_b_u_i_l_d_._y_a_m_l_/
 _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_e_s_u_l_t_s_._p_r_e_-_c_o_m_m_i_t_._c_i_/_b_a_d_g_e_/_g_i_t_h_u_b_/_O_S_O_c_e_a_n_A_c_o_u_s_t_i_c_s_/
 _e_c_h_o_p_y_p_e_/_m_a_s_t_e_r_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_e_c_h_o_p_y_p_e_/_b_a_d_g_e_/
 _?_v_e_r_s_i_o_n_=_l_a_t_e_s_t_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_O_S_O_c_e_a_n_A_c_o_u_s_t_i_c_s_/_e_c_h_o_p_y_p_e_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/
 _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_G_T_9_8_F_9_1_9_X_R_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_e_c_h_o_p_y_p_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_n_d_a_/_v_n_/
 _c_o_n_d_a_-_f_o_r_g_e_/_e_c_h_o_p_y_p_e_._s_v_g_]
-Echopype is a package built to enable interoperability and scalability in ocean
-sonar data processing. These data are widely used for obtaining information
-about the distribution and abundance of marine animals, such as fish and krill.
-Our ability to collect large volumes of sonar data from a variety of ocean
-platforms has grown significantly in the last decade. However, most of the new
-data remain under-utilized. echopype aims to address the root cause of this
-problem - the lack of interoperable data format and scalable analysis workflows
-that adapt well with increasing data volume - by providing open-source tools as
-entry points for scientists to make discovery using these new data. Watch the
-[echopype talk](https://www.youtube.com/watch?v=qboH7MyHrpU) at SciPy 2019 for
-background, discussions and a quick demo! ## Documentation Learn more about
-echopype in the official documentation at https://echopype.readthedocs.io.
-Check out executable examples in the companion repository https://github.com/
-OSOceanAcoustics/echopype-examples. ## Contributing You can find information
-about how to contribute to echopype at our [Contributing Page](https://
-echopype.readthedocs.io/en/latest/contributing.html). ## Echopype doesn't run
-on your data? Please report any bugs by [creating issues on GitHub](https://
-medium.com/nyc-planning-digital/writing-a-proper-github-issue-97427d62a20f).
-[Pull requests](https://jarednielsen.com/learn-git-fork-pull-request/) are
-always welcome! Contributors ------------ [![Contributors](https://
-contrib.rocks/image?repo=OSOceanAcoustics/echopype)](https://github.com/
-OSOceanAcoustics/echopype/graphs/contributors) Wu-Jung Lee ([@leewujung](https:
-//github.com/leewujung)) founded the echopype project in 2018. It is currently
-led by Wu-Jung Lee and Emilio Mayorga ([@emiliom](https://github.com/emiliom)),
-who are primary developers together with Landung "Don" Setiawan ([@lsetiawan]
-(https://github.com/lsetiawan)), and previously Brandon Reyes ([@b-reyes]
-(https://github.com/b-reyes)), Kavin Nguyen ([@ngkavin](https://github.com/
-ngkavin)) and Imran Majeed ([@imranmaj](https://github.com/imranmaj)).
-Valentina Staneva ([@valentina-s](https://github.com/valentina-s)) is also part
-of the development team. Other contributors are listed in [echopype
-documentation](https://echopype.readthedocs.io). We thank Dave Billenness of
-ASL Environmental Sciences for providing the AZFP Matlab Toolbox as reference
-for our development of AZFP support in echopype. We also thank Rick Towler (
-[@rhtowler](https://github.com/rhtowler)) of the NOAA Alaska Fisheries Science
-Center for providing low-level file parsing routines for Simrad EK60 and EK80
-echosounders. ## License Echopype is licensed under the open source [Apache 2.0
-license](https://opensource.org/licenses/Apache-2.0). --------------- Copyright
-(c) 2018-2023, Echopype Developers.
+[![ssec](https://img.shields.io/badge/SSEC-Project-purple?logo=data:image/
+png;base64,iVBORw0KGgoAAAANSUhEUgAAAA0AAAAOCAQAAABedl5ZAAAACXBIWXMAAAHKAAABygHMtnUxAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAMNJREFUGBltwcEqwwEcAOAfc1F2sNsOTqSlNUopSv5jW1YzHHYY/
+6YtLa1Jy4mbl3Bz8QIeyKM4fMaUxr4vZnEpjWnmLMSYCysxTcddhF25+EvJia5hhCudULAePyRalvUteXIfBgYxJufRuaKuprKsbDjVUrUj40FNQ11PTzEmrCmrevPhRcVQai8m1PRVvOPZgX2JttWYsGhD3atbHWcyUqX4oqDtJkJiJHUYv+R1JbaNHJmP/
++Q1HLu2GbNoSm3Ft0+Y1YMdPSTSwQAAAABJRU5ErkJggg==&style=plastic)](https://
+escience.washington.edu/echopype/) Echopype is a package built to enable
+interoperability and scalability in ocean sonar data processing. These data are
+widely used for obtaining information about the distribution and abundance of
+marine animals, such as fish and krill. Our ability to collect large volumes of
+sonar data from a variety of ocean platforms has grown significantly in the
+last decade. However, most of the new data remain under-utilized. echopype aims
+to address the root cause of this problem - the lack of interoperable data
+format and scalable analysis workflows that adapt well with increasing data
+volume - by providing open-source tools as entry points for scientists to make
+discovery using these new data. Watch the [echopype talk](https://
+www.youtube.com/watch?v=qboH7MyHrpU) at SciPy 2019 for background, discussions
+and a quick demo! ## Documentation Learn more about echopype in the official
+documentation at https://echopype.readthedocs.io. Check out executable examples
+in the companion repository https://github.com/OSOceanAcoustics/echopype-
+examples. ## Contributing You can find information about how to contribute to
+echopype at our [Contributing Page](https://echopype.readthedocs.io/en/latest/
+contributing.html). ## [Google Summer of Code logo]In collaboration with the
+[Integrated Ocean Observing System (IOOS)](https://ioos.noaa.gov/), the
+Echopype team aims to recruit talented [Google Summer of Code (GSoC)](https://
+summerofcode.withgoogle.com/) participants to help us upgrade the robustness
+and scalability of the Echopype package. If you are a GSoC 2024 contributor,
+please head over to [GSoC contributor's guide](gsoc_contrib_guide.md) to get
+more information specific to the program. ## Echopype doesn't run on your data?
+Please report any bugs by [creating issues on GitHub](https://medium.com/nyc-
+planning-digital/writing-a-proper-github-issue-97427d62a20f). [Pull requests]
+(https://jarednielsen.com/learn-git-fork-pull-request/) are always welcome! ##
+Contributors [![Contributors](https://contrib.rocks/
+image?repo=OSOceanAcoustics/echopype)](https://github.com/OSOceanAcoustics/
+echopype/graphs/contributors) Wu-Jung Lee ([@leewujung](https://github.com/
+leewujung)) founded the echopype project in 2018 and continue to be the primary
+contributor together with Praneeth Ratna([@praneethratna](https://github.com/
+praneethratna)). Emilio Mayorga ([@emiliom](https://github.com/emiliom)),
+Landung "Don" Setiawan ([@lsetiawan](https://github.com/lsetiawan)), Brandon
+Reyes ([@b-reyes](https://github.com/b-reyes)), Kavin Nguyen ([@ngkavin](https:
+//github.com/ngkavin)) and Imran Majeed ([@imranmaj](https://github.com/
+imranmaj)) have contributed significantly to the code. Valentina Staneva (
+[@valentina-s](https://github.com/valentina-s)) is also part of the development
+team. A complete list of direct contributors is on our [GitHub Contributors
+Page](https://github.com/OSOceanAcoustics/echopype/graphs/contributors). ##
+Acknowledgement We thank Dave Billenness of ASL Environmental Sciences for
+providing the AZFP Matlab Toolbox as reference for developing support for the
+AZFP echosounder, and Rick Towler ([@rhtowler](https://github.com/rhtowler)) of
+the NOAA Alaska Fisheries Science Center for providing low-level file parsing
+routines for Simrad EK60 and EK80 echosounders. We also thank funding support
+from the National Science Foundation and NOAA Ocean Exploration, and software
+engineering support from the University of Washington Scientific Software
+Engineering Center (SSEC), as part of the Schmidt Futures Virtual Institute for
+Scientific Software (VISS) in 2023.
+_[_N_O_A_A___l_o_g_o_]_[_N_S_F___l_o_g_o_]_[_S_S_E_C___l_o_g_o_]
+## License Echopype is licensed under the open source [Apache 2.0 license]
+(https://opensource.org/licenses/Apache-2.0). --------------- Copyright (c)
+2018-2024, Echopype Developers.
```

### Comparing `echopype-0.8.3/echopype/__init__.py` & `echopype-0.8.4/echopype/__init__.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/calibrate/api.py` & `echopype-0.8.4/echopype/calibrate/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/calibrate/cal_params.py` & `echopype-0.8.4/echopype/calibrate/cal_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,32 +282,32 @@
         raise ValueError(f"Unknown parameter {param}")
 
     # Check parameter exists
     if param not in vend:
         raise ValueError(f"{param} does not exist in the Vendor_specific group!")
 
     # Find idx to select the corresponding param value
-    # by matching beam["transmit_duration_nominal"] with ds_vend["pulse_length"]
+    # by matching beam["transmit_duration_nominal"] with vend["pulse_length"]
     transmit_isnull = beam["transmit_duration_nominal"].isnull()
     idxmin = np.abs(beam["transmit_duration_nominal"] - vend["pulse_length"]).idxmin(
         dim="pulse_length_bin"
     )
 
     # fill nan position with 0 (will remove before return)
     # and convert to int for indexing
     idxmin = idxmin.where(~transmit_isnull, 0).astype(int)
 
     # Get param dataarray into correct shape
-    da_param = (
-        vend[param]
-        .expand_dims(dim={"ping_time": idxmin["ping_time"]})  # expand dims for direct indexing
-        .sortby(idxmin.channel)  # sortby in case channel sequence differs in vend and beam
-    )
+    da_param = vend[param].transpose("pulse_length_bin", "channel")
+
+    if not np.array_equal(da_param.channel.data, idxmin.channel.data):
+        da_param = da_param.sortby(
+            da_param.channel, ascending=False
+        )  # sortby because channel sequence differs in vend and beam
 
-    # Select corresponding index and clean up the original nan elements
     da_param = da_param.sel(pulse_length_bin=idxmin, drop=True)
 
     # Set the nan elements back to nan.
     # Doing the `.where` will result in float64,
     # which is fine since we're dealing with nan
     da_param = da_param.where(~transmit_isnull, np.nan)
 
@@ -496,17 +496,17 @@
                         # scaled according to frequency ratio
                         out_dict[p] = beam[p] + 20 * np.log10(
                             beam["frequency_nominal"] / freq_center
                         )
                     elif p == "gain_correction":
                         # interpolate or pull from narrowband table
                         out_dict[p] = _get_interp_da(
-                            da_param=None
-                            if "gain" not in vend
-                            else vend["gain"],  # freq-dep values
+                            da_param=(
+                                None if "gain" not in vend else vend["gain"]
+                            ),  # freq-dep values
                             freq_center=freq_center,
                             alternative=get_vend_cal_params_power(beam=beam, vend=vend, param=p),
                         )
                     elif p == "impedance_transducer":
                         out_dict[p] = _get_interp_da(
                             da_param=None if p not in vend else vend[p],
                             freq_center=freq_center,
```

### Comparing `echopype-0.8.3/echopype/calibrate/calibrate_azfp.py` & `echopype-0.8.4/echopype/calibrate/calibrate_azfp.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/calibrate/calibrate_base.py` & `echopype-0.8.4/echopype/calibrate/calibrate_base.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/calibrate/calibrate_ek.py` & `echopype-0.8.4/echopype/calibrate/calibrate_ek.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,14 +469,18 @@
         ) ** 2
         fac_athwart = (
             np.abs(-self.cal_params["angle_offset_athwartship"])
             / (self.cal_params["beamwidth_athwartship"] / 2)
         ) ** 2
         B_theta_phi_m = 0.5 * 6.0206 * (fac_along + fac_athwart - 0.18 * fac_along * fac_athwart)
 
+        # Zero out NaNs that appear due to 1) multiplex ping patterns and 2) single beam transducer
+        # systems that don't contain angle offset information.
+        B_theta_phi_m = B_theta_phi_m.fillna(0)
+
         return B_theta_phi_m
 
     def _cal_complex_samples(self, cal_type: str) -> xr.Dataset:
         """Calibrate complex data from EK80.
 
         Parameters
         ----------
```

### Comparing `echopype-0.8.3/echopype/calibrate/ecs.py` & `echopype-0.8.4/echopype/calibrate/ecs.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/calibrate/ek80_complex.py` & `echopype-0.8.4/echopype/calibrate/ek80_complex.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,38 +222,39 @@
         Timestamp for the transmit replica
     """
     # Make sure it is BB mode data
     # This is already checked in calibrate_ek
     # but keeping this here for use as standalone function
     if waveform_mode == "BB" and np.all(beam["transmit_type"] == "CW"):
         raise TypeError("File does not contain BB mode complex samples!")
-
     # Generate all transmit replica
     y_all = {}
     y_time_all = {}
-    # TODO: expand to deal with the case with varying tx param across ping_time
+    # TODO: expand to deal with the case with varying non-NaN tx param across ping_time
     tx_param_names = [
         "transmit_duration_nominal",
         "slope",
         "transmit_frequency_start",
         "transmit_frequency_stop",
     ]
     for ch in beam["channel"].values:
         tx_params = {}
         for p in tx_param_names:
-            tx_params[p] = np.unique(beam[p].sel(channel=ch))
+            # Extract beam values and filter out NaNs
+            beam_values = np.unique(beam[p].sel(channel=ch))
+            # Filter out NaN values
+            beam_values_without_nan = beam_values[~np.isnan(beam_values)]
+            tx_params[p] = beam_values_without_nan
             if tx_params[p].size != 1:
                 raise TypeError("File contains changing %s!" % p)
         fs_chan = fs.sel(channel=ch).data if isinstance(fs, xr.DataArray) else fs
         tx_params["fs"] = fs_chan
         y_ch, _ = tapered_chirp(**tx_params)
-
         # Filter and decimate chirp template
         y_ch, y_tmp_time = filter_decimate_chirp(coeff_ch=coeff[ch], y_ch=y_ch, fs=fs_chan)
-
         # Fill into output dict
         y_all[ch] = y_ch
         y_time_all[ch] = y_tmp_time
 
     return y_all, y_time_all
 
 
@@ -269,42 +270,52 @@
 
     Returns
     -------
     xr.DataArray
         A data array containing pulse compression output.
     """
     pc_all = []
+
     for chan in backscatter["channel"]:
+        # Select channel `chan` and drop the specific beam dimension if all of the values are nan.
         backscatter_chan = backscatter.sel(channel=chan).dropna(dim="beam", how="all")
 
+        # Create NaN mask
+        # If `backscatter_chan` is lazy loaded, then `nan_mask` too will be lazy loaded.
+        nan_mask = np.isnan(backscatter_chan)
+
+        # Zero out backscatter NaN values
+        # If `nan_mask` is lazy loaded, then resulting `backscatter_chan` will be lazy loaded.
+        backscatter_chan = xr.where(nan_mask, 0.0 + 0j, backscatter_chan)
+
+        # Extract transmit values
         tx = chirp[str(chan.values)]
+
+        # Compute complex conjugate of transmit values and reverse order of elements
         replica = np.flipud(np.conj(tx))
+
+        # Apply convolve on backscatter (along range sample dimension) and replica
         pc = xr.apply_ufunc(
-            lambda m: np.apply_along_axis(
-                lambda m: (signal.convolve(m, replica, mode="full")[tx.size - 1 :]),
-                axis=2,
-                arr=m,
-            ),
+            lambda m: (signal.convolve(m, replica, mode="full")[replica.size - 1 :]),
             backscatter_chan,
             input_core_dims=[["range_sample"]],
             output_core_dims=[["range_sample"]],
-            # exclude_dims={"range_sample"},
-        )
+            dask="parallelized",
+            vectorize=True,
+            output_dtypes=[np.complex64],
+        ).compute()
+
+        # Restore NaN values in the resulting array.
+        # Computing of `nan_mask` here is necessary in the case when `nan_mask` is lazy loaded
+        # or else the resulting `pc` will also be lazy loaded.
+        pc = xr.where(nan_mask.compute(), np.nan, pc)
 
         pc_all.append(pc)
 
-    pc_all = xr.DataArray(
-        pc_all,
-        coords={
-            "channel": backscatter["channel"],
-            "ping_time": backscatter["ping_time"],
-            "beam": backscatter["beam"],
-            "range_sample": backscatter["range_sample"],
-        },
-    )
+    pc_all = xr.concat(pc_all, dim="channel")
 
     return pc_all
 
 
 def get_norm_fac(chirp: Dict) -> xr.DataArray:
     """
     Get normalization factor from the chirp dictionary.
```

### Comparing `echopype-0.8.3/echopype/calibrate/env_params.py` & `echopype-0.8.4/echopype/calibrate/env_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,31 +45,35 @@
     Returns
     -------
     Environment parameter with correctly broadcasted timestamps
     """
     if isinstance(p, xr.DataArray):
         if "time1" not in p.coords:
             return p
-        else:
-            # If there's only 1 time1 value,
-            # or if after dropping NaN there's only 1 time1 value
-            if p["time1"].size == 1 or p.dropna(dim="time1").size == 1:
-                return p.dropna(dim="time1").squeeze(dim="time1").drop("time1")
-
-            # Direct assignment if all timestamps are identical (EK60 data)
-            elif np.all(p["time1"].values == ping_time.values):
-                return p.rename({"time1": "ping_time"})
-
-            elif ping_time is None:
-                raise ValueError(f"ping_time needs to be provided for interpolating {p.name}")
-
-            else:
-                return p.dropna(dim="time1").interp(time1=ping_time)
-    else:
-        return p
+
+        # If there's only 1 time1 value:
+        if p["time1"].size == 1:
+            return p.squeeze(dim="time1").drop_vars("time1")
+
+        # If after dropping NaN along time1 dimension there's only 1 time1 value:
+        if p.dropna(dim="time1").size == 1:
+            return p.dropna(dim="time1").squeeze(dim="time1").drop_vars("time1")
+
+        if ping_time is None:
+            raise ValueError(
+                f"ping_time needs to be provided for comparison or interpolating {p.name}"
+            )
+
+        # Direct assignment if all timestamps are identical (EK60 data)
+        if np.array_equal(p["time1"].data, ping_time.data):
+            return p.rename({"time1": "ping_time"})
+
+        # Interpolate `p` to `ping_time`
+        return p.dropna(dim="time1").interp(time1=ping_time)
+    return p
 
 
 def sanitize_user_env_dict(
     user_dict: Dict[str, Union[int, float, List, xr.DataArray]],
     channel: Union[List, xr.DataArray],
 ) -> Dict[str, Union[int, float, xr.DataArray]]:
     """
```

### Comparing `echopype-0.8.3/echopype/calibrate/env_params_old.py` & `echopype-0.8.4/echopype/calibrate/env_params_old.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/calibrate/range.py` & `echopype-0.8.4/echopype/calibrate/range.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/clean/api.py` & `echopype-0.8.4/echopype/clean/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/clean/noise_est.py` & `echopype-0.8.4/echopype/clean/noise_est.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/commongrid/api.py` & `echopype-0.8.4/echopype/commongrid/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functions for enhancing the spatial and temporal coherence of data.
 """
+
 import logging
 from typing import Literal
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
@@ -26,16 +27,17 @@
 
 
 @add_processing_level("L3*")
 def compute_MVBS(
     ds_Sv: xr.Dataset,
     range_var: Literal["echo_range", "depth"] = "echo_range",
     range_bin: str = "20m",
-    ping_time_bin: str = "20S",
+    ping_time_bin: str = "20s",
     method="map-reduce",
+    skipna=True,
     closed: Literal["left", "right"] = "left",
     **flox_kwargs,
 ):
     """
     Compute Mean Volume Backscattering Strength (MVBS)
     based on intervals of range (``echo_range``) or depth (``depth``)
     and ``ping_time`` specified in physical units.
@@ -51,20 +53,23 @@
     range_var: {'echo_range', 'depth'}, default 'echo_range'
         The variable to use for range binning.
         Must be one of ``echo_range`` or ``depth``.
         Note that ``depth`` is only available if the input dataset contains
         ``depth`` as a data variable.
     range_bin : str, default '20m'
         bin size along ``echo_range`` or ``depth`` in meters.
-    ping_time_bin : str, default '20S'
+    ping_time_bin : str, default '20s'
         bin size along ``ping_time``
     method: str, default 'map-reduce'
         The flox strategy for reduction of dask arrays only.
         See flox `documentation <https://flox.readthedocs.io/en/latest/implementation.html>`_
         for more details.
+    skipna: bool, default True
+        If true, the mean operation skips NaN values.
+        Else, the mean operation includes NaN values.
     closed: {'left', 'right'}, default 'left'
         Which side of bin interval is closed.
     **flox_kwargs
         Additional keyword arguments to be passed
         to flox reduction function.
 
     Returns
@@ -100,14 +105,15 @@
     range_interval = _convert_bins_to_interval_index(range_interval, closed=closed)
     raw_MVBS = compute_raw_MVBS(
         ds_Sv,
         range_interval,
         ping_interval,
         range_var=range_var,
         method=method,
+        skipna=skipna,
         **flox_kwargs,
     )
 
     # create MVBS dataset
     # by transforming the binned dimensions to regular coords
     ds_MVBS = xr.Dataset(
         data_vars={"Sv": (["channel", "ping_time", range_var], raw_MVBS["Sv"].data)},
@@ -263,14 +269,15 @@
 
 @add_processing_level("L4")
 def compute_NASC(
     ds_Sv: xr.Dataset,
     range_bin: str = "10m",
     dist_bin: str = "0.5nmi",
     method: str = "map-reduce",
+    skipna=True,
     closed: Literal["left", "right"] = "left",
     **flox_kwargs,
 ) -> xr.Dataset:
     """
     Compute Nautical Areal Scattering Coefficient (NASC) from an Sv dataset.
 
     Parameters
@@ -282,14 +289,17 @@
         bin size along ``depth`` in meters (m).
     dist_bin : str, default '0.5nmi'
         bin size along ``distance`` in nautical miles (nmi).
     method: str, default 'map-reduce'
         The flox strategy for reduction of dask arrays only.
         See flox `documentation <https://flox.readthedocs.io/en/latest/implementation.html>`_
         for more details.
+    skipna: bool, default True
+        If true, the mean operation skips NaN values.
+        Else, the mean operation includes NaN values.
     closed: {'left', 'right'}, default 'left'
         Which side of bin interval is closed.
     **flox_kwargs
         Additional keyword arguments to be passed
         to flox reduction function.
 
     Returns
@@ -352,14 +362,15 @@
     range_interval = _convert_bins_to_interval_index(range_interval, closed=closed)
 
     raw_NASC = compute_raw_NASC(
         ds_Sv,
         range_interval,
         dist_interval,
         method=method,
+        skipna=skipna,
         **flox_kwargs,
     )
 
     # create MVBS dataset
     # by transforming the binned dimensions to regular coords
     ds_NASC = xr.Dataset(
         data_vars={"NASC": (["channel", "distance", range_var], raw_NASC["sv"].data)},
```

### Comparing `echopype-0.8.3/echopype/commongrid/utils.py` & `echopype-0.8.4/echopype/commongrid/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 def compute_raw_MVBS(
     ds_Sv: xr.Dataset,
     range_interval: Union[pd.IntervalIndex, np.ndarray],
     ping_interval: Union[pd.IntervalIndex, np.ndarray],
     range_var: Literal["echo_range", "depth"] = "echo_range",
     method="map-reduce",
+    skipna=True,
     **flox_kwargs,
 ):
     """
     Compute the raw unformatted MVBS of ``ds_Sv``.
 
     Parameters
     ----------
@@ -41,14 +42,17 @@
     range_var: {'echo_range', 'depth'}, default 'echo_range'
         The variable to use for range binning.
         Either ``echo_range`` or ``depth``.
     method: str
         The flox strategy for reduction of dask arrays only.
         See flox `documentation <https://flox.readthedocs.io/en/latest/implementation.html>`_
         for more details.
+    skipna: bool, default True
+        If true, the mean operation skips NaN values.
+        Else, the mean operation includes NaN values.
     **flox_kwargs
         Additional keyword arguments to be passed
         to flox reduction function.
 
     Returns
     -------
     xr.Dataset
@@ -61,14 +65,16 @@
     sv_mean = _groupby_x_along_channels(
         ds_Sv,
         range_interval,
         x_interval=ping_interval,
         x_var=x_var,
         range_var=range_var,
         method=method,
+        func="nanmean" if skipna else "mean",
+        skipna=skipna,
         **flox_kwargs,
     )
 
     # This is MVBS computation
     # apply inverse mapping to get back to the original domain and store values
     da_MVBS = sv_mean.pipe(_lin2log)
     # return xr.merge([ds_Pos, da_MVBS])
@@ -76,14 +82,15 @@
 
 
 def compute_raw_NASC(
     ds_Sv: xr.Dataset,
     range_interval: Union[pd.IntervalIndex, np.ndarray],
     dist_interval: Union[pd.IntervalIndex, np.ndarray],
     method="map-reduce",
+    skipna=True,
     **flox_kwargs,
 ):
     """
     Compute the raw unformatted NASC of ``ds_Sv``.
 
     Parameters
     ----------
@@ -96,14 +103,17 @@
     dist_interval : pd.IntervalIndex or np.ndarray
         1D array or interval index representing
         the bins required for ``distance_nmi``.
     method: str
         The flox strategy for reduction of dask arrays only.
         See flox `documentation <https://flox.readthedocs.io/en/latest/implementation.html>`_
         for more details.
+    skipna: bool, default True
+        If true, the mean operation skips NaN values.
+        Else, the mean operation includes NaN values.
     **flox_kwargs
         Additional keyword arguments to be passed
         to flox reduction function.
 
     Returns
     -------
     xr.Dataset
@@ -122,24 +132,27 @@
     sv_mean = _groupby_x_along_channels(
         ds_Sv,
         range_interval,
         x_interval=dist_interval,
         x_var=x_var,
         range_var=range_var,
         method=method,
+        func="nanmean" if skipna else "mean",
+        skipna=skipna,
         **flox_kwargs,
     )
 
     # Get mean ping_time along distance_nmi
     # this is only done for NASC computation,
     # since for MVBS the ping_time is used for binning already.
     ds_ping_time = xarray_reduce(
         ds_Sv["ping_time"],
         ds_Sv[x_var],
         func="nanmean",
+        skipna=True,
         expected_groups=(dist_interval),
         isbin=True,
         method=method,
     )
 
     # Mean height: approach to use flox
     # Numerator (h_mean_num):
@@ -150,26 +163,28 @@
     #   - create a datararray filled with 1, with 1D coordinate (distance)
     #   - flox xarray_reduce along distance, summing over each 1D bin
     # h_mean = N/D
     da_denom = xr.ones_like(ds_Sv[x_var])
     h_mean_denom = xarray_reduce(
         da_denom,
         ds_Sv[x_var],
-        func="sum",
+        func="nansum",
+        skipna=True,
         expected_groups=(dist_interval),
         isbin=[True],
         method=method,
     )
 
     h_mean_num = xarray_reduce(
         ds_Sv[range_var].diff(dim=range_dim, label="lower"),  # use lower end label after diff
         ds_Sv["channel"],
         ds_Sv[x_var],
         ds_Sv[range_var].isel(**{range_dim: slice(0, -1)}),
-        func="sum",
+        func="nansum",
+        skipna=True,
         expected_groups=(None, dist_interval, range_interval),
         isbin=[False, True, True],
         method=method,
     )
     h_mean = h_mean_num / h_mean_denom
 
     # Combine to compute NASC and name it
@@ -476,14 +491,16 @@
 def _groupby_x_along_channels(
     ds_Sv: xr.Dataset,
     range_interval: Union[pd.IntervalIndex, np.ndarray],
     x_interval: Union[pd.IntervalIndex, np.ndarray],
     x_var: Literal["ping_time", "distance_nmi"] = "ping_time",
     range_var: Literal["echo_range", "depth"] = "echo_range",
     method: str = "map-reduce",
+    func: str = "nanmean",
+    skipna: bool = True,
     **flox_kwargs,
 ) -> xr.Dataset:
     """
     Perform groupby of ``ds_Sv`` along each channel for the given
     intervals to get the 'sv' mean value.
 
     Parameters
@@ -513,14 +530,23 @@
         Either ``echo_range`` or ``depth``.
 
         **For NASC, this must be ``depth``.**
     method: str
         The flox strategy for reduction of dask arrays only.
         See flox `documentation <https://flox.readthedocs.io/en/latest/implementation.html>`_
         for more details.
+    func: str, default 'nanmean'
+        The aggregation function used for reducing the data array.
+        By default, 'nanmean' is used. Other options can be found in the flox `documentation
+        <https://flox.readthedocs.io/en/latest/generated/flox.xarray.xarray_reduce.html>`_.
+    skipna: bool, default True
+        If true, aggregation function skips NaN values.
+        Else, aggregation function includes NaN values.
+        Note that if ``func`` is set to 'mean' and ``skipna`` is set to True, then aggregation
+        will have the same behavior as if func is set to 'nanmean'.
     **flox_kwargs
         Additional keyword arguments to be passed
         to flox reduction function.
 
     Returns
     -------
     xr.Dataset
@@ -536,22 +562,39 @@
     if x_var == "distance_nmi" and range_var != "depth":
         logger.warning("x_var is 'distance_nmi', setting range_var to 'depth'")
         range_var = "depth"
 
     # average should be done in linear domain
     sv = ds_Sv["Sv"].pipe(_log2lin)
 
+    # Check for any NaNs in the coordinate arrays:
+    named_arrays = {
+        x_var: ds_Sv[x_var].data,
+        range_var: ds_Sv[range_var].data,
+    }
+    aggregation_msg = (
+        "Aggregation may be negatively impacted since Flox will not aggregate any "
+        "```Sv``` values that have corresponding NaN coordinate values. Consider handling "
+        "these values before calling your intended commongrid function."
+    )
+    for array_name, array in named_arrays.items():
+        if np.isnan(array).any():
+            logging.warning(
+                f"The ```{array_name}``` coordinate array contain NaNs. {aggregation_msg}"
+            )
+
     # reduce along ping_time or distance_nmi
     # and echo_range or depth
     # by binning and averaging
     sv_mean = xarray_reduce(
         sv,
         ds_Sv["channel"],
         ds_Sv[x_var],
         ds_Sv[range_var],
-        func="nanmean",
         expected_groups=(None, x_interval, range_interval),
         isbin=[False, True, True],
         method=method,
+        func=func,
+        skipna=skipna,
         **flox_kwargs,
     )
     return sv_mean
```

### Comparing `echopype-0.8.3/echopype/consolidate/api.py` & `echopype-0.8.4/echopype/consolidate/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 import numpy as np
 import xarray as xr
 
 from ..calibrate.ek80_complex import get_filter_coeff
 from ..echodata import EchoData
 from ..echodata.simrad import retrieve_correct_beam_group
 from ..utils.io import get_file_format, open_source
+from ..utils.log import _init_logger
 from ..utils.prov import add_processing_level
 from .split_beam_angle import get_angle_complex_samples, get_angle_power_samples
 
+logger = _init_logger(__name__)
+
 POSITION_VARIABLES = ["latitude", "longitude"]
 
 
 def swap_dims_channel_frequency(ds: Union[xr.Dataset, str, pathlib.Path]) -> xr.Dataset:
     """
     Use frequency_nominal in place of channel to be dataset dimension and coorindate.
 
@@ -187,18 +190,46 @@
 
     ds = open_source(ds, "dataset", {})
     echodata = open_source(echodata, "echodata", {})
 
     if "longitude" not in echodata["Platform"] or echodata["Platform"]["longitude"].isnull().all():
         raise ValueError("Coordinate variables not present or all nan")
 
+    # Check if any latitude/longitude value is NaN/0
+    contains_nan_lat_lon = (
+        np.isnan(echodata["Platform"]["latitude"].values).any()
+        or np.isnan(echodata["Platform"]["longitude"].values).any()
+    )
+    contains_zero_lat_lon = (echodata["Platform"]["latitude"].values == 0).any() or (
+        echodata["Platform"]["longitude"].values == 0
+    ).any()
+    interp_msg = (
+        "Interpolation may be negatively impacted, "
+        "consider handling these values before calling ``add_location``."
+    )
+    if contains_nan_lat_lon:
+        logger.warning(f"Latitude and/or longitude arrays contain NaNs. {interp_msg}")
+    if contains_zero_lat_lon:
+        logger.warning(f"Latitude and/or longitude arrays contain zeros. {interp_msg}")
+
     interp_ds = ds.copy()
     time_dim_name = list(echodata["Platform"]["longitude"].dims)[0]
+
+    # Check if there are duplicates in time_dim_name
+    if len(np.unique(echodata["Platform"][time_dim_name].data)) != len(
+        echodata["Platform"][time_dim_name].data
+    ):
+        raise ValueError(
+            f'The ``echodata["Platform"]["{time_dim_name}"]`` array contains duplicate values. '
+            "Downstream interpolation on the position variables requires unique time values."
+        )
+
     interp_ds["latitude"] = sel_interp("latitude", time_dim_name)
     interp_ds["longitude"] = sel_interp("longitude", time_dim_name)
+
     # Most attributes are attached automatically via interpolation
     # here we add the history
     history_attr = (
         f"{datetime.datetime.utcnow()} +00:00. "
         "Interpolated or propagated from Platform latitude/longitude."  # noqa
     )
     for da_name in POSITION_VARIABLES:
```

### Comparing `echopype-0.8.3/echopype/consolidate/split_beam_angle.py` & `echopype-0.8.4/echopype/consolidate/split_beam_angle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Contains functions necessary to compute the split-beam (alongship/athwartship)
 angles and add them to a Dataset.
 """
+
 from typing import List, Tuple
 
 import numpy as np
 import xarray as xr
 
 from ..calibrate.ek80_complex import compress_pulse, get_norm_fac, get_transmit_signal
```

### Comparing `echopype-0.8.3/echopype/convert/__init__.py` & `echopype-0.8.4/echopype/convert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 The current version supports:
 
 - Simrad EK60 echosounder ``.raw`` data
 - Simrad EK80 echosounder ``.raw`` data
 - ASL Environmental Sciences AZFP echosounder ``.01A`` data
 """
+
 # flake8: noqa
 from .parse_ad2cp import ParseAd2cp
 from .parse_azfp import ParseAZFP
 from .parse_base import ParseBase
 from .parse_ek60 import ParseEK60
 from .parse_ek80 import ParseEK80
 from .set_groups_ad2cp import SetGroupsAd2cp
```

### Comparing `echopype-0.8.3/echopype/convert/ad2cp_fields.yaml` & `echopype-0.8.4/echopype/convert/ad2cp_fields.yaml`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/convert/api.py` & `echopype-0.8.4/echopype/convert/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/convert/parse_ad2cp.py` & `echopype-0.8.4/echopype/convert/parse_ad2cp.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/convert/parse_azfp.py` & `echopype-0.8.4/echopype/convert/parse_azfp.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,52 @@
 
 from ..utils.log import _init_logger
 from ..utils.misc import camelcase2snakecase
 from .parse_base import ParseBase
 
 FILENAME_DATETIME_AZFP = "\\w+.01A"
 
+# Common Sv_offset values for frequency > 38 kHz
+SV_OFFSET_HF = {
+    300: 1.1,
+    500: 0.8,
+    700: 0.5,
+    900: 0.3,
+    1000: 0.3,
+}
+SV_OFFSET_LF = {
+    500: 1.1,
+    1000: 0.7,
+}
+SV_OFFSET = {
+    38000.0: {**SV_OFFSET_LF},
+    67000.0: {
+        500: 1.1,
+        **SV_OFFSET_HF,
+    },
+    125000.0: {
+        150: 1.4,
+        250: 1.3,
+        **SV_OFFSET_HF,
+    },
+    200000.0: {
+        150: 1.4,
+        250: 1.3,
+        **SV_OFFSET_HF,
+    },
+    455000.0: {
+        250: 1.3,
+        **SV_OFFSET_HF,
+    },
+    769000.0: {
+        150: 1.4,
+        **SV_OFFSET_HF,
+    },
+}
+
 HEADER_FIELDS = (
     ("profile_flag", "u2"),
     ("profile_number", "u2"),
     ("serial_number", "u2"),
     ("ping_status", "u2"),
     ("burst_int", "u4"),
     ("year", "u2"),  # Year
@@ -307,14 +345,30 @@
                 self.unpacked_data[key] = np.asarray(val)
 
         # cast all list parameter values to np array, so they are easier to reference
         for key, val in self.parameters.items():
             if isinstance(val, list):
                 self.parameters[key] = np.asarray(val)
 
+        # Get frequency values
+        freq_old = self.unpacked_data["frequency"]
+
+        # Obtain sorted frequency indices
+        self.freq_ind_sorted = freq_old.argsort()
+
+        # Obtain sorted frequencies
+        self.freq_sorted = freq_old[self.freq_ind_sorted] * 1000.0
+
+        # Build Sv offset
+        self.Sv_offset = np.zeros_like(self.freq_sorted)
+        for ind, ich in enumerate(self.freq_ind_sorted):
+            self.Sv_offset[ind] = self._calc_Sv_offset(
+                self.freq_sorted[ind], self.unpacked_data["pulse_len"][ich]
+            )
+
     def _print_status(self):
         """Prints message to console giving information about the raw file being parsed."""
         filename = os.path.basename(self.source_file)
         timestamp = dt(
             self.unpacked_data["year"][0],
             self.unpacked_data["month"][0],
             self.unpacked_data["day"][0],
@@ -476,26 +530,36 @@
                     ).replace(tzinfo=None),
                     "[ns]",
                 )
             )
         self.ping_time = ping_time
 
     @staticmethod
-    def _calc_Sv_offset(f, pulse_len):
-        """Calculate the compensation factor for Sv calculation."""
-        # TODO: this method seems should be in echopype.process
-        if f > 38000:
-            if pulse_len == 300:
-                return 1.1
-            elif pulse_len == 500:
-                return 0.8
-            elif pulse_len == 700:
-                return 0.5
-            elif pulse_len == 900:
-                return 0.3
-            elif pulse_len == 1000:
-                return 0.3
-        else:
-            if pulse_len == 500:
-                return 1.1
-            elif pulse_len == 1000:
-                return 0.7
+    def _calc_Sv_offset(freq, pulse_len):
+        """
+        Calculate the compensation factor for Sv calculation.
+
+        Parameters
+        ----------
+        freq : number
+            transmit frequency
+        pulse_len : number
+            pulse length
+        """
+        # Check if the specified freq is in the allowable Sv_offset dict
+        if freq not in SV_OFFSET.keys():
+            raise ValueError(
+                f"Frequency {freq} Hz is not in the Sv offset dictionary! "
+                "Please contact AZFP Environmental Sciences "
+                "and raise an issue in the echopype repository."
+            )
+
+        # Check if the specified freq-pulse length combination is in the allowable Sv_offset dict
+        if pulse_len not in SV_OFFSET[freq]:
+            raise ValueError(
+                f"Pulse length {pulse_len} us is not in the Sv offset dictionary "
+                f"for the {freq} Hz channel! "  # add freq info
+                "Please contact AZFP Environmental Sciences "
+                "and raise an issue in the echopype repository."
+            )
+
+        return SV_OFFSET[freq][pulse_len]
```

### Comparing `echopype-0.8.3/echopype/convert/parse_base.py` & `echopype-0.8.4/echopype/convert/parse_base.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/convert/set_groups_ad2cp.py` & `echopype-0.8.4/echopype/convert/set_groups_ad2cp.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,20 +199,22 @@
             if field_exists[field_name]
         }
         data_vars: Dict[
             str,
             Union[Tuple[List[str], np.ndarray, Dict[str, str]], Tuple[Tuple[()], None]],
         ] = {
             var_name: (
-                [dim.dimension_name() for dim in dims[field_name]],
-                combined_fields[field_name],
-                attrs.get(field_name, {}),
+                (
+                    [dim.dimension_name() for dim in dims[field_name]],
+                    combined_fields[field_name],
+                    attrs.get(field_name, {}),
+                )
+                if field_exists[field_name]
+                else ((), None)
             )
-            if field_exists[field_name]
-            else ((), None)
             for field_name, var_name in var_names.items()
         }  # type: ignore
         coords: Dict[str, np.ndarray] = dict()
         for time_dim, time_idxs in self.times_idx.items():
             if time_dim in used_dims:
                 coords[time_dim.dimension_name()] = self.timestamps[time_idxs]
         for ahrs_dim, ahrs_coords in AHRS_COORDS.items():
```

### Comparing `echopype-0.8.3/echopype/convert/set_groups_azfp.py` & `echopype-0.8.4/echopype/convert/set_groups_azfp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Class to save unpacked echosounder data to appropriate groups in netcdf or zarr.
 """
+
 from typing import List
 
 import numpy as np
 import xarray as xr
 
 from ..utils.coding import set_time_encodings
 from .set_groups_base import SetGroupsBase
@@ -50,50 +51,35 @@
             "descr": "contains backscatter power (uncalibrated) and other beam or channel-specific data.",  # noqa
         }
     ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        # get frequency values
-        freq_old = list(self.parser_obj.unpacked_data["frequency"])
-
-        # sort the frequencies in ascending order
-        freq_new = freq_old[:]
-        freq_new.sort(reverse=False)
-
-        # obtain sorted frequency indices
-        self.freq_ind_sorted = [freq_new.index(ch) for ch in freq_old]
-
-        # obtain sorted frequencies
-        self.freq_sorted = self.parser_obj.unpacked_data["frequency"][self.freq_ind_sorted]
-
         # obtain channel_ids
         self.channel_ids_sorted = self._create_unique_channel_name()
 
-        # Put Frequency in Hz (this should be done after create_unique_channel_name)
-        self.freq_sorted = self.freq_sorted * 1000  # Frequency in Hz
-
     def _create_unique_channel_name(self):
         """
         Creates a unique channel name for AZFP sensor
         using the variable unpacked_data created by
         the AZFP parser
         """
 
         serial_number = self.parser_obj.unpacked_data["serial_number"]
         frequency_number = self.parser_obj.parameters["frequency_number_phase1"]
 
         if serial_number.size == 1:
-            freq_as_str = self.freq_sorted.astype(int).astype(str)
+            freq_sorted_in_kHz = self.parser_obj.freq_sorted / 1000.0
+            freq_in_kHz_as_str = freq_sorted_in_kHz.astype(int).astype(str)
 
             # TODO: replace str(i+1) with Frequency Number from XML
             channel_id = [
                 str(serial_number) + "-" + freq + "-" + frequency_number[i]
-                for i, freq in enumerate(freq_as_str)
+                for i, freq in enumerate(freq_in_kHz_as_str)
             ]
 
             return channel_id
         else:
             raise NotImplementedError(
                 "Creating a channel name for more than"
                 + " one serial number has not been implemented."
@@ -122,15 +108,15 @@
                         "standard_name": "speed_of_sound_in_sea_water",
                         "units": "m/s",
                         "valid_min": 0.0,
                     },
                 ),
                 "frequency_nominal": (
                     ["channel"],
-                    self.freq_sorted,
+                    self.parser_obj.freq_sorted,
                     {
                         "units": "Hz",
                         "long_name": "Transducer frequency",
                         "valid_min": 0.0,
                         "standard_name": "sound_frequency",
                     },
                 ),
@@ -302,15 +288,15 @@
                         "position_offset_x",
                         "position_offset_y",
                         "position_offset_z",
                     ]
                 },
                 "frequency_nominal": (
                     ["channel"],
-                    self.freq_sorted,
+                    self.parser_obj.freq_sorted,
                     {
                         "units": "Hz",
                         "long_name": "Transducer frequency",
                         "valid_min": 0.0,
                         "standard_name": "sound_frequency",
                     },
                 ),
@@ -346,20 +332,20 @@
         ds = ds.assign_attrs(platform_dict)
         return set_time_encodings(ds)
 
     def set_beam(self) -> List[xr.Dataset]:
         """Set the Beam group."""
         unpacked_data = self.parser_obj.unpacked_data
         parameters = self.parser_obj.parameters
-        dig_rate = unpacked_data["dig_rate"][self.freq_ind_sorted]  # dim: freq
+        dig_rate = unpacked_data["dig_rate"][self.parser_obj.freq_ind_sorted]  # dim: freq
         ping_time = self.parser_obj.ping_time
 
         # Build variables in the output xarray Dataset
         N = []  # for storing backscatter_r values for each frequency
-        for ich in self.freq_ind_sorted:
+        for ich in self.parser_obj.freq_ind_sorted:
             N.append(
                 np.array(
                     [unpacked_data["counts"][p][ich] for p in range(len(unpacked_data["year"]))]
                 )
             )
 
         # Largest number of counts along the range dimension among the different channels
@@ -371,18 +357,18 @@
             N_tmp = np.full((len(N), len(ping_time), longest_range_sample), np.nan)
             for i, n in enumerate(N):
                 N_tmp[i, :, : n.shape[1]] = n
             N = N_tmp
             del N_tmp
 
         tdn = (
-            unpacked_data["pulse_len"][self.freq_ind_sorted] / 1e6
+            unpacked_data["pulse_len"][self.parser_obj.freq_ind_sorted] / 1e6
         )  # Convert microseconds to seconds
         range_samples_per_bin = unpacked_data["range_samples_per_bin"][
-            self.freq_ind_sorted
+            self.parser_obj.freq_ind_sorted
         ]  # from data header
 
         # Calculate sample interval in seconds
         if len(dig_rate) == len(range_samples_per_bin):
             # TODO: below only correct if range_samples_per_bin=1,
             #  need to implement p.86 for the case when averaging is used
             sample_int = range_samples_per_bin / dig_rate
@@ -390,15 +376,15 @@
             # TODO: not sure what this error means
             raise ValueError("dig_rate and range_samples not unique across frequencies")
 
         ds = xr.Dataset(
             {
                 "frequency_nominal": (
                     ["channel"],
-                    self.freq_sorted,
+                    self.parser_obj.freq_sorted,
                     {
                         "units": "Hz",
                         "long_name": "Transducer frequency",
                         "valid_min": 0.0,
                         "standard_name": "sound_frequency",
                     },
                 ),
@@ -436,24 +422,26 @@
                             "long_name"
                         ],
                         "units": "count",
                     },
                 ),
                 "equivalent_beam_angle": (
                     ["channel"],
-                    parameters["BP"][self.freq_ind_sorted],
+                    parameters["BP"][self.parser_obj.freq_ind_sorted],
                     {
                         "long_name": "Equivalent beam angle",
                         "units": "sr",
                         "valid_range": (0.0, 4 * np.pi),
                     },
                 ),
                 "gain_correction": (
                     ["channel"],
-                    np.array(unpacked_data["gain"][self.freq_ind_sorted], dtype=np.float64),
+                    np.array(
+                        unpacked_data["gain"][self.parser_obj.freq_ind_sorted], dtype=np.float64
+                    ),
                     {"long_name": "Gain correction", "units": "dB"},
                 ),
                 "sample_interval": (
                     ["channel"],
                     sample_int,
                     {
                         "long_name": "Interval between recorded raw data samples",
@@ -468,20 +456,20 @@
                         "long_name": "Nominal bandwidth of transmitted pulse",
                         "units": "s",
                         "valid_min": 0.0,
                     },
                 ),
                 "transmit_frequency_start": (
                     ["channel"],
-                    self.freq_sorted,
+                    self.parser_obj.freq_sorted,
                     self._varattrs["beam_var_default"]["transmit_frequency_start"],
                 ),
                 "transmit_frequency_stop": (
                     ["channel"],
-                    self.freq_sorted,
+                    self.parser_obj.freq_sorted,
                     self._varattrs["beam_var_default"]["transmit_frequency_stop"],
                 ),
                 "transmit_type": (
                     [],
                     "CW",
                     {
                         "long_name": "Type of transmitted pulse",
@@ -551,90 +539,85 @@
         return [set_time_encodings(ds)]
 
     def set_vendor(self) -> xr.Dataset:
         """Set the Vendor_specific group."""
         unpacked_data = self.parser_obj.unpacked_data
         parameters = self.parser_obj.parameters
         ping_time = self.parser_obj.ping_time
+        Sv_offset = self.parser_obj.Sv_offset
         phase_params = ["burst_interval", "pings_per_burst", "average_burst_pings"]
         phase_freq_params = [
             "dig_rate",
             "range_samples",
             "range_averaging_samples",
             "lock_out_index",
             "gain",
             "storage_format",
         ]
         tdn = []
         for num in parameters["phase_number"]:
-            tdn.append(parameters[f"pulse_len_phase{num}"][self.freq_ind_sorted] / 1e6)
+            tdn.append(parameters[f"pulse_len_phase{num}"][self.parser_obj.freq_ind_sorted] / 1e6)
         tdn = np.array(tdn)
         for param in phase_freq_params:
             for num in parameters["phase_number"]:
-                parameters[param].append(parameters[f"{param}_phase{num}"][self.freq_ind_sorted])
+                parameters[param].append(
+                    parameters[f"{param}_phase{num}"][self.parser_obj.freq_ind_sorted]
+                )
         for param in phase_params:
             for num in parameters["phase_number"]:
                 parameters[param].append(parameters[f"{param}_phase{num}"])
         anc = np.array(unpacked_data["ancillary"])  # convert to np array for easy slicing
 
-        # Build variables in the output xarray Dataset
-        Sv_offset = np.zeros_like(self.freq_sorted)
-        for ind, ich in enumerate(self.freq_ind_sorted):
-            # TODO: should not access the private function, better to compute Sv_offset in parser
-            Sv_offset[ind] = self.parser_obj._calc_Sv_offset(
-                self.freq_sorted[ind], unpacked_data["pulse_len"][ich]
-            )
-
         ds = xr.Dataset(
             {
                 "frequency_nominal": (
                     ["channel"],
-                    self.freq_sorted,
+                    self.parser_obj.freq_sorted,
                     {
                         "units": "Hz",
                         "long_name": "Transducer frequency",
                         "valid_min": 0.0,
                         "standard_name": "sound_frequency",
                     },
                 ),
                 # unpacked ping by ping data from 01A file
                 "digitization_rate": (
                     ["channel"],
-                    unpacked_data["dig_rate"][self.freq_ind_sorted],
+                    unpacked_data["dig_rate"][self.parser_obj.freq_ind_sorted],
                     {
                         "long_name": "Number of samples per second in kHz that is processed by the "
                         "A/D converter when digitizing the returned acoustic signal"
                     },
                 ),
                 "lock_out_index": (
                     ["channel"],
-                    unpacked_data["lock_out_index"][self.freq_ind_sorted],
+                    unpacked_data["lock_out_index"][self.parser_obj.freq_ind_sorted],
                     {
                         "long_name": "The distance, rounded to the nearest Bin Size after the "
                         "pulse is transmitted that over which AZFP will ignore echoes"
                     },
                 ),
                 "number_of_bins_per_channel": (
                     ["channel"],
-                    unpacked_data["num_bins"][self.freq_ind_sorted],
+                    unpacked_data["num_bins"][self.parser_obj.freq_ind_sorted],
                     {"long_name": "Number of bins per channel"},
                 ),
                 "number_of_samples_per_average_bin": (
                     ["channel"],
-                    unpacked_data["range_samples_per_bin"][self.freq_ind_sorted],
+                    unpacked_data["range_samples_per_bin"][self.parser_obj.freq_ind_sorted],
                     {"long_name": "Range samples per bin for each channel"},
                 ),
                 "board_number": (
                     ["channel"],
-                    unpacked_data["board_num"][self.freq_ind_sorted],
+                    unpacked_data["board_num"][self.parser_obj.freq_ind_sorted],
                     {"long_name": "The board the data came from channel 1-4"},
                 ),
                 "data_type": (
                     ["channel"],
-                    unpacked_data["data_type"][self.freq_ind_sorted],
+                    unpacked_data["data_type"][self.parser_obj.freq_ind_sorted],
                     {
                         "long_name": "Datatype for each channel 1=Avg unpacked_data (5bytes), "
                         "0=raw (2bytes)"
                     },
                 ),
                 "ping_status": (["ping_time"], unpacked_data["ping_status"]),
                 "number_of_acquired_pings": (
@@ -746,46 +729,46 @@
                     parameters["lock_out_index"],
                     {
                         "long_name": "(From XML file) The distance, rounded to the nearest "
                         "Bin Size after the pulse is transmitted that over which AZFP will "
                         "ignore echoes"
                     },
                 ),
-                "DS": (["channel"], parameters["DS"][self.freq_ind_sorted]),
+                "DS": (["channel"], parameters["DS"][self.parser_obj.freq_ind_sorted]),
                 "EL": (
                     ["channel"],
-                    parameters["EL"][self.freq_ind_sorted],
+                    parameters["EL"][self.parser_obj.freq_ind_sorted],
                     {"long_name": "Sound pressure at the transducer", "units": "dB"},
                 ),
                 "TVR": (
                     ["channel"],
-                    parameters["TVR"][self.freq_ind_sorted],
+                    parameters["TVR"][self.parser_obj.freq_ind_sorted],
                     {
                         "long_name": "Transmit voltage response of the transducer",
                         "units": "dB re 1uPa/V at 1m",
                     },
                 ),
                 "VTX0": (
                     ["channel"],
-                    parameters["VTX0"][self.freq_ind_sorted],
+                    parameters["VTX0"][self.parser_obj.freq_ind_sorted],
                     {"long_name": "Amplified voltage 0 sent to the transducer"},
                 ),
                 "VTX1": (
                     ["channel"],
-                    parameters["VTX1"][self.freq_ind_sorted],
+                    parameters["VTX1"][self.parser_obj.freq_ind_sorted],
                     {"long_name": "Amplified voltage 1 sent to the transducer"},
                 ),
                 "VTX2": (
                     ["channel"],
-                    parameters["VTX2"][self.freq_ind_sorted],
+                    parameters["VTX2"][self.parser_obj.freq_ind_sorted],
                     {"long_name": "Amplified voltage 2 sent to the transducer"},
                 ),
                 "VTX3": (
                     ["channel"],
-                    parameters["VTX3"][self.freq_ind_sorted],
+                    parameters["VTX3"][self.parser_obj.freq_ind_sorted],
                     {"long_name": "Amplified voltage 3 sent to the transducer"},
                 ),
                 "Sv_offset": (["channel"], Sv_offset),
                 "number_of_samples_digitized_per_pings": (
                     ["phase_number", "channel"],
                     parameters["range_samples"],
                 ),
```

### Comparing `echopype-0.8.3/echopype/convert/set_groups_base.py` & `echopype-0.8.4/echopype/convert/set_groups_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Set
 
 import numpy as np
 import pynmea2
 import xarray as xr
 
 from ..echodata.convention import sonarnetcdf_1
-from ..utils.coding import COMPRESSION_SETTINGS, set_time_encodings
+from ..utils.coding import COMPRESSION_SETTINGS, DEFAULT_TIME_ENCODING, set_time_encodings
 from ..utils.prov import echopype_prov_attrs, source_files_vars
 
 NMEA_SENTENCE_DEFAULT = ["GGA", "GLL", "RMC"]
 
 
 class SetGroupsBase(abc.ABC):
     """Base class for saving groups to netcdf or zarr from echosounder data files."""
@@ -124,19 +124,24 @@
         else:
             return time_val
 
     def set_nmea(self) -> xr.Dataset:
         """Set the Platform/NMEA group."""
         # Save nan if nmea data is not encoded in the raw file
         if len(self.parser_obj.nmea["nmea_string"]) != 0:
-            # Convert np.datetime64 numbers to seconds since 1900-01-01 00:00:00Z
+            # Convert np.datetime64 numbers to nanoseconds since 1970-01-01 00:00:00Z
             # due to xarray.to_netcdf() error on encoding np.datetime64 objects directly
-            time = (
-                self.parser_obj.nmea["timestamp"] - np.datetime64("1900-01-01T00:00:00")
-            ) / np.timedelta64(1, "s")
+            # print(np.array(self.parser_obj.nmea["timestamp"])[idx_loc].shape)
+            time, _, _ = xr.coding.times.encode_cf_datetime(
+                self.parser_obj.nmea["timestamp"],
+                **{
+                    "units": DEFAULT_TIME_ENCODING["units"],
+                    "calendar": DEFAULT_TIME_ENCODING["calendar"],
+                },
+            )
             raw_nmea = self.parser_obj.nmea["nmea_string"]
         else:
             time = [np.nan]
             raw_nmea = [np.nan]
 
         # Handle potential nan timestamp for time
         time = self._nan_timestamp_handler(time)
@@ -211,23 +216,24 @@
         else:
             lat, lon = [np.nan], [np.nan]
         msg_type = (
             [x.sentence_type if hasattr(x, "sentence_type") else np.nan for x in nmea_msg]
             if nmea_msg
             else [np.nan]
         )
-        time1 = (
-            (
-                np.array(self.parser_obj.nmea["timestamp"])[idx_loc]
-                - np.datetime64("1900-01-01T00:00:00")
+        if nmea_msg:
+            time1, _, _ = xr.coding.times.encode_cf_datetime(
+                np.array(self.parser_obj.nmea["timestamp"])[idx_loc],
+                **{
+                    "units": DEFAULT_TIME_ENCODING["units"],
+                    "calendar": DEFAULT_TIME_ENCODING["calendar"],
+                },
             )
-            / np.timedelta64(1, "s")
-            if nmea_msg
-            else [np.nan]
-        )
+        else:
+            time1 = [np.nan]
 
         return time1, msg_type, lat, lon
 
     def _beam_groups_vars(self):
         """Stage beam_group coordinate and beam_group_descr variables sharing
         a common dimension, beam_group, to be inserted in the Sonar group"""
         beam_groups_vars = {
```

### Comparing `echopype-0.8.3/echopype/convert/set_groups_ek60.py` & `echopype-0.8.4/echopype/convert/set_groups_ek60.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/convert/set_groups_ek80.py` & `echopype-0.8.4/echopype/convert/set_groups_ek80.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,17 +166,19 @@
                         "comment": "Time coordinate corresponding to environmental "
                         "variables. Note that Platform.time3 is the same "
                         "as Environment.time1.",
                     },
                 ),
                 "sound_velocity_profile_depth": (
                     ["sound_velocity_profile_depth"],
-                    self.parser_obj.environment["sound_velocity_profile"][::2]
-                    if "sound_velocity_profile" in self.parser_obj.environment
-                    else [],
+                    (
+                        self.parser_obj.environment["sound_velocity_profile"][::2]
+                        if "sound_velocity_profile" in self.parser_obj.environment
+                        else []
+                    ),
                     {
                         "standard_name": "depth",
                         "units": "m",
                         "axis": "Z",
                         "positive": "down",
                         "valid_min": 0.0,
                     },
```

### Comparing `echopype-0.8.3/echopype/convert/utils/ek_date_conversion.py` & `echopype-0.8.4/echopype/convert/utils/ek_date_conversion.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/convert/utils/ek_raw_io.py` & `echopype-0.8.4/echopype/convert/utils/ek_raw_io.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/convert/utils/ek_raw_parsers.py` & `echopype-0.8.4/echopype/convert/utils/ek_raw_parsers.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/convert/utils/ek_swap.py` & `echopype-0.8.4/echopype/convert/utils/ek_swap.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/core.py` & `echopype-0.8.4/echopype/core.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/api.py` & `echopype-0.8.4/echopype/echodata/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/combine.py` & `echopype-0.8.4/echopype/echodata/combine.py`

 * *Files 0% similar despite different names*

```diff
@@ -729,17 +729,19 @@
     combined_mapping = []
     for idx, ed in enumerate(eds):
         is_combined = ed["Provenance"].attrs.get("is_combined", False)
         combined_mapping.append(
             {
                 "is_combined": is_combined,
                 "attrs_dict": _get_prov_attrs(ed["Provenance"], is_combined),
-                "echodata_filename": [str(s) for s in ed["Provenance"][ED_FILENAME].values]
-                if is_combined
-                else [echodata_filenames[idx]],
+                "echodata_filename": (
+                    [str(s) for s in ed["Provenance"][ED_FILENAME].values]
+                    if is_combined
+                    else [echodata_filenames[idx]]
+                ),
             }
         )
     # Get single boolean value to see if there's any combined files
     any_combined = any(d["is_combined"] for d in combined_mapping)
 
     if any_combined:
         # Fetches the true echodata filenames if there are any combined files
@@ -751,17 +753,19 @@
     tree_dict = {}
     for ed_group in all_group_paths:
         # collect the group Dataset from all eds that have their channels unselected
         all_chan_ds_list = [ed[ed_group] for ed in eds]
 
         # select only the appropriate channels from each Dataset
         ds_list = [
-            ds.sel(channel=ed_group_chan_sel[ed_group])
-            if ed_group_chan_sel[ed_group] is not None
-            else ds
+            (
+                ds.sel(channel=ed_group_chan_sel[ed_group])
+                if ed_group_chan_sel[ed_group] is not None
+                else ds
+            )
             for ds in all_chan_ds_list
         ]
 
         if ds_list:
             if not any_combined:
                 # Get all of the keys and attributes
                 # for regular non combined echodata object
```

### Comparing `echopype-0.8.3/echopype/echodata/convention/1.0.yml` & `echopype-0.8.4/echopype/echodata/convention/1.0.yml`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/convention/conv.py` & `echopype-0.8.4/echopype/echodata/convention/conv.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/convention/utils.py` & `echopype-0.8.4/echopype/echodata/convention/utils.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/echodata.py` & `echopype-0.8.4/echopype/echodata/echodata.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
             {
                 v["ext_time_dim_name"]
                 for v in mappings_expanded.values()
                 if v["ext_time_dim_name"] != "scalar"
             }
         )
         time_dims_max = max([int(dim[-1]) for dim in platform.dims if dim.startswith("time")])
-        new_time_dims = [f"time{time_dims_max+i+1}" for i in range(len(ext_time_dims))]
+        new_time_dims = [f"time{time_dims_max + i + 1}" for i in range(len(ext_time_dims))]
         # Map each new time dim name to the external time dim name:
         new_time_dims_mappings = {new: ext for new, ext in zip(new_time_dims, ext_time_dims)}
 
         # Process variable updates by corresponding new time dimensions
         for time_dim in new_time_dims:
             ext_time_dim = new_time_dims_mappings[time_dim]
             mappings_selected = {
```

### Comparing `echopype-0.8.3/echopype/echodata/sensor_ep_version_mapping/ep_version_mapper.py` & `echopype-0.8.4/echopype/echodata/sensor_ep_version_mapping/ep_version_mapper.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/sensor_ep_version_mapping/v05x_to_v06x.py` & `echopype-0.8.4/echopype/echodata/sensor_ep_version_mapping/v05x_to_v06x.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,29 +258,29 @@
 
         ed_obj["Sonar/Beam_group1"] = ed_obj["Sonar/Beam_group1"].drop(
             ["beamwidth_receive_athwartship", "beamwidth_transmit_alongship"]
         )
 
     if sensor in ["EK60", "EK80"]:
         for beam_group in ed_obj._tree["Sonar"].children.values():
-            beam_group.ds.angle_sensitivity_alongship.attrs[
-                "long_name"
-            ] = "alongship angle sensitivity of the transducer"
-
-            beam_group.ds.angle_sensitivity_athwartship.attrs[
-                "long_name"
-            ] = "athwartship angle sensitivity of the transducer"
-
-            beam_group.ds.angle_offset_alongship.attrs[
-                "long_name"
-            ] = "electrical alongship angle offset of the transducer"
-
-            beam_group.ds.angle_offset_athwartship.attrs[
-                "long_name"
-            ] = "electrical athwartship angle offset of the transducer"
+            beam_group.ds.angle_sensitivity_alongship.attrs["long_name"] = (
+                "alongship angle sensitivity of the transducer"
+            )
+
+            beam_group.ds.angle_sensitivity_athwartship.attrs["long_name"] = (
+                "athwartship angle sensitivity of the transducer"
+            )
+
+            beam_group.ds.angle_offset_alongship.attrs["long_name"] = (
+                "electrical alongship angle offset of the transducer"
+            )
+
+            beam_group.ds.angle_offset_athwartship.attrs["long_name"] = (
+                "electrical athwartship angle offset of the transducer"
+            )
 
 
 def _add_comment_to_beam_vars(ed_obj, sensor):
     """
     For EK60 and EK80
     Add the ``comment`` attribute to the variables
     ``beamwidth_twoway_alongship/athwartship``,
@@ -329,31 +329,31 @@
             )
 
             beam_group.ds.angle_offset_athwartship.attrs["comment"] = (
                 "Introduced in echopype for Simrad echosounders. The athwartship "
                 "angle corresponds to the major angle in SONAR-netCDF4 vers 2. "
             )
 
-            beam_group.ds.angle_sensitivity_alongship.attrs[
-                "comment"
-            ] = beam_group.ds.angle_offset_alongship.attrs["comment"]
-
-            beam_group.ds.angle_sensitivity_athwartship.attrs[
-                "comment"
-            ] = beam_group.ds.angle_offset_athwartship.attrs["comment"]
+            beam_group.ds.angle_sensitivity_alongship.attrs["comment"] = (
+                beam_group.ds.angle_offset_alongship.attrs["comment"]
+            )
+
+            beam_group.ds.angle_sensitivity_athwartship.attrs["comment"] = (
+                beam_group.ds.angle_offset_athwartship.attrs["comment"]
+            )
 
             if "angle_alongship" in beam_group.ds:
-                beam_group.ds.angle_alongship.attrs[
-                    "comment"
-                ] = beam_group.ds.angle_offset_alongship.attrs["comment"]
+                beam_group.ds.angle_alongship.attrs["comment"] = (
+                    beam_group.ds.angle_offset_alongship.attrs["comment"]
+                )
 
             if "angle_athwartship" in beam_group.ds:
-                beam_group.ds.angle_athwartship.attrs[
-                    "comment"
-                ] = beam_group.ds.angle_offset_athwartship.attrs["comment"]
+                beam_group.ds.angle_athwartship.attrs["comment"] = (
+                    beam_group.ds.angle_offset_athwartship.attrs["comment"]
+                )
 
 
 def _beam_groups_to_convention(ed_obj, set_grp_cls):
     """
     Adds ``beam`` and ``ping_time`` dimensions to variables
     in ``Beam_groupX`` so that they comply with the convention.
     For beam groups containing the ``quadrant``,
```

### Comparing `echopype-0.8.3/echopype/echodata/simrad.py` & `echopype-0.8.4/echopype/echodata/simrad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains functions that are specific to Simrad echo sounders
 """
+
 from typing import Optional, Tuple
 
 import numpy as np
 
 from .echodata import EchoData
```

### Comparing `echopype-0.8.3/echopype/echodata/utils_platform.py` & `echopype-0.8.4/echopype/echodata/utils_platform.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/widgets/static/css/style.css` & `echopype-0.8.4/echopype/echodata/widgets/static/css/style.css`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/widgets/static/html/icons-svg-inline.html` & `echopype-0.8.4/echopype/echodata/widgets/static/html/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/widgets/templates/echodata.html.j2` & `echopype-0.8.4/echopype/echodata/widgets/templates/echodata.html.j2`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/widgets/utils.py` & `echopype-0.8.4/echopype/echodata/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/echodata/widgets/widgets.py` & `echopype-0.8.4/echopype/echodata/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/mask/api.py` & `echopype-0.8.4/echopype/mask/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import datetime
 import operator as op
 import pathlib
 from typing import List, Optional, Union
 
+import dask
+import dask.array
 import numpy as np
 import xarray as xr
 
 from ..utils.io import validate_source
 from ..utils.prov import add_processing_level, echopype_prov_attrs, insert_input_processing_level
 from .freq_diff import _check_freq_diff_source_Sv, _parse_freq_diff_eq
 
@@ -99,18 +101,34 @@
                     mask_val, engine=file_type, chunks={}, **storage_options_mask[mask_ind]
                 )
 
             # check mask coordinates
             # the coordinate sequence matters, so fix the tuple form
             allowed_dims = [
                 ("ping_time", "range_sample"),
+                ("ping_time", "depth"),
                 ("channel", "ping_time", "range_sample"),
+                ("channel", "ping_time", "depth"),
             ]
             if mask[mask_ind].dims not in allowed_dims:
-                raise ValueError("All masks must have dimensions ('ping_time', 'range_sample')!")
+                raise ValueError(
+                    "Masks must have one of the following dimensions: "
+                    "('ping_time', 'range_sample'), ('ping_time', 'depth'), "
+                    "('channel', 'ping_time', 'range_sample'), "
+                    "('channel', 'ping_time', 'depth')"
+                )
+
+        # Check for the channel dimension consistency
+        channel_dim_shapes = set()
+        for mask_indiv in mask:
+            if "channel" in mask_indiv.dims:
+                for mask_chan_ind in range(len(mask_indiv["channel"])):
+                    channel_dim_shapes.add(mask_indiv.isel(channel=mask_chan_ind).shape)
+        if len(channel_dim_shapes) > 1:
+            raise ValueError("All masks must have the same shape in the 'channel' dimension.")
 
     else:
         if not isinstance(storage_options_mask, dict):
             raise ValueError(
                 "The provided input storage_options_mask should be a single "
                 "dict because mask is a single value!"
             )
@@ -122,32 +140,32 @@
             # open up DataArray using mask path
             mask = xr.open_dataarray(mask, engine=file_type, chunks={}, **storage_options_mask)
 
     return mask
 
 
 def _check_var_name_fill_value(
-    source_ds: xr.Dataset, var_name: str, fill_value: Union[int, float, np.ndarray, xr.DataArray]
+    source_ds: xr.Dataset, var_name: str, fill_value: Union[int, float, xr.DataArray]
 ) -> Union[int, float, np.ndarray, xr.DataArray]:
     """
     Ensures that the inputs ``var_name`` and ``fill_value`` for the function
     ``apply_mask`` were appropriately provided.
 
     Parameters
     ----------
     source_ds: xr.Dataset
         A Dataset that contains the variable ``var_name``
     var_name: str
         The variable name in ``source_ds`` that the mask should be applied to
-    fill_value: int or float or np.ndarray or xr.DataArray
+    fill_value: int, float, or xr.DataArray
         Specifies the value(s) at false indices
 
     Returns
     -------
-    fill_value: int or float or np.ndarray or xr.DataArray
+    fill_value: int, float, or xr.DataArray
         fill_value with sanitized dimensions
 
     Raises
     ------
     TypeError
         If ``var_name`` or ``fill_value`` are not an accepted type
     ValueError
@@ -161,25 +179,20 @@
         raise TypeError("The input var_name must be a string!")
 
     # ensure var_name is in source_ds
     if var_name not in source_ds.variables:
         raise ValueError("The Dataset source_ds does not contain the variable var_name!")
 
     # check the type of fill_value
-    if not isinstance(fill_value, (int, float, np.ndarray, xr.DataArray)):
-        raise TypeError(
-            "The input fill_value must be of type int or " "float or np.ndarray or xr.DataArray!"
-        )
+    if not isinstance(fill_value, (int, float, xr.DataArray)):
+        raise TypeError("The input fill_value must be of type int, float, or xr.DataArray!")
 
     # make sure that fill_values is the same shape as var_name
-    if isinstance(fill_value, (np.ndarray, xr.DataArray)):
-        if isinstance(fill_value, xr.DataArray):
-            fill_value = fill_value.data.squeeze()  # squeeze out length=1 channel dimension
-        elif isinstance(fill_value, np.ndarray):
-            fill_value = fill_value.squeeze()  # squeeze out length=1 channel dimension
+    if isinstance(fill_value, xr.DataArray):
+        fill_value = fill_value.data.squeeze()  # squeeze out length=1 channel dimension
 
         source_ds_shape = (
             source_ds[var_name].isel(channel=0).shape
             if "channel" in source_ds[var_name].coords
             else source_ds[var_name].shape
         )
 
@@ -242,45 +255,61 @@
 
 
 @add_processing_level("L3*")
 def apply_mask(
     source_ds: Union[xr.Dataset, str, pathlib.Path],
     mask: Union[xr.DataArray, str, pathlib.Path, List[Union[xr.DataArray, str, pathlib.Path]]],
     var_name: str = "Sv",
-    fill_value: Union[int, float, np.ndarray, xr.DataArray] = np.nan,
+    fill_value: Union[int, float, xr.DataArray] = np.nan,
     storage_options_ds: dict = {},
     storage_options_mask: Union[dict, List[dict]] = {},
 ) -> xr.Dataset:
     """
     Applies the provided mask(s) to the Sv variable ``var_name``
     in the provided Dataset ``source_ds``.
 
+    The code allows for these 3 cases of `source_ds` and `mask` dimensions:
+
+    1) No channel in both `source_ds` and `mask`,
+    but they have matching `ping_time` and
+    `depth` (or `range_sample`) dimensions.
+    2) `source_ds` and `mask` both have matching `channel`,
+    `ping_time`, and `depth` (or `range_sample`) dimensions.
+    3) `source_ds` has the channel dimension and `mask` doesn't,
+    but they have matching
+    `ping_time` and `depth` (or `range_sample`) dimensions.
+
+    If a user only wants to apply masks to a subset of the channels in `source_ds`,
+    they could put 1s to allow all data entries in the other channels.
+
     Parameters
     ----------
     source_ds: xr.Dataset, str, or pathlib.Path
         Points to a Dataset that contains the variable the mask should be applied to
     mask: xr.DataArray, str, pathlib.Path, or a list of these datatypes
         The mask(s) to be applied.
-        Can be a single input or list that corresponds to a DataArray or a path.
-        Each entry in the list must have dimensions ``('ping_time', 'range_sample')``.
-        Multi-channel masks are not currently supported.
+        Can be a individual input or a list that corresponds to a DataArray or a path.
+        Each individual input or entry in the list must contain dimensions
+        ``('ping_time', 'range_sample')`` or dimensions ``('ping_time', 'depth')``.
+        The mask can also contain the dimension ``channel``.
         If a path is provided this should point to a zarr or netcdf file with only
         one data variable in it.
         If the input ``mask`` is a list, a logical AND will be used to produce the final
         mask that will be applied to ``var_name``.
     var_name: str, default="Sv"
         The Sv variable name in ``source_ds`` that the mask should be applied to.
-        This variable needs to have coordinates ``ping_time`` and ``range_sample``,
-        and can optionally also have coordinate ``channel``.
+        This variable needs to have coordinates ``('ping_time', 'range_sample')`` or
+        coordinates ``('ping_time', 'depth')``, and can optionally also have coordinate
+        ``channel``.
         In the case of a multi-channel Sv data variable, the ``mask`` will be broadcast
         to all channels.
-    fill_value: int, float, np.ndarray, or xr.DataArray, default=np.nan
+    fill_value: int, float, or xr.DataArray, default=np.nan
         Value(s) at masked indices.
-        If ``fill_value`` is of type ``np.ndarray`` or ``xr.DataArray``,
-        it must have the same shape as each entry of ``mask``.
+        If ``fill_value`` is of type ``xr.DataArray`` it must have the same shape as each
+        entry of ``mask``.
     storage_options_ds: dict, default={}
         Any additional parameters for the storage backend, corresponding to the
         path provided for ``source_ds``
     storage_options_mask: dict or list of dict, default={}
         Any additional parameters for the storage backend, corresponding to the
         path provided for ``mask``. If ``mask`` is a list, then this input should either
         be a list of dictionaries or a single dictionary with storage options that
@@ -299,71 +328,76 @@
     mask = _validate_and_collect_mask_input(mask, storage_options_mask)
 
     # Check var_name and sanitize fill_value dimensions if an array
     fill_value = _check_var_name_fill_value(source_ds, var_name, fill_value)
 
     # Obtain final mask to be applied to var_name
     if isinstance(mask, list):
-        # perform a logical AND element-wise operation across the masks
-        final_mask = np.logical_and.reduce(mask)
+        # Broadcast all input masks together before combining them
+        broadcasted_masks = xr.broadcast(*mask)
+
+        # Perform a logical AND element-wise operation across the masks
+        final_mask = np.logical_and.reduce(broadcasted_masks)
 
         # xr.where has issues with attrs when final_mask is an array, so we make it a DataArray
-        final_mask = xr.DataArray(final_mask, coords=mask[0].coords)
+        final_mask = xr.DataArray(final_mask, coords=broadcasted_masks[0].coords)
     else:
         final_mask = mask
 
-    # Sanity check: final_mask should be of the same shape as source_ds[var_name]
-    #               along the ping_time and range_sample dimensions
-    def get_ch_shape(da):
-        return da.isel(channel=0).shape if "channel" in da.dims else da.shape
-
-    # Below operate on the actual data array to be masked
+    # Operate on the actual data array to be masked
     source_da = source_ds[var_name]
 
-    source_da_shape = get_ch_shape(source_da)
-    final_mask_shape = get_ch_shape(final_mask)
-
-    if final_mask_shape != source_da_shape:
+    # The final_mask should be of the same shape as source_ds[var_name]
+    # along the ping_time and range_sample dimensions.
+    source_da_chan_shape = (
+        source_da.isel(channel=0).shape if "channel" in source_da.dims else source_da.shape
+    )
+    final_mask_chan_shape = (
+        final_mask.isel(channel=0).shape if "channel" in final_mask.dims else final_mask.shape
+    )
+    if final_mask_chan_shape != source_da_chan_shape:
         raise ValueError(
             f"The final constructed mask is not of the same shape as source_ds[{var_name}] "
-            "along the ping_time and range_sample dimensions!"
+            "along the ping_time, and range_sample dimensions!"
         )
-
-    # final_mask is always an xr.DataArray with at most length=1 channel dimension
-    if "channel" in final_mask.dims:
-        final_mask = final_mask.isel(channel=0)
-
-    # Make sure fill_value and final_mask are expanded in dimensions
-    if "channel" in source_da.dims:
-        if isinstance(fill_value, np.ndarray):
-            fill_value = np.array([fill_value] * source_da["channel"].size)
-        final_mask = np.array([final_mask.data] * source_da["channel"].size)
+    # If final_mask has dim channel then source_da must have dim channel
+    if "channel" in final_mask.dims and "channel" not in source_da.dims:
+        raise ValueError(
+            "The final constructed mask has the channel dimension, "
+            f"so source_ds[{var_name}] must also have the channel dimension."
+        )
+    # If final_mask and source_da both have channel dimension, then they must
+    # have the same number of channels.
+    elif "channel" in final_mask.dims and "channel" in source_da.dims:
+        if len(final_mask["channel"]) != len(source_da["channel"]):
+            raise ValueError(
+                f"If both the final constructed mask and source_ds[{var_name}] "
+                "have the channel dimension, that dimension should match between the two."
+            )
 
     # Apply the mask to var_name
-    # Somehow keep_attrs=True errors out here, so will attach later
     var_name_masked = xr.where(final_mask, x=source_da, y=fill_value)
 
     # Obtain a shallow copy of source_ds
     output_ds = source_ds.copy(deep=False)
 
     # Replace var_name with var_name_masked
     output_ds[var_name] = var_name_masked
     output_ds[var_name] = output_ds[var_name].assign_attrs(source_da.attrs)
 
     # Add or modify variable and global (dataset) provenance attributes
     output_ds[var_name] = output_ds[var_name].assign_attrs(
         _variable_prov_attrs(output_ds[var_name], mask)
     )
 
+    # Attribute handling
     process_type = "mask"
     prov_dict = echopype_prov_attrs(process_type=process_type)
     prov_dict[f"{process_type}_function"] = "mask.apply_mask"
-
     output_ds = output_ds.assign_attrs(prov_dict)
-
     output_ds = insert_input_processing_level(output_ds, input_ds=source_ds)
 
     return output_ds
 
 
 def frequency_differencing(
     source_Sv: Union[xr.Dataset, str, pathlib.Path],
@@ -445,16 +479,16 @@
     >>> freq_nom = xr.DataArray(data=np.array([1.0, 2.0]),
     ...                         coords={"channel": ['chan1', 'chan2']})
     ...
     >>> # construct mock Sv Dataset
     >>> Sv_ds = xr.Dataset(data_vars={"Sv": Sv_da, "frequency_nominal": freq_nom})
     ...
     >>> # compute frequency-differencing mask using channel names
-    >>> echopype.mask.frequency_differencing(source_Sv=mock_Sv_ds, storage_options={},
-    ...                                      freqABEq=None, chanABEq = '"chan1" - "chan2">=10.0')
+    >>> echopype.mask.frequency_differencing(source_Sv=Sv_ds, storage_options={},
+    ...                                      freqABEq=None, chanABEq = '"chan1" - "chan2">=10.0dB')
     <xarray.DataArray 'mask' (ping_time: 5, range_sample: 5)>
     array([[False, False, False, False, False],
            [False, False, False, False, False],
            [ True,  True,  True,  True,  True],
            [ True,  True,  True,  True,  True],
            [ True,  True,  True,  True,  True]])
     Coordinates:
@@ -487,27 +521,84 @@
         chanB = str(source_Sv.channel.isel(channel=freqB_pos).values)
 
     else:
         # get individual channels
         chanA = chanAB[0]
         chanB = chanAB[1]
 
-    # get the left-hand side of condition
-    lhs = source_Sv["Sv"].sel(channel=chanA) - source_Sv["Sv"].sel(channel=chanB)
+    def _get_lhs(
+        Sv_block: np.ndarray, chanA_idx: int, chanB_idx: int, chan_dim_idx: int = 0
+    ) -> np.ndarray:
+        """Get left-hand side of condition"""
+
+        def _sel_channel(chan_idx):
+            return tuple(
+                [chan_idx if i == chan_dim_idx else slice(None) for i in range(Sv_block.ndim)]
+            )
+
+        # get the left-hand side of condition (lhs)
+        return Sv_block[_sel_channel(chanA_idx)] - Sv_block[_sel_channel(chanB_idx)]
+
+    def _create_mask(lhs: np.ndarray, diff: float) -> np.ndarray:
+        """Create mask using operator lookup table"""
+        return xr.where(str2ops[operator](lhs, diff), True, False)
+
+    # Get the Sv data array
+    Sv_data_array = source_Sv["Sv"]
+
+    # Determine channel index based on names
+    channels = list(source_Sv["channel"].to_numpy())
+    chanA_idx = channels.index(chanA)
+    chanB_idx = channels.index(chanB)
+    # Get the channel dimension index for filtering
+    chan_dim_idx = Sv_data_array.dims.index("channel")
+
+    # If Sv data is not dask array
+    if not isinstance(Sv_data_array.variable._data, dask.array.Array):
+        # get the left-hand side of condition
+        lhs = _get_lhs(Sv_data_array, chanA_idx, chanB_idx, chan_dim_idx=chan_dim_idx)
+
+        # create mask using operator lookup table
+        da = _create_mask(lhs, diff)
+    # If Sv data is dask array
+    else:
+        # Get the final data array template
+        template = Sv_data_array.isel(channel=0).drop_vars("channel")
+
+        dask_array_data = Sv_data_array.data
+        # Perform block wise computation
+        dask_array_result = (
+            dask_array_data
+            # Compute the left-hand side of condition
+            # drop the first axis (channel) as it is dropped in the result
+            .map_blocks(
+                _get_lhs,
+                chanA_idx,
+                chanB_idx,
+                chan_dim_idx=chan_dim_idx,
+                dtype=dask_array_data.dtype,
+                drop_axis=0,
+            )
+            # create mask using operator lookup table
+            .map_blocks(_create_mask, diff)
+        )
+
+        # Create DataArray of the result
+        da = xr.DataArray(
+            data=dask_array_result,
+            coords=template.coords,
+        )
 
-    # create mask using operator lookup table
-    da = xr.where(str2ops[operator](lhs, diff), True, False)
+    xr_dataarray_attrs = {
+        "mask_type": "frequency differencing",
+        "history": f"{datetime.datetime.utcnow()} +00:00. "
+        "Mask created by mask.frequency_differencing. "
+        f"Operation: Sv['{chanA}'] - Sv['{chanB}'] {operator} {diff}",
+    }
 
     # assign a name to DataArray
     da.name = "mask"
 
     # assign provenance attributes
-    mask_attrs = {"mask_type": "frequency differencing"}
-    history_attr = (
-        f"{datetime.datetime.utcnow()} +00:00. "
-        "Mask created by mask.frequency_differencing. "
-        f"Operation: Sv['{chanA}'] - Sv['{chanB}'] {operator} {diff}"
-    )
-
-    da = da.assign_attrs({**mask_attrs, **{"history": history_attr}})
+    da = da.assign_attrs(xr_dataarray_attrs)
 
     return da
```

### Comparing `echopype-0.8.3/echopype/mask/freq_diff.py` & `echopype-0.8.4/echopype/mask/freq_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     """
 
     if (freqABEq is None) and (chanABEq is None):
         raise ValueError("Either freqAB or chanAB must be given!")
     elif (freqABEq is not None) and (chanABEq is not None):
         raise ValueError("Only one of freqAB or chanAB should be given, but not both!")
     elif freqABEq is not None:
-        freqAPattern = r"(?P<freqA>\d*\.\d+)\s*(?P<unitA>\w?)Hz"
-        freqBPattern = r"(?P<freqB>\d*\.\d+)\s*(?P<unitB>\w?)Hz"
+        freqAPattern = r"(?P<freqA>\d*\.?\d+)\s*(?P<unitA>\w?)Hz"
+        freqBPattern = r"(?P<freqB>\d*\.?\d+)\s*(?P<unitB>\w?)Hz"
         operatorPattern = r"\s*(?P<cmp>\S*?)\s*"
         rhsPattern = r"(?P<db>\d*\.?\d+)\s*dB"
         diffMatcher = re.compile(
             freqAPattern + r"\s*-\s*" + freqBPattern + operatorPattern + rhsPattern
         )
         eqMatched = diffMatcher.match(freqABEq)
         if eqMatched is None:
```

### Comparing `echopype-0.8.3/echopype/metrics/summary_statistics.py` & `echopype-0.8.4/echopype/metrics/summary_statistics.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/qc/api.py` & `echopype-0.8.4/echopype/qc/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/utils/coding.py` & `echopype-0.8.4/echopype/utils/coding.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import xarray as xr
 import zarr
 from dask.array.core import auto_chunks
 from dask.utils import parse_bytes
 from xarray import coding
 
 DEFAULT_TIME_ENCODING = {
-    "units": "seconds since 1900-01-01T00:00:00+00:00",
+    "units": "nanoseconds since 1970-01-01T00:00:00Z",
     "calendar": "gregorian",
-    "_FillValue": np.nan,
-    "dtype": np.dtype("float64"),
+    "dtype": np.dtype("int64"),
 }
 
 COMPRESSION_SETTINGS = {
     "netcdf4": {"zlib": True, "complevel": 4},
     # zarr compressors were chosen based on xarray results
     "zarr": {
         "float": {"compressor": zarr.Blosc(cname="zstd", clevel=3, shuffle=2)},
@@ -67,32 +66,38 @@
                 expected_dtype = var.dtype
 
             if not np.issubdtype(var.dtype, expected_dtype):
                 ds[name] = var.astype(expected_dtype)
     return ds
 
 
-def _encode_dataarray(da, dtype):
+def _encode_time_dataarray(da):
     """Encodes and decode datetime64 array similar to writing to file"""
     if da.size == 0:
         return da
-    read_encoding = {
-        "units": "seconds since 1900-01-01T00:00:00+00:00",
-        "calendar": "gregorian",
-    }
-
-    if dtype in [np.float64, np.int64]:
+    if da.dtype == np.int64:
         encoded_data = da
+    elif da.dtype == np.float64:
+        raise ValueError("Encoded time data array must be of type ```np.int64```.")
     else:
         # fmt: off
         encoded_data, _, _ = coding.times.encode_cf_datetime(
-            da, **read_encoding
+            da, **{
+                "units": DEFAULT_TIME_ENCODING["units"],
+                "calendar": DEFAULT_TIME_ENCODING["calendar"],
+            }
         )
         # fmt: on
-    return coding.times.decode_cf_datetime(encoded_data, **read_encoding)
+    return coding.times.decode_cf_datetime(
+        encoded_data,
+        **{
+            "units": DEFAULT_TIME_ENCODING["units"],
+            "calendar": DEFAULT_TIME_ENCODING["calendar"],
+        },
+    )
 
 
 def _get_auto_chunk(
     variable: xr.DataArray, chunk_size: "int | str | float" = "100MB"
 ) -> Tuple[int]:
     """
     Calculate default chunks for a data array based on desired chunk size
@@ -123,18 +128,17 @@
     for var, encoding in DEFAULT_ENCODINGS.items():
         if var in new_ds:
             da = new_ds[var].copy()
             # Process all variable names matching the patterns *_time* or time<digits>
             # Examples: ping_time, ping_time_2, time1, time2
             if bool(search(r"_time|^time[\d]+$", var)):
                 new_ds[var] = xr.apply_ufunc(
-                    _encode_dataarray,
+                    _encode_time_dataarray,
                     da,
                     keep_attrs=True,
-                    kwargs={"dtype": da.dtype},
                 )
 
             new_ds[var].encoding = encoding
 
     return new_ds
```

### Comparing `echopype-0.8.3/echopype/utils/compute.py` & `echopype-0.8.4/echopype/utils/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """compute.py
 
 Module containing various helper functions
 for performing computations within echopype.
 """
+
 from typing import Union
 
 import dask.array
 import numpy as np
 
 
 def _log2lin(data: Union[dask.array.Array, np.ndarray]) -> Union[dask.array.Array, np.ndarray]:
```

### Comparing `echopype-0.8.3/echopype/utils/io.py` & `echopype-0.8.4/echopype/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 echopype utilities for file handling
 """
+
 import os
 import pathlib
 import platform
 import sys
 import tempfile
 import uuid
 from pathlib import Path, WindowsPath
```

### Comparing `echopype-0.8.3/echopype/utils/log.py` & `echopype-0.8.4/echopype/utils/log.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/utils/misc.py` & `echopype-0.8.4/echopype/utils/misc.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/utils/prov.py` & `echopype-0.8.4/echopype/utils/prov.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/utils/uwa.py` & `echopype-0.8.4/echopype/utils/uwa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utilities for calculating seawater acoustic properties.
 """
+
 import numpy as np
 
 
 def calc_sound_speed(temperature=27, salinity=35, pressure=10, formula_source="Mackenzie"):
     """
     Calculate sound speed in [m/s].
 
@@ -32,20 +33,15 @@
     Mackenzie KV (1981) Nine‐term equation for sound speed in the oceans.
     The Journal of the Acoustical Society of America, 70(3), 807–812.
     https://doi.org/10.1121/1.386920
     The ranges of validity encompass the following:
     temperature −2 to 30 °C, salinity 30 to 40 ppt, and depth 0 to 8000 m.
     """
     if formula_source == "Mackenzie":
-        ss = (
-            1448.96
-            + 4.591 * temperature
-            - 5.304e-2 * temperature**2
-            + 2.374e-4 * temperature**3
-        )
+        ss = 1448.96 + 4.591 * temperature - 5.304e-2 * temperature**2 + 2.374e-4 * temperature**3
         ss += 1.340 * (salinity - 35) + 1.630e-2 * pressure + 1.675e-7 * pressure**2
         ss += -1.025e-2 * temperature * (salinity - 35) - 7.139e-13 * temperature * pressure**3
     elif formula_source == "AZFP":
         z = temperature / 10
         ss = (
             1449.05
             + z * (45.7 + z * (-5.21 + 0.23 * z))
```

### Comparing `echopype-0.8.3/echopype/visualize/api.py` & `echopype-0.8.4/echopype/visualize/api.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/visualize/cm.py` & `echopype-0.8.4/echopype/visualize/cm.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype/visualize/plot.py` & `echopype-0.8.4/echopype/visualize/plot.py`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/echopype.egg-info/PKG-INFO` & `echopype-0.8.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echopype
-Version: 0.8.3
+Version: 0.8.4
 Summary: Enhancing the interoperability and scalability in analyzing ocean sonar data
 Home-page: https://github.com/OSOceanAcoustics/echopype
 Author: Wu-Jung Lee
 Author-email: leewujung@gmail.com
 Maintainer: Wu-Jung Lee
 Maintainer-email: leewujung@gmail.com
 License: Apache License, Version 2.0
@@ -64,55 +64,101 @@
   </a>
 
   <a href="https://anaconda.org/conda-forge/echopype">
     <img src="https://img.shields.io/conda/vn/conda-forge/echopype.svg"/>
   </a>
 </div>
 
+[![ssec](https://img.shields.io/badge/SSEC-Project-purple?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA0AAAAOCAQAAABedl5ZAAAACXBIWXMAAAHKAAABygHMtnUxAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAMNJREFUGBltwcEqwwEcAOAfc1F2sNsOTqSlNUopSv5jW1YzHHYY/6YtLa1Jy4mbl3Bz8QIeyKM4fMaUxr4vZnEpjWnmLMSYCysxTcddhF25+EvJia5hhCudULAePyRalvUteXIfBgYxJufRuaKuprKsbDjVUrUj40FNQ11PTzEmrCmrevPhRcVQai8m1PRVvOPZgX2JttWYsGhD3atbHWcyUqX4oqDtJkJiJHUYv+R1JbaNHJmP/+Q1HLu2GbNoSm3Ft0+Y1YMdPSTSwQAAAABJRU5ErkJggg==&style=plastic)](https://escience.washington.edu/echopype/)
+
 Echopype is a package built to enable interoperability and scalability in ocean sonar data processing. These data are widely used for obtaining information about the distribution and abundance of marine animals, such as fish and krill. Our ability to collect large volumes of sonar data from a variety of ocean platforms has grown significantly in the last decade. However, most of the new data remain under-utilized. echopype aims to address the root cause of this problem - the lack of interoperable data format and scalable analysis workflows that adapt well with increasing data volume - by providing open-source tools as entry points for scientists to make discovery using these new data.
 
 Watch the [echopype talk](https://www.youtube.com/watch?v=qboH7MyHrpU)
 at SciPy 2019 for background, discussions and a quick demo!
 
+
 ## Documentation
 
 Learn more about echopype in the official documentation at https://echopype.readthedocs.io. Check out executable examples in the companion repository https://github.com/OSOceanAcoustics/echopype-examples.
 
 
 ## Contributing
 
 You can find information about how to contribute to echopype at our [Contributing Page](https://echopype.readthedocs.io/en/latest/contributing.html).
 
+## <img src="docs/source/images/GSoC-logo-horizontal.svg" alt="Google Summer of Code logo" width="300" style="padding-right: 50px; vertical-align: middle">
+
+In collaboration with the [Integrated Ocean Observing System (IOOS)](https://ioos.noaa.gov/), the Echopype team aims to recruit talented [Google Summer of Code (GSoC)](https://summerofcode.withgoogle.com/)
+participants to help us upgrade the robustness and scalability of the Echopype package.
+
+If you are a GSoC 2024 contributor, please head over to [GSoC contributor's guide](gsoc_contrib_guide.md) to get more information specific to the program.
+
+
 
 ## Echopype doesn't run on your data?
 
 Please report any bugs by [creating issues on GitHub](https://medium.com/nyc-planning-digital/writing-a-proper-github-issue-97427d62a20f).
 
 [Pull requests](https://jarednielsen.com/learn-git-fork-pull-request/) are always welcome!
 
 
-Contributors
-------------
+## Contributors
 
 [![Contributors](https://contrib.rocks/image?repo=OSOceanAcoustics/echopype)](https://github.com/OSOceanAcoustics/echopype/graphs/contributors)
 
-Wu-Jung Lee ([@leewujung](https://github.com/leewujung)) founded the echopype project in 2018. It is currently led by Wu-Jung Lee and Emilio Mayorga ([@emiliom](https://github.com/emiliom)), who are primary developers together with Landung "Don" Setiawan ([@lsetiawan](https://github.com/lsetiawan)), and previously Brandon Reyes ([@b-reyes](https://github.com/b-reyes)), Kavin Nguyen ([@ngkavin](https://github.com/ngkavin)) and Imran Majeed ([@imranmaj](https://github.com/imranmaj)). Valentina Staneva ([@valentina-s](https://github.com/valentina-s)) is also part of the development team.
+Wu-Jung Lee ([@leewujung](https://github.com/leewujung))
+founded the echopype project in 2018 and continue to be the primary contributor
+together with Praneeth Ratna([@praneethratna](https://github.com/praneethratna)).
+Emilio Mayorga ([@emiliom](https://github.com/emiliom)),
+Landung "Don" Setiawan ([@lsetiawan](https://github.com/lsetiawan)),
+Brandon Reyes ([@b-reyes](https://github.com/b-reyes)),
+Kavin Nguyen ([@ngkavin](https://github.com/ngkavin))
+and Imran Majeed ([@imranmaj](https://github.com/imranmaj))
+have contributed significantly to the code.
+Valentina Staneva ([@valentina-s](https://github.com/valentina-s)) is also part of the development team.
 
-Other contributors are listed in [echopype documentation](https://echopype.readthedocs.io).
+A complete list of direct contributors is on our [GitHub Contributors Page](https://github.com/OSOceanAcoustics/echopype/graphs/contributors).
+
+
+## Acknowledgement
 
 We thank Dave Billenness of ASL Environmental Sciences for
-providing the AZFP Matlab Toolbox as reference for our
-development of AZFP support in echopype.
-We also thank Rick Towler ([@rhtowler](https://github.com/rhtowler))
+providing the AZFP Matlab Toolbox as reference for developing
+support for the AZFP echosounder,
+and Rick Towler ([@rhtowler](https://github.com/rhtowler))
 of the NOAA Alaska Fisheries Science Center
 for providing low-level file parsing routines for
 Simrad EK60 and EK80 echosounders.
 
+We also thank funding support from
+the National Science Foundation and NOAA Ocean Exploration,
+and software engineering support from
+the University of Washington Scientific Software Engineering Center (SSEC),
+as part of the Schmidt Futures Virtual Institute for Scientific Software (VISS) in 2023.
+
+<div>
+  <a href="https://oceanexplorer.noaa.gov/news/oer-updates/2021/fy21-ffo-schedule.html">
+    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/79/NOAA_logo.svg/936px-NOAA_logo.svg.png" alt="NOAA_logo" width="120">
+  </a>
+
+  <a href="https://www.nsf.gov/awardsearch/showAward?AWD_ID=1849930&HistoricalAwards=false">
+    <img src="https://upload.wikimedia.org/wikipedia/commons/7/7e/NSF_logo.png" alt="NSF_logo" width="120">
+  </a>
+
+  <a href="https://escience.washington.edu/software-engineering/ssec/">
+    <img src="https://avatars.githubusercontent.com/u/122321194?s=200&v=4" alt="SSEC_logo" width="120">
+  </a>
+</div>
+
+
+
+
+
 ## License
 
 Echopype is licensed under the open source [Apache 2.0 license](https://opensource.org/licenses/Apache-2.0).
 
 ---------------
 
-Copyright (c) 2018-2023, Echopype Developers.
+Copyright (c) 2018-2024, Echopype Developers.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: echopype Version: 0.8.3 Summary: Enhancing the
+Metadata-Version: 2.1 Name: echopype Version: 0.8.4 Summary: Enhancing the
 interoperability and scalability in analyzing ocean sonar data Home-page:
 https://github.com/OSOceanAcoustics/echopype Author: Wu-Jung Lee Author-email:
 leewujung@gmail.com Maintainer: Wu-Jung Lee Maintainer-email:
 leewujung@gmail.com License: Apache License, Version 2.0 Platform: OS
 Independent Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
@@ -18,45 +18,63 @@
 _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_O_S_O_c_e_a_n_A_c_o_u_s_t_i_c_s_/_e_c_h_o_p_y_p_e_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_b_u_i_l_d_._y_a_m_l_/
 _b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_e_s_u_l_t_s_._p_r_e_-_c_o_m_m_i_t_._c_i_/_b_a_d_g_e_/_g_i_t_h_u_b_/_O_S_O_c_e_a_n_A_c_o_u_s_t_i_c_s_/
 _e_c_h_o_p_y_p_e_/_m_a_s_t_e_r_._s_v_g_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_e_c_h_o_p_y_p_e_/_b_a_d_g_e_/
 _?_v_e_r_s_i_o_n_=_l_a_t_e_s_t_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_O_S_O_c_e_a_n_A_c_o_u_s_t_i_c_s_/_e_c_h_o_p_y_p_e_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/
 _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_G_T_9_8_F_9_1_9_X_R_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_e_c_h_o_p_y_p_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_n_d_a_/_v_n_/
 _c_o_n_d_a_-_f_o_r_g_e_/_e_c_h_o_p_y_p_e_._s_v_g_]
-Echopype is a package built to enable interoperability and scalability in ocean
-sonar data processing. These data are widely used for obtaining information
-about the distribution and abundance of marine animals, such as fish and krill.
-Our ability to collect large volumes of sonar data from a variety of ocean
-platforms has grown significantly in the last decade. However, most of the new
-data remain under-utilized. echopype aims to address the root cause of this
-problem - the lack of interoperable data format and scalable analysis workflows
-that adapt well with increasing data volume - by providing open-source tools as
-entry points for scientists to make discovery using these new data. Watch the
-[echopype talk](https://www.youtube.com/watch?v=qboH7MyHrpU) at SciPy 2019 for
-background, discussions and a quick demo! ## Documentation Learn more about
-echopype in the official documentation at https://echopype.readthedocs.io.
-Check out executable examples in the companion repository https://github.com/
-OSOceanAcoustics/echopype-examples. ## Contributing You can find information
-about how to contribute to echopype at our [Contributing Page](https://
-echopype.readthedocs.io/en/latest/contributing.html). ## Echopype doesn't run
-on your data? Please report any bugs by [creating issues on GitHub](https://
-medium.com/nyc-planning-digital/writing-a-proper-github-issue-97427d62a20f).
-[Pull requests](https://jarednielsen.com/learn-git-fork-pull-request/) are
-always welcome! Contributors ------------ [![Contributors](https://
-contrib.rocks/image?repo=OSOceanAcoustics/echopype)](https://github.com/
-OSOceanAcoustics/echopype/graphs/contributors) Wu-Jung Lee ([@leewujung](https:
-//github.com/leewujung)) founded the echopype project in 2018. It is currently
-led by Wu-Jung Lee and Emilio Mayorga ([@emiliom](https://github.com/emiliom)),
-who are primary developers together with Landung "Don" Setiawan ([@lsetiawan]
-(https://github.com/lsetiawan)), and previously Brandon Reyes ([@b-reyes]
-(https://github.com/b-reyes)), Kavin Nguyen ([@ngkavin](https://github.com/
-ngkavin)) and Imran Majeed ([@imranmaj](https://github.com/imranmaj)).
-Valentina Staneva ([@valentina-s](https://github.com/valentina-s)) is also part
-of the development team. Other contributors are listed in [echopype
-documentation](https://echopype.readthedocs.io). We thank Dave Billenness of
-ASL Environmental Sciences for providing the AZFP Matlab Toolbox as reference
-for our development of AZFP support in echopype. We also thank Rick Towler (
-[@rhtowler](https://github.com/rhtowler)) of the NOAA Alaska Fisheries Science
-Center for providing low-level file parsing routines for Simrad EK60 and EK80
-echosounders. ## License Echopype is licensed under the open source [Apache 2.0
-license](https://opensource.org/licenses/Apache-2.0). --------------- Copyright
-(c) 2018-2023, Echopype Developers.
+[![ssec](https://img.shields.io/badge/SSEC-Project-purple?logo=data:image/
+png;base64,iVBORw0KGgoAAAANSUhEUgAAAA0AAAAOCAQAAABedl5ZAAAACXBIWXMAAAHKAAABygHMtnUxAAAAGXRFWHRTb2Z0d2FyZQB3d3cuaW5rc2NhcGUub3Jnm+48GgAAAMNJREFUGBltwcEqwwEcAOAfc1F2sNsOTqSlNUopSv5jW1YzHHYY/
+6YtLa1Jy4mbl3Bz8QIeyKM4fMaUxr4vZnEpjWnmLMSYCysxTcddhF25+EvJia5hhCudULAePyRalvUteXIfBgYxJufRuaKuprKsbDjVUrUj40FNQ11PTzEmrCmrevPhRcVQai8m1PRVvOPZgX2JttWYsGhD3atbHWcyUqX4oqDtJkJiJHUYv+R1JbaNHJmP/
++Q1HLu2GbNoSm3Ft0+Y1YMdPSTSwQAAAABJRU5ErkJggg==&style=plastic)](https://
+escience.washington.edu/echopype/) Echopype is a package built to enable
+interoperability and scalability in ocean sonar data processing. These data are
+widely used for obtaining information about the distribution and abundance of
+marine animals, such as fish and krill. Our ability to collect large volumes of
+sonar data from a variety of ocean platforms has grown significantly in the
+last decade. However, most of the new data remain under-utilized. echopype aims
+to address the root cause of this problem - the lack of interoperable data
+format and scalable analysis workflows that adapt well with increasing data
+volume - by providing open-source tools as entry points for scientists to make
+discovery using these new data. Watch the [echopype talk](https://
+www.youtube.com/watch?v=qboH7MyHrpU) at SciPy 2019 for background, discussions
+and a quick demo! ## Documentation Learn more about echopype in the official
+documentation at https://echopype.readthedocs.io. Check out executable examples
+in the companion repository https://github.com/OSOceanAcoustics/echopype-
+examples. ## Contributing You can find information about how to contribute to
+echopype at our [Contributing Page](https://echopype.readthedocs.io/en/latest/
+contributing.html). ## [Google Summer of Code logo]In collaboration with the
+[Integrated Ocean Observing System (IOOS)](https://ioos.noaa.gov/), the
+Echopype team aims to recruit talented [Google Summer of Code (GSoC)](https://
+summerofcode.withgoogle.com/) participants to help us upgrade the robustness
+and scalability of the Echopype package. If you are a GSoC 2024 contributor,
+please head over to [GSoC contributor's guide](gsoc_contrib_guide.md) to get
+more information specific to the program. ## Echopype doesn't run on your data?
+Please report any bugs by [creating issues on GitHub](https://medium.com/nyc-
+planning-digital/writing-a-proper-github-issue-97427d62a20f). [Pull requests]
+(https://jarednielsen.com/learn-git-fork-pull-request/) are always welcome! ##
+Contributors [![Contributors](https://contrib.rocks/
+image?repo=OSOceanAcoustics/echopype)](https://github.com/OSOceanAcoustics/
+echopype/graphs/contributors) Wu-Jung Lee ([@leewujung](https://github.com/
+leewujung)) founded the echopype project in 2018 and continue to be the primary
+contributor together with Praneeth Ratna([@praneethratna](https://github.com/
+praneethratna)). Emilio Mayorga ([@emiliom](https://github.com/emiliom)),
+Landung "Don" Setiawan ([@lsetiawan](https://github.com/lsetiawan)), Brandon
+Reyes ([@b-reyes](https://github.com/b-reyes)), Kavin Nguyen ([@ngkavin](https:
+//github.com/ngkavin)) and Imran Majeed ([@imranmaj](https://github.com/
+imranmaj)) have contributed significantly to the code. Valentina Staneva (
+[@valentina-s](https://github.com/valentina-s)) is also part of the development
+team. A complete list of direct contributors is on our [GitHub Contributors
+Page](https://github.com/OSOceanAcoustics/echopype/graphs/contributors). ##
+Acknowledgement We thank Dave Billenness of ASL Environmental Sciences for
+providing the AZFP Matlab Toolbox as reference for developing support for the
+AZFP echosounder, and Rick Towler ([@rhtowler](https://github.com/rhtowler)) of
+the NOAA Alaska Fisheries Science Center for providing low-level file parsing
+routines for Simrad EK60 and EK80 echosounders. We also thank funding support
+from the National Science Foundation and NOAA Ocean Exploration, and software
+engineering support from the University of Washington Scientific Software
+Engineering Center (SSEC), as part of the Schmidt Futures Virtual Institute for
+Scientific Software (VISS) in 2023.
+_[_N_O_A_A___l_o_g_o_]_[_N_S_F___l_o_g_o_]_[_S_S_E_C___l_o_g_o_]
+## License Echopype is licensed under the open source [Apache 2.0 license]
+(https://opensource.org/licenses/Apache-2.0). --------------- Copyright (c)
+2018-2024, Echopype Developers.
```

### Comparing `echopype-0.8.3/echopype.egg-info/SOURCES.txt` & `echopype-0.8.4/echopype.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .flake8
 CITATION.cff
 LICENSE
 MANIFEST.in
 README.md
 _echopype_version.py
+gsoc_contrib_guide.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 echopype/__init__.py
 echopype/core.py
```

### Comparing `echopype-0.8.3/pyproject.toml` & `echopype-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `echopype-0.8.3/setup.cfg` & `echopype-0.8.4/setup.cfg`

 * *Files identical despite different names*

