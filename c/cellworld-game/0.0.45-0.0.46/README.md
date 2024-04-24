# Comparing `tmp/cellworld_game-0.0.45.tar.gz` & `tmp/cellworld_game-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_game-0.0.45.tar", last modified: Tue Apr 23 23:34:32 2024, max compression
+gzip compressed data, was "cellworld_game-0.0.46.tar", last modified: Wed Apr 24 01:44:43 2024, max compression
```

## Comparing `cellworld_game-0.0.45.tar` & `cellworld_game-0.0.46.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 23:34:32.009029 cellworld_game-0.0.45/
--rw-rw-rw-   0        0        0       36 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2024-04-23 23:34:32.007029 cellworld_game-0.0.45/PKG-INFO
--rw-rw-rw-   0        0        0       33 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 23:34:31.978029 cellworld_game-0.0.45/cellworld_game/
--rw-rw-rw-   0        0        0       33 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game/README.md
--rw-rw-rw-   0        0        0      432 2024-04-22 19:42:31.000000 cellworld_game-0.0.45/cellworld_game/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:34:32.001028 cellworld_game-0.0.45/cellworld_game/__pycache__/
--rw-rw-rw-   0        0        0      746 2024-04-22 19:55:16.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     9878 2024-04-23 17:26:05.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     6793 2024-04-23 17:37:12.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/botevade.cpython-312.pyc
--rw-rw-rw-   0        0        0     4974 2024-04-10 15:31:18.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
--rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/geometry.cpython-312.pyc
--rw-rw-rw-   0        0        0     8930 2024-04-23 15:17:25.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/model.cpython-312.pyc
--rw-rw-rw-   0        0        0     2208 2024-04-23 16:26:46.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/mouse.cpython-312.pyc
--rw-rw-rw-   0        0        0     2598 2024-04-21 15:32:53.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/navigation.cpython-312.pyc
--rw-rw-rw-   0        0        0     5807 2024-04-23 17:27:58.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     6071 2024-04-21 15:32:53.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
--rw-rw-rw-   0        0        0      870 2024-04-21 15:16:32.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/resources.cpython-312.pyc
--rw-rw-rw-   0        0        0     2760 2024-04-22 18:51:18.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/robot.cpython-312.pyc
--rw-rw-rw-   0        0        0     9945 2024-04-23 16:16:30.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/util.cpython-312.pyc
--rw-rw-rw-   0        0        0     9750 2024-04-23 17:30:08.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/view.cpython-312.pyc
--rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.45/cellworld_game/__pycache__/visibility.cpython-312.pyc
--rw-rw-rw-   0        0        0     6025 2024-04-23 17:23:52.000000 cellworld_game-0.0.45/cellworld_game/agent.py
--rw-rw-rw-   0        0        0     5255 2024-04-23 17:37:06.000000 cellworld_game-0.0.45/cellworld_game/botevade.py
--rw-rw-rw-   0        0        0     3620 2024-04-10 15:24:24.000000 cellworld_game-0.0.45/cellworld_game/cellworld_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:34:32.005028 cellworld_game-0.0.45/cellworld_game/files/
--rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.45/cellworld_game/files/agent.png
--rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.45/cellworld_game/files/predator.png
--rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.45/cellworld_game/files/prey.png
--rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.45/cellworld_game/geometry.py
--rw-rw-rw-   0        0        0     1636 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game/license.txt
--rw-rw-rw-   0        0        0     7065 2024-04-23 15:16:43.000000 cellworld_game-0.0.45/cellworld_game/model.py
--rw-rw-rw-   0        0        0     1167 2024-04-23 16:26:41.000000 cellworld_game-0.0.45/cellworld_game/mouse.py
--rw-rw-rw-   0        0        0     1717 2024-04-21 15:19:56.000000 cellworld_game-0.0.45/cellworld_game/navigation.py
--rw-rw-rw-   0        0        0     4411 2024-04-23 17:27:55.000000 cellworld_game-0.0.45/cellworld_game/navigation_agent.py
--rw-rw-rw-   0        0        0     4973 2024-04-21 15:20:54.000000 cellworld_game-0.0.45/cellworld_game/ray_tracing.py
--rw-rw-rw-   0        0        0      220 2024-04-19 14:17:58.000000 cellworld_game-0.0.45/cellworld_game/resources.py
--rw-rw-rw-   0        0        0     1555 2024-04-22 18:49:08.000000 cellworld_game-0.0.45/cellworld_game/robot.py
--rw-rw-rw-   0        0        0      183 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game/setup.cfg
--rw-rw-rw-   0        0        0     7912 2024-04-23 16:14:29.000000 cellworld_game-0.0.45/cellworld_game/util.py
--rw-rw-rw-   0        0        0     6582 2024-04-23 17:30:02.000000 cellworld_game-0.0.45/cellworld_game/view.py
--rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.45/cellworld_game/visibility.py
-drwxrwxrwx   0        0        0        0 2024-04-23 23:34:32.006029 cellworld_game-0.0.45/cellworld_game.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1621 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/cellworld_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 23:34:32.009029 cellworld_game-0.0.45/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-04-23 23:34:31.000000 cellworld_game-0.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:44:43.093804 cellworld_game-0.0.46/
+-rw-rw-rw-   0        0        0       36 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/MANIFEST.in
+-rw-rw-rw-   0        0        0      474 2024-04-24 01:44:43.091789 cellworld_game-0.0.46/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 01:44:43.055784 cellworld_game-0.0.46/cellworld_game/
+-rw-rw-rw-   0        0        0       33 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game/README.md
+-rw-rw-rw-   0        0        0      432 2024-04-22 19:42:31.000000 cellworld_game-0.0.46/cellworld_game/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:44:43.084783 cellworld_game-0.0.46/cellworld_game/__pycache__/
+-rw-rw-rw-   0        0        0      746 2024-04-22 19:55:16.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9878 2024-04-23 17:26:05.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6793 2024-04-23 17:37:12.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/botevade.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4974 2024-04-10 15:31:18.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/geometry.cpython-312.pyc
+-rw-rw-rw-   0        0        0     8930 2024-04-23 15:17:25.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/model.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2208 2024-04-23 16:26:46.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/mouse.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2598 2024-04-21 15:32:53.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/navigation.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5807 2024-04-23 17:27:58.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6071 2024-04-21 15:32:53.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
+-rw-rw-rw-   0        0        0      870 2024-04-21 15:16:32.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/resources.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2760 2024-04-22 18:51:18.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/robot.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9945 2024-04-23 16:16:30.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/util.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9750 2024-04-23 17:30:08.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/view.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.46/cellworld_game/__pycache__/visibility.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6025 2024-04-23 17:23:52.000000 cellworld_game-0.0.46/cellworld_game/agent.py
+-rw-rw-rw-   0        0        0     5255 2024-04-23 17:37:06.000000 cellworld_game-0.0.46/cellworld_game/botevade.py
+-rw-rw-rw-   0        0        0     3620 2024-04-10 15:24:24.000000 cellworld_game-0.0.46/cellworld_game/cellworld_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:44:43.089784 cellworld_game-0.0.46/cellworld_game/files/
+-rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.46/cellworld_game/files/agent.png
+-rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.46/cellworld_game/files/predator.png
+-rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.46/cellworld_game/files/prey.png
+-rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.46/cellworld_game/geometry.py
+-rw-rw-rw-   0        0        0     1636 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game/license.txt
+-rw-rw-rw-   0        0        0     7065 2024-04-23 15:16:43.000000 cellworld_game-0.0.46/cellworld_game/model.py
+-rw-rw-rw-   0        0        0     1167 2024-04-23 16:26:41.000000 cellworld_game-0.0.46/cellworld_game/mouse.py
+-rw-rw-rw-   0        0        0     1717 2024-04-21 15:19:56.000000 cellworld_game-0.0.46/cellworld_game/navigation.py
+-rw-rw-rw-   0        0        0     4411 2024-04-23 17:27:55.000000 cellworld_game-0.0.46/cellworld_game/navigation_agent.py
+-rw-rw-rw-   0        0        0     4973 2024-04-21 15:20:54.000000 cellworld_game-0.0.46/cellworld_game/ray_tracing.py
+-rw-rw-rw-   0        0        0      220 2024-04-19 14:17:58.000000 cellworld_game-0.0.46/cellworld_game/resources.py
+-rw-rw-rw-   0        0        0     1555 2024-04-22 18:49:08.000000 cellworld_game-0.0.46/cellworld_game/robot.py
+-rw-rw-rw-   0        0        0      183 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game/setup.cfg
+-rw-rw-rw-   0        0        0     7912 2024-04-23 16:14:29.000000 cellworld_game-0.0.46/cellworld_game/util.py
+-rw-rw-rw-   0        0        0     6582 2024-04-23 17:30:02.000000 cellworld_game-0.0.46/cellworld_game/view.py
+-rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.46/cellworld_game/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-24 01:44:43.090865 cellworld_game-0.0.46/cellworld_game.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1621 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/cellworld_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 01:44:43.093804 cellworld_game-0.0.46/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-04-24 01:44:42.000000 cellworld_game-0.0.46/setup.py
```

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/__init__.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/agent.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/botevade.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/botevade.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/geometry.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/geometry.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/model.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/model.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/mouse.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/mouse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/navigation.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/navigation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/resources.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/resources.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/robot.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/robot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/util.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/util.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/view.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/view.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/__pycache__/visibility.cpython-312.pyc` & `cellworld_game-0.0.46/cellworld_game/__pycache__/visibility.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/agent.py` & `cellworld_game-0.0.46/cellworld_game/agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/botevade.py` & `cellworld_game-0.0.46/cellworld_game/botevade.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/cellworld_loader.py` & `cellworld_game-0.0.46/cellworld_game/cellworld_loader.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/files/agent.png` & `cellworld_game-0.0.46/cellworld_game/files/agent.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/files/predator.png` & `cellworld_game-0.0.46/cellworld_game/files/predator.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/files/prey.png` & `cellworld_game-0.0.46/cellworld_game/files/prey.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/license.txt` & `cellworld_game-0.0.46/cellworld_game/license.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/model.py` & `cellworld_game-0.0.46/cellworld_game/model.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/mouse.py` & `cellworld_game-0.0.46/cellworld_game/mouse.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/navigation.py` & `cellworld_game-0.0.46/cellworld_game/navigation.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/navigation_agent.py` & `cellworld_game-0.0.46/cellworld_game/navigation_agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/ray_tracing.py` & `cellworld_game-0.0.46/cellworld_game/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/robot.py` & `cellworld_game-0.0.46/cellworld_game/robot.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/util.py` & `cellworld_game-0.0.46/cellworld_game/util.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/view.py` & `cellworld_game-0.0.46/cellworld_game/view.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game/visibility.py` & `cellworld_game-0.0.46/cellworld_game/visibility.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/cellworld_game.egg-info/SOURCES.txt` & `cellworld_game-0.0.46/cellworld_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.45/setup.py` & `cellworld_game-0.0.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,9 +7,9 @@
       author_email='germanespinosa@gmail.com',
       long_description=open('./cellworld_game/README.md').read() + '\n---\n<small>Package created with Easy-pack</small>\n',
       long_description_content_type='text/markdown',
       packages=['cellworld_game'],
       install_requires=['cellworld', 'pygame', 'shapely'],
       license='MIT',
       include_package_data=True,
-      version='0.0.45',
+      version='0.0.46',
       zip_safe=False)
```

