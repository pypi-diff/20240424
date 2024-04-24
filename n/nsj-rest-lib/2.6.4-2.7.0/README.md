# Comparing `tmp/nsj_rest_lib-2.6.4.tar.gz` & `tmp/nsj_rest_lib-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-2.6.4.tar", last modified: Thu Apr 18 14:26:57 2024, max compression
+gzip compressed data, was "nsj_rest_lib-2.7.0.tar", last modified: Wed Apr 24 19:51:17 2024, max compression
```

## Comparing `nsj_rest_lib-2.6.4.tar` & `nsj_rest_lib-2.7.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4082 2024-03-19 17:07:11.000000 nsj_rest_lib-2.6.4/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      914 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/constants.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4408 2023-08-20 19:12:24.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5436 2024-02-05 21:10:11.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4841 2023-09-27 21:20:22.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4849 2024-03-04 22:24:04.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4902 2023-09-27 21:20:22.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    35092 2024-03-04 17:45:18.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1419 2023-10-05 17:46:49.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.365512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10906 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/dto.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2055 2023-08-26 23:46:06.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/entity.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/conjunto_type.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10094 2024-02-05 19:44:51.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4605 2024-03-04 22:21:11.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_left_join_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6071 2023-12-28 20:47:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7331 2024-03-05 22:27:27.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_sql_join_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      144 2023-10-06 22:45:32.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/after_insert_update_data.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    16234 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1785 2023-08-26 23:46:06.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      396 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      841 2023-09-15 22:16:41.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    55849 2024-04-18 14:26:34.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      845 2024-03-06 20:26:30.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-10-23 23:15:21.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      362 2024-02-29 18:49:26.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/join_aux.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     6826 2023-12-13 16:07:49.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/type_validator_util.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/validate_data.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      367 2023-12-28 20:47:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib/wsgi.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-18 14:26:57.369512 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/
--rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2063 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      138 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2024-04-18 14:26:57.000000 nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4082 2024-03-19 17:07:11.000000 nsj_rest_lib-2.7.0/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      914 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.672138 nsj_rest_lib-2.7.0/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.672138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/constants.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4408 2023-08-20 19:12:24.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5436 2024-02-05 21:10:11.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4841 2023-09-27 21:20:22.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4849 2024-03-04 22:24:04.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4902 2023-09-27 21:20:22.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    35092 2024-03-04 17:45:18.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1419 2023-10-05 17:46:49.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    13776 2024-04-24 19:50:59.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/decorator/dto.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2055 2023-08-26 23:46:06.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/decorator/entity.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/conjunto_type.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10094 2024-02-05 19:44:51.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4605 2024-03-04 22:21:11.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_left_join_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6071 2023-12-28 20:47:57.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3325 2024-04-24 19:50:59.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_object_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7331 2024-03-05 22:27:27.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_sql_join_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      144 2023-10-06 22:45:32.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/dto/after_insert_update_data.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    16734 2024-04-24 19:50:59.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1785 2023-08-26 23:46:06.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      396 2024-02-29 18:49:26.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      841 2023-09-15 22:16:41.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    55849 2024-04-18 14:26:34.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      845 2024-03-06 20:26:30.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/util/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-10-23 23:15:21.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/util/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      362 2024-02-29 18:49:26.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/util/join_aux.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     6826 2023-12-13 16:07:49.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/util/type_validator_util.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/validator/validate_data.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      367 2023-12-28 20:47:57.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib/wsgi.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2024-04-24 19:51:17.676138 nsj_rest_lib-2.7.0/src/nsj_rest_lib.egg-info/
+-rw-r--r--   0 sergio    (1000) sergio    (1000)     4938 2024-04-24 19:51:17.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2111 2024-04-24 19:51:17.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2024-04-24 19:51:17.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      138 2024-04-24 19:51:17.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2024-04-24 19:51:17.000000 nsj_rest_lib-2.7.0/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-2.6.4/PKG-INFO` & `nsj_rest_lib-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 2.6.4
+Version: 2.7.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-2.6.4/README.md` & `nsj_rest_lib-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/setup.cfg` & `nsj_rest_lib-2.7.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 2.6.4
+version = 2.7.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/patch_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/dao/dao_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/decorator/dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,274 +1,310 @@
+import functools
 from typing import Any, Dict
 
 from nsj_rest_lib.descriptor.conjunto_type import ConjuntoType
 from nsj_rest_lib.descriptor.dto_field import DTOField
 from nsj_rest_lib.descriptor.dto_list_field import DTOListField
 from nsj_rest_lib.descriptor.dto_left_join_field import DTOLeftJoinField, LeftJoinQuery
+from nsj_rest_lib.descriptor.dto_object_field import DTOObjectField
 from nsj_rest_lib.descriptor.dto_sql_join_field import DTOSQLJoinField, SQLJoinQuery
 
 
-class DTO:
-    def __init__(
-        self,
-        fixed_filters: Dict[str, Any] = None,
-        conjunto_type: ConjuntoType = None,
-        conjunto_field: str = None,
-        filter_aliases: Dict[str, Any] = None,
-    ) -> None:
-        super().__init__()
-
-        self._fixed_filters = fixed_filters
-        self._conjunto_type = conjunto_type
-        self._conjunto_field = conjunto_field
-        self._filter_aliases = filter_aliases
-
-        if (self._conjunto_type is None and self._conjunto_field is not None) or (
-            self._conjunto_type is not None and self._conjunto_field is None
-        ):
-            raise Exception(
-                "Os parâmetros conjunto_type e conjunto_field devem ser preenchidos juntos (se um for não nulo, ambos devem ser preenchidos)."
-            )
-
-    def __call__(self, cls: object):
-        """
-        Iterating DTO class to handle DTOFields descriptors.
-        """
-
-        # Creating resume_fields in cls, if needed
-        self._check_class_attribute(cls, "resume_fields", set())
-
-        # Creating fields_map in cls, if needed
-        self._check_class_attribute(cls, "fields_map", {})
-
-        # Creating list_fields_map in cls, if needed
-        self._check_class_attribute(cls, "list_fields_map", {})
-
-        # Creating left_join_fields_map in cls, if needed
-        self._check_class_attribute(cls, "left_join_fields_map", {})
-
-        # Creating left_join_fields_map_to_query in cls, if needed
-        self._check_class_attribute(cls, "left_join_fields_map_to_query", {})
-
-        # Creating sql_join_fields_map in cls, if needed
-        self._check_class_attribute(cls, "sql_join_fields_map", {})
-
-        # Creating sql_join_fields_map_to_query in cls, if needed
-        self._check_class_attribute(cls, "sql_join_fields_map_to_query", {})
-
-        # Creating field_filters_map in cls, if needed
-        self._check_class_attribute(cls, "field_filters_map", {})
-
-        # Creating pk_field in cls, if needed
-        # TODO Refatorar para suportar PKs compostas
-        self._check_class_attribute(cls, "pk_field", None)
-
-        # Criando a propriedade "partition_fields" na classe "cls", se necessário
-        self._check_class_attribute(cls, "partition_fields", set())
-
-        # Criando a propriedade "uniques" na classe "cls", se necessário
-        self._check_class_attribute(cls, "uniques", {})
-
-        # Criando a propriedade "candidate_keys" na classe "cls", se necessário
-        self._check_class_attribute(cls, "candidate_keys", [])
-
-        # Criando a propriedade "search_fields" na classe "cls", se necessário
-        self._check_class_attribute(cls, "search_fields", set())
-
-        # Iterating for the class attributes
-        for key, attr in cls.__dict__.items():
-            # Test if the attribute uses the DTOFiel descriptor
-            if isinstance(attr, DTOField):
-                # Storing field in fields_map
-                getattr(cls, "fields_map")[key] = attr
-
-                # Setting a better name to storage_name
-                attr.storage_name = f"{key}"
-                attr.name = f"{key}"
-
-                # Checking filters name
-                self._check_filters(cls, key, attr)
-
-                # Copying type from annotation (if exists)
-                if key in cls.__annotations__:
-                    attr.expected_type = cls.__annotations__[key]
-
-                # Checking if it is a resume field (to store)
-                if attr.resume:
-                    resume_fields = getattr(cls, "resume_fields")
-                    if not (key in resume_fields):
-                        resume_fields.add(key)
+def DTO(
+    fixed_filters: Dict[str, Any] = None,
+    conjunto_type: ConjuntoType = None,
+    conjunto_field: str = None,
+    filter_aliases: Dict[str, Any] = None,
+):
 
+    def DTOWrapper(classe):
+
+        class DTOClass:
+
+            def __init__(
+                self,
+            ) -> None:
+                super().__init__()
+
+                self._fixed_filters = fixed_filters
+                self._conjunto_type = conjunto_type
+                self._conjunto_field = conjunto_field
+                self._filter_aliases = filter_aliases
+
+                if (
+                    self._conjunto_type is None and self._conjunto_field is not None
+                ) or (self._conjunto_type is not None and self._conjunto_field is None):
+                    raise Exception(
+                        "Os parâmetros conjunto_type e conjunto_field devem ser preenchidos juntos (se um for não nulo, ambos devem ser preenchidos)."
+                    )
+
+            @functools.wraps(classe)
+            def __call__(self, cls: object):
+                """
+                Iterating DTO class to handle DTOFields descriptors.
+                """
+
+                # Creating resume_fields in cls, if needed
+                self._check_class_attribute(cls, "resume_fields", set())
+
+                # Creating fields_map in cls, if needed
+                self._check_class_attribute(cls, "fields_map", {})
+
+                # Creating list_fields_map in cls, if needed
+                self._check_class_attribute(cls, "list_fields_map", {})
+
+                # Creating left_join_fields_map in cls, if needed
+                self._check_class_attribute(cls, "left_join_fields_map", {})
+
+                # Creating left_join_fields_map_to_query in cls, if needed
+                self._check_class_attribute(cls, "left_join_fields_map_to_query", {})
+
+                # Creating sql_join_fields_map in cls, if needed
+                self._check_class_attribute(cls, "sql_join_fields_map", {})
+
+                # Creating sql_join_fields_map_to_query in cls, if needed
+                self._check_class_attribute(cls, "sql_join_fields_map_to_query", {})
+
+                # Creating object_fields_map in cls, if needed
+                self._check_class_attribute(cls, "object_fields_map", {})
+
+                # Creating field_filters_map in cls, if needed
+                self._check_class_attribute(cls, "field_filters_map", {})
+
+                # Creating pk_field in cls, if needed
                 # TODO Refatorar para suportar PKs compostas
-                # Setting PK info
-                if attr.pk:
-                    setattr(cls, "pk_field", f"{key}")
-
-                # Verifica se é um campo de particionamento, e o guarda em caso positivo
-                if attr.partition_data:
-                    partition_fields = getattr(cls, "partition_fields")
-                    if not (key in partition_fields):
-                        partition_fields.add(key)
-
-                # Verifica se é um campo pertencente a uma unique, a populando o dicionário de uniques
-                if attr.unique:
-                    uniques = getattr(cls, "uniques")
-                    fields_unique = uniques.setdefault(attr.unique, set())
-                    fields_unique.add(key)
-
-                # Verifica se é uma chave candidata
-                if attr.candidate_key:
-                    getattr(cls, "candidate_keys").append(key)
-
-                # Verifica se é um campo passível de busca
-                if attr.search:
-                    getattr(cls, "search_fields").add(key)
-
-            elif isinstance(attr, DTOListField):
-                # Storing field in fields_map
-                getattr(cls, "list_fields_map")[key] = attr
-
-                # Setting a better name to storage_name
-                attr.storage_name = f"{key}"
-                attr.name = f"{key}"
-
-            elif isinstance(attr, DTOLeftJoinField):
-                # Storing field in fields_map
-                getattr(cls, "left_join_fields_map")[key] = attr
-
-                # Setting a better name to storage_name
-                attr.storage_name = f"{key}"
-                attr.name = f"{key}"
-
-                # Copying type from annotation (if exists)
-                if key in cls.__annotations__:
-                    attr.expected_type = cls.__annotations__[key]
-
-                # Checking if it is a resume field (to store)
-                if attr.resume:
-                    resume_fields = getattr(cls, "resume_fields")
-                    if not (key in resume_fields):
-                        resume_fields.add(key)
-
-                # Montando o mapa de controle das queries (para o service_base)
-                self.set_left_join_fields_map_to_query(key, attr, cls)
-
-            elif isinstance(attr, DTOSQLJoinField):
-                # Storing field in fields_map
-                getattr(cls, "sql_join_fields_map")[key] = attr
-
-                # Setting a better name to storage_name
-                attr.storage_name = f"{key}"
-                attr.name = f"{key}"
-
-                # Copying type from annotation (if exists)
-                if key in cls.__annotations__:
-                    attr.expected_type = cls.__annotations__[key]
-
-                # Checking if it is a resume field (to store)
-                if attr.resume:
-                    resume_fields = getattr(cls, "resume_fields")
-                    if not (key in resume_fields):
-                        resume_fields.add(key)
-
-                # Montando o mapa de controle das queries (para o service_base)
-                self.set_sql_join_fields_map_to_query(key, attr, cls)
-
-        # Setting fixed filters
-        setattr(cls, "fixed_filters", self._fixed_filters)
-
-        # Setting tipo de Conjunto
-        setattr(cls, "conjunto_type", self._conjunto_type)
-        setattr(cls, "conjunto_field", self._conjunto_field)
-
-        # Setting filter aliases
-        setattr(cls, "filter_aliases", self._filter_aliases)
-
-        return cls
-
-    def _check_filters(self, cls: object, field_name: str, dto_field: DTOField):
-        """
-        Check filters (if exists), and setting default filter name.
-        """
-
-        if dto_field.filters is None:
-            return
-
-        # Handling each filter
-        for filter in dto_field.filters:
-            # Resolving filter name
-            filter_name = field_name
-            if filter.name is not None:
-                filter_name = filter.name
-
-            # Storing field filter name
-            filter.field_name = field_name
-
-            # Adding into field filters map
-            field_filters_map = getattr(cls, "field_filters_map")
-            field_filters_map[filter_name] = filter
-
-    def _check_class_attribute(self, cls: object, attr_name: str, default_value: Any):
-        """
-        Add attribute "attr_name" in class "cls", if not exists.
-        """
-
-        if attr_name not in cls.__dict__:
-            setattr(cls, attr_name, default_value)
-
-    def set_left_join_fields_map_to_query(
-        self,
-        field: str,
-        attr: DTOLeftJoinField,
-        cls: object,
-    ):
-        # Recuperando o map de facilitação das queries
-        left_join_fields_map_to_query: dict[str, LeftJoinQuery] = getattr(
-            cls, "left_join_fields_map_to_query"
-        )
-
-        # Verificando se o objeto de query, relativo a esse campo,
-        # já estava no mapa (e colocando, caso negativo)
-        map_key = (
-            f"{attr.dto_type}____{attr.entity_type}____{attr.entity_relation_owner}"
-        )
-        left_join_query = left_join_fields_map_to_query.setdefault(
-            map_key, LeftJoinQuery()
-        )
-
-        # Preenchendo as propriedades que serão úteis para as queries
-        left_join_query.related_dto = attr.dto_type
-        left_join_query.related_entity = attr.entity_type
-        left_join_query.fields.append(field)
-        left_join_query.left_join_fields.append(attr)
-        left_join_query.entity_relation_owner = attr.entity_relation_owner
-
-    def set_sql_join_fields_map_to_query(
-        self,
-        field: str,
-        attr: DTOSQLJoinField,
-        cls: object,
-    ):
-        # Recuperando o map de facilitação das queries
-        sql_join_fields_map_to_query: dict[str, SQLJoinQuery] = getattr(
-            cls, "sql_join_fields_map_to_query"
-        )
-
-        # Verificando se o objeto de query, relativo a esse campo,
-        # já estava no mapa (e colocando, caso negativo)
-        map_key = f"{attr.dto_type}____{attr.entity_type}____{attr.entity_relation_owner}____{attr.join_type}"
-        sql_join_query = sql_join_fields_map_to_query.setdefault(
-            map_key, SQLJoinQuery()
-        )
-
-        # Preenchendo as propriedades que serão úteis para as queries
-        sql_join_query.related_dto = attr.dto_type
-        sql_join_query.related_entity = attr.entity_type
-        sql_join_query.fields.append(field)
-        sql_join_query.related_fields.append(attr.related_dto_field)
-        sql_join_query.join_fields.append(attr)
-        sql_join_query.entity_relation_owner = attr.entity_relation_owner
-        sql_join_query.join_type = attr.join_type
-        sql_join_query.relation_field = attr.relation_field
+                self._check_class_attribute(cls, "pk_field", None)
+
+                # Criando a propriedade "partition_fields" na classe "cls", se necessário
+                self._check_class_attribute(cls, "partition_fields", set())
+
+                # Criando a propriedade "uniques" na classe "cls", se necessário
+                self._check_class_attribute(cls, "uniques", {})
+
+                # Criando a propriedade "candidate_keys" na classe "cls", se necessário
+                self._check_class_attribute(cls, "candidate_keys", [])
+
+                # Criando a propriedade "search_fields" na classe "cls", se necessário
+                self._check_class_attribute(cls, "search_fields", set())
+
+                # Iterating for the class attributes
+                for key, attr in cls.__dict__.items():
+                    # Test if the attribute uses the DTOFiel descriptor
+                    if isinstance(attr, DTOField):
+                        # Storing field in fields_map
+                        getattr(cls, "fields_map")[key] = attr
+
+                        # Setting a better name to storage_name
+                        attr.storage_name = f"{key}"
+                        attr.name = f"{key}"
+
+                        # Checking filters name
+                        self._check_filters(cls, key, attr)
+
+                        # Copying type from annotation (if exists)
+                        if key in cls.__annotations__:
+                            attr.expected_type = cls.__annotations__[key]
+
+                        # Checking if it is a resume field (to store)
+                        if attr.resume:
+                            resume_fields = getattr(cls, "resume_fields")
+                            if key not in resume_fields:
+                                resume_fields.add(key)
+
+                        # TODO Refatorar para suportar PKs compostas
+                        # Setting PK info
+                        if attr.pk:
+                            setattr(cls, "pk_field", f"{key}")
+
+                        # Verifica se é um campo de particionamento, e o guarda em caso positivo
+                        if attr.partition_data:
+                            partition_fields = getattr(cls, "partition_fields")
+                            if key not in partition_fields:
+                                partition_fields.add(key)
+
+                        # Verifica se é um campo pertencente a uma unique, a populando o dicionário de uniques
+                        if attr.unique:
+                            uniques = getattr(cls, "uniques")
+                            fields_unique = uniques.setdefault(attr.unique, set())
+                            fields_unique.add(key)
+
+                        # Verifica se é uma chave candidata
+                        if attr.candidate_key:
+                            getattr(cls, "candidate_keys").append(key)
+
+                        # Verifica se é um campo passível de busca
+                        if attr.search:
+                            getattr(cls, "search_fields").add(key)
+
+                    elif isinstance(attr, DTOListField):
+                        # Storing field in fields_map
+                        getattr(cls, "list_fields_map")[key] = attr
+
+                        # Setting a better name to storage_name
+                        attr.storage_name = f"{key}"
+                        attr.name = f"{key}"
+
+                    elif isinstance(attr, DTOLeftJoinField):
+                        # Storing field in fields_map
+                        getattr(cls, "left_join_fields_map")[key] = attr
+
+                        # Setting a better name to storage_name
+                        attr.storage_name = f"{key}"
+                        attr.name = f"{key}"
+
+                        # Copying type from annotation (if exists)
+                        if key in cls.__annotations__:
+                            attr.expected_type = cls.__annotations__[key]
+
+                        # Checking if it is a resume field (to store)
+                        if attr.resume:
+                            resume_fields = getattr(cls, "resume_fields")
+                            if key not in resume_fields:
+                                resume_fields.add(key)
+
+                        # Montando o mapa de controle das queries (para o service_base)
+                        self.set_left_join_fields_map_to_query(key, attr, cls)
+
+                    elif isinstance(attr, DTOSQLJoinField):
+                        # Storing field in fields_map
+                        getattr(cls, "sql_join_fields_map")[key] = attr
+
+                        # Setting a better name to storage_name
+                        attr.storage_name = f"{key}"
+                        attr.name = f"{key}"
+
+                        # Copying type from annotation (if exists)
+                        if key in cls.__annotations__:
+                            attr.expected_type = cls.__annotations__[key]
+
+                        # Checking if it is a resume field (to store)
+                        if attr.resume:
+                            resume_fields = getattr(cls, "resume_fields")
+                            if key not in resume_fields:
+                                resume_fields.add(key)
+
+                        # Montando o mapa de controle das queries (para o service_base)
+                        self.set_sql_join_fields_map_to_query(key, attr, cls)
+
+                    elif isinstance(attr, DTOObjectField):
+                        # Storing field in fields_map
+                        getattr(cls, "object_fields_map")[key] = attr
+
+                        # Setting a better name to storage_name
+                        attr.storage_name = f"{key}"
+                        attr.name = f"{key}"
+
+                        # Copying type from annotation (if exists)
+                        if key in cls.__annotations__:
+                            attr.expected_type = cls.__annotations__[key]
+
+                        # Checking if it is a resume field (to store)
+                        if attr.resume:
+                            resume_fields = getattr(cls, "resume_fields")
+                            if key not in resume_fields:
+                                resume_fields.add(key)
+
+                # Setting fixed filters
+                setattr(cls, "fixed_filters", self._fixed_filters)
+
+                # Setting tipo de Conjunto
+                setattr(cls, "conjunto_type", self._conjunto_type)
+                setattr(cls, "conjunto_field", self._conjunto_field)
+
+                # Setting filter aliases
+                setattr(cls, "filter_aliases", self._filter_aliases)
+
+                return cls
+
+            def _check_filters(self, cls: object, field_name: str, dto_field: DTOField):
+                """
+                Check filters (if exists), and setting default filter name.
+                """
+
+                if dto_field.filters is None:
+                    return
+
+                # Handling each filter
+                for filter in dto_field.filters:
+                    # Resolving filter name
+                    filter_name = field_name
+                    if filter.name is not None:
+                        filter_name = filter.name
+
+                    # Storing field filter name
+                    filter.field_name = field_name
+
+                    # Adding into field filters map
+                    field_filters_map = getattr(cls, "field_filters_map")
+                    field_filters_map[filter_name] = filter
+
+            def _check_class_attribute(
+                self, cls: object, attr_name: str, default_value: Any
+            ):
+                """
+                Add attribute "attr_name" in class "cls", if not exists.
+                """
+
+                if attr_name not in cls.__dict__:
+                    setattr(cls, attr_name, default_value)
+
+            def set_left_join_fields_map_to_query(
+                self,
+                field: str,
+                attr: DTOLeftJoinField,
+                cls: object,
+            ):
+                # Recuperando o map de facilitação das queries
+                left_join_fields_map_to_query: dict[str, LeftJoinQuery] = getattr(
+                    cls, "left_join_fields_map_to_query"
+                )
+
+                # Verificando se o objeto de query, relativo a esse campo,
+                # já estava no mapa (e colocando, caso negativo)
+                map_key = f"{attr.dto_type}____{attr.entity_type}____{attr.entity_relation_owner}"
+                left_join_query = left_join_fields_map_to_query.setdefault(
+                    map_key, LeftJoinQuery()
+                )
+
+                # Preenchendo as propriedades que serão úteis para as queries
+                left_join_query.related_dto = attr.dto_type
+                left_join_query.related_entity = attr.entity_type
+                left_join_query.fields.append(field)
+                left_join_query.left_join_fields.append(attr)
+                left_join_query.entity_relation_owner = attr.entity_relation_owner
+
+            def set_sql_join_fields_map_to_query(
+                self,
+                field: str,
+                attr: DTOSQLJoinField,
+                cls: object,
+            ):
+                # Recuperando o map de facilitação das queries
+                sql_join_fields_map_to_query: dict[str, SQLJoinQuery] = getattr(
+                    cls, "sql_join_fields_map_to_query"
+                )
+
+                # Verificando se o objeto de query, relativo a esse campo,
+                # já estava no mapa (e colocando, caso negativo)
+                map_key = f"{attr.dto_type}____{attr.entity_type}____{attr.entity_relation_owner}____{attr.join_type}"
+                sql_join_query = sql_join_fields_map_to_query.setdefault(
+                    map_key, SQLJoinQuery()
+                )
+
+                # Preenchendo as propriedades que serão úteis para as queries
+                sql_join_query.related_dto = attr.dto_type
+                sql_join_query.related_entity = attr.entity_type
+                sql_join_query.fields.append(field)
+                sql_join_query.related_fields.append(attr.related_dto_field)
+                sql_join_query.join_fields.append(attr)
+                sql_join_query.entity_relation_owner = attr.entity_relation_owner
+                sql_join_query.join_type = attr.join_type
+                sql_join_query.relation_field = attr.relation_field
+
+                if sql_join_query.sql_alias is None:
+                    sql_join_query.sql_alias = (
+                        f"join_table_{len(sql_join_fields_map_to_query)}"
+                    )
+
+        return DTOClass().__call__(classe)
 
-        if sql_join_query.sql_alias is None:
-            sql_join_query.sql_alias = f"join_table_{len(sql_join_fields_map_to_query)}"
+    return DTOWrapper
```

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/decorator/entity.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/decorator/entity.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_left_join_field.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_left_join_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/descriptor/dto_sql_join_field.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/descriptor/dto_sql_join_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/dto/dto_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     partition_fields: Set[str] = set()
     fields_map: Dict[str, DTOField] = {}
     list_fields_map: dict = {}
     left_join_fields_map: dict = {}
     left_join_fields_map_to_query: dict = {}
     sql_join_fields_map: dict = {}
     sql_join_fields_map_to_query: dict = {}
+    object_fields_map: dict = {}
     field_filters_map: Dict[str, DTOFieldFilter]
     # TODO Refatorar para suportar PK composto
     pk_field: str
     fixed_filters: Dict[str, Any]
     conjunto_type: ConjuntoType
     conjunto_field: str
     escape_validator: bool
@@ -138,14 +139,25 @@
 
             # Atribuindo o valor à propriedade do DTO
             if field in kwargs:
                 setattr(self, field, kwargs[field])
             else:
                 setattr(self, field, None)
 
+        # Setando os campos registrados como fields object
+        for field in self.__class__.object_fields_map:
+            # Recuperando a configuração do campo
+            aux_dto_field = self.__class__.object_fields_map[field]
+
+            # Atribuindo o valor à propriedade do DTO
+            if field in kwargs:
+                setattr(self, field, aux_dto_field.expected_type(**kwargs[field]))
+            else:
+                setattr(self, field, None)
+
         # Setando os campos registrados como fields de lista
         if entity is None:
             for field in self.__class__.list_fields_map:
                 dto_list_field = self.__class__.list_fields_map[field]
 
                 if field in kwargs:
                     if not isinstance(kwargs[field], list):
```

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/service/service_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/util/type_validator_util.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/util/type_validator_util.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 2.6.4
+Version: 2.7.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-2.6.4/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-2.7.0/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/nsj_rest_lib/decorator/entity.py
 src/nsj_rest_lib/descriptor/__init__.py
 src/nsj_rest_lib/descriptor/conjunto_type.py
 src/nsj_rest_lib/descriptor/dto_field.py
 src/nsj_rest_lib/descriptor/dto_field_validators.py
 src/nsj_rest_lib/descriptor/dto_left_join_field.py
 src/nsj_rest_lib/descriptor/dto_list_field.py
+src/nsj_rest_lib/descriptor/dto_object_field.py
 src/nsj_rest_lib/descriptor/dto_sql_join_field.py
 src/nsj_rest_lib/descriptor/filter_operator.py
 src/nsj_rest_lib/dto/__init__.py
 src/nsj_rest_lib/dto/after_insert_update_data.py
 src/nsj_rest_lib/dto/dto_base.py
 src/nsj_rest_lib/entity/__init__.py
 src/nsj_rest_lib/entity/entity_base.py
```

