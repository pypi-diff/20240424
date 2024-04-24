# Comparing `tmp/udiskie-2.5.2.tar.gz` & `tmp/udiskie-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udiskie-2.5.2.tar", last modified: Fri Jan 26 23:29:39 2024, max compression
+gzip compressed data, was "udiskie-2.5.3.tar", last modified: Wed Apr 24 17:55:06 2024, max compression
```

## Comparing `udiskie-2.5.2.tar` & `udiskie-2.5.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.535805 udiskie-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    15476 2024-01-26 23:29:28.000000 udiskie-2.5.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-01-26 23:29:28.000000 udiskie-2.5.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-26 23:29:28.000000 udiskie-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20851 2024-01-26 23:29:39.535805 udiskie-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-01-26 23:29:28.000000 udiskie-2.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.527804 udiskie-2.5.2/completions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.531804 udiskie-2.5.2/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-01-26 23:29:28.000000 udiskie-2.5.2/completions/bash/udiskie
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-01-26 23:29:28.000000 udiskie-2.5.2/completions/bash/udiskie-info
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-01-26 23:29:28.000000 udiskie-2.5.2/completions/bash/udiskie-mount
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-01-26 23:29:28.000000 udiskie-2.5.2/completions/bash/udiskie-umount
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.531804 udiskie-2.5.2/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-01-26 23:29:28.000000 udiskie-2.5.2/completions/zsh/_udiskie
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-01-26 23:29:28.000000 udiskie-2.5.2/completions/zsh/_udiskie-canonical_paths
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-01-26 23:29:28.000000 udiskie-2.5.2/completions/zsh/_udiskie-mount
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-01-26 23:29:28.000000 udiskie-2.5.2/completions/zsh/_udiskie-umount
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.531804 udiskie-2.5.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-26 23:29:28.000000 udiskie-2.5.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-26 23:29:28.000000 udiskie-2.5.2/doc/asciidoc.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-01-26 23:29:28.000000 udiskie-2.5.2/doc/udiskie.8.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.531804 udiskie-2.5.2/lang/
--rw-r--r--   0 runner    (1001) docker     (127)    18418 2024-01-26 23:29:28.000000 udiskie-2.5.2/lang/de.po
--rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-01-26 23:29:28.000000 udiskie-2.5.2/lang/en_US.po
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-01-26 23:29:28.000000 udiskie-2.5.2/lang/es_ES.po
--rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-01-26 23:29:28.000000 udiskie-2.5.2/lang/it_IT.po
--rw-r--r--   0 runner    (1001) docker     (127)    21089 2024-01-26 23:29:28.000000 udiskie-2.5.2/lang/ru_RU.po
--rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-01-26 23:29:28.000000 udiskie-2.5.2/lang/sk_SK.po
--rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-01-26 23:29:28.000000 udiskie-2.5.2/lang/tr_TR.po
--rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-01-26 23:29:28.000000 udiskie-2.5.2/lang/udiskie.pot
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-26 23:29:39.535805 udiskie-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-01-26 23:29:28.000000 udiskie-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.531804 udiskie-2.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-01-26 23:29:28.000000 udiskie-2.5.2/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-01-26 23:29:28.000000 udiskie-2.5.2/test/test_match.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.535805 udiskie-2.5.2/udiskie/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/appindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/async_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/automount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    25433 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/dbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/depend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.535805 udiskie-2.5.2/udiskie/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-checkbox-checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-checkbox-unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-detach.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-eject.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-lock.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-mount.svg
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-submenu.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-unlock.svg
--rw-r--r--   0 runner    (1001) docker     (127)    33595 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/icons/udiskie-unmount.svg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)    33731 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/password_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/tray.py
--rw-r--r--   0 runner    (1001) docker     (127)    31514 2024-01-26 23:29:28.000000 udiskie-2.5.2/udiskie/udisks2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 23:29:39.535805 udiskie-2.5.2/udiskie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20851 2024-01-26 23:29:39.000000 udiskie-2.5.2/udiskie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-01-26 23:29:39.000000 udiskie-2.5.2/udiskie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 23:29:39.000000 udiskie-2.5.2/udiskie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-26 23:29:39.000000 udiskie-2.5.2/udiskie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-26 23:29:39.000000 udiskie-2.5.2/udiskie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-26 23:29:39.000000 udiskie-2.5.2/udiskie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 23:29:39.000000 udiskie-2.5.2/udiskie.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.366941 udiskie-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-04-24 17:54:50.000000 udiskie-2.5.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-24 17:54:50.000000 udiskie-2.5.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 17:54:50.000000 udiskie-2.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-04-24 17:55:06.366941 udiskie-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-24 17:54:50.000000 udiskie-2.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.362941 udiskie-2.5.3/completions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.362941 udiskie-2.5.3/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 17:54:50.000000 udiskie-2.5.3/completions/bash/udiskie
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 17:54:50.000000 udiskie-2.5.3/completions/bash/udiskie-info
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 17:54:50.000000 udiskie-2.5.3/completions/bash/udiskie-mount
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 17:54:50.000000 udiskie-2.5.3/completions/bash/udiskie-umount
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.362941 udiskie-2.5.3/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-24 17:54:50.000000 udiskie-2.5.3/completions/zsh/_udiskie
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-24 17:54:50.000000 udiskie-2.5.3/completions/zsh/_udiskie-canonical_paths
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-24 17:54:50.000000 udiskie-2.5.3/completions/zsh/_udiskie-mount
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-24 17:54:50.000000 udiskie-2.5.3/completions/zsh/_udiskie-umount
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.362941 udiskie-2.5.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 17:54:50.000000 udiskie-2.5.3/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-24 17:54:50.000000 udiskie-2.5.3/doc/asciidoc.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-24 17:54:50.000000 udiskie-2.5.3/doc/udiskie.8.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.362941 udiskie-2.5.3/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)    18418 2024-04-24 17:54:50.000000 udiskie-2.5.3/lang/de.po
+-rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-04-24 17:54:50.000000 udiskie-2.5.3/lang/en_US.po
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-04-24 17:54:50.000000 udiskie-2.5.3/lang/es_ES.po
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-04-24 17:54:50.000000 udiskie-2.5.3/lang/it_IT.po
+-rw-r--r--   0 runner    (1001) docker     (127)    21089 2024-04-24 17:54:50.000000 udiskie-2.5.3/lang/ru_RU.po
+-rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-24 17:54:50.000000 udiskie-2.5.3/lang/sk_SK.po
+-rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-04-24 17:54:50.000000 udiskie-2.5.3/lang/tr_TR.po
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-04-24 17:54:50.000000 udiskie-2.5.3/lang/udiskie.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 17:55:06.370941 udiskie-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-24 17:54:50.000000 udiskie-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.362941 udiskie-2.5.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-24 17:54:50.000000 udiskie-2.5.3/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-24 17:54:50.000000 udiskie-2.5.3/test/test_match.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.366941 udiskie-2.5.3/udiskie/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/appindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/automount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25482 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/depend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.366941 udiskie-2.5.3/udiskie/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-checkbox-checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-checkbox-unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-detach.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-eject.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-lock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-mount.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-submenu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-unlock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    33595 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/icons/udiskie-unmount.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33731 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/password_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/tray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31514 2024-04-24 17:54:50.000000 udiskie-2.5.3/udiskie/udisks2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:55:06.366941 udiskie-2.5.3/udiskie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-04-24 17:55:06.000000 udiskie-2.5.3/udiskie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 17:55:06.000000 udiskie-2.5.3/udiskie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:55:06.000000 udiskie-2.5.3/udiskie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 17:55:06.000000 udiskie-2.5.3/udiskie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 17:55:06.000000 udiskie-2.5.3/udiskie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 17:55:06.000000 udiskie-2.5.3/udiskie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:55:06.000000 udiskie-2.5.3/udiskie.egg-info/zip-safe
```

### Comparing `udiskie-2.5.2/CHANGES.rst` & `udiskie-2.5.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGELOG
 ---------
 
+2.5.3
+-----
+Date 24.04.2024
+
+- allow matching against a list of values in config rules (``device_config``)
+  [thanks @dajt1725]
+- fix ``--terminal`` command line option (was not doing anything) [@dajt1725]
+- fix AttributeError when *python-keyring-keyutils* is installed instead of
+  *keyutils* [thanks @bubbleguuum]
+
+
 2.5.2
 ~~~~~
 Date: 27.01.2024
 
 - drop external dependency on distutils (#278)
 - rename ``--notify-command`` to ``--event-hook`` to prevent misunderstandings (#279)
```

### Comparing `udiskie-2.5.2/COPYING` & `udiskie-2.5.3/COPYING`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/PKG-INFO` & `udiskie-2.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udiskie
-Version: 2.5.2
+Version: 2.5.3
 Summary: Removable disk automounter for udisks
 Home-page: https://github.com/coldfix/udiskie
 Author: Byron Clark
 Author-email: byron@theclarkfamily.name
 Maintainer: Thomas Gläßle
 Maintainer-email: t_glaessle@gmx.de
 License: MIT
@@ -157,14 +157,25 @@
 
 .. _lang: https://github.com/coldfix/udiskie/tree/master/lang
 .. _udiskie.pot: https://raw.githubusercontent.com/coldfix/udiskie/master/lang/udiskie.pot
 
 CHANGELOG
 ---------
 
+2.5.3
+-----
+Date 24.04.2024
+
+- allow matching against a list of values in config rules (``device_config``)
+  [thanks @dajt1725]
+- fix ``--terminal`` command line option (was not doing anything) [@dajt1725]
+- fix AttributeError when *python-keyring-keyutils* is installed instead of
+  *keyutils* [thanks @bubbleguuum]
+
+
 2.5.2
 ~~~~~
 Date: 27.01.2024
 
 - drop external dependency on distutils (#278)
 - rename ``--notify-command`` to ``--event-hook`` to prevent misunderstandings (#279)
```

### Comparing `udiskie-2.5.2/README.rst` & `udiskie-2.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/completions/bash/udiskie` & `udiskie-2.5.3/completions/bash/udiskie`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/completions/bash/udiskie-info` & `udiskie-2.5.3/completions/bash/udiskie-info`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/completions/bash/udiskie-mount` & `udiskie-2.5.3/completions/bash/udiskie-mount`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/completions/bash/udiskie-umount` & `udiskie-2.5.3/completions/bash/udiskie-umount`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/completions/zsh/_udiskie` & `udiskie-2.5.3/completions/zsh/_udiskie`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/completions/zsh/_udiskie-canonical_paths` & `udiskie-2.5.3/completions/zsh/_udiskie-canonical_paths`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/completions/zsh/_udiskie-mount` & `udiskie-2.5.3/completions/zsh/_udiskie-mount`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/completions/zsh/_udiskie-umount` & `udiskie-2.5.3/completions/zsh/_udiskie-umount`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/doc/asciidoc.conf` & `udiskie-2.5.3/doc/asciidoc.conf`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/doc/udiskie.8.txt` & `udiskie-2.5.3/doc/udiskie.8.txt`

 * *Files 6% similar despite different names*

```diff
@@ -228,18 +228,22 @@
   # List of device option rules. Each item can match any combination of device
   # attributes. Additionally, it defines the resulting action (see below).
   # Any rule can contain multiple filters (AND) and multiple actions.
   # Only the first matching rule that defines a given action is used.
   # The rules defined here are simply prepended to the builtin device rules,
   # so that it is possible to completely overwrite the defaults by specifying
   # a catch-all rule (i.e. a rule without device attributes).
+  # Filter rules can be passed a list of values, in which case the rule is matched
+  # if the attribute matches any of the values in the list.
 
 - device_file: /dev/dm-5    # [filter]
   ignore:      false        # [action] never ignore this device
-- id_uuid: 9d53-13ba        # [filter] match by device UUID
+- id_uuid:                  # [filter] match by device UUID
+  - 9d53-13ba               # This rule matches on either of these uids
+  - 8675-309a
   options: [noexec, nodev]  # [action] mount options can be given as list
   ignore:  false            # [action] never ignore this device (even if fs=FAT)
   automount: false          # [action] do not automount this device
 - id_type: vfat             # [filter] match file system type
   ignore:  true             # [action] ignore all FAT devices
 
 - id_type: ntfs             # [filter] (optional)
```

### Comparing `udiskie-2.5.2/lang/de.po` & `udiskie-2.5.3/lang/de.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the udiskie package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: udiskie 2.4.2\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-01-27 00:26+0100\n"
+"POT-Creation-Date: 2024-04-16 21:10+0000\n"
 "PO-Revision-Date: 2022-04-18 00:28+0000\n"
 "Last-Translator: Thomas G. <t_glaessle@gmx.de>\n"
 "Language-Team: German <https://weblate.coldfix.de/projects/udiskie/udiskie/"
 "de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -47,15 +47,15 @@
 msgstr "%(message)s"
 
 #: ../udiskie/cli.py:141
 #, python-format
 msgid "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 msgstr "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 
-#: ../udiskie/cli.py:385
+#: ../udiskie/cli.py:386
 msgid ""
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
@@ -64,60 +64,60 @@
 "sein:\n"
 "\t- libnotify ist nicht installiert\n"
 "\t- die Typbibliothek wird durch ein separates Paket bereitgestellt\n"
 "\t- libnotify wurde ohne Introspektion kompiliert\n"
 "\n"
 "udiskie wird ohne Benachrichtigungen gestartet."
 
-#: ../udiskie/cli.py:399
+#: ../udiskie/cli.py:400
 msgid ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "Es wurde keine X oder Wayland Sitzung erkannt.\n"
 "udiskie wird daher ohne Trayicon gestartet.\n"
 
-#: ../udiskie/cli.py:406
+#: ../udiskie/cli.py:407
 msgid ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "Typbibliothek für 'Gtk 3.0' ist nicht verfügbar. Mögliche Gründen können "
 "sein:\n"
 "\t- GTK3 ist nicht installiert\n"
 "\t- die Typbibliothek wird durch ein separates Paket bereitgestellt\n"
 "\t- GTK3 wurde ohne Introspektion kompiliert\n"
 "udiskie wird ohne Trayicon gestartet.\n"
 
-#: ../udiskie/cli.py:416
+#: ../udiskie/cli.py:417
 msgid ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 msgstr ""
 "Typbibliothek für 'AppIndicator3 0.1' ist nicht verfügbar. Mögliche Gründe "
 "können sein:\n"
 "\t- libappindicator ist nicht installiert\n"
 "\t- die Typbibliothek wird durch ein separates Packet bereitgestellt\n"
 "\t- libappindicator wurde ohne Introspektion kompiliert\n"
 "udiskie wird ohne Benachrichtigungssymbol gestartet.\n"
 
-#: ../udiskie/cli.py:435
+#: ../udiskie/cli.py:436
 msgid ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 msgstr ""
 
-#: ../udiskie/cli.py:442
+#: ../udiskie/cli.py:443
 msgid "Ignoring 'notify_command' in favor of 'event_hook'."
 msgstr ""
 
 #: ../udiskie/config.py:129
 msgid "Unknown matching attribute: {!r}"
 msgstr "Unbekannte Vergleichseigenschaft: {!r}"
```

### Comparing `udiskie-2.5.2/lang/en_US.po` & `udiskie-2.5.3/lang/en_US.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # English translations for udiskie package.
 # Copyright (C) 2024 Thomas Gläßle
 # This file is distributed under the same license as the udiskie package.
 # Automatically generated, 2024.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: udiskie 2.5.1\n"
+"Project-Id-Version: udiskie 2.5.2\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-01-27 00:26+0100\n"
-"PO-Revision-Date: 2024-01-27 00:26+0100\n"
+"POT-Creation-Date: 2024-04-16 21:10+0000\n"
+"PO-Revision-Date: 2024-04-16 21:10+0000\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -44,15 +44,15 @@
 msgstr "%(message)s"
 
 #: ../udiskie/cli.py:141
 #, python-format
 msgid "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 msgstr "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 
-#: ../udiskie/cli.py:385
+#: ../udiskie/cli.py:386
 msgid ""
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
@@ -60,61 +60,61 @@
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
 
-#: ../udiskie/cli.py:399
+#: ../udiskie/cli.py:400
 msgid ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 
-#: ../udiskie/cli.py:406
+#: ../udiskie/cli.py:407
 msgid ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 
-#: ../udiskie/cli.py:416
+#: ../udiskie/cli.py:417
 msgid ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 msgstr ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 
-#: ../udiskie/cli.py:435
+#: ../udiskie/cli.py:436
 msgid ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 msgstr ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 
-#: ../udiskie/cli.py:442
+#: ../udiskie/cli.py:443
 msgid "Ignoring 'notify_command' in favor of 'event_hook'."
 msgstr "Ignoring 'notify_command' in favor of 'event_hook'."
 
 #: ../udiskie/config.py:129
 msgid "Unknown matching attribute: {!r}"
 msgstr "Unknown matching attribute: {!r}"
```

### Comparing `udiskie-2.5.2/lang/es_ES.po` & `udiskie-2.5.3/lang/es_ES.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the udiskie package.
 # Alejandro Pérez <alejandro.perez.mendez@gmail.com>, 2014.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: udiskie\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-01-27 00:26+0100\n"
+"POT-Creation-Date: 2024-04-16 21:10+0000\n"
 "PO-Revision-Date: 2014-07-23 18:43+0100\n"
 "Last-Translator: Alejandro Pérez <alejandro.perez.mendez@gmail.com>\n"
 "Language-Team: Spanish alejandro.perez.mendez@gmail.com\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -47,56 +47,56 @@
 msgstr "%(message)s"
 
 #: ../udiskie/cli.py:141
 #, python-format
 msgid "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 msgstr "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 
-#: ../udiskie/cli.py:385
+#: ../udiskie/cli.py:386
 msgid ""
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
 msgstr ""
 
-#: ../udiskie/cli.py:399
+#: ../udiskie/cli.py:400
 msgid ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:406
+#: ../udiskie/cli.py:407
 msgid ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:416
+#: ../udiskie/cli.py:417
 msgid ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:435
+#: ../udiskie/cli.py:436
 msgid ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 msgstr ""
 
-#: ../udiskie/cli.py:442
+#: ../udiskie/cli.py:443
 msgid "Ignoring 'notify_command' in favor of 'event_hook'."
 msgstr ""
 
 #: ../udiskie/config.py:129
 msgid "Unknown matching attribute: {!r}"
 msgstr "Atributo de filtrado desconocido: {!r}"
```

### Comparing `udiskie-2.5.2/lang/it_IT.po` & `udiskie-2.5.3/lang/it_IT.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the udiskie package.
 # Stefano Mecocci <mecocci15@gmail.com>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: udiskie\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-01-27 00:26+0100\n"
+"POT-Creation-Date: 2024-04-16 21:10+0000\n"
 "PO-Revision-Date: 2022-04-17 13:10+0000\n"
 "Last-Translator: Weblate Admin <weblate@coldfix.de>\n"
 "Language-Team: Italian <http://weblate.coldfix.de/projects/udiskie/udiskie/"
 "it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -49,15 +49,15 @@
 msgstr "%(message)s"
 
 #: ../udiskie/cli.py:141
 #, python-format
 msgid "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 msgstr "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 
-#: ../udiskie/cli.py:385
+#: ../udiskie/cli.py:386
 msgid ""
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
@@ -65,59 +65,59 @@
 "Typelib per 'libnotify' non è disponibile. Fra le possibili cause:\n"
 "\t- libnotify non è installato\n"
 "\t- typelib è fornito da un pacchetto separato\n"
 "\t- La build di libnotify è stata eseguita con introspezione disabilitata\n"
 "\n"
 "Avvio di udiskie con notifiche disattivate."
 
-#: ../udiskie/cli.py:399
+#: ../udiskie/cli.py:400
 #, fuzzy
 msgid ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "Non è stata rilevata una sessione X. \n"
 "Avvio di udiskie senza icona di sistema.\n"
 
-#: ../udiskie/cli.py:406
+#: ../udiskie/cli.py:407
 msgid ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "Typelib per 'Gtk 3.0' non è disponibile. Fra le possibili cause:\n"
 "\t- GTK3 non è installato\n"
 "\t- typelib è fornito da un pacchetto separato\n"
 "\t- La build di GTK3 è stata eseguita con introspezione disabilitata\n"
 "Avvio di udiskie senza icona di sistema.\n"
 
-#: ../udiskie/cli.py:416
+#: ../udiskie/cli.py:417
 msgid ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 msgstr ""
 "Typelib per 'AppIndicator3 0.1' non è disponibile. Fra le possibili cause:\n"
 "\t- libappindicator non è installato\n"
 "\t- typelib è fornita da un pacchetto separato\n"
 "\t- La build è stata eseguita con introspezione disabilitata\n"
 "Avvio di udiskie senza icona di sistema.\n"
 
-#: ../udiskie/cli.py:435
+#: ../udiskie/cli.py:436
 msgid ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 msgstr ""
 
-#: ../udiskie/cli.py:442
+#: ../udiskie/cli.py:443
 msgid "Ignoring 'notify_command' in favor of 'event_hook'."
 msgstr ""
 
 #: ../udiskie/config.py:129
 msgid "Unknown matching attribute: {!r}"
 msgstr ""
```

### Comparing `udiskie-2.5.2/lang/ru_RU.po` & `udiskie-2.5.3/lang/ru_RU.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the udiskie package.
 # mr-GreyWolf <mr.greywolf@list.ru>, 2019.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-01-27 00:26+0100\n"
+"POT-Creation-Date: 2024-04-16 21:10+0000\n"
 "PO-Revision-Date: 2022-04-17 13:10+0000\n"
 "Last-Translator: Weblate Admin <weblate@coldfix.de>\n"
 "Language-Team: Russian <http://weblate.coldfix.de/projects/udiskie/udiskie/"
 "ru/>\n"
 "Language: ru_RU\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -49,15 +49,15 @@
 msgstr "%(message)s"
 
 #: ../udiskie/cli.py:141
 #, python-format
 msgid "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 msgstr "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 
-#: ../udiskie/cli.py:385
+#: ../udiskie/cli.py:386
 msgid ""
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
@@ -65,60 +65,60 @@
 "Typelib для 'libnotify'  недоступна. Возможные причины:\n"
 "\t- libnotify не установлена\n"
 "\t- typelib поставляется в виде отдельного пакета\n"
 "\t- libnotify была собрана с отключенным самоанализом\n"
 "\n"
 "Запуск udiskie выполнен без уведомлений."
 
-#: ../udiskie/cli.py:399
+#: ../udiskie/cli.py:400
 #, fuzzy
 msgid ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "Не запущено в сессии X-Windows. \n"
 "Запустите udiskie без иконки в трее.\n"
 
-#: ../udiskie/cli.py:406
+#: ../udiskie/cli.py:407
 msgid ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "Typelib для GTK 3.0 недоступен. Возможные причины:\n"
 "\t- GTK3 не установлен\n"
 "\t- typelib поставляется в виде отдельного пакета\n"
 "\t- GTK3 был собран с отключенным самоанализом\n"
 "Запуск udiskie выполнен без иконки в трее.\n"
 
-#: ../udiskie/cli.py:416
+#: ../udiskie/cli.py:417
 #, fuzzy
 msgid ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 msgstr ""
 "Typelib для GTK 3.0 недоступен. Возможные причины:\n"
 "\t- GTK3 не установлен\n"
 "\t- typelib поставляется в виде отдельного пакета\n"
 "\t- GTK3 был собран с отключенным самоанализом\n"
 "Запуск udiskie выполнен без иконки в трее.\n"
 
-#: ../udiskie/cli.py:435
+#: ../udiskie/cli.py:436
 msgid ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 msgstr ""
 
-#: ../udiskie/cli.py:442
+#: ../udiskie/cli.py:443
 msgid "Ignoring 'notify_command' in favor of 'event_hook'."
 msgstr ""
 
 #: ../udiskie/config.py:129
 msgid "Unknown matching attribute: {!r}"
 msgstr "Неизвестный атрибут соответствия: {!r}"
```

### Comparing `udiskie-2.5.2/lang/sk_SK.po` & `udiskie-2.5.3/lang/sk_SK.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is distributed under the same license as the udiskie package.
 # oli <jose1711@gmail.com>, 2019.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-01-27 00:26+0100\n"
+"POT-Creation-Date: 2024-04-16 21:10+0000\n"
 "PO-Revision-Date: 2019-05-02 14:20+0200\n"
 "Last-Translator: Jose Riha <jose1711@gmail.com>\n"
 "Language-Team: Slovak\n"
 "Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -40,56 +40,56 @@
 msgstr "%(message)s"
 
 #: ../udiskie/cli.py:141
 #, python-format
 msgid "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 msgstr "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 
-#: ../udiskie/cli.py:385
+#: ../udiskie/cli.py:386
 msgid ""
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
 msgstr ""
 
-#: ../udiskie/cli.py:399
+#: ../udiskie/cli.py:400
 msgid ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:406
+#: ../udiskie/cli.py:407
 msgid ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:416
+#: ../udiskie/cli.py:417
 msgid ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:435
+#: ../udiskie/cli.py:436
 msgid ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 msgstr ""
 
-#: ../udiskie/cli.py:442
+#: ../udiskie/cli.py:443
 msgid "Ignoring 'notify_command' in favor of 'event_hook'."
 msgstr ""
 
 #: ../udiskie/config.py:129
 msgid "Unknown matching attribute: {!r}"
 msgstr "Neznámy atribút pre vyhľadávanie: {!r}"
```

### Comparing `udiskie-2.5.2/lang/tr_TR.po` & `udiskie-2.5.3/lang/tr_TR.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the udiskie package.
 # Oğuz Ersen <oguzersen@protonmail.com>, 2021-2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: udiskie\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-01-27 00:26+0100\n"
+"POT-Creation-Date: 2024-04-16 21:10+0000\n"
 "PO-Revision-Date: 2022-02-18 23:04+0300\n"
 "Last-Translator: Oğuz Ersen <oguzersen@protonmail.com>\n"
 "Language-Team: Turkish\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -46,15 +46,15 @@
 msgstr "%(message)s"
 
 #: ../udiskie/cli.py:141
 #, python-format
 msgid "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 msgstr "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 
-#: ../udiskie/cli.py:385
+#: ../udiskie/cli.py:386
 msgid ""
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
@@ -62,60 +62,60 @@
 "'libnotify' için typelib kullanılamıyor. Olası nedenler şunlardır:\n"
 "\t- libnotify kurulu değil\n"
 "\t- typelib ayrı bir paket tarafından sağlanıyor\n"
 "\t- libnotify, iç gözlem devre dışı bırakılarak oluşturuldu\n"
 "\n"
 "udiskie, bildirimler olmadan başlatılıyor."
 
-#: ../udiskie/cli.py:399
+#: ../udiskie/cli.py:400
 msgid ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "X veya Wayland oturumu içinde çalıştırılmadı.\n"
 "udiskie, tepsi simgesi olmadan başlatılıyor.\n"
 
-#: ../udiskie/cli.py:406
+#: ../udiskie/cli.py:407
 msgid ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 "'Gtk 3.0' için typelib kullanılamıyor. Olası nedenler şunlardır:\n"
 "\t- GTK3 kurulu değil\n"
 "\t- typelib ayrı bir paket tarafından sağlanıyor\n"
 "\t- GTK3, iç gözlem devre dışı bırakılarak oluşturuldu\n"
 "\n"
 "udiskie, tepsi simgesi olmadan başlatılıyor.\n"
 
-#: ../udiskie/cli.py:416
+#: ../udiskie/cli.py:417
 msgid ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 msgstr ""
 "'AppIndicator3 0.1' için typelib kullanılamıyor. Olası nedenler şunlardır:\n"
 "\t- libappindicator kurulu değil\n"
 "\t- typelib ayrı bir paket tarafından sağlanıyor\n"
 "\t- iç gözlem devre dışı bırakılarak oluşturuldu\n"
 "\n"
 "udiskie, appindicator simgesi olmadan başlatılıyor.\n"
 
-#: ../udiskie/cli.py:435
+#: ../udiskie/cli.py:436
 msgid ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 msgstr ""
 
-#: ../udiskie/cli.py:442
+#: ../udiskie/cli.py:443
 msgid "Ignoring 'notify_command' in favor of 'event_hook'."
 msgstr ""
 
 #: ../udiskie/config.py:129
 msgid "Unknown matching attribute: {!r}"
 msgstr "Bilinmeyen eşleşen özellik: {!r}"
```

### Comparing `udiskie-2.5.2/lang/udiskie.pot` & `udiskie-2.5.3/lang/udiskie.pot`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Copyright (C) 2024 Thomas Gläßle
 # This file is distributed under the same license as the udiskie package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: udiskie 2.5.1\n"
+"Project-Id-Version: udiskie 2.5.2\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-01-27 00:26+0100\n"
+"POT-Creation-Date: 2024-04-16 21:10+0000\n"
 "PO-Revision-Date: 2024-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -38,56 +38,56 @@
 msgstr ""
 
 #: ../udiskie/cli.py:141
 #, python-format
 msgid "%(levelname)s [%(asctime)s] %(name)s: %(message)s"
 msgstr ""
 
-#: ../udiskie/cli.py:385
+#: ../udiskie/cli.py:386
 msgid ""
 "Typelib for 'libnotify' is not available. Possible causes include:\n"
 "\t- libnotify is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- libnotify was built with introspection disabled\n"
 "\n"
 "Starting udiskie without notifications."
 msgstr ""
 
-#: ../udiskie/cli.py:399
+#: ../udiskie/cli.py:400
 msgid ""
 "Not run within X or Wayland session.\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:406
+#: ../udiskie/cli.py:407
 msgid ""
 "Typelib for 'Gtk 3.0' is not available. Possible causes include:\n"
 "\t- GTK3 is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- GTK3 was built with introspection disabled\n"
 "Starting udiskie without tray icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:416
+#: ../udiskie/cli.py:417
 msgid ""
 "Typelib for 'AppIndicator3 0.1' is not available. Possible causes include:\n"
 "\t- libappindicator is not installed\n"
 "\t- the typelib is provided by a separate package\n"
 "\t- it was built with introspection disabled\n"
 "Starting udiskie without appindicator icon.\n"
 msgstr ""
 
-#: ../udiskie/cli.py:435
+#: ../udiskie/cli.py:436
 msgid ""
 "The 'notify_command' option was renamed to 'event_hook'. The old name still "
 "works, but may be removed in a future version. Please change your command "
 "line and config to use the new name."
 msgstr ""
 
-#: ../udiskie/cli.py:442
+#: ../udiskie/cli.py:443
 msgid "Ignoring 'notify_command' in favor of 'event_hook'."
 msgstr ""
 
 #: ../udiskie/config.py:129
 msgid "Unknown matching attribute: {!r}"
 msgstr ""
```

### Comparing `udiskie-2.5.2/setup.cfg` & `udiskie-2.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/setup.py` & `udiskie-2.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/test/test_cache.py` & `udiskie-2.5.3/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/test/test_match.py` & `udiskie-2.5.3/test/test_match.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/appindicator.py` & `udiskie-2.5.3/udiskie/appindicator.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/async_.py` & `udiskie-2.5.3/udiskie/async_.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/automount.py` & `udiskie-2.5.3/udiskie/automount.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/cli.py` & `udiskie-2.5.3/udiskie/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,14 +341,15 @@
             '--no-tray': False,
             '--smart-tray': 'auto'}),
         'menu': Value('--menu'),
         'appindicator': Switch('appindicator'),
         'file_manager': OptionalValue('--file-manager'),
         'password_prompt': OptionalValue('--password-prompt'),
         'password_cache': OptionalValue('--password-cache'),
+        'terminal': OptionalValue('--terminal'),
         'notify_command': OptionalValue('--notify-command'),
         'event_hook': OptionalValue('--event-hook'),
         'menu_checkbox_workaround': OptionalValue('--menu-checkbox-workaround'),
         'menu_update_workaround': OptionalValue('--menu-update-workaround'),
     })
 
     def _init(self):
```

### Comparing `udiskie-2.5.2/udiskie/common.py` & `udiskie-2.5.3/udiskie/common.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/config.py` & `udiskie-2.5.3/udiskie/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     else:
         return '{}={}'.format(k, v)
 
 
 def match_value(value, pattern):
     if isinstance(value, (list, tuple)):
         return any(match_value(v, pattern) for v in value)
+    if isinstance(pattern, (list, tuple)):
+        return any(match_value(value, p) for p in pattern)
     if isinstance(value, str) and isinstance(pattern, str):
         return fnmatch.fnmatch(value.lower(), pattern.lower())
     return lower(value) == lower(pattern)
 
 
 class DeviceFilter:
```

### Comparing `udiskie-2.5.2/udiskie/dbus.py` & `udiskie-2.5.3/udiskie/dbus.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/depend.py` & `udiskie-2.5.3/udiskie/depend.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/__init__.py` & `udiskie-2.5.3/udiskie/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-checkbox-checked.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-checkbox-checked.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-checkbox-unchecked.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-checkbox-unchecked.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-detach.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-detach.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-eject.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-eject.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-lock.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-lock.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-mount.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-mount.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-submenu.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-submenu.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-unlock.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-unlock.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/icons/udiskie-unmount.svg` & `udiskie-2.5.3/udiskie/icons/udiskie-unmount.svg`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/locale.py` & `udiskie-2.5.3/udiskie/locale.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/mount.py` & `udiskie-2.5.3/udiskie/mount.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/notify.py` & `udiskie-2.5.3/udiskie/notify.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/password_dialog.ui` & `udiskie-2.5.3/udiskie/password_dialog.ui`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/prompt.py` & `udiskie-2.5.3/udiskie/prompt.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/tray.py` & `udiskie-2.5.3/udiskie/tray.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie/udisks2.py` & `udiskie-2.5.3/udiskie/udisks2.py`

 * *Files identical despite different names*

### Comparing `udiskie-2.5.2/udiskie.egg-info/PKG-INFO` & `udiskie-2.5.3/udiskie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udiskie
-Version: 2.5.2
+Version: 2.5.3
 Summary: Removable disk automounter for udisks
 Home-page: https://github.com/coldfix/udiskie
 Author: Byron Clark
 Author-email: byron@theclarkfamily.name
 Maintainer: Thomas Gläßle
 Maintainer-email: t_glaessle@gmx.de
 License: MIT
@@ -157,14 +157,25 @@
 
 .. _lang: https://github.com/coldfix/udiskie/tree/master/lang
 .. _udiskie.pot: https://raw.githubusercontent.com/coldfix/udiskie/master/lang/udiskie.pot
 
 CHANGELOG
 ---------
 
+2.5.3
+-----
+Date 24.04.2024
+
+- allow matching against a list of values in config rules (``device_config``)
+  [thanks @dajt1725]
+- fix ``--terminal`` command line option (was not doing anything) [@dajt1725]
+- fix AttributeError when *python-keyring-keyutils* is installed instead of
+  *keyutils* [thanks @bubbleguuum]
+
+
 2.5.2
 ~~~~~
 Date: 27.01.2024
 
 - drop external dependency on distutils (#278)
 - rename ``--notify-command`` to ``--event-hook`` to prevent misunderstandings (#279)
```

### Comparing `udiskie-2.5.2/udiskie.egg-info/SOURCES.txt` & `udiskie-2.5.3/udiskie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

