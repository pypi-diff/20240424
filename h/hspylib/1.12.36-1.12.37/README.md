# Comparing `tmp/hspylib-1.12.36.tar.gz` & `tmp/hspylib-1.12.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-1.12.36.tar", last modified: Sun Apr 21 04:42:13 2024, max compression
+gzip compressed data, was "hspylib-1.12.37.tar", last modified: Wed Apr 24 19:01:13 2024, max compression
```

## Comparing `hspylib-1.12.36.tar` & `hspylib-1.12.37.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.425635 hspylib-1.12.36/
--rw-r--r--   0 hugo       (503) staff       (20)       25 2023-09-24 15:24:10.000000 hspylib-1.12.36/MANIFEST.in
--rw-r--r--   0 hugo       (503) staff       (20)    13229 2024-04-21 04:42:13.424615 hspylib-1.12.36/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)    11869 2024-04-21 04:42:08.000000 hspylib-1.12.36/README.md
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.388815 hspylib-1.12.36/hspylib/
--rw-r--r--   0 hugo       (503) staff       (20)        7 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/.version
--rw-r--r--   0 hugo       (503) staff       (20)      886 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/__classpath__.py
--rw-r--r--   0 hugo       (503) staff       (20)      167 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/__init__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.394554 hspylib-1.12.36/hspylib/core/
--rw-r--r--   0 hugo       (503) staff       (20)      347 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     6055 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/collection_filter.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.396628 hspylib-1.12.36/hspylib/core/config/
--rw-r--r--   0 hugo       (503) staff       (20)      211 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/config/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3380 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/config/app_config.py
--rw-r--r--   0 hugo       (503) staff       (20)     3131 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/config/parser_factory.py
--rw-r--r--   0 hugo       (503) staff       (20)     4727 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/config/properties.py
--rw-r--r--   0 hugo       (503) staff       (20)     1819 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/constants.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.397497 hspylib-1.12.36/hspylib/core/decorator/
--rw-r--r--   0 hugo       (503) staff       (20)      172 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/decorator/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2015 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/decorator/decorators.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.401100 hspylib-1.12.36/hspylib/core/enums/
--rw-r--r--   0 hugo       (503) staff       (20)      244 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/enums/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3429 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/charset.py
--rw-r--r--   0 hugo       (503) staff       (20)     4335 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/content_type.py
--rw-r--r--   0 hugo       (503) staff       (20)     2926 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/enumeration.py
--rw-r--r--   0 hugo       (503) staff       (20)     6356 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/http_code.py
--rw-r--r--   0 hugo       (503) staff       (20)     1745 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/enums/http_method.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.402334 hspylib-1.12.36/hspylib/core/exception/
--rw-r--r--   0 hugo       (503) staff       (20)      172 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/exception/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2256 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/exception/exceptions.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.403866 hspylib-1.12.36/hspylib/core/metaclass/
--rw-r--r--   0 hugo       (503) staff       (20)      189 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/metaclass/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     6243 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/metaclass/classpath.py
--rw-r--r--   0 hugo       (503) staff       (20)     2847 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/metaclass/singleton.py
--rw-r--r--   0 hugo       (503) staff       (20)     5082 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/namespace.py
--rw-r--r--   0 hugo       (503) staff       (20)     3611 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/preconditions.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.406658 hspylib-1.12.36/hspylib/core/tools/
--rw-r--r--   0 hugo       (503) staff       (20)      239 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/core/tools/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     8802 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/tools/commons.py
--rw-r--r--   0 hugo       (503) staff       (20)     3403 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/tools/dict_tools.py
--rwxr-xr-x   0 hugo       (503) staff       (20)     7170 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/tools/json_path.py
--rw-r--r--   0 hugo       (503) staff       (20)     8084 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/core/tools/text_tools.py
--rw-r--r--   0 hugo       (503) staff       (20)     2243 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/tools/validator.py
--rw-r--r--   0 hugo       (503) staff       (20)     1617 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/core/zoned_datetime.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.407124 hspylib-1.12.36/hspylib/modules/
--rw-r--r--   0 hugo       (503) staff       (20)      240 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/__init__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.409737 hspylib-1.12.36/hspylib/modules/application/
--rw-r--r--   0 hugo       (503) staff       (20)      250 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/application/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     7687 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/modules/application/application.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.412863 hspylib-1.12.36/hspylib/modules/application/argparse/
--rw-r--r--   0 hugo       (503) staff       (20)      297 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/application/argparse/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1073 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/argument_parser.py
--rw-r--r--   0 hugo       (503) staff       (20)     1343 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/arguments_builder.py
--rw-r--r--   0 hugo       (503) staff       (20)     2780 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/chained_arguments_builder.py
--rw-r--r--   0 hugo       (503) staff       (20)     1619 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/options_builder.py
--rw-r--r--   0 hugo       (503) staff       (20)     1532 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/argparse/parser_action.py
--rw-r--r--   0 hugo       (503) staff       (20)     1935 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/exit_hooks.py
--rw-r--r--   0 hugo       (503) staff       (20)     2177 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/exit_status.py
--rw-r--r--   0 hugo       (503) staff       (20)     2990 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/application/version.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.414074 hspylib-1.12.36/hspylib/modules/cache/
--rw-r--r--   0 hugo       (503) staff       (20)      193 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/cache/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2585 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/cache/ttl_cache.py
--rw-r--r--   0 hugo       (503) staff       (20)     2801 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/cache/ttl_keyring_be.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.415285 hspylib-1.12.36/hspylib/modules/cli/
--rw-r--r--   0 hugo       (503) staff       (20)      181 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/cli/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     7286 2024-04-21 04:40:06.000000 hspylib-1.12.36/hspylib/modules/cli/keyboard.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.417037 hspylib-1.12.36/hspylib/modules/cli/vt100/
--rw-r--r--   0 hugo       (503) staff       (20)      204 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/cli/vt100/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     5709 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/modules/cli/vt100/vt_100.py
--rw-r--r--   0 hugo       (503) staff       (20)     5115 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/modules/cli/vt100/vt_code.py
--rw-r--r--   0 hugo       (503) staff       (20)     2582 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/cli/vt100/vt_color.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.419018 hspylib-1.12.36/hspylib/modules/eventbus/
--rw-r--r--   0 hugo       (503) staff       (20)      186 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/eventbus/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1242 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/eventbus/event.py
--rw-r--r--   0 hugo       (503) staff       (20)     3721 2024-03-23 00:45:19.000000 hspylib-1.12.36/hspylib/modules/eventbus/eventbus.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.421996 hspylib-1.12.36/hspylib/modules/fetch/
--rw-r--r--   0 hugo       (503) staff       (20)      227 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/fetch/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     4779 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/fetch/fetch.py
--rw-r--r--   0 hugo       (503) staff       (20)     1888 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/fetch/http_response.py
--rw-r--r--   0 hugo       (503) staff       (20)     5412 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/fetch/uri_builder.py
--rw-r--r--   0 hugo       (503) staff       (20)     1082 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/fetch/uri_scheme.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.422825 hspylib-1.12.36/hspylib/modules/security/
--rw-r--r--   0 hugo       (503) staff       (20)      172 2024-04-21 04:42:09.000000 hspylib-1.12.36/hspylib/modules/security/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     6481 2024-01-06 13:35:49.000000 hspylib-1.12.36/hspylib/modules/security/security.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-21 04:42:13.423620 hspylib-1.12.36/hspylib.egg-info/
--rw-r--r--   0 hugo       (503) staff       (20)    13229 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)     2449 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (503) staff       (20)        1 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (503) staff       (20)      129 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/requires.txt
--rw-r--r--   0 hugo       (503) staff       (20)       13 2024-04-21 04:42:13.000000 hspylib-1.12.36/hspylib.egg-info/top_level.txt
--rw-r--r--   0 hugo       (503) staff       (20)       38 2024-04-21 04:42:13.425770 hspylib-1.12.36/setup.cfg
--rw-r--r--   0 hugo       (503) staff       (20)     2003 2024-01-06 13:35:49.000000 hspylib-1.12.36/setup.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.832086 hspylib-1.12.37/
+-rw-r--r--   0 hjunior    (501) staff       (20)       25 2024-02-16 22:31:12.000000 hspylib-1.12.37/MANIFEST.in
+-rw-r--r--   0 hjunior    (501) staff       (20)    13229 2024-04-24 19:01:13.828555 hspylib-1.12.37/PKG-INFO
+-rw-r--r--   0 hjunior    (501) staff       (20)    11869 2024-04-24 19:01:05.000000 hspylib-1.12.37/README.md
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.656016 hspylib-1.12.37/hspylib/
+-rw-r--r--   0 hjunior    (501) staff       (20)        7 2024-04-24 19:01:05.000000 hspylib-1.12.37/hspylib/.version
+-rw-r--r--   0 hjunior    (501) staff       (20)      886 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/__classpath__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)      167 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/__init__.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.685783 hspylib-1.12.37/hspylib/core/
+-rw-r--r--   0 hjunior    (501) staff       (20)      347 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/core/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     6055 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/collection_filter.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.700139 hspylib-1.12.37/hspylib/core/config/
+-rw-r--r--   0 hjunior    (501) staff       (20)      248 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/core/config/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3459 2024-04-24 18:07:19.000000 hspylib-1.12.37/hspylib/core/config/app_config.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3131 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/config/parser_factory.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2275 2024-04-24 18:33:44.000000 hspylib-1.12.37/hspylib/core/config/path_object.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     4727 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/config/properties.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2056 2024-04-24 15:42:06.000000 hspylib-1.12.37/hspylib/core/config/settings.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1819 2024-03-20 19:25:39.000000 hspylib-1.12.37/hspylib/core/constants.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.704257 hspylib-1.12.37/hspylib/core/decorator/
+-rw-r--r--   0 hjunior    (501) staff       (20)      172 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/core/decorator/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2015 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/decorator/decorators.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.718488 hspylib-1.12.37/hspylib/core/enums/
+-rw-r--r--   0 hjunior    (501) staff       (20)      244 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/core/enums/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3429 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/enums/charset.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     4335 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/enums/content_type.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2926 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/enums/enumeration.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     6356 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/enums/http_code.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1745 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/enums/http_method.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.723527 hspylib-1.12.37/hspylib/core/exception/
+-rw-r--r--   0 hjunior    (501) staff       (20)      172 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/core/exception/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2256 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.731065 hspylib-1.12.37/hspylib/core/metaclass/
+-rw-r--r--   0 hjunior    (501) staff       (20)      189 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/core/metaclass/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     6243 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/metaclass/classpath.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2847 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/metaclass/singleton.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     5082 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/namespace.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3611 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/preconditions.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.745100 hspylib-1.12.37/hspylib/core/tools/
+-rw-r--r--   0 hjunior    (501) staff       (20)      239 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/core/tools/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     8802 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/tools/commons.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3403 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/tools/dict_tools.py
+-rwxr-xr-x   0 hjunior    (501) staff       (20)     7170 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/tools/json_path.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     8084 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/tools/text_tools.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2243 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/tools/validator.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1617 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/core/zoned_datetime.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.747425 hspylib-1.12.37/hspylib/modules/
+-rw-r--r--   0 hjunior    (501) staff       (20)      240 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/__init__.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.756888 hspylib-1.12.37/hspylib/modules/application/
+-rw-r--r--   0 hjunior    (501) staff       (20)      250 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/application/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     7687 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/application.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.774659 hspylib-1.12.37/hspylib/modules/application/argparse/
+-rw-r--r--   0 hjunior    (501) staff       (20)      297 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/application/argparse/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1073 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/argparse/argument_parser.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1343 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/argparse/arguments_builder.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2780 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/argparse/chained_arguments_builder.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1619 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/argparse/options_builder.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1532 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/argparse/parser_action.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1935 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/exit_hooks.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2177 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/exit_status.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2990 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/application/version.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.782633 hspylib-1.12.37/hspylib/modules/cache/
+-rw-r--r--   0 hjunior    (501) staff       (20)      193 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/cache/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2585 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/cache/ttl_cache.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2801 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/cache/ttl_keyring_be.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.786975 hspylib-1.12.37/hspylib/modules/cli/
+-rw-r--r--   0 hjunior    (501) staff       (20)      181 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/cli/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     7286 2024-04-22 15:29:28.000000 hspylib-1.12.37/hspylib/modules/cli/keyboard.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.798313 hspylib-1.12.37/hspylib/modules/cli/vt100/
+-rw-r--r--   0 hjunior    (501) staff       (20)      204 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/cli/vt100/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     5709 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/cli/vt100/vt_100.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     5115 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/cli/vt100/vt_code.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2582 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/cli/vt100/vt_color.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.804792 hspylib-1.12.37/hspylib/modules/eventbus/
+-rw-r--r--   0 hjunior    (501) staff       (20)      186 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/eventbus/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1242 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/eventbus/event.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3721 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/eventbus/eventbus.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.814614 hspylib-1.12.37/hspylib/modules/fetch/
+-rw-r--r--   0 hjunior    (501) staff       (20)      227 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/fetch/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     4779 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/fetch/fetch.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1888 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/fetch/http_response.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     5412 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/fetch/uri_builder.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1082 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/fetch/uri_scheme.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.819833 hspylib-1.12.37/hspylib/modules/security/
+-rw-r--r--   0 hjunior    (501) staff       (20)      172 2024-04-24 19:01:06.000000 hspylib-1.12.37/hspylib/modules/security/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     6481 2024-03-20 19:25:41.000000 hspylib-1.12.37/hspylib/modules/security/security.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-24 19:01:13.825692 hspylib-1.12.37/hspylib.egg-info/
+-rw-r--r--   0 hjunior    (501) staff       (20)    13229 2024-04-24 19:01:13.000000 hspylib-1.12.37/hspylib.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (501) staff       (20)     2516 2024-04-24 19:01:13.000000 hspylib-1.12.37/hspylib.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (501) staff       (20)        1 2024-04-24 19:01:13.000000 hspylib-1.12.37/hspylib.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (501) staff       (20)      129 2024-04-24 19:01:13.000000 hspylib-1.12.37/hspylib.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (501) staff       (20)       13 2024-04-24 19:01:13.000000 hspylib-1.12.37/hspylib.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (501) staff       (20)       38 2024-04-24 19:01:13.832361 hspylib-1.12.37/setup.cfg
+-rw-r--r--   0 hjunior    (501) staff       (20)     2003 2024-03-20 19:25:41.000000 hspylib-1.12.37/setup.py
```

### Comparing `hspylib-1.12.36/PKG-INFO` & `hspylib-1.12.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib
-Version: 1.12.36
+Version: 1.12.37
 Summary: HsPyLib - Core python library
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib/
```

### Comparing `hspylib-1.12.36/README.md` & `hspylib-1.12.37/README.md`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/__classpath__.py` & `hspylib-1.12.37/hspylib/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/collection_filter.py` & `hspylib-1.12.37/hspylib/core/collection_filter.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/config/app_config.py` & `hspylib-1.12.37/hspylib/core/config/app_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-
+from hspylib.core.config.path_object import PathObject
 from hspylib.core.config.properties import Properties
 from hspylib.core.metaclass.classpath import AnyPath
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_argument
 from hspylib.core.tools.commons import run_dir, to_bool
 from textwrap import dedent
 from typing import Any, Optional
@@ -37,16 +37,17 @@
       |-Resources-dir = {}
       |-Properties:
        \\-{}
     """
     )
 
     def __init__(self, resource_dir: AnyPath, filename: str | None = None, profile: str | None = None):
-        check_argument(os.path.exists(str(resource_dir)), "Unable to locate resources dir: {}", resource_dir)
-        self._resource_dir = str(resource_dir)
+        path_obj = PathObject.of(resource_dir)
+        check_argument(path_obj.exists, "Unable to locate resources dir: {}", resource_dir)
+        self._resource_dir = str(path_obj)
         self._properties = Properties(filename=filename, load_dir=resource_dir, profile=profile)
         log.info(self)
 
     # pylint: disable=consider-using-f-string
     def __str__(self) -> str:
         return "\n{}{}{}".format(
             "-=" * 40,
```

### Comparing `hspylib-1.12.36/hspylib/core/config/parser_factory.py` & `hspylib-1.12.37/hspylib/core/config/parser_factory.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/config/properties.py` & `hspylib-1.12.37/hspylib/core/config/properties.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/constants.py` & `hspylib-1.12.37/hspylib/core/constants.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/decorator/decorators.py` & `hspylib-1.12.37/hspylib/core/decorator/decorators.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/enums/charset.py` & `hspylib-1.12.37/hspylib/core/enums/charset.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/enums/content_type.py` & `hspylib-1.12.37/hspylib/core/enums/content_type.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/enums/enumeration.py` & `hspylib-1.12.37/hspylib/core/enums/enumeration.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/enums/http_code.py` & `hspylib-1.12.37/hspylib/core/enums/http_code.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/enums/http_method.py` & `hspylib-1.12.37/hspylib/core/enums/http_method.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/exception/exceptions.py` & `hspylib-1.12.37/hspylib/core/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/metaclass/classpath.py` & `hspylib-1.12.37/hspylib/core/metaclass/classpath.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/metaclass/singleton.py` & `hspylib-1.12.37/hspylib/core/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/namespace.py` & `hspylib-1.12.37/hspylib/core/namespace.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/preconditions.py` & `hspylib-1.12.37/hspylib/core/preconditions.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/tools/commons.py` & `hspylib-1.12.37/hspylib/core/tools/commons.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/tools/dict_tools.py` & `hspylib-1.12.37/hspylib/core/tools/dict_tools.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/tools/json_path.py` & `hspylib-1.12.37/hspylib/core/tools/json_path.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/tools/text_tools.py` & `hspylib-1.12.37/hspylib/core/tools/text_tools.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/tools/validator.py` & `hspylib-1.12.37/hspylib/core/tools/validator.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/core/zoned_datetime.py` & `hspylib-1.12.37/hspylib/core/zoned_datetime.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/application.py` & `hspylib-1.12.37/hspylib/modules/application/application.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/argparse/argument_parser.py` & `hspylib-1.12.37/hspylib/modules/application/argparse/argument_parser.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/argparse/arguments_builder.py` & `hspylib-1.12.37/hspylib/modules/application/argparse/arguments_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/argparse/chained_arguments_builder.py` & `hspylib-1.12.37/hspylib/modules/application/argparse/chained_arguments_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/argparse/options_builder.py` & `hspylib-1.12.37/hspylib/modules/application/argparse/options_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/argparse/parser_action.py` & `hspylib-1.12.37/hspylib/modules/application/argparse/parser_action.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/exit_hooks.py` & `hspylib-1.12.37/hspylib/modules/application/exit_hooks.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/exit_status.py` & `hspylib-1.12.37/hspylib/modules/application/exit_status.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/application/version.py` & `hspylib-1.12.37/hspylib/modules/application/version.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/cache/ttl_cache.py` & `hspylib-1.12.37/hspylib/modules/cache/ttl_cache.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/cache/ttl_keyring_be.py` & `hspylib-1.12.37/hspylib/modules/cache/ttl_keyring_be.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/cli/keyboard.py` & `hspylib-1.12.37/hspylib/modules/cli/keyboard.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/cli/vt100/vt_100.py` & `hspylib-1.12.37/hspylib/modules/cli/vt100/vt_100.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/cli/vt100/vt_code.py` & `hspylib-1.12.37/hspylib/modules/cli/vt100/vt_code.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/cli/vt100/vt_color.py` & `hspylib-1.12.37/hspylib/modules/cli/vt100/vt_color.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/eventbus/event.py` & `hspylib-1.12.37/hspylib/modules/eventbus/event.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/eventbus/eventbus.py` & `hspylib-1.12.37/hspylib/modules/eventbus/eventbus.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/fetch/fetch.py` & `hspylib-1.12.37/hspylib/modules/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/fetch/http_response.py` & `hspylib-1.12.37/hspylib/modules/fetch/http_response.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/fetch/uri_builder.py` & `hspylib-1.12.37/hspylib/modules/fetch/uri_builder.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/fetch/uri_scheme.py` & `hspylib-1.12.37/hspylib/modules/fetch/uri_scheme.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib/modules/security/security.py` & `hspylib-1.12.37/hspylib/modules/security/security.py`

 * *Files identical despite different names*

### Comparing `hspylib-1.12.36/hspylib.egg-info/PKG-INFO` & `hspylib-1.12.37/hspylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib
-Version: 1.12.36
+Version: 1.12.37
 Summary: HsPyLib - Core python library
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib/
```

### Comparing `hspylib-1.12.36/hspylib.egg-info/SOURCES.txt` & `hspylib-1.12.37/hspylib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 hspylib/core/constants.py
 hspylib/core/namespace.py
 hspylib/core/preconditions.py
 hspylib/core/zoned_datetime.py
 hspylib/core/config/__init__.py
 hspylib/core/config/app_config.py
 hspylib/core/config/parser_factory.py
+hspylib/core/config/path_object.py
 hspylib/core/config/properties.py
+hspylib/core/config/settings.py
 hspylib/core/decorator/__init__.py
 hspylib/core/decorator/decorators.py
 hspylib/core/enums/__init__.py
 hspylib/core/enums/charset.py
 hspylib/core/enums/content_type.py
 hspylib/core/enums/enumeration.py
 hspylib/core/enums/http_code.py
```

### Comparing `hspylib-1.12.36/setup.py` & `hspylib-1.12.37/setup.py`

 * *Files identical despite different names*

