# Comparing `tmp/nitrokeyapp-2.2.2.tar.gz` & `tmp/nitrokeyapp-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrokeyapp-2.2.2.tar", max compression
+gzip compressed data, was "nitrokeyapp-2.3.0.tar", max compression
```

## Comparing `nitrokeyapp-2.2.2.tar` & `nitrokeyapp-2.3.0.tar`

### file list

```diff
@@ -1,86 +1,92 @@
--rw-r--r--   0        0        0    11357 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/LICENSE
--rw-r--r--   0        0        0     1117 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/README.md
--rw-r--r--   0        0        0        7 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/VERSION
--rw-r--r--   0        0        0      468 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/__init__.py
--rw-r--r--   0        0        0     1128 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/__main__.py
--rw-r--r--   0        0        0     1824 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/device_data.py
--rw-r--r--   0        0        0      480 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/device_view.py
--rw-r--r--   0        0        0     1281 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/error_dialog.py
--rw-r--r--   0        0        0       45 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/exceptions.py
--rw-r--r--   0        0        0    13336 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/gui.py
--rw-r--r--   0        0        0     3112 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/information_box.py
--rw-r--r--   0        0        0     1801 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/logger.py
--rw-r--r--   0        0        0     2304 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/nk3_button.py
--rw-r--r--   0        0        0     5021 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/overview_tab.py
--rw-r--r--   0        0        0     3520 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/qt_utils_mix_in.py
--rw-r--r--   0        0        0    28064 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/secrets_tab/__init__.py
--rw-r--r--   0        0        0     3553 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/secrets_tab/data.py
--rw-r--r--   0        0        0     2341 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/secrets_tab/ui.py
--rw-r--r--   0        0        0    21486 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/secrets_tab/worker.py
--rw-r--r--   0        0        0      278 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/3RDPARTY.txt
--rw-r--r--   0        0        0    35147 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/LICENSES/GPLv3
--rw-r--r--   0        0        0     7652 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/LICENSES/LGPLv3
--rw-r--r--   0        0        0     1093 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/LICENSES/MIT
--rw-r--r--   0        0        0     4337 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/add_secret_dialog.ui
--rw-r--r--   0        0        0     2303 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/error_dialog.ui
--rw-r--r--   0        0        0       55 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/CMakeLists.txt
--rw-r--r--   0        0        0    26999 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_arabic.qm
--rw-r--r--   0        0        0    73416 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_arabic.ts
--rw-r--r--   0        0        0    77531 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_de_DE.qm
--rw-r--r--   0        0        0    81884 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_de_DE.ts
--rw-r--r--   0        0        0    44748 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_en.qm
--rw-r--r--   0        0        0    68806 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_en.ts
--rw-r--r--   0        0        0    66398 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_fr.qm
--rw-r--r--   0        0        0    82364 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_fr.ts
--rw-r--r--   0        0        0    76801 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_it.qm
--rw-r--r--   0        0        0    84421 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_it.ts
--rw-r--r--   0        0        0    77737 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_pl.qm
--rw-r--r--   0        0        0    82418 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_pl.ts
--rw-r--r--   0        0        0    50434 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/HiddenVolumes_0.png
--rw-r--r--   0        0        0     4524 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/OTP_generate.svg
--rw-r--r--   0        0        0    34411 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/ProgressWheel.GIF
--rw-r--r--   0        0        0      448 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/add_circle.svg
--rw-r--r--   0        0        0    20621 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/app_logo.svg
--rw-r--r--   0        0        0      872 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/black_nitrokey-app-icon.svg
--rw-r--r--   0        0        0      203 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/close.svg
--rw-r--r--   0        0        0      321 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/content_copy.svg
--rw-r--r--   0        0        0      300 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/delete.svg
--rw-r--r--   0        0        0     1113 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/dialpad.svg
--rw-r--r--   0        0        0    81265 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/dialpad_off.svg
--rw-r--r--   0        0        0      159 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/done.svg
--rw-r--r--   0        0        0    47547 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/down_arrow.svg
--rw-r--r--   0        0        0      310 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/edit.svg
--rw-r--r--   0        0        0      390 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/encrypted.svg
--rw-r--r--   0        0        0      676 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/help.svg
--rw-r--r--   0        0        0      224 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/home.svg
--rw-r--r--   0        0        0      709 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/info.svg
--rw-r--r--   0        0        0      856 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/lock.svg
--rw-r--r--   0        0        0      847 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/lock_open.svg
--rw-r--r--   0        0        0     7587 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/nitrokey.svg
--rw-r--r--   0        0        0    34473 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/progressWheel2.gif
--rw-r--r--   0        0        0     5856 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/red_nitrokey-app-icon.svg
--rw-r--r--   0        0        0      314 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/refresh.svg
--rw-r--r--   0        0        0    13157 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/right_arrow.svg
--rw-r--r--   0        0        0     1130 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/save.svg
--rw-r--r--   0        0        0     2049 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/settings.svg
--rw-r--r--   0        0        0      568 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/touch.svg
--rw-r--r--   0        0        0     3158 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/touch_off.svg
--rw-r--r--   0        0        0      535 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/visibility.svg
--rw-r--r--   0        0        0      656 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/visibility_off.svg
--rw-r--r--   0        0        0      984 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/warning.svg
--rw-r--r--   0        0        0     2003 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/licensedialog.ui
--rw-r--r--   0        0        0    16426 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/mainwindow.ui
--rw-r--r--   0        0        0      399 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/nitrokey_theme.xml
--rw-r--r--   0        0        0    16581 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/overview_tab.ui
--rw-r--r--   0        0        0    25436 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/secrets_tab.ui
--rw-r--r--   0        0        0     3633 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/securitydialog.ui
--rw-r--r--   0        0        0    13809 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/settings.ui
--rw-r--r--   0        0        0    14584 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui/welcome_tab.ui
--rw-r--r--   0        0        0     3044 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/ui_loader.py
--rw-r--r--   0        0        0    12440 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/update.py
--rw-r--r--   0        0        0     2046 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/welcome_tab.py
--rw-r--r--   0        0        0     2152 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/windows_notification.py
--rw-r--r--   0        0        0     1746 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/nitrokeyapp/worker.py
--rw-r--r--   0        0        0     1988 2024-03-05 12:46:40.000000 nitrokeyapp-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 nitrokeyapp-2.2.2/setup.py
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 nitrokeyapp-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1117 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/README.md
+-rw-r--r--   0        0        0        7 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/VERSION
+-rw-r--r--   0        0        0      468 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/__init__.py
+-rw-r--r--   0        0        0     1128 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/__main__.py
+-rw-r--r--   0        0        0      486 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/common_ui.py
+-rw-r--r--   0        0        0     2864 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/device_data.py
+-rw-r--r--   0        0        0     2940 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/device_manager.py
+-rw-r--r--   0        0        0      587 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/device_view.py
+-rw-r--r--   0        0        0     1281 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/error_dialog.py
+-rw-r--r--   0        0        0       45 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/exceptions.py
+-rw-r--r--   0        0        0    11447 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/gui.py
+-rw-r--r--   0        0        0     3653 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/information_box.py
+-rw-r--r--   0        0        0     1801 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/logger.py
+-rw-r--r--   0        0        0     2559 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/nk3_button.py
+-rw-r--r--   0        0        0     6869 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/overview_tab/__init__.py
+-rw-r--r--   0        0        0     1886 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/overview_tab/worker.py
+-rw-r--r--   0        0        0     1513 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/progress_box.py
+-rw-r--r--   0        0        0      998 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/prompt_box.py
+-rw-r--r--   0        0        0     3520 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/qt_utils_mix_in.py
+-rw-r--r--   0        0        0    31294 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/secrets_tab/__init__.py
+-rw-r--r--   0        0        0     3553 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/secrets_tab/data.py
+-rw-r--r--   0        0        0     2341 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/secrets_tab/ui.py
+-rw-r--r--   0        0        0    23023 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/secrets_tab/worker.py
+-rw-r--r--   0        0        0     1563 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/touch.py
+-rw-r--r--   0        0        0      278 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/3RDPARTY.txt
+-rw-r--r--   0        0        0    35147 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/LICENSES/GPLv3
+-rw-r--r--   0        0        0     7652 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/LICENSES/LGPLv3
+-rw-r--r--   0        0        0     1093 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/LICENSES/MIT
+-rw-r--r--   0        0        0     4337 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/add_secret_dialog.ui
+-rw-r--r--   0        0        0     2303 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/error_dialog.ui
+-rw-r--r--   0        0        0       55 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/CMakeLists.txt
+-rw-r--r--   0        0        0    26999 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_arabic.qm
+-rw-r--r--   0        0        0    73416 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_arabic.ts
+-rw-r--r--   0        0        0    77531 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_de_DE.qm
+-rw-r--r--   0        0        0    81884 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_de_DE.ts
+-rw-r--r--   0        0        0    44748 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_en.qm
+-rw-r--r--   0        0        0    68806 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_en.ts
+-rw-r--r--   0        0        0    66398 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_fr.qm
+-rw-r--r--   0        0        0    82364 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_fr.ts
+-rw-r--r--   0        0        0    76801 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_it.qm
+-rw-r--r--   0        0        0    84421 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_it.ts
+-rw-r--r--   0        0        0    77737 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_pl.qm
+-rw-r--r--   0        0        0    82418 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_pl.ts
+-rw-r--r--   0        0        0    50434 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/HiddenVolumes_0.png
+-rw-r--r--   0        0        0     4524 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/OTP_generate.svg
+-rw-r--r--   0        0        0    34411 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/ProgressWheel.GIF
+-rw-r--r--   0        0        0      448 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/add_circle.svg
+-rw-r--r--   0        0        0    20621 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/app_logo.svg
+-rw-r--r--   0        0        0      872 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/black_nitrokey-app-icon.svg
+-rw-r--r--   0        0        0      203 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/close.svg
+-rw-r--r--   0        0        0      321 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/content_copy.svg
+-rw-r--r--   0        0        0      300 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/delete.svg
+-rw-r--r--   0        0        0     1113 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/dialpad.svg
+-rw-r--r--   0        0        0    81265 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/dialpad_off.svg
+-rw-r--r--   0        0        0      159 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/done.svg
+-rw-r--r--   0        0        0    47547 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/down_arrow.svg
+-rw-r--r--   0        0        0      310 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/edit.svg
+-rw-r--r--   0        0        0      390 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/encrypted.svg
+-rw-r--r--   0        0        0      676 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/help.svg
+-rw-r--r--   0        0        0      224 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/home.svg
+-rw-r--r--   0        0        0      709 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/info.svg
+-rw-r--r--   0        0        0      856 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/lock.svg
+-rw-r--r--   0        0        0      847 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/lock_open.svg
+-rw-r--r--   0        0        0     7587 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/nitrokey.svg
+-rw-r--r--   0        0        0    34473 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/progressWheel2.gif
+-rw-r--r--   0        0        0     5856 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/red_nitrokey-app-icon.svg
+-rw-r--r--   0        0        0      314 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/refresh.svg
+-rw-r--r--   0        0        0    13157 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/right_arrow.svg
+-rw-r--r--   0        0        0     1130 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/save.svg
+-rw-r--r--   0        0        0     2049 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/settings.svg
+-rw-r--r--   0        0        0      568 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/touch.svg
+-rw-r--r--   0        0        0     3158 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/touch_off.svg
+-rw-r--r--   0        0        0      535 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/visibility.svg
+-rw-r--r--   0        0        0      656 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/visibility_off.svg
+-rw-r--r--   0        0        0      984 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/warning.svg
+-rw-r--r--   0        0        0     2003 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/licensedialog.ui
+-rw-r--r--   0        0        0    16757 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/mainwindow.ui
+-rw-r--r--   0        0        0      399 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/nitrokey_theme.xml
+-rw-r--r--   0        0        0    15634 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/overview_tab.ui
+-rw-r--r--   0        0        0    25436 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/secrets_tab.ui
+-rw-r--r--   0        0        0     3633 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/securitydialog.ui
+-rw-r--r--   0        0        0    13809 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/settings.ui
+-rw-r--r--   0        0        0    14584 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui/welcome_tab.ui
+-rw-r--r--   0        0        0     3044 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/ui_loader.py
+-rw-r--r--   0        0        0     7994 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/update.py
+-rw-r--r--   0        0        0     2050 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/welcome_tab.py
+-rw-r--r--   0        0        0     2152 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/windows_notification.py
+-rw-r--r--   0        0        0     1594 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/nitrokeyapp/worker.py
+-rw-r--r--   0        0        0     1998 2024-04-19 08:38:46.000000 nitrokeyapp-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 nitrokeyapp-2.3.0/setup.py
+-rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 nitrokeyapp-2.3.0/PKG-INFO
```

### Comparing `nitrokeyapp-2.2.2/LICENSE` & `nitrokeyapp-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/README.md` & `nitrokeyapp-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/__main__.py` & `nitrokeyapp-2.3.0/nitrokeyapp/__main__.py`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/error_dialog.py` & `nitrokeyapp-2.3.0/nitrokeyapp/error_dialog.py`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/gui.py` & `nitrokeyapp-2.3.0/nitrokeyapp/gui.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,99 +3,38 @@
 import webbrowser
 from types import TracebackType
 from typing import Optional, Type
 
 if platform.system() == "Linux":
     import pyudev
 
-# Nitrokey 3
-from pynitrokey.nk3 import Nitrokey3Device
-
-# pyqt5
 from PySide6 import QtWidgets
-from PySide6.QtCore import Qt, QTimer, Signal, Slot
+from PySide6.QtCore import Qt, Signal, Slot
 from PySide6.QtGui import QCursor
 
 from nitrokeyapp.device_data import DeviceData
+from nitrokeyapp.device_manager import DeviceManager
 from nitrokeyapp.device_view import DeviceView
 from nitrokeyapp.error_dialog import ErrorDialog
 from nitrokeyapp.information_box import InfoBox
 from nitrokeyapp.nk3_button import Nk3Button
 from nitrokeyapp.overview_tab import OverviewTab
-
-# from nitrokeyapp.loading_screen import LoadingScreen
+from nitrokeyapp.progress_box import ProgressBox
+from nitrokeyapp.prompt_box import PromptBox
 from nitrokeyapp.qt_utils_mix_in import QtUtilsMixIn
 from nitrokeyapp.secrets_tab import SecretsTab
+from nitrokeyapp.touch import TouchIndicator
 
 # import wizards and stuff
 from nitrokeyapp.welcome_tab import WelcomeTab
 from nitrokeyapp.windows_notification import WindowsUSBNotifi
 
 logger = logging.getLogger(__name__)
 
 
-class TouchDialog(QtWidgets.QMessageBox):
-    def __init__(self, parent: QtWidgets.QWidget) -> None:
-        super().__init__(parent)
-
-        self.setWindowModality(Qt.WindowModality.ApplicationModal)
-        self.setWindowTitle("Touch Confirmation")
-        self.setText("Press the button on the Nitrokey 3 if the LED blinks.")
-
-    @Slot()
-    def start(self) -> None:
-        self.show()
-
-    @Slot()
-    def stop(self) -> None:
-        self.close()
-
-
-class TouchIndicator(QtWidgets.QWidget):
-    def __init__(self, info_box: InfoBox, parent: "GUI") -> None:
-        super().__init__(parent)
-
-        # TODO: dont pass entire top-lvl obj
-        self.owner = parent
-        self.active_btn: Optional[Nk3Button] = None
-        self.info_box = info_box
-
-        # show status bar info 750ms late
-        t = QTimer(self)
-        t.setSingleShot(True)
-        t.setInterval(750)
-        t.timeout.connect(self.info_box.set_touch_status)
-        self.info_box_timer: QTimer = t
-
-    @Slot()
-    def start(self) -> None:
-        if self.active_btn:
-            return
-
-        self.info_box_timer.start()
-
-        for btn in self.owner.device_buttons:
-            if btn.data == self.owner.selected_device:
-                self.active_btn = btn
-                break
-        if self.active_btn:
-            self.active_btn.start_touch()
-
-    @Slot()
-    def stop(self) -> None:
-        if self.active_btn:
-            self.active_btn.stop_touch()
-            self.active_btn = None
-
-        # self.info_box.hide_status()
-        if self.info_box_timer.isActive():
-            self.info_box_timer.stop()
-        self.info_box.hide_touch()
-
-
 class GUI(QtUtilsMixIn, QtWidgets.QMainWindow):
     trigger_handle_exception = Signal(object, BaseException, object)
     sig_device_change = Signal(object)
 
     def __init__(self, qt_app: QtWidgets.QApplication, log_file: str):
         QtWidgets.QMainWindow.__init__(self)
         QtUtilsMixIn.__init__(self)
@@ -113,17 +52,19 @@
             self.observer.start()
 
         # windows
         if platform.system() == "Windows":
             logger.info("OS:Windows")
             WindowsUSBNotifi(self.detect_added_devices, self.detect_removed_devices)
 
-        self.devices: list[DeviceData] = []
+        # self.devices: list[DeviceData] = []
+        self.device_manager = DeviceManager()
         self.device_buttons: list[Nk3Button] = []
         self.selected_device: Optional[DeviceData] = None
+
         self.log_file = log_file
 
         self.trigger_handle_exception.connect(self.handle_exception)
 
         # loads main ui
         # self.ui === self -> this tricks mypy due to monkey-patching self
         self.ui = self.load_ui("mainwindow.ui", self)
@@ -132,47 +73,65 @@
             self.ui.information_frame,
             self.ui.status_icon,
             self.ui.status,
             self.ui.device_info,
             self.ui.pin_icon,
         )
 
+        self.prompt_box = PromptBox(self)
+
+        self.progress_box = ProgressBox(self.ui.progress_bar)
+
         self.welcome_widget = WelcomeTab(self.log_file, self)
 
         # hint for mypy
         self.content = self.ui.content
         self.content.layout().addWidget(self.welcome_widget)
 
-        # self.touch_dialog = TouchDialog(self)
         self.touch_dialog = TouchIndicator(self.info_box, self)
 
-        self.overview_tab = OverviewTab(self.info_box, self)
-        self.secrets_tab = SecretsTab(self.info_box, self)
+        self.overview_tab = OverviewTab(self)
+        self.secrets_tab = SecretsTab(self)
+
         self.views: list[DeviceView] = [self.overview_tab, self.secrets_tab]
         for view in self.views:
             if view.worker:
+
                 view.worker.busy_state_changed.connect(self.set_busy)
-                view.worker.error.connect(self.handle_error)
-                view.worker.start_touch.connect(self.touch_dialog.start)
-                view.worker.stop_touch.connect(self.touch_dialog.stop)
+
+                view.common_ui.touch.start.connect(self.touch_dialog.start)
+                view.common_ui.touch.stop.connect(self.touch_dialog.stop)
+
+                view.common_ui.info.info.connect(self.info_box.set_status)
+                view.common_ui.info.error.connect(self.info_box.set_error_status)
+                view.common_ui.info.pin_cached.connect(self.info_box.set_pin_icon)
+                view.common_ui.info.pin_cleared.connect(self.info_box.unset_pin_icon)
+                self.info_box.pin_pressed.connect(view.common_ui.info.pin_pressed)
+
+                view.common_ui.prompt.confirm.connect(self.prompt_box.confirm)
+                self.prompt_box.confirmed.connect(view.common_ui.prompt.confirmed)
+
+                view.common_ui.progress.start.connect(self.progress_box.show)
+                view.common_ui.progress.stop.connect(self.progress_box.hide)
+                view.common_ui.progress.progress.connect(self.progress_box.update)
 
         # main window widgets
         self.home_button = self.ui.btn_home
         self.help_btn = self.ui.btn_dial_help
 
         self.l_insert_nitrokey = self.ui.label_insert_Nitrokey
 
         # set some props, initial enabled/visible, finally show()
         self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
 
         # hint for mypy
         self.tabs = self.ui.tabs
         for view in self.views:
             self.tabs.addTab(view.widget, view.title)
-        self.tabs.currentChanged.connect(self.slot_tab_changed)
+        self.tabs.currentChanged.connect(self.tab_changed)
 
         # set some spacing between Nitrokey buttons
         self.ui.nitrokeyButtonsLayout.setSpacing(8)
         self.sig_device_change.connect(self.device_connect)
 
         self.help_btn.clicked.connect(
             lambda: webbrowser.open("https://docs.nitrokey.com/nitrokey3")
@@ -188,195 +147,165 @@
             logger.info("device removed event")
             self.detect_removed_devices()
 
         elif action == "bind":
             logger.info("device bind event")
             self.detect_added_devices()
 
-    @Slot(object, BaseException, object)
-    def handle_exception(
-        self,
-        ty: Type[BaseException],
-        e: BaseException,
-        tb: Optional[TracebackType],
-    ) -> None:
-        logger.error("Unhandled exception", exc_info=(ty, e, tb))
-
-        dialog = ErrorDialog(self.log_file, self)
-        dialog.set_exception(ty, e, tb)
-
     def toggle_update_btn(self) -> None:
-        device_count = len(self.devices)
+        device_count = self.device_manager.count()
         if device_count == 0:
             self.l_insert_nitrokey.show()
-        self.overview_tab.set_update_enabled(device_count == 1)
+        self.overview_tab.set_update_enabled(device_count <= 1)
 
     def detect_added_devices(self) -> None:
-        try:
-            nk3_list = Nitrokey3Device.list()
-        except Exception as e:
-            logger.info(repr(e))
+        devs = self.device_manager.add()
+
+        # show device as the connection might been updated
+        if len(devs) == 0 and self.selected_device:
+            self.show_device(self.selected_device)
+
+        if not devs:
+            logger.info("failed adding device")
             return
 
-        if len(nk3_list):
-            list_of_added = [device.uuid_prefix for device in self.devices]
-            logger.info(f"list of added: {list_of_added}")
-            for device in nk3_list:
-                data = DeviceData(device)
-                if data.uuid_prefix not in list_of_added:
-                    if data.uuid:
-                        logger.info(f"{data.path}: Nitrokey 3 {data.uuid}")
-                    else:
-                        logger.info(f"{data.path}: Nitrokey 3 without UUID")
-                    self.add_device(data)
-                    logger.info("nk3 connected")
-                    self.l_insert_nitrokey.hide()
-                    self.toggle_update_btn()
-                else:
-                    if (
-                        self.selected_device
-                        and self.selected_device.uuid_prefix == data.uuid_prefix
-                        and self.selected_device.path != data.path
-                    ):
-                        self.selected_device = data
-                        self.refresh()
-        else:
-            logger.info("no nk3 in list. no admin?")
+        # add as nk3 device
+        logger.info(f"nk3 connected: {devs}")
+        desc = ", ".join(
+            (str(dev.uuid) if not dev.is_bootloader else "NK3 (BL)") for dev in devs
+        )
+
+        self.info_box.set_status(f"Nitrokey 3 added: {desc}")
+        for dev in devs:
+            self.add_device(dev)
 
     def detect_removed_devices(self) -> None:
-        list_of_removed: list[DeviceData] = []
-        if self.devices:
-            try:
-                nk3_list = [device.uuid() for device in Nitrokey3Device.list()]
-            except Exception as e:
-                logger.info(f"detect removed failed: {e}")
-                return
-            logger.info(f"list nk3: {nk3_list}")
-
-            list_of_removed = [
-                data
-                for data in self.devices
-                if ((data.uuid not in nk3_list) and not data.updating)
-            ]
-
-        for data in list_of_removed:
-            self.remove_device(data)
-
-        if list_of_removed:
-            who = [d.uuid_prefix for d in list_of_removed]
-            logger.info(f"nk3 instance(s) removed: {' '.join(who)}")
-            self.info_box.set_status(f"Nitrokey 3 removed: {' '.join(who)}")
-            self.toggle_update_btn()
+        devs = self.device_manager.remove()
+        if not devs:
+            logger.info("failed removing device")
+            return
+
+        desc = ", ".join(
+            (str(dev.uuid) if not dev.is_bootloader else "NK3 (BL)") for dev in devs
+        )
+        self.info_box.set_status(f"Nitrokey 3 removed: {desc}")
+        logger.info(f"nk3 disconnected: {devs}")
+        for dev in devs:
+            self.remove_device(dev)
 
     def add_device(self, data: DeviceData) -> None:
+        self.toggle_update_btn()
+
         button = Nk3Button(data)
-        button.clicked.connect(lambda: self.device_selected(data))
+        button.clicked.connect(lambda: self.show_device(data))
         self.ui.nitrokeyButtonsLayout.addWidget(button)
-        self.devices.append(data)
         self.device_buttons.append(button)
-        if self.selected_device:
-            button.fold()
-        self.widget_show()
+
+        if not self.selected_device:
+            self.selected_device = data
+
+        self.l_insert_nitrokey.hide()
 
     def remove_device(self, data: DeviceData) -> None:
+        self.toggle_update_btn()
         if self.selected_device == data:
             self.selected_device = None
-            self.refresh()
+            self.hide_device()
+
+        def remove_button(btn: Nk3Button) -> None:
+            self.ui.nitrokeyButtonsLayout.removeWidget(button)
+            self.device_buttons.remove(button)
+            button.destroy()
 
         for button in self.device_buttons:
-            if button.data.uuid == data.uuid:
-                self.ui.nitrokeyButtonsLayout.removeWidget(button)
-                self.device_buttons.remove(button)
-                button.close()
-
-        self.devices.remove(data)
-        self.widget_show()
-
-    def refresh(self, set_busy: bool = True) -> None:
-        """
-        Should be called if the selected device or the selected tab is changed
-        """
-        if set_busy:
-            self.overview_tab.busy_state_changed.connect(self.set_busy)
-
-        if self.selected_device:
-            self.welcome_widget.hide()
-            self.info_box.set_device(f"Nitrokey 3 - {self.selected_device.uuid_prefix}")
-            self.views[self.tabs.currentIndex()].refresh(self.selected_device)
-            self.tabs.show()
-
-            self.ui.vertical_navigation.setMinimumWidth(80)
-            self.ui.vertical_navigation.setMaximumWidth(80)
-            self.ui.btn_dial_help.hide()
-            for btn in self.device_buttons:
-                btn.fold()
-            self.ui.main_logo.setMaximumWidth(48)
-            self.ui.main_logo.setMaximumHeight(48)
-            self.ui.main_logo.setMinimumWidth(48)
-            self.ui.main_logo.setMinimumHeight(48)
+            if button.data.is_bootloader:
+                if button.data.path == data.path:
+                    remove_button(button)
+            elif button.data.uuid == data.uuid:
+                remove_button(button)
 
-        else:
-            self.info_box.hide_device()
-            for view in self.views:
-                view.reset()
-            self.tabs.hide()
-
-            self.ui.vertical_navigation.setMinimumWidth(200)
-            self.ui.btn_dial_help.show()
-            for btn in self.device_buttons:
-                btn.unfold()
-            self.ui.main_logo.setMaximumWidth(120)
-            self.ui.main_logo.setMaximumHeight(120)
-            self.ui.main_logo.setMinimumWidth(64)
-            self.ui.main_logo.setMinimumHeight(64)
+        if self.device_manager.count() == 0:
+            self.l_insert_nitrokey.show()
 
     def init_gui(self) -> None:
-        self.tabs.hide()
+        self.hide_device()
         self.detect_added_devices()
+        device_count = self.device_manager.count()
+        if device_count == 1:
+            data = self.device_manager._devices[0]
+            self.show_device(data)
+
+        self.overview_tab.busy_state_changed.connect(self.set_busy)
 
-    def device_selected(self, data: DeviceData) -> None:
+    def show_navigation(self) -> None:
+        for btn in self.device_buttons:
+            btn.fold()
+
+        self.ui.vertical_navigation.setMinimumWidth(80)
+        self.ui.vertical_navigation.setMaximumWidth(80)
+        self.ui.btn_dial_help.hide()
+
+        self.ui.main_logo.setMaximumWidth(48)
+        self.ui.main_logo.setMaximumHeight(48)
+        self.ui.main_logo.setMinimumWidth(48)
+        self.ui.main_logo.setMinimumHeight(48)
+
+    def hide_navigation(self) -> None:
+        for btn in self.device_buttons:
+            btn.unfold()
+
+        self.ui.vertical_navigation.setMinimumWidth(200)
+        self.ui.vertical_navigation.setMaximumWidth(200)
+        self.ui.btn_dial_help.show()
+
+        self.ui.main_logo.setMaximumWidth(120)
+        self.ui.main_logo.setMaximumHeight(120)
+        self.ui.main_logo.setMinimumWidth(64)
+        self.ui.main_logo.setMinimumHeight(64)
+
+    def show_device(self, data: DeviceData) -> None:
         self.selected_device = data
-        self.info_box.set_device(f"Nitrokey 3 - {data.uuid_prefix}")
-        self.refresh()
+        for btn in self.device_buttons:
+            if btn.data == data:
+                btn.setChecked(True)
+            else:
+                btn.setChecked(False)
+
+        self.info_box.set_device(data.name)
+        self.tabs.show()
+        self.tabs.setCurrentIndex(0)
+        self.show_navigation()
+        self.welcome_widget.hide()
+
+        # enforce refreshing the current view
+        view = self.views[self.tabs.currentIndex()]
+        view.refresh(data, force=True)
 
-    def widget_show(self) -> None:
-        device_count = len(self.devices)
-        if device_count == 1:
-            data = self.devices[0]
-            self.device_selected(data)
-            # TODO: solve centrally
-            self.tabs.setCurrentIndex(0)
-        else:
-            self.tabs.hide()
-            self.welcome_widget.show()
-            self.selected_device = None
-            self.info_box.hide_device()
-            self.refresh(set_busy=False)
+    def hide_device(self) -> None:
+        self.selected_device = None
+
+        self.info_box.hide_device()
+        self.tabs.hide()
+        self.hide_navigation()
+        self.welcome_widget.show()
 
     @Slot(int)
-    def slot_tab_changed(self, idx: int) -> None:
-        # TODO: not a good place
-        for view in self.views:
-            view.reset()
+    def tab_changed(self, idx: int) -> None:
+        view = self.views[self.tabs.currentIndex()]
+        view.refresh(self.selected_device)
+
         if idx == 0:
             self.info_box.pin_icon.hide()
         else:
             self.info_box.pin_icon.show()
 
-        self.refresh()
-
     # main-window callbacks
     @Slot()
     def home_button_pressed(self) -> None:
-        for view in self.views:
-            view.reset()
-        self.welcome_widget.show()
-        self.tabs.hide()
-        self.selected_device = None
-        self.refresh()
+        self.hide_device()
 
     @Slot(bool)
     def set_busy(self, busy: bool) -> None:
         if busy:
             self.setCursor(QCursor(Qt.CursorShape.WaitCursor))
             self.home_button.setEnabled(False)
             self.tabs.setEnabled(False)
@@ -384,12 +313,25 @@
             self.unsetCursor()
             self.home_button.setEnabled(True)
             self.tabs.setEnabled(True)
 
         # TODO: setEnabled?
         # self.setEnabled(not busy)
 
+    # error & exception handling
     @Slot(str, Exception)
     def handle_error(self, sender: str, exc: Exception) -> None:
         msg = f"{sender} - {exc}"
         self.info_box.set_error_status(msg)
         # self.user_err(msg, "Error", self)
+
+    @Slot(object, BaseException, object)
+    def handle_exception(
+        self,
+        ty: Type[BaseException],
+        e: BaseException,
+        tb: Optional[TracebackType],
+    ) -> None:
+        logger.error("Unhandled exception", exc_info=(ty, e, tb))
+
+        dialog = ErrorDialog(self.log_file, self)
+        dialog.set_exception(ty, e, tb)
```

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/logger.py` & `nitrokeyapp-2.3.0/nitrokeyapp/logger.py`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/nk3_button.py` & `nitrokeyapp-2.3.0/nitrokeyapp/nk3_button.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+from typing import Optional
+
 from PySide6 import QtCore, QtGui, QtWidgets
 from qt_material import apply_stylesheet
 
 from nitrokeyapp import get_theme_path
 from nitrokeyapp.device_data import DeviceData
 from nitrokeyapp.qt_utils_mix_in import QtUtilsMixIn
 
 
 class Nk3Button(QtWidgets.QPushButton):
     def __init__(
         self,
         data: DeviceData,
     ) -> None:
-        super().__init__(
-            QtUtilsMixIn.get_qicon("nitrokey.svg"),
-            "Nitrokey 3: " f"{data.uuid_prefix}",
-        )
+        super().__init__(QtUtilsMixIn.get_qicon("nitrokey.svg"), data.name)
+
         self.data = data
+        self.bootloader_data: Optional[DeviceData] = None
+
         # needs to create button in the vertical navigation with the nitrokey type and serial number as text
         # set material stylesheet if no system theme is set
         if not self.style().objectName() or self.style().objectName() == "fusion":
             apply_stylesheet(self, theme=get_theme_path())
 
+        self.setCheckable(True)
+        self.setDefault(False)
+        self.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
+
         self.effect = QtWidgets.QGraphicsColorizeEffect(self)
         self.effect.setColor(QtGui.QColor(115, 215, 125))
         self.effect.setStrength(0)
         self.setGraphicsEffect(self.effect)
 
         anims = QtCore.QSequentialAnimationGroup()
 
@@ -57,10 +63,14 @@
     def stop_touch(self) -> None:
         self.animation.stop()
         self.setToolTip("")
         self.effect.setStrength(0)
 
     def fold(self) -> None:
         self.setText("")
+        self.setMinimumWidth(58)
+        self.setMaximumWidth(58)
 
     def unfold(self) -> None:
-        self.setText("Nitrokey 3: " f"{str(self.data.uuid)[:5]}")
+        self.setText(self.data.name)
+        self.setMinimumWidth(178)
+        self.setMaximumWidth(178)
```

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/qt_utils_mix_in.py` & `nitrokeyapp-2.3.0/nitrokeyapp/qt_utils_mix_in.py`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/secrets_tab/__init__.py` & `nitrokeyapp-2.3.0/nitrokeyapp/secrets_tab/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from random import randbytes
 from typing import Callable, Optional
 
 from PySide6.QtCore import Qt, QThread, QTimer, Signal, Slot
 from PySide6.QtGui import QGuiApplication
 from PySide6.QtWidgets import QLineEdit, QListWidgetItem, QWidget
 
+from nitrokeyapp.common_ui import CommonUi
 from nitrokeyapp.device_data import DeviceData
-from nitrokeyapp.information_box import InfoBox
 from nitrokeyapp.qt_utils_mix_in import QtUtilsMixIn
 from nitrokeyapp.worker import Worker
 
 from .data import Credential, OtherKind, OtpData, OtpKind
 from .worker import SecretsWorker
 
 # TODO:
@@ -62,43 +62,38 @@
     trigger_check_device = Signal(DeviceData)
     trigger_delete_credential = Signal(DeviceData, Credential)
     trigger_generate_otp = Signal(DeviceData, Credential)
     trigger_refresh_credentials = Signal(DeviceData, bool)
     trigger_get_credential = Signal(DeviceData, Credential)
     trigger_edit_credential = Signal(DeviceData, Credential, bytes, bytes)
 
-    def __init__(self, info_box: InfoBox, parent: Optional[QWidget] = None) -> None:
+    def __init__(self, parent: Optional[QWidget] = None) -> None:
         QWidget.__init__(self, parent)
         QtUtilsMixIn.__init__(self)
 
-        self.info_box = info_box
+        self.common_ui = CommonUi()
 
         self.worker_thread = QThread()
-        self._worker = SecretsWorker(self)
+        self._worker = SecretsWorker(self.common_ui, self)
         self._worker.moveToThread(self.worker_thread)
         self.worker_thread.start()
 
         self.trigger_add_credential.connect(self._worker.add_credential)
         self.trigger_check_device.connect(self._worker.check_device)
         self.trigger_delete_credential.connect(self._worker.delete_credential)
         self.trigger_generate_otp.connect(self._worker.generate_otp)
         self.trigger_refresh_credentials.connect(self._worker.refresh_credentials)
         self.trigger_get_credential.connect(self._worker.get_credential)
         self.trigger_edit_credential.connect(self._worker.edit_credential)
 
-        self._worker.pin_cache.pin_cleared.connect(
-            lambda: (
-                self.info_box.set_pin_icon(pin_cached=False),
-                self.uncheck_checkbox(True),
-            )
-        )
-        self._worker.pin_cache.pin_cached.connect(
-            lambda: self.info_box.set_pin_icon(pin_cached=True)
-        )
-        self.info_box.pin_icon.pressed.connect(self._worker.pin_cache.clear)
+        self._worker.pin_cache.pin_cleared.connect(self.common_ui.info.pin_cleared)
+        self._worker.pin_cache.pin_cleared.connect(lambda: self.uncheck_checkbox(True))
+
+        self._worker.pin_cache.pin_cached.connect(self.common_ui.info.pin_cached)
+        self.common_ui.info.pin_pressed.connect(self._worker.pin_cache.clear)
 
         self._worker.credential_added.connect(self.credential_added)
         self._worker.credential_deleted.connect(self.credential_deleted)
         self._worker.credentials_listed.connect(self.credentials_listed)
         self._worker.credential_edited.connect(self.credential_edited)
         self._worker.device_checked.connect(self.device_checked)
         self._worker.otp_generated.connect(self.otp_generated)
@@ -179,16 +174,19 @@
 
         self.ui.btn_add.pressed.connect(self.add_new_credential)
         self.ui.btn_abort.pressed.connect(lambda: self.show_secrets(True))
         self.ui.btn_save.pressed.connect(self.save_credential)
         self.ui.btn_edit.pressed.connect(self.prepare_edit_credential)
 
         self.ui.name.textChanged.connect(self.check_credential)
+        self.ui.username.textChanged.connect(self.check_credential)
+        self.ui.password.textChanged.connect(self.check_credential)
         self.ui.otp.textChanged.connect(self.check_credential)
         self.ui.select_algorithm.currentIndexChanged.connect(self.check_credential)
+        self.ui.comment.textChanged.connect(self.check_credential)
 
         self.ui.btn_refresh.pressed.connect(self.refresh_credential_list)
         self.ui.is_protected.stateChanged.connect(self.refresh_credential_list)
         self.ui.secrets_list.currentItemChanged.connect(self.credential_changed)
         self.ui.secrets_list.itemClicked.connect(self.credential_clicked)
 
         self.ui.btn_delete.pressed.connect(self.delete_credential)
@@ -230,17 +228,18 @@
             self.ui.page_incompatible.show()
             self.hide_credential()
 
     def refresh(self, data: DeviceData) -> None:
         if data == self.data:
             return
         self.data = data
+        self._worker.pin_cache.clear()
 
         self.reset_ui()
-        self.trigger_check_device.emit(data)
+        self.trigger_check_device.emit(self.data)
 
     @Slot(bool)
     def device_checked(self, compatible: bool) -> None:
         self.show_secrets(compatible)
         if compatible:
             self.refresh_credential_list()
 
@@ -288,14 +287,15 @@
         if active_item:
             self.ui.secrets_list.setCurrentItem(active_item)
 
     @Slot(OtpData)
     def otp_generated(self, data: OtpData) -> None:
         self.ui.otp.setText(data.otp)
         self.data_otp = data.otp
+        self.common_ui.info.info.emit("Secret is generated")
 
         if data.validity:
             start, end = data.validity
             period = int((end - start).total_seconds())
             self.ui.otp_timeout_progress.setMaximum(period + period)
 
             self.otp_timeout = end + (end - start)
@@ -363,37 +363,38 @@
         self.ui.btn_abort.hide()
         self.ui.btn_save.hide()
         self.ui.btn_delete.hide()
         self.ui.btn_edit.show()
 
         self.ui.name.hide()
         self.ui.name_label.show()
+        self.ui.name.setText(credential.name)
         self.ui.name_label.setText(credential.name)
 
         if credential.login:
             self.ui.username.setText(credential.login.decode(errors="replace"))
             self.action_username_copy.setEnabled(True)
         else:
-            self.ui.username.setText("")
+            self.ui.username.clear()
             self.action_username_copy.setEnabled(False)
 
         if credential.password:
             self.ui.password.setText(credential.password.decode(errors="replace"))
             self.action_password_copy.setEnabled(True)
             self.action_password_show.setEnabled(True)
         else:
-            self.ui.password.setText("")
+            self.ui.password.clear()
             self.action_password_copy.setEnabled(False)
             self.action_password_show.setEnabled(False)
 
         if credential.comment:
             self.ui.comment.setText(credential.comment.decode(errors="replace"))
             self.action_comment_copy.setEnabled(True)
         else:
-            self.ui.comment.setText("")
+            self.ui.comment.clear()
             self.action_comment_copy.setEnabled(False)
 
         self.ui.name.setReadOnly(True)
         self.ui.username.setReadOnly(True)
         self.ui.password.setReadOnly(True)
         self.ui.comment.setReadOnly(True)
 
@@ -458,25 +459,25 @@
         self.ui.name.show()
         self.ui.name_label.hide()
         self.ui.name.setText(credential.name)
 
         if credential.login:
             self.ui.username.setText(credential.login.decode(errors="replace"))
         else:
-            self.ui.username.setText("")
+            self.ui.username.clear()
 
         if credential.password:
             self.ui.password.setText(credential.password.decode(errors="replace"))
         else:
-            self.ui.password.setText("")
+            self.ui.password.clear()
 
         if credential.comment:
             self.ui.comment.setText(credential.comment.decode(errors="replace"))
         else:
-            self.ui.comment.setText("")
+            self.ui.comment.clear()
         self.ui.name.setReadOnly(False)
         self.ui.username.setReadOnly(False)
         self.ui.password.setReadOnly(False)
         self.ui.comment.setReadOnly(False)
 
         self.ui.is_pin_protected.setChecked(credential.protected)
         self.ui.is_touch_protected.setChecked(credential.touch_required)
@@ -484,14 +485,15 @@
         self.ui.is_pin_protected.setEnabled(False)
         self.ui.is_touch_protected.setEnabled(True)
 
         self.hide_otp()
 
         self.ui.algorithm_tab.show()
         self.ui.algorithm_tab.setCurrentIndex(0)
+        self.ui.select_algorithm.setMaxCount(3)
         self.ui.algorithm_show.hide()
         self.ui.algorithm_edit.show()
         self.ui.select_algorithm.show()
         self.ui.otp.show()
 
         # already existing otp requires confirmation to change
         if credential.otp or credential.other:
@@ -513,15 +515,15 @@
                 self.ui.algorithm_edit.hide()
                 self.ui.algorithm.setText(str(credential.otp or credential.other) + ":")
                 self.action_otp_edit.setVisible(False)
                 self.ui.otp.setPlaceholderText("<cannot edit>")
 
         # no otp there, just offer it as in add
         else:
-            self.ui.otp.setText("")
+            self.ui.otp.clear()
             self.ui.otp.setReadOnly(False)
             self.ui.otp.setPlaceholderText("<empty>")
             self.ui.select_algorithm.setCurrentText(str(credential.otp))
             self.ui.select_algorithm.setEnabled(True)
 
         self.check_credential()
 
@@ -532,18 +534,17 @@
             self.hide_hmac_view()
 
     def act_enable_otp_edit(self) -> None:
         assert self.active_credential
         self.active_credential.new_secret = True
 
         self.ui.otp.setReadOnly(False)
-        self.ui.select_algorithm.setMaxCount(3)
         self.ui.select_algorithm.setEnabled(True)
         self.ui.otp.setPlaceholderText("<empty>")
-        self.ui.otp.setText("")
+        self.ui.otp.clear()
 
         self.check_credential()
 
     @Slot()
     def add_new_credential(self) -> None:
 
         if not self.data:
@@ -558,20 +559,21 @@
         for action in self.line_actions:
             action.setVisible(False)
         self.action_password_show.setVisible(True)
         self.action_password_show.setEnabled(True)
 
         self.ui.name.show()
         self.ui.name_label.hide()
-        self.ui.name.setText("")
+        self.ui.name.clear()
 
-        self.ui.otp.setText("")
-        self.ui.username.setText("")
-        self.ui.password.setText("")
-        self.ui.comment.setText("")
+        self.ui.otp.clear()
+        self.ui.otp.setPlaceholderText("<empty>")
+        self.ui.username.clear()
+        self.ui.password.clear()
+        self.ui.comment.clear()
 
         self.ui.name.setReadOnly(False)
         self.ui.otp.setReadOnly(False)
         self.ui.username.setReadOnly(False)
         self.ui.password.setReadOnly(False)
         self.ui.comment.setReadOnly(False)
 
@@ -602,41 +604,97 @@
         self.ui.btn_edit.hide()
         self.ui.btn_save.show()
 
         self.check_credential()
 
     @Slot()
     def check_credential(self) -> None:
+        self.common_ui.info.info.emit("")
+
+        tool_Tip = "Credeantial cannot be saved:"
         can_save = True
+        check_secret = self.ui.otp.text()
 
-        otp_secret = self.ui.otp.text()
+        name_len = len(str.encode(self.ui.name.text()))
+        username_len = len(str.encode(self.ui.username.text()))
+        password_len = len(str.encode(self.ui.password.text()))
+        comment_len = len(str.encode(self.ui.comment.text()))
 
         algo = self.ui.select_algorithm.currentText()
+
+        if len(self.ui.name.text()) < 3:
+            can_save = False
+        if len(self.ui.name.text()) == 0:
+            self.common_ui.info.info.emit("Enter a Credential Name")
+            tool_Tip = tool_Tip + "\n- Enter a Credential Name"
+        if len(self.ui.name.text()) >= 1 and len(self.ui.name.text()) < 3:
+            self.common_ui.info.info.emit("Credential Name is too short")
+            tool_Tip = tool_Tip + "\n- Credential Name is too short"
+        if name_len >= 128:
+            can_save = False
+            self.common_ui.info.info.emit("Credential Name is too long")
+            tool_Tip = tool_Tip + "\n- Credential Name is too long"
+
+        if username_len >= 128:
+            can_save = False
+            self.common_ui.info.info.emit("Username is too long")
+            tool_Tip = tool_Tip + "\n- Username is too long"
+
+        if password_len >= 128:
+            can_save = False
+            self.common_ui.info.info.emit("Password is too long")
+            tool_Tip = tool_Tip + "\n- Password is too long"
+
+        if comment_len >= 128:
+            can_save = False
+            self.common_ui.info.info.emit("Comment is too long")
+            tool_Tip = tool_Tip + "\n- Comment is too long"
+
         if self.ui.select_algorithm.isEnabled():
+            if algo == "None":
+                self.ui.otp.setReadOnly(True)
+                self.ui.otp.setPlaceholderText("<Select Algotithm>")
+            else:
+                self.ui.otp.setReadOnly(False)
+                self.ui.otp.setPlaceholderText("<empty>")
+
             if algo == "HMAC":
                 self.show_hmac_view()
-                if len(otp_secret) != 32:
+                if len(check_secret) != 32:
                     can_save = False
+                    self.common_ui.info.info.emit(
+                        "The HMAC-Secret is not 32 chars long"
+                    )
+                    tool_Tip = tool_Tip + "\n- The HMAC-Secret is not 32 chars long"
             else:
                 self.hide_hmac_view()
 
-            if algo != "None" and not is_base32(otp_secret):
+            if algo != "None" and len(check_secret) != len(check_secret.encode()):
                 can_save = False
-
-            if algo != "None" and len(otp_secret) < 1:
+                self.common_ui.info.info.emit("Invalid character in Secret")
+                tool_Tip = tool_Tip + "\n- Invalid character in Secret"
+            elif not is_base32(check_secret) and len(check_secret) > 1:
                 can_save = False
+                self.common_ui.info.info.emit("Secret is not in Base32")
+                tool_Tip = tool_Tip + "\n- Secret is not in Base32"
 
-        if len(self.ui.name.text()) < 3:
-            can_save = False
+            if algo != "None" and len(check_secret) < 1:
+                can_save = False
+                self.common_ui.info.info.emit("Enter a Secret")
+                tool_Tip = tool_Tip + "\n- Enter a Secret"
 
         self.ui.btn_save.setEnabled(can_save)
+        if can_save:
+            tool_Tip = "Credential Save"
+
+        self.ui.btn_save.setToolTip(tool_Tip)
 
     def act_copy_line_edit(self, obj: QLineEdit) -> None:
         self.clipboard.setText(obj.text())
-        self.info_box.set_status("contents copied to clipboard")
+        self.common_ui.info.info.emit("contents copied to clipboard")
         self.line2copy_action[obj].setIcon(self.get_qicon("done.svg"))
         QTimer.singleShot(
             5000,
             lambda: self.line2copy_action[obj].setIcon(
                 self.get_qicon("content_copy.svg")
             ),
         )
@@ -693,14 +751,23 @@
         self.ui.is_pin_protected.hide()
 
         self.ui.is_touch_protection_label.hide()
         self.ui.is_touch_protected.hide()
 
     def hide_hmac_view(self) -> None:
 
+        if self.active_credential is None and self.ui.name_label.text() == "HmacSlot2":
+            self.ui.name_label.clear()
+            self.ui.name_label.hide()
+            self.ui.name.clear()
+            self.ui.name.show()
+            self.ui.otp.clear()
+
+        self.action_hmac_gen.setVisible(False)
+
         self.ui.username_label.show()
         self.ui.username.show()
 
         self.ui.password_label.show()
         self.ui.password.show()
 
         self.ui.comment_label.show()
```

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/secrets_tab/data.py` & `nitrokeyapp-2.3.0/nitrokeyapp/secrets_tab/data.py`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/secrets_tab/ui.py` & `nitrokeyapp-2.3.0/nitrokeyapp/secrets_tab/ui.py`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/secrets_tab/worker.py` & `nitrokeyapp-2.3.0/nitrokeyapp/secrets_tab/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Dict, Optional
 
 from pynitrokey.nk3.secrets_app import SecretsApp, SecretsAppException
-from pynitrokey.nk3.utils import Uuid
+from pynitrokey.trussed.utils import Uuid
 from PySide6.QtCore import QObject, Signal, Slot
 from PySide6.QtWidgets import QWidget
 
+from nitrokeyapp.common_ui import CommonUi
 from nitrokeyapp.device_data import DeviceData
 from nitrokeyapp.worker import Job, Worker
 
 from .data import Credential, OtpData, OtpKind
 from .ui import PinUi
 
 logger = logging.getLogger(__name__)
@@ -21,16 +22,16 @@
 class PinCache(QObject):
     uuid: Optional[Uuid] = None
     pin: Optional[str] = None
 
     pin_cached = Signal()
     pin_cleared = Signal()
 
-    def __init__(self, *v: tuple, **kw: dict) -> None:
-        super().__init__(*v, **kw)  # type: ignore [arg-type]
+    def __init__(self) -> None:
+        super().__init__()
 
     @Slot()
     def clear(self) -> None:
         self.uuid = None
         self.pin = None
         self.pin_cleared.emit()
 
@@ -48,16 +49,20 @@
 
         self.pin_cached.emit()
 
 
 class CheckDeviceJob(Job):
     device_checked = Signal(bool)
 
-    def __init__(self, data: DeviceData) -> None:
-        super().__init__()
+    def __init__(
+        self,
+        common_ui: CommonUi,
+        data: DeviceData,
+    ) -> None:
+        super().__init__(common_ui)
 
         self.data = data
 
         self.device_checked.connect(lambda _: self.finished.emit())
 
     def run(self) -> None:
         compatible = False
@@ -81,20 +86,21 @@
 
     # internal signals
     query_pin = Signal(int)
     choose_pin = Signal()
 
     def __init__(
         self,
+        common_ui: CommonUi,
         pin_cache: PinCache,
         pin_ui: PinUi,
         data: DeviceData,
         set_pin: bool = False,
     ) -> None:
-        super().__init__()
+        super().__init__(common_ui)
 
         self.pin_cache = pin_cache
         self.data = data
         self.set_pin = set_pin
 
         self.pin_verified.connect(lambda _: self.finished.emit())
 
@@ -153,45 +159,47 @@
         if select.pin_attempt_counter:
             self.pin_queried(pin)
         else:
             self.trigger_error("Failed to set Secrets PIN")
 
     @Slot(str)
     def trigger_error(self, msg: str) -> None:
-        self.error.emit(self.__class__.__name__, Exception(msg))
+        self.common_ui.info.error.emit(msg)
         self.pin_verified.emit(False)
 
 
 class EditCredentialJob(Job):
     credential_edited = Signal(Credential)
 
     def __init__(
         self,
+        common_ui: CommonUi,
         pin_cache: PinCache,
         pin_ui: PinUi,
         data: DeviceData,
         credential: Credential,
         secret: bytes,
         old_cred_id: bytes,
     ) -> None:
-        super().__init__()
+        super().__init__(common_ui)
 
         self.pin_cache = pin_cache
         self.pin_ui = pin_ui
         self.data = data
         self.credential = credential
         self.secret = secret
         self.old_cred_id = old_cred_id
 
         self.all_credentials: Optional[Dict[bytes, Credential]] = None
 
         self.credential_edited.connect(lambda _: self.finished.emit())
 
     def run(self) -> None:
         list_credentials_job = ListCredentialsJob(
+            self.common_ui,
             self.pin_cache,
             self.pin_ui,
             self.data,
             pin_protected=True,
         )
         list_credentials_job.credentials_listed.connect(self.check_credential)
         self.spawn(list_credentials_job)
@@ -214,14 +222,15 @@
             self.trigger_error(
                 f"A credential with the name {self.credential.name} does already exist."
             )
             return
 
         if self.credential.protected:
             verify_pin_job = VerifyPinJob(
+                self.common_ui,
                 self.pin_cache,
                 self.pin_ui,
                 self.data,
                 set_pin=self.credential.protected,
             )
             verify_pin_job.pin_verified.connect(self.edit_credential)
             self.spawn(verify_pin_job)
@@ -249,15 +258,20 @@
                 temp_cred_id = self.temp_rename_credential(self.old_cred_id)
                 self.add_credential(self.credential, self.secret, temp_cred_id)
 
     def add_credential(
         self, cred: Credential, secret: bytes, then_delete_id: bytes
     ) -> None:
         add_job = AddCredentialJob(
-            self.pin_cache, self.pin_ui, self.data, credential=cred, secret=secret
+            self.common_ui,
+            self.pin_cache,
+            self.pin_ui,
+            self.data,
+            credential=cred,
+            secret=secret,
         )
         add_job.credential_added.connect(
             lambda cred: self.handle_created(cred, then_delete_id)
         )
         self.spawn(add_job)
 
     @Slot(Credential)
@@ -269,14 +283,15 @@
     def delete_credential(self, cred_id: bytes) -> None:
         cred = Credential(
             id=cred_id,
             protected=self.credential.protected,
             touch_required=self.credential.touch_required,
         )
         del_job = DeleteCredentialJob(
+            self.common_ui,
             self.pin_cache,
             self.pin_ui,
             self.data,
             credential=cred,
         )
         del_job.credential_deleted.connect(self.handle_deleted)
         self.spawn(del_job)
@@ -331,32 +346,34 @@
 
 
 class AddCredentialJob(Job):
     credential_added = Signal(Credential)
 
     def __init__(
         self,
+        common_ui: CommonUi,
         pin_cache: PinCache,
         pin_ui: PinUi,
         data: DeviceData,
         credential: Credential,
         secret: bytes,
     ) -> None:
-        super().__init__()
+        super().__init__(common_ui)
 
         self.pin_cache = pin_cache
         self.pin_ui = pin_ui
         self.data = data
         self.credential = credential
         self.secret = secret
 
         self.credential_added.connect(lambda _: self.finished.emit())
 
     def run(self) -> None:
         list_credentials_job = ListCredentialsJob(
+            self.common_ui,
             self.pin_cache,
             self.pin_ui,
             self.data,
             pin_protected=True,
         )
         list_credentials_job.credentials_listed.connect(self.check_credential)
         self.spawn(list_credentials_job)
@@ -366,14 +383,15 @@
         ids = set([credential.id for credential in credentials])
         if self.credential.id in ids:
             self.trigger_error(
                 f"A credential with the name {self.credential.name} already exists."
             )
         elif self.credential.protected:
             verify_pin_job = VerifyPinJob(
+                self.common_ui,
                 self.pin_cache,
                 self.pin_ui,
                 self.data,
                 set_pin=self.credential.protected,
             )
             verify_pin_job.pin_verified.connect(self.add_credential)
             self.spawn(verify_pin_job)
@@ -420,32 +438,38 @@
 
 
 class DeleteCredentialJob(Job):
     credential_deleted = Signal(Credential)
 
     def __init__(
         self,
+        common_ui: CommonUi,
         pin_cache: PinCache,
         pin_ui: PinUi,
         data: DeviceData,
         credential: Credential,
     ) -> None:
-        super().__init__()
+        super().__init__(common_ui)
 
         self.pin_cache = pin_cache
         self.pin_ui = pin_ui
         self.data = data
         self.credential = credential
 
         self.credential_deleted.connect(lambda _: self.finished.emit())
 
     def run(self) -> None:
         with self.touch_prompt():
             if self.credential.protected:
-                verify_pin_job = VerifyPinJob(self.pin_cache, self.pin_ui, self.data)
+                verify_pin_job = VerifyPinJob(
+                    self.common_ui,
+                    self.pin_cache,
+                    self.pin_ui,
+                    self.data,
+                )
                 verify_pin_job.pin_verified.connect(self.delete_credential)
                 self.spawn(verify_pin_job)
             else:
                 self.delete_credential()
 
     @Slot()
     def delete_credential(self) -> None:
@@ -463,31 +487,37 @@
 class GenerateOtpJob(Job):
     # TODO: make period and digits configurable
 
     otp_generated = Signal(OtpData)
 
     def __init__(
         self,
+        common_ui: CommonUi,
         pin_cache: PinCache,
         pin_ui: PinUi,
         data: DeviceData,
         credential: Credential,
     ) -> None:
-        super().__init__()
+        super().__init__(common_ui)
 
         self.pin_cache = pin_cache
         self.pin_ui = pin_ui
         self.data = data
         self.credential = credential
 
         self.otp_generated.connect(lambda _: self.finished.emit())
 
     def run(self) -> None:
         if self.credential.protected:
-            verify_pin_job = VerifyPinJob(self.pin_cache, self.pin_ui, self.data)
+            verify_pin_job = VerifyPinJob(
+                self.common_ui,
+                self.pin_cache,
+                self.pin_ui,
+                self.data,
+            )
             verify_pin_job.pin_verified.connect(self.generate_otp)
             self.spawn(verify_pin_job)
         else:
             self.generate_otp()
 
     @Slot()
     def generate_otp(self) -> None:
@@ -517,28 +547,35 @@
 
 
 class ListCredentialsJob(Job):
     credentials_listed = Signal(list)
     uncheck_checkbox = Signal(bool)
 
     def __init__(
-        self, pin_cache: PinCache, pin_ui: PinUi, data: DeviceData, pin_protected: bool
+        self,
+        common_ui: CommonUi,
+        pin_cache: PinCache,
+        pin_ui: PinUi,
+        data: DeviceData,
+        pin_protected: bool,
     ) -> None:
-        super().__init__()
+        super().__init__(common_ui)
 
         self.pin_cache = pin_cache
         self.pin_ui = pin_ui
         self.data = data
         self.pin_protected = pin_protected
 
         self.credentials_listed.connect(lambda _: self.finished.emit())
 
     def run(self) -> None:
         if self.pin_protected:
-            verify_pin_job = VerifyPinJob(self.pin_cache, self.pin_ui, self.data)
+            verify_pin_job = VerifyPinJob(
+                self.common_ui, self.pin_cache, self.pin_ui, self.data
+            )
             verify_pin_job.pin_verified.connect(self.list_protected_credentials)
             self.spawn(verify_pin_job)
         else:
             with self.data.open() as device:
                 secrets = SecretsApp(device)
                 credentials = Credential.list(secrets)
             self.credentials_listed.emit(credentials)
@@ -558,32 +595,38 @@
 
 
 class GetCredentialJob(Job):
     received_credential = Signal(Credential)
 
     def __init__(
         self,
+        common_ui: CommonUi,
         pin_cache: PinCache,
         pin_ui: PinUi,
         data: DeviceData,
         credential: Credential,
     ) -> None:
-        super().__init__()
+        super().__init__(common_ui)
 
         self.pin_cache = pin_cache
         self.pin_ui = pin_ui
         self.data = data
         self.credential = credential
 
         self.received_credential.connect(lambda _: self.finished.emit())
 
     def run(self) -> None:
         with self.touch_prompt():
             if self.credential.protected:
-                verify_pin_job = VerifyPinJob(self.pin_cache, self.pin_ui, self.data)
+                verify_pin_job = VerifyPinJob(
+                    self.common_ui,
+                    self.pin_cache,
+                    self.pin_ui,
+                    self.data,
+                )
                 verify_pin_job.pin_verified.connect(self.get_credential)
                 self.spawn(verify_pin_job)
             else:
                 self.get_credential()
 
     @Slot()
     def get_credential(self) -> None:
@@ -607,65 +650,106 @@
     credential_deleted = Signal(Credential)
     credentials_listed = Signal(list)
     uncheck_checkbox = Signal(bool)
     device_checked = Signal(bool)
     otp_generated = Signal(OtpData)
     received_credential = Signal(Credential)
 
-    def __init__(self, widget: QWidget) -> None:
-        super().__init__()
+    def __init__(
+        self,
+        common_ui: CommonUi,
+        widget: QWidget,
+    ) -> None:
+        super().__init__(common_ui)
 
         self.pin_cache = PinCache()
         self.pin_ui = PinUi(widget)
 
     @Slot(DeviceData)
     def check_device(self, data: DeviceData) -> None:
-        job = CheckDeviceJob(data)
+        job = CheckDeviceJob(self.common_ui, data)
         job.device_checked.connect(self.device_checked)
         self.run(job)
 
     @Slot(DeviceData, Credential, bytes)
     def add_credential(
         self, data: DeviceData, credential: Credential, secret: bytes
     ) -> None:
-        job = AddCredentialJob(self.pin_cache, self.pin_ui, data, credential, secret)
+        job = AddCredentialJob(
+            self.common_ui,
+            self.pin_cache,
+            self.pin_ui,
+            data,
+            credential,
+            secret,
+        )
         job.credential_added.connect(self.credential_added)
         self.run(job)
 
     @Slot(DeviceData, Credential)
     def delete_credential(self, data: DeviceData, credential: Credential) -> None:
-        job = DeleteCredentialJob(self.pin_cache, self.pin_ui, data, credential)
+        job = DeleteCredentialJob(
+            self.common_ui,
+            self.pin_cache,
+            self.pin_ui,
+            data,
+            credential,
+        )
         job.credential_deleted.connect(self.credential_deleted)
         self.run(job)
 
     @Slot(DeviceData, Credential)
     def generate_otp(self, data: DeviceData, credential: Credential) -> None:
-        job = GenerateOtpJob(self.pin_cache, self.pin_ui, data, credential)
+        job = GenerateOtpJob(
+            self.common_ui,
+            self.pin_cache,
+            self.pin_ui,
+            data,
+            credential,
+        )
         job.otp_generated.connect(self.otp_generated)
         self.run(job)
 
     @Slot(DeviceData, bool)
     def refresh_credentials(self, data: DeviceData, pin_protected: bool) -> None:
-        job = ListCredentialsJob(self.pin_cache, self.pin_ui, data, pin_protected)
+        job = ListCredentialsJob(
+            self.common_ui,
+            self.pin_cache,
+            self.pin_ui,
+            data,
+            pin_protected,
+        )
         job.credentials_listed.connect(self.credentials_listed)
         job.uncheck_checkbox.connect(self.uncheck_checkbox)
         self.run(job)
 
     @Slot(DeviceData, Credential)
     def get_credential(self, data: DeviceData, credential: Credential) -> None:
-        job = GetCredentialJob(self.pin_cache, self.pin_ui, data, credential)
+        job = GetCredentialJob(
+            self.common_ui,
+            self.pin_cache,
+            self.pin_ui,
+            data,
+            credential,
+        )
         job.received_credential.connect(self.received_credential)
         self.run(job)
 
     @Slot(DeviceData, Credential, bytes, str)
     def edit_credential(
         self,
         data: DeviceData,
         credential: Credential,
         secret: bytes,
         old_cred_id: bytes,
     ) -> None:
         job = EditCredentialJob(
-            self.pin_cache, self.pin_ui, data, credential, secret, old_cred_id
+            self.common_ui,
+            self.pin_cache,
+            self.pin_ui,
+            data,
+            credential,
+            secret,
+            old_cred_id,
         )
         job.credential_edited.connect(self.credential_edited)
         self.run(job)
```

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/LICENSES/GPLv3` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/LICENSES/GPLv3`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/LICENSES/LGPLv3` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/LICENSES/LGPLv3`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/LICENSES/MIT` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/LICENSES/MIT`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/add_secret_dialog.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/add_secret_dialog.ui`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/error_dialog.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/error_dialog.ui`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_arabic.qm` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_arabic.qm`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_arabic.ts` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_arabic.ts`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_de_DE.qm` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_de_DE.qm`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_de_DE.ts` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_de_DE.ts`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_en.qm` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_en.qm`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_en.ts` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_en.ts`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_fr.qm` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_fr.qm`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_fr.ts` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_fr.ts`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_it.qm` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_it.qm`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_it.ts` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_it.ts`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_pl.qm` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_pl.qm`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/i18n/nitrokey_pl.ts` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/i18n/nitrokey_pl.ts`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/HiddenVolumes_0.png` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/HiddenVolumes_0.png`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/OTP_generate.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/OTP_generate.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/ProgressWheel.GIF` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/ProgressWheel.GIF`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/app_logo.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/app_logo.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/black_nitrokey-app-icon.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/black_nitrokey-app-icon.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/dialpad.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/dialpad.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/dialpad_off.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/dialpad_off.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/down_arrow.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/down_arrow.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/help.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/help.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/info.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/info.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/lock.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/lock_open.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/lock_open.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/nitrokey.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/nitrokey.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/progressWheel2.gif` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/progressWheel2.gif`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/red_nitrokey-app-icon.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/red_nitrokey-app-icon.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/right_arrow.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/right_arrow.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/save.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/save.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/settings.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/touch.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/touch.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/touch_off.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/touch_off.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/visibility.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/visibility.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/visibility_off.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/visibility_off.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/icons/warning.svg` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/licensedialog.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/licensedialog.ui`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/mainwindow.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/mainwindow.ui`

 * *Files 1% similar despite different names*

#### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/mainwindow.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/mainwindow.ui`

```diff
@@ -50,15 +50,15 @@
           <verstretch>0</verstretch>
         </sizepolicy>
       </property>
       <property name="styleSheet">
         <string notr="true"/>
       </property>
       <layout class="QGridLayout" name="gridLayout_2">
-        <item row="1" column="1">
+        <item row="2" column="1">
           <widget class="QFrame" name="information_frame">
             <property name="sizePolicy">
               <sizepolicy hsizetype="Expanding" vsizetype="Preferred">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
@@ -175,15 +175,15 @@
                     </widget>
                   </item>
                 </layout>
               </item>
             </layout>
           </widget>
         </item>
-        <item row="0" column="0" rowspan="2" alignment="Qt::AlignHCenter">
+        <item row="0" column="0" rowspan="3" alignment="Qt::AlignHCenter">
           <widget class="QFrame" name="vertical_navigation">
             <property name="sizePolicy">
               <sizepolicy hsizetype="Fixed" vsizetype="Preferred">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
@@ -527,14 +527,27 @@
                     <bool>false</bool>
                   </property>
                 </widget>
               </item>
             </layout>
           </widget>
         </item>
+        <item row="1" column="1">
+          <widget class="QProgressBar" name="progress_bar">
+            <property name="value">
+              <number>0</number>
+            </property>
+            <property name="textVisible">
+              <bool>true</bool>
+            </property>
+            <property name="format">
+              <string/>
+            </property>
+          </widget>
+        </item>
       </layout>
     </widget>
   </widget>
   <layoutdefault spacing="6" margin="11"/>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/overview_tab.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/overview_tab.ui`

 * *Files 2% similar despite different names*

#### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/overview_tab.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/overview_tab.ui`

```diff
@@ -20,15 +20,15 @@
       <string>Form</string>
     </property>
     <property name="styleSheet">
       <string notr="true"/>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
-        <widget class="QScrollArea" name="scrollArea_2">
+        <widget class="QScrollArea" name="___overview_space">
           <property name="autoFillBackground">
             <bool>false</bool>
           </property>
           <property name="styleSheet">
             <string notr="true">QScrollArea{ border-width: 0px ; }</string>
           </property>
           <property name="frameShape">
@@ -42,35 +42,35 @@
           </property>
           <property name="midLineWidth">
             <number>0</number>
           </property>
           <property name="widgetResizable">
             <bool>true</bool>
           </property>
-          <widget class="QWidget" name="scrollAreaWidgetContents_3">
+          <widget class="QWidget" name="___overview">
             <property name="geometry">
               <rect>
                 <x>0</x>
                 <y>0</y>
-                <width>476</width>
-                <height>342</height>
+                <width>488</width>
+                <height>465</height>
               </rect>
             </property>
             <property name="sizePolicy">
               <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                 <horstretch>0</horstretch>
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <property name="styleSheet">
               <string notr="true"/>
             </property>
             <layout class="QFormLayout" name="formLayout">
               <item row="0" column="0">
-                <widget class="QFrame" name="Nitrokey3">
+                <widget class="QFrame" name="___nk3_info_space">
                   <property name="enabled">
                     <bool>true</bool>
                   </property>
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
@@ -95,15 +95,15 @@
                     <number>5</number>
                   </property>
                   <property name="midLineWidth">
                     <number>5</number>
                   </property>
                   <layout class="QFormLayout" name="formLayout_4">
                     <item row="0" column="0" colspan="2">
-                      <widget class="QLabel" name="label_nk3">
+                      <widget class="QLabel" name="nk3_label">
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="minimumSize">
@@ -123,15 +123,15 @@
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignVCenter</set>
                         </property>
                       </widget>
                     </item>
                     <item row="1" column="0">
-                      <widget class="QLabel" name="label_uuid">
+                      <widget class="QLabel" name="___uuid_label">
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="minimumSize">
@@ -145,25 +145,25 @@
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignVCenter</set>
                         </property>
                       </widget>
                     </item>
                     <item row="1" column="1">
-                      <widget class="QLabel" name="nk3_lineedit_uuid">
+                      <widget class="QLabel" name="nk3_uuid">
                         <property name="text">
                           <string>TextLabel</string>
                         </property>
                         <property name="textInteractionFlags">
                           <set>Qt::LinksAccessibleByMouse|Qt::TextSelectableByKeyboard|Qt::TextSelectableByMouse</set>
                         </property>
                       </widget>
                     </item>
                     <item row="2" column="0">
-                      <widget class="QLabel" name="label_path">
+                      <widget class="QLabel" name="___path_label">
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="minimumSize">
@@ -177,25 +177,25 @@
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignVCenter</set>
                         </property>
                       </widget>
                     </item>
                     <item row="2" column="1">
-                      <widget class="QLabel" name="nk3_lineedit_path">
+                      <widget class="QLabel" name="nk3_path">
                         <property name="text">
                           <string>TextLabel</string>
                         </property>
                         <property name="textInteractionFlags">
                           <set>Qt::LinksAccessibleByMouse|Qt::TextSelectableByKeyboard|Qt::TextSelectableByMouse</set>
                         </property>
                       </widget>
                     </item>
                     <item row="3" column="0">
-                      <widget class="QLabel" name="label_version">
+                      <widget class="QLabel" name="___version_label">
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="minimumSize">
@@ -209,25 +209,25 @@
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignVCenter</set>
                         </property>
                       </widget>
                     </item>
                     <item row="3" column="1">
-                      <widget class="QLabel" name="nk3_lineedit_version">
+                      <widget class="QLabel" name="nk3_version">
                         <property name="text">
                           <string>TextLabel</string>
                         </property>
                         <property name="textInteractionFlags">
                           <set>Qt::LinksAccessibleByMouse|Qt::TextSelectableByKeyboard|Qt::TextSelectableByMouse</set>
                         </property>
                       </widget>
                     </item>
                     <item row="4" column="0">
-                      <widget class="QLabel" name="label_variant">
+                      <widget class="QLabel" name="___variant_label">
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="minimumSize">
@@ -241,25 +241,25 @@
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignVCenter</set>
                         </property>
                       </widget>
                     </item>
                     <item row="4" column="1">
-                      <widget class="QLabel" name="nk3_lineedit_variant">
+                      <widget class="QLabel" name="nk3_variant">
                         <property name="text">
                           <string>TextLabel</string>
                         </property>
                         <property name="textInteractionFlags">
                           <set>Qt::LinksAccessibleByMouse|Qt::TextSelectableByKeyboard|Qt::TextSelectableByMouse</set>
                         </property>
                       </widget>
                     </item>
                     <item row="5" column="0">
-                      <widget class="QLabel" name="label_init_status">
+                      <widget class="QLabel" name="status_label">
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="minimumSize">
@@ -273,27 +273,27 @@
                         </property>
                         <property name="alignment">
                           <set>Qt::AlignLeading|Qt::AlignLeft|Qt::AlignVCenter</set>
                         </property>
                       </widget>
                     </item>
                     <item row="5" column="1">
-                      <layout class="QHBoxLayout" name="horizontalLayout">
+                      <layout class="QHBoxLayout" name="status_space">
                         <item>
-                          <widget class="QLabel" name="nk3_lineedit_init_status">
+                          <widget class="QLabel" name="nk3_status">
                             <property name="text">
                               <string>TextLabel</string>
                             </property>
                             <property name="textInteractionFlags">
                               <set>Qt::LinksAccessibleByMouse|Qt::TextSelectableByKeyboard|Qt::TextSelectableByMouse</set>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="QLabel" name="warnNoticeIcon">
+                          <widget class="QLabel" name="icon_warn_notice">
                             <property name="sizePolicy">
                               <sizepolicy hsizetype="MinimumExpanding" vsizetype="Minimum">
                                 <horstretch>0</horstretch>
                                 <verstretch>0</verstretch>
                               </sizepolicy>
                             </property>
                             <property name="maximumSize">
@@ -325,15 +325,15 @@
                             </property>
                             <property name="openExternalLinks">
                               <bool>true</bool>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="QLabel" name="moreInfo">
+                          <widget class="QLabel" name="more_info">
                             <property name="text">
                               <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;a href=&quot;https://docs.nitrokey.com/nitrokey3/&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#c80636;&quot;&gt;More Info&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                             </property>
                             <property name="openExternalLinks">
                               <bool>true</bool>
                             </property>
                           </widget>
@@ -366,51 +366,51 @@
                             <width>20</width>
                             <height>10</height>
                           </size>
                         </property>
                       </spacer>
                     </item>
                     <item row="7" column="0" colspan="2">
-                      <layout class="QHBoxLayout" name="buttonLayout_nk3">
+                      <layout class="QHBoxLayout" name="___button_layout">
                         <item>
-                          <widget class="QPushButton" name="pushButtonUpdate">
+                          <widget class="QPushButton" name="btn_update">
                             <property name="text">
-                              <string>Update</string>
+                              <string>Check for Update</string>
                             </property>
                           </widget>
                         </item>
                       </layout>
                     </item>
                   </layout>
                 </widget>
               </item>
               <item row="1" column="0">
-                <widget class="QPushButton" name="more_options_btn">
+                <widget class="QPushButton" name="btn_more_options">
                   <property name="text">
                     <string>More Options</string>
                   </property>
                   <property name="icon">
                     <iconset>
-                      <normaloff>icons/right_arrow.svg</normaloff>
-                      icons/right_arrow.svg
+                      <normaloff>icons/right_arrow.png</normaloff>
+                      icons/right_arrow.png
                     </iconset>
                   </property>
                   <property name="checkable">
                     <bool>true</bool>
                   </property>
                   <property name="checked">
                     <bool>false</bool>
                   </property>
                   <property name="flat">
                     <bool>true</bool>
                   </property>
                 </widget>
               </item>
               <item row="2" column="0">
-                <widget class="QFrame" name="more_options_frame">
+                <widget class="QFrame" name="frame_more_options">
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
                   <property name="minimumSize">
@@ -429,60 +429,25 @@
                     <number>5</number>
                   </property>
                   <property name="midLineWidth">
                     <number>5</number>
                   </property>
                   <layout class="QVBoxLayout" name="verticalLayout_2">
                     <item>
-                      <widget class="QPushButton" name="update_with_file_btn">
+                      <widget class="QPushButton" name="btn_update_with_file">
                         <property name="text">
                           <string>Update with local Firmware</string>
                         </property>
                       </widget>
                     </item>
                   </layout>
                 </widget>
               </item>
             </layout>
           </widget>
         </widget>
       </item>
-      <item>
-        <widget class="QProgressBar" name="progressBar_Download">
-          <property name="value">
-            <number>0</number>
-          </property>
-          <property name="textVisible">
-            <bool>true</bool>
-          </property>
-          <property name="format">
-            <string>Download Firmware %p%</string>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QProgressBar" name="progressBar_Update">
-          <property name="value">
-            <number>0</number>
-          </property>
-          <property name="format">
-            <string>Update the Nitrokey %p%</string>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QProgressBar" name="progressBar_Finalization">
-          <property name="value">
-            <number>0</number>
-          </property>
-          <property name="format">
-            <string>Finalization %p%</string>
-          </property>
-        </widget>
-      </item>
     </layout>
   </widget>
-  <resources>
-    <include location="resources.qrc"/>
-  </resources>
+  <resources/>
   <connections/>
 </ui>
```

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/secrets_tab.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/secrets_tab.ui`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/securitydialog.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/securitydialog.ui`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/settings.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/settings.ui`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui/welcome_tab.ui` & `nitrokeyapp-2.3.0/nitrokeyapp/ui/welcome_tab.ui`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/ui_loader.py` & `nitrokeyapp-2.3.0/nitrokeyapp/ui_loader.py`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/welcome_tab.py` & `nitrokeyapp-2.3.0/nitrokeyapp/welcome_tab.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import webbrowser
 from typing import Optional
 
-from pynitrokey.nk3.utils import Version
+from pynitrokey.trussed.utils import Version
 from pynitrokey.updates import Release, Repository
 from PySide6.QtCore import Slot
 from PySide6.QtWidgets import QWidget
 
 from nitrokeyapp import __version__
 from nitrokeyapp.logger import save_log
 from nitrokeyapp.qt_utils_mix_in import QtUtilsMixIn
```

### Comparing `nitrokeyapp-2.2.2/nitrokeyapp/windows_notification.py` & `nitrokeyapp-2.3.0/nitrokeyapp/windows_notification.py`

 * *Files identical despite different names*

### Comparing `nitrokeyapp-2.2.2/pyproject.toml` & `nitrokeyapp-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nitrokeyapp"
-version = "2.2.2"
+version = "2.3.0"
 description = "Graphical application to manage Nitrokey devices"
 authors = [
   "Nitrokey <pypi@nitrokey.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/nitrokey/nitrokey-app2"
@@ -30,15 +30,15 @@
 [tool.poetry.scripts]
 nitrokeyapp = "nitrokeyapp.__main__:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pySide6 = ">=6.6.0"
 pyudev = "^0.24.1"
-pynitrokey = "0.4.45"
+pynitrokey = ">=0.4.46,<0.4.48"
 pywin32 = { version = "305", markers = "sys_platform =='win32'" }
 qt_material = "^2.14"
 
 [tool.poetry.group.dev.dependencies]
 PySide6-stubs = "^6.4.2"
 black = ">=22.1.0,<23"
 flake8 = "^6.1.0"
```

### Comparing `nitrokeyapp-2.2.2/setup.py` & `nitrokeyapp-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['nitrokeyapp', 'nitrokeyapp.secrets_tab']
+['nitrokeyapp', 'nitrokeyapp.overview_tab', 'nitrokeyapp.secrets_tab']
 
 package_data = \
 {'': ['*'], 'nitrokeyapp': ['ui/*', 'ui/LICENSES/*', 'ui/i18n/*', 'ui/icons/*']}
 
 install_requires = \
 ['pySide6>=6.6.0',
- 'pynitrokey==0.4.45',
+ 'pynitrokey>=0.4.46,<0.4.48',
  'pyudev>=0.24.1,<0.25.0',
  'qt_material>=2.14,<3.0']
 
 extras_require = \
 {':sys_platform == "win32"': ['pywin32==305']}
 
 entry_points = \
 {'console_scripts': ['nitrokeyapp = nitrokeyapp.__main__:main']}
 
 setup_kwargs = {
     'name': 'nitrokeyapp',
-    'version': '2.2.2',
+    'version': '2.3.0',
     'description': 'Graphical application to manage Nitrokey devices',
     'long_description': '# Nitrokey App 2\n\nThis application allows to manage Nitrokey 3 devices. To manage Nitrokey Pro and Nitrokey Storage devices, use the older [Nitrokey App](https://github.com/Nitrokey/nitrokey-app).\n\n## Features\n\nThe following features are currently implemented.\n\n- Firmware update\n- Passwords\n    - TOTP\n    - HOTP\n\n## Download\n\nExecutable binaries for Linux and Windows as well as a MSI installer for Windows can be downloaded from the [releases](https://github.com/Nitrokey/nitrokey-app2/releases).\n\n### Compiling for Linux and macOS\n\nThis project uses [Poetry](https://python-poetry.org/) as its dependency management and packaging system.\nSee the [documentation](https://python-poetry.org/docs/) of *Poetry* for available commands.\n\nThe application can be compiled by executing:\n\n```\ngit clone https://github.com/Nitrokey/nitrokey-app2.git\ncd nitrokey-app2\nmake init\nmake build\npoetry shell\nnitrokeyapp\n```\n\n## Dependencies\n\n* [pynitrokey ](https://github.com/Nitrokey/pynitrokey)\n* Python >3.9\n\n## Author\n\nNitrokey GmbH, Jan Suhr and [contributors](https://github.com/Nitrokey/nitrokey-app2/graphs/contributors).\n',
     'author': 'Nitrokey',
     'author_email': 'pypi@nitrokey.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nitrokey/nitrokey-app2',
```

### Comparing `nitrokeyapp-2.2.2/PKG-INFO` & `nitrokeyapp-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitrokeyapp
-Version: 2.2.2
+Version: 2.3.0
 Summary: Graphical application to manage Nitrokey devices
 Home-page: https://github.com/nitrokey/nitrokey-app2
 License: Apache-2.0
 Author: Nitrokey
 Author-email: pypi@nitrokey.com
 Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: pySide6 (>=6.6.0)
-Requires-Dist: pynitrokey (==0.4.45)
+Requires-Dist: pynitrokey (>=0.4.46,<0.4.48)
 Requires-Dist: pyudev (>=0.24.1,<0.25.0)
 Requires-Dist: pywin32 (==305) ; sys_platform == "win32"
 Requires-Dist: qt_material (>=2.14,<3.0)
 Project-URL: Documentation, https://docs.nitrokey.com/software/nk-app2/
 Project-URL: Repository, https://github.com/nitrokey/nitrokey-app2
 Description-Content-Type: text/markdown
```

