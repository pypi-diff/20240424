# Comparing `tmp/pynest_api-0.2.1.tar.gz` & `tmp/pynest_api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynest_api-0.2.1.tar", last modified: Mon Apr 15 12:04:19 2024, max compression
+gzip compressed data, was "pynest_api-0.2.2.tar", last modified: Wed Apr 24 08:19:33 2024, max compression
```

## Comparing `pynest_api-0.2.1.tar` & `pynest_api-0.2.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.467748 pynest_api-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-15 12:03:50.000000 pynest_api-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-15 12:04:19.467748 pynest_api-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-15 12:03:50.000000 pynest_api-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.455748 pynest_api-0.2.1/nest/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.455748 pynest_api-0.2.1/nest/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/cli/click_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.455748 pynest_api-0.2.1/nest/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/route_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.459748 pynest_api-0.2.1/nest/common/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/base_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/blank_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/mongo_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/mysql_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/orm_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/postgres_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/sqlite_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/common/templates/templates_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.459748 pynest_api-0.2.1/nest/core/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.459748 pynest_api-0.2.1/nest/core/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/database/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/database/odm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/database/odm_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/database/orm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/database/orm_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.463748 pynest_api-0.2.1/nest/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/class_based_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/http_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/injectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/decorators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/pynest_app_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/pynest_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/pynest_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/core/pynest_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.463748 pynest_api-0.2.1/nest/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.463748 pynest_api-0.2.1/nest/plugins/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.463748 pynest_api-0.2.1/nest/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.463748 pynest_api-0.2.1/nest/plugins/modules/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/modules/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.463748 pynest_api-0.2.1/nest/plugins/modules/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/modules/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/modules/redis/redis_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/modules/redis/redis_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/modules/redis/redis_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/modules/redis/redis_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.463748 pynest_api-0.2.1/nest/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:03:50.000000 pynest_api-0.2.1/nest/plugins/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:04:19.463748 pynest_api-0.2.1/pynest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-15 12:04:19.000000 pynest_api-0.2.1/pynest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-15 12:04:19.000000 pynest_api-0.2.1/pynest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:04:19.000000 pynest_api-0.2.1/pynest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 12:04:19.000000 pynest_api-0.2.1/pynest_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 12:04:19.000000 pynest_api-0.2.1/pynest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 12:04:19.000000 pynest_api-0.2.1/pynest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-15 12:03:50.000000 pynest_api-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:04:19.467748 pynest_api-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.427373 pynest_api-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 08:18:56.000000 pynest_api-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-24 08:19:33.427373 pynest_api-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-24 08:18:56.000000 pynest_api-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.415373 pynest_api-0.2.2/nest/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.415373 pynest_api-0.2.2/nest/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/cli/click_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.419373 pynest_api-0.2.2/nest/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/route_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.419373 pynest_api-0.2.2/nest/common/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/blank_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/mongo_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/mysql_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/orm_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/postgres_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/sqlite_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/templates_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.419373 pynest_api-0.2.2/nest/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.419373 pynest_api-0.2.2/nest/core/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/odm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/odm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/orm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/orm_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/class_based_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/injectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/pynest_app_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/pynest_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/pynest_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/pynest_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/modules/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/modules/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/redis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/redis_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/redis_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/redis_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/pynest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-24 08:18:56.000000 pynest_api-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:19:33.427373 pynest_api-0.2.2/setup.cfg
```

### Comparing `pynest_api-0.2.1/LICENSE` & `pynest_api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/PKG-INFO` & `pynest_api-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynest-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyNest is a FastAPI Abstraction for building microservices, influenced by NestJS.
 Author-email: Itay Dar <itay2803@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 PyNest
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 Requires-Dist: click>=8.1.6
 Requires-Dist: fastapi<1.0.0,>=0.88.0
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: uvicorn>=0.23.1
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: astor>=0.8.1
 Requires-Dist: black>=23.11.0
-Requires-Dist: injector>=0.21.0
+Requires-Dist: injector>=0.20.1
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: sqlalchemy==2.0.19
 Requires-Dist: alembic==1.7.4
 Provides-Extra: test
 Requires-Dist: pytest==6.2.5; extra == "test"
 Provides-Extra: orm
 Requires-Dist: sqlalchemy==2.0.19; extra == "orm"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynest-api Version: 0.2.1 Summary: PyNest is a
+Metadata-Version: 2.1 Name: pynest-api Version: 0.2.2 Summary: PyNest is a
 FastAPI Abstraction for building microservices, influenced by NestJS. Author-
 email: Itay Dar
 gmail.com> License: MIT License Copyright (c) 2023 PyNest Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -21,15 +21,15 @@
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8.1 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: click>=8.1.6 Requires-Dist: fastapi<1.0.0,>=0.88.0
 Requires-Dist: python-dotenv>=1.0.0 Requires-Dist: uvicorn>=0.23.1 Requires-
 Dist: PyYAML>=6.0.1 Requires-Dist: astor>=0.8.1 Requires-Dist: black>=23.11.0
-Requires-Dist: injector>=0.21.0 Requires-Dist: pydantic<2.0.0 Requires-Dist:
+Requires-Dist: injector>=0.20.1 Requires-Dist: pydantic<2.0.0 Requires-Dist:
 sqlalchemy==2.0.19 Requires-Dist: alembic==1.7.4 Provides-Extra: test Requires-
 Dist: pytest==6.2.5; extra == "test" Provides-Extra: orm Requires-Dist:
 sqlalchemy==2.0.19; extra == "orm" Requires-Dist: alembic==1.7.4; extra ==
 "orm" Provides-Extra: mongo Requires-Dist: pymongo==3.12.0; extra == "mongo"
 Requires-Dist: motor==3.2.0; extra == "mongo" Requires-Dist: beanie==1.20.0;
 extra == "mongo"
                           [docs/imgs/pynest-logo.png]
```

### Comparing `pynest_api-0.2.1/README.md` & `pynest_api-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/cli/cli.py` & `pynest_api-0.2.2/nest/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/cli/click_handlers.py` & `pynest_api-0.2.2/nest/cli/click_handlers.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/module.py` & `pynest_api-0.2.2/nest/common/module.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/route_resolver.py` & `pynest_api-0.2.2/nest/common/route_resolver.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/templates/base_template.py` & `pynest_api-0.2.2/nest/common/templates/base_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/templates/blank_template.py` & `pynest_api-0.2.2/nest/common/templates/blank_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/templates/mongo_template.py` & `pynest_api-0.2.2/nest/common/templates/mongo_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/templates/mysql_template.py` & `pynest_api-0.2.2/nest/common/templates/mysql_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/templates/orm_template.py` & `pynest_api-0.2.2/nest/common/templates/orm_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/templates/postgres_template.py` & `pynest_api-0.2.2/nest/common/templates/postgres_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/templates/sqlite_template.py` & `pynest_api-0.2.2/nest/common/templates/sqlite_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/common/templates/templates_factory.py` & `pynest_api-0.2.2/nest/common/templates/templates_factory.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/database/base_config.py` & `pynest_api-0.2.2/nest/core/database/base_config.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/database/odm_config.py` & `pynest_api-0.2.2/nest/core/database/odm_config.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/database/odm_provider.py` & `pynest_api-0.2.2/nest/core/database/odm_provider.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/database/orm_config.py` & `pynest_api-0.2.2/nest/core/database/orm_config.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/database/orm_provider.py` & `pynest_api-0.2.2/nest/core/database/orm_provider.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/decorators/class_based_view.py` & `pynest_api-0.2.2/nest/core/decorators/class_based_view.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/decorators/controller.py` & `pynest_api-0.2.2/nest/core/decorators/controller.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/decorators/database.py` & `pynest_api-0.2.2/nest/core/decorators/database.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/decorators/http_method.py` & `pynest_api-0.2.2/nest/core/decorators/http_method.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/decorators/http_methods.py` & `pynest_api-0.2.2/nest/core/decorators/http_methods.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/decorators/injectable.py` & `pynest_api-0.2.2/nest/core/decorators/injectable.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/decorators/module.py` & `pynest_api-0.2.2/nest/core/decorators/module.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/decorators/utils.py` & `pynest_api-0.2.2/nest/core/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/pynest_app_context.py` & `pynest_api-0.2.2/nest/core/pynest_app_context.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/pynest_application.py` & `pynest_api-0.2.2/nest/core/pynest_application.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/pynest_container.py` & `pynest_api-0.2.2/nest/core/pynest_container.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/core/pynest_factory.py` & `pynest_api-0.2.2/nest/core/pynest_factory.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/plugins/modules/redis/redis_controller.py` & `pynest_api-0.2.2/nest/plugins/modules/redis/redis_controller.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/nest/plugins/modules/redis/redis_service.py` & `pynest_api-0.2.2/nest/plugins/modules/redis/redis_service.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/pynest_api.egg-info/PKG-INFO` & `pynest_api-0.2.2/pynest_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynest-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: PyNest is a FastAPI Abstraction for building microservices, influenced by NestJS.
 Author-email: Itay Dar <itay2803@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 PyNest
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 Requires-Dist: click>=8.1.6
 Requires-Dist: fastapi<1.0.0,>=0.88.0
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: uvicorn>=0.23.1
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: astor>=0.8.1
 Requires-Dist: black>=23.11.0
-Requires-Dist: injector>=0.21.0
+Requires-Dist: injector>=0.20.1
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: sqlalchemy==2.0.19
 Requires-Dist: alembic==1.7.4
 Provides-Extra: test
 Requires-Dist: pytest==6.2.5; extra == "test"
 Provides-Extra: orm
 Requires-Dist: sqlalchemy==2.0.19; extra == "orm"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynest-api Version: 0.2.1 Summary: PyNest is a
+Metadata-Version: 2.1 Name: pynest-api Version: 0.2.2 Summary: PyNest is a
 FastAPI Abstraction for building microservices, influenced by NestJS. Author-
 email: Itay Dar
 gmail.com> License: MIT License Copyright (c) 2023 PyNest Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -21,15 +21,15 @@
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8.1 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: click>=8.1.6 Requires-Dist: fastapi<1.0.0,>=0.88.0
 Requires-Dist: python-dotenv>=1.0.0 Requires-Dist: uvicorn>=0.23.1 Requires-
 Dist: PyYAML>=6.0.1 Requires-Dist: astor>=0.8.1 Requires-Dist: black>=23.11.0
-Requires-Dist: injector>=0.21.0 Requires-Dist: pydantic<2.0.0 Requires-Dist:
+Requires-Dist: injector>=0.20.1 Requires-Dist: pydantic<2.0.0 Requires-Dist:
 sqlalchemy==2.0.19 Requires-Dist: alembic==1.7.4 Provides-Extra: test Requires-
 Dist: pytest==6.2.5; extra == "test" Provides-Extra: orm Requires-Dist:
 sqlalchemy==2.0.19; extra == "orm" Requires-Dist: alembic==1.7.4; extra ==
 "orm" Provides-Extra: mongo Requires-Dist: pymongo==3.12.0; extra == "mongo"
 Requires-Dist: motor==3.2.0; extra == "mongo" Requires-Dist: beanie==1.20.0;
 extra == "mongo"
                           [docs/imgs/pynest-logo.png]
```

### Comparing `pynest_api-0.2.1/pynest_api.egg-info/SOURCES.txt` & `pynest_api-0.2.2/pynest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.1/pyproject.toml` & `pynest_api-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "click>=8.1.6",
     "fastapi>=0.88.0,<1.0.0",
     "python-dotenv>=1.0.0",
     "uvicorn>=0.23.1",
     "PyYAML>=6.0.1",
     "astor>=0.8.1",
     "black>=23.11.0",
-    "injector>=0.21.0",
+    "injector>=0.20.1",
     "pydantic<2.0.0",
     "sqlalchemy == 2.0.19",
     "alembic == 1.7.4",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "nest.__init__.__version__" }
```

