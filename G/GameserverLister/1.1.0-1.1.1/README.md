# Comparing `tmp/GameserverLister-1.1.0.tar.gz` & `tmp/gameserverlister-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameserverLister-1.1.0.tar", last modified: Fri Sep  8 12:12:04 2023, max compression
+gzip compressed data, was "gameserverlister-1.1.1.tar", last modified: Tue Apr 23 22:53:55 2024, max compression
```

## Comparing `GameserverLister-1.1.0.tar` & `gameserverlister-1.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:04.414989 GameserverLister-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:04.406988 GameserverLister-1.1.0/GameserverLister/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:04.410989 GameserverLister-1.1.0/GameserverLister/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/bfbc2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/gametools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/medalofhonor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:04.410989 GameserverLister-1.1.0/GameserverLister/commands/options/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/options/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/options/gameport.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/options/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/options/queryport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/quake3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/commands/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:04.410989 GameserverLister-1.1.0/GameserverLister/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    16878 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/common/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/common/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/common/weblinks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:04.410989 GameserverLister-1.1.0/GameserverLister/games/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/games/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/games/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/games/gametools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8787 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/games/quake3.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/games/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/games/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:04.410989 GameserverLister-1.1.0/GameserverLister/listers/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/battlelog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/bfbc2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/gamespy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/gametools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/medalofhonor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/quake3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/unreal2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/GameserverLister/listers/valve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:04.406988 GameserverLister-1.1.0/GameserverLister.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18226 2023-09-08 12:12:04.000000 GameserverLister-1.1.0/GameserverLister.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2023-09-08 12:12:04.000000 GameserverLister-1.1.0/GameserverLister.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 12:12:04.000000 GameserverLister-1.1.0/GameserverLister.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-08 12:12:04.000000 GameserverLister-1.1.0/GameserverLister.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-08 12:12:04.000000 GameserverLister-1.1.0/GameserverLister.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-08 12:12:04.000000 GameserverLister-1.1.0/GameserverLister.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18226 2023-09-08 12:12:04.414989 GameserverLister-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2023-09-08 12:12:04.414989 GameserverLister-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 12:11:55.000000 GameserverLister-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:55.389425 gameserverlister-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:55.381425 gameserverlister-1.1.1/GameserverLister/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:55.381425 gameserverlister-1.1.1/GameserverLister/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/bfbc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/medalofhonor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:55.385425 gameserverlister-1.1.1/GameserverLister/commands/options/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/options/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/options/gameport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/options/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/options/queryport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/commands/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:55.385425 gameserverlister-1.1.1/GameserverLister/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/common/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/common/weblinks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:55.385425 gameserverlister-1.1.1/GameserverLister/games/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/games/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/games/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/games/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8787 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/games/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/games/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/games/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:55.385425 gameserverlister-1.1.1/GameserverLister/listers/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/battlelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/bfbc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/gamespy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/gametools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/medalofhonor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/quake3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/unreal2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/GameserverLister/listers/valve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:53:55.389425 gameserverlister-1.1.1/GameserverLister.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18226 2024-04-23 22:53:55.000000 gameserverlister-1.1.1/GameserverLister.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-23 22:53:55.000000 gameserverlister-1.1.1/GameserverLister.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:53:55.000000 gameserverlister-1.1.1/GameserverLister.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 22:53:55.000000 gameserverlister-1.1.1/GameserverLister.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 22:53:55.000000 gameserverlister-1.1.1/GameserverLister.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 22:53:55.000000 gameserverlister-1.1.1/GameserverLister.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18226 2024-04-23 22:53:55.389425 gameserverlister-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-23 22:53:55.389425 gameserverlister-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:53:45.000000 gameserverlister-1.1.1/setup.py
```

### Comparing `GameserverLister-1.1.0/GameserverLister/__main__.py` & `gameserverlister-1.1.1/GameserverLister/__main__.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/battlelog.py` & `gameserverlister-1.1.1/GameserverLister/commands/battlelog.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/bfbc2.py` & `gameserverlister-1.1.1/GameserverLister/commands/bfbc2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/gamespy.py` & `gameserverlister-1.1.1/GameserverLister/commands/gamespy.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/gametools.py` & `gameserverlister-1.1.1/GameserverLister/commands/gametools.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/medalofhonor.py` & `gameserverlister-1.1.1/GameserverLister/commands/medalofhonor.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/options/common.py` & `gameserverlister-1.1.1/GameserverLister/commands/options/common.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/options/http.py` & `gameserverlister-1.1.1/GameserverLister/commands/options/http.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/quake3.py` & `gameserverlister-1.1.1/GameserverLister/commands/quake3.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/unreal2.py` & `gameserverlister-1.1.1/GameserverLister/commands/unreal2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/commands/valve.py` & `gameserverlister-1.1.1/GameserverLister/commands/valve.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/common/helpers.py` & `gameserverlister-1.1.1/GameserverLister/common/helpers.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/common/servers.py` & `gameserverlister-1.1.1/GameserverLister/common/servers.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/common/types.py` & `gameserverlister-1.1.1/GameserverLister/common/types.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/common/weblinks.py` & `gameserverlister-1.1.1/GameserverLister/common/weblinks.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/games/gamespy.py` & `gameserverlister-1.1.1/GameserverLister/games/gamespy.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/games/quake3.py` & `gameserverlister-1.1.1/GameserverLister/games/quake3.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/games/unreal2.py` & `gameserverlister-1.1.1/GameserverLister/games/unreal2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/games/valve.py` & `gameserverlister-1.1.1/GameserverLister/games/valve.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/__init__.py` & `gameserverlister-1.1.1/GameserverLister/listers/__init__.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/battlelog.py` & `gameserverlister-1.1.1/GameserverLister/listers/battlelog.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/bfbc2.py` & `gameserverlister-1.1.1/GameserverLister/listers/bfbc2.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     def update_server_list(self):
         request_ok = False
         attempt = 0
         max_attempts = 3
         servers = None
         while not request_ok and attempt < max_attempts:
             try:
-                logging.info('Fetching server list from FESL/Theater API')
-                resp = self.session.get('https://fesl.cetteup.com/servers/pc', timeout=self.request_timeout)
+                logging.info('Fetching server list from Project Rome API')
+                resp = self.session.get('http://api.emulatornexus.com/v1/rome/servers', timeout=self.request_timeout)
 
                 if resp.ok:
                     servers = resp.json()
                     request_ok = True
                 else:
                     attempt += 1
             except requests.exceptions.RequestException as e:
@@ -43,20 +43,20 @@
             logging.error('Failed to retrieve server list, exiting')
             sys.exit(1)
 
         # Add servers from list
         found_servers = []
         for server in servers:
             found_server = BadCompany2Server(
-                guid_from_ip_port(server['I'], server['P']),
-                server['N'],
-                int(server['LID']),
-                int(server['GID']),
-                server['I'],
-                int(server['P'])
+                guid_from_ip_port(server['remote_ip'], server['remote_port']),
+                server['hostname'],
+                257, # Project Rome only uses 257, but will return all servers regardless of the given LID
+                server['id'],
+                server['remote_ip'],
+                server['remote_port']
             )
 
             if self.add_links:
                 found_server.add_links(self.build_server_links(
                     found_server.uid,
                     found_server.ip,
                     found_server.game_port
@@ -66,15 +66,15 @@
 
         self.add_update_servers(found_servers)
 
     def check_if_server_still_exists(self, server: BadCompany2Server, checks_since_last_ok: int) -> Tuple[bool, bool, int]:
         check_ok = True
         found = False
         try:
-            response = self.session.get(f'https://fesl.cetteup.com/servers/pc/{server.lid}/{server.gid}',
+            response = self.session.get(f'http://api.emulatornexus.com/v1/rome/server/{server.gid}',
                                         timeout=self.request_timeout)
 
             if response.ok:
                 found = True
             elif response.status_code == 404:
                 found = False
             else:
```

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/common.py` & `gameserverlister-1.1.1/GameserverLister/listers/common.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/gamespy.py` & `gameserverlister-1.1.1/GameserverLister/listers/gamespy.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/gametools.py` & `gameserverlister-1.1.1/GameserverLister/listers/gametools.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/medalofhonor.py` & `gameserverlister-1.1.1/GameserverLister/listers/medalofhonor.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/quake3.py` & `gameserverlister-1.1.1/GameserverLister/listers/quake3.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/unreal2.py` & `gameserverlister-1.1.1/GameserverLister/listers/unreal2.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister/listers/valve.py` & `gameserverlister-1.1.1/GameserverLister/listers/valve.py`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/GameserverLister.egg-info/PKG-INFO` & `gameserverlister-1.1.1/GameserverLister.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameserverLister
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python command line tool to retrieve game server lists for various games
 Home-page: https://github.com/cetteup/GameserverLister
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/GameserverLister/issues
 Classifier: Development Status :: 4 - Beta
@@ -101,15 +101,15 @@
 | ARK: Survival Evolved                  | Valve                | Valve ¹                                                                                                           |
 | Arma 2                                 | Valve                | Valve ¹                                                                                                           |
 | Arma 3                                 | Valve                | Valve ¹                                                                                                           |
 | Battlefield 1942                       | GameSpy              | bf1942.org, openspy.net, qtracker.com                                                                             |
 | Battlefield Vietnam                    | GameSpy              | openspy.net, qtracker.com                                                                                         |
 | Battlefield 2                          | GamsSpy              | bf2hub.com, playbf2.ru                                                                                            |
 | Battlefield 2142                       | GameSpy              | novgames.ru, openspy.net, play2142.ru                                                                             |
-| Battlefield: Bad Company 2             | fesl/theater         | Electronic Arts                                                                                                   |
+| Battlefield: Bad Company 2             | fesl/theater         | Project Rome (emulatornexus.com)                                                                                  |
 | Battlefield 3                          | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield 4                          | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield Hardline                   | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield 1                          | Gametools API        | api.gametools.network                                                                                             |
 | Battlefield 5                          | Gametools API        | api.gametools.network                                                                                             |
 | Call of Duty                           | Quake3               | Activision                                                                                                        |
 | Call of Duty: United Offensive         | Quake3               | Activision                                                                                                        |
```

### Comparing `GameserverLister-1.1.0/GameserverLister.egg-info/SOURCES.txt` & `gameserverlister-1.1.1/GameserverLister.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/LICENSE.md` & `gameserverlister-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `GameserverLister-1.1.0/PKG-INFO` & `gameserverlister-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameserverLister
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python command line tool to retrieve game server lists for various games
 Home-page: https://github.com/cetteup/GameserverLister
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/GameserverLister/issues
 Classifier: Development Status :: 4 - Beta
@@ -101,15 +101,15 @@
 | ARK: Survival Evolved                  | Valve                | Valve ¹                                                                                                           |
 | Arma 2                                 | Valve                | Valve ¹                                                                                                           |
 | Arma 3                                 | Valve                | Valve ¹                                                                                                           |
 | Battlefield 1942                       | GameSpy              | bf1942.org, openspy.net, qtracker.com                                                                             |
 | Battlefield Vietnam                    | GameSpy              | openspy.net, qtracker.com                                                                                         |
 | Battlefield 2                          | GamsSpy              | bf2hub.com, playbf2.ru                                                                                            |
 | Battlefield 2142                       | GameSpy              | novgames.ru, openspy.net, play2142.ru                                                                             |
-| Battlefield: Bad Company 2             | fesl/theater         | Electronic Arts                                                                                                   |
+| Battlefield: Bad Company 2             | fesl/theater         | Project Rome (emulatornexus.com)                                                                                  |
 | Battlefield 3                          | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield 4                          | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield Hardline                   | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield 1                          | Gametools API        | api.gametools.network                                                                                             |
 | Battlefield 5                          | Gametools API        | api.gametools.network                                                                                             |
 | Call of Duty                           | Quake3               | Activision                                                                                                        |
 | Call of Duty: United Offensive         | Quake3               | Activision                                                                                                        |
```

### Comparing `GameserverLister-1.1.0/README.md` & `gameserverlister-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 | ARK: Survival Evolved                  | Valve                | Valve ¹                                                                                                           |
 | Arma 2                                 | Valve                | Valve ¹                                                                                                           |
 | Arma 3                                 | Valve                | Valve ¹                                                                                                           |
 | Battlefield 1942                       | GameSpy              | bf1942.org, openspy.net, qtracker.com                                                                             |
 | Battlefield Vietnam                    | GameSpy              | openspy.net, qtracker.com                                                                                         |
 | Battlefield 2                          | GamsSpy              | bf2hub.com, playbf2.ru                                                                                            |
 | Battlefield 2142                       | GameSpy              | novgames.ru, openspy.net, play2142.ru                                                                             |
-| Battlefield: Bad Company 2             | fesl/theater         | Electronic Arts                                                                                                   |
+| Battlefield: Bad Company 2             | fesl/theater         | Project Rome (emulatornexus.com)                                                                                  |
 | Battlefield 3                          | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield 4                          | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield Hardline                   | Battlelog            | battlelog.com                                                                                                     |
 | Battlefield 1                          | Gametools API        | api.gametools.network                                                                                             |
 | Battlefield 5                          | Gametools API        | api.gametools.network                                                                                             |
 | Call of Duty                           | Quake3               | Activision                                                                                                        |
 | Call of Duty: United Offensive         | Quake3               | Activision                                                                                                        |
```

### Comparing `GameserverLister-1.1.0/setup.cfg` & `gameserverlister-1.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = GameserverLister
-version = 1.1.0
+version = 1.1.1
 description = Python command line tool to retrieve game server lists for various games
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cetteup/GameserverLister
 project_urls = 
 	Bug Tracker = https://github.com/cetteup/GameserverLister/issues
 author = cetteup
```

