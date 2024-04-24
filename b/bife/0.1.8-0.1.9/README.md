# Comparing `tmp/bife-0.1.8.tar.gz` & `tmp/bife-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bife-0.1.8.tar", max compression
+gzip compressed data, was "bife-0.1.9.tar", max compression
```

## Comparing `bife-0.1.8.tar` & `bife-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       85 2024-04-22 02:45:19.055830 bife-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-22 02:39:49.833680 bife-0.1.8/bife/__init__.py
--rw-r--r--   0        0        0     2650 2024-04-22 15:40:11.399329 bife-0.1.8/bife/cli.py
--rw-r--r--   0        0        0      495 2024-04-22 12:09:18.233425 bife-0.1.8/bife/config.py
--rw-r--r--   0        0        0      279 2024-04-22 13:59:09.601032 bife-0.1.8/bife/structs/default/.env
--rw-r--r--   0        0        0     1600 2024-04-22 14:12:19.194773 bife-0.1.8/bife/structs/default/__pycache__/config.cpython-312.pyc
--rw-r--r--   0        0        0     3713 2024-04-22 15:44:51.110952 bife-0.1.8/bife/structs/default/__pycache__/run.cpython-312.pyc
--rw-r--r--   0        0        0      146 2024-04-22 14:04:03.061025 bife-0.1.8/bife/structs/default/app.py
--rw-r--r--   0        0        0      897 2024-04-22 14:11:09.854621 bife-0.1.8/bife/structs/default/config.py
--rw-r--r--   0        0        0      767 2024-04-22 13:46:10.333940 bife-0.1.8/bife/structs/default/general/controller.py
--rw-r--r--   0        0        0      460 2024-04-22 13:34:06.000656 bife-0.1.8/bife/structs/default/general/models.py
--rw-r--r--   0        0        0     1884 2024-04-22 13:35:30.117469 bife-0.1.8/bife/structs/default/general/repository.py
--rw-r--r--   0        0        0      133 2024-04-22 13:27:30.803393 bife-0.1.8/bife/structs/default/general/schemas.py
--rw-r--r--   0        0        0       36 2024-04-22 13:40:25.451966 bife-0.1.8/bife/structs/default/libs/api/__init__.py
--rw-r--r--   0        0        0      216 2024-04-22 13:40:25.453609 bife-0.1.8/bife/structs/default/libs/api/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2792 2024-04-22 13:40:25.454192 bife-0.1.8/bife/structs/default/libs/api/__pycache__/api_handler.cpython-312.pyc
--rw-r--r--   0        0        0      646 2024-04-22 13:42:15.501476 bife-0.1.8/bife/structs/default/libs/api/api_handler.py
--rw-r--r--   0        0        0     4278 2024-04-22 13:41:19.970294 bife-0.1.8/bife/structs/default/libs/bootstrap/__pycache__/bootstrap.cpython-312.pyc
--rw-r--r--   0        0        0     1940 2024-04-22 15:00:16.228757 bife-0.1.8/bife/structs/default/libs/bootstrap/bootstrap.py
--rw-r--r--   0        0        0       69 2024-04-22 13:35:29.966018 bife-0.1.8/bife/structs/default/libs/database/__init__.py
--rw-r--r--   0        0        0      194 2024-04-22 13:30:55.974437 bife-0.1.8/bife/structs/default/libs/database/base.py
--rw-r--r--   0        0        0      908 2024-04-22 14:54:26.813661 bife-0.1.8/bife/structs/default/libs/database/database_handler.py
--rw-r--r--   0        0        0       31 2024-04-22 13:41:47.115679 bife-0.1.8/bife/structs/default/libs/security/__init__.py
--rw-r--r--   0        0        0      216 2024-04-22 13:41:47.116983 bife-0.1.8/bife/structs/default/libs/security/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7767 2024-04-22 13:41:47.118527 bife-0.1.8/bife/structs/default/libs/security/__pycache__/security.cpython-312.pyc
--rw-r--r--   0        0        0     5151 2024-04-22 14:53:56.609218 bife-0.1.8/bife/structs/default/libs/security/security.py
--rw-r--r--   0        0        0      222 2024-04-22 14:04:14.559846 bife-0.1.8/bife/structs/default/main.py
--rw-r--r--   0        0        0     4582 2024-04-22 13:46:54.950456 bife-0.1.8/bife/structs/default/modules/user/__pycache__/controller.cpython-312.pyc
--rw-r--r--   0        0        0     1484 2024-04-22 13:46:54.950924 bife-0.1.8/bife/structs/default/modules/user/__pycache__/events.cpython-312.pyc
--rw-r--r--   0        0        0     1371 2024-04-22 13:46:54.951387 bife-0.1.8/bife/structs/default/modules/user/__pycache__/ext.cpython-312.pyc
--rw-r--r--   0        0        0     2516 2024-04-22 13:46:54.951793 bife-0.1.8/bife/structs/default/modules/user/__pycache__/models.cpython-312.pyc
--rw-r--r--   0        0        0     2832 2024-04-22 13:46:54.952346 bife-0.1.8/bife/structs/default/modules/user/__pycache__/repository.cpython-312.pyc
--rw-r--r--   0        0        0     1430 2024-04-22 13:46:54.952664 bife-0.1.8/bife/structs/default/modules/user/__pycache__/schemas.cpython-312.pyc
--rw-r--r--   0        0        0     5341 2024-04-22 13:46:54.953183 bife-0.1.8/bife/structs/default/modules/user/__pycache__/service.cpython-312.pyc
--rw-r--r--   0        0        0     4452 2024-04-22 13:46:54.953624 bife-0.1.8/bife/structs/default/modules/user/__pycache__/teste_controller.cpython-312.pyc
--rw-r--r--   0        0        0     2476 2024-04-22 13:52:14.991526 bife-0.1.8/bife/structs/default/modules/user/controller.py
--rw-r--r--   0        0        0      459 2024-04-22 13:48:43.595303 bife-0.1.8/bife/structs/default/modules/user/events.py
--rw-r--r--   0        0        0      369 2024-04-22 13:46:54.954576 bife-0.1.8/bife/structs/default/modules/user/ext.py
--rw-r--r--   0        0        0     1298 2024-04-22 13:46:54.954815 bife-0.1.8/bife/structs/default/modules/user/models.py
--rw-r--r--   0        0        0     1508 2024-04-22 13:46:54.955086 bife-0.1.8/bife/structs/default/modules/user/repository.py
--rw-r--r--   0        0        0      650 2024-04-22 13:46:54.955451 bife-0.1.8/bife/structs/default/modules/user/schemas.py
--rw-r--r--   0        0        0     2603 2024-04-22 13:50:58.022496 bife-0.1.8/bife/structs/default/modules/user/service.py
--rw-r--r--   0        0        0     1754 2024-04-22 15:45:12.344313 bife-0.1.8/bife/structs/default/run.py
--rw-r--r--   0        0        0       43 2024-04-22 14:54:48.702085 bife-0.1.8/bife/structs/default/utils/__init__.py
--rw-r--r--   0        0        0      184 2024-04-22 13:52:03.374193 bife-0.1.8/bife/structs/default/utils/email_validator.py
--rw-r--r--   0        0        0      808 2024-04-22 15:45:16.992222 bife-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 bife-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       85 2024-04-22 02:45:19.055830 bife-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 02:39:49.833680 bife-0.1.9/bife/__init__.py
+-rw-r--r--   0        0        0     2638 2024-04-22 16:22:06.825672 bife-0.1.9/bife/cli.py
+-rw-r--r--   0        0        0      495 2024-04-22 12:09:18.233425 bife-0.1.9/bife/config.py
+-rw-r--r--   0        0        0      279 2024-04-22 13:59:09.601032 bife-0.1.9/bife/structs/default/.env
+-rw-r--r--   0        0        0     1600 2024-04-22 14:12:19.194773 bife-0.1.9/bife/structs/default/__pycache__/config.cpython-312.pyc
+-rw-r--r--   0        0        0     3713 2024-04-22 15:44:51.110952 bife-0.1.9/bife/structs/default/__pycache__/run.cpython-312.pyc
+-rw-r--r--   0        0        0      146 2024-04-22 14:04:03.061025 bife-0.1.9/bife/structs/default/app.py
+-rw-r--r--   0        0        0      897 2024-04-22 14:11:09.854621 bife-0.1.9/bife/structs/default/config.py
+-rw-r--r--   0        0        0      767 2024-04-22 13:46:10.333940 bife-0.1.9/bife/structs/default/general/controller.py
+-rw-r--r--   0        0        0      460 2024-04-22 13:34:06.000656 bife-0.1.9/bife/structs/default/general/models.py
+-rw-r--r--   0        0        0     1884 2024-04-22 13:35:30.117469 bife-0.1.9/bife/structs/default/general/repository.py
+-rw-r--r--   0        0        0      133 2024-04-22 13:27:30.803393 bife-0.1.9/bife/structs/default/general/schemas.py
+-rw-r--r--   0        0        0       36 2024-04-22 13:40:25.451966 bife-0.1.9/bife/structs/default/libs/api/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-22 13:40:25.453609 bife-0.1.9/bife/structs/default/libs/api/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     2792 2024-04-22 13:40:25.454192 bife-0.1.9/bife/structs/default/libs/api/__pycache__/api_handler.cpython-312.pyc
+-rw-r--r--   0        0        0      646 2024-04-22 13:42:15.501476 bife-0.1.9/bife/structs/default/libs/api/api_handler.py
+-rw-r--r--   0        0        0     4278 2024-04-22 13:41:19.970294 bife-0.1.9/bife/structs/default/libs/bootstrap/__pycache__/bootstrap.cpython-312.pyc
+-rw-r--r--   0        0        0     1960 2024-04-22 16:22:06.841956 bife-0.1.9/bife/structs/default/libs/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0       69 2024-04-22 13:35:29.966018 bife-0.1.9/bife/structs/default/libs/database/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-22 13:30:55.974437 bife-0.1.9/bife/structs/default/libs/database/base.py
+-rw-r--r--   0        0        0      930 2024-04-22 16:22:06.688479 bife-0.1.9/bife/structs/default/libs/database/database_handler.py
+-rw-r--r--   0        0        0       31 2024-04-22 13:41:47.115679 bife-0.1.9/bife/structs/default/libs/security/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-22 13:41:47.116983 bife-0.1.9/bife/structs/default/libs/security/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7767 2024-04-22 13:41:47.118527 bife-0.1.9/bife/structs/default/libs/security/__pycache__/security.cpython-312.pyc
+-rw-r--r--   0        0        0     5151 2024-04-22 14:53:56.609218 bife-0.1.9/bife/structs/default/libs/security/security.py
+-rw-r--r--   0        0        0      222 2024-04-22 14:04:14.559846 bife-0.1.9/bife/structs/default/main.py
+-rw-r--r--   0        0        0     4582 2024-04-22 13:46:54.950456 bife-0.1.9/bife/structs/default/modules/user/__pycache__/controller.cpython-312.pyc
+-rw-r--r--   0        0        0     1484 2024-04-22 13:46:54.950924 bife-0.1.9/bife/structs/default/modules/user/__pycache__/events.cpython-312.pyc
+-rw-r--r--   0        0        0     1371 2024-04-22 13:46:54.951387 bife-0.1.9/bife/structs/default/modules/user/__pycache__/ext.cpython-312.pyc
+-rw-r--r--   0        0        0     2516 2024-04-22 13:46:54.951793 bife-0.1.9/bife/structs/default/modules/user/__pycache__/models.cpython-312.pyc
+-rw-r--r--   0        0        0     2832 2024-04-22 13:46:54.952346 bife-0.1.9/bife/structs/default/modules/user/__pycache__/repository.cpython-312.pyc
+-rw-r--r--   0        0        0     1430 2024-04-22 13:46:54.952664 bife-0.1.9/bife/structs/default/modules/user/__pycache__/schemas.cpython-312.pyc
+-rw-r--r--   0        0        0     5341 2024-04-22 13:46:54.953183 bife-0.1.9/bife/structs/default/modules/user/__pycache__/service.cpython-312.pyc
+-rw-r--r--   0        0        0     4452 2024-04-22 13:46:54.953624 bife-0.1.9/bife/structs/default/modules/user/__pycache__/teste_controller.cpython-312.pyc
+-rw-r--r--   0        0        0     2213 2024-04-22 16:22:22.462832 bife-0.1.9/bife/structs/default/modules/user/controller.py
+-rw-r--r--   0        0        0      459 2024-04-22 13:48:43.595303 bife-0.1.9/bife/structs/default/modules/user/events.py
+-rw-r--r--   0        0        0      369 2024-04-22 13:46:54.954576 bife-0.1.9/bife/structs/default/modules/user/ext.py
+-rw-r--r--   0        0        0     1298 2024-04-22 13:46:54.954815 bife-0.1.9/bife/structs/default/modules/user/models.py
+-rw-r--r--   0        0        0     1508 2024-04-22 13:46:54.955086 bife-0.1.9/bife/structs/default/modules/user/repository.py
+-rw-r--r--   0        0        0      650 2024-04-22 13:46:54.955451 bife-0.1.9/bife/structs/default/modules/user/schemas.py
+-rw-r--r--   0        0        0     2603 2024-04-22 13:50:58.022496 bife-0.1.9/bife/structs/default/modules/user/service.py
+-rw-r--r--   0        0        0     1950 2024-04-22 16:22:06.711167 bife-0.1.9/bife/structs/default/run.py
+-rw-r--r--   0        0        0       44 2024-04-22 16:22:06.679237 bife-0.1.9/bife/structs/default/utils/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-22 13:52:03.374193 bife-0.1.9/bife/structs/default/utils/email_validator.py
+-rw-r--r--   0        0        0      808 2024-04-22 16:22:31.085637 bife-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 bife-0.1.9/PKG-INFO
```

### Comparing `bife-0.1.8/bife/cli.py` & `bife-0.1.9/bife/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
 from pick import pick
 
 from .config import DatabaseConfig, ModuleConfig, UserConfig
-from .structs.default.run import run, new_module
+from .structs.default.run import new_module, run
 
 
 class BifeCreateProject:
     def run(self):
         if len(sys.argv) == 1:
             print('Please, tell me the name of your project!')
             sys.exit(1)
@@ -80,8 +80,7 @@
                 bife = BifeCreateProject()
                 bife.run()
             else:
                 print('Error, tell a application name')
                 sys.exit(1)
         elif sys.argv[2] == 'module':
             new_module(sys.argv[3])
-
```

### Comparing `bife-0.1.8/bife/structs/default/__pycache__/config.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/__pycache__/config.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/__pycache__/run.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/__pycache__/run.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/config.py` & `bife-0.1.9/bife/structs/default/config.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/general/controller.py` & `bife-0.1.9/bife/structs/default/general/controller.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/general/repository.py` & `bife-0.1.9/bife/structs/default/general/repository.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/libs/api/__pycache__/api_handler.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/libs/api/__pycache__/api_handler.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/libs/api/api_handler.py` & `bife-0.1.9/bife/structs/default/libs/api/api_handler.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/libs/bootstrap/__pycache__/bootstrap.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/libs/bootstrap/__pycache__/bootstrap.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/libs/bootstrap/bootstrap.py` & `bife-0.1.9/bife/structs/default/libs/bootstrap/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import importlib
 import os
 from typing import Optional
 
-from fastapi import APIRouter
-
 from config import get_config
+from fastapi import APIRouter
 from fastapi.routing import Mount
 from fastapi.staticfiles import StaticFiles
 from libs.api.api_handler import ApiHandler
 
 config = get_config()
 
 
 class Bootstrap:
     def __init__(self) -> None:
         self.controllers = []
-        self.current_path: str = os.path.join(os.path.relpath(os.path.join(os.getcwd())), '${project_name}')
+        self.current_path: str = os.path.join(
+            os.path.relpath(os.path.join(os.getcwd())), '${project_name}'
+        )
         path = self.get_project_path()
         modules_path = self.get_module_path(path)
         for root, _, files in os.walk(modules_path):
             for file in files:
                 if 'controller' in file.lower() and file.endswith('.py'):
                     module_path = (
                         root.replace('/', '.')[2:]
@@ -50,8 +51,7 @@
             ):
                 continue
             return root
 
     def setup_fastapi_app(self, app: ApiHandler):
         for controller in self.controllers:
             app.add_router(controller)
-
```

### Comparing `bife-0.1.8/bife/structs/default/libs/database/database_handler.py` & `bife-0.1.9/bife/structs/default/libs/database/database_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 class DatabaseHandler:
 
     instance: Optional['DatabaseHandler'] = None
     config = get_config()
 
     def __init__(self) -> None:
-        self._engine = create_engine(self.config.DATABASE_CONNECTION, max_overflow=-1)
+        self._engine = create_engine(
+            self.config.DATABASE_CONNECTION, max_overflow=-1
+        )
         self.session_manger = sessionmaker(self._engine)
 
     def __new__(cls: Type['DatabaseHandler']) -> 'DatabaseHandler':
         if cls.instance is None:
             cls.instance = super(DatabaseHandler, cls).__new__(cls)
         return cls.instance
```

### Comparing `bife-0.1.8/bife/structs/default/libs/security/__pycache__/security.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/libs/security/__pycache__/security.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/libs/security/security.py` & `bife-0.1.9/bife/structs/default/libs/security/security.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/__pycache__/controller.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/modules/user/__pycache__/controller.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/__pycache__/events.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/modules/user/__pycache__/events.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/__pycache__/ext.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/modules/user/__pycache__/ext.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/__pycache__/models.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/modules/user/__pycache__/models.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/__pycache__/repository.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/modules/user/__pycache__/repository.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/__pycache__/schemas.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/modules/user/__pycache__/schemas.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/__pycache__/service.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/modules/user/__pycache__/service.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/__pycache__/teste_controller.cpython-312.pyc` & `bife-0.1.9/bife/structs/default/modules/user/__pycache__/teste_controller.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/controller.py` & `bife-0.1.9/bife/structs/default/modules/user/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,57 +16,52 @@
 from .repository import UserRepository
 from .schemas import LoginUserRequest, RegisterUserRequest, UserAuthResponse
 from .service import UserService
 
 router: APIRouter = APIRouter(tags=['user'], prefix='/user')
 security: Security = Security()
 
-
-class UserController:
-
-    repository: UserRepository = UserRepository()
-    service: UserService = UserService()
-    events: UserEvents = UserEvents()
-
-    @router.post('/login', response_model=UserAuthResponse)
-    def user_login(self, data: LoginUserRequest, response: Response):
-        try:
-            user = self.repository.login_user(data)
-        except UserNotFound as e:
-            raise HTTPException(status.HTTP_404_NOT_FOUND, e.args[0])
-        except (InvalidPassword, InvalidUserLogin) as e:
-            raise HTTPException(status.HTTP_400_BAD_REQUEST, e.args[0])
-
-        tokens = self.service.generate_access_token(user.uuid)
-        response.set_cookie('access_token', tokens['access_token'])
-        response.set_cookie(
-            'refresh_access_token', tokens['refresh_access_token']
-        )
-        return UserAuthResponse(**tokens)
-
-    @router.post('/register', response_model=UserAuthResponse)
-    def register_user(self, data: RegisterUserRequest, response: Response):
-        try:
-            user = self.repository.register_user(data)
-        except (
-            InvalidUsername,
-            InvalidEmail,
-            InvalidGender,
-            InvalidName,
-            InvalidPassword,
-        ) as e:
-            raise HTTPException(status.HTTP_400_BAD_REQUEST, e.args[0])
-        except UserAlreadyExists as e:
-            raise HTTPException(status.HTTP_409_CONFLICT, e.args[0])
-        tokens = self.service.generate_access_token(user.uuid)
-        response.set_cookie('access_token', tokens['access_token'])
-        response.set_cookie(
-            'refresh_access_token', tokens['refresh_access_token']
-        )
-        return UserAuthResponse(**tokens)
-
-    @router.get('/me')
-    def get_about_user(
-        self,
-        current_user: UserModel = Depends(security.get_current_user),
-    ):
-        return current_user.__dict__
+repository: UserRepository = UserRepository()
+service: UserService = UserService()
+events: UserEvents = UserEvents()
+
+
+@router.post('/login', response_model=UserAuthResponse)
+def user_login(data: LoginUserRequest, response: Response):
+    try:
+        user = repository.login_user(data)
+    except UserNotFound as e:
+        raise HTTPException(status.HTTP_404_NOT_FOUND, e.args[0])
+    except (InvalidPassword, InvalidUserLogin) as e:
+        raise HTTPException(status.HTTP_400_BAD_REQUEST, e.args[0])
+
+    tokens = service.generate_access_token(user.uuid)
+    response.set_cookie('access_token', tokens['access_token'])
+    response.set_cookie('refresh_access_token', tokens['refresh_access_token'])
+    return UserAuthResponse(**tokens)
+
+
+@router.post('/register', response_model=UserAuthResponse)
+def register_user(data: RegisterUserRequest, response: Response):
+    try:
+        user = repository.register_user(data)
+    except (
+        InvalidUsername,
+        InvalidEmail,
+        InvalidGender,
+        InvalidName,
+        InvalidPassword,
+    ) as e:
+        raise HTTPException(status.HTTP_400_BAD_REQUEST, e.args[0])
+    except UserAlreadyExists as e:
+        raise HTTPException(status.HTTP_409_CONFLICT, e.args[0])
+    tokens = service.generate_access_token(user.uuid)
+    response.set_cookie('access_token', tokens['access_token'])
+    response.set_cookie('refresh_access_token', tokens['refresh_access_token'])
+    return UserAuthResponse(**tokens)
+
+
+@router.get('/me')
+def get_about_user(
+    current_user: UserModel = Depends(security.get_current_user),
+):
+    return current_user.__dict__
```

### Comparing `bife-0.1.8/bife/structs/default/modules/user/models.py` & `bife-0.1.9/bife/structs/default/modules/user/models.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/repository.py` & `bife-0.1.9/bife/structs/default/modules/user/repository.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/schemas.py` & `bife-0.1.9/bife/structs/default/modules/user/schemas.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/modules/user/service.py` & `bife-0.1.9/bife/structs/default/modules/user/service.py`

 * *Files identical despite different names*

### Comparing `bife-0.1.8/bife/structs/default/run.py` & `bife-0.1.9/bife/structs/default/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,63 @@
 import pathlib
 import shutil
 
 from mako.template import Template
 
 from ...config import DatabaseConfig, ModuleConfig, UserConfig
 
+
 def run(
     project_name: str,
     module_config: ModuleConfig,
     user_config: UserConfig,
     database_config: DatabaseConfig,
 ):
     current_dir = os.path.dirname(__file__)
-    shutil.copytree(os.path.join(current_dir, 'libs/'), os.path.join(project_name, 'libs'))
-    template = Template(open(os.path.join(current_dir, 'libs', 'bootstrap', 'bootstrap.py')).read())
+    shutil.copytree(
+        os.path.join(current_dir, 'libs/'), os.path.join(project_name, 'libs')
+    )
+    template = Template(
+        open(
+            os.path.join(current_dir, 'libs', 'bootstrap', 'bootstrap.py')
+        ).read()
+    )
     boostrap_content = template.render(project_name=project_name)
-    with open(os.path.join(project_name, 'libs', 'bootstrap', 'bootstrap.py'), 'w') as file:
+    with open(
+        os.path.join(project_name, 'libs', 'bootstrap', 'bootstrap.py'), 'w'
+    ) as file:
         file.write(boostrap_content)
-    shutil.copytree(os.path.join(current_dir, 'utils/'), os.path.join(project_name, 'utils'))
+    shutil.copytree(
+        os.path.join(current_dir, 'utils/'),
+        os.path.join(project_name, 'utils'),
+    )
     os.makedirs(os.path.join(project_name, module_config.module_path))
-    shutil.copytree(os.path.join(current_dir, 'modules/user/'), os.path.join(project_name, module_config.module_path, 'user'))
-    shutil.copy(os.path.join(current_dir, 'config.py'), os.path.join(project_name, 'config.py'))
-    shutil.copy(os.path.join(current_dir, 'main.py'), os.path.join(project_name, 'main.py'))
-    shutil.copy(os.path.join(current_dir, 'app.py'), os.path.join(project_name, 'app.py'))
+    shutil.copytree(
+        os.path.join(current_dir, 'modules/user/'),
+        os.path.join(project_name, module_config.module_path, 'user'),
+    )
+    shutil.copy(
+        os.path.join(current_dir, 'config.py'),
+        os.path.join(project_name, 'config.py'),
+    )
+    shutil.copy(
+        os.path.join(current_dir, 'main.py'),
+        os.path.join(project_name, 'main.py'),
+    )
+    shutil.copy(
+        os.path.join(current_dir, 'app.py'),
+        os.path.join(project_name, 'app.py'),
+    )
     if not os.path.isfile(os.path.join(current_dir, '.env')):
         with open('.env', 'w') as file:
             file.write('')
     with open('.env', 'a') as file:
         template = Template(open(os.path.join(current_dir, '.env')).read())
         content = template.render(project_name=project_name)
         file.write(f'\n{content}')
-    print(f'Please, install the packages: fastapi pyjwt argon2-cffi sqlalchemy python-dotenv')
+    print(
+        f'Please, install the packages: fastapi pyjwt argon2-cffi sqlalchemy python-dotenv'
+    )
+
 
 def new_module(module_name: str):
-    ...
+    ...
```

