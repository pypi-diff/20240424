# Comparing `tmp/social-auth-app-django-5.4.0.tar.gz` & `tmp/social-auth-app-django-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-auth-app-django-5.4.0.tar", last modified: Tue Oct 17 07:41:24 2023, max compression
+gzip compressed data, was "social-auth-app-django-5.4.1.tar", last modified: Wed Apr 24 17:22:32 2024, max compression
```

## Comparing `social-auth-app-django-5.4.0.tar` & `social-auth-app-django-5.4.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:24.227967 social-auth-app-django-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2023-10-17 07:41:24.227967 social-auth-app-django-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 07:41:24.227967 social-auth-app-django-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:24.223967 social-auth-app-django-5.4.0/social_auth_app_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2023-10-17 07:41:24.000000 social-auth-app-django-5.4.0/social_auth_app_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-10-17 07:41:24.000000 social-auth-app-django-5.4.0/social_auth_app_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 07:41:24.000000 social-auth-app-django-5.4.0/social_auth_app_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 07:41:24.000000 social-auth-app-django-5.4.0/social_auth_app_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-17 07:41:24.000000 social-auth-app-django-5.4.0/social_auth_app_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-17 07:41:24.000000 social-auth-app-django-5.4.0/social_auth_app_django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:24.223967 social-auth-app-django-5.4.0/social_django/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:24.223967 social-auth-app-django-5.4.0/social_django/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:24.223967 social-auth-app-django-5.4.0/social_django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/management/commands/clearsocial.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:24.227967 social-auth-app-django-5.4.0/social_django/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0002_add_related_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0003_alter_email_max_length.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0004_auto_20160423_0400.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0005_auto_20160727_2333.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0006_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0007_code_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0008_partial_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0009_auto_20191118_0520.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0010_uid_db_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0011_alter_id_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0012_usersocialauth_extra_data_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0013_migrate_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0014_remove_usersocialauth_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/0015_rename_extra_data_new_usersocialauth_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/social_django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:24.227967 social-auth-app-django-5.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/test_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-10-17 07:41:13.000000 social-auth-app-django-5.4.0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:32.757662 social-auth-app-django-5.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 17:22:32.757662 social-auth-app-django-5.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:22:32.757662 social-auth-app-django-5.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:32.749662 social-auth-app-django-5.4.1/social_auth_app_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 17:22:32.000000 social-auth-app-django-5.4.1/social_auth_app_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-24 17:22:32.000000 social-auth-app-django-5.4.1/social_auth_app_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:22:32.000000 social-auth-app-django-5.4.1/social_auth_app_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:22:32.000000 social-auth-app-django-5.4.1/social_auth_app_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 17:22:32.000000 social-auth-app-django-5.4.1/social_auth_app_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 17:22:32.000000 social-auth-app-django-5.4.1/social_auth_app_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:32.753661 social-auth-app-django-5.4.1/social_django/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:32.753661 social-auth-app-django-5.4.1/social_django/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:32.753661 social-auth-app-django-5.4.1/social_django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/management/commands/clearsocial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:32.757662 social-auth-app-django-5.4.1/social_django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0002_add_related_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0003_alter_email_max_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0004_auto_20160423_0400.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0005_auto_20160727_2333.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0006_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0007_code_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0008_partial_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0009_auto_20191118_0520.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0010_uid_db_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0011_alter_id_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0012_usersocialauth_extra_data_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0013_migrate_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0014_remove_usersocialauth_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/0015_rename_extra_data_new_usersocialauth_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/social_django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:32.757662 social-auth-app-django-5.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/test_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 17:22:24.000000 social-auth-app-django-5.4.1/tests/urls.py
```

### Comparing `social-auth-app-django-5.4.0/CHANGELOG.md` & `social-auth-app-django-5.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
+## [5.4.1](https://github.com/python-social-auth/social-app-django/releases/tag/5.4.1) - 2024-04-24
+
+### Changed
+- Added reverse migration for JSON field
+- Fixed improper handling of case sensitivity with MySQL/MariaDB (CVE-2024-32879)
+
 ## [5.4.0](https://github.com/python-social-auth/social-app-django/releases/tag/5.4.0) - 2023-10-17
 
 ### Changed
 - Improved JSON field migration performance
 - Introduce configuration to request POST only requests for social authentication
 - Updated list of supported Django and Python versions
```

### Comparing `social-auth-app-django-5.4.0/LICENSE` & `social-auth-app-django-5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/PKG-INFO` & `social-auth-app-django-5.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-app-django
-Version: 5.4.0
+Version: 5.4.1
 Summary: Python Social Authentication, Django integration.
 Home-page: https://github.com/python-social-auth/social-app-django
 Author: Matias Aguirre
 Author-email: matiasaguirre@gmail.com
 License: BSD
 Keywords: django,social auth
 Platform: UNKNOWN
```

### Comparing `social-auth-app-django-5.4.0/README.md` & `social-auth-app-django-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/setup.py` & `social-auth-app-django-5.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Setup file for easy installation"""
+
 import re
 from os.path import dirname, join
 
 from setuptools import setup
 
 VERSION_RE = re.compile(r"__version__ = \"([\d\.]+)\"")
```

### Comparing `social-auth-app-django-5.4.0/social_auth_app_django.egg-info/PKG-INFO` & `social-auth-app-django-5.4.1/social_auth_app_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-app-django
-Version: 5.4.0
+Version: 5.4.1
 Summary: Python Social Authentication, Django integration.
 Home-page: https://github.com/python-social-auth/social-app-django
 Author: Matias Aguirre
 Author-email: matiasaguirre@gmail.com
 License: BSD
 Keywords: django,social auth
 Platform: UNKNOWN
```

### Comparing `social-auth-app-django-5.4.0/social_auth_app_django.egg-info/SOURCES.txt` & `social-auth-app-django-5.4.1/social_auth_app_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/__init__.py` & `social-auth-app-django-5.4.1/social_django/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "5.4.0"
+__version__ = "5.4.1"
 
 
 from social_core.backends.base import BaseAuth
 
 # django.contrib.auth.load_backend() will import and instanciate the
 # authentication backend ignoring the possibility that it might
 # require more arguments. Here we set a monkey patch to
```

### Comparing `social-auth-app-django-5.4.0/social_django/admin.py` & `social-auth-app-django-5.4.1/social_django/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Admin settings"""
+
 from itertools import chain
 
 from django.conf import settings
 from django.contrib import admin
 from social_core.utils import setting_name
 
 from .models import Association, Nonce, UserSocialAuth
```

### Comparing `social-auth-app-django-5.4.0/social_django/context_processors.py` & `social-auth-app-django-5.4.1/social_django/context_processors.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/fields.py` & `social-auth-app-django-5.4.1/social_django/fields.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/management/commands/clearsocial.py` & `social-auth-app-django-5.4.1/social_django/management/commands/clearsocial.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/middleware.py` & `social-auth-app-django-5.4.1/social_django/middleware.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0001_initial.py` & `social-auth-app-django-5.4.1/social_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0002_add_related_name.py` & `social-auth-app-django-5.4.1/social_django/migrations/0002_add_related_name.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0003_alter_email_max_length.py` & `social-auth-app-django-5.4.1/social_django/migrations/0003_alter_email_max_length.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0006_partial.py` & `social-auth-app-django-5.4.1/social_django/migrations/0006_partial.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0007_code_timestamp.py` & `social-auth-app-django-5.4.1/social_django/migrations/0007_code_timestamp.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0008_partial_timestamp.py` & `social-auth-app-django-5.4.1/social_django/migrations/0008_partial_timestamp.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0009_auto_20191118_0520.py` & `social-auth-app-django-5.4.1/social_django/migrations/0009_auto_20191118_0520.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0011_alter_id_fields.py` & `social-auth-app-django-5.4.1/social_django/migrations/0011_alter_id_fields.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0012_usersocialauth_extra_data_new.py` & `social-auth-app-django-5.4.1/social_django/migrations/0012_usersocialauth_extra_data_new.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0013_migrate_extra_data.py` & `social-auth-app-django-5.4.1/social_django/migrations/0013_migrate_extra_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 4.0 on 2023-06-10 07:10
 
 import json
 
-from django.db import migrations
+from django.db import migrations, models
 
 
 def migrate_json_field(apps, schema_editor):
     UserSocialAuth = apps.get_model("social_django", "UserSocialAuth")
     Partial = apps.get_model("social_django", "Partial")
     db_alias = schema_editor.connection.alias
     to_be_updated = []
@@ -37,15 +37,54 @@
                 old_value = json.loads(old_value)
             except json.JSONDecodeError as error:
                 print(f"Failed to migrate data {old_value}: {error}")
         auth.data_new = old_value
         auth.save(update_fields=["data_new"])
 
 
+def migrate_json_field_backwards(apps, schema_editor):
+    UserSocialAuth = apps.get_model("social_django", "UserSocialAuth")
+    Partial = apps.get_model("social_django", "Partial")
+    db_alias = schema_editor.connection.alias
+    to_be_updated = []
+
+    is_text_field = isinstance(
+        UserSocialAuth._meta.get_field("extra_data"),
+        models.TextField,
+    )
+    for auth in UserSocialAuth.objects.using(db_alias).iterator():
+        new_value = auth.extra_data_new
+        if is_text_field:
+            new_value = json.dumps(new_value)
+        auth.extra_data = new_value
+        to_be_updated.append(auth)
+
+        if len(to_be_updated) >= 1000:
+            UserSocialAuth.objects.bulk_update(to_be_updated, ["extra_data"])
+            to_be_updated.clear()
+
+    if to_be_updated:
+        UserSocialAuth.objects.bulk_update(to_be_updated, ["extra_data"])
+        to_be_updated.clear()
+
+    is_text_field = issubclass(
+        Partial._meta.get_field("data"),
+        models.TextField,
+    )
+    for auth in Partial.objects.using(db_alias).all():
+        new_value = auth.data_new
+        if is_text_field:
+            new_value = json.dumps(new_value)
+        auth.data = new_value
+        auth.save(update_fields=["data"])
+
+
 class Migration(migrations.Migration):
     dependencies = [
         ("social_django", "0012_usersocialauth_extra_data_new"),
     ]
 
     operations = [
-        migrations.RunPython(migrate_json_field, elidable=True),
+        migrations.RunPython(
+            migrate_json_field, migrate_json_field_backwards, elidable=True
+        ),
     ]
```

### Comparing `social-auth-app-django-5.4.0/social_django/migrations/0015_rename_extra_data_new_usersocialauth_extra_data.py` & `social-auth-app-django-5.4.1/social_django/migrations/0015_rename_extra_data_new_usersocialauth_extra_data.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/models.py` & `social-auth-app-django-5.4.1/social_django/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Django ORM models for Social Auth"""
+
 from django.conf import settings
 from django.db import models
 from django.db.utils import IntegrityError
 from social_core.utils import setting_name
 
 from .managers import UserSocialAuthManager
 from .storage import (
@@ -49,19 +50,23 @@
         return str(self.user)
 
     class Meta:
         app_label = "social_django"
         abstract = True
 
     @classmethod
-    def get_social_auth(cls, provider, uid):
-        try:
-            return cls.objects.select_related("user").get(provider=provider, uid=uid)
-        except cls.DoesNotExist:
-            return None
+    def get_social_auth(cls, provider: str, uid: str):
+        for social in cls.objects.select_related("user").filter(
+            provider=provider, uid=uid
+        ):
+            # We need to compare to filter out case-insensitive lookups in
+            # some databases (MySQL/MariaDB)
+            if social.uid == uid:
+                return social
+        return None
 
     @classmethod
     def username_max_length(cls):
         username_field = cls.username_field()
         field = cls.user_model()._meta.get_field(username_field)
         return field.max_length
```

### Comparing `social-auth-app-django-5.4.0/social_django/storage.py` & `social-auth-app-django-5.4.1/social_django/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Django ORM models for Social Auth"""
+
 import base64
 
 from django.core.exceptions import FieldDoesNotExist
 from django.db import router, transaction
 from django.db.utils import IntegrityError
 from social_core.storage import (
     AssociationMixin,
```

### Comparing `social-auth-app-django-5.4.0/social_django/strategy.py` & `social-auth-app-django-5.4.1/social_django/strategy.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/urls.py` & `social-auth-app-django-5.4.1/social_django/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """URLs module"""
+
 from django.conf import settings
 from django.urls import path
 from social_core.utils import setting_name
 
 from . import views
 
 extra = getattr(settings, setting_name("TRAILING_SLASH"), True) and "/" or ""
```

### Comparing `social-auth-app-django-5.4.0/social_django/utils.py` & `social-auth-app-django-5.4.1/social_django/utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/social_django/views.py` & `social-auth-app-django-5.4.1/social_django/views.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/tests/settings.py` & `social-auth-app-django-5.4.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/tests/test_admin.py` & `social-auth-app-django-5.4.1/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/tests/test_context_processors.py` & `social-auth-app-django-5.4.1/tests/test_context_processors.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/tests/test_middleware.py` & `social-auth-app-django-5.4.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/tests/test_migrations.py` & `social-auth-app-django-5.4.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/tests/test_models.py` & `social-auth-app-django-5.4.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/tests/test_strategy.py` & `social-auth-app-django-5.4.1/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `social-auth-app-django-5.4.0/tests/test_views.py` & `social-auth-app-django-5.4.1/tests/test_views.py`

 * *Files identical despite different names*

