# Comparing `tmp/lifx-photons-core-0.9.4.tar.gz` & `tmp/lifx-photons-core-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lifx-photons-core-0.9.4.tar", last modified: Thu Jan  3 03:11:26 2019, max compression
+gzip compressed data, was "dist/lifx-photons-core-0.9.5.tar", last modified: Mon Jan 21 04:28:48 2019, max compression
```

## Comparing `lifx-photons-core-0.9.4.tar` & `lifx-photons-core-0.9.5.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      626 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/PKG-INFO
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_control/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     5998 2018-12-31 06:26:03.000000 lifx-photons-core-0.9.4/photons_control/tile.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      637 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_control/addon.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3576 2018-11-10 02:13:28.000000 lifx-photons-core-0.9.4/photons_control/attributes.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      436 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_control/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2350 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.4/photons_control/multizone.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     5507 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.4/photons_control/transform.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2516 2018-11-10 02:13:28.000000 lifx-photons-core-0.9.4/photons_control/payloads.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    11777 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_control/script.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      937 2018-11-10 02:13:28.000000 lifx-photons-core-0.9.4/photons_control/colour.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     6856 2018-11-10 02:12:53.000000 lifx-photons-core-0.9.4/photons_products_registry.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_app/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     7368 2018-11-28 01:46:46.000000 lifx-photons-core-0.9.4/photons_app/registers.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2000 2018-12-26 11:09:30.000000 lifx-photons-core-0.9.4/photons_app/runner.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3459 2018-11-28 09:53:20.000000 lifx-photons-core-0.9.4/photons_app/formatter.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_app/option_spec/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     5173 2018-12-26 10:58:10.000000 lifx-photons-core-0.9.4/photons_app/option_spec/photons_app_spec.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_app/option_spec/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     5683 2018-11-28 01:32:45.000000 lifx-photons-core-0.9.4/photons_app/option_spec/task_objs.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    10339 2018-11-28 09:53:20.000000 lifx-photons-core-0.9.4/photons_app/collector.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     7891 2018-11-28 01:35:23.000000 lifx-photons-core-0.9.4/photons_app/actions.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1137 2019-01-03 03:10:56.000000 lifx-photons-core-0.9.4/photons_app/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      739 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_app/task_finder.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_app/sphinx/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3682 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_app/sphinx/tasks.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_app/sphinx/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1571 2018-11-10 02:13:28.000000 lifx-photons-core-0.9.4/photons_app/sphinx/docstrings.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1445 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_app/sphinx/code_for.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1181 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_app/sphinx/target_fields.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     4924 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_app/sphinx/structures.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     5962 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_app/test_helpers.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2036 2018-11-28 01:31:25.000000 lifx-photons-core-0.9.4/photons_app/errors.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    24537 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_app/helpers.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     4883 2018-11-28 01:50:52.000000 lifx-photons-core-0.9.4/photons_app/special.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     6987 2018-11-28 01:41:39.000000 lifx-photons-core-0.9.4/photons_app/executor.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    13011 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.4/photons_colour.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    43140 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.4/photons_device_finder.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2023 2018-11-28 02:06:28.000000 lifx-photons-core-0.9.4/setup.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_transport/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1006 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_transport/addon.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_transport/target/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     8008 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_transport/target/bridge.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2682 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_transport/target/receiver.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1441 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_transport/target/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3913 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_transport/target/waiter.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     5070 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_transport/target/result.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2555 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_transport/target/retry_options.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     6200 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_transport/target/target.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     9034 2018-12-22 09:44:49.000000 lifx-photons-core-0.9.4/photons_transport/target/writer.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      292 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_transport/target/errors.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2357 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_transport/target/script.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    11442 2018-12-22 09:47:31.000000 lifx-photons-core-0.9.4/photons_transport/target/item.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      248 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_transport/__init__.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_protocol/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      208 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_protocol/addon.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      337 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_protocol/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    36299 2018-12-22 11:07:10.000000 lifx-photons-core-0.9.4/photons_protocol/types.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     7235 2018-11-17 23:07:44.000000 lifx-photons-core-0.9.4/photons_protocol/packing.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     8398 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_protocol/messages.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      362 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_protocol/errors.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    19507 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_protocol/packets.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      523 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_core.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)       38 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/setup.cfg
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_themes/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     7621 2018-12-27 03:36:43.000000 lifx-photons-core-0.9.4/photons_themes/addon.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     4891 2018-12-22 03:08:13.000000 lifx-photons-core-0.9.4/photons_themes/theme.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      700 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_themes/coords.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_themes/appliers/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      494 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_themes/appliers/single.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2037 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_themes/appliers/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     4215 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_themes/appliers/splotch.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2348 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_themes/appliers/stripes.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3754 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_themes/appliers/base.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      474 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_themes/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2697 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_themes/collections.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    10928 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_themes/canvas.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_messages/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      324 2018-11-10 02:12:53.000000 lifx-photons-core-0.9.4/photons_messages/addon.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      318 2019-01-03 00:26:49.000000 lifx-photons-core-0.9.4/photons_messages/enums.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2307 2019-01-03 00:26:55.000000 lifx-photons-core-0.9.4/photons_messages/fields.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      906 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.4/photons_messages/__init__.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_messages/sphinx/
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_messages/sphinx/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2753 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_messages/sphinx/messages.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     6309 2018-11-17 23:40:12.000000 lifx-photons-core-0.9.4/photons_messages/frame.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     7058 2019-01-03 00:26:49.000000 lifx-photons-core-0.9.4/photons_messages/messages.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      245 2018-02-26 04:52:14.000000 lifx-photons-core-0.9.4/README.rst
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_socket/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      762 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.4/photons_socket/addon.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     6427 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.4/photons_socket/fake.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      749 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.4/photons_socket/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     5201 2018-11-27 04:46:13.000000 lifx-photons-core-0.9.4/photons_socket/connection.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     4550 2018-11-27 04:46:33.000000 lifx-photons-core-0.9.4/photons_socket/target.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_tile_paint/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1225 2018-12-29 23:45:09.000000 lifx-photons-core-0.9.4/photons_tile_paint/options.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     4398 2018-12-26 01:21:17.000000 lifx-photons-core-0.9.4/photons_tile_paint/addon.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_tile_paint/pacman/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      468 2018-12-30 00:07:39.000000 lifx-photons-core-0.9.4/photons_tile_paint/pacman/options.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/pacman/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2092 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/pacman/font.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      885 2018-12-30 00:42:59.000000 lifx-photons-core-0.9.4/photons_tile_paint/pacman/animation.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2553 2018-12-30 00:34:05.000000 lifx-photons-core-0.9.4/photons_tile_paint/pacman/state.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2019 2018-12-27 02:59:01.000000 lifx-photons-core-0.9.4/photons_tile_paint/orientation.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     4546 2018-12-29 23:46:32.000000 lifx-photons-core-0.9.4/photons_tile_paint/twinkles.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      238 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2472 2018-12-29 23:46:16.000000 lifx-photons-core-0.9.4/photons_tile_paint/dice.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2138 2018-12-30 00:07:56.000000 lifx-photons-core-0.9.4/photons_tile_paint/nyan.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_tile_paint/marquee/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      915 2018-12-30 00:06:28.000000 lifx-photons-core-0.9.4/photons_tile_paint/marquee/options.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/marquee/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2863 2018-12-30 00:24:19.000000 lifx-photons-core-0.9.4/photons_tile_paint/marquee/animation.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_tile_paint/time/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      460 2018-12-29 23:46:45.000000 lifx-photons-core-0.9.4/photons_tile_paint/time/options.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/time/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1615 2018-12-24 22:41:59.000000 lifx-photons-core-0.9.4/photons_tile_paint/time/animation.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     9010 2018-12-30 00:11:01.000000 lifx-photons-core-0.9.4/photons_tile_paint/animation.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     7964 2018-12-29 23:17:52.000000 lifx-photons-core-0.9.4/photons_tile_paint/set_state.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      916 2018-12-29 23:47:16.000000 lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/options.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1557 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/font.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      736 2018-12-30 00:42:40.000000 lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/animation.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3013 2018-12-23 02:09:32.000000 lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/state.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/photons_tile_paint/font/
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/font/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1003 2019-01-02 05:41:04.000000 lifx-photons-core-0.9.4/photons_tile_paint/font/dice.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    12766 2018-12-22 06:12:43.000000 lifx-photons-core-0.9.4/photons_tile_paint/font/alphabet.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)      736 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.4/photons_tile_paint/font/base.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     8247 2018-12-29 23:46:03.000000 lifx-photons-core-0.9.4/photons_tile_paint/falling.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/lifx_photons_core.egg-info/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      626 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/lifx_photons_core.egg-info/PKG-INFO
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3583 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/lifx_photons_core.egg-info/SOURCES.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)      435 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/lifx_photons_core.egg-info/entry_points.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)      205 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/lifx_photons_core.egg-info/requires.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)      205 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/lifx_photons_core.egg-info/top_level.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)        1 2019-01-03 03:11:26.000000 lifx-photons-core-0.9.4/lifx_photons_core.egg-info/dependency_links.txt
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:48.000000 lifx-photons-core-0.9.5/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      626 2019-01-21 04:28:48.000000 lifx-photons-core-0.9.5/PKG-INFO
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_control/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5998 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_control/tile.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      637 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_control/addon.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3576 2019-01-16 22:08:34.000000 lifx-photons-core-0.9.5/photons_control/attributes.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      436 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_control/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2350 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.5/photons_control/multizone.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5507 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.5/photons_control/transform.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2516 2018-11-10 02:13:28.000000 lifx-photons-core-0.9.5/photons_control/payloads.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    11777 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_control/script.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      937 2018-11-10 02:13:28.000000 lifx-photons-core-0.9.5/photons_control/colour.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     6856 2018-11-10 02:12:53.000000 lifx-photons-core-0.9.5/photons_products_registry.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_app/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7368 2018-11-28 01:46:46.000000 lifx-photons-core-0.9.5/photons_app/registers.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2000 2018-12-26 11:09:30.000000 lifx-photons-core-0.9.5/photons_app/runner.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3459 2018-11-28 09:53:20.000000 lifx-photons-core-0.9.5/photons_app/formatter.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_app/option_spec/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5173 2018-12-26 10:58:10.000000 lifx-photons-core-0.9.5/photons_app/option_spec/photons_app_spec.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_app/option_spec/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5683 2018-11-28 01:32:45.000000 lifx-photons-core-0.9.5/photons_app/option_spec/task_objs.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    10339 2018-11-28 09:53:20.000000 lifx-photons-core-0.9.5/photons_app/collector.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7891 2018-11-28 01:35:23.000000 lifx-photons-core-0.9.5/photons_app/actions.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1137 2019-01-21 04:26:05.000000 lifx-photons-core-0.9.5/photons_app/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      739 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_app/task_finder.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_app/sphinx/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3682 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_app/sphinx/tasks.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_app/sphinx/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1571 2018-11-10 02:13:28.000000 lifx-photons-core-0.9.5/photons_app/sphinx/docstrings.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1445 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_app/sphinx/code_for.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1181 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_app/sphinx/target_fields.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     4924 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_app/sphinx/structures.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5962 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_app/test_helpers.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2036 2018-11-28 01:31:25.000000 lifx-photons-core-0.9.5/photons_app/errors.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    24537 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_app/helpers.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     4883 2018-11-28 01:50:52.000000 lifx-photons-core-0.9.5/photons_app/special.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     6987 2018-11-28 01:41:39.000000 lifx-photons-core-0.9.5/photons_app/executor.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    13094 2019-01-17 23:11:02.000000 lifx-photons-core-0.9.5/photons_colour.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    43140 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.5/photons_device_finder.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2023 2018-11-28 02:06:28.000000 lifx-photons-core-0.9.5/setup.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:48.000000 lifx-photons-core-0.9.5/photons_transport/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1006 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_transport/addon.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:48.000000 lifx-photons-core-0.9.5/photons_transport/target/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     8008 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_transport/target/bridge.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2682 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_transport/target/receiver.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1441 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_transport/target/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3913 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_transport/target/waiter.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5070 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_transport/target/result.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2555 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_transport/target/retry_options.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     6200 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_transport/target/target.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     9034 2018-12-22 09:44:49.000000 lifx-photons-core-0.9.5/photons_transport/target/writer.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      292 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_transport/target/errors.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2357 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_transport/target/script.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    11442 2019-01-16 06:18:06.000000 lifx-photons-core-0.9.5/photons_transport/target/item.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      248 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_transport/__init__.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_protocol/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      208 2019-01-12 01:40:12.000000 lifx-photons-core-0.9.5/photons_protocol/addon.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      337 2019-01-12 01:40:12.000000 lifx-photons-core-0.9.5/photons_protocol/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    37888 2019-01-12 01:40:12.000000 lifx-photons-core-0.9.5/photons_protocol/types.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7235 2019-01-12 01:40:12.000000 lifx-photons-core-0.9.5/photons_protocol/packing.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     8398 2019-01-12 01:40:12.000000 lifx-photons-core-0.9.5/photons_protocol/messages.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      362 2019-01-12 01:40:12.000000 lifx-photons-core-0.9.5/photons_protocol/errors.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    19507 2019-01-12 01:40:12.000000 lifx-photons-core-0.9.5/photons_protocol/packets.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      523 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_core.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)       38 2019-01-21 04:28:48.000000 lifx-photons-core-0.9.5/setup.cfg
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_themes/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7621 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_themes/addon.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5436 2019-01-08 11:00:37.000000 lifx-photons-core-0.9.5/photons_themes/theme.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      700 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_themes/coords.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_themes/appliers/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      494 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_themes/appliers/single.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2037 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_themes/appliers/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     4215 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_themes/appliers/splotch.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2348 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_themes/appliers/stripes.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3754 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_themes/appliers/base.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      474 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_themes/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2697 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_themes/collections.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    10928 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_themes/canvas.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_messages/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      324 2018-11-10 02:12:53.000000 lifx-photons-core-0.9.5/photons_messages/addon.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      318 2019-01-17 23:01:39.000000 lifx-photons-core-0.9.5/photons_messages/enums.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2340 2019-01-17 23:01:39.000000 lifx-photons-core-0.9.5/photons_messages/fields.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      906 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.5/photons_messages/__init__.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_messages/sphinx/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_messages/sphinx/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2753 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_messages/sphinx/messages.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     6309 2018-11-17 23:40:12.000000 lifx-photons-core-0.9.5/photons_messages/frame.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7058 2019-01-17 23:01:39.000000 lifx-photons-core-0.9.5/photons_messages/messages.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      245 2018-02-26 04:52:14.000000 lifx-photons-core-0.9.5/README.rst
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_socket/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      762 2018-11-10 02:06:43.000000 lifx-photons-core-0.9.5/photons_socket/addon.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     6427 2018-12-17 00:22:18.000000 lifx-photons-core-0.9.5/photons_socket/fake.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      749 2018-11-29 03:34:38.000000 lifx-photons-core-0.9.5/photons_socket/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5201 2018-11-27 04:46:13.000000 lifx-photons-core-0.9.5/photons_socket/connection.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     4550 2018-11-27 04:46:33.000000 lifx-photons-core-0.9.5/photons_socket/target.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_tile_paint/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     4248 2019-01-08 21:56:23.000000 lifx-photons-core-0.9.5/photons_tile_paint/options.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     4636 2019-01-08 21:56:25.000000 lifx-photons-core-0.9.5/photons_tile_paint/addon.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_tile_paint/pacman/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      468 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/pacman/options.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/pacman/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2092 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/pacman/font.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      885 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/pacman/animation.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2553 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/pacman/state.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2019 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/orientation.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     4546 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/twinkles.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      238 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2618 2019-01-06 06:30:53.000000 lifx-photons-core-0.9.5/photons_tile_paint/dice.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2138 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/nyan.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_tile_paint/marquee/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      915 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/marquee/options.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/marquee/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2863 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/marquee/animation.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7520 2019-01-12 04:40:30.000000 lifx-photons-core-0.9.5/photons_tile_paint/balls.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:48.000000 lifx-photons-core-0.9.5/photons_tile_paint/time/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      460 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/time/options.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/time/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1615 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/time/animation.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     9010 2019-01-06 01:19:17.000000 lifx-photons-core-0.9.5/photons_tile_paint/animation.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7915 2019-01-08 11:00:37.000000 lifx-photons-core-0.9.5/photons_tile_paint/set_state.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      916 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/options.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1557 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/font.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      736 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/animation.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3013 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/state.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/photons_tile_paint/font/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/font/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1003 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/font/dice.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    12766 2019-01-05 23:38:45.000000 lifx-photons-core-0.9.5/photons_tile_paint/font/alphabet.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      736 2018-11-10 02:07:07.000000 lifx-photons-core-0.9.5/photons_tile_paint/font/base.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7153 2019-01-08 21:56:23.000000 lifx-photons-core-0.9.5/photons_tile_paint/falling.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/lifx_photons_core.egg-info/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      626 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/lifx_photons_core.egg-info/PKG-INFO
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3611 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/lifx_photons_core.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      435 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/lifx_photons_core.egg-info/entry_points.txt
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      205 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/lifx_photons_core.egg-info/requires.txt
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      205 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/lifx_photons_core.egg-info/top_level.txt
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        1 2019-01-21 04:28:47.000000 lifx-photons-core-0.9.5/lifx_photons_core.egg-info/dependency_links.txt
```

### Comparing `lifx-photons-core-0.9.4/PKG-INFO` & `lifx-photons-core-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-photons-core
-Version: 0.9.4
+Version: 0.9.5
 Summary: The core modules of the photons framework
 Home-page: http://github.com/delfick/photons-core
 Author: Stephen Moore
 Author-email: delfick755@gmail.com
 License: MIT
 Description: Photons
         =======
```

### Comparing `lifx-photons-core-0.9.4/photons_control/tile.py` & `lifx-photons-core-0.9.5/photons_control/tile.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_control/addon.py` & `lifx-photons-core-0.9.5/photons_control/addon.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_control/attributes.py` & `lifx-photons-core-0.9.5/photons_control/attributes.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_control/multizone.py` & `lifx-photons-core-0.9.5/photons_control/multizone.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_control/transform.py` & `lifx-photons-core-0.9.5/photons_control/transform.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_control/payloads.py` & `lifx-photons-core-0.9.5/photons_control/payloads.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_control/script.py` & `lifx-photons-core-0.9.5/photons_control/script.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_control/colour.py` & `lifx-photons-core-0.9.5/photons_control/colour.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_products_registry.py` & `lifx-photons-core-0.9.5/photons_products_registry.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/registers.py` & `lifx-photons-core-0.9.5/photons_app/registers.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/runner.py` & `lifx-photons-core-0.9.5/photons_app/runner.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/formatter.py` & `lifx-photons-core-0.9.5/photons_app/formatter.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/option_spec/photons_app_spec.py` & `lifx-photons-core-0.9.5/photons_app/option_spec/photons_app_spec.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/option_spec/task_objs.py` & `lifx-photons-core-0.9.5/photons_app/option_spec/task_objs.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/collector.py` & `lifx-photons-core-0.9.5/photons_app/collector.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/actions.py` & `lifx-photons-core-0.9.5/photons_app/actions.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/__init__.py` & `lifx-photons-core-0.9.5/photons_app/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = "0.9.4"
+VERSION = "0.9.5"
 
 __shortdesc__ = """Base module for all photons applications"""
 
 __doc__ = """
 Photons
 =======
```

### Comparing `lifx-photons-core-0.9.4/photons_app/task_finder.py` & `lifx-photons-core-0.9.5/photons_app/task_finder.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/sphinx/tasks.py` & `lifx-photons-core-0.9.5/photons_app/sphinx/tasks.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/sphinx/docstrings.py` & `lifx-photons-core-0.9.5/photons_app/sphinx/docstrings.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/sphinx/code_for.py` & `lifx-photons-core-0.9.5/photons_app/sphinx/code_for.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/sphinx/target_fields.py` & `lifx-photons-core-0.9.5/photons_app/sphinx/target_fields.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/sphinx/structures.py` & `lifx-photons-core-0.9.5/photons_app/sphinx/structures.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/test_helpers.py` & `lifx-photons-core-0.9.5/photons_app/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/errors.py` & `lifx-photons-core-0.9.5/photons_app/errors.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/helpers.py` & `lifx-photons-core-0.9.5/photons_app/helpers.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/special.py` & `lifx-photons-core-0.9.5/photons_app/special.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_app/executor.py` & `lifx-photons-core-0.9.5/photons_app/executor.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_colour.py` & `lifx-photons-core-0.9.5/photons_colour.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,17 +324,19 @@
         func = getattr(kls, effect)
         if not getattr(func, "_is_effect", None):
             log.warning("Trying to get an effect that's on Effect, but isn't an effect\teffect=%s", effect)
             raise NoSuchEffect(effect=effect)
         return getattr(kls(), effect)(**kwargs)
 
     @effect
-    def pulse(self, cycles=1, duty_cycle=0.5, transient=1, period=1.0, skew_ratio=1, **kwargs):
+    def pulse(self, cycles=1, duty_cycle=0.5, transient=1, period=1.0, skew_ratio=sb.NotSpecified, **kwargs):
         """Options to make the light(s) pulse `color` and then back to its original color"""
-        return dict(waveform=Waveform.PULSE, cycles=cycles, skew_ratio=skew_ratio - duty_cycle, transient=transient, period=period)
+        if skew_ratio is sb.NotSpecified:
+            skew_ratio = 1 - duty_cycle
+        return dict(waveform=Waveform.PULSE, cycles=cycles, skew_ratio=skew_ratio, transient=transient, period=period)
 
     @effect
     def sine(self, cycles=1, period=1.0, peak=0.5, transient=1, skew_ratio=sb.NotSpecified, **kwargs):
         """Options to make the light(s) transition to `color` and back in a smooth sine wave"""
         if skew_ratio is sb.NotSpecified:
             skew_ratio = peak
         return dict(waveform=Waveform.SINE, cycles=cycles, skew_ratio=skew_ratio, transient=transient, period=period)
```

### Comparing `lifx-photons-core-0.9.4/photons_device_finder.py` & `lifx-photons-core-0.9.5/photons_device_finder.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/setup.py` & `lifx-photons-core-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/addon.py` & `lifx-photons-core-0.9.5/photons_transport/addon.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/bridge.py` & `lifx-photons-core-0.9.5/photons_transport/target/bridge.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/receiver.py` & `lifx-photons-core-0.9.5/photons_transport/target/receiver.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/__init__.py` & `lifx-photons-core-0.9.5/photons_transport/target/__init__.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/waiter.py` & `lifx-photons-core-0.9.5/photons_transport/target/waiter.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/result.py` & `lifx-photons-core-0.9.5/photons_transport/target/result.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/retry_options.py` & `lifx-photons-core-0.9.5/photons_transport/target/retry_options.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/target.py` & `lifx-photons-core-0.9.5/photons_transport/target/target.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/writer.py` & `lifx-photons-core-0.9.5/photons_transport/target/writer.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/script.py` & `lifx-photons-core-0.9.5/photons_transport/target/script.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_transport/target/item.py` & `lifx-photons-core-0.9.5/photons_transport/target/item.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_protocol/types.py` & `lifx-photons-core-0.9.5/photons_protocol/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,28 @@
 import enum
 import re
 
 log = logging.getLogger("photons_protocol.packets.builder")
 
 Optional = type("Optional", (), {})()
 
+class UnknownEnum:
+    def __init__(self, val):
+        self.name = "UNKNOWN"
+        self.value = val
+
+    def __repr__(self):
+        return f"<UNKNOWN: {self.value}>"
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and other.value == self.value
+
 regexes = {
-      "version_number": re.compile("(?P<major>\d+)\.(?P<minor>\d+)")
+      "version_number": re.compile(r"(?P<major>\d+)\.(?P<minor>\d+)")
+    , "unknown_enum": re.compile(r"<UNKNOWN: (?P<value>\d+)>")
     }
 
 class Type(object):
     """
     A specification of how to pack and unpack bits from/to a packet
 
     struct_format
@@ -63,14 +75,15 @@
     _unpack_transform = sb.NotSpecified
 
     _many = False
     _optional = False
     _allow_float = False
     _version_number = False
     _allow_callable = False
+    _unknown_enum_values = False
 
     def __init__(self, struct_format, conversion):
         self.conversion = conversion
         self.struct_format = struct_format
 
     def __call__(self, size_bits, left=sb.NotSpecified):
         """
@@ -94,14 +107,16 @@
         result._many_size = self._many_size
         result._transform = self._transform
         result._unpack_transform = self._unpack_transform
         result._optional = self._optional
         result._allow_float = self._allow_float
         result._version_number = self._version_number
         result._allow_callable = self._allow_callable
+        result._unknown_enum_values = self._unknown_enum_values
+
         result.original_size = getattr(self, "original_size", size_bits)
         if left is not sb.NotSpecified:
             result.left_cut = left
         elif hasattr(self, "left_cut"):
             result.left_cut = self.left_cut
         return result
 
@@ -118,18 +133,19 @@
 
     def version_number(self):
         """Set the _version_number option"""
         res = self.S(self.size_bits)
         res._version_number = True
         return res
 
-    def enum(self, enum):
+    def enum(self, enum, allow_unknown=False):
         """Set the _enum option"""
         res = self.S(self.size_bits)
         res._enum = enum
+        res._unknown_enum_values = allow_unknown
         return res
 
     def dynamic(self, dynamiser):
         """Set a function that returns what fields make up this one chunk of bytes"""
         res = self.S(self.size_bits)
         res._dynamic = dynamiser
         return res
@@ -328,15 +344,19 @@
         bitmask = None
         if self._bitmask is not sb.NotSpecified:
             bitmask = self._bitmask
 
         if self._version_number:
             return version_number_spec(unpacking=unpacking)
 
-        return integer_spec(pkt, enum, bitmask, unpacking=unpacking, allow_float=self._allow_float)
+        return integer_spec(pkt, enum, bitmask
+            , unpacking = unpacking
+            , allow_float = self._allow_float
+            , unknown_enum_values = self._unknown_enum_values
+            )
 
     def do_transform(self, pkt, value):
         """Perform transformation on a value"""
         if self._transform is sb.NotSpecified:
             return value
         else:
             return self._transform(pkt, value)
@@ -545,20 +565,21 @@
     """
     Normalise an integer
 
     Take into account whether we have ``enum`` or ``bitmask`` and ``allow_float``
 
     .. automethod:: photons_protocol.types.integer_spec.normalise_filled
     """
-    def setup(self, pkt, enum, bitmask, unpacking=False, allow_float=False):
+    def setup(self, pkt, enum, bitmask, unpacking=False, allow_float=False, unknown_enum_values=False):
         self.pkt = pkt
         self.enum = enum
         self.bitmask = bitmask
         self.unpacking = unpacking
         self.allow_float = allow_float
+        self.unknown_enum_values = unknown_enum_values
         if self.enum and self.bitmask:
             raise ProgrammerError("Sorry, can't specify enum and bitmask for the same type")
 
     def normalise_filled(self, meta, val):
         """
         If we don't have an enum or bitmask
 
@@ -573,15 +594,16 @@
         """
         if self.enum is None and self.bitmask is None:
             if self.allow_float and type(val) is float:
                 return val
             return sb.integer_spec().normalise(meta, val)
 
         if self.enum:
-            return enum_spec(self.pkt, self.enum, unpacking=self.unpacking).normalise(meta, val)
+            kwargs = dict(unpacking=self.unpacking, allow_unknown=self.unknown_enum_values)
+            return enum_spec(self.pkt, self.enum, **kwargs).normalise(meta, val)
         else:
             return bitmask_spec(self.pkt, self.bitmask, unpacking=self.unpacking).normalise(meta, val)
 
 class bitmask_spec(sb.Spec):
     """
     A bitmask is essentially an Enum with values that can be used as a mask.
 
@@ -715,18 +737,19 @@
 
     Enum may either be a enum.Enum class or a callable that takes in the packet and returns an enum.Enum.
 
     When unpacking, we are converting into a member of the enum.
 
     When not unpacking, we are converting into the value of that member of the enum
     """
-    def setup(self, pkt, enum, unpacking=False):
+    def setup(self, pkt, enum, unpacking=False, allow_unknown=False):
         self.pkt = pkt
         self.enum = enum
         self.unpacking = unpacking
+        self.allow_unknown = allow_unknown
 
     def normalise_filled(self, meta, val):
         em = self.determine_enum()
 
         if self.unpacking:
             return self.unpack(em, meta, val)
         else:
@@ -741,25 +764,45 @@
 
         available = []
         for name, member in em.__members__.items():
             available.append((name, member.value))
             if val == name or val == repr(member) or val == member.value:
                 return member
 
+        if self.allow_unknown:
+            if isinstance(val, int) and not isinstance(val, bool):
+                return UnknownEnum(val)
+            elif isinstance(val, UnknownEnum):
+                return val
+            elif isinstance(val, str):
+                m = regexes["unknown_enum"].match(val)
+                if m:
+                    return UnknownEnum(int(m["value"]))
+
         # Only here if didn't match any members
         raise BadConversion("Value is not a valid value of the enum", val=val, enum=em, available=available, meta=meta)
 
     def pack(self, em, meta, val):
         """Get us the value of the specified member of the enum"""
         available = []
         for name, member in em.__members__.items():
             available.append((name, member.value))
             if val == name or val == repr(member) or val == member.value or val is member:
                 return member.value
 
+        if self.allow_unknown:
+            if isinstance(val, int) and not isinstance(val, bool):
+                return val
+            elif isinstance(val, UnknownEnum):
+                return val.value
+            elif isinstance(val, str):
+                m = regexes["unknown_enum"].match(val)
+                if m:
+                    return int(m["value"])
+
         if isinstance(val, enum.Enum):
             raise BadConversion("Can't convert value of wrong Enum", val=val, wanted=em, got=type(val), meta=meta)
         else:
             raise BadConversion("Value wasn't a valid enum value", val=val, available=available, meta=meta)
 
     def determine_enum(self):
         """
```

### Comparing `lifx-photons-core-0.9.4/photons_protocol/packing.py` & `lifx-photons-core-0.9.5/photons_protocol/packing.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_protocol/messages.py` & `lifx-photons-core-0.9.5/photons_protocol/messages.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_protocol/packets.py` & `lifx-photons-core-0.9.5/photons_protocol/packets.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_core.py` & `lifx-photons-core-0.9.5/photons_core.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_themes/addon.py` & `lifx-photons-core-0.9.5/photons_themes/addon.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_themes/theme.py` & `lifx-photons-core-0.9.5/photons_themes/theme.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,14 @@
     """
     def __init__(self, hue, saturation, brightness, kelvin):
         self.hue = hue
         self.saturation = saturation
         self.brightness = brightness
         self.kelvin = int(kelvin)
 
-    def as_dict(self):
-        return {"hue": self.hue, "saturation": self.saturation, "brightness": self.brightness, "kelvin": self.kelvin}
-
     @classmethod
     def average(kls, colors):
         """
         Return the average of all the provided colors
 
         If there are no colors we return white.
         """
@@ -68,14 +65,32 @@
     def __eq__(self, other):
         """A color is equal if it has the same hsbk value"""
         return other.hue == self.hue and other.saturation == self.saturation and other.brightness == self.brightness and other.kelvin == self.kelvin
 
     def __hash__(self):
         return hash((self.hue, self.saturation, self.brightness, self.kelvin))
 
+    def as_dict(self):
+        return {"hue": self.hue, "saturation": self.saturation, "brightness": self.brightness, "kelvin": self.kelvin}
+
+    @property
+    def cache_key(self):
+        """
+        Return as tuple of tuples
+
+        This is used by the tile_paint module to use as a key for caching
+
+        It is essentially the same as tuple(sorted(color.as_dict().items()))
+        """
+        return (("brightness", self.brightness), ("hue", self.hue), ("kelvin", self.kelvin), ("saturation", self.saturation))
+
+    def clone(self):
+        """Return another ThemeColor with the same hsbk values"""
+        return self.__class__(self.hue, self.saturation, self.brightness, self.kelvin)
+
     def limit_distance_to(self, other):
         """
         Return a color within 90 hue points of this color
 
         We take or add 90 depending on whether the other color is more than 180 hue points away
         where that is calculated by moving forward and wrapping around 360
 
@@ -88,15 +103,15 @@
             if h < 0:
                 h += 360
             return ThemeColor(h, self.saturation, self.brightness, self.kelvin)
         else:
             return self
 
     def __repr__(self):
-        return "<Color {}>".format(str((self.hue, self.saturation, self.brightness, self.kelvin)))
+        return f"<Color ({self.hue}, {self.saturation}, {self.brightness}, {self.kelvin})>"
 
 class Theme:
     """A wrapper around a list of ThemeColor objects"""
     def __init__(self):
         self.colors = []
 
     def add_hsbk(self, hue, saturation, brightness, kelvin):
```

### Comparing `lifx-photons-core-0.9.4/photons_themes/coords.py` & `lifx-photons-core-0.9.5/photons_themes/coords.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_themes/appliers/__init__.py` & `lifx-photons-core-0.9.5/photons_themes/appliers/__init__.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_themes/appliers/splotch.py` & `lifx-photons-core-0.9.5/photons_themes/appliers/splotch.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_themes/appliers/stripes.py` & `lifx-photons-core-0.9.5/photons_themes/appliers/stripes.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_themes/appliers/base.py` & `lifx-photons-core-0.9.5/photons_themes/appliers/base.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_themes/collections.py` & `lifx-photons-core-0.9.5/photons_themes/collections.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_themes/canvas.py` & `lifx-photons-core-0.9.5/photons_themes/canvas.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_messages/fields.py` & `lifx-photons-core-0.9.5/photons_messages/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 waveform_period = T.Uint32.default(0).transform(
       lambda _, value: int(1000 * float(value))
     , lambda value: float(value) / 1000
     ).allow_float()
 
 waveform_skew_ratio = T.Int16.default(0).transform(
-      lambda _, value: int(32767 * float(value))
-    , lambda value: float(value) / 32767
+      lambda _, v: int(65535 * (0 if v is sb.NotSpecified else float(v))) - 32768
+    , lambda v: float(v + 32768) / 65535
     ).allow_float()
 
 hsbk_with_optional = (
       ("hue", scaled_hue.optional())
     , ("saturation", scaled_to_65535.optional())
     , ("brightness", scaled_to_65535.optional())
     , ("kelvin", T.Uint16.optional())
```

### Comparing `lifx-photons-core-0.9.4/photons_messages/__init__.py` & `lifx-photons-core-0.9.5/photons_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_messages/sphinx/messages.py` & `lifx-photons-core-0.9.5/photons_messages/sphinx/messages.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_messages/frame.py` & `lifx-photons-core-0.9.5/photons_messages/frame.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_messages/messages.py` & `lifx-photons-core-0.9.5/photons_messages/messages.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_socket/addon.py` & `lifx-photons-core-0.9.5/photons_socket/addon.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_socket/fake.py` & `lifx-photons-core-0.9.5/photons_socket/fake.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_socket/__init__.py` & `lifx-photons-core-0.9.5/photons_socket/__init__.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_socket/connection.py` & `lifx-photons-core-0.9.5/photons_socket/connection.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_socket/target.py` & `lifx-photons-core-0.9.5/photons_socket/target.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/addon.py` & `lifx-photons-core-0.9.5/photons_tile_paint/addon.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 
 from photons_tile_paint.falling import TileFallingAnimation
 from photons_tile_paint.falling import TileFallingOptions
 
 from photons_tile_paint.dice import TileDiceRollAnimation
 from photons_tile_paint.dice import TileDiceRollOptions
 
+from photons_tile_paint.balls import TileBallsAnimation
+from photons_tile_paint.balls import TileBallsOptions
+
 class Animations:
     @classmethod
     def animators(kls):
         for attr in dir(kls):
             if not attr.startswith("_"):
                 val = getattr(kls, attr)
                 if isinstance(val, Animator):
@@ -125,14 +128,20 @@
 
     tile_dice_roll = Animator(TileDiceRollAnimation, TileDiceRollOptions
         , """
           A dice roll
           """
         )
 
+    tile_balls = Animator(TileBallsAnimation, TileBallsOptions
+        , """
+          Bouncing balls
+          """
+        )
+
 for name, animator in Animations.animators():
     locals()[name] = animator.make_action()
 
 if __name__ == "__main__":
     from photons_app.executor import main
     import sys
     main(["lan:tile_twinkles"] + sys.argv[1:])
```

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/pacman/font.py` & `lifx-photons-core-0.9.5/photons_tile_paint/pacman/font.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/pacman/animation.py` & `lifx-photons-core-0.9.5/photons_tile_paint/pacman/animation.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/pacman/state.py` & `lifx-photons-core-0.9.5/photons_tile_paint/pacman/state.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/orientation.py` & `lifx-photons-core-0.9.5/photons_tile_paint/orientation.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/twinkles.py` & `lifx-photons-core-0.9.5/photons_tile_paint/twinkles.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/dice.py` & `lifx-photons-core-0.9.5/photons_tile_paint/dice.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,33 +49,37 @@
                 raise Finish()
             else:
                 self.every = 0.01
                 self.duration = 0
                 prev_state = None
 
         if prev_state is None or time.time() - prev_state["last_state"] > 0.05:
+            chs = []
+            while len(chs) < len(coords):
+                chs.extend(random.sample(list(dice.values()), k=5))
+
             state = {
-                  "chars": random.sample(list(dice.values()), k=5)
+                  "chars": random.sample(chs, k=len(coords))
                 , "last_state": time.time()
                 , "started": time.time() if prev_state is None else prev_state["started"]
                 }
 
         if time.time() - state["started"] > self.options.roll_time:
             return {"chars": -1}
 
         return state
 
     def make_canvas(self, state, coords):
         chars = state["chars"]
 
         if state["chars"] == -1:
             self.every = 0.5
-            chars = [full_character] * 5
+            chars = [full_character] * len(coords)
 
         if state["chars"] == -2:
             self.duration = 0.5
             self.every = 1.5
-            chars = [random.choice(list(dice.values()))] * 5
+            chars = [random.choice(list(dice.values()))] * len(coords)
 
         canvas = Canvas()
         put_characters_on_canvas(canvas, chars, coords, self.options.dice_color.color)
         return canvas
```

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/nyan.py` & `lifx-photons-core-0.9.5/photons_tile_paint/nyan.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/marquee/options.py` & `lifx-photons-core-0.9.5/photons_tile_paint/marquee/options.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/marquee/animation.py` & `lifx-photons-core-0.9.5/photons_tile_paint/marquee/animation.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/time/animation.py` & `lifx-photons-core-0.9.5/photons_tile_paint/time/animation.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/animation.py` & `lifx-photons-core-0.9.5/photons_tile_paint/animation.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/set_state.py` & `lifx-photons-core-0.9.5/photons_tile_paint/set_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,22 +198,21 @@
         if val not in self.duration_bits_cache:
             self.duration_bits_cache[val] = self.bits(T.Uint32, int(val * 1000))
         return self.duration_bits_cache[val]
 
     def colors_bits(self, colors):
         res = []
         for color in colors:
-            dct = color.as_dict()
-            fields = tuple(sorted(dct.items()))
+            fields = color.cache_key
             if fields not in self.cache:
                 bits = []
-                bits.append(self.bits(hsbk[0][1], int(65535 * (dct["hue"] / 360))))
-                bits.append(self.bits(hsbk[1][1], int(65535 * dct["saturation"])))
-                bits.append(self.bits(hsbk[2][1], int(65535 * dct["brightness"])))
-                bits.append(self.bits(hsbk[3][1], dct["kelvin"]))
+                bits.append(self.bits(hsbk[0][1], int(65535 * (color.hue / 360))))
+                bits.append(self.bits(hsbk[1][1], int(65535 * color.saturation)))
+                bits.append(self.bits(hsbk[2][1], int(65535 * color.brightness)))
+                bits.append(self.bits(hsbk[3][1], color.kelvin))
                 self.cache[fields] = functools.reduce(operator.add, bits)
             res.append(self.cache[fields])
         return functools.reduce(operator.add, res)
 
     def make_target(self, target):
         if target not in self.targets_cache:
             val = target
```

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/options.py` & `lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/options.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/font.py` & `lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/font.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/animation.py` & `lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/animation.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/gameoflife/state.py` & `lifx-photons-core-0.9.5/photons_tile_paint/gameoflife/state.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/font/dice.py` & `lifx-photons-core-0.9.5/photons_tile_paint/font/dice.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/font/alphabet.py` & `lifx-photons-core-0.9.5/photons_tile_paint/font/alphabet.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/photons_tile_paint/font/base.py` & `lifx-photons-core-0.9.5/photons_tile_paint/font/base.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-core-0.9.4/lifx_photons_core.egg-info/PKG-INFO` & `lifx-photons-core-0.9.5/lifx_photons_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-photons-core
-Version: 0.9.4
+Version: 0.9.5
 Summary: The core modules of the photons framework
 Home-page: http://github.com/delfick/photons-core
 Author: Stephen Moore
 Author-email: delfick755@gmail.com
 License: MIT
 Description: Photons
         =======
```

### Comparing `lifx-photons-core-0.9.4/lifx_photons_core.egg-info/SOURCES.txt` & `lifx-photons-core-0.9.5/lifx_photons_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 photons_themes/appliers/base.py
 photons_themes/appliers/single.py
 photons_themes/appliers/splotch.py
 photons_themes/appliers/stripes.py
 photons_tile_paint/__init__.py
 photons_tile_paint/addon.py
 photons_tile_paint/animation.py
+photons_tile_paint/balls.py
 photons_tile_paint/dice.py
 photons_tile_paint/falling.py
 photons_tile_paint/nyan.py
 photons_tile_paint/options.py
 photons_tile_paint/orientation.py
 photons_tile_paint/set_state.py
 photons_tile_paint/twinkles.py
```

