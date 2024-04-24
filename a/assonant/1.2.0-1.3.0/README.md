# Comparing `tmp/assonant-1.2.0.tar.gz` & `tmp/assonant-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assonant-1.2.0.tar", last modified: Tue Apr  2 11:54:38 2024, max compression
+gzip compressed data, was "assonant-1.3.0.tar", last modified: Wed Apr 24 13:07:04 2024, max compression
```

## Comparing `assonant-1.2.0.tar` & `assonant-1.3.0.tar`

### file list

```diff
@@ -1,76 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     6513 2024-04-02 11:54:38.233060 assonant-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2024-04-01 19:04:21.000000 assonant-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.225060 assonant-1.2.0/assonant/
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/_kafka/
--rw-rw-rw-   0 root         (0) root         (0)       82 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/_kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5920 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/_kafka/producer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/_nexus/
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/_nexus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/_nexus/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    22987 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/_nexus/nexus_object_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/data_classes/
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-03-27 18:55:31.000000 assonant-1.2.0/assonant/data_classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/assonant_data_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/data_classes/components/
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-28 14:10:38.000000 assonant-1.2.0/assonant/data_classes/components/attenuator.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2024-03-28 13:44:08.000000 assonant-1.2.0/assonant/data_classes/components/beam.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-03-28 13:44:08.000000 assonant-1.2.0/assonant/data_classes/components/beam_stopper.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-03-28 13:28:11.000000 assonant-1.2.0/assonant/data_classes/components/bending_magnet.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/components/bvs.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-28 14:06:26.000000 assonant-1.2.0/assonant/data_classes/components/collimator.py
--rw-rw-rw-   0 root         (0) root         (0)     9495 2024-03-27 19:22:57.000000 assonant-1.2.0/assonant/data_classes/components/component.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-03-26 18:27:23.000000 assonant-1.2.0/assonant/data_classes/components/detector.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/components/fresnel_zone_plate.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/components/mirror.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-03-26 18:27:23.000000 assonant-1.2.0/assonant/data_classes/components/monochromator.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/components/pinhole.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/components/sample.py
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/components/sensor.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-03-28 14:01:19.000000 assonant-1.2.0/assonant/data_classes/components/shutter.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/components/slit.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-03-28 13:28:11.000000 assonant-1.2.0/assonant/data_classes/components/storage_ring.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2024-03-28 13:28:11.000000 assonant-1.2.0/assonant/data_classes/components/undulator.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-03-28 13:28:11.000000 assonant-1.2.0/assonant/data_classes/components/wiggler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/data_classes/data_handlers/
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/axis.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/data_field.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/data_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/external_link.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/time_series.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2024-03-26 18:27:23.000000 assonant-1.2.0/assonant/data_classes/entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/data_classes/events/
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/events/assonant_event.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/events/experiment_done.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-27 18:55:31.000000 assonant-1.2.0/assonant/data_classes/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/assonant/data_classes/types/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/types/measurement_type.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/types/scope_type.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/types/transformation_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/assonant/data_sender/
--rw-rw-rw-   0 root         (0) root         (0)      341 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/_assonant_data_sender_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     2693 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/_data_sender_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/_kafka_data_sender.py
--rw-rw-rw-   0 root         (0) root         (0)     1527 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/assonant_data_sender.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/assonant/file_writer/
--rw-rw-rw-   0 root         (0) root         (0)      338 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      727 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/_assonant_file_writer_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     2346 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/_file_writer_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/_nexus_file_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/assonant_file_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/assonant.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6513 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2546 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      147 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-01 19:04:21.000000 assonant-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 11:54:38.233060 assonant-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.633624 assonant-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     6513 2024-04-24 13:07:04.629624 assonant-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2024-04-24 13:04:35.000000 assonant-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.617624 assonant-1.3.0/assonant/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-24 11:59:14.000000 assonant-1.3.0/assonant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.617624 assonant-1.3.0/assonant/_kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/_kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5920 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/_kafka/producer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.617624 assonant-1.3.0/assonant/_nexus/
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/_nexus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/_nexus/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29596 2024-04-23 19:33:42.000000 assonant-1.3.0/assonant/_nexus/nexus_object_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.617624 assonant-1.3.0/assonant/data_classes/
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/assonant_data_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.625624 assonant-1.3.0/assonant/data_classes/components/
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-04-23 19:33:42.000000 assonant-1.3.0/assonant/data_classes/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-28 14:10:38.000000 assonant-1.3.0/assonant/data_classes/components/attenuator.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-03-28 13:44:08.000000 assonant-1.3.0/assonant/data_classes/components/beam.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-03-28 13:44:08.000000 assonant-1.3.0/assonant/data_classes/components/beam_stopper.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/components/beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-03-28 13:28:11.000000 assonant-1.3.0/assonant/data_classes/components/bending_magnet.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/components/bvs.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-28 14:06:26.000000 assonant-1.3.0/assonant/data_classes/components/collimator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9719 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/components/component.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-23 19:33:42.000000 assonant-1.3.0/assonant/data_classes/components/cryojet.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-03-26 18:27:23.000000 assonant-1.3.0/assonant/data_classes/components/detector.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2024-04-23 17:05:24.000000 assonant-1.3.0/assonant/data_classes/components/dewar.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-01 17:43:16.000000 assonant-1.3.0/assonant/data_classes/components/fresnel_zone_plate.py
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-23 19:33:42.000000 assonant-1.3.0/assonant/data_classes/components/granite_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/components/mirror.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-03-26 18:27:23.000000 assonant-1.3.0/assonant/data_classes/components/monochromator.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-01 17:43:16.000000 assonant-1.3.0/assonant/data_classes/components/pinhole.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/components/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/components/sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-03-28 14:01:19.000000 assonant-1.3.0/assonant/data_classes/components/shutter.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/components/slit.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-03-28 13:28:11.000000 assonant-1.3.0/assonant/data_classes/components/storage_ring.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-03-28 13:28:11.000000 assonant-1.3.0/assonant/data_classes/components/undulator.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-03-28 13:28:11.000000 assonant-1.3.0/assonant/data_classes/components/wiggler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.625624 assonant-1.3.0/assonant/data_classes/data_handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/data_handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/data_handlers/axis.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-15 13:48:25.000000 assonant-1.3.0/assonant/data_classes/data_handlers/data_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/data_handlers/data_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/data_handlers/external_link.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/data_handlers/time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     4709 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.625624 assonant-1.3.0/assonant/data_classes/enums/
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/enums/beamline_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/enums/measurement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/enums/scope_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-22 20:49:32.000000 assonant-1.3.0/assonant/data_classes/enums/transformation_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.629624 assonant-1.3.0/assonant/data_classes/events/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/events/assonant_event.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_classes/events/experiment_done.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-27 18:55:31.000000 assonant-1.3.0/assonant/data_classes/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.629624 assonant-1.3.0/assonant/data_sender/
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_sender/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_sender/_assonant_data_sender_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2693 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_sender/_data_sender_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_sender/_kafka_data_sender.py
+-rw-rw-rw-   0 root         (0) root         (0)     1527 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_sender/assonant_data_sender.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/data_sender/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.629624 assonant-1.3.0/assonant/file_writer/
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/file_writer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      727 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/file_writer/_assonant_file_writer_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/file_writer/_file_writer_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/file_writer/_nexus_file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/file_writer/assonant_file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-03-20 19:48:00.000000 assonant-1.3.0/assonant/file_writer/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:07:04.629624 assonant-1.3.0/assonant.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6513 2024-04-24 13:07:04.000000 assonant-1.3.0/assonant.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2771 2024-04-24 13:07:04.000000 assonant-1.3.0/assonant.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:07:04.000000 assonant-1.3.0/assonant.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2024-04-24 13:07:04.000000 assonant-1.3.0/assonant.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-24 13:07:04.000000 assonant-1.3.0/assonant.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-24 13:04:35.000000 assonant-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 13:07:04.633624 assonant-1.3.0/setup.cfg
```

### Comparing `assonant-1.2.0/PKG-INFO` & `assonant-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assonant
-Version: 1.2.0
+Version: 1.3.0
 Summary: (Meta)Data standardization package for Sirius, the 4th generation brazillian synchrotron light source
 Author: Data Science and Management Group @ GCD
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,15 +25,15 @@
     Welcome to Assonant 🎶 𝄇
 </h1>
 <p align="center">
     <em>A beamline-agnostic event processing engine for data collection and organization</em>
 </p>
 <p align="center">
 <a href="https://gitlab.cnpem.br/GCD/data-management/assonant#readme" target="_blank">
-    <img alt="Version" src="https://img.shields.io/badge/version-1.2.0-blue.svg?cacheSeconds=2592000"/>
+    <img alt="Version" src="https://img.shields.io/badge/version-1.3.0-blue.svg?cacheSeconds=2592000"/>
 </a>
 <a href="https://gitlab.cnpem.br/GCD/data-science/data-management/assonant/commits/dev" target="_blank">
     <img alt="Maintenance" src="https://img.shields.io/badge/Developing%3F-yes-green.svg"/>
 </a>
 <a href="https://pypi.org/project/fastapi" target="_blank">
     <img src="https://img.shields.io/badge/pyversions-3.7|3.8|3.9|3.10-orange" alt="Supported Python versions">
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: assonant Version: 1.2.0 Summary: (Meta)Data
+Metadata-Version: 2.1 Name: assonant Version: 1.3.0 Summary: (Meta)Data
 standardization package for Sirius, the 4th generation brazillian synchrotron
 light source Author: Data Science and Management Group @ GCD Classifier:
 License :: OSI Approved :: GNU Lesser General Public License v3 or later
 (LGPLv3+) Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist: annotated-
```

### Comparing `assonant-1.2.0/README.md` & `assonant-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     Welcome to Assonant 🎶 𝄇
 </h1>
 <p align="center">
     <em>A beamline-agnostic event processing engine for data collection and organization</em>
 </p>
 <p align="center">
 <a href="https://gitlab.cnpem.br/GCD/data-management/assonant#readme" target="_blank">
-    <img alt="Version" src="https://img.shields.io/badge/version-1.2.0-blue.svg?cacheSeconds=2592000"/>
+    <img alt="Version" src="https://img.shields.io/badge/version-1.3.0-blue.svg?cacheSeconds=2592000"/>
 </a>
 <a href="https://gitlab.cnpem.br/GCD/data-science/data-management/assonant/commits/dev" target="_blank">
     <img alt="Maintenance" src="https://img.shields.io/badge/Developing%3F-yes-green.svg"/>
 </a>
 <a href="https://pypi.org/project/fastapi" target="_blank">
     <img src="https://img.shields.io/badge/pyversions-3.7|3.8|3.9|3.10-orange" alt="Supported Python versions">
 </a>
```

### Comparing `assonant-1.2.0/assonant/_kafka/producer.py` & `assonant-1.3.0/assonant/_kafka/producer.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/_nexus/nexus_object_factory.py` & `assonant-1.3.0/assonant/_nexus/nexus_object_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Factory class to deal with NeXus Object Creation."""
 
-
+from collections.abc import Iterable
 from typing import Dict, List
 
+import numpy as np
 from nexusformat.nexus import *
 
 from assonant.data_classes import AssonantDataClass, Entry
 from assonant.data_classes.components import (
     BVS,
     Attenuator,
     Beam,
+    Beamline,
     BeamStopper,
     BendingMagnet,
     Collimator,
     Component,
+    Cryojet,
     Detector,
     DetectorModule,
     DetectorROI,
+    Dewar,
     FresnelZonePlate,
+    GraniteBase,
     Mirror,
     Monochromator,
     MonochromatorCrystal,
     MonochromatorVelocitySelector,
     Pinhole,
     Sample,
     Sensor,
@@ -46,34 +51,45 @@
     """NeXus Object Factory Class.
 
     Class that implements the factory design pattern
     (https://refactoring.guru/design-patterns/factory-method) to fully abstract
     the procedure of creating NeXus object out of AssonantDataClass objects.
     """
 
-    def create_nxobject(self, data_obj: AssonantDataClass, pack_into_nxroot: bool = False) -> NXobject:
+    def create_nxobject(
+        self, data_obj: AssonantDataClass, pack_into_nxroot: bool = False, convert_missing_data: bool = True
+    ) -> NXobject:
         """Creates the respective Nexus object based on the passed AssonantDataClass specific type.
 
         Args:
             data_obj (AssonantDataClass): Data object which will be used for the
             NeXus object creation
             pack_into_nxroot (bool, optional): If returned object should be or not
             packed inside a NXroot. Defaults to False.
+            convert_missing_data (bool, optional): If None values within DataField classes
+            should be transformed or not in a np.nan value. Defaults to True.
 
         Raises:
             NeXusObjectFactoryError: The 'obj' argument type does not fit any of the
             supported types
 
         Returns:
             NXobject: NeXus object respective to the data object passed as the
             data_obj argument
         """
         if isinstance(data_obj, Entry):
             print("Constructor Called: ExperimentEntry")
             nxobject = self._create_entry(data_obj)
+
+            # Dev note: Special case for entry which all data is contained on its beamline field
+            nxobject.insert(self.create_nxobject(data_obj.beamline))
+
+        elif isinstance(data_obj, Beamline):
+            print("Constructor Called: Beamline")
+            nxobject = self._create_beamline(data_obj)
         elif isinstance(data_obj, Sample):
             print("Constructor Called: Sample")
             nxobject = self._create_sample(data_obj)
         elif isinstance(data_obj, Detector):
             print("Constructor Called: Detector")
             nxobject = self._create_detector(data_obj)
         elif isinstance(data_obj, Monochromator):
@@ -88,14 +104,18 @@
         elif isinstance(data_obj, Slit):
             print("Constructor Called: Slit")
             nxobject = self._create_slit(data_obj)
         elif isinstance(data_obj, TimeSeries):
             print("Constructor Called: TimeSeries")
             nxobject = self._create_time_series(data_obj)
         elif isinstance(data_obj, DataField):
+            if convert_missing_data is True:
+                print("Converting missing values from DataField...")
+                data_obj = self._convert_none_values_from_data_field(data_field=data_obj)
+                print("Missing values conversion finished.")
             print("Constructor Called: Datafield")
             nxobject = self._create_data_field(data_obj)
         elif isinstance(data_obj, ExternalLink):
             print("Constructor Called: ExternalLink")
             nxobject = self._create_external_link(data_obj)
         elif isinstance(data_obj, DetectorROI):
             print("Constructor Called: DetectorROI")
@@ -141,14 +161,23 @@
             nxobject = self._create_pinhole(data_obj)
         elif isinstance(data_obj, FresnelZonePlate):
             print("Constructor Called: FresnelZonePlate")
             nxobject = self._create_fresnel_zone_plate(data_obj)
         elif isinstance(data_obj, Sensor):
             print("Constructor Called: Sensor")
             nxobject = self._create_sensor(data_obj)
+        elif isinstance(data_obj, Dewar):
+            print("Constructor Called: Dewar")
+            nxobject = self._create_dewar(data_obj)
+        elif isinstance(data_obj, Cryojet):
+            print("Constructor Called: Cryojet")
+            nxobject = self._create_cryojet(data_obj)
+        elif isinstance(data_obj, GraniteBase):
+            print("Constructor Called: GraniteBase")
+            nxobject = self._create_granite_base(data_obj)
         else:
             raise NeXusObjectFactoryError(
                 f"NeXus object factory doesn't have an constructor method to deal with objects of type: {type(data_obj)}"
             )
 
         # Check if there are subgroups to be created based on special fields
         if hasattr(data_obj, "fields"):
@@ -304,24 +333,27 @@
         if data_field.unit is not None:
             attrs["unit"] = data_field.unit
 
         nxobject = NXfield(value=data_field.value, attrs=attrs)
 
         return nxobject
 
-    def _create_detector_roi(self, detector_roi: DetectorROI) -> NXobject:
+    def _create_detector_roi(self, detector_roi: DetectorROI) -> NXgroup:
         """Private method to create the NeXus object respective to the DetectorROI data class.
 
         Args:
             detector_roi (DetectorROI): Data object containing detector region of interest (ROI) data.
 
         Returns:
-            NXobject: NeXus object respective to the DetectorROI data object.
+            NXgroup: NeXus object respective to the DetectorROI data object.
         """
-        nxobject = NXgroup(name=detector_roi.name)
+        # Dev note: Currently, these type of data are stored in a contributed definition called NXregion. Due
+        # to that the nexusformat package don't provide support for it so the nxclass attribute must be
+        # set manually.
+        nxobject = NXgroup(name=detector_roi.name, nxclass="NXregion")
         return nxobject
 
     def _create_detector_module(self, detector_module: DetectorModule) -> NXdetector_module:
         """Private method to create the NeXus object respective to the DetectorModule data class.
 
         Args:
             detector_module (DetectorModule): Data object containing detector module data.
@@ -499,14 +531,72 @@
 
         Returns:
             NXsensor: NeXus object respective to the Sensor data object.
         """
         nxobject = NXsensor(name=sensor.name, measurement=sensor.measurement_type.value)
         return nxobject
 
+    def _create_dewar(self, dewar: Dewar) -> NXgroup:
+        """Private method to create the NeXus object respective to the Dewar data class.
+
+        Args:
+            dewar (Dewar): Data object containing dewar data.
+
+        Returns:
+            NXgroup: NeXus object respective to the Dewar data object.
+        """
+        # Dev note: Currently, there is no base or contributed definition on NeXus for this type of component.
+        # Due to that, a temporary nxclass value will be set to allow future automatized replacement if a
+        # standard for it is defined.
+        nxobject = NXgroup(name=dewar.name, nxclass="NXcustom_dewar")
+        return nxobject
+
+    def _create_cryojet(self, cryojet: Cryojet) -> NXgroup:
+        """Private method to create the NeXus object respective to the Cryojet data class.
+
+        Args:
+            cryojet (Cryojet): Data object containing dewar data.
+
+        Returns:
+            NXgroup: NeXus object respective to the Cryojet data object.
+        """
+        # Dev note: Currently, there is no base or contributed definition on NeXus for this type of component.
+        # Due to that, a temporary nxclass value will be set to allow future automatized replacement if a
+        # standard for it is defined.
+        nxobject = NXgroup(name=cryojet.name, nxclass="NXcustom_cryojet")
+        return nxobject
+
+    def _create_granite_base(self, granite_base: GraniteBase) -> NXgroup:
+        """Private method to create the NeXus object respective to the Cryojet data class.
+
+        Args:
+            granite_base (GraniteBase): Data object containing granite base data.
+
+        Returns:
+            NXgroup: NeXus object respective to the GraniteBase data object.
+        """
+        # Dev note: Currently, there is no base or contributed definition on NeXus for this type of component.
+        # Due to that, a temporary nxclass value will be set to allow future automatized replacement if a
+        # standard for it is defined.
+        nxobject = NXgroup(name=granite_base.name, nxclass="NXcustom_granite_base")
+        return nxobject
+
+    def _create_beamline(self, beamline: Beamline) -> NXinstrument:
+        """Private method to create the NeXus object respective to the Beamline data class.
+
+        Args:
+            beamline (Beamline): Data object containing beamline data.
+
+        Returns:
+            NXinstrument: NeXus object respective to the Beamline data object.
+        """
+        nxobject = NXinstrument(name="instrument")
+        nxobject["name"] = beamline.name.value
+        return nxobject
+
     def _create_transformations(self, nxobject: NXobject, positions: List[Axis]) -> NXobject:
         """Create a NXtransformations group to store positioning data passed as a list of Axis objects.
 
         Args:
             nxobject (NXobject): NeXus object containing current objects
             positions (List[Axis]): List of Axis objects containing each of them the positioning data related to a
             specific monitored axis.
@@ -561,19 +651,85 @@
             subcomponents (List[Component]): List containing Component object which will be
             converted to their respective NXobjects and inserted on passed NXobject.
 
         Returns:
             NXobject: Passed NXobject updated with subcomponents groups created into it.
         """
         if subcomponents != []:
-            if isinstance(nxobject, NXentry):
-                # Dev note: According to NeXus definitions, NXentry must contain an
-                # NXinstrument group inside it and any information related to devices
-                # should be added below it, what explain the reason for this specific
-                # treatment.
-                nxobject.insert(NXinstrument(name="instrument"))
-                for subcomponent in subcomponents:
-                    nxobject["instrument"].insert(self.create_nxobject(subcomponent))
-            else:
-                for subcomponent in subcomponents:
-                    nxobject.insert(self.create_nxobject(subcomponent))
+            for subcomponent in subcomponents:
+                nxobject.insert(self.create_nxobject(subcomponent))
         return nxobject
+
+    def _convert_none_values_from_list(self, lst: List) -> List:
+        """Transform None value within a list into np.nan.
+
+        Args:
+            lst (List): List containing values to be verified.
+
+        Raises:
+            NeXusObjectFactoryError: Raised when any error occurs when iterating the list.
+
+        Returns:
+            List: List with None values transformed into np.nan.
+        """
+        try:
+            return [value if value is not None else np.nan for value in lst]
+        except Exception as e:
+            raise NeXusObjectFactoryError(f"An error ocurred when iterating list of{type(lst)} type.") from e
+
+    def _convert_none_values_from_dict(self, d: Dict) -> Dict:
+        """Transform None value within a dictionary into np.nan.
+
+        Args:
+            d (Dict): Dictionary containing values to be verified.
+
+        Raises:
+            NeXusObjectFactoryError: Raised when any error occurs when iterating dictionary elements.
+
+        Returns:
+            Dict: Dictionary with None values transformed into np.nan.
+        """
+        try:
+            for key in d:
+                if isinstance(d[key], Iterable):
+                    d[key] = self._convert_none_values_from_iterable(iterable=d[key])
+                elif d[key] is None:
+                    d[key] = np.nan
+            return d
+        except Exception as e:
+            raise NeXusObjectFactoryError("An error ocurred when iterating dict.") from e
+
+    def _convert_none_values_from_iterable(self, iterable: Iterable) -> Iterable:
+        if isinstance(iterable, str):
+            pass  # No changed needed for this cases
+        elif isinstance(iterable, List) or isinstance(iterable, np.ndarray):
+            iterable = self._convert_none_values_from_list(iterable)
+        elif isinstance(iterable, Dict):
+            iterable = self._convert_none_values_from_dict(iterable)
+        else:
+            raise NeXusObjectFactoryError(
+                f"Iterable from type {type(iterable)} is not suported for None values convertion."
+            )
+
+        return iterable
+
+    def _convert_none_values_from_data_field(self, data_field: DataField) -> DataField:
+        """Transform None values within a DataField value field into np.nan.
+
+        Args:
+            data_field (DataField): DataField object which value field will be verified.
+
+        Returns:
+            DataField: DataField object with None values within its value field transformed into np.nan.
+        """
+        try:
+            if isinstance(data_field.value, Iterable):
+                data_field.value = self._convert_none_values_from_iterable(iterable=data_field.value)
+            elif data_field.value is None:
+                data_field.value = np.nan
+        except Exception as e:
+            raise NeXusObjectFactoryError("An error occured when converting DataField None values.") from e
+
+        if data_field.unit is None:
+            data_field.unit = np.nan
+
+        return data_field
```

### Comparing `assonant-1.2.0/assonant/data_classes/assonant_data_class.py` & `assonant-1.3.0/assonant/data_classes/assonant_data_class.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/data_classes/components/__init__.py` & `assonant-1.3.0/assonant/data_classes/components/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 
 Data classes that defines available Assonant components.
 """
 
 from .attenuator import Attenuator
 from .beam import Beam
 from .beam_stopper import BeamStopper
+from .beamline import Beamline
 from .bending_magnet import BendingMagnet
 from .bvs import BVS
 from .collimator import Collimator
 from .component import Component
+from .cryojet import Cryojet
 from .detector import Detector, DetectorModule, DetectorROI
+from .dewar import Dewar
 from .fresnel_zone_plate import FresnelZonePlate
+from .granite_base import GraniteBase
 from .mirror import Mirror
 from .monochromator import (
     Monochromator,
     MonochromatorCrystal,
     MonochromatorVelocitySelector,
 )
 from .pinhole import Pinhole
@@ -27,22 +31,26 @@
 from .undulator import Undulator
 from .wiggler import Wiggler
 
 __all__ = [
     "Attenuator",
     "Beam",
     "BeamStopper",
+    "Beamline",
     "BendingMagnet",
     "BVS",
     "Collimator",
     "Component",
+    "Cryojet",
     "Detector",
     "DetectorModule",
     "DetectorROI",
+    "Dewar",
     "FresnelZonePlate",
+    "GraniteBase",
     "Mirror",
     "Monochromator",
     "MonochromatorCrystal",
     "MonochromatorVelocitySelector",
     "Pinhole",
     "Sample",
     "Sensor",
```

### Comparing `assonant-1.2.0/assonant/data_classes/components/component.py` & `assonant-1.3.0/assonant/data_classes/components/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from typing import Dict, List, Optional, Type, Union
 
 import numpy as np
 
 from ..assonant_data_class import AssonantDataClass
 from ..data_handlers import Axis, DataField, DataHandler, TimeSeries
+from ..enums import TransformationType
 from ..exceptions import AssonantDataClassesError
-from ..types import TransformationType
 
 
 # TODO: Make this class abstract
 class Component(AssonantDataClass):
     """Abstract class that creates the base common requirements to define an Assonant Component.
 
     Components are more generic definitions which may be composed by many subcomponents if more
@@ -19,189 +19,200 @@
     """
 
     name: str
     subcomponents: Optional[List["Component"]] = []
     positions: Optional[List[Axis]] = []
     fields: Optional[Dict[str, DataHandler]] = {}
 
-    def add_subcomponent(self, component: "Component"):
-        """Add new subcomponent to component.
+    def add_subcomponent(self, component: Union["Component", List["Component"]]):
+        """Add new subcomponent or list of new subcomponents to component.
 
         Args:
-            component (Component): Component object which will be add as
+            component (Union[Component, List[Component]]): Component object or List of Components which will be add as
             subcomponent from called Component object.
         """
-        self.subcomponents.append(component)
+        if isinstance(component, List):
+            for _component in component:
+                self.subcomponents.append(_component)
+        else:
+            self.subcomponents.append(component)
 
     def add_position(
         self,
         name: str,
         transformation_type: TransformationType,
-        value: Union[int, float, str, List, Type[np.ndarray]],
+        value: Union[int, float, str, List, Type[np.ndarray], None],
         unit: Optional[str] = None,
-        extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]] = None,
+        extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray], None]]] = {},
     ):
         """Add new positional field to component.
 
         Args:
             name (str): Axis name.
             transformation_type (TransformationType): Type of transformation done by axis.
-            value (Union[int, float, str, List, Type[np.ndarray]]): Value related to axis
+            value (Union[int, float, str, List, Type[np.ndarray], None]): Value related to axis
             collected data.
             unit (Optional[str], optional): Measurement unit related to value parameter.
             Defaults to None.
-            extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]], optional): Dictionary
-            containing any aditional metadata related to collected data. Defaults to None.
+            extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray],
+            None]]], optional): Dictionary
+            containing any aditional metadata related to collected data. Defaults to {}.
         """
         try:
             new_axis = Axis(
                 name=name,
                 transformation_type=transformation_type,
                 value=DataField(
                     value=value,
                     unit=unit,
-                    extra_metadata={} if extra_metadata is None else extra_metadata,
+                    extra_metadata=extra_metadata,
                 ),
             )
         except Exception as e:
             raise AssonantDataClassesError(f"Failed to create Axis Data Handler for {self.name} Component.") from e
         try:
             self.positions.append(new_axis)
         except Exception as e:
             raise AssonantDataClassesError(f"Failed to add Axis to {self.name} Component positions list.") from e
 
     def add_timeseries_position(
         self,
         name: str,
         transformation_type: TransformationType,
-        value: Union[int, float, str, List, Type[np.ndarray]],
-        timestamps: Union[int, float, str, List, Type[np.ndarray]],
+        value: Union[int, float, str, List, Type[np.ndarray], None],
+        timestamps: Union[int, float, str, List, Type[np.ndarray], None],
         unit: Optional[str] = None,
-        extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]] = None,
+        extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray], None]]] = {},
         timestamps_unit: Optional[str] = None,
-        timestamp_extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]] = None,
+        timestamp_extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray], None]]] = {},
     ):
         """Add new positional field to component.
 
         Args:
             name (str): Axis name
             transformation_type (TransformationType): Transformation type of the Axis
-            value (Union[int, float, str, List, Type[np.ndarray]]): Value related to
+            value (Union[int, float, str, List, Type[np.ndarray], None]): Value related to
             axis collected data
-            timestamps (Union[int, float, str, List, Type[np.ndarray]]): Timestamps
+            timestamps (Union[int, float, str, List, Type[np.ndarray], None]): Timestamps
             related to data collected from the axis.
             unit (Optional[str], optional): Measurement unit related to value
             field. Defaults to None.
-            extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]], optional): Dictionary
-            containing extra metadata about value field. Defaults to None.
+            extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray],
+            None]]], optional): Dictionary
+            containing extra metadata about value field. Defaults to {}.
             tracked it as a TimeSeries. Defaults to None.
             timestamps_unit (Optional[str], optional): Measurement unit related to
             timestamp field. Defaults to None.
-            timestamp_extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]], optional):
-            Dictionary containing extra metadata about timestamps field. Defaults to None.
+            timestamp_extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray],
+            None]]], optional): Dict
+            containing extra metadata about timestamps field. Defaults to {}.
         """
         # Check if positions should be saved as a DataField or TimeSeries
         try:
             new_axis = Axis(
                 name=name,
                 transformation_type=transformation_type,
                 value=TimeSeries(
                     value=DataField(
                         value=value,
                         unit=unit,
-                        extra_metadata={} if extra_metadata is None else extra_metadata,
+                        extra_metadata=extra_metadata,
                     ),
                     timestamps=DataField(
                         value=timestamps,
                         unit=timestamps_unit,
-                        extra_metadata={} if timestamp_extra_metadata is None else timestamp_extra_metadata,
+                        extra_metadata=timestamp_extra_metadata,
                     ),
                 ),
             )
         except Exception as e:
             raise AssonantDataClassesError(
-                f"Failed to create Axis Data Handler with TimeSeries data for {self.name} " f"Component."
+                f"Failed to create Axis Data TimeSeries with TimeSeries data for {self.name} Component."
             ) from e
         try:
             self.positions.append(new_axis)
         except Exception as e:
             raise AssonantDataClassesError(
-                f"Failed to add Axis with TimeSeries data to {self.name} Component positions" f" list."
+                f"Failed to add Axis with TimeSeries data to {self.name} Component positions list."
             ) from e
 
     def add_field(
         self,
         name: str,
-        value: Union[int, float, str, List, Type[np.ndarray]],
+        value: Union[int, float, str, List, Type[np.ndarray], None],
         unit: Optional[str] = None,
-        extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]] = None,
+        extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray], None]]] = {},
     ):
         """Add new positional field to component that data was collected as a TimeSeries.
 
         Args:
             name (str): Field name.
-            value (Union[int, float, str, List, Type[np.ndarray]]): Value related to field
+            value (Union[int, float, str, List, Type[np.ndarray], None]): Value related to field
             collected data.
             unit (Optional[str], optional): Measurement unit related to value parameter.
             Defaults to None.
-            extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]], optional): Dictionary
-            containing any aditional metadata related to collected data. Defaults to None.
+            extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray], None]]], optional): Dict
+            containing any aditional metadata related to collected data. Defaults to {}.
         """
         try:
             new_field = DataField(
                 value=value,
                 unit=unit,
-                extra_metadata={} if extra_metadata is None else extra_metadata,
+                extra_metadata=extra_metadata,
             )
         except Exception as e:
             raise AssonantDataClassesError(f"Failed to create DataField Data Handler for {self.name} Component.") from e
         if name not in self.fields:
             self.fields[name] = new_field
         else:
             raise AssonantDataClassesError(f"Field name already exists on: {self.name} Component.")
 
     def add_timeseries_field(
         self,
         name: str,
-        value: Union[int, float, str, List, Type[np.ndarray]],
-        timestamps: Union[int, float, str, List, Type[np.ndarray]],
+        value: Union[int, float, str, List, Type[np.ndarray], None],
+        timestamps: Union[int, float, str, List, Type[np.ndarray], None],
         unit: Optional[str] = None,
-        extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]] = None,
+        extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray], None]]] = {},
         timestamps_unit: Optional[str] = None,
-        timestamp_extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]] = None,
+        timestamp_extra_metadata: Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray], None]]] = {},
     ):
         """Add new positional field to component that data was collected as a TimeSeries.
 
         Args:
             name (str): Field name.
-            value (Union[int, float, str, List, Type[np.ndarray]]): Value related to field
+            value (Union[int, float, str, List, Type[np.ndarray], None]): Value related to field
             collected data.
-            timestamps (Union[int, float, str, List, Type[np.ndarray]]): Timestamps related to data collected
+            timestamps (Union[int, float, str, List, Type[np.ndarray], None]): Timestamps related to data collected
             from the field.
             unit (Optional[str], optional): Measurement unit related to value parameter.
             Defaults to None.
-            extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]], optional): Dictionary
-            containing any aditional metadata related to collected data. Defaults to None.
+            extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray],
+            None]]], optional): Dictionary
+            containing any aditional metadata related to collected data. Defaults to {}.
             timestamps_unit (Optional[str], optional): Measurement unit related to
             timestamp field. Defaults to None.
-            timestamp_extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray]]]], optional):
-            Dictionary containing extra metadata about timestamps field. Defaults to None.
+            timestamp_extra_metadata (Optional[Dict[str, Union[int, float, str, List, Type[np.ndarray],
+            None]]], optional): Dictionary
+            containing extra metadata about timestamps field. Defaults to {}.
         """
         try:
             new_field = TimeSeries(
                 value=DataField(
                     value=value,
                     unit=unit,
-                    extra_metadata={} if extra_metadata is None else extra_metadata,
+                    extra_metadata=extra_metadata,
                 ),
                 timestamps=DataField(
                     value=timestamps,
                     unit=timestamps_unit,
-                    extra_metadata={} if timestamp_extra_metadata is None else timestamp_extra_metadata,
+                    extra_metadata=timestamp_extra_metadata,
                 ),
             )
         except Exception as e:
-            raise AssonantDataClassesError(f"Failed to create DataField Data Handler for {self.name} Component.") from e
+            raise AssonantDataClassesError(
+                f"Failed to create TimeSeries Data Handler for {self.name} Component."
+            ) from e
         if name not in self.fields:
             self.fields[name] = new_field
         else:
             raise AssonantDataClassesError(f"Field name already exists on: {self.name} Component.")
```

### Comparing `assonant-1.2.0/assonant/data_classes/components/sensor.py` & `assonant-1.3.0/assonant/data_classes/components/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Assonant Sensor component data class."""
 
-from ..types import MeasurementType
+from ..enums import MeasurementType
 from .component import Component
 
 
 class Sensor(Component):
     """Data class to handle all data required to define a sensor with a specific measurement.
 
     This class was created handle measurements that are not necessarly related to a specific device.
```

### Comparing `assonant-1.2.0/assonant/data_classes/data_handlers/axis.py` & `assonant-1.3.0/assonant/data_classes/data_handlers/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Assonant Axis data handler."""
 from typing import Union
 
-from ..types import TransformationType
+from ..enums import TransformationType
 from .data_field import DataField
 from .data_handler import DataHandler
 from .time_series import TimeSeries
 
 
 class Axis(DataHandler):
     """Data class to handle data related to an axis position.
```

### Comparing `assonant-1.2.0/assonant/data_classes/events/assonant_event.py` & `assonant-1.3.0/assonant/data_classes/events/assonant_event.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/data_sender/_assonant_data_sender_interface.py` & `assonant-1.3.0/assonant/data_sender/_assonant_data_sender_interface.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/data_sender/_data_sender_factory.py` & `assonant-1.3.0/assonant/data_sender/_data_sender_factory.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/data_sender/_kafka_data_sender.py` & `assonant-1.3.0/assonant/data_sender/_kafka_data_sender.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/data_sender/assonant_data_sender.py` & `assonant-1.3.0/assonant/data_sender/assonant_data_sender.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/file_writer/_assonant_file_writer_interface.py` & `assonant-1.3.0/assonant/file_writer/_assonant_file_writer_interface.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/file_writer/_file_writer_factory.py` & `assonant-1.3.0/assonant/file_writer/_file_writer_factory.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/file_writer/_nexus_file_writer.py` & `assonant-1.3.0/assonant/file_writer/_nexus_file_writer.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant/file_writer/assonant_file_writer.py` & `assonant-1.3.0/assonant/file_writer/assonant_file_writer.py`

 * *Files identical despite different names*

### Comparing `assonant-1.2.0/assonant.egg-info/PKG-INFO` & `assonant-1.3.0/assonant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assonant
-Version: 1.2.0
+Version: 1.3.0
 Summary: (Meta)Data standardization package for Sirius, the 4th generation brazillian synchrotron light source
 Author: Data Science and Management Group @ GCD
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,15 +25,15 @@
     Welcome to Assonant 🎶 𝄇
 </h1>
 <p align="center">
     <em>A beamline-agnostic event processing engine for data collection and organization</em>
 </p>
 <p align="center">
 <a href="https://gitlab.cnpem.br/GCD/data-management/assonant#readme" target="_blank">
-    <img alt="Version" src="https://img.shields.io/badge/version-1.2.0-blue.svg?cacheSeconds=2592000"/>
+    <img alt="Version" src="https://img.shields.io/badge/version-1.3.0-blue.svg?cacheSeconds=2592000"/>
 </a>
 <a href="https://gitlab.cnpem.br/GCD/data-science/data-management/assonant/commits/dev" target="_blank">
     <img alt="Maintenance" src="https://img.shields.io/badge/Developing%3F-yes-green.svg"/>
 </a>
 <a href="https://pypi.org/project/fastapi" target="_blank">
     <img src="https://img.shields.io/badge/pyversions-3.7|3.8|3.9|3.10-orange" alt="Supported Python versions">
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: assonant Version: 1.2.0 Summary: (Meta)Data
+Metadata-Version: 2.1 Name: assonant Version: 1.3.0 Summary: (Meta)Data
 standardization package for Sirius, the 4th generation brazillian synchrotron
 light source Author: Data Science and Management Group @ GCD Classifier:
 License :: OSI Approved :: GNU Lesser General Public License v3 or later
 (LGPLv3+) Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist: annotated-
```

### Comparing `assonant-1.2.0/assonant.egg-info/SOURCES.txt` & `assonant-1.3.0/assonant.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 assonant/data_classes/assonant_data_class.py
 assonant/data_classes/entry.py
 assonant/data_classes/exceptions.py
 assonant/data_classes/components/__init__.py
 assonant/data_classes/components/attenuator.py
 assonant/data_classes/components/beam.py
 assonant/data_classes/components/beam_stopper.py
+assonant/data_classes/components/beamline.py
 assonant/data_classes/components/bending_magnet.py
 assonant/data_classes/components/bvs.py
 assonant/data_classes/components/collimator.py
 assonant/data_classes/components/component.py
+assonant/data_classes/components/cryojet.py
 assonant/data_classes/components/detector.py
+assonant/data_classes/components/dewar.py
 assonant/data_classes/components/fresnel_zone_plate.py
+assonant/data_classes/components/granite_base.py
 assonant/data_classes/components/mirror.py
 assonant/data_classes/components/monochromator.py
 assonant/data_classes/components/pinhole.py
 assonant/data_classes/components/sample.py
 assonant/data_classes/components/sensor.py
 assonant/data_classes/components/shutter.py
 assonant/data_classes/components/slit.py
@@ -37,21 +41,22 @@
 assonant/data_classes/components/wiggler.py
 assonant/data_classes/data_handlers/__init__.py
 assonant/data_classes/data_handlers/axis.py
 assonant/data_classes/data_handlers/data_field.py
 assonant/data_classes/data_handlers/data_handler.py
 assonant/data_classes/data_handlers/external_link.py
 assonant/data_classes/data_handlers/time_series.py
+assonant/data_classes/enums/__init__.py
+assonant/data_classes/enums/beamline_name.py
+assonant/data_classes/enums/measurement_type.py
+assonant/data_classes/enums/scope_type.py
+assonant/data_classes/enums/transformation_type.py
 assonant/data_classes/events/__init__.py
 assonant/data_classes/events/assonant_event.py
 assonant/data_classes/events/experiment_done.py
-assonant/data_classes/types/__init__.py
-assonant/data_classes/types/measurement_type.py
-assonant/data_classes/types/scope_type.py
-assonant/data_classes/types/transformation_type.py
 assonant/data_sender/__init__.py
 assonant/data_sender/_assonant_data_sender_interface.py
 assonant/data_sender/_data_sender_factory.py
 assonant/data_sender/_kafka_data_sender.py
 assonant/data_sender/assonant_data_sender.py
 assonant/data_sender/exceptions.py
 assonant/file_writer/__init__.py
```

### Comparing `assonant-1.2.0/pyproject.toml` & `assonant-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "assonant"
-version="1.2.0"
+version="1.3.0"
 description = "(Meta)Data standardization package for Sirius, the 4th generation brazillian synchrotron light source"
 authors = [
     {name = "Data Science and Management Group @ GCD"}
 ]
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.7"
```

