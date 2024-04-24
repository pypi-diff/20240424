# Comparing `tmp/ctypes-windows-sdk-0.0.8.tar.gz` & `tmp/ctypes-windows-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ctypes-windows-sdk-0.0.8.tar", last modified: Tue Jun 16 08:14:42 2020, max compression
+gzip compressed data, was "dist/ctypes-windows-sdk-0.0.9.tar", last modified: Tue Mar 30 10:16:38 2021, max compression
```

## Comparing `ctypes-windows-sdk-0.0.8.tar` & `ctypes-windows-sdk-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      304 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/ctypes_windows_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/ctypes_windows_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1339 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/ctypes_windows_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/ctypes_windows_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       60 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/ctypes_windows_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/cwinsdk/
--rw-r--r--   0 runner    (1001) docker     (116)     1857 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/cwinsdk/km/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/km/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/cwinsdk/km/crt/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/km/crt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      362 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/km/crt/excpt.py
--rw-r--r--   0 runner    (1001) docker     (116)      439 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/km/dderror.py
--rw-r--r--   0 runner    (1001) docker     (116)     2920 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/km/wdm.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/
--rw-r--r--   0 runner    (1001) docker     (116)      123 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/WTypesbase.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      645 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/basetsd.py
--rw-r--r--   0 runner    (1001) docker     (116)     3508 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/devioctl.py
--rw-r--r--   0 runner    (1001) docker     (116)       99 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/ehstorioctl.py
--rw-r--r--   0 runner    (1001) docker     (116)      495 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/guiddef.py
--rw-r--r--   0 runner    (1001) docker     (116)     1720 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/minwindef.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/ntdddisk.py
--rw-r--r--   0 runner    (1001) docker     (116)     3946 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/ntddscsi.py
--rw-r--r--   0 runner    (1001) docker     (116)      525 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/ntddstor.py
--rw-r--r--   0 runner    (1001) docker     (116)      708 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/ntdef.py
--rw-r--r--   0 runner    (1001) docker     (116)     1438 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/secext.py
--rw-r--r--   0 runner    (1001) docker     (116)      136 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/windef.py
--rw-r--r--   0 runner    (1001) docker     (116)   112988 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/shared/winerror.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/
--rw-r--r--   0 runner    (1001) docker     (116)      117 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/AudioSessionTypes.py
--rw-r--r--   0 runner    (1001) docker     (116)    17194 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/KnownFolders.py
--rw-r--r--   0 runner    (1001) docker     (116)      430 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/ShlObj_core.py
--rw-r--r--   0 runner    (1001) docker     (116)      103 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/Unknwn.py
--rw-r--r--   0 runner    (1001) docker     (116)    16191 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/WinBase.py
--rw-r--r--   0 runner    (1001) docker     (116)    11497 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/WinUser.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      985 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/combaseapi.py
--rw-r--r--   0 runner    (1001) docker     (116)     4305 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/consoleapi.py
--rw-r--r--   0 runner    (1001) docker     (116)     8702 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/consoleapi2.py
--rw-r--r--   0 runner    (1001) docker     (116)     3687 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/fileapi.py
--rw-r--r--   0 runner    (1001) docker     (116)      590 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/handleapi.py
--rw-r--r--   0 runner    (1001) docker     (116)     2141 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/ioapiset.py
--rw-r--r--   0 runner    (1001) docker     (116)     2489 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/libloaderapi.py
--rw-r--r--   0 runner    (1001) docker     (116)     2284 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/minwinbase.py
--rw-r--r--   0 runner    (1001) docker     (116)     3902 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/processenv.py
--rw-r--r--   0 runner    (1001) docker     (116)      450 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/processthreadsapi.py
--rw-r--r--   0 runner    (1001) docker     (116)     3061 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/reason.py
--rw-r--r--   0 runner    (1001) docker     (116)    21110 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/securitybaseapi.py
--rw-r--r--   0 runner    (1001) docker     (116)      148 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/shtypes.py
--rw-r--r--   0 runner    (1001) docker     (116)     8936 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/sysinfoapi.py
--rw-r--r--   0 runner    (1001) docker     (116)     3635 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/wincontypes.py
--rw-r--r--   0 runner    (1001) docker     (116)     2534 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/wingdi.py
--rw-r--r--   0 runner    (1001) docker     (116)    43050 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/winioctl.py
--rw-r--r--   0 runner    (1001) docker     (116)   272467 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/um/winnt.py
--rw-r--r--   0 runner    (1001) docker     (116)      855 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/cwinsdk/windows.py
--rw-r--r--   0 runner    (1001) docker     (116)       67 2020-06-16 08:14:42.000000 ctypes-windows-sdk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      870 2020-06-16 08:14:40.000000 ctypes-windows-sdk-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/ctypes_windows_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/ctypes_windows_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/ctypes_windows_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/ctypes_windows_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/ctypes_windows_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/cwinsdk/
+-rw-r--r--   0 runner    (1001) docker     (121)     1883 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/cwinsdk/km/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/km/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/cwinsdk/km/crt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/km/crt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/km/crt/excpt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/km/dderror.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2921 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/km/wdm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/WTypesbase.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/basetsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3507 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/devioctl.py
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/ehstorioctl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/guiddef.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/minwindef.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/ntdddisk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3971 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/ntddscsi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/ntddstor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/ntdef.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1412 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/secext.py
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/windef.py
+-rw-r--r--   0 runner    (1001) docker     (121)   112988 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/shared/winerror.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/AudioSessionTypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17195 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/KnownFolders.py
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/ShlObj_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/Unknwn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16195 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/WinBase.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11497 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/WinUser.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      985 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/combaseapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4305 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/consoleapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8675 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/consoleapi2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3660 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/fileapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/handleapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/ioapiset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2462 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/libloaderapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/minwinbase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3874 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/processenv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/processthreadsapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3060 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/reason.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21110 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/securitybaseapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/shtypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9127 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/sysinfoapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3636 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/wincontypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/wingdi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43007 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/winioctl.py
+-rw-r--r--   0 runner    (1001) docker     (121)   272436 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/um/winnt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/cwinsdk/windows.py
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-03-30 10:16:38.000000 ctypes-windows-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2021-03-30 10:16:35.000000 ctypes-windows-sdk-0.0.9/setup.py
```

### Comparing `ctypes-windows-sdk-0.0.8/PKG-INFO` & `ctypes-windows-sdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctypes-windows-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Ctypes port of Windows SDK
 Home-page: https://github.com/Dobatymo/ctypes-windows-sdk
 Author: Dobatymo
 License: UNKNOWN
 Description: # ctypes-windows-sdk
         
         A totally incomplete and random port of the C Windows SDK for Python ctypes. No dependencies besides the Python standard library.
```

### Comparing `ctypes-windows-sdk-0.0.8/ctypes_windows_sdk.egg-info/PKG-INFO` & `ctypes-windows-sdk-0.0.9/ctypes_windows_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctypes-windows-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Ctypes port of Windows SDK
 Home-page: https://github.com/Dobatymo/ctypes-windows-sdk
 Author: Dobatymo
 License: UNKNOWN
 Description: # ctypes-windows-sdk
         
         A totally incomplete and random port of the C Windows SDK for Python ctypes. No dependencies besides the Python standard library.
```

### Comparing `ctypes-windows-sdk-0.0.8/ctypes_windows_sdk.egg-info/SOURCES.txt` & `ctypes-windows-sdk-0.0.9/ctypes_windows_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 ctypes_windows_sdk.egg-info/PKG-INFO
 ctypes_windows_sdk.egg-info/SOURCES.txt
 ctypes_windows_sdk.egg-info/dependency_links.txt
 ctypes_windows_sdk.egg-info/top_level.txt
 cwinsdk/__init__.py
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/__init__.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import platform
-from ctypes import c_int, LibraryLoader, WinDLL, WinError
+from ctypes import LibraryLoader, WinDLL, WinError, c_int
 from ctypes.wintypes import HANDLE
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-	from typing import Iterable, Iterator
 	from ctypes import Structure
+	from typing import Any, Callable, Iterable, Iterator, Tuple
 
 windll = LibraryLoader(WinDLL)
 
 INVALID_HANDLE_VALUE = HANDLE(-1).value # copied from cwinsdk.um.handleapi to prevent cyclic imports
 S_OK = 0 # copied from cwinsdk.shared.winerror
 
 class CEnum(c_int):
@@ -68,13 +68,13 @@
 def s_ok(result, func, arguments):
 	if result != S_OK:
 		raise WinError(result)  # no error code set in windows
 
 	return result
 
 def _not_available(funcname):
-	# type: (str) -> None
+	# type: (str) -> Callable
 
 	def inner(*args, **kwargs):
 		raise OSError("{}() is not available on {}".format(funcname, platform.platform()))
 
 	return inner
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/km/wdm.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/km/wdm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from .. import CEnum
 
+
 class SECURITY_IMPERSONATION_LEVEL(CEnum):
 	SecurityAnonymous = 0
 	SecurityIdentification = 1
 	SecurityImpersonation = 2
 	SecurityDelegation = 3
 
 def CTL_CODE(DeviceType, Function, Method, Access):
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/basetsd.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/basetsd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import POINTER
-from ctypes import c_int, c_uint, c_long, c_ulong, c_int64, c_uint64
+from ctypes import POINTER, c_int, c_int64, c_long, c_uint, c_uint64, c_ulong
 from platform import machine
 
 X64 = machine().endswith('64')
 
 if X64:
 	INT_PTR = c_int64
 	UINT_PTR = c_uint64
 	LONG_PTR = c_int64
 	ULONG_PTR = c_uint64
 	PULONG_PTR = POINTER(c_uint64)
 else:
 	INT_PTR = c_int
 	UINT_PTR = c_uint
-	LONG_PTR = c_long 
+	LONG_PTR = c_long
 	ULONG_PTR = c_ulong
 	PULONG_PTR = POINTER(c_ulong)
 
 SIZE_T = ULONG_PTR
 SSIZE_T = LONG_PTR
 
 DWORD_PTR = ULONG_PTR
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/devioctl.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/devioctl.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,8 +100,8 @@
 
 METHOD_DIRECT_TO_HARDWARE = METHOD_IN_DIRECT
 METHOD_DIRECT_FROM_HARDWARE = METHOD_OUT_DIRECT
 
 FILE_ANY_ACCESS = 0
 FILE_SPECIAL_ACCESS = FILE_ANY_ACCESS
 FILE_READ_ACCESS = 0x0001
-FILE_WRITE_ACCESS = 0x0002 
+FILE_WRITE_ACCESS = 0x0002
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/minwindef.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/minwindef.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import Structure, POINTER
-from ctypes import c_ulong, c_int, c_ubyte, c_ushort, c_float, c_uint, c_long, c_void_p
+from ctypes import POINTER, Structure, c_float, c_int, c_long, c_ubyte, c_uint, c_ulong, c_ushort, c_void_p
 from ctypes.wintypes import HANDLE
 
-from .basetsd import UINT_PTR, LONG_PTR
+from .basetsd import LONG_PTR, UINT_PTR
 
 CPOINTER = POINTER
 
 ULONG = c_ulong
 PULONG = POINTER(ULONG)
 USHORT = c_ushort
 PUSHORT = POINTER(USHORT)
 UCHAR = c_ubyte
 PUCHAR = POINTER(UCHAR)
 
 MAX_PATH = 260
 
 DWORD = c_ulong
-BOOL = c_int 
+BOOL = c_int
 BYTE = c_ubyte
-WORD = c_ushort 
-FLOAT = c_float 
+WORD = c_ushort
+FLOAT = c_float
 PFLOAT = POINTER(FLOAT)
 PBOOL = POINTER(BOOL)
 LPBOOL = POINTER(BOOL)
 PBYTE = POINTER(BYTE)
 LPBYTE = POINTER(BYTE)
 PINT = POINTER(c_int)
 LPINT = POINTER(c_int)
@@ -38,17 +37,17 @@
 LPVOID = c_void_p
 LPCVOID = CPOINTER(c_long)
 
 INT = c_int
 UINT = c_uint
 PUINT = POINTER(UINT)
 
-WPARAM = UINT_PTR 
-LPARAM = LONG_PTR 
-LRESULT = LONG_PTR 
+WPARAM = UINT_PTR
+LPARAM = LONG_PTR
+LRESULT = LONG_PTR
 
 SPHANDLE = POINTER(HANDLE)
 LPHANDLE = POINTER(HANDLE)
 HGLOBAL = HANDLE
 HLOCAL = HANDLE
 GLOBALHANDLE = HANDLE
 LOCALHANDLE = HANDLE
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/ntdddisk.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/ntdddisk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import Structure
 from ctypes.wintypes import ULONG
 
+from .devioctl import CTL_CODE, FILE_DEVICE_DISK, FILE_READ_ACCESS, FILE_WRITE_ACCESS, METHOD_BUFFERED
 from .ntdef import UCHAR
-from .devioctl import CTL_CODE, FILE_DEVICE_DISK, METHOD_BUFFERED, FILE_READ_ACCESS, FILE_WRITE_ACCESS
 
 IOCTL_DISK_BASE = FILE_DEVICE_DISK
 SMART_GET_VERSION = CTL_CODE(IOCTL_DISK_BASE, 0x0020, METHOD_BUFFERED, FILE_READ_ACCESS)
 SMART_SEND_DRIVE_COMMAND = CTL_CODE(IOCTL_DISK_BASE, 0x0021, METHOD_BUFFERED, FILE_READ_ACCESS | FILE_WRITE_ACCESS)
 SMART_RCV_DRIVE_DATA = CTL_CODE(IOCTL_DISK_BASE, 0x0022, METHOD_BUFFERED, FILE_READ_ACCESS | FILE_WRITE_ACCESS)
 
 CAP_ATA_ID_CMD = 1
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/ntddscsi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/ntddscsi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import Structure
 from ctypes.wintypes import ULONG, USHORT
 
 from .basetsd import ULONG_PTR
-from .ntdef import UCHAR, PVOID
-from .devioctl import CTL_CODE, FILE_DEVICE_CONTROLLER, METHOD_BUFFERED, FILE_READ_ACCESS, FILE_WRITE_ACCESS, FILE_ANY_ACCESS
+from .devioctl import (CTL_CODE, FILE_ANY_ACCESS, FILE_DEVICE_CONTROLLER, FILE_READ_ACCESS, FILE_WRITE_ACCESS,
+                       METHOD_BUFFERED)
+from .ntdef import PVOID, UCHAR
 
 IOCTL_SCSI_BASE = FILE_DEVICE_CONTROLLER
 FILE_DEVICE_SCSI = 0x0000001b
 
 DD_SCSI_DEVICE_NAME = br"\Device\ScsiPort"
 
 IOCTL_SCSI_PASS_THROUGH = CTL_CODE(IOCTL_SCSI_BASE, 0x0401, METHOD_BUFFERED, FILE_READ_ACCESS | FILE_WRITE_ACCESS)
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/ntddstor.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/ntddstor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from .. import CEnum
 
+
 class STORAGE_BUS_TYPE(CEnum):
 	BusTypeUnknown = 0x00
 	BusTypeScsi = 0x1
 	BusTypeAtapi = 0x2
 	BusTypeAta = 0x3
 	BusType1394 = 0x4
 	BusTypeSsa = 0x5
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/ntdef.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/ntdef.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import POINTER
-from ctypes import c_void_p, c_char, c_short, c_long, c_double, c_ubyte, c_ushort, c_ulong, c_int64, c_uint64
+from ctypes import POINTER, c_char, c_double, c_int64, c_long, c_short, c_ubyte, c_uint64, c_ulong, c_ushort, c_void_p
 from ctypes.wintypes import WCHAR
 
 PWCHAR = POINTER(WCHAR)
 LPWCH = POINTER(WCHAR)
 PWCH = POINTER(WCHAR)
 
 LPCWCH = POINTER(WCHAR) # const
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/secext.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/secext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from ctypes.wintypes import BOOLEAN
-from ctypes.wintypes import LPSTR, LPWSTR, LPCSTR, LPCWSTR
+from ctypes.wintypes import BOOLEAN, LPCSTR, LPCWSTR, LPSTR, LPWSTR
 
 from .. import CEnum, windll
 from .minwindef import PULONG
 
+
 class EXTENDED_NAME_FORMAT(CEnum):
 	NameUnknown = 0
 	NameFullyQualifiedDN = 1
 	NameSamCompatible = 2
 	NameDisplay = 3
 	NameUniqueId = 6
 	NameCanonical = 7
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/shared/winerror.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/shared/winerror.py`

 * *Files identical despite different names*

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/KnownFolders.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/KnownFolders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ctypes import c_ubyte
 
 from ..shared.guiddef import GUID
 
+
 def DEFINE_KNOWN_FOLDER(l, w1, w2, b1, b2, b3, b4, b5, b6, b7, b8):
 	return GUID(l, w1, w2, (c_ubyte*8)(b1, b2, b3, b4, b5, b6, b7, b8))
 
 FOLDERID_NetworkFolder = DEFINE_KNOWN_FOLDER(0xD20BEEC4, 0x5CA8, 0x4905, 0xAE, 0x3B, 0xBF, 0x25, 0x1E, 0xA0, 0x9B, 0x53)
 FOLDERID_ComputerFolder = DEFINE_KNOWN_FOLDER(0x0AC0837C, 0xBBF8, 0x452A, 0x85, 0x0D, 0x79, 0xD0, 0x8E, 0x66, 0x7C, 0xA7)
 FOLDERID_InternetFolder = DEFINE_KNOWN_FOLDER(0x4D9F7874, 0x4E0C, 0x4904, 0x96, 0x7B, 0x40, 0xB0, 0xD2, 0x0C, 0x3E, 0x4B)
 FOLDERID_ControlPanelFolder = DEFINE_KNOWN_FOLDER(0x82A74AEB, 0xAEB4, 0x465C, 0xA0, 0x14, 0xD0, 0x97, 0xEE, 0x34, 0x6D, 0x63)
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/WinBase.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/WinBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import POINTER, Structure, Union, c_char
-from ctypes.wintypes import BOOL, LPVOID, WORD, DWORD, WCHAR, BYTE, ULONG # CHAR not in py2
-from ctypes.wintypes import LPSTR, LPWSTR, LPCSTR, LPCWSTR
+from ctypes.wintypes import (BOOL, BYTE, DWORD, LPCSTR, LPCWSTR, LPSTR, LPVOID, LPWSTR, ULONG, WCHAR,  # CHAR not in py2
+                             WORD)
 
 from .. import CEnum, windll
-from .minwinbase import *
-from .fileapi import *
-from .handleapi import *
-
-from .winnt import *
+from ..km.wdm import SECURITY_IMPERSONATION_LEVEL
 from ..shared.basetsd import SIZE_T, ULONG64
 from ..shared.minwindef import ATOM
 from ..shared.ntdef import CHAR
-from ..km.wdm import SECURITY_IMPERSONATION_LEVEL
+from .fileapi import *
+from .handleapi import *
+from .minwinbase import *
+from .winnt import *
 
 FILE_BEGIN = 0
 FILE_CURRENT = 1
 FILE_END = 2
 
 WAIT_FAILED = 0xFFFFFFFF
 WAIT_OBJECT_0 = STATUS_WAIT_0 + 0
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/WinUser.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/WinUser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import c_int
-from ctypes.wintypes import BOOL, UINT, DWORD
+from ctypes.wintypes import BOOL, DWORD, UINT
 
 from .. import windll
 
 # constants
 
 SB_HORZ = 0
 SB_VERT = 1
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/combaseapi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/combaseapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from ctypes.wintypes import LPVOID, DWORD
+from ctypes.wintypes import DWORD, LPVOID
 
 from .. import windll
-from .Unknwn import LPUNKNOWN
 from ..shared.basetsd import SIZE_T
-from ..shared.guiddef import REFCLSID, REFIID, LPIID
+from ..shared.guiddef import LPIID, REFCLSID, REFIID
 from ..shared.ntdef import HRESULT
 from ..shared.WTypesbase import LPCOLESTR
+from .Unknwn import LPUNKNOWN
 
 CoCreateInstance = windll.ole32.CoCreateInstance
 CoCreateInstance.argtypes = [REFCLSID, LPUNKNOWN, DWORD, REFIID, LPVOID]
 CoCreateInstance.restype = HRESULT
 
 CoInitializeEx = windll.ole32.CoInitializeEx
 CoInitializeEx.argtypes = [LPVOID, DWORD]
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/consoleapi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/consoleapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import Structure, POINTER, CFUNCTYPE
-from ctypes.wintypes import BOOL, DWORD, ULONG, UINT, HANDLE, LPVOID
+from ctypes import CFUNCTYPE, POINTER, Structure
+from ctypes.wintypes import BOOL, DWORD, HANDLE, LPVOID, UINT, ULONG
 
-from .. import windll, nonzero
+from .. import nonzero, windll
 from ..shared.minwindef import LPDWORD
 from ..shared.ntdef import HRESULT
-from .wincontypes import COORD, PINPUT_RECORD, HPCON
+from .wincontypes import COORD, HPCON, PINPUT_RECORD
 
 # defines
 
 ATTACH_PARENT_PROCESS = DWORD(-1)
 
 ENABLE_PROCESSED_INPUT = 0x0001
 ENABLE_LINE_INPUT = 0x0002
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/consoleapi2.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/consoleapi2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import Structure, POINTER
-from ctypes.wintypes import BOOL, WORD, ULONG, DWORD, WCHAR, HANDLE, LPVOID
-from ctypes.wintypes import LPSTR, LPWSTR, LPCSTR, LPCWSTR
+from ctypes import POINTER, Structure
+from ctypes.wintypes import BOOL, DWORD, HANDLE, LPCSTR, LPCWSTR, LPSTR, LPVOID, LPWSTR, ULONG, WCHAR, WORD
 
 from .. import windll
-from .wincontypes import COORD, SMALL_RECT, INPUT_RECORD, CHAR_INFO
-from .minwinbase import SECURITY_ATTRIBUTES
-from ..shared.windef import COLORREF
-from ..shared.minwindef import UINT, LPDWORD
+from ..shared.minwindef import LPDWORD, UINT
 from ..shared.ntdef import CHAR
+from ..shared.windef import COLORREF
+from .minwinbase import SECURITY_ATTRIBUTES
+from .wincontypes import CHAR_INFO, COORD, INPUT_RECORD, SMALL_RECT
 
 FOREGROUND_BLUE = 0x0001
 FOREGROUND_GREEN = 0x0002
 FOREGROUND_RED = 0x0004
 FOREGROUND_INTENSITY = 0x0008
 BACKGROUND_BLUE = 0x0010
 BACKGROUND_GREEN = 0x0020
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/fileapi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/fileapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import Structure, POINTER
-from ctypes.wintypes import BOOL, DWORD, LONG, HANDLE, ULARGE_INTEGER
-from ctypes.wintypes import LPSTR, LPWSTR, LPCSTR, LPCWSTR
+from ctypes import POINTER, Structure
+from ctypes.wintypes import BOOL, DWORD, HANDLE, LONG, LPCSTR, LPCWSTR, LPSTR, LPWSTR, ULARGE_INTEGER
 
-from .. import windll, nonzero
-from .minwinbase import LPSECURITY_ATTRIBUTES, LPOVERLAPPED
-from ..shared.ntdef import ULONGLONG
+from .. import nonzero, windll
 from ..shared.minwindef import FILETIME
+from ..shared.ntdef import ULONGLONG
+from .minwinbase import LPOVERLAPPED, LPSECURITY_ATTRIBUTES
 
 CREATE_NEW = 1
 CREATE_ALWAYS = 2
 OPEN_EXISTING = 3
 OPEN_ALWAYS = 4
 TRUNCATE_EXISTING = 5
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/handleapi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/handleapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes.wintypes import HANDLE, BOOL, DWORD
+from ctypes.wintypes import BOOL, DWORD, HANDLE
 
-from .. import windll, nonzero
+from .. import nonzero, windll
 from ..shared.minwindef import LPHANDLE
 
 INVALID_HANDLE_VALUE = HANDLE(-1).value
 
 # functions
 
 CloseHandle = windll.kernel32.CloseHandle
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/ioapiset.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/ioapiset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import POINTER
-from ctypes.wintypes import LPVOID, BOOL, HANDLE, DWORD, ULONG
+from ctypes.wintypes import BOOL, DWORD, HANDLE, LPVOID, ULONG
 
-from .. import windll, _not_available
-from ..shared.basetsd import ULONG_PTR, PULONG_PTR
-from ..shared.minwindef import PULONG, LPDWORD
+from .. import _not_available, windll
+from ..shared.basetsd import PULONG_PTR, ULONG_PTR
+from ..shared.minwindef import LPDWORD, PULONG
 from .minwinbase import LPOVERLAPPED, LPOVERLAPPED_ENTRY
 
 CreateIoCompletionPort = windll.kernel32.CreateIoCompletionPort
 CreateIoCompletionPort.argtypes = [HANDLE, HANDLE, ULONG_PTR, DWORD]
-CreateIoCompletionPort.restype = HANDLE 
- 
+CreateIoCompletionPort.restype = HANDLE
+
 GetQueuedCompletionStatus = windll.kernel32.GetQueuedCompletionStatus
 GetQueuedCompletionStatus.argtypes = [HANDLE, LPDWORD, PULONG_PTR, POINTER(LPOVERLAPPED), DWORD]
-GetQueuedCompletionStatus.restype = BOOL 
+GetQueuedCompletionStatus.restype = BOOL
 
 GetQueuedCompletionStatusEx = windll.kernel32.GetQueuedCompletionStatusEx
 GetQueuedCompletionStatusEx.argtypes = [HANDLE, LPOVERLAPPED_ENTRY, ULONG, PULONG, DWORD, BOOL]
-GetQueuedCompletionStatusEx.restype = BOOL 
- 
+GetQueuedCompletionStatusEx.restype = BOOL
+
 PostQueuedCompletionStatus = windll.kernel32.PostQueuedCompletionStatus
 PostQueuedCompletionStatus.argtypes = [HANDLE, DWORD, ULONG_PTR, LPOVERLAPPED]
-PostQueuedCompletionStatus.restype = BOOL 
- 
+PostQueuedCompletionStatus.restype = BOOL
+
 DeviceIoControl = windll.kernel32.DeviceIoControl
 DeviceIoControl.argtypes = [HANDLE, DWORD, LPVOID, DWORD, LPVOID, DWORD, LPDWORD, LPOVERLAPPED]
-DeviceIoControl.restype = BOOL 
+DeviceIoControl.restype = BOOL
 
 GetOverlappedResult = windll.kernel32.GetOverlappedResult
 GetOverlappedResult.argtypes = [HANDLE, LPOVERLAPPED, LPDWORD, BOOL]
-GetOverlappedResult.restype = BOOL 
+GetOverlappedResult.restype = BOOL
 
 CancelIoEx = windll.kernel32.CancelIoEx
 CancelIoEx.argtypes = [HANDLE, LPOVERLAPPED]
-CancelIoEx.restype = BOOL 
+CancelIoEx.restype = BOOL
 
 CancelIo = windll.kernel32.CancelIo
 CancelIo.argtypes = [HANDLE]
-CancelIo.restype = BOOL 
+CancelIo.restype = BOOL
 
 try: # only windows 8+
 	GetOverlappedResultEx = windll.kernel32.GetOverlappedResultEx
 	GetOverlappedResultEx.argtypes = [HANDLE, LPOVERLAPPED, LPDWORD, DWORD, BOOL]
-	GetOverlappedResultEx.restype = BOOL 
+	GetOverlappedResultEx.restype = BOOL
 except AttributeError:
 	GetOverlappedResultEx = _not_available("GetOverlappedResultEx")
 
 CancelSynchronousIo = windll.kernel32.CancelSynchronousIo
 CancelSynchronousIo.argtypes = [HANDLE]
-CancelSynchronousIo.restype = BOOL 
+CancelSynchronousIo.restype = BOOL
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/libloaderapi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/libloaderapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import CFUNCTYPE
-from ctypes.wintypes import BOOL, WORD, DWORD, LPVOID
-from ctypes.wintypes import LPSTR, LPWSTR, LPCSTR, LPCWSTR
+from ctypes.wintypes import BOOL, DWORD, LPCSTR, LPCWSTR, LPSTR, LPVOID, LPWSTR, WORD
 
 from .. import windll
-from ..shared.minwindef import HMODULE, HRSRC, HGLOBAL
 from ..shared.basetsd import LONG_PTR
+from ..shared.minwindef import HGLOBAL, HMODULE, HRSRC
 from .winnt import LANGID
 
 FARPROC = LPVOID # todo: where does this come from?
 
 ENUMRESTYPEPROCW = CFUNCTYPE(BOOL, HMODULE, LPWSTR, LONG_PTR)
 ENUMRESTYPEPROCA = CFUNCTYPE(BOOL, HMODULE, LPSTR, LONG_PTR)
 ENUMRESNAMEPROCW = CFUNCTYPE(BOOL, HMODULE, LPCWSTR, LPWSTR, LONG_PTR)
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/minwinbase.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/minwinbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import Structure, POINTER, Union
-from ctypes.wintypes import DWORD, LPVOID, BOOL, HANDLE, WORD
+from ctypes import POINTER, Structure, Union
+from ctypes.wintypes import BOOL, DWORD, HANDLE, LPVOID, WORD
 
 from .. import CEnum, windll
-from ..shared.ntdef import PVOID
 from ..shared.basetsd import ULONG_PTR
+from ..shared.ntdef import PVOID
+
 
 class SECURITY_ATTRIBUTES(Structure):
 	_fields_ = [
 		("nLength", DWORD),
 		("lpSecurityDescriptor", LPVOID),
 		("bInheritHandle", BOOL),
 	]
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/processenv.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/processenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import POINTER
-from ctypes.wintypes import BOOL, HANDLE, DWORD
-from ctypes.wintypes import LPSTR, LPCSTR, LPWSTR, LPCWSTR
+from ctypes.wintypes import BOOL, DWORD, HANDLE, LPCSTR, LPCWSTR, LPSTR, LPWSTR
 
-from .. import windll, validhandle, nonzero
-from .winnt import LPWCH, LPCH, PHANDLE
+from .. import nonzero, validhandle, windll
+from .winnt import LPCH, LPWCH, PHANDLE
 
 SetEnvironmentStringsW = windll.kernel32.SetEnvironmentStringsW
 SetEnvironmentStringsW.argtypes = [LPWCH]
 SetEnvironmentStringsW.restype = BOOL
- 
+
 GetStdHandle = windll.kernel32.GetStdHandle
 GetStdHandle.argtypes = [DWORD]
 GetStdHandle.restype = HANDLE
 GetStdHandle.errcheck = validhandle
 
 SetStdHandle = windll.kernel32.SetStdHandle
 SetStdHandle.argtypes = [DWORD, HANDLE]
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/reason.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/reason.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 SHTDN_REASON_MINOR_OTHERDRIVER = 0x0000000e
 SHTDN_REASON_MINOR_BLUESCREEN = 0x0000000F
 SHTDN_REASON_MINOR_SERVICEPACK = 0x00000010
 SHTDN_REASON_MINOR_HOTFIX = 0x00000011
 SHTDN_REASON_MINOR_SECURITYFIX = 0x00000012
 SHTDN_REASON_MINOR_SECURITY = 0x00000013
 SHTDN_REASON_MINOR_NETWORK_CONNECTIVITY = 0x00000014
-SHTDN_REASON_MINOR_WMI = 0x00000015 
+SHTDN_REASON_MINOR_WMI = 0x00000015
 SHTDN_REASON_MINOR_SERVICEPACK_UNINSTALL = 0x00000016
 SHTDN_REASON_MINOR_HOTFIX_UNINSTALL = 0x00000017
 SHTDN_REASON_MINOR_SECURITYFIX_UNINSTALL = 0x00000018
 SHTDN_REASON_MINOR_MMC = 0x00000019
 SHTDN_REASON_MINOR_SYSTEMRESTORE = 0x0000001a
 SHTDN_REASON_MINOR_TERMSRV = 0x00000020
 SHTDN_REASON_MINOR_DC_PROMOTION = 0x00000021
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/securitybaseapi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/securitybaseapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import POINTER
-from ctypes.wintypes import HANDLE, DWORD, BOOL, LPCWSTR, LPVOID, LPWSTR
+from ctypes.wintypes import BOOL, DWORD, HANDLE, LPCWSTR, LPVOID, LPWSTR
 
 from .. import windll
-from ..shared.minwindef import PDWORD, LPDWORD, LPBOOL
-from .winnt import PTOKEN_PRIVILEGES, PSECURITY_DESCRIPTOR, PGENERIC_MAPPING, PPRIVILEGE_SET, PSID, POBJECT_TYPE_LIST
+from ..shared.minwindef import LPBOOL, LPDWORD, PDWORD
+from .winnt import PGENERIC_MAPPING, POBJECT_TYPE_LIST, PPRIVILEGE_SET, PSECURITY_DESCRIPTOR, PSID, PTOKEN_PRIVILEGES
 
 AccessCheck = windll.advapi32.AccessCheck
 AccessCheck.argtypes = [PSECURITY_DESCRIPTOR, HANDLE, DWORD, PGENERIC_MAPPING, PPRIVILEGE_SET, LPDWORD, LPDWORD, LPBOOL]
 AccessCheck.restype = BOOL
 
 AccessCheckAndAuditAlarmW = windll.advapi32.AccessCheckAndAuditAlarmW
 AccessCheckAndAuditAlarmW.argtypes = [LPCWSTR, LPVOID, LPWSTR, LPWSTR, PSECURITY_DESCRIPTOR, DWORD, PGENERIC_MAPPING, BOOL, LPDWORD, LPBOOL, LPBOOL]
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/sysinfoapi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/sysinfoapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import POINTER, Structure, Union, c_double
-from ctypes.wintypes import WORD, BOOL, UINT, DWORD, LPVOID, LPSTR, LPWSTR, LPCWSTR, ULONG, HANDLE, USHORT, LPCSTR
+from ctypes.wintypes import BOOL, DWORD, HANDLE, LPCSTR, LPCWSTR, LPSTR, LPVOID, LPWSTR, UINT, ULONG, USHORT, WORD
 
 from .. import CEnum, windll
-from .winnt import DWORDLONG, LPOSVERSIONINFOA, LPOSVERSIONINFOW, PSYSTEM_LOGICAL_PROCESSOR_INFORMATION, LOGICAL_PROCESSOR_RELATIONSHIP, PSYSTEM_LOGICAL_PROCESSOR_INFORMATION_EX, PULONGLONG, PSYSTEM_PROCESSOR_CYCLE_TIME_INFORMATION
-from .minwinbase import SYSTEMTIME, LPSYSTEMTIME, LPFILETIME
 from ..shared.basetsd import DWORD_PTR
-from ..shared.ntdef import ULONGLONG, PVOID
-from ..shared.minwindef import PDWORD, PBOOL, LPDWORD, UCHAR
+from ..shared.minwindef import LPDWORD, PBOOL, PDWORD, UCHAR
+from ..shared.ntdef import PVOID, ULONGLONG
+from .minwinbase import LPFILETIME, LPSYSTEMTIME, SYSTEMTIME
+from .winnt import (DWORDLONG, LOGICAL_PROCESSOR_RELATIONSHIP, LPOSVERSIONINFOA, LPOSVERSIONINFOW,
+                    PSYSTEM_LOGICAL_PROCESSOR_INFORMATION, PSYSTEM_LOGICAL_PROCESSOR_INFORMATION_EX,
+                    PSYSTEM_PROCESSOR_CYCLE_TIME_INFORMATION, PULONGLONG)
+
 
 class SYSTEM_INFO_DUMMYSTRUCTNAME(Structure):
 	_fields_ = [
 		("wProcessorArchitecture", WORD),
 		("wReserved", WORD),
 	]
 
@@ -166,17 +169,20 @@
 GetLogicalProcessorInformationEx.argtypes = [LOGICAL_PROCESSOR_RELATIONSHIP, PSYSTEM_LOGICAL_PROCESSOR_INFORMATION_EX, PDWORD]
 GetLogicalProcessorInformationEx.restype = BOOL
 
 GetNativeSystemInfo = windll.kernel32.GetNativeSystemInfo
 GetNativeSystemInfo.argtypes = [LPSYSTEM_INFO]
 GetNativeSystemInfo.restype = None
 
-GetSystemTimePreciseAsFileTime = windll.kernel32.GetSystemTimePreciseAsFileTime
-GetSystemTimePreciseAsFileTime.argtypes = [LPFILETIME]
-GetSystemTimePreciseAsFileTime.restype = None
+try:
+	GetSystemTimePreciseAsFileTime = windll.kernel32.GetSystemTimePreciseAsFileTime
+	GetSystemTimePreciseAsFileTime.argtypes = [LPFILETIME]
+	GetSystemTimePreciseAsFileTime.restype = None
+except AttributeError:
+	pass
 
 GetProductInfo = windll.kernel32.GetProductInfo
 GetProductInfo.argtypes = [DWORD, DWORD, DWORD, DWORD, PDWORD]
 GetProductInfo.restype = BOOL
 
 VerSetConditionMask = windll.kernel32.VerSetConditionMask
 VerSetConditionMask.argtypes = [ULONGLONG, ULONG, UCHAR]
@@ -190,39 +196,48 @@
 EnumSystemFirmwareTables.argtypes = [DWORD, PVOID, DWORD]
 EnumSystemFirmwareTables.restype = UINT
 
 GetSystemFirmwareTable = windll.kernel32.GetSystemFirmwareTable
 GetSystemFirmwareTable.argtypes = [DWORD, DWORD, PVOID, DWORD]
 GetSystemFirmwareTable.restype = UINT
 
-DnsHostnameToComputerNameExW = windll.kernel32.DnsHostnameToComputerNameExW
-DnsHostnameToComputerNameExW.argtypes = [LPCWSTR, LPWSTR, LPDWORD]
-DnsHostnameToComputerNameExW.restype = BOOL
+try:
+	DnsHostnameToComputerNameExW = windll.kernel32.DnsHostnameToComputerNameExW
+	DnsHostnameToComputerNameExW.argtypes = [LPCWSTR, LPWSTR, LPDWORD]
+	DnsHostnameToComputerNameExW.restype = BOOL
+except AttributeError:
+	pass
 
 GetPhysicallyInstalledSystemMemory = windll.kernel32.GetPhysicallyInstalledSystemMemory
 GetPhysicallyInstalledSystemMemory.argtypes = [PULONGLONG]
 GetPhysicallyInstalledSystemMemory.restype = BOOL
 
 SCEX2_ALT_NETBIOS_NAME = 0x00000001
 
-SetComputerNameEx2W = windll.kernel32.SetComputerNameEx2W
-SetComputerNameEx2W.argtypes = [COMPUTER_NAME_FORMAT, DWORD, LPCWSTR]
-SetComputerNameEx2W.restype = BOOL
+try:
+	SetComputerNameEx2W = windll.kernel32.SetComputerNameEx2W
+	SetComputerNameEx2W.argtypes = [COMPUTER_NAME_FORMAT, DWORD, LPCWSTR]
+	SetComputerNameEx2W.restype = BOOL
+except AttributeError:
+	pass
 
 SetSystemTimeAdjustment = windll.kernel32.SetSystemTimeAdjustment
 SetSystemTimeAdjustment.argtypes = [DWORD, BOOL]
 SetSystemTimeAdjustment.restype = BOOL
 
 #SetSystemTimeAdjustmentPrecise = windll.mincore.SetSystemTimeAdjustmentPrecise
 #SetSystemTimeAdjustmentPrecise.argtypes = [DWORD64, BOOL]
 #SetSystemTimeAdjustmentPrecise.restype = BOOL
 
-InstallELAMCertificateInfo = windll.kernel32.InstallELAMCertificateInfo
-InstallELAMCertificateInfo.argtypes = [HANDLE]
-InstallELAMCertificateInfo.restype = BOOL
+try:
+	InstallELAMCertificateInfo = windll.kernel32.InstallELAMCertificateInfo
+	InstallELAMCertificateInfo.argtypes = [HANDLE]
+	InstallELAMCertificateInfo.restype = BOOL
+except AttributeError:
+	pass
 
 GetProcessorSystemCycleTime = windll.kernel32.GetProcessorSystemCycleTime
 GetProcessorSystemCycleTime.argtypes = [USHORT, PSYSTEM_PROCESSOR_CYCLE_TIME_INFORMATION, PDWORD]
 GetProcessorSystemCycleTime.restype = BOOL
 
 #GetOsManufacturingMode = windll.XXX.GetOsManufacturingMode
 #GetOsManufacturingMode.argtypes = [PBOOL]
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/wincontypes.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/wincontypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import Structure, Union, POINTER, c_void_p
-from ctypes.wintypes import BOOL, WORD, SHORT, WCHAR, DWORD, UINT
+from ctypes import POINTER, Structure, Union, c_void_p
+from ctypes.wintypes import BOOL, DWORD, SHORT, UINT, WCHAR, WORD
 
 from ..shared.ntdef import CHAR
 
+
 class COORD(Structure):
 	# no pack
 	_fields_ = [
 		("X", SHORT),
 		("Y", SHORT)
 	]
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/wingdi.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/wingdi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import POINTER, c_int, Structure
-from ctypes.wintypes import LPCSTR, HANDLE, LPCWSTR, DWORD, BOOL, UINT, LPVOID, WORD, LONG, BYTE
+from ctypes import POINTER, Structure, c_int
+from ctypes.wintypes import BOOL, BYTE, DWORD, HANDLE, LONG, LPCSTR, LPCWSTR, LPVOID, UINT, WORD
 
 from .. import windll
 
 HDC = HANDLE
 HGDIOBJ = HANDLE
 HBITMAP = HANDLE
 
 DIB_RGB_COLORS = 0
 HORZRES = 8
 VERTRES = 10
 SRCCOPY = 0x00CC0020
 CAPTUREBLT = 0x40000000
 
 from warnings import warn
+
 warn("Don't use last parameter of `CreateDCA` or `CreateDCW`, as `DEVMODEA` and `DEVMODEW` are not defined correctly.")
 DEVMODEA = c_int
 DEVMODEW = c_int
 
 class RGBQUAD(Structure):
 	_fields_ = [
 		("rgbBlue", BYTE),
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/winioctl.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/winioctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from ctypes import Structure, Union
 from ctypes.wintypes import BOOLEAN, BYTE, DWORD, LARGE_INTEGER, WCHAR
 
 from .. import CEnum, windll
-from ..shared.ntddstor import STORAGE_BUS_TYPE
-from ..shared.guiddef import GUID
 from ..shared.basetsd import DWORD64
+from ..shared.guiddef import GUID
+from ..shared.ntddstor import STORAGE_BUS_TYPE
 from .winnt import FILE_READ_DATA, FILE_WRITE_DATA
 
+
 def CTL_CODE(DeviceType, Function, Method, Access):
 	return (DeviceType << 16) | (Access << 14) | (Function << 2) | Method
 
 def DEVICE_TYPE_FROM_CTL_CODE(ctrlCode):
 	((DWORD)(ctrlCode & 0xffff0000)) >> 16
 
 def METHOD_FROM_CTL_CODE(ctrlCode):
@@ -267,38 +268,38 @@
 FSCTL_INVALIDATE_VOLUMES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 21, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_QUERY_FAT_BPB = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 22, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_REQUEST_FILTER_OPLOCK = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 23, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_FILESYSTEM_GET_STATISTICS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 24, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_GET_NTFS_VOLUME_DATA = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 25, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_GET_NTFS_FILE_RECORD = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 26, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_GET_VOLUME_BITMAP = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 27, METHOD_NEITHER, FILE_ANY_ACCESS)
-FSCTL_GET_RETRIEVAL_POINTERS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 28, METHOD_NEITHER, FILE_ANY_ACCESS) 
+FSCTL_GET_RETRIEVAL_POINTERS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 28, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_MOVE_FILE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 29, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_IS_VOLUME_DIRTY = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 30, METHOD_BUFFERED, FILE_ANY_ACCESS)
 
 FSCTL_ALLOW_EXTENDED_DASD_IO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 32, METHOD_NEITHER, FILE_ANY_ACCESS)
 
 FSCTL_FIND_FILES_BY_SID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 35, METHOD_NEITHER, FILE_ANY_ACCESS)
 
-FSCTL_SET_OBJECT_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 38, METHOD_BUFFERED, FILE_SPECIAL_ACCESS) 
-FSCTL_GET_OBJECT_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 39, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_SET_OBJECT_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 38, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
+FSCTL_GET_OBJECT_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 39, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_DELETE_OBJECT_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 40, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
-FSCTL_SET_REPARSE_POINT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 41, METHOD_BUFFERED, FILE_SPECIAL_ACCESS) 
-FSCTL_GET_REPARSE_POINT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 42, METHOD_BUFFERED, FILE_ANY_ACCESS) 
-FSCTL_DELETE_REPARSE_POINT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 43, METHOD_BUFFERED, FILE_SPECIAL_ACCESS) 
+FSCTL_SET_REPARSE_POINT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 41, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
+FSCTL_GET_REPARSE_POINT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 42, METHOD_BUFFERED, FILE_ANY_ACCESS)
+FSCTL_DELETE_REPARSE_POINT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 43, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_ENUM_USN_DATA = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 44, METHOD_NEITHER, FILE_ANY_ACCESS)
-FSCTL_SECURITY_ID_CHECK = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 45, METHOD_NEITHER, FILE_READ_DATA) 
+FSCTL_SECURITY_ID_CHECK = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 45, METHOD_NEITHER, FILE_READ_DATA)
 FSCTL_READ_USN_JOURNAL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 46, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_SET_OBJECT_ID_EXTENDED = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 47, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
-FSCTL_CREATE_OR_GET_OBJECT_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 48, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_CREATE_OR_GET_OBJECT_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 48, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SET_SPARSE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 49, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_SET_ZERO_DATA = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 50, METHOD_BUFFERED, FILE_WRITE_DATA)
-FSCTL_QUERY_ALLOCATED_RANGES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 51, METHOD_NEITHER, FILE_READ_DATA) 
+FSCTL_QUERY_ALLOCATED_RANGES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 51, METHOD_NEITHER, FILE_READ_DATA)
 FSCTL_ENABLE_UPGRADE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 52, METHOD_BUFFERED, FILE_WRITE_DATA)
-FSCTL_SET_ENCRYPTION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 53, METHOD_NEITHER, FILE_ANY_ACCESS) 
+FSCTL_SET_ENCRYPTION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 53, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_ENCRYPTION_FSCTL_IO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 54, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_WRITE_RAW_ENCRYPTED = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 55, METHOD_NEITHER, FILE_SPECIAL_ACCESS)
 FSCTL_READ_RAW_ENCRYPTED = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 56, METHOD_NEITHER, FILE_SPECIAL_ACCESS)
 FSCTL_CREATE_USN_JOURNAL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 57, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_READ_FILE_USN_DATA = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 58, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_WRITE_USN_CLOSE_RECORD = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 59, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_EXTEND_VOLUME = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 60, METHOD_BUFFERED, FILE_ANY_ACCESS)
@@ -309,84 +310,84 @@
 FSCTL_SIS_LINK_FILES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 65, METHOD_BUFFERED, FILE_READ_DATA | FILE_WRITE_DATA)
 
 FSCTL_RECALL_FILE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 69, METHOD_NEITHER, FILE_ANY_ACCESS)
 
 FSCTL_READ_FROM_PLEX = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 71, METHOD_OUT_DIRECT, FILE_READ_DATA)
 FSCTL_FILE_PREFETCH = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 72, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 
-FSCTL_MAKE_MEDIA_COMPATIBLE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 76, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_SET_DEFECT_MANAGEMENT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 77, METHOD_BUFFERED, FILE_WRITE_DATA) 
+FSCTL_MAKE_MEDIA_COMPATIBLE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 76, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_SET_DEFECT_MANAGEMENT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 77, METHOD_BUFFERED, FILE_WRITE_DATA)
 FSCTL_QUERY_SPARING_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 78, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_QUERY_ON_DISK_VOLUME_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 79, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_SET_VOLUME_COMPRESSION_STATE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 80, METHOD_BUFFERED, FILE_SPECIAL_ACCESS) 
+FSCTL_SET_VOLUME_COMPRESSION_STATE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 80, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 
-FSCTL_TXFS_MODIFY_RM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 81, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_TXFS_QUERY_RM_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 82, METHOD_BUFFERED, FILE_READ_DATA) 
+FSCTL_TXFS_MODIFY_RM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 81, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_TXFS_QUERY_RM_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 82, METHOD_BUFFERED, FILE_READ_DATA)
 
-FSCTL_TXFS_ROLLFORWARD_REDO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 84, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_TXFS_ROLLFORWARD_UNDO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 85, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_TXFS_START_RM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 86, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_TXFS_SHUTDOWN_RM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 87, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_TXFS_READ_BACKUP_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 88, METHOD_BUFFERED, FILE_READ_DATA) 
-FSCTL_TXFS_WRITE_BACKUP_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 89, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_TXFS_CREATE_SECONDARY_RM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 90, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_TXFS_GET_METADATA_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 91, METHOD_BUFFERED, FILE_READ_DATA) 
-FSCTL_TXFS_GET_TRANSACTED_VERSION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 92, METHOD_BUFFERED, FILE_READ_DATA) 
+FSCTL_TXFS_ROLLFORWARD_REDO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 84, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_TXFS_ROLLFORWARD_UNDO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 85, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_TXFS_START_RM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 86, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_TXFS_SHUTDOWN_RM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 87, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_TXFS_READ_BACKUP_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 88, METHOD_BUFFERED, FILE_READ_DATA)
+FSCTL_TXFS_WRITE_BACKUP_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 89, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_TXFS_CREATE_SECONDARY_RM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 90, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_TXFS_GET_METADATA_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 91, METHOD_BUFFERED, FILE_READ_DATA)
+FSCTL_TXFS_GET_TRANSACTED_VERSION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 92, METHOD_BUFFERED, FILE_READ_DATA)
 
-FSCTL_TXFS_SAVEPOINT_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 94, METHOD_BUFFERED, FILE_WRITE_DATA) 
-FSCTL_TXFS_CREATE_MINIVERSION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 95, METHOD_BUFFERED, FILE_WRITE_DATA) 
+FSCTL_TXFS_SAVEPOINT_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 94, METHOD_BUFFERED, FILE_WRITE_DATA)
+FSCTL_TXFS_CREATE_MINIVERSION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 95, METHOD_BUFFERED, FILE_WRITE_DATA)
 
-FSCTL_TXFS_TRANSACTION_ACTIVE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 99, METHOD_BUFFERED, FILE_READ_DATA) 
+FSCTL_TXFS_TRANSACTION_ACTIVE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 99, METHOD_BUFFERED, FILE_READ_DATA)
 FSCTL_SET_ZERO_ON_DEALLOCATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 101, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_SET_REPAIR = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 102, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_GET_REPAIR = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 103, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_WAIT_FOR_REPAIR = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 104, METHOD_BUFFERED, FILE_ANY_ACCESS)
 
 FSCTL_INITIATE_REPAIR = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 106, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSC_INTERNAL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 107, METHOD_NEITHER, FILE_ANY_ACCESS)
-FSCTL_SHRINK_VOLUME = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 108, METHOD_BUFFERED, FILE_SPECIAL_ACCESS) 
+FSCTL_SHRINK_VOLUME = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 108, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_SET_SHORT_NAME_BEHAVIOR = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 109, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_DFSR_SET_GHOST_HANDLE_STATE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 110, METHOD_BUFFERED, FILE_ANY_ACCESS)
 
-FSCTL_TXFS_LIST_TRANSACTION_LOCKED_FILES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 120, METHOD_BUFFERED, FILE_READ_DATA) 
+FSCTL_TXFS_LIST_TRANSACTION_LOCKED_FILES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 120, METHOD_BUFFERED, FILE_READ_DATA)
 FSCTL_TXFS_LIST_TRANSACTIONS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 121, METHOD_BUFFERED, FILE_READ_DATA)
 FSCTL_QUERY_PAGEFILE_ENCRYPTION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 122, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_RESET_VOLUME_ALLOCATION_HINTS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 123, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_QUERY_DEPENDENT_VOLUME = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 124, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_QUERY_DEPENDENT_VOLUME = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 124, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SD_GLOBAL_CHANGE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 125, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_TXFS_READ_BACKUP_INFORMATION2 = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 126, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_TXFS_READ_BACKUP_INFORMATION2 = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 126, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_LOOKUP_STREAM_FROM_CLUSTER = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 127, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_TXFS_WRITE_BACKUP_INFORMATION2 = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 128, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_TXFS_WRITE_BACKUP_INFORMATION2 = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 128, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_FILE_TYPE_NOTIFICATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 129, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_FILE_LEVEL_TRIM = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 130, METHOD_BUFFERED, FILE_WRITE_DATA)
 
 FSCTL_GET_BOOT_AREA_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 140, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_GET_RETRIEVAL_POINTER_BASE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 141, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SET_PERSISTENT_VOLUME_STATE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 142, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_QUERY_PERSISTENT_VOLUME_STATE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 143, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_QUERY_PERSISTENT_VOLUME_STATE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 143, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_REQUEST_OPLOCK = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 144, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_TUNNEL_REQUEST = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 145, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_IS_CSV_FILE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 146, METHOD_BUFFERED, FILE_ANY_ACCESS) 
-FSCTL_QUERY_FILE_SYSTEM_RECOGNITION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 147, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_IS_CSV_FILE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 146, METHOD_BUFFERED, FILE_ANY_ACCESS)
+FSCTL_QUERY_FILE_SYSTEM_RECOGNITION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 147, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_GET_VOLUME_PATH_NAME = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 148, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_GET_VOLUME_NAME_FOR_VOLUME_MOUNT_POINT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 149, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_GET_VOLUME_PATH_NAMES_FOR_VOLUME_NAME = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 150, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_IS_FILE_ON_CSV_VOLUME = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 151, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CORRUPTION_HANDLING = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 152, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_OFFLOAD_READ = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 153, METHOD_BUFFERED, FILE_READ_ACCESS)
 FSCTL_OFFLOAD_WRITE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 154, METHOD_BUFFERED, FILE_WRITE_ACCESS)
 FSCTL_CSV_INTERNAL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 155, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SET_PURGE_FAILURE_MODE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 156, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_QUERY_FILE_LAYOUT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 157, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_IS_VOLUME_OWNED_BYCSVFS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 158, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_GET_INTEGRITY_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 159, METHOD_BUFFERED, FILE_ANY_ACCESS) 
-FSCTL_SET_INTEGRITY_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 160, METHOD_BUFFERED, FILE_READ_DATA | FILE_WRITE_DATA) 
+FSCTL_GET_INTEGRITY_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 159, METHOD_BUFFERED, FILE_ANY_ACCESS)
+FSCTL_SET_INTEGRITY_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 160, METHOD_BUFFERED, FILE_READ_DATA | FILE_WRITE_DATA)
 FSCTL_QUERY_FILE_REGIONS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 161, METHOD_BUFFERED, FILE_ANY_ACCESS)
 
-FSCTL_RKF_INTERNAL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 171, METHOD_NEITHER, FILE_ANY_ACCESS) 
+FSCTL_RKF_INTERNAL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 171, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_SCRUB_DATA = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 172, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_REPAIR_COPIES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 173, METHOD_BUFFERED, FILE_READ_DATA | FILE_WRITE_DATA)
 FSCTL_DISABLE_LOCAL_BUFFERING = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 174, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_MGMT_LOCK = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 175, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_QUERY_DOWN_LEVEL_FILE_SYSTEM_CHARACTERISTICS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 176, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_ADVANCE_FILE_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 177, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_SYNC_TUNNEL_REQUEST = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 178, METHOD_BUFFERED, FILE_ANY_ACCESS)
@@ -394,15 +395,15 @@
 FSCTL_WRITE_USN_REASON = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 180, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_CONTROL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 181, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_GET_REFS_VOLUME_DATA = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 182, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_CSV_H_BREAKING_SYNC_TUNNEL_REQUEST = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 185, METHOD_BUFFERED, FILE_ANY_ACCESS)
 
 FSCTL_QUERY_STORAGE_CLASSES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 187, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_QUERY_REGION_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 188, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_USN_TRACK_MODIFIED_RANGES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 189, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_USN_TRACK_MODIFIED_RANGES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 189, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_QUERY_SHARED_VIRTUAL_DISK_SUPPORT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 192, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SVHDX_SYNC_TUNNEL_REQUEST = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 193, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SVHDX_SET_INITIATOR_INFORMATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 194, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SET_EXTERNAL_BACKING = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 195, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_GET_EXTERNAL_BACKING = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 196, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_DELETE_EXTERNAL_BACKING = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 197, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_ENUM_EXTERNAL_BACKING = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 198, METHOD_BUFFERED, FILE_ANY_ACCESS)
@@ -416,21 +417,21 @@
 FSCTL_STORAGE_QOS_CONTROL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 212, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_INITIATE_FILE_METADATA_OPTIMIZATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 215, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_QUERY_FILE_METADATA_OPTIMIZATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 216, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 FSCTL_SVHDX_ASYNC_TUNNEL_REQUEST = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 217, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_GET_WOF_VERSION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 218, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_HCS_SYNC_TUNNEL_REQUEST = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 219, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_HCS_ASYNC_TUNNEL_REQUEST = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 220, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_QUERY_EXTENT_READ_CACHE_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 221, METHOD_NEITHER, FILE_ANY_ACCESS) 
-FSCTL_QUERY_REFS_VOLUME_COUNTER_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 222, METHOD_NEITHER, FILE_ANY_ACCESS) 
+FSCTL_QUERY_EXTENT_READ_CACHE_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 221, METHOD_NEITHER, FILE_ANY_ACCESS)
+FSCTL_QUERY_REFS_VOLUME_COUNTER_INFO = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 222, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_CLEAN_VOLUME_METADATA = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 223, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_SET_INTEGRITY_INFORMATION_EX = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 224, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_SET_INTEGRITY_INFORMATION_EX = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 224, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SUSPEND_OVERLAY = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 225, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_VIRTUAL_STORAGE_QUERY_PROPERTY = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 226, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_FILESYSTEM_GET_STATISTICS_EX = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 227, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_FILESYSTEM_GET_STATISTICS_EX = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 227, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_QUERY_VOLUME_CONTAINER_STATE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 228, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SET_LAYER_ROOT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 229, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_QUERY_DIRECT_ACCESS_EXTENTS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 230, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_NOTIFY_STORAGE_SPACE_ALLOCATION = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 231, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SSDI_STORAGE_REQUEST = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 232, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_QUERY_DIRECT_IMAGE_ORIGINAL_BASE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 233, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_READ_UNPRIVILEGED_USN_JOURNAL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 234, METHOD_NEITHER, FILE_ANY_ACCESS)
@@ -451,23 +452,23 @@
 FSCTL_DUPLICATE_EXTENTS_TO_FILE_EX = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 250, METHOD_BUFFERED, FILE_WRITE_DATA)
 FSCTL_QUERY_BAD_RANGES = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 251, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SET_DAX_ALLOC_ALIGNMENT_HINT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 252, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_DELETE_CORRUPTED_REFS_CONTAINER = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 253, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SCRUB_UNDISCOVERABLE_ID = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 254, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_NOTIFY_DATA_CHANGE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 255, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_START_VIRTUALIZATION_INSTANCE_EX = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 256, METHOD_BUFFERED, FILE_ANY_ACCESS)
-FSCTL_ENCRYPTION_KEY_CONTROL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 257, METHOD_BUFFERED, FILE_ANY_ACCESS) 
+FSCTL_ENCRYPTION_KEY_CONTROL = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 257, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_VIRTUAL_STORAGE_SET_BEHAVIOR = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 258, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_SET_REPARSE_POINT_EX = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 259, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
-FSCTL_REARRANGE_FILE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 264, METHOD_BUFFERED, FILE_READ_ACCESS | FILE_WRITE_ACCESS) 
+FSCTL_REARRANGE_FILE = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 264, METHOD_BUFFERED, FILE_READ_ACCESS | FILE_WRITE_ACCESS)
 FSCTL_VIRTUAL_STORAGE_PASSTHROUGH = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 265, METHOD_BUFFERED, FILE_ANY_ACCESS)
 FSCTL_GET_RETRIEVAL_POINTER_COUNT = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 266, METHOD_NEITHER, FILE_ANY_ACCESS)
 FSCTL_ENABLE_PER_IO_FLAGS = CTL_CODE(FILE_DEVICE_FILE_SYSTEM, 267, METHOD_BUFFERED, FILE_ANY_ACCESS)
 
-""" FILE_DEVICE_AVIO is not defined anywhere in `Windows Kits\10\Include\10.0.17763.0`
+r""" FILE_DEVICE_AVIO is not defined anywhere in `Windows Kits\10\Include\10.0.17763.0`
 IOCTL_AVIO_ALLOCATE_STREAM = CTL_CODE(FILE_DEVICE_AVIO, 1, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 IOCTL_AVIO_FREE_STREAM = CTL_CODE(FILE_DEVICE_AVIO, 2, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 IOCTL_AVIO_MODIFY_STREAM = CTL_CODE(FILE_DEVICE_AVIO, 3, METHOD_BUFFERED, FILE_SPECIAL_ACCESS)
 """
 
 class STORAGE_QUERY_TYPE(CEnum):
 	PropertyStandardQuery = 0
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/um/winnt.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/um/winnt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from ctypes import Structure, Union, sizeof, POINTER, CFUNCTYPE
-from ctypes import c_char, c_short, c_long
-from ctypes.wintypes import BYTE, WORD, DWORD, WCHAR, HANDLE
+from ctypes import CFUNCTYPE, POINTER, Structure, Union, c_char, c_long, c_short, sizeof
+from ctypes.wintypes import BYTE, DWORD, HANDLE, WCHAR, WORD
 
 from .. import CEnum, windll
-from ..shared.guiddef import GUID
-from ..shared.basetsd import KAFFINITY, DWORD64, PDWORD64, ULONG_PTR
-from ..shared.ntdef import CHAR, PVOID64, PVOID, LONGLONG, ULONGLONG
 from ..km.crt.excpt import EXCEPTION_DISPOSITION
+from ..shared.basetsd import DWORD64, KAFFINITY, PDWORD64, ULONG_PTR
+from ..shared.guiddef import GUID
+from ..shared.ntdef import CHAR, LONGLONG, PVOID, PVOID64, ULONGLONG
 
-CHAR = c_char
 SHORT = c_short
 LONG = c_long
 
 CPOINTER = POINTER
 
 ANYSIZE_ARRAY = 1
 
@@ -9432,8 +9430,8 @@
 ACTIVATION_CONTEXT_SECTION_COM_INTERFACE_REDIRECTION = 5
 ACTIVATION_CONTEXT_SECTION_COM_TYPE_LIBRARY_REDIRECTION = 6
 ACTIVATION_CONTEXT_SECTION_COM_PROGID_REDIRECTION = 7
 ACTIVATION_CONTEXT_SECTION_GLOBAL_OBJECT_RENAME_TABLE = 8
 ACTIVATION_CONTEXT_SECTION_CLR_SURROGATES = 9
 ACTIVATION_CONTEXT_SECTION_APPLICATION_SETTINGS = 10
 ACTIVATION_CONTEXT_SECTION_COMPATIBILITY_INFO = 11
-'''
+'''
```

### Comparing `ctypes-windows-sdk-0.0.8/cwinsdk/windows.py` & `ctypes-windows-sdk-0.0.9/cwinsdk/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from .shared.ntdddisk import *
 from .shared.ntddscsi import *
 from .shared.ntddstor import *
 from .shared.ntdef import *
 from .shared.secext import *
 from .shared.windef import *
 from .shared.winerror import *
-
 from .um.consoleapi2 import *
 from .um.fileapi import *
 from .um.handleapi import *
 from .um.ioapiset import *
 from .um.libloaderapi import *
 from .um.minwinbase import *
 from .um.processenv import *
```

### Comparing `ctypes-windows-sdk-0.0.8/setup.py` & `ctypes-windows-sdk-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from setuptools import setup
-
 from io import open
 
+from setuptools import setup
+
 with open("README.md", "r", encoding="utf-8") as fr:
 	long_description = fr.read()
 
 setup(
 	author="Dobatymo",
 	name="ctypes-windows-sdk",
-	version="0.0.8",
+	version="0.0.9",
 	url="https://github.com/Dobatymo/ctypes-windows-sdk",
 	description="Ctypes port of Windows SDK",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	classifiers=[
 		"Development Status :: 3 - Alpha",
 		"Intended Audience :: Developers",
```

