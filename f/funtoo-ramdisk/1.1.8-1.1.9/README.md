# Comparing `tmp/funtoo_ramdisk-1.1.8.tar.gz` & `tmp/funtoo_ramdisk-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funtoo_ramdisk-1.1.8.tar", last modified: Tue Apr 16 04:27:16 2024, max compression
+gzip compressed data, was "funtoo_ramdisk-1.1.9.tar", last modified: Tue Apr 16 20:01:37 2024, max compression
```

## Comparing `funtoo_ramdisk-1.1.8.tar` & `funtoo_ramdisk-1.1.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       77 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8769 2024-04-16 04:27:06.000000 funtoo_ramdisk-1.1.8/ChangeLog.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      111 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/MANIFEST.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16421 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2024-04-16 04:26:37.000000 funtoo_ramdisk-1.1.8/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1901 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/bin/ramdisk
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/doc/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7107 2024-04-16 04:27:12.000000 funtoo_ramdisk-1.1.8/doc/manpage.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7113 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/doc/manpage.rst.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7642 2024-04-16 04:27:12.000000 funtoo_ramdisk-1.1.8/doc/ramdisk.8
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6309 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/args.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2041 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/config_files.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/const.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12207 2024-04-16 04:26:14.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/initramfs.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1602 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/kernel.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1252 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/log.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    15949 2024-04-15 03:11:58.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/modules.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1167 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/plugin_base.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk/plugins/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/plugins/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      361 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/plugins/btrfs.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      359 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/plugins/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      782 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/plugins/lvm.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      319 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/initrd.defaults
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6059 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/initrd.scripts
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/plugins/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/plugins/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/plugins/scan_mode/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/plugins/scan_mode/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      645 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      117 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/plugins/scan_mode/udev.sh
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2048 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/initramfs.cpio
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2174 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/linuxrc
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/module_configs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/module_configs/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/module_configs/full/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/module_configs/full/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2091 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/module_configs/full/modules.autoload
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1349 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/module_configs/full/modules.copy
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1375 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/utilities.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2024-04-16 04:27:12.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk/version.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/funtoo_ramdisk.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16421 2024-04-16 04:27:16.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1374 2024-04-16 04:27:16.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2024-04-16 04:27:16.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        5 2024-04-16 04:27:16.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       15 2024-04-16 04:27:16.000000 funtoo_ramdisk-1.1.8/funtoo_ramdisk.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      721 2024-04-15 03:17:25.000000 funtoo_ramdisk-1.1.8/make.sh
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2024-04-16 04:27:16.168194 funtoo_ramdisk-1.1.8/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      944 2024-04-16 04:27:12.000000 funtoo_ramdisk-1.1.8/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      950 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.8/setup.py.in
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.844900 funtoo_ramdisk-1.1.9/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       77 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9246 2024-04-16 20:00:59.000000 funtoo_ramdisk-1.1.9/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      111 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/MANIFEST.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16996 2024-04-16 20:01:37.844900 funtoo_ramdisk-1.1.9/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4927 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2024-04-16 20:00:59.000000 funtoo_ramdisk-1.1.9/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.834896 funtoo_ramdisk-1.1.9/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1901 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/bin/ramdisk
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.834896 funtoo_ramdisk-1.1.9/doc/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7205 2024-04-16 20:01:33.000000 funtoo_ramdisk-1.1.9/doc/manpage.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7211 2024-04-16 20:00:59.000000 funtoo_ramdisk-1.1.9/doc/manpage.rst.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:33.000000 funtoo_ramdisk-1.1.9/doc/ramdisk.8
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.834896 funtoo_ramdisk-1.1.9/funtoo_ramdisk/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6309 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/args.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2041 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/config_files.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1946 2024-04-16 17:49:45.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/const.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    12640 2024-04-16 20:00:59.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/initramfs.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1602 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/kernel.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1252 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/log.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    15949 2024-04-15 03:11:58.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/modules.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1167 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/plugin_base.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.834896 funtoo_ramdisk-1.1.9/funtoo_ramdisk/plugins/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/plugins/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      361 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/plugins/btrfs.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      359 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/plugins/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      782 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/plugins/lvm.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.834896 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.834896 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      319 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/initrd.defaults
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6136 2024-04-16 20:00:59.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/initrd.scripts
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.834896 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/plugins/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/plugins/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.834896 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/plugins/scan_mode/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/plugins/scan_mode/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      645 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      117 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/plugins/scan_mode/udev.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2048 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/initramfs.cpio
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2174 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/linuxrc
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.844900 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/module_configs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/module_configs/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.844900 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/module_configs/full/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/module_configs/full/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2091 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/module_configs/full/modules.autoload
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1349 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/module_configs/full/modules.copy
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1375 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/utilities.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2024-04-16 20:01:33.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk/version.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2024-04-16 20:01:37.844900 funtoo_ramdisk-1.1.9/funtoo_ramdisk.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    16996 2024-04-16 20:01:37.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1374 2024-04-16 20:01:37.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2024-04-16 20:01:37.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        5 2024-04-16 20:01:37.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       15 2024-04-16 20:01:37.000000 funtoo_ramdisk-1.1.9/funtoo_ramdisk.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      724 2024-04-16 20:00:59.000000 funtoo_ramdisk-1.1.9/make.sh
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2024-04-16 20:01:37.844900 funtoo_ramdisk-1.1.9/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      944 2024-04-16 20:01:33.000000 funtoo_ramdisk-1.1.9/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      950 2024-04-15 03:09:33.000000 funtoo_ramdisk-1.1.9/setup.py.in
```

### Comparing `funtoo_ramdisk-1.1.8/ChangeLog.rst` & `funtoo_ramdisk-1.1.9/ChangeLog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+funtoo-ramdisk 1.1.9
+--------------------
+
+Released on April 16, 2024.
+
+This is a minor feature release.
+
+* Add a ``--keep`` option which will preserve the contents of the
+  temporary directory so that errors and tracebacks can be investigated. 
+  This can be enabled via ebuilds to allow exploration of any ramdisk-
+  related errors.
+
+* Improve handling of a permissions error when copying the ramdisk to
+  a final location (provide error message instead of full traceback.)
+
 funtoo-ramdisk 1.1.8
 --------------------
 
 Released on April 16, 2024.
 
 This is a minor bug release.
```

### Comparing `funtoo_ramdisk-1.1.8/PKG-INFO` & `funtoo_ramdisk-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-ramdisk
-Version: 1.1.8
+Version: 1.1.9
 Summary: Funtoo framework for creating initial ramdisks.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse
 Author: Daniel Robbins, Funtoo Solutions Inc.
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -21,15 +21,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.8
+:Version: 1.1.9
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -114,14 +114,15 @@
 OPTIONS
 =======
 
 --debug                 Enable debug output.
 --backtrace             Display full python backtrace/traceback instead of just a
                         short error summary.
 --force                 Overwrite target initramfs if it exists.
+--keep                  Keep the temporary directory after execution for investigation/debugging.
 --version               Show this program's version number and exit.
 --help                  Show this help message and exit.
 --fs_foot=<path>        This defaults to ``/``, and specifies the filesystem root to look at
                         for finding both kernel sources (in ``/usr/src``) and kernel modules
                         (in ``/lib/modules``). This option also applies to ``ramdisk list
                         kernels``.
 --kernel=<kernel>       Specify what kernel to build a ramdisk for. Use
@@ -168,14 +169,29 @@
 
 
 
 
 ChangeLog
 =========
 
+funtoo-ramdisk 1.1.9
+--------------------
+
+Released on April 16, 2024.
+
+This is a minor feature release.
+
+* Add a ``--keep`` option which will preserve the contents of the
+  temporary directory so that errors and tracebacks can be investigated. 
+  This can be enabled via ebuilds to allow exploration of any ramdisk-
+  related errors.
+
+* Improve handling of a permissions error when copying the ramdisk to
+  a final location (provide error message instead of full traceback.)
+
 funtoo-ramdisk 1.1.8
 --------------------
 
 Released on April 16, 2024.
 
 This is a minor bug release.
```

### Comparing `funtoo_ramdisk-1.1.8/README.rst` & `funtoo_ramdisk-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/bin/ramdisk` & `funtoo_ramdisk-1.1.9/bin/ramdisk`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/doc/manpage.rst` & `funtoo_ramdisk-1.1.9/doc/manpage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.8
+:Version: 1.1.9
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -100,14 +100,15 @@
 OPTIONS
 =======
 
 --debug                 Enable debug output.
 --backtrace             Display full python backtrace/traceback instead of just a
                         short error summary.
 --force                 Overwrite target initramfs if it exists.
+--keep                  Keep the temporary directory after execution for investigation/debugging.
 --version               Show this program's version number and exit.
 --help                  Show this help message and exit.
 --fs_foot=<path>        This defaults to ``/``, and specifies the filesystem root to look at
                         for finding both kernel sources (in ``/usr/src``) and kernel modules
                         (in ``/lib/modules``). This option also applies to ``ramdisk list
                         kernels``.
 --kernel=<kernel>       Specify what kernel to build a ramdisk for. Use
```

### Comparing `funtoo_ramdisk-1.1.8/doc/manpage.rst.in` & `funtoo_ramdisk-1.1.9/doc/manpage.rst.in`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 OPTIONS
 =======
 
 --debug                 Enable debug output.
 --backtrace             Display full python backtrace/traceback instead of just a
                         short error summary.
 --force                 Overwrite target initramfs if it exists.
+--keep                  Keep the temporary directory after execution for investigation/debugging.
 --version               Show this program's version number and exit.
 --help                  Show this help message and exit.
 --fs_foot=<path>        This defaults to ``/``, and specifies the filesystem root to look at
                         for finding both kernel sources (in ``/usr/src``) and kernel modules
                         (in ``/lib/modules``). This option also applies to ``ramdisk list
                         kernels``.
 --kernel=<kernel>       Specify what kernel to build a ramdisk for. Use
```

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/args.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/args.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/config_files.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/config_files.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/const.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 	}
 
 	global_options = {
 		"--debug": False,
 		"--backtrace": False,
 		"--force": False,
 		"--help": False,
-		"--version": False
+		"--version": False,
+		"--keep": False
 	}
 
 	global_settings = {
 		"--fs_root": "/",
 	}
 
 	action_settings = {
```

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/initramfs.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/initramfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 			"depmod",
 			"modinfo"
 		]:
 			os.symlink("busybox", os.path.join(self.initramfs_root, "bin", applet))
 
 	@property
 	def temp_initramfs(self):
-		return os.path.join(self.temp_root, "initramfs.cpio")
+		return os.path.join(self.temp_root.name, "initramfs.cpio")
 
 	def create_ramdisk_binary(self):
 		# We use a "starter" initramfs.cpio with some pre-existing device nodes, because the current user may
 		# not have permission to create literal device nodes on the local filesystem:
 		shutil.copy(os.path.join(self.support_root, "initramfs.cpio"), self.temp_initramfs)
 		status = os.system(f'( cd "{self.initramfs_root}" && find . -print | cpio --quiet -o --format=newc --append -F "{self.temp_initramfs}" )')
 		if status:
@@ -261,16 +261,17 @@
 			self.log.debug(f"Running from git repository [turquoise2]{os.path.dirname(self.args.git_path)}[default]")
 
 	def create_ramdisk(self):
 		self.find_kernel()
 		self.print_banner()
 		self.display_enabled_plugins()
 		self.init_module_scanner()
-		with tempfile.TemporaryDirectory(prefix="ramdisk-", dir=self.args.values.temp_root) as self.temp_root:
-			self.initramfs_root = os.path.join(self.temp_root, "initramfs")
+		self.temp_root = tempfile.TemporaryDirectory(prefix="ramdisk-", dir=self.args.values.temp_root)
+		try:
+			self.initramfs_root = os.path.join(self.temp_root.name, "initramfs")
 			os.makedirs(self.initramfs_root)
 			final_cpio = os.path.abspath(self.args.values.destination)
 			if os.path.exists(final_cpio) and not self.args.values.force:
 				raise FileExistsError("Specified destination initramfs already exists -- use --force to overwrite.")
 			fstab_sanity_check()
 			self.log.debug(f"Using {self.initramfs_root} to build initramfs")
 			self.log.info(f"Creating initramfs...")
@@ -283,20 +284,31 @@
 				return False
 			self.copy_modules()
 			# TODO: add firmware?
 			# TODO: this needs cleaning up:
 			self.create_ramdisk_binary()
 			out_cpio = self.compress_ramdisk()
 			os.makedirs(os.path.dirname(final_cpio), exist_ok=True)
-			shutil.copy(out_cpio, final_cpio)
+			try:
+				shutil.copy(out_cpio, final_cpio)
+			except PermissionError as pe:
+				self.log.error(f"Unable to write to {final_cpio}.")
+				return False
 			self.log.info(f"Orig. Size:  [turquoise2]{self.size_initial / 1000000:6.2f} MiB[default]")
 			self.log.info(f"Final Size:  [turquoise2]{self.size_final / 1000000:6.2f} MiB[default]")
 			self.log.info(f"Ratio:       [orange1]{(self.size_final / self.size_initial) * 100:.2f}% [turquoise2]({self.size_initial/self.size_final:.2f}x)[default]")
 			self.log.done(f"Created:     [orange1]{final_cpio}[default]")
 			return True
+		finally:
+			if not self.args.values.keep:
+				self.temp_root.cleanup()
+			else:
+				if getattr(self.temp_root, "_finalizer"):
+					self.temp_root._finalizer.detach()
+				self.log.info(f"Keeping ramdisk temporary directory [orange1]{self.temp_root.name}[default] due to [turquoise2]--keep[default] option")
 
 	def list_plugins(self):
 		for plugin in self.plugins:
 			print(plugin)
 
 	def list_kernels(self):
 		link = os.path.join(self.args.values.fs_root, "usr/src/linux")
```

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/kernel.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/kernel.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/log.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/log.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/modules.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/modules.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/plugin_base.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/plugin_base.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/plugins/lvm.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/plugins/lvm.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/initrd.scripts` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/initrd.scripts`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
   for plugin in $PLUGINS; do
     source_file="/etc/plugins/${plugin}.sh"
     if [ ! -e "${source_file}" ]; then
       bad_msg "Specified ramdisk.activate plugin $plugin does not exist at $source_file -- cannot execute!"
       sleep 10
     else
       good_msg "Executing plugin at ${source_file}"
+    # TODO: add debug logging for plugins so we get command output in dmesg.
     . ${source_file}
     [ $? -ne 0 ] && sleep 10
     fi
   done
 }
 
 backup() {
```

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/etc/plugins/scan_mode/legacy.sh`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/initramfs.cpio` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/initramfs.cpio`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/linuxrc` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/linuxrc`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/module_configs/full/modules.autoload` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/module_configs/full/modules.autoload`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/support/module_configs/full/modules.copy` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/support/module_configs/full/modules.copy`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk/utilities.py` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk/utilities.py`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk.egg-info/PKG-INFO` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-ramdisk
-Version: 1.1.8
+Version: 1.1.9
 Summary: Funtoo framework for creating initial ramdisks.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse
 Author: Daniel Robbins, Funtoo Solutions Inc.
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -21,15 +21,15 @@
 --------------------------------------------------
 
 :Author: Daniel Robbins <drobbins@funtoo.org>
 :Copyright: Copyright 2023 Daniel Robbins, Funtoo Solutions, Inc.
  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0.
-:Version: 1.1.8
+:Version: 1.1.9
 :Manual section: 8
 :Manual group: Funtoo Linux
 
 SYNOPSIS
 ========
 
   ``ramdisk`` [build] [*OPTION...*] ``initramfs_outfile``
@@ -114,14 +114,15 @@
 OPTIONS
 =======
 
 --debug                 Enable debug output.
 --backtrace             Display full python backtrace/traceback instead of just a
                         short error summary.
 --force                 Overwrite target initramfs if it exists.
+--keep                  Keep the temporary directory after execution for investigation/debugging.
 --version               Show this program's version number and exit.
 --help                  Show this help message and exit.
 --fs_foot=<path>        This defaults to ``/``, and specifies the filesystem root to look at
                         for finding both kernel sources (in ``/usr/src``) and kernel modules
                         (in ``/lib/modules``). This option also applies to ``ramdisk list
                         kernels``.
 --kernel=<kernel>       Specify what kernel to build a ramdisk for. Use
@@ -168,14 +169,29 @@
 
 
 
 
 ChangeLog
 =========
 
+funtoo-ramdisk 1.1.9
+--------------------
+
+Released on April 16, 2024.
+
+This is a minor feature release.
+
+* Add a ``--keep`` option which will preserve the contents of the
+  temporary directory so that errors and tracebacks can be investigated. 
+  This can be enabled via ebuilds to allow exploration of any ramdisk-
+  related errors.
+
+* Improve handling of a permissions error when copying the ramdisk to
+  a final location (provide error message instead of full traceback.)
+
 funtoo-ramdisk 1.1.8
 --------------------
 
 Released on April 16, 2024.
 
 This is a minor bug release.
```

### Comparing `funtoo_ramdisk-1.1.8/funtoo_ramdisk.egg-info/SOURCES.txt` & `funtoo_ramdisk-1.1.9/funtoo_ramdisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funtoo_ramdisk-1.1.8/make.sh` & `funtoo_ramdisk-1.1.9/make.sh`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	cat > funtoo_ramdisk/version.py << EOF
 __version__ = "$VERSION"
 EOF
 	for x in setup.py doc/manpage.rst; do
 		sed -e "s/##VERSION##/$VERSION/g" \
 		${x}.in > ${x}
 	done
-	rst2man doc/manpage.rst > doc/ramdisk.8
+	rst2man.py doc/manpage.rst > doc/ramdisk.8
 }
 
 commit() {
 	git commit -a -m "$PKGNAME $VERSION release."
 	git tag -f "$VERSION"
 	git push
 	git push --tags -f
```

### Comparing `funtoo_ramdisk-1.1.8/setup.py` & `funtoo_ramdisk-1.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open("ChangeLog.rst", "r") as fh:
 	long_description += fh.read()
 
 print(long_description)
 
 setuptools.setup(
 	name="funtoo-ramdisk",
-	version="1.1.8",
+	version="1.1.9",
 	author="Daniel Robbins, Funtoo Solutions Inc.",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for creating initial ramdisks.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-ramdisk/browse",
 	scripts=["bin/ramdisk"],
```

### Comparing `funtoo_ramdisk-1.1.8/setup.py.in` & `funtoo_ramdisk-1.1.9/setup.py.in`

 * *Files identical despite different names*

