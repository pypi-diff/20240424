# Comparing `tmp/ourskyai_astro_api-1.3.3368.tar.gz` & `tmp/ourskyai_astro_api-1.3.3442.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3368.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3442.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3368.tar` & `ourskyai_astro_api-1.3.3442.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    11057 2024-04-18 04:36:56.128272 ourskyai_astro_api-1.3.3368/README.md
--rw-r--r--   0        0        0     5741 2024-04-18 04:36:59.984380 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-04-18 04:37:00.024381 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   253842 2024-04-18 04:37:00.136384 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-04-18 04:37:00.176385 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-04-18 04:37:00.240387 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-04-18 04:37:00.276388 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-04-18 04:37:00.352390 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5100 2024-04-18 04:37:00.408391 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-04-18 04:37:00.456393 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-04-18 04:37:00.536395 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-04-18 04:37:00.596397 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     1904 2024-04-18 04:37:00.644398 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-04-18 04:37:00.728400 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     2155 2024-04-18 04:37:00.776402 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-04-18 04:37:00.836403 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-04-18 04:37:00.900405 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-04-18 04:37:00.952407 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-04-18 04:37:01.012408 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-04-18 04:37:01.076410 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-04-18 04:37:01.128412 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-04-18 04:37:01.180413 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-04-18 04:37:01.224414 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-04-18 04:37:01.280416 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-04-18 04:37:01.344418 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-04-18 04:37:01.392419 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-04-18 04:37:01.484422 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-04-18 04:37:01.528423 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-04-18 04:37:01.568424 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-04-18 04:37:01.628425 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-04-18 04:37:01.712428 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-04-18 04:37:01.772430 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-04-18 04:37:01.808431 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-04-18 04:37:01.840432 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-04-18 04:37:01.884433 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-04-18 04:37:01.940434 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-04-18 04:37:02.004436 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-04-18 04:37:02.060438 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-04-18 04:37:02.116439 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-04-18 04:37:02.160441 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-04-18 04:37:02.208442 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-04-18 04:37:02.256443 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-04-18 04:37:02.296444 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-04-18 04:37:02.332445 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-04-18 04:37:02.388447 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-04-18 04:37:02.432448 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-04-18 04:37:02.464449 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-04-18 04:37:02.512450 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-04-18 04:37:02.568452 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5167 2024-04-18 04:37:02.628454 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-04-18 04:37:02.672455 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-04-18 04:37:02.716456 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-04-18 04:37:02.808459 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-04-18 04:37:02.852460 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-04-18 04:37:02.928462 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-04-18 04:37:03.004464 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-04-18 04:37:03.044465 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-04-18 04:37:03.080466 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-04-18 04:37:03.128467 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-04-18 04:37:03.188469 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-04-18 04:37:03.236471 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-04-18 04:37:03.300472 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-04-18 04:37:03.352474 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-04-18 04:37:03.400475 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-04-18 04:37:03.448476 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-04-18 04:37:03.532479 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-04-18 04:37:03.596481 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-04-18 04:37:03.648482 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-04-18 04:37:03.684483 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-04-18 04:37:03.776486 ourskyai_astro_api-1.3.3368/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-04-18 04:37:03.836487 ourskyai_astro_api-1.3.3368/pyproject.toml
--rw-r--r--   0        0        0    12025 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3368/PKG-INFO
+-rw-r--r--   0        0        0    11057 2024-04-24 17:24:19.912631 ourskyai_astro_api-1.3.3442/README.md
+-rw-r--r--   0        0        0     5741 2024-04-24 17:24:23.540665 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-04-24 17:24:23.572666 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   253842 2024-04-24 17:24:23.664666 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-04-24 17:24:23.736667 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-24 17:24:23.800668 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-04-24 17:24:23.840668 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-04-24 17:24:23.916669 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5100 2024-04-24 17:24:23.992669 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-04-24 17:24:24.048670 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-04-24 17:24:24.108671 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-04-24 17:24:24.204671 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     1904 2024-04-24 17:24:24.256672 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-04-24 17:24:24.328673 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     2155 2024-04-24 17:24:24.376673 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-04-24 17:24:24.440674 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-04-24 17:24:24.488674 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-04-24 17:24:24.536675 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-04-24 17:24:24.596675 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-04-24 17:24:24.644676 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-04-24 17:24:24.704676 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-04-24 17:24:24.756677 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-04-24 17:24:24.796677 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-04-24 17:24:24.848677 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-04-24 17:24:24.892678 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-04-24 17:24:24.936679 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-04-24 17:24:24.972679 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-04-24 17:24:25.024679 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-04-24 17:24:25.072680 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-04-24 17:24:25.144680 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-04-24 17:24:25.196681 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     3777 2024-04-24 17:24:25.256682 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-04-24 17:24:25.316682 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-04-24 17:24:25.376683 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-04-24 17:24:25.416683 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-04-24 17:24:25.468683 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-04-24 17:24:25.532684 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-04-24 17:24:25.628685 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-04-24 17:24:25.688686 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-04-24 17:24:25.796687 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-04-24 17:24:25.876687 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-04-24 17:24:26.028689 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-04-24 17:24:26.100690 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-04-24 17:24:26.164690 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-04-24 17:24:26.224691 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-04-24 17:24:26.280691 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-04-24 17:24:26.324692 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-04-24 17:24:26.384692 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-04-24 17:24:26.420693 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5167 2024-04-24 17:24:26.480693 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-04-24 17:24:26.564694 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-04-24 17:24:26.612694 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-04-24 17:24:26.720695 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-04-24 17:24:26.772696 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-04-24 17:24:26.820696 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-04-24 17:24:26.872697 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-04-24 17:24:26.952698 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-04-24 17:24:27.036698 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-04-24 17:24:27.112699 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-04-24 17:24:27.156700 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-04-24 17:24:27.236700 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-04-24 17:24:27.296701 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-04-24 17:24:27.360701 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-04-24 17:24:27.424702 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-04-24 17:24:27.484702 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-04-24 17:24:27.536703 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-04-24 17:24:27.592704 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-04-24 17:24:27.652704 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-04-24 17:24:27.688705 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-04-24 17:24:27.736705 ourskyai_astro_api-1.3.3442/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-04-24 17:24:27.804705 ourskyai_astro_api-1.3.3442/pyproject.toml
+-rw-r--r--   0        0        0    12025 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3442/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3368/README.md` & `ourskyai_astro_api-1.3.3442/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3368
-- Package version: 1.3.3368
+- API version: 1.3.3442
+- Package version: 1.3.3442
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3368"
+__version__ = "1.3.3442"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3368/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3442/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3368\n"\
-               "SDK Package Version: 1.3.3368".\
+               "Version of the API: 1.3.3442\n"\
+               "SDK Package Version: 1.3.3442".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/asset_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/filter_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/mount_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/shutter_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/successful_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/tracking_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_job_status.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_platform_credit_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_platform_credit_unit.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3368/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3442/ourskyai_astro_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3368/pyproject.toml` & `ourskyai_astro_api-1.3.3442/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3368"
+version = "1.3.3442"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3368/PKG-INFO` & `ourskyai_astro_api-1.3.3442/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3368
+Version: 1.3.3442
 Summary: OurSky Astro
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Astro
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-astro-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3368
-- Package version: 1.3.3368
+- API version: 1.3.3442
+- Package version: 1.3.3442
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

