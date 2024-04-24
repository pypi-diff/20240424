# Comparing `tmp/bugsnag-4.6.2.tar.gz` & `tmp/bugsnag-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugsnag-4.6.2.tar", last modified: Tue Mar  5 09:16:50 2024, max compression
+gzip compressed data, was "bugsnag-4.7.0.tar", last modified: Wed Apr 24 08:29:30 2024, max compression
```

## Comparing `bugsnag-4.6.2.tar` & `bugsnag-4.7.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.987995 bugsnag-4.6.2/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1050 2022-10-04 14:38:17.000000 bugsnag-4.6.2/LICENSE.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)     1312 2024-03-05 09:16:50.988075 bugsnag-4.6.2/PKG-INFO
--rw-r--r--   0 joe.haines   (504) staff       (20)     1975 2023-01-18 16:09:16.000000 bugsnag-4.6.2/README.md
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.983155 bugsnag-4.6.2/bugsnag/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1442 2023-11-15 08:51:17.000000 bugsnag-4.6.2/bugsnag/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     4743 2022-10-04 14:38:17.000000 bugsnag-4.6.2/bugsnag/asgi.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     3389 2023-08-16 11:10:44.000000 bugsnag-4.6.2/bugsnag/breadcrumbs.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.984090 bugsnag-4.6.2/bugsnag/celery/
--rw-r--r--   0 joe.haines   (504) staff       (20)      977 2023-09-05 09:37:24.000000 bugsnag-4.6.2/bugsnag/celery/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    11775 2023-11-17 09:10:29.000000 bugsnag-4.6.2/bugsnag/client.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    20429 2024-03-04 13:13:02.000000 bugsnag-4.6.2/bugsnag/configuration.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     1683 2023-11-15 08:51:17.000000 bugsnag-4.6.2/bugsnag/context.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5195 2024-03-04 13:13:02.000000 bugsnag-4.6.2/bugsnag/delivery.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.984521 bugsnag-4.6.2/bugsnag/django/
--rw-r--r--   0 joe.haines   (504) staff       (20)     3654 2023-09-01 09:33:43.000000 bugsnag-4.6.2/bugsnag/django/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     2087 2023-11-15 08:51:17.000000 bugsnag-4.6.2/bugsnag/django/middleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      114 2022-10-26 12:09:12.000000 bugsnag-4.6.2/bugsnag/django/utils.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      695 2022-10-04 14:38:17.000000 bugsnag-4.6.2/bugsnag/error.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    15503 2023-11-15 08:51:17.000000 bugsnag-4.6.2/bugsnag/event.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     2894 2023-11-15 08:51:17.000000 bugsnag-4.6.2/bugsnag/feature_flags.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.984657 bugsnag-4.6.2/bugsnag/flask/
--rw-r--r--   0 joe.haines   (504) staff       (20)     2368 2023-12-11 08:33:38.000000 bugsnag-4.6.2/bugsnag/flask/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     6512 2023-08-09 13:05:44.000000 bugsnag-4.6.2/bugsnag/handlers.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5174 2023-11-15 08:51:17.000000 bugsnag-4.6.2/bugsnag/legacy.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     5336 2023-01-19 12:01:29.000000 bugsnag-4.6.2/bugsnag/middleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      464 2022-10-04 14:38:17.000000 bugsnag-4.6.2/bugsnag/notification.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      146 2024-03-04 13:14:13.000000 bugsnag-4.6.2/bugsnag/notifier.py
--rw-r--r--   0 joe.haines   (504) staff       (20)        0 2022-10-04 14:38:17.000000 bugsnag-4.6.2/bugsnag/py.typed
--rw-r--r--   0 joe.haines   (504) staff       (20)     5095 2024-03-04 13:13:02.000000 bugsnag-4.6.2/bugsnag/sessiontracker.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.984802 bugsnag-4.6.2/bugsnag/tornado/
--rw-r--r--   0 joe.haines   (504) staff       (20)     5900 2023-11-15 08:51:17.000000 bugsnag-4.6.2/bugsnag/tornado/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    15227 2023-12-11 08:33:38.000000 bugsnag-4.6.2/bugsnag/utils.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     1096 2022-10-04 14:38:17.000000 bugsnag-4.6.2/bugsnag/uwsgi.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.985114 bugsnag-4.6.2/bugsnag/wsgi/
--rw-r--r--   0 joe.haines   (504) staff       (20)      147 2022-10-04 14:38:17.000000 bugsnag-4.6.2/bugsnag/wsgi/__init__.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     3822 2023-11-15 08:51:17.000000 bugsnag-4.6.2/bugsnag/wsgi/middleware.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.983946 bugsnag-4.6.2/bugsnag.egg-info/
--rw-r--r--   0 joe.haines   (504) staff       (20)     1312 2024-03-05 09:16:50.000000 bugsnag-4.6.2/bugsnag.egg-info/PKG-INFO
--rw-r--r--   0 joe.haines   (504) staff       (20)     1221 2024-03-05 09:16:50.000000 bugsnag-4.6.2/bugsnag.egg-info/SOURCES.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)        1 2024-03-05 09:16:50.000000 bugsnag-4.6.2/bugsnag.egg-info/dependency_links.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)       29 2024-03-05 09:16:50.000000 bugsnag-4.6.2/bugsnag.egg-info/requires.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)        8 2024-03-05 09:16:50.000000 bugsnag-4.6.2/bugsnag.egg-info/top_level.txt
--rw-r--r--   0 joe.haines   (504) staff       (20)       76 2024-03-05 09:16:50.988303 bugsnag-4.6.2/setup.cfg
--rwxr-xr-x   0 joe.haines   (504) staff       (20)     1653 2024-03-04 13:14:09.000000 bugsnag-4.6.2/setup.py
-drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-03-05 09:16:50.987845 bugsnag-4.6.2/tests/
--rw-r--r--   0 joe.haines   (504) staff       (20)    11758 2023-11-15 08:51:17.000000 bugsnag-4.6.2/tests/test_breadcrumbs.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    56434 2023-12-11 08:33:38.000000 bugsnag-4.6.2/tests/test_client.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    24428 2024-03-04 13:13:02.000000 bugsnag-4.6.2/tests/test_configuration.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     4141 2023-11-15 08:51:17.000000 bugsnag-4.6.2/tests/test_context.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     2350 2024-01-23 16:19:51.000000 bugsnag-4.6.2/tests/test_delivery.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    18688 2023-11-15 08:51:17.000000 bugsnag-4.6.2/tests/test_event.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    14774 2023-12-11 08:33:38.000000 bugsnag-4.6.2/tests/test_exception_groups.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    10736 2023-11-15 08:51:17.000000 bugsnag-4.6.2/tests/test_feature_flags.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    24308 2023-12-11 08:33:38.000000 bugsnag-4.6.2/tests/test_handlers.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     4539 2022-11-02 11:51:55.000000 bugsnag-4.6.2/tests/test_middleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      777 2022-10-04 14:38:17.000000 bugsnag-4.6.2/tests/test_notification.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    36483 2023-12-11 08:33:38.000000 bugsnag-4.6.2/tests/test_notify.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     3255 2022-10-04 14:38:17.000000 bugsnag-4.6.2/tests/test_path_encoding.py
--rw-r--r--   0 joe.haines   (504) staff       (20)      477 2022-10-04 14:38:17.000000 bugsnag-4.6.2/tests/test_request_config.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     2200 2022-10-04 14:38:17.000000 bugsnag-4.6.2/tests/test_sessionmiddleware.py
--rw-r--r--   0 joe.haines   (504) staff       (20)     6154 2023-12-11 08:33:38.000000 bugsnag-4.6.2/tests/test_sessiontracker.py
--rw-r--r--   0 joe.haines   (504) staff       (20)    22469 2023-11-16 15:02:21.000000 bugsnag-4.6.2/tests/test_utils.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.049447 bugsnag-4.7.0/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1050 2022-10-04 14:38:17.000000 bugsnag-4.7.0/LICENSE.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1363 2024-04-24 08:29:30.049516 bugsnag-4.7.0/PKG-INFO
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2025 2024-04-24 08:25:03.000000 bugsnag-4.7.0/README.md
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.041028 bugsnag-4.7.0/bugsnag/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1523 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4743 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/asgi.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3389 2023-08-16 11:10:44.000000 bugsnag-4.7.0/bugsnag/breadcrumbs.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.042321 bugsnag-4.7.0/bugsnag/celery/
+-rw-r--r--   0 joe.haines   (504) staff       (20)      977 2024-04-22 09:23:08.000000 bugsnag-4.7.0/bugsnag/celery/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    18533 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/client.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    20568 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/configuration.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1683 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/context.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5809 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/delivery.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.043273 bugsnag-4.7.0/bugsnag/django/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3654 2023-09-01 09:33:43.000000 bugsnag-4.7.0/bugsnag/django/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2087 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/django/middleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      114 2022-10-26 12:09:12.000000 bugsnag-4.7.0/bugsnag/django/utils.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      695 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/error.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    15555 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/event.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2894 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/feature_flags.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.043552 bugsnag-4.7.0/bugsnag/flask/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2368 2023-12-11 08:33:38.000000 bugsnag-4.7.0/bugsnag/flask/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     6512 2023-08-09 13:05:44.000000 bugsnag-4.7.0/bugsnag/handlers.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5271 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/legacy.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5336 2023-01-19 12:01:29.000000 bugsnag-4.7.0/bugsnag/middleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      464 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/notification.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      146 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/notifier.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)        0 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/py.typed
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1533 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/request_tracker.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5628 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/sessiontracker.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.043821 bugsnag-4.7.0/bugsnag/tornado/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     5900 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/tornado/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    15245 2024-04-24 08:25:03.000000 bugsnag-4.7.0/bugsnag/utils.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1096 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/uwsgi.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.044325 bugsnag-4.7.0/bugsnag/wsgi/
+-rw-r--r--   0 joe.haines   (504) staff       (20)      147 2022-10-04 14:38:17.000000 bugsnag-4.7.0/bugsnag/wsgi/__init__.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3822 2023-11-15 08:51:17.000000 bugsnag-4.7.0/bugsnag/wsgi/middleware.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.042155 bugsnag-4.7.0/bugsnag.egg-info/
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1363 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/PKG-INFO
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1278 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/SOURCES.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)        1 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/dependency_links.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)       29 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/requires.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)        8 2024-04-24 08:29:30.000000 bugsnag-4.7.0/bugsnag.egg-info/top_level.txt
+-rw-r--r--   0 joe.haines   (504) staff       (20)       76 2024-04-24 08:29:30.049744 bugsnag-4.7.0/setup.cfg
+-rwxr-xr-x   0 joe.haines   (504) staff       (20)     1703 2024-04-24 08:25:03.000000 bugsnag-4.7.0/setup.py
+drwxr-xr-x   0 joe.haines   (504) staff       (20)        0 2024-04-24 08:29:30.049060 bugsnag-4.7.0/tests/
+-rw-r--r--   0 joe.haines   (504) staff       (20)    11758 2023-11-15 08:51:17.000000 bugsnag-4.7.0/tests/test_breadcrumbs.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    68059 2024-04-24 08:25:03.000000 bugsnag-4.7.0/tests/test_client.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    24428 2024-03-05 09:31:55.000000 bugsnag-4.7.0/tests/test_configuration.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4141 2023-11-15 08:51:17.000000 bugsnag-4.7.0/tests/test_context.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     6259 2024-04-24 08:25:03.000000 bugsnag-4.7.0/tests/test_delivery.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    18688 2023-11-15 08:51:17.000000 bugsnag-4.7.0/tests/test_event.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    14774 2023-12-11 08:33:38.000000 bugsnag-4.7.0/tests/test_exception_groups.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    10736 2023-11-15 08:51:17.000000 bugsnag-4.7.0/tests/test_feature_flags.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    24308 2023-12-11 08:33:38.000000 bugsnag-4.7.0/tests/test_handlers.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     4539 2022-11-02 11:51:55.000000 bugsnag-4.7.0/tests/test_middleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      777 2022-10-04 14:38:17.000000 bugsnag-4.7.0/tests/test_notification.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    36483 2023-12-11 08:33:38.000000 bugsnag-4.7.0/tests/test_notify.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     3255 2022-10-04 14:38:17.000000 bugsnag-4.7.0/tests/test_path_encoding.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)      477 2022-10-04 14:38:17.000000 bugsnag-4.7.0/tests/test_request_config.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     1509 2024-04-24 08:25:03.000000 bugsnag-4.7.0/tests/test_request_tracker.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     2200 2022-10-04 14:38:17.000000 bugsnag-4.7.0/tests/test_sessionmiddleware.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)     7408 2024-04-24 08:25:03.000000 bugsnag-4.7.0/tests/test_sessiontracker.py
+-rw-r--r--   0 joe.haines   (504) staff       (20)    22469 2023-11-16 15:02:21.000000 bugsnag-4.7.0/tests/test_utils.py
```

### Comparing `bugsnag-4.6.2/LICENSE.txt` & `bugsnag-4.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/PKG-INFO` & `bugsnag-4.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugsnag
-Version: 4.6.2
+Version: 4.7.0
 Summary: Automatic error monitoring for django, flask, etc.
 Home-page: https://bugsnag.com/
 Author: Simon Maynard
 Author-email: simon@bugsnag.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Requires-Python: >=3.5, <4
 Provides-Extra: flask
 License-File: LICENSE.txt
 
 
 Bugsnag
```

### Comparing `bugsnag-4.6.2/README.md` & `bugsnag-4.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # Bugsnag exception reporter for Python
 [![Build status](https://img.shields.io/travis/bugsnag/bugsnag-python/master.svg?style=flat-square)](https://travis-ci.com/bugsnag/bugsnag-python)
 [![Documentation](https://img.shields.io/badge/documentation-latest-blue.svg)](https://docs.bugsnag.com/platforms/python/)
 
-The Bugsnag exception reporter for Python automatically detects and reports
-exceptions thrown your **Django**, **WSGI**, **Tornado**, **Flask** or
-**plain Python** app.  Any uncaught exceptions will trigger a notification to be
-sent to your Bugsnag project. Learn more about [monitoring and reporting Python errors](https://www.bugsnag.com/platforms/python-error-reporting/) with Bugsnag.
+The Bugsnag exception reporter for Python automatically detects and reports exceptions thrown your **ASGI**, **AWS Lambda**, **Bottle**, **Celery**, **Django**, **Flask**, **Tornado**, **WSGI** or **plain Python** app.  Any uncaught exceptions will trigger a notification to be sent to your Bugsnag project. Learn more about [monitoring and reporting Python errors](https://www.bugsnag.com/platforms/python-error-reporting/) with Bugsnag.
 
 
 ## Features
 
 * Automatically report unhandled exceptions and crashes
 * Report handled exceptions
 * Attach user information and custom diagnostic data to determine how many
```

### Comparing `bugsnag-4.6.2/bugsnag/__init__.py` & `bugsnag-4.7.0/bugsnag/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 from bugsnag.feature_flags import FeatureFlag
 from bugsnag.legacy import (configuration, configure, configure_request,
                             add_metadata_tab, clear_request_config, notify,
                             auto_notify, before_notify, start_session,
                             auto_notify_exc_info, logger, leave_breadcrumb,
                             add_on_breadcrumb, remove_on_breadcrumb,
                             add_feature_flag, add_feature_flags,
-                            clear_feature_flag, clear_feature_flags)
+                            clear_feature_flag, clear_feature_flags,
+                            aws_lambda_handler)
 
 __all__ = ('Client', 'Event', 'Configuration', 'RequestConfiguration',
            'configuration', 'configure', 'configure_request',
            'add_metadata_tab', 'clear_request_config', 'notify',
            'auto_notify', 'before_notify', 'start_session',
            'auto_notify_exc_info', 'Notification', 'logger',
            'BreadcrumbType', 'Breadcrumb', 'Breadcrumbs',
            'OnBreadcrumbCallback', 'leave_breadcrumb', 'add_on_breadcrumb',
            'remove_on_breadcrumb', 'FeatureFlag', 'add_feature_flag',
-           'add_feature_flags', 'clear_feature_flag', 'clear_feature_flags')
+           'add_feature_flags', 'clear_feature_flag', 'clear_feature_flags',
+           'aws_lambda_handler')
```

### Comparing `bugsnag-4.6.2/bugsnag/asgi.py` & `bugsnag-4.7.0/bugsnag/asgi.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/breadcrumbs.py` & `bugsnag-4.7.0/bugsnag/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/celery/__init__.py` & `bugsnag-4.7.0/bugsnag/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/configuration.py` & `bugsnag-4.7.0/bugsnag/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -600,14 +600,18 @@
         if instance is None:
             instance = RequestConfiguration()
             _request_info.set(instance)  # type: ignore
 
         return instance
 
     @classmethod
+    def set_instance(cls, instance: 'RequestConfiguration') -> None:
+        _request_info.set(instance)  # type: ignore
+
+    @classmethod
     def clear(cls):
         """
         Clear this thread's instance of the RequestConfiguration.
         """
         _request_info.set(None)
 
     def __init__(self):
```

### Comparing `bugsnag-4.6.2/bugsnag/context.py` & `bugsnag-4.7.0/bugsnag/context.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/delivery.py` & `bugsnag-4.7.0/bugsnag/delivery.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,31 @@
 
 DEFAULT_ENDPOINT = 'https://notify.bugsnag.com'
 DEFAULT_SESSIONS_ENDPOINT = 'https://sessions.bugsnag.com'
 
 __all__ = ('default_headers', 'Delivery')
 
 
+def _noop():
+    pass
+
+
+def _marshall_post_delivery_callback(post_delivery_callback):
+    if not callable(post_delivery_callback):
+        return _noop
+
+    def safe_post_delivery_callback():
+        try:
+            post_delivery_callback()
+        except Exception:
+            pass
+
+    return safe_post_delivery_callback
+
+
 def create_default_delivery():
     if requests is not None:
         return RequestsDelivery()
 
     return UrllibDelivery()
 
 
@@ -77,28 +94,37 @@
 
             options['endpoint'] = config.session_endpoint
             options['success'] = 202
 
             self.deliver(config, payload, options)
 
     def queue_request(self, request: Callable, config, options: Dict):
+        post_delivery_callback = _marshall_post_delivery_callback(
+            options.pop('post_delivery_callback', None)
+        )
+
         if config.asynchronous and options.pop('asynchronous', True):
             # if an exception escapes the thread, our threading.excepthook
             # will catch it and attempt to deliver it
             # this will cause an infinite loop if delivery can never succeed,
             # e.g. because the URL is unreachable
             def safe_request():
                 try:
                     request()
                 except Exception as e:
                     config.logger.exception('Notifying Bugsnag failed %s', e)
+                finally:
+                    post_delivery_callback()
 
             Thread(target=safe_request).start()
         else:
-            request()
+            try:
+                request()
+            finally:
+                post_delivery_callback()
 
 
 class UrllibDelivery(Delivery):
     def deliver(self, config, payload: Any, options=None):
         if options is None:
             options = {}
```

### Comparing `bugsnag-4.6.2/bugsnag/django/__init__.py` & `bugsnag-4.7.0/bugsnag/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/django/middleware.py` & `bugsnag-4.7.0/bugsnag/django/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/error.py` & `bugsnag-4.7.0/bugsnag/error.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/event.py` & `bugsnag-4.7.0/bugsnag/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,14 +432,15 @@
             keyword_filters=self.config.params_filters
         )
 
         # Construct the payload dictionary
         return encoder.encode({
             "apiKey": self.api_key,
             "notifier": _NOTIFIER_INFORMATION,
+            "payloadVersion": self.PAYLOAD_VERSION,
             "events": [{
                 "severity": self.severity,
                 "severityReason": self.severity_reason,
                 "unhandled": self.unhandled,
                 "releaseStage": self.release_stage,
                 "app": {
                     "version": self.app_version,
```

### Comparing `bugsnag-4.6.2/bugsnag/feature_flags.py` & `bugsnag-4.7.0/bugsnag/feature_flags.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/flask/__init__.py` & `bugsnag-4.7.0/bugsnag/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/handlers.py` & `bugsnag-4.7.0/bugsnag/handlers.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/legacy.py` & `bugsnag-4.7.0/bugsnag/legacy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Any, Tuple, Type, Optional, Union, List
+from typing import Dict, Any, Tuple, Type, Optional, Union, List, Callable
 import types
 import sys
 
 from bugsnag.breadcrumbs import BreadcrumbType, OnBreadcrumbCallback
 from bugsnag.feature_flags import FeatureFlag
 from bugsnag.configuration import RequestConfiguration
 from bugsnag.client import Client
@@ -34,19 +34,15 @@
 
 def add_metadata_tab(tab_name: str, data: Dict[str, Any]):
     """
     Add metaData to the tab
 
     bugsnag.add_metadata_tab("user", {"id": "1", "name": "Conrad"})
     """
-    metadata = RequestConfiguration.get_instance().metadata
-    if tab_name not in metadata:
-        metadata[tab_name] = {}
-
-    metadata[tab_name].update(data)
+    default_client.add_metadata_tab(tab_name, data)
 
 
 def clear_request_config():
     """
     Clears the per-request settings.
     """
     RequestConfiguration.clear()
@@ -176,7 +172,14 @@
 
 def clear_feature_flag(name: Union[str, bytes]) -> None:
     default_client.clear_feature_flag(name)
 
 
 def clear_feature_flags() -> None:
     default_client.clear_feature_flags()
+
+
+def aws_lambda_handler(
+    real_handler: Optional[Callable] = None,
+    flush_timeout_ms: int = 2000,
+) -> Callable:
+    return default_client.aws_lambda_handler(real_handler, flush_timeout_ms)
```

### Comparing `bugsnag-4.6.2/bugsnag/middleware.py` & `bugsnag-4.7.0/bugsnag/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/sessiontracker.py` & `bugsnag-4.7.0/bugsnag/sessiontracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from bugsnag.utils import ThreadContextVar
     # flake8: noqa
     _session_info = ThreadContextVar('bugsnag-session', default={})  # type: ignore
 
 from bugsnag.notifier import _NOTIFIER_INFORMATION
 from bugsnag.utils import FilterDict, SanitizingJSONEncoder
 from bugsnag.event import Event
+from bugsnag.request_tracker import RequestTracker
 
 
 __all__ = []  # type: List[str]
 
 
 class SessionTracker:
 
@@ -32,14 +33,15 @@
 
     def __init__(self, configuration):
         self.session_counts = {}  # type: Dict[str, int]
         self.config = configuration
         self.mutex = Lock()
         self.auto_sessions = False
         self.delivery_thread = None
+        self._request_tracker = RequestTracker()
 
     def start_session(self):
         if not self.auto_sessions:
             self.auto_sessions = True
             self.__start_delivery()
 
         start_time = strftime('%Y-%m-%dT%H:%M:00', gmtime())
@@ -134,23 +136,33 @@
             )
 
             encoded_payload = encoder.encode(payload)
 
             deliver = self.config.delivery.deliver_sessions
 
             if 'options' in deliver.__code__.co_varnames:
-                deliver(
-                    self.config,
-                    encoded_payload,
-                    options={'asynchronous': asynchronous}
-                )
+                try:
+                    post_delivery_callback = self._request_tracker.new_request()
+
+                    deliver(
+                        self.config,
+                        encoded_payload,
+                        options={
+                            'asynchronous': asynchronous,
+                            'post_delivery_callback': post_delivery_callback,
+                        }
+                    )
+                except Exception:
+                    # ensure the request is not still marked as pending
+                    post_delivery_callback()
+                    raise
+
             else:
                 deliver(self.config, encoded_payload)
 
-
         except Exception as e:
             self.config.logger.exception('Sending sessions failed %s', e)
 
 
 class SessionMiddleware:
     """
     Session middleware ensures that a session is appended to the event.
```

### Comparing `bugsnag-4.6.2/bugsnag/tornado/__init__.py` & `bugsnag-4.7.0/bugsnag/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/utils.py` & `bugsnag-4.7.0/bugsnag/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     >>> is_json_content_type('application/json')
     True
     """
     type, subtype, suffix, _ = parse_content_type(value.lower())
     return type == 'application' and (subtype == 'json' or suffix == 'json')
 
 
-_ignore_modules = ('__main__', 'builtins')
+_ignore_modules = ('__main__', 'builtins', 'bugsnag.client')
 
 
 def partly_qualified_class_name(obj):
     module = inspect.getmodule(obj)
 
     if module is None or module.__name__ in _ignore_modules:
         return obj.__class__.__name__
```

### Comparing `bugsnag-4.6.2/bugsnag/uwsgi.py` & `bugsnag-4.7.0/bugsnag/uwsgi.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag/wsgi/middleware.py` & `bugsnag-4.7.0/bugsnag/wsgi/middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/bugsnag.egg-info/PKG-INFO` & `bugsnag-4.7.0/bugsnag.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugsnag
-Version: 4.6.2
+Version: 4.7.0
 Summary: Automatic error monitoring for django, flask, etc.
 Home-page: https://bugsnag.com/
 Author: Simon Maynard
 Author-email: simon@bugsnag.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Requires-Python: >=3.5, <4
 Provides-Extra: flask
 License-File: LICENSE.txt
 
 
 Bugsnag
```

### Comparing `bugsnag-4.6.2/bugsnag.egg-info/SOURCES.txt` & `bugsnag-4.7.0/bugsnag.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 bugsnag/feature_flags.py
 bugsnag/handlers.py
 bugsnag/legacy.py
 bugsnag/middleware.py
 bugsnag/notification.py
 bugsnag/notifier.py
 bugsnag/py.typed
+bugsnag/request_tracker.py
 bugsnag/sessiontracker.py
 bugsnag/utils.py
 bugsnag/uwsgi.py
 bugsnag.egg-info/PKG-INFO
 bugsnag.egg-info/SOURCES.txt
 bugsnag.egg-info/dependency_links.txt
 bugsnag.egg-info/requires.txt
@@ -44,10 +45,11 @@
 tests/test_feature_flags.py
 tests/test_handlers.py
 tests/test_middleware.py
 tests/test_notification.py
 tests/test_notify.py
 tests/test_path_encoding.py
 tests/test_request_config.py
+tests/test_request_tracker.py
 tests/test_sessionmiddleware.py
 tests/test_sessiontracker.py
 tests/test_utils.py
```

### Comparing `bugsnag-4.6.2/setup.py` & `bugsnag-4.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 and solve your bugs as fast as possible.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='bugsnag',
-    version='4.6.2',
+    version='4.7.0',
     description='Automatic error monitoring for django, flask, etc.',
     long_description=__doc__,
     author='Simon Maynard',
     author_email='simon@bugsnag.com',
     url='https://bugsnag.com/',
     license='MIT',
     python_requires='>=3.5, <4',
@@ -35,14 +35,15 @@
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Software Development'
     ],
     package_data={
         'bugsnag': ['py.typed'],
     },
     test_suite='tests',
     install_requires=['webob'],
```

### Comparing `bugsnag-4.6.2/tests/test_breadcrumbs.py` & `bugsnag-4.7.0/tests/test_breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_client.py` & `bugsnag-4.7.0/tests/test_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import os
 import re
 import sys
+import time
 import pytest
 import inspect
 import logging
+import threading
 from datetime import datetime, timedelta, timezone
 from unittest.mock import Mock, ANY
 from tests import fixtures
 
 from bugsnag import (
     Client,
     Configuration,
     BreadcrumbType,
     Breadcrumb,
     FeatureFlag
 )
 
 import bugsnag.legacy as legacy
-from tests.utils import IntegrationTest, ScaryException
+from tests.utils import (
+    BrokenDelivery,
+    IntegrationTest,
+    QueueingDelivery,
+    ScaryException,
+)
 
 timestamp_regex = r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{3}(?:[+-]\d{2}:\d{2}|Z)'  # noqa: E501
 
 
 def is_valid_timestamp(timestamp: str) -> bool:
     return bool(re.search(timestamp_regex, timestamp))
 
@@ -1684,14 +1691,300 @@
         assert self.client.feature_flags == [
             FeatureFlag('a', '1'),
             FeatureFlag('b'),
             FeatureFlag('c', '3'),
             FeatureFlag('e')
         ]
 
+    def test_in_flight_event_request_tracking_in_notify(self):
+        delivery = QueueingDelivery()
+        configuration = Configuration()
+        configuration.configure(delivery=delivery, api_key='abc')
+
+        client = Client(configuration)
+        assert not client._request_tracker.has_in_flight_requests()
+
+        client.notify(Exception('Oh no'))
+        assert client._request_tracker.has_in_flight_requests()
+
+        delivery.flush_request_queue()
+        assert not client._request_tracker.has_in_flight_requests()
+
+    def test_in_flight_event_request_tracking_in_notify_failure(self):
+        configuration = Configuration()
+        configuration.configure(delivery=BrokenDelivery(), api_key='abc')
+
+        client = Client(configuration)
+        assert not client._request_tracker.has_in_flight_requests()
+
+        client.notify(Exception('Oh no'))
+        assert not client._request_tracker.has_in_flight_requests()
+
+    def test_in_flight_event_request_tracking_in_notify_exc_info(self):
+        delivery = QueueingDelivery()
+        configuration = Configuration()
+        configuration.configure(delivery=delivery, api_key='abc')
+
+        client = Client(configuration)
+        assert not client._request_tracker.has_in_flight_requests()
+
+        try:
+            raise Exception(':)')
+        except Exception:
+            client.notify_exc_info(*sys.exc_info())
+
+        assert client._request_tracker.has_in_flight_requests()
+
+        delivery.flush_request_queue()
+        assert not client._request_tracker.has_in_flight_requests()
+
+    def test_in_flight_event_request_tracking_in_notify_exc_info_failure(self):
+        configuration = Configuration()
+        configuration.configure(delivery=BrokenDelivery(), api_key='abc')
+
+        client = Client(configuration)
+        assert not client._request_tracker.has_in_flight_requests()
+
+        try:
+            raise Exception(':)')
+        except Exception:
+            client.notify_exc_info(*sys.exc_info())
+
+        assert not client._request_tracker.has_in_flight_requests()
+
+    def test_flush_returns_immediately_when_no_requests_are_outstanding(self):
+        start_s = time.time()
+        self.client.flush(10)
+        end_s = time.time()
+
+        assert end_s - start_s < 0.01
+
+    def test_flush_raises_if_timeout_is_exceeded(self):
+        delivery = QueueingDelivery()
+        configuration = Configuration()
+        configuration.configure(delivery=delivery, api_key='abc')
+
+        client = Client(configuration)
+        client.notify(Exception('oh dear'))
+
+        with pytest.raises(Exception) as exception:
+            client.flush(10)
+
+            assert str(exception) == 'Exception: flush timed out after 10ms'
+
+    def test_flush_waits_for_outstanding_events_before_returning(self):
+        delivery = QueueingDelivery()
+        configuration = Configuration()
+        configuration.configure(delivery=delivery, api_key='abc')
+
+        client = Client(configuration)
+        client.notify(Exception('oh dear'))
+        client.notify(Exception('oh no'))
+        client.notify(Exception('oh my'))
+
+        def flush_request_queue():
+            time.sleep(0.05)
+            assert client._request_tracker.has_in_flight_requests()
+
+            delivery.flush_request_queue()
+            assert not client._request_tracker.has_in_flight_requests()
+
+        thread = threading.Thread(target=flush_request_queue)
+        thread.start()
+
+        client.flush(100)
+
+        # the thread should have stopped before flush could exit
+        assert not thread.is_alive()
+
+    def test_flush_waits_for_outstanding_sessions_before_returning(self):
+        delivery = QueueingDelivery()
+        configuration = Configuration()
+        configuration.configure(delivery=delivery, api_key='abc')
+
+        client = Client(configuration)
+        client.session_tracker.start_session()
+        client.session_tracker.start_session()
+
+        def flush_request_queue():
+            request_tracker = client.session_tracker._request_tracker
+
+            time.sleep(0.05)
+            assert request_tracker.has_in_flight_requests()
+
+            delivery.flush_request_queue()
+            assert not request_tracker.has_in_flight_requests()
+
+        thread = threading.Thread(target=flush_request_queue)
+        thread.start()
+
+        client.flush(100)
+
+        # the thread should have stopped before flush could exit
+        assert not thread.is_alive()
+
+    def test_aws_lambda_handler_decorator(self):
+        aws_lambda_context = LambdaContext(function_name='abcdef')
+
+        @self.client.aws_lambda_handler
+        def my_handler(event, context):
+            assert event == {'a': 1}
+            assert context == aws_lambda_context
+
+            raise Exception('oh dear')
+
+        with pytest.raises(Exception) as exception:
+            my_handler({'a': 1}, aws_lambda_context)
+
+            assert str(exception) == 'Exception: oh dear'
+
+        assert self.sent_report_count == 1
+        assert self.sent_session_count == 1
+
+        payload = self.server.events_received[0]['json_body']
+        event = payload['events'][0]
+
+        assert event['unhandled']
+        assert event['exceptions'][0]['message'] == 'oh dear'
+        assert event['metaData']['AWS Lambda Event'] == {'a': 1}
+        assert event['metaData']['AWS Lambda Context'] == {
+            'function_name': 'abcdef',
+            'function_version': 'function_version',
+            'invoked_function_arn': 'invoked_function_arn',
+            'memory_limit_in_mb': 'memory_limit_in_mb',
+            'aws_request_id': 'aws_request_id',
+            'log_group_name': 'log_group_name',
+            'log_stream_name': 'log_stream_name',
+            'identity': 'identity',
+            'client_context': 'client_context',
+        }
+
+    def test_aws_lambda_handler_decorator_accepts_flush_timeout(self):
+        aws_lambda_context = LambdaContext(function_version='$LATEST')
+
+        @self.client.aws_lambda_handler(flush_timeout_ms=1000)
+        def my_handler(event, context):
+            assert event == {'z': 9}
+            assert context == aws_lambda_context
+
+            raise Exception('oh dear')
+
+        with pytest.raises(Exception) as exception:
+            my_handler({'z': 9}, aws_lambda_context)
+
+            assert str(exception) == 'Exception: oh dear'
+
+        assert self.sent_report_count == 1
+        assert self.sent_session_count == 1
+
+        payload = self.server.events_received[0]['json_body']
+        event = payload['events'][0]
+
+        assert event['unhandled']
+        assert event['exceptions'][0]['message'] == 'oh dear'
+        assert event['metaData']['AWS Lambda Event'] == {'z': 9}
+        assert event['metaData']['AWS Lambda Context'] == {
+            'function_name': 'function_name',
+            'function_version': '$LATEST',
+            'invoked_function_arn': 'invoked_function_arn',
+            'memory_limit_in_mb': 'memory_limit_in_mb',
+            'aws_request_id': 'aws_request_id',
+            'log_group_name': 'log_group_name',
+            'log_stream_name': 'log_stream_name',
+            'identity': 'identity',
+            'client_context': 'client_context',
+        }
+
+    def test_aws_lambda_handler_decorator_warns_after_timeout(self):
+        aws_lambda_context = LambdaContext()
+        client = Client(delivery=QueueingDelivery(), api_key='abc')
+
+        @client.aws_lambda_handler(flush_timeout_ms=50)
+        def my_handler(event, context):
+            assert event == {'z': 9}
+            assert context == aws_lambda_context
+
+            raise Exception('oh dear')
+
+        with pytest.warns(UserWarning) as warnings:
+            with pytest.raises(Exception) as exception:
+                my_handler({'z': 9}, aws_lambda_context)
+
+                assert str(exception) == 'Exception: oh dear'
+
+            assert len(warnings) == 1
+            assert warnings[0].message.args[0] == \
+                'Delivery may be unsuccessful: flush timed out after 50ms'
+
+        assert self.sent_report_count == 0
+        assert self.sent_session_count == 0
+
+    def test_aws_lambda_handler_decorator_warns_of_potential_timeout(self):
+        aws_lambda_context = LambdaContext(remaining_time_in_millis=2)
+
+        @self.client.aws_lambda_handler(lambda_timeout_notify_ms=1)
+        def my_handler(event, context):
+            assert event == {'z': 9}
+            assert context == aws_lambda_context
+
+            self.client.leave_breadcrumb('hello 1')
+            self.client.leave_breadcrumb('hello 2')
+            self.client.leave_breadcrumb('hello 3')
+
+            self.client.add_feature_flag('a')
+            self.client.add_feature_flag('b', '1')
+            self.client.add_feature_flag('c')
+
+            time.sleep(0.1)
+
+        my_handler({'z': 9}, aws_lambda_context)
+
+        assert self.sent_report_count == 1
+        assert self.sent_session_count == 1
+
+        payload = self.server.events_received[0]['json_body']
+        event = payload['events'][0]
+
+        assert event['metaData']['AWS Lambda Event'] == {'z': 9}
+        assert event['metaData']['AWS Lambda Context'] == {
+            'function_name': 'function_name',
+            'function_version': 'function_version',
+            'invoked_function_arn': 'invoked_function_arn',
+            'memory_limit_in_mb': 'memory_limit_in_mb',
+            'aws_request_id': 'aws_request_id',
+            'log_group_name': 'log_group_name',
+            'log_stream_name': 'log_stream_name',
+            'identity': 'identity',
+            'client_context': 'client_context',
+        }
+
+        assert len(event['breadcrumbs']) == 3
+        assert event['breadcrumbs'][0]['name'] == 'hello 1'
+        assert event['breadcrumbs'][1]['name'] == 'hello 2'
+        assert event['breadcrumbs'][2]['name'] == 'hello 3'
+
+        assert event['featureFlags'] == [
+            {'featureFlag': 'a'},
+            {'featureFlag': 'b', 'variant': '1'},
+            {'featureFlag': 'c'},
+        ]
+
+        exception = event['exceptions'][0]
+
+        assert exception['message'] == 'Lambda will timeout in 2ms'
+        assert exception['errorClass'] == 'LambdaTimeoutApproaching'
+
+        # the stacktrace should have a single frame pointing to the user's
+        # lambda handler
+        stacktrace = exception['stacktrace']
+
+        assert len(stacktrace) == 1
+        assert stacktrace[0]['file'] == 'test_client.py'
+        assert stacktrace[0]['method'] == 'my_handler'
+
 
 @pytest.mark.parametrize("metadata,type", [
     (1234, 'int'),
     ('abc', 'str'),
     ([1, 2, 3], 'list'),
     (True, 'bool'),
     (False, 'bool'),
@@ -1714,7 +2007,37 @@
 
     breadcrumb = client.configuration.breadcrumbs[0]
 
     assert breadcrumb.message == 'abcxyz'
     assert breadcrumb.metadata == {}
     assert breadcrumb.type == BreadcrumbType.MANUAL
     assert is_valid_timestamp(breadcrumb.timestamp)
+
+
+class LambdaContext:
+    def __init__(
+        self,
+        function_name='function_name',
+        function_version='function_version',
+        invoked_function_arn='invoked_function_arn',
+        memory_limit_in_mb='memory_limit_in_mb',
+        aws_request_id='aws_request_id',
+        log_group_name='log_group_name',
+        log_stream_name='log_stream_name',
+        identity='identity',
+        client_context='client_context',
+        remaining_time_in_millis=10000
+    ):
+        self.function_name = function_name
+        self.function_version = function_version
+        self.invoked_function_arn = invoked_function_arn
+        self.memory_limit_in_mb = memory_limit_in_mb
+        self.aws_request_id = aws_request_id
+        self.log_group_name = log_group_name
+        self.log_stream_name = log_stream_name
+        self.identity = identity
+        self.client_context = client_context
+        self.another_attribute = 'another_attribute'
+        self.remaining_time_in_millis = remaining_time_in_millis
+
+    def get_remaining_time_in_millis(self) -> int:
+        return self.remaining_time_in_millis
```

### Comparing `bugsnag-4.6.2/tests/test_configuration.py` & `bugsnag-4.7.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_context.py` & `bugsnag-4.7.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_event.py` & `bugsnag-4.7.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_exception_groups.py` & `bugsnag-4.7.0/tests/test_exception_groups.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_feature_flags.py` & `bugsnag-4.7.0/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_handlers.py` & `bugsnag-4.7.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_middleware.py` & `bugsnag-4.7.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_notification.py` & `bugsnag-4.7.0/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_notify.py` & `bugsnag-4.7.0/tests/test_notify.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_path_encoding.py` & `bugsnag-4.7.0/tests/test_path_encoding.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_sessionmiddleware.py` & `bugsnag-4.7.0/tests/test_sessionmiddleware.py`

 * *Files identical despite different names*

### Comparing `bugsnag-4.6.2/tests/test_sessiontracker.py` & `bugsnag-4.7.0/tests/test_sessiontracker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import platform
 
 from bugsnag import Client
 from bugsnag.configuration import Configuration
 from bugsnag.notifier import _NOTIFIER_INFORMATION
 from bugsnag.sessiontracker import SessionTracker
-from tests.utils import IntegrationTest
+from tests.utils import BrokenDelivery, IntegrationTest, QueueingDelivery
 from unittest.mock import Mock
 
 
 def force_timer_to_fire(timer):
     assert timer is not None
 
     # setting and clearing the 'finished' Event forces the timer to fire
@@ -188,7 +188,41 @@
         client.session_tracker.start_session()
 
         force_timer_to_fire(client.session_tracker.delivery_thread)
 
         self.server.wait_for_session()
 
         assert self.server.sent_session_count == 1
+
+    def test_session_tracker_tracks_in_flight_requests(self):
+        delivery = QueueingDelivery()
+        client = Client(
+            api_key='a05afff2bd2ffaf0ab0f52715bbdcffd',
+            auto_capture_sessions=False,
+            session_endpoint=self.server.sessions_url,
+            asynchronous=False,
+            delivery=delivery,
+        )
+
+        client.session_tracker.start_session()
+        client.session_tracker.send_sessions()
+
+        request_tracker = client.session_tracker._request_tracker
+        assert request_tracker.has_in_flight_requests()
+
+        delivery.flush_request_queue()
+        assert not request_tracker.has_in_flight_requests()
+
+    def test_session_tracker_tracks_in_flight_requests_failure(self):
+        client = Client(
+            api_key='a05afff2bd2ffaf0ab0f52715bbdcffd',
+            auto_capture_sessions=False,
+            session_endpoint=self.server.sessions_url,
+            asynchronous=False,
+            delivery=BrokenDelivery(),
+        )
+
+        client.session_tracker.start_session()
+        client.session_tracker.send_sessions()
+
+        request_tracker = client.session_tracker._request_tracker
+        assert not request_tracker.has_in_flight_requests()
```

### Comparing `bugsnag-4.6.2/tests/test_utils.py` & `bugsnag-4.7.0/tests/test_utils.py`

 * *Files identical despite different names*

