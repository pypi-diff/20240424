# Comparing `tmp/ourskyai_platform_api-1.3.3368.tar.gz` & `tmp/ourskyai_platform_api-1.3.3442.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3368.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3442.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3368.tar` & `ourskyai_platform_api-1.3.3442.tar`

### file list

```diff
@@ -1,68 +1,72 @@
--rw-r--r--   0        0        0     8889 2024-04-18 04:36:56.096271 ourskyai_platform_api-1.3.3368/README.md
--rw-r--r--   0        0        0     5613 2024-04-18 04:36:59.540367 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-04-18 04:36:59.576368 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   185893 2024-04-18 04:36:59.660370 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-04-18 04:36:59.732373 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-04-18 04:36:59.784374 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-04-18 04:36:59.836376 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-04-18 04:36:59.892377 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     4942 2024-04-18 04:36:59.960379 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-04-18 04:37:00.020381 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-04-18 04:37:00.096383 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-04-18 04:37:00.144384 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     2158 2024-04-18 04:37:00.208386 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-04-18 04:37:00.256387 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-04-18 04:37:00.308389 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-04-18 04:37:00.356390 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-04-18 04:37:00.412392 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-04-18 04:37:00.460393 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-04-18 04:37:00.500394 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-04-18 04:37:00.564396 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-04-18 04:37:00.624397 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     4920 2024-04-18 04:37:00.680399 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-04-18 04:37:00.740401 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-04-18 04:37:00.788402 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-04-18 04:37:00.844404 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-04-18 04:37:00.912406 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-04-18 04:37:00.960407 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-04-18 04:37:00.996408 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2710 2024-04-18 04:37:01.052410 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-04-18 04:37:01.112411 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-04-18 04:37:01.160412 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-04-18 04:37:01.196413 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-04-18 04:37:01.272415 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-04-18 04:37:01.328417 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3298 2024-04-18 04:37:01.372418 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-04-18 04:37:01.432420 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-04-18 04:37:01.476421 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-04-18 04:37:01.528423 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-04-18 04:37:01.580424 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-04-18 04:37:01.624426 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-04-18 04:37:01.668427 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3985 2024-04-18 04:37:01.760429 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-04-18 04:37:01.820431 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5170 2024-04-18 04:37:01.868432 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3305 2024-04-18 04:37:01.936434 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-04-18 04:37:01.984435 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-04-18 04:37:02.032437 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-04-18 04:37:02.080438 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-04-18 04:37:02.128440 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1595 2024-04-18 04:37:02.172441 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-04-18 04:37:02.220442 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-04-18 04:37:02.260443 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-04-18 04:37:02.296444 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2054 2024-04-18 04:37:02.356446 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2053 2024-04-18 04:37:02.404447 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-04-18 04:37:02.452449 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-04-18 04:37:02.500450 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-04-18 04:37:02.560452 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-04-18 04:37:02.640454 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-04-18 04:37:02.700456 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-04-18 04:37:02.748457 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-04-18 04:37:02.796458 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-04-18 04:37:02.876460 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-04-18 04:37:02.924462 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-04-18 04:37:02.960463 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-04-18 04:37:03.012464 ourskyai_platform_api-1.3.3368/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-04-18 04:37:03.068466 ourskyai_platform_api-1.3.3368/pyproject.toml
--rw-r--r--   0        0        0     9866 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3368/PKG-INFO
+-rw-r--r--   0        0        0     9332 2024-04-24 17:24:19.940631 ourskyai_platform_api-1.3.3442/README.md
+-rw-r--r--   0        0        0     6036 2024-04-24 17:24:23.876668 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-24 17:24:23.904669 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   192993 2024-04-24 17:24:24.004670 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-04-24 17:24:24.064670 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-24 17:24:24.116671 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-04-24 17:24:24.156671 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-04-24 17:24:24.224672 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5365 2024-04-24 17:24:24.276672 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-24 17:24:24.328673 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-04-24 17:24:24.408673 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-04-24 17:24:24.460674 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     2158 2024-04-24 17:24:24.556675 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-04-24 17:24:24.620675 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-04-24 17:24:24.680676 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-04-24 17:24:24.752677 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-04-24 17:24:24.808677 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-04-24 17:24:24.872678 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-04-24 17:24:24.928678 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-04-24 17:24:24.996679 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-04-24 17:24:25.048679 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     4920 2024-04-24 17:24:25.108680 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-04-24 17:24:25.176681 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-04-24 17:24:25.232681 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-04-24 17:24:25.276682 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-04-24 17:24:25.336682 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-04-24 17:24:25.388683 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-04-24 17:24:25.428683 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2710 2024-04-24 17:24:25.528684 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-04-24 17:24:25.576685 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-04-24 17:24:25.644685 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-04-24 17:24:25.708686 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-04-24 17:24:25.760686 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-04-24 17:24:25.828687 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3298 2024-04-24 17:24:25.884687 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-04-24 17:24:25.948688 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-04-24 17:24:25.984688 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-04-24 17:24:26.080689 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-04-24 17:24:26.144690 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-04-24 17:24:26.216691 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-04-24 17:24:26.256691 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2902 2024-04-24 17:24:26.312692 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-04-24 17:24:26.368692 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-04-24 17:24:26.444693 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5170 2024-04-24 17:24:26.496693 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3305 2024-04-24 17:24:26.532693 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-04-24 17:24:26.588694 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-04-24 17:24:26.656695 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-04-24 17:24:26.692695 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-04-24 17:24:26.744696 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1595 2024-04-24 17:24:26.804696 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-04-24 17:24:26.852697 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-04-24 17:24:26.960698 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-04-24 17:24:27.016698 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-04-24 17:24:27.080699 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2097 2024-04-24 17:24:27.124699 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0      870 2024-04-24 17:24:27.200700 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_plate_solve_catalog_identifier.py
+-rw-r--r--   0        0        0     2054 2024-04-24 17:24:27.276701 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2053 2024-04-24 17:24:27.348701 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-04-24 17:24:27.412702 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-04-24 17:24:27.496703 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-04-24 17:24:27.544703 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-04-24 17:24:27.620704 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-04-24 17:24:27.668704 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-04-24 17:24:27.732705 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-04-24 17:24:27.792705 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-04-24 17:24:27.876706 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-04-24 17:24:27.924707 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-04-24 17:24:27.956707 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-04-24 17:24:27.996707 ourskyai_platform_api-1.3.3442/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-04-24 17:24:28.044708 ourskyai_platform_api-1.3.3442/pyproject.toml
+-rw-r--r--   0        0        0    10309 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3442/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3368/README.md` & `ourskyai_platform_api-1.3.3442/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
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
@@ -101,14 +101,15 @@
 *DefaultApi* | [**v1_get_node_diagnostic_tasks**](docs/DefaultApi.md#v1_get_node_diagnostic_tasks) | **GET** /v1/node-diagnostic-tasks | 
 *DefaultApi* | [**v1_get_node_properties**](docs/DefaultApi.md#v1_get_node_properties) | **GET** /v1/node-properties | 
 *DefaultApi* | [**v1_get_nodes**](docs/DefaultApi.md#v1_get_nodes) | **GET** /v1/nodes | 
 *DefaultApi* | [**v1_get_optical_tube**](docs/DefaultApi.md#v1_get_optical_tube) | **GET** /v1/optical-tube | 
 *DefaultApi* | [**v1_get_or_create_camera**](docs/DefaultApi.md#v1_get_or_create_camera) | **PUT** /v1/camera-match | 
 *DefaultApi* | [**v1_get_or_create_mount**](docs/DefaultApi.md#v1_get_or_create_mount) | **PUT** /v1/mount-match | 
 *DefaultApi* | [**v1_get_or_create_optical_tube**](docs/DefaultApi.md#v1_get_or_create_optical_tube) | **PUT** /v1/optical-tube-match | 
+*DefaultApi* | [**v1_get_plate_solve_catalog_diff**](docs/DefaultApi.md#v1_get_plate_solve_catalog_diff) | **PUT** /v1/plate-solve-catalog-diff | 
 *DefaultApi* | [**v1_mount_match**](docs/DefaultApi.md#v1_mount_match) | **GET** /v1/mount-match | 
 *DefaultApi* | [**v1_optical_tube_match**](docs/DefaultApi.md#v1_optical_tube_match) | **GET** /v1/optical-tube-match | 
 *DefaultApi* | [**v1_update_node**](docs/DefaultApi.md#v1_update_node) | **PUT** /v1/node | 
 *DefaultApi* | [**v1_update_node_components**](docs/DefaultApi.md#v1_update_node_components) | **PUT** /v1/node-components | 
 *DefaultApi* | [**v2_complete_observation**](docs/DefaultApi.md#v2_complete_observation) | **PUT** /v2/observation-complete | 
 
 
@@ -142,26 +143,30 @@
  - [V1GainCurve](docs/V1GainCurve.md)
  - [V1GainCurvePoint](docs/V1GainCurvePoint.md)
  - [V1GetInstructionRequest](docs/V1GetInstructionRequest.md)
  - [V1GetNodes](docs/V1GetNodes.md)
  - [V1GetOrCreateCameraRequest](docs/V1GetOrCreateCameraRequest.md)
  - [V1GetOrCreateMountRequest](docs/V1GetOrCreateMountRequest.md)
  - [V1GetOrCreateOpticalTubeRequest](docs/V1GetOrCreateOpticalTubeRequest.md)
+ - [V1GetPlateSolveCatalogDiffRequest](docs/V1GetPlateSolveCatalogDiffRequest.md)
  - [V1GroundStationParticipant](docs/V1GroundStationParticipant.md)
  - [V1ImageSet](docs/V1ImageSet.md)
  - [V1ImageSetImage](docs/V1ImageSetImage.md)
  - [V1Instruction](docs/V1Instruction.md)
  - [V1Metric](docs/V1Metric.md)
  - [V1Mount](docs/V1Mount.md)
  - [V1Node](docs/V1Node.md)
  - [V1NodeComponentType](docs/V1NodeComponentType.md)
  - [V1NodeDiagnosticType](docs/V1NodeDiagnosticType.md)
  - [V1NodeWithLocation](docs/V1NodeWithLocation.md)
  - [V1ObservationInstruction](docs/V1ObservationInstruction.md)
  - [V1OpticalTube](docs/V1OpticalTube.md)
+ - [V1PlateSolveCatalogFile](docs/V1PlateSolveCatalogFile.md)
+ - [V1PlateSolveCatalogFileDownload](docs/V1PlateSolveCatalogFileDownload.md)
+ - [V1PlateSolveCatalogIdentifier](docs/V1PlateSolveCatalogIdentifier.md)
  - [V1ReadNoisePoint](docs/V1ReadNoisePoint.md)
  - [V1SetupAction](docs/V1SetupAction.md)
  - [V1SlewTiming](docs/V1SlewTiming.md)
  - [V1SlewTimingInterval](docs/V1SlewTimingInterval.md)
  - [V1UpdateNodeComponentsRequest](docs/V1UpdateNodeComponentsRequest.md)
  - [V1UpdateNodeComponentsRequestCamera](docs/V1UpdateNodeComponentsRequestCamera.md)
  - [V1UpdateNodeComponentsRequestMount](docs/V1UpdateNodeComponentsRequestMount.md)
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3368"
+__version__ = "1.3.3442"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
@@ -59,26 +59,30 @@
 from ourskyai_platform_api.models.v1_gain_curve import V1GainCurve
 from ourskyai_platform_api.models.v1_gain_curve_point import V1GainCurvePoint
 from ourskyai_platform_api.models.v1_get_instruction_request import V1GetInstructionRequest
 from ourskyai_platform_api.models.v1_get_nodes import V1GetNodes
 from ourskyai_platform_api.models.v1_get_or_create_camera_request import V1GetOrCreateCameraRequest
 from ourskyai_platform_api.models.v1_get_or_create_mount_request import V1GetOrCreateMountRequest
 from ourskyai_platform_api.models.v1_get_or_create_optical_tube_request import V1GetOrCreateOpticalTubeRequest
+from ourskyai_platform_api.models.v1_get_plate_solve_catalog_diff_request import V1GetPlateSolveCatalogDiffRequest
 from ourskyai_platform_api.models.v1_ground_station_participant import V1GroundStationParticipant
 from ourskyai_platform_api.models.v1_image_set import V1ImageSet
 from ourskyai_platform_api.models.v1_image_set_image import V1ImageSetImage
 from ourskyai_platform_api.models.v1_instruction import V1Instruction
 from ourskyai_platform_api.models.v1_metric import V1Metric
 from ourskyai_platform_api.models.v1_mount import V1Mount
 from ourskyai_platform_api.models.v1_node import V1Node
 from ourskyai_platform_api.models.v1_node_component_type import V1NodeComponentType
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_node_with_location import V1NodeWithLocation
 from ourskyai_platform_api.models.v1_observation_instruction import V1ObservationInstruction
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
+from ourskyai_platform_api.models.v1_plate_solve_catalog_file import V1PlateSolveCatalogFile
+from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
+from ourskyai_platform_api.models.v1_plate_solve_catalog_identifier import V1PlateSolveCatalogIdentifier
 from ourskyai_platform_api.models.v1_read_noise_point import V1ReadNoisePoint
 from ourskyai_platform_api.models.v1_setup_action import V1SetupAction
 from ourskyai_platform_api.models.v1_slew_timing import V1SlewTiming
 from ourskyai_platform_api.models.v1_slew_timing_interval import V1SlewTimingInterval
 from ourskyai_platform_api.models.v1_update_node_components_request import V1UpdateNodeComponentsRequest
 from ourskyai_platform_api.models.v1_update_node_components_request_camera import V1UpdateNodeComponentsRequestCamera
 from ourskyai_platform_api.models.v1_update_node_components_request_mount import V1UpdateNodeComponentsRequestMount
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/api/default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
@@ -35,23 +35,25 @@
 from ourskyai_platform_api.models.v1_create_node_request import V1CreateNodeRequest
 from ourskyai_platform_api.models.v1_create_optical_tube_request import V1CreateOpticalTubeRequest
 from ourskyai_platform_api.models.v1_get_instruction_request import V1GetInstructionRequest
 from ourskyai_platform_api.models.v1_get_nodes import V1GetNodes
 from ourskyai_platform_api.models.v1_get_or_create_camera_request import V1GetOrCreateCameraRequest
 from ourskyai_platform_api.models.v1_get_or_create_mount_request import V1GetOrCreateMountRequest
 from ourskyai_platform_api.models.v1_get_or_create_optical_tube_request import V1GetOrCreateOpticalTubeRequest
+from ourskyai_platform_api.models.v1_get_plate_solve_catalog_diff_request import V1GetPlateSolveCatalogDiffRequest
 from ourskyai_platform_api.models.v1_ground_station_participant import V1GroundStationParticipant
 from ourskyai_platform_api.models.v1_image_set import V1ImageSet
 from ourskyai_platform_api.models.v1_image_set_image import V1ImageSetImage
 from ourskyai_platform_api.models.v1_instruction import V1Instruction
 from ourskyai_platform_api.models.v1_metric import V1Metric
 from ourskyai_platform_api.models.v1_mount import V1Mount
 from ourskyai_platform_api.models.v1_node import V1Node
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
+from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
 from ourskyai_platform_api.models.v1_update_node_components_request import V1UpdateNodeComponentsRequest
 from ourskyai_platform_api.models.v1_update_node_request import V1UpdateNodeRequest
 from ourskyai_platform_api.models.v2_complete_observation_request import V2CompleteObservationRequest
 
 from ourskyai_platform_api.api_client import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.exceptions import (  # noqa: F401
@@ -3545,14 +3547,161 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def v1_get_plate_solve_catalog_diff(self, v1_get_plate_solve_catalog_diff_request : V1GetPlateSolveCatalogDiffRequest, **kwargs) -> List[V1PlateSolveCatalogFileDownload]:  # noqa: E501
+        """v1_get_plate_solve_catalog_diff  # noqa: E501
+
+        Get a diff of plate solve catalog files.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_plate_solve_catalog_diff(v1_get_plate_solve_catalog_diff_request, async_req=True)
+        >>> result = thread.get()
+
+        :param v1_get_plate_solve_catalog_diff_request: (required)
+        :type v1_get_plate_solve_catalog_diff_request: V1GetPlateSolveCatalogDiffRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: List[V1PlateSolveCatalogFileDownload]
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the v1_get_plate_solve_catalog_diff_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.v1_get_plate_solve_catalog_diff_with_http_info(v1_get_plate_solve_catalog_diff_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def v1_get_plate_solve_catalog_diff_with_http_info(self, v1_get_plate_solve_catalog_diff_request : V1GetPlateSolveCatalogDiffRequest, **kwargs) -> ApiResponse:  # noqa: E501
+        """v1_get_plate_solve_catalog_diff  # noqa: E501
+
+        Get a diff of plate solve catalog files.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_get_plate_solve_catalog_diff_with_http_info(v1_get_plate_solve_catalog_diff_request, async_req=True)
+        >>> result = thread.get()
+
+        :param v1_get_plate_solve_catalog_diff_request: (required)
+        :type v1_get_plate_solve_catalog_diff_request: V1GetPlateSolveCatalogDiffRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(List[V1PlateSolveCatalogFileDownload], status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'v1_get_plate_solve_catalog_diff_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_get_plate_solve_catalog_diff" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['v1_get_plate_solve_catalog_diff_request'] is not None:
+            _body_params = _params['v1_get_plate_solve_catalog_diff_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['Roles', 'BearerToken']  # noqa: E501
+
+        _response_types_map = {
+            '200': "List[V1PlateSolveCatalogFileDownload]",
+        }
+
+        return self.api_client.call_api(
+            '/v1/plate-solve-catalog-diff', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
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

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
@@ -42,26 +42,30 @@
 from ourskyai_platform_api.models.v1_gain_curve import V1GainCurve
 from ourskyai_platform_api.models.v1_gain_curve_point import V1GainCurvePoint
 from ourskyai_platform_api.models.v1_get_instruction_request import V1GetInstructionRequest
 from ourskyai_platform_api.models.v1_get_nodes import V1GetNodes
 from ourskyai_platform_api.models.v1_get_or_create_camera_request import V1GetOrCreateCameraRequest
 from ourskyai_platform_api.models.v1_get_or_create_mount_request import V1GetOrCreateMountRequest
 from ourskyai_platform_api.models.v1_get_or_create_optical_tube_request import V1GetOrCreateOpticalTubeRequest
+from ourskyai_platform_api.models.v1_get_plate_solve_catalog_diff_request import V1GetPlateSolveCatalogDiffRequest
 from ourskyai_platform_api.models.v1_ground_station_participant import V1GroundStationParticipant
 from ourskyai_platform_api.models.v1_image_set import V1ImageSet
 from ourskyai_platform_api.models.v1_image_set_image import V1ImageSetImage
 from ourskyai_platform_api.models.v1_instruction import V1Instruction
 from ourskyai_platform_api.models.v1_metric import V1Metric
 from ourskyai_platform_api.models.v1_mount import V1Mount
 from ourskyai_platform_api.models.v1_node import V1Node
 from ourskyai_platform_api.models.v1_node_component_type import V1NodeComponentType
 from ourskyai_platform_api.models.v1_node_diagnostic_type import V1NodeDiagnosticType
 from ourskyai_platform_api.models.v1_node_with_location import V1NodeWithLocation
 from ourskyai_platform_api.models.v1_observation_instruction import V1ObservationInstruction
 from ourskyai_platform_api.models.v1_optical_tube import V1OpticalTube
+from ourskyai_platform_api.models.v1_plate_solve_catalog_file import V1PlateSolveCatalogFile
+from ourskyai_platform_api.models.v1_plate_solve_catalog_file_download import V1PlateSolveCatalogFileDownload
+from ourskyai_platform_api.models.v1_plate_solve_catalog_identifier import V1PlateSolveCatalogIdentifier
 from ourskyai_platform_api.models.v1_read_noise_point import V1ReadNoisePoint
 from ourskyai_platform_api.models.v1_setup_action import V1SetupAction
 from ourskyai_platform_api.models.v1_slew_timing import V1SlewTiming
 from ourskyai_platform_api.models.v1_slew_timing_interval import V1SlewTimingInterval
 from ourskyai_platform_api.models.v1_update_node_components_request import V1UpdateNodeComponentsRequest
 from ourskyai_platform_api.models.v1_update_node_components_request_camera import V1UpdateNodeComponentsRequestCamera
 from ourskyai_platform_api.models.v1_update_node_components_request_mount import V1UpdateNodeComponentsRequestMount
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/camera_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/empty_success.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/metric_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/mount_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/node_state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/shutter_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/successful_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/tracking_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class V1CompleteObservationRequest(BaseModel):
+class V2CompleteObservationRequest(BaseModel):
     """
-    V1CompleteObservationRequest
+    V2CompleteObservationRequest
     """
     image_set_id: StrictStr = Field(..., alias="imageSetId")
-    __properties = ["imageSetId"]
+    expected_image_count: StrictInt = Field(..., alias="expectedImageCount")
+    __properties = ["imageSetId", "expectedImageCount"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -38,34 +39,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1CompleteObservationRequest:
-        """Create an instance of V1CompleteObservationRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> V2CompleteObservationRequest:
+        """Create an instance of V2CompleteObservationRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V1CompleteObservationRequest:
-        """Create an instance of V1CompleteObservationRequest from a dict"""
+    def from_dict(cls, obj: dict) -> V2CompleteObservationRequest:
+        """Create an instance of V2CompleteObservationRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return V1CompleteObservationRequest.parse_obj(obj)
+            return V2CompleteObservationRequest.parse_obj(obj)
 
-        _obj = V1CompleteObservationRequest.parse_obj({
-            "image_set_id": obj.get("imageSetId")
+        _obj = V2CompleteObservationRequest.parse_obj({
+            "image_set_id": obj.get("imageSetId"),
+            "expected_image_count": obj.get("expectedImageCount")
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_component_type.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_plate_solve_catalog_identifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,26 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1NodeComponentType(str, Enum):
+class V1PlateSolveCatalogIdentifier(str, Enum):
     """
-    V1NodeComponentType
+    V1PlateSolveCatalogIdentifier
     """
 
     """
     allowed enum values
     """
-    CAMERA = 'CAMERA'
-    MOUNT = 'MOUNT'
-    OPTICAL_TUBE = 'OPTICAL_TUBE'
-    COMPUTER = 'COMPUTER'
+    TWO_MASS_4100 = 'TWO_MASS_4100'
+    TWO_MASS_LITE = 'TWO_MASS_LITE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1NodeComponentType:
-        """Create an instance of V1NodeComponentType from a JSON string"""
-        return V1NodeComponentType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1PlateSolveCatalogIdentifier:
+        """Create an instance of V1PlateSolveCatalogIdentifier from a JSON string"""
+        return V1PlateSolveCatalogIdentifier(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
-class V2CompleteObservationRequest(BaseModel):
+class V1CompleteObservationRequest(BaseModel):
     """
-    V2CompleteObservationRequest
+    V1CompleteObservationRequest
     """
     image_set_id: StrictStr = Field(..., alias="imageSetId")
-    expected_image_count: StrictInt = Field(..., alias="expectedImageCount")
-    __properties = ["imageSetId", "expectedImageCount"]
+    __properties = ["imageSetId"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,35 +38,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> V2CompleteObservationRequest:
-        """Create an instance of V2CompleteObservationRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> V1CompleteObservationRequest:
+        """Create an instance of V1CompleteObservationRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> V2CompleteObservationRequest:
-        """Create an instance of V2CompleteObservationRequest from a dict"""
+    def from_dict(cls, obj: dict) -> V1CompleteObservationRequest:
+        """Create an instance of V1CompleteObservationRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return V2CompleteObservationRequest.parse_obj(obj)
+            return V1CompleteObservationRequest.parse_obj(obj)
 
-        _obj = V2CompleteObservationRequest.parse_obj({
-            "image_set_id": obj.get("imageSetId"),
-            "expected_image_count": obj.get("expectedImageCount")
+        _obj = V1CompleteObservationRequest.parse_obj({
+            "image_set_id": obj.get("imageSetId")
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3368/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3442/ourskyai_platform_api/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3368
+    The version of the OpenAPI document: 1.3.3442
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3368/pyproject.toml` & `ourskyai_platform_api-1.3.3442/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3368"
+version = "1.3.3442"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3368/PKG-INFO` & `ourskyai_platform_api-1.3.3442/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3368
+Version: 1.3.3442
 Summary: OurSky Platform
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-platform-api
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
@@ -126,14 +126,15 @@
 *DefaultApi* | [**v1_get_node_diagnostic_tasks**](docs/DefaultApi.md#v1_get_node_diagnostic_tasks) | **GET** /v1/node-diagnostic-tasks | 
 *DefaultApi* | [**v1_get_node_properties**](docs/DefaultApi.md#v1_get_node_properties) | **GET** /v1/node-properties | 
 *DefaultApi* | [**v1_get_nodes**](docs/DefaultApi.md#v1_get_nodes) | **GET** /v1/nodes | 
 *DefaultApi* | [**v1_get_optical_tube**](docs/DefaultApi.md#v1_get_optical_tube) | **GET** /v1/optical-tube | 
 *DefaultApi* | [**v1_get_or_create_camera**](docs/DefaultApi.md#v1_get_or_create_camera) | **PUT** /v1/camera-match | 
 *DefaultApi* | [**v1_get_or_create_mount**](docs/DefaultApi.md#v1_get_or_create_mount) | **PUT** /v1/mount-match | 
 *DefaultApi* | [**v1_get_or_create_optical_tube**](docs/DefaultApi.md#v1_get_or_create_optical_tube) | **PUT** /v1/optical-tube-match | 
+*DefaultApi* | [**v1_get_plate_solve_catalog_diff**](docs/DefaultApi.md#v1_get_plate_solve_catalog_diff) | **PUT** /v1/plate-solve-catalog-diff | 
 *DefaultApi* | [**v1_mount_match**](docs/DefaultApi.md#v1_mount_match) | **GET** /v1/mount-match | 
 *DefaultApi* | [**v1_optical_tube_match**](docs/DefaultApi.md#v1_optical_tube_match) | **GET** /v1/optical-tube-match | 
 *DefaultApi* | [**v1_update_node**](docs/DefaultApi.md#v1_update_node) | **PUT** /v1/node | 
 *DefaultApi* | [**v1_update_node_components**](docs/DefaultApi.md#v1_update_node_components) | **PUT** /v1/node-components | 
 *DefaultApi* | [**v2_complete_observation**](docs/DefaultApi.md#v2_complete_observation) | **PUT** /v2/observation-complete | 
 
 
@@ -167,26 +168,30 @@
  - [V1GainCurve](docs/V1GainCurve.md)
  - [V1GainCurvePoint](docs/V1GainCurvePoint.md)
  - [V1GetInstructionRequest](docs/V1GetInstructionRequest.md)
  - [V1GetNodes](docs/V1GetNodes.md)
  - [V1GetOrCreateCameraRequest](docs/V1GetOrCreateCameraRequest.md)
  - [V1GetOrCreateMountRequest](docs/V1GetOrCreateMountRequest.md)
  - [V1GetOrCreateOpticalTubeRequest](docs/V1GetOrCreateOpticalTubeRequest.md)
+ - [V1GetPlateSolveCatalogDiffRequest](docs/V1GetPlateSolveCatalogDiffRequest.md)
  - [V1GroundStationParticipant](docs/V1GroundStationParticipant.md)
  - [V1ImageSet](docs/V1ImageSet.md)
  - [V1ImageSetImage](docs/V1ImageSetImage.md)
  - [V1Instruction](docs/V1Instruction.md)
  - [V1Metric](docs/V1Metric.md)
  - [V1Mount](docs/V1Mount.md)
  - [V1Node](docs/V1Node.md)
  - [V1NodeComponentType](docs/V1NodeComponentType.md)
  - [V1NodeDiagnosticType](docs/V1NodeDiagnosticType.md)
  - [V1NodeWithLocation](docs/V1NodeWithLocation.md)
  - [V1ObservationInstruction](docs/V1ObservationInstruction.md)
  - [V1OpticalTube](docs/V1OpticalTube.md)
+ - [V1PlateSolveCatalogFile](docs/V1PlateSolveCatalogFile.md)
+ - [V1PlateSolveCatalogFileDownload](docs/V1PlateSolveCatalogFileDownload.md)
+ - [V1PlateSolveCatalogIdentifier](docs/V1PlateSolveCatalogIdentifier.md)
  - [V1ReadNoisePoint](docs/V1ReadNoisePoint.md)
  - [V1SetupAction](docs/V1SetupAction.md)
  - [V1SlewTiming](docs/V1SlewTiming.md)
  - [V1SlewTimingInterval](docs/V1SlewTimingInterval.md)
  - [V1UpdateNodeComponentsRequest](docs/V1UpdateNodeComponentsRequest.md)
  - [V1UpdateNodeComponentsRequestCamera](docs/V1UpdateNodeComponentsRequestCamera.md)
  - [V1UpdateNodeComponentsRequestMount](docs/V1UpdateNodeComponentsRequestMount.md)
```

