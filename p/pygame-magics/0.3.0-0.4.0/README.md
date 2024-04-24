# Comparing `tmp/pygame_magics-0.3.0.tar.gz` & `tmp/pygame_magics-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_magics-0.3.0.tar", last modified: Wed Apr 24 17:39:53 2024, max compression
+gzip compressed data, was "pygame_magics-0.4.0.tar", last modified: Wed Apr 24 18:44:21 2024, max compression
```

## Comparing `pygame_magics-0.3.0.tar` & `pygame_magics-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:39:53.492866 pygame_magics-0.3.0/
--rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 17:39:53.492644 pygame_magics-0.3.0/PKG-INFO
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:39:53.490587 pygame_magics-0.3.0/pygame_magics/
--rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:21:17.000000 pygame_magics-0.3.0/pygame_magics/__init__.py
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:39:53.491500 pygame_magics-0.3.0/pygame_magics/camera/
--rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 16:50:43.000000 pygame_magics-0.3.0/pygame_magics/camera/__init__.py
--rw-r--r--   0 senya      (501) staff       (20)     2844 2024-04-24 17:35:59.000000 pygame_magics-0.3.0/pygame_magics/camera/camera.py
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:39:53.492380 pygame_magics-0.3.0/pygame_magics/entities/
--rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:05:40.000000 pygame_magics-0.3.0/pygame_magics/entities/__init__.py
--rw-r--r--   0 senya      (501) staff       (20)      869 2024-04-24 17:35:59.000000 pygame_magics-0.3.0/pygame_magics/entities/enemy.py
--rw-r--r--   0 senya      (501) staff       (20)      409 2024-04-24 17:35:59.000000 pygame_magics-0.3.0/pygame_magics/entities/experience_orb.py
--rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:05:53.000000 pygame_magics-0.3.0/pygame_magics/entities/player.py
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 17:39:53.491248 pygame_magics-0.3.0/pygame_magics.egg-info/
--rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 17:39:53.000000 pygame_magics-0.3.0/pygame_magics.egg-info/PKG-INFO
--rw-r--r--   0 senya      (501) staff       (20)      423 2024-04-24 17:39:53.000000 pygame_magics-0.3.0/pygame_magics.egg-info/SOURCES.txt
--rw-r--r--   0 senya      (501) staff       (20)        1 2024-04-24 17:39:53.000000 pygame_magics-0.3.0/pygame_magics.egg-info/dependency_links.txt
--rw-r--r--   0 senya      (501) staff       (20)        7 2024-04-24 17:39:53.000000 pygame_magics-0.3.0/pygame_magics.egg-info/requires.txt
--rw-r--r--   0 senya      (501) staff       (20)       14 2024-04-24 17:39:53.000000 pygame_magics-0.3.0/pygame_magics.egg-info/top_level.txt
--rw-r--r--   0 senya      (501) staff       (20)       38 2024-04-24 17:39:53.492911 pygame_magics-0.3.0/setup.cfg
--rw-r--r--   0 senya      (501) staff       (20)      879 2024-04-24 17:38:17.000000 pygame_magics-0.3.0/setup.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.544132 pygame_magics-0.4.0/
+-rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 18:44:21.543893 pygame_magics-0.4.0/PKG-INFO
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.541042 pygame_magics-0.4.0/pygame_magics/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:21:17.000000 pygame_magics-0.4.0/pygame_magics/__init__.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.541978 pygame_magics-0.4.0/pygame_magics/camera/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 16:50:43.000000 pygame_magics-0.4.0/pygame_magics/camera/__init__.py
+-rw-r--r--   0 senya      (501) staff       (20)     2795 2024-04-24 17:55:58.000000 pygame_magics-0.4.0/pygame_magics/camera/camera.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.543527 pygame_magics-0.4.0/pygame_magics/entities/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:05:40.000000 pygame_magics-0.4.0/pygame_magics/entities/__init__.py
+-rw-r--r--   0 senya      (501) staff       (20)      820 2024-04-24 17:55:59.000000 pygame_magics-0.4.0/pygame_magics/entities/enemy.py
+-rw-r--r--   0 senya      (501) staff       (20)      619 2024-04-24 18:42:39.000000 pygame_magics-0.4.0/pygame_magics/entities/experience_orb.py
+-rw-r--r--   0 senya      (501) staff       (20)     3212 2024-04-24 18:39:32.000000 pygame_magics-0.4.0/pygame_magics/entities/magic_bolt.py
+-rw-r--r--   0 senya      (501) staff       (20)     1992 2024-04-24 18:39:32.000000 pygame_magics-0.4.0/pygame_magics/entities/player.py
+-rw-r--r--   0 senya      (501) staff       (20)     2950 2024-04-24 18:44:00.000000 pygame_magics-0.4.0/pygame_magics/entities/setup_m.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.541721 pygame_magics-0.4.0/pygame_magics.egg-info/
+-rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/PKG-INFO
+-rw-r--r--   0 senya      (501) staff       (20)      494 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/SOURCES.txt
+-rw-r--r--   0 senya      (501) staff       (20)        1 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/dependency_links.txt
+-rw-r--r--   0 senya      (501) staff       (20)        7 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/requires.txt
+-rw-r--r--   0 senya      (501) staff       (20)       14 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/top_level.txt
+-rw-r--r--   0 senya      (501) staff       (20)       38 2024-04-24 18:44:21.544184 pygame_magics-0.4.0/setup.cfg
+-rw-r--r--   0 senya      (501) staff       (20)      879 2024-04-24 18:44:19.000000 pygame_magics-0.4.0/setup.py
```

### Comparing `pygame_magics-0.3.0/PKG-INFO` & `pygame_magics-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_magics
-Version: 0.3.0
+Version: 0.4.0
 Summary: Magic survival funcs
 Home-page: https://github.com/MCtop4ik/pygame-magics
 Author: MCtop4ik
 Author-email: senyaza@mail.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygame_magics-0.3.0/pygame_magics/camera/camera.py` & `pygame_magics-0.4.0/pygame_magics/camera/camera.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import pygame_magics
+import pygame
 
 
-class CameraGroup(pygame_magics.sprite.Group):
+class CameraGroup(pygame.sprite.Group):
 
     def __init__(self, map_x, map_y, field_img, size_coefficient=1):
         """
             https://github.com/clear-code-projects/Pygame-Cameras
             https://www.youtube.com/watch?v=u7LPRqrzry8
         """
         super().__init__()
-        self.display_surface = pygame_magics.display.get_surface()
+        self.display_surface = pygame.display.get_surface()
 
-        self.ground_surf = pygame_magics.image.load(field_img)
-        self.ground_surf = pygame_magics.transform.scale(self.ground_surf, (self.ground_surf.get_width() * size_coefficient,
-                                                                            self.ground_surf.get_height() * size_coefficient))
+        self.ground_surf = pygame.image.load(field_img)
+        self.ground_surf = pygame.transform.scale(self.ground_surf, (self.ground_surf.get_width() * size_coefficient,
+                                                                     self.ground_surf.get_height() * size_coefficient))
         self.ground_rect = self.ground_surf.get_rect(topleft=(-map_x, -map_y))
 
         self.map_x = map_x
         self.map_y = map_y
 
-        self.offset = pygame_magics.math.Vector2(800, 300)
+        self.offset = pygame.math.Vector2(800, 300)
         self.half_w = self.display_surface.get_size()[0] // 2
         self.half_h = self.display_surface.get_size()[1] // 2
 
     def center_target_camera(self, target):
         self.offset.x = target.rect.centerx - self.half_w
         self.offset.y = target.rect.centery - self.half_h
```

### Comparing `pygame_magics-0.3.0/pygame_magics.egg-info/PKG-INFO` & `pygame_magics-0.4.0/pygame_magics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-magics
-Version: 0.3.0
+Version: 0.4.0
 Summary: Magic survival funcs
 Home-page: https://github.com/MCtop4ik/pygame-magics
 Author: MCtop4ik
 Author-email: senyaza@mail.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygame_magics-0.3.0/setup.py` & `pygame_magics-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pygame_magics',
-    version='0.3.0',
+    version='0.4.0',
     author='MCtop4ik',
     author_email='senyaza@mail.ru',
     description='Magic survival funcs',
     long_description='Hyper grest library for magic survival',
     long_description_content_type='text/markdown',
     url='https://github.com/MCtop4ik/pygame-magics',
     packages=find_packages(),
```

