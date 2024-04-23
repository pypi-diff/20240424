# Comparing `tmp/neon-skill-update-2.1.3a5.tar.gz` & `tmp/neon-skill-update-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-update-2.1.3a5.tar", last modified: Mon Apr 22 20:43:14 2024, max compression
+gzip compressed data, was "neon-skill-update-3.0.0.tar", last modified: Tue Apr 23 23:26:26 2024, max compression
```

## Comparing `neon-skill-update-2.1.3a5.tar` & `neon-skill-update-3.0.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:43:14.697986 neon-skill-update-2.1.3a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-22 20:43:14.697986 neon-skill-update-2.1.3a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    31812 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:43:14.685986 neon-skill-update-2.1.3a5/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:43:14.685986 neon-skill-update-2.1.3a5/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:43:14.697986 neon-skill-update-2.1.3a5/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/alpha.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/ask_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/ask_download_image.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/ask_overwrite_drive.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/ask_update_anyways.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/ask_update_configuration.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/beta.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/check_error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/check_updates.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/confirm_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/confirm_no_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/core_version.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/downloading_image.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/drive_instructions.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/error_installing_os.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/error_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/error_unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/error_updating_os.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/help_online.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/help_support.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/no_image_file.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/no_valid_device.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/not_updating.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_download_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_download_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_downloading_os.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_downloading_update.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_installation_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_os_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_update_failure.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_update_success.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/notify_writing_image.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/point.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/starting_installation.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/starting_update.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/up_to_date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/update_continuing.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/update_core.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/update_in_progress.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/update_initramfs_success.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/update_os.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/update_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/update_system.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/update_track_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/word_beta.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/dialog/word_stable.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:43:14.697986 neon-skill-update-2.1.3a5/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/intent/core_version.intent
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/intent/update_configuration.intent
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/intent/update_device.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:43:14.697986 neon-skill-update-2.1.3a5/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/vocab/beta.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/vocab/create.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/vocab/media.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/vocab/os.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/vocab/stable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/locale/en-us/vocab/updates.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:43:14.697986 neon-skill-update-2.1.3a5/neon_skill_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-22 20:43:14.000000 neon-skill-update-2.1.3a5/neon_skill_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-22 20:43:14.000000 neon-skill-update-2.1.3a5/neon_skill_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:43:14.000000 neon-skill-update-2.1.3a5/neon_skill_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-22 20:43:14.000000 neon-skill-update-2.1.3a5/neon_skill_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-22 20:43:14.000000 neon-skill-update-2.1.3a5/neon_skill_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 20:43:14.000000 neon-skill-update-2.1.3a5/neon_skill_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 20:43:14.697986 neon-skill-update-2.1.3a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:43:14.697986 neon-skill-update-2.1.3a5/test/
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-22 20:43:11.000000 neon-skill-update-2.1.3a5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:26:26.483059 neon-skill-update-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-23 23:26:26.483059 neon-skill-update-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    31812 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:26:26.471058 neon-skill-update-3.0.0/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:26:26.471058 neon-skill-update-3.0.0/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:26:26.479058 neon-skill-update-3.0.0/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/alpha.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/ask_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/ask_download_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/ask_overwrite_drive.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/ask_update_anyways.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/ask_update_configuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/check_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/check_updates.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/confirm_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/confirm_no_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/core_version.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/downloading_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/drive_instructions.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/error_installing_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/error_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/error_unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/error_updating_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/help_online.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/help_support.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/no_image_file.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/no_valid_device.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/not_updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_download_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_download_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_downloading_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_downloading_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_installation_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_os_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_update_failure.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_update_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/notify_writing_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/point.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/starting_installation.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/starting_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/up_to_date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/update_continuing.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/update_core.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/update_in_progress.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/update_initramfs_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/update_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/update_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/update_system.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/update_track_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/word_beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/dialog/word_stable.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:26:26.483059 neon-skill-update-3.0.0/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/intent/core_version.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/intent/update_configuration.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/intent/update_device.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:26:26.483059 neon-skill-update-3.0.0/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/vocab/beta.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/vocab/create.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/vocab/media.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/vocab/os.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/vocab/stable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/locale/en-us/vocab/updates.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:26:26.483059 neon-skill-update-3.0.0/neon_skill_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-23 23:26:26.000000 neon-skill-update-3.0.0/neon_skill_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-23 23:26:26.000000 neon-skill-update-3.0.0/neon_skill_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:26:26.000000 neon-skill-update-3.0.0/neon_skill_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:26:26.000000 neon-skill-update-3.0.0/neon_skill_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 23:26:26.000000 neon-skill-update-3.0.0/neon_skill_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 23:26:26.000000 neon-skill-update-3.0.0/neon_skill_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:26:26.483059 neon-skill-update-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:26:26.483059 neon-skill-update-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-23 23:26:05.000000 neon-skill-update-3.0.0/version.py
```

### Comparing `neon-skill-update-2.1.3a5/LICENSE.md` & `neon-skill-update-3.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a5/PKG-INFO` & `neon-skill-update-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 2.1.3a5
+Version: 3.0.0
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-2.1.3a5/README.md` & `neon-skill-update-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a5/__init__.py` & `neon-skill-update-3.0.0/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a5/neon_skill_update.egg-info/PKG-INFO` & `neon-skill-update-3.0.0/neon_skill_update.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 2.1.3a5
+Version: 3.0.0
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-2.1.3a5/neon_skill_update.egg-info/SOURCES.txt` & `neon-skill-update-3.0.0/neon_skill_update.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a5/setup.py` & `neon-skill-update-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a5/skill.json` & `neon-skill-update-3.0.0/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a5/test/test_skill.py` & `neon-skill-update-3.0.0/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a5/version.py` & `neon-skill-update-3.0.0/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.1.3a5"
+__version__ = "3.0.0"
```

