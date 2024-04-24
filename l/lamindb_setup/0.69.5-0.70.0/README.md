# Comparing `tmp/lamindb_setup-0.69.5.tar.gz` & `tmp/lamindb_setup-0.70.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.69.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.70.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.69.5.tar` & `lamindb_setup-0.70.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0     8290 2024-04-16 19:27:14.643060 lamindb_setup-0.69.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.69.5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.69.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.69.5/.gitignore
--rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.69.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.69.5/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.69.5/README.md
--rw-r--r--   0        0        0    96860 2024-04-22 05:51:48.799859 lamindb_setup-0.69.5/docs/changelog.md
--rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.69.5/docs/hub-cloud/01-init-on-prem-instance.ipynb
--rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.69.5/docs/hub-cloud/02-connect-on-prem-instance.ipynb
--rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.69.5/docs/hub-cloud/03-set-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.69.5/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     3106 2024-04-08 06:13:37.564530 lamindb_setup-0.69.5/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     3806 2024-04-21 08:00:19.897288 lamindb_setup-0.69.5/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.69.5/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.69.5/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.69.5/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.69.5/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.69.5/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.69.5/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.69.5/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.69.5/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.69.5/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.69.5/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.69.5/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.69.5/docs/index.md
--rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.69.5/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.69.5/docs/reference.md
--rw-r--r--   0        0        0     1558 2024-04-22 05:51:36.763309 lamindb_setup-0.69.5/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.69.5/lamindb_setup/_add_remote_storage.py
--rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.69.5/lamindb_setup/_cache.py
--rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.69.5/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.69.5/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.69.5/lamindb_setup/_close.py
--rw-r--r--   0        0        0    11789 2024-04-19 17:16:01.027505 lamindb_setup-0.69.5/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.69.5/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.69.5/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2084 2024-04-15 04:44:50.596309 lamindb_setup-0.69.5/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1836 2024-04-15 06:35:29.022278 lamindb_setup-0.69.5/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11479 2024-04-08 10:33:42.801066 lamindb_setup-0.69.5/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     8672 2024-04-17 08:15:10.952927 lamindb_setup-0.69.5/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.69.5/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.69.5/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.69.5/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.69.5/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      369 2024-04-16 15:26:03.848647 lamindb_setup-0.69.5/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     1762 2024-04-08 09:34:48.611370 lamindb_setup-0.69.5/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.69.5/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.69.5/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5520 2024-04-15 15:03:26.266397 lamindb_setup-0.69.5/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    10990 2024-04-15 15:03:26.266901 lamindb_setup-0.69.5/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.69.5/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.69.5/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.69.5/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    11556 2024-04-16 19:47:35.808698 lamindb_setup-0.69.5/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.69.5/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.69.5/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    13044 2024-04-16 19:47:35.808927 lamindb_setup-0.69.5/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.69.5/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.69.5/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.69.5/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.69.5/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     3335 2024-04-16 15:26:03.848992 lamindb_setup-0.69.5/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.69.5/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.69.5/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      497 2024-04-05 12:59:33.028024 lamindb_setup-0.69.5/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    24510 2024-04-21 08:00:19.898318 lamindb_setup-0.69.5/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     4265 2024-04-08 09:34:48.612298 lamindb_setup-0.69.5/noxfile.py
--rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.69.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-19 17:16:01.027907 lamindb_setup-0.69.5/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.69.5/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.69.5/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.69.5/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.69.5/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.69.5/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0      548 2024-04-08 09:34:48.612599 lamindb_setup-0.69.5/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11318 2024-04-15 15:03:26.267377 lamindb_setup-0.69.5/tests/hub-local/test_all.py
--rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.69.5/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.69.5/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      158 2024-04-16 15:26:03.849537 lamindb_setup-0.69.5/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1432 2024-04-15 15:03:26.267758 lamindb_setup-0.69.5/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.69.5/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.69.5/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.69.5/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.69.5/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.69.5/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.69.5/PKG-INFO
+-rw-r--r--   0        0        0     8290 2024-04-16 19:27:14.643060 lamindb_setup-0.70.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.70.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.70.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-04-16 19:27:14.643308 lamindb_setup-0.70.0/.gitignore
+-rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.70.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.70.0/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.70.0/README.md
+-rw-r--r--   0        0        0    97544 2024-04-24 10:46:02.552654 lamindb_setup-0.70.0/docs/changelog.md
+-rw-r--r--   0        0        0     2573 2024-04-23 21:24:09.761470 lamindb_setup-0.70.0/docs/hub-cloud/01-init-local-instance.ipynb
+-rw-r--r--   0        0        0     3947 2024-04-23 21:24:09.761588 lamindb_setup-0.70.0/docs/hub-cloud/02-connect-local-instance.ipynb
+-rw-r--r--   0        0        0     5817 2024-04-23 13:03:29.807601 lamindb_setup-0.70.0/docs/hub-cloud/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.70.0/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     3111 2024-04-23 13:03:29.807936 lamindb_setup-0.70.0/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3806 2024-04-21 08:00:19.897288 lamindb_setup-0.70.0/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     2779 2024-04-23 21:24:09.761821 lamindb_setup-0.70.0/docs/hub-cloud/07-connect-hybrid-instance.ipynb
+-rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.70.0/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.70.0/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-04-22 13:06:55.467504 lamindb_setup-0.70.0/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.70.0/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.70.0/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2711 2024-04-23 13:03:29.808107 lamindb_setup-0.70.0/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.70.0/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.70.0/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.70.0/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6181 2024-04-22 20:26:08.605836 lamindb_setup-0.70.0/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.70.0/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.70.0/docs/index.md
+-rw-r--r--   0        0        0      516 2024-04-23 21:24:09.762085 lamindb_setup-0.70.0/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.70.0/docs/reference.md
+-rw-r--r--   0        0        0     1558 2024-04-24 10:45:41.099277 lamindb_setup-0.70.0/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.70.0/lamindb_setup/_add_remote_storage.py
+-rw-r--r--   0        0        0      809 2024-04-23 11:01:04.804829 lamindb_setup-0.70.0/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.70.0/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.70.0/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.70.0/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    11908 2024-04-24 10:00:32.983268 lamindb_setup-0.70.0/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     5861 2024-04-24 09:58:58.984598 lamindb_setup-0.70.0/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.70.0/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2084 2024-04-15 04:44:50.596309 lamindb_setup-0.70.0/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1836 2024-04-15 06:35:29.022278 lamindb_setup-0.70.0/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11480 2024-04-23 14:54:28.059779 lamindb_setup-0.70.0/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     8810 2024-04-23 21:24:09.762839 lamindb_setup-0.70.0/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      796 2024-04-23 14:54:28.060356 lamindb_setup-0.70.0/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.70.0/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     3658 2024-04-23 14:54:28.060603 lamindb_setup-0.70.0/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.70.0/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      369 2024-04-16 15:26:03.848647 lamindb_setup-0.70.0/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     1762 2024-04-08 09:34:48.611370 lamindb_setup-0.70.0/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.70.0/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.70.0/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5520 2024-04-15 15:03:26.266397 lamindb_setup-0.70.0/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    11294 2024-04-23 21:24:09.763136 lamindb_setup-0.70.0/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.70.0/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.70.0/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.70.0/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    13927 2024-04-24 09:59:49.631691 lamindb_setup-0.70.0/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3745 2024-04-23 14:54:28.061051 lamindb_setup-0.70.0/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2571 2024-04-23 14:54:28.061337 lamindb_setup-0.70.0/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    11750 2024-04-23 21:24:09.763780 lamindb_setup-0.70.0/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.70.0/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1282 2024-04-23 14:54:28.061801 lamindb_setup-0.70.0/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.70.0/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.70.0/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     3411 2024-04-23 21:24:09.764077 lamindb_setup-0.70.0/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.70.0/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.70.0/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      497 2024-04-05 12:59:33.028024 lamindb_setup-0.70.0/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    25078 2024-04-23 14:26:22.574000 lamindb_setup-0.70.0/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     4265 2024-04-08 09:34:48.612298 lamindb_setup-0.70.0/noxfile.py
+-rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.70.0/pyproject.toml
+-rw-r--r--   0        0        0     5379 2024-04-23 21:24:09.764323 lamindb_setup-0.70.0/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.70.0/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     6179 2024-04-23 13:03:29.809705 lamindb_setup-0.70.0/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.70.0/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.70.0/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.70.0/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0      548 2024-04-08 09:34:48.612599 lamindb_setup-0.70.0/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11329 2024-04-23 14:54:28.062287 lamindb_setup-0.70.0/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0      398 2024-04-22 20:59:53.004753 lamindb_setup-0.70.0/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.70.0/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      158 2024-04-16 15:26:03.849537 lamindb_setup-0.70.0/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1432 2024-04-15 15:03:26.267758 lamindb_setup-0.70.0/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.70.0/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.70.0/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.70.0/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.70.0/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      842 2024-04-22 06:08:16.280331 lamindb_setup-0.70.0/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.70.0/PKG-INFO
```

### Comparing `lamindb_setup-0.69.5/.github/workflows/build.yml` & `lamindb_setup-0.70.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/.github/workflows/latest-changes.yml` & `lamindb_setup-0.70.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/.gitignore` & `lamindb_setup-0.70.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/.pre-commit-config.yaml` & `lamindb_setup-0.70.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/LICENSE` & `lamindb_setup-0.70.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/changelog.md` & `lamindb_setup-0.70.0/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Introduce `local_storage` mode for cloud instances | [728](https://github.com/laminlabs/lamindb-setup/pull/728) | [falexwolf](https://github.com/falexwolf) | 2024-04-23 | 0.70.0
+🚚 Make `.uuid` attributes private | [727](https://github.com/laminlabs/lamindb-setup/pull/727) | [falexwolf](https://github.com/falexwolf) | 2024-04-23 |
+🚚 Rename `is_cloud` to `type_is_cloud` | [726](https://github.com/laminlabs/lamindb-setup/pull/726) | [falexwolf](https://github.com/falexwolf) | 2024-04-23 |
+🚸 In `.delete()`, check for data deletion & delete from hub | [725](https://github.com/laminlabs/lamindb-setup/pull/725) | [falexwolf](https://github.com/falexwolf) | 2024-04-22 |
 ✨ Upload dirs inplace | [722](https://github.com/laminlabs/lamindb-setup/pull/722) | [Koncopd](https://github.com/Koncopd) | 2024-04-20 | 0.69.5
 ♻️ Do not always read from local cache | [720](https://github.com/laminlabs/lamindb-setup/pull/720) | [falexwolf](https://github.com/falexwolf) | 2024-04-19 | 0.69.4
 ♻️ Improve suffix handling | [718](https://github.com/laminlabs/lamindb-setup/pull/718) | [falexwolf](https://github.com/falexwolf) | 2024-04-19 | 0.69.3
 ✨ Enable hybrid storage mode | [717](https://github.com/laminlabs/lamindb-setup/pull/717) | [falexwolf](https://github.com/falexwolf) | 2024-04-16 | 0.69.1
 🚸 Better migrations warning | [716](https://github.com/laminlabs/lamindb-setup/pull/716) | [falexwolf](https://github.com/falexwolf) | 2024-04-16 |
 🚸 Refresh token also upon access-aws | [715](https://github.com/laminlabs/lamindb-setup/pull/715) | [falexwolf](https://github.com/falexwolf) | 2024-04-15 |
 🚸 Skip hub request for a purely local instance | [713](https://github.com/laminlabs/lamindb-setup/pull/713) | [falexwolf](https://github.com/falexwolf) | 2024-04-08 | 0.69.0
```

### Comparing `lamindb_setup-0.69.5/docs/hub-cloud/01-init-on-prem-instance.ipynb` & `lamindb_setup-0.70.0/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.74313884644767%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict()}, 'source': ['# Test SQLite file locking'], "*

 * *            "'id': '4c28a5ac', delete: ['attachments']}, 1: {'metadata': {replace: OrderedDict()}, "*

 * *            "'source': ['!lamin login testuser2'], 'id': '89b7057a'}, 2: {'source': ['import "*

 * *            "pytest\\n', 'import lamindb_setup as ln_setup\\n', 'from "*

 * *            "lamindb_setup.core.cloud_sqlite_locker import Locker, InstanceLockedException\\n', "*

 * *            "'from lamindb_setup.core.upath im […]*

```diff
@@ -1,343 +1,259 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
-            "metadata": {
-                "tags": []
-            },
+            "id": "4c28a5ac",
+            "metadata": {},
             "source": [
-                "# Init on-prem instance"
+                "# Test SQLite file locking"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "89b7057a",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "!lamin login testuser1"
+                "!lamin login testuser2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "69eeefee",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb_setup as ln_setup"
+                "import pytest\n",
+                "import lamindb_setup as ln_setup\n",
+                "from lamindb_setup.core.cloud_sqlite_locker import Locker, InstanceLockedException\n",
+                "from lamindb_setup.core.upath import UPath"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0acefaf3",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Local database & storage"
+                "root = UPath(\"s3://lamindb-ci/test-load-lock\", cache_regions=True)"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4afc62b6",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### SQLite"
+                "exclusion = root / \".lamindb/_exclusion/\"\n",
+                "# if cache is present, then .exists() for intermediate keys return False\n",
+                "# bug in s3fs\n",
+                "exclusion.fs.invalidate_cache()\n",
+                "if exclusion.exists():\n",
+                "    exclusion.rmdir()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "7d142acd",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.init(storage=\"./mydata\")"
+                "assert ln_setup.settings.user.handle == \"testuser2\""
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "201d1baf",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "This automatically assigns an instance name that equals the name of the storage root along with a few other settings:"
+                "ln_setup.init(storage=\"s3://lamindb-ci/test-load-lock\", name=\"test-load-lock\")\n",
+                "instance_id = ln_setup.settings.instance.id\n",
+                "ln_setup.close()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "f628325e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.settings.instance"
+                "# lock with some random id\n",
+                "locker = Locker(\"randuseridtt\", storage_root=root, instance_id=instance_id)"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f3cad961",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "If you want to register the instance on the hub at lamin.ai, use {func}`lamindb_setup.register`."
+                "locker.lock()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "72bdc453",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "from pathlib import Path\n",
-                "\n",
-                "assert ln_setup.settings.instance.storage.is_cloud == False\n",
-                "assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle\n",
-                "assert ln_setup.settings.instance.name == \"mydata\"\n",
-                "assert ln_setup.settings.storage.root.as_posix() == Path(\"mydata\").resolve().as_posix()\n",
-                "assert ln_setup.settings.storage.id is not None\n",
-                "assert (\n",
-                "    ln_setup.settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/{ln_setup.settings.instance.id.hex}.lndb\"\n",
-                ")"
+                "# with pytest.raises(InstanceLockedException):\n",
+                "#    ln_setup.connect(\"test-load-lock\"), would like to test this, but need another python session"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "9c0471c1",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "See the info on the current instance & user:"
+                "locker.unlock()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "6b1d536f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.settings"
+                "# ln_setup.connect(\"test-load-lock\")\n",
+                "# ln_setup.close()"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "c8c615dd",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "To delete an instance, call:"
+                "# lock through testuser1, who has user id \"DzTjkKse\"\n",
+                "locker = Locker(\"DzTjkKse\", storage_root=root, instance_id=instance_id)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "171439b1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln_setup.delete(\"mydata\", force=True)"
+                "locker.lock()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "a4754388",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "from lamindb_setup.core._settings_store import instance_settings_file\n",
+                "# with pytest.raises(InstanceLockedException) as error:\n",
+                "#     ln_setup.connect(\"test-load-lock\")\n",
                 "\n",
-                "settings_file = instance_settings_file(\"mydata\", \"testuser1\")\n",
-                "assert settings_file.exists() == False"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Postgres"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "source": [
-                "```\n",
-                "from laminci.db import setup_local_test_postgres\n",
-                "pgurl = setup_local_test_postgres()\n",
-                "```"
+                "# assert (\n",
+                "#     \"InstanceLockedException: Cannot load the instance, it is locked by 'testuser1'\"\n",
+                "#     \" (uid: 'DzTjkKse', name: 'Test User1').\"\n",
+                "#     in error.exconly()\n",
+                "# )"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "A connection string for postgres looks like this:\n",
-                "```\n",
-                "'postgresql://postgres:pwd@0.0.0.0:5432/pgtest'\n",
-                "```"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "You can call init like so:"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "```\n",
-                "ln_setup.init(storage=\"./mydatapg\", db='postgresql://postgres:pwd@0.0.0.0:5432/pgtest')\n",
-                "```"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Your instance name will then be `pgtest`!"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Custom instance name"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Instead of having the instance name be auto-determined from `storage` or `db`, you can provide a custom name:"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "```\n",
-                "ln_setup.init(storage=\"./mystorage\", name=\"mydata2\", db=pgurl)\n",
-                "```"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Configure with default cloud storage"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### AWS"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "c9bd3d47",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "You need to have access to AWS S3 (run `pip instsall awscli` and `aws configure`)."
+                "locker.unlock()"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2c392fee",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Consider the special case of a cloud SQLite instance:"
+                "# ln_setup.connect(\"test-load-lock\")"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "bb510295",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "```\n",
-                "ln_setup.init(storage=\"s3://lamindb-ci/mydata\")\n",
-                "```"
+                "# test ignore_prev_locker=True in unlock_cloud_sqlite_upon_exception\n",
+                "# i.e. test that the locker doesn't unlock if the locker hasn't changed during the function execution\n",
+                "# with pytest.raises(RuntimeError):\n",
+                "#     ln_setup.connect(\"test-load-lock\")\n",
+                "\n",
+                "# assert ln_setup.settings.instance._cloud_sqlite_locker._has_lock"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "10a1086d",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Under the hood LaminDB then keeps track of a cloud & and a synched local SQLite file."
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "source": [
-                "```\n",
-                "# you can inspect these:\n",
-                "ln_setup.settings.instance._sqlite_file\n",
-                "ln_setup.settings.instance._sqlite_file_local\n",
-                "```"
+                "# ln_setup.close()"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "a94a7a60",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### GCP"
+                "# purely technical varibale to test failed load after locking\n",
+                "# ln_setup._connect_instance._TEST_FAILED_LOAD = True\n",
+                "\n",
+                "# with pytest.raises(RuntimeError):\n",
+                "#     ln_setup.connect(\"test-load-lock\")\n",
+                "\n",
+                "# assert ln_setup.core.cloud_sqlite_locker._locker._has_lock is None\n",
+                "\n",
+                "# ln_setup._connect_instance._TEST_FAILED_LOAD = False"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "48bcdf82",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "You need to authenticate for Google Cloud.\n",
-                "\n",
-                "* Either, set the environment variable `export GOOGLE_APPLICATION_CREDENTIALS=<HOME-DIR>/.lndb/<GOOGLE CLOUD PROJECT>.json`.\n",
-                "* Alternatively, if you set up the `gcloud` CLI, log in with `gcloud auth application-default login`.\n"
+                "# ln_setup.connect(\"test-load-lock\", _test=True)"
             ]
         },
         {
-            "attachments": {},
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "b8b0c52a",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "```\n",
-                "ln_setup.init(storage=\"gs://lamindb-ci-us\")\n",
-                "```"
+                "ln_setup.delete(\"test-load-lock\", force=True)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -349,18 +265,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "40d3a090f54c6569ab1632332b64b2c03c39dcf918b08424e98f38b5ae0af88f"
-            }
+            "version": "3.9.17"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `lamindb_setup-0.69.5/docs/hub-cloud/02-connect-on-prem-instance.ipynb` & `lamindb_setup-0.70.0/docs/hub-cloud/02-connect-local-instance.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9865496882924768%*

 * *Differences: {"'cells'": "{0: {'source': ['# Connect to local instance']}, 1: {'source': {insert: [(0, '# here, "*

 * *            'we construct a case in which the storage location of the previous instance was '*

 * *            "moved\\n'), (2, '!lamin delete --force mydata\\n')], delete: [1]}}, 7: {'source': "*

 * *            "{insert: [(2, 'assert ln_setup.settings.instance.storage.type_is_cloud == "*

 * *            "False\\n')], delete: [2]}}, 10: {'source': ['Delete:']}, delete: [1]}",*

 * * "'metadata'": "{'language_info': {'version':  […]*

```diff
@@ -4,36 +4,29 @@
             "attachments": {},
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Load & delete an on-prem instance"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "f165d50c",
-            "metadata": {},
-            "source": [
-                "Here, we construct a case in which the storage location of the previous instance was moved:"
+                "# Connect to local instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5fd65a65-5c34-462e-a980-a5aed1a2713f",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
+                "# here, we construct a case in which the storage location of the previous instance was moved\n",
                 "!lamin close\n",
-                "!yes | lamin delete mydata\n",
+                "!lamin delete --force mydata\n",
                 "!lamin init --storage mydata\n",
                 "!rm -r ./mydata_new_loc\n",
                 "!mv mydata ./mydata_new_loc\n",
                 "!lamin close"
             ]
         },
         {
@@ -95,15 +88,15 @@
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "\n",
-                "assert ln_setup.settings.instance.storage.is_cloud == False\n",
+                "assert ln_setup.settings.instance.storage.type_is_cloud == False\n",
                 "assert ln_setup.settings.instance.name == \"mydata\"\n",
                 "assert (\n",
                 "    ln_setup.settings.instance.storage.root.as_posix()\n",
                 "    == Path(\"./mydata_new_loc\").resolve().as_posix()\n",
                 ")\n",
                 "assert (\n",
                 "    ln_setup.settings.instance.db\n",
@@ -137,15 +130,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "e3701120",
             "metadata": {},
             "source": [
-                "## Delete an instance"
+                "Delete:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8e54d8cd",
             "metadata": {},
@@ -169,15 +162,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.10.13"
         },
         "vscode": {
             "interpreter": {
                 "hash": "5c7b89af1651d0b8571dde13640ecdccf7d5a6204171d6ab33e7c296e100e08a"
             }
         }
     },
```

### Comparing `lamindb_setup-0.69.5/docs/hub-cloud/03-set-storage.ipynb` & `lamindb_setup-0.70.0/docs/hub-cloud/03-set-storage.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998816287878788%*

 * *Differences: {"'cells'": "{16: {'source': {insert: [(0, 'assert ln_setup.settings.storage.type_is_cloud\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -178,15 +178,15 @@
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "assert ln_setup.settings.storage.is_cloud\n",
+                "assert ln_setup.settings.storage.type_is_cloud\n",
                 "assert ln_setup.settings.storage.root_as_str == \"s3://lamindb-ci\"\n",
                 "assert ln_setup.settings.storage.region == \"us-west-1\"\n",
                 "# root.fs contains the underlying fsspec filesystem\n",
                 "assert (\n",
                 "    ln_setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
                 ")"
             ]
```

### Comparing `lamindb_setup-0.69.5/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.70.0/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.70.0/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995370370370371%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(0, 'assert ln_setup.settings.instance.storage.type_is_cloud "*

 * *            "== True\\n')], delete: [0]}}}"}*

```diff
@@ -86,15 +86,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln_setup.settings.instance.storage.is_cloud == True\n",
+                "assert ln_setup.settings.instance.storage.type_is_cloud == True\n",
                 "assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle\n",
                 "assert ln_setup.settings.instance.name == \"my-hosted\"\n",
                 "assert ln_setup.settings.storage.root.as_posix().startswith(hosted_buckets)\n",
                 "assert ln_setup.settings.storage.id is not None"
             ]
         },
         {
```

### Comparing `lamindb_setup-0.69.5/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.70.0/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.70.0/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.70.0/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.70.0/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.70.0/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.70.0/docs/hub-prod/test-empty-init.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997106481481481%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(0, 'assert ln_setup.settings.storage.type_is_cloud\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -67,15 +67,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "544dbae3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln_setup.settings.storage.is_cloud\n",
+                "assert ln_setup.settings.storage.type_is_cloud\n",
                 "assert ln_setup.settings.storage.root_as_str == root_str\n",
                 "assert ln_setup.settings.storage.region == \"us-east-1\"\n",
                 "assert (\n",
                 "    str(ln_setup.settings.instance._sqlite_file)\n",
                 "    == f\"{root_str}/{ln_setup.settings.instance.id.hex}.lndb\"\n",
                 ")"
             ]
```

### Comparing `lamindb_setup-0.69.5/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.70.0/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.70.0/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.70.0/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/__init__.py` & `lamindb_setup-0.70.0/lamindb_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.69.5"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.70.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._close import close  # noqa
 from ._delete import delete  # noqa
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_add_remote_storage.py` & `lamindb_setup-0.70.0/lamindb_setup/_add_remote_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_cache.py` & `lamindb_setup-0.70.0/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_check_setup.py` & `lamindb_setup-0.70.0/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_close.py` & `lamindb_setup-0.70.0/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.70.0/lamindb_setup/_connect_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,25 @@
 
 
 # this is for testing purposes only
 # set to True only to test failed load
 _TEST_FAILED_LOAD = False
 
 
+INSTANCE_NOT_FOUND_MESSAGE = (
+    "'{owner}/{name}' not found:"
+    " '{hub_result}'\nCheck your permissions:"
+    " https://lamin.ai/{owner}/{name}"
+)
+
+
+class InstanceNotFoundError(SystemExit):
+    pass
+
+
 def check_db_dsn_equal_up_to_credentials(db_dsn_hub, db_dsn_local):
     return (
         db_dsn_hub.scheme == db_dsn_local.scheme
         and db_dsn_hub.host == db_dsn_local.host
         and db_dsn_hub.database == db_dsn_local.database
         and db_dsn_hub.port == db_dsn_local.port
     )
@@ -117,14 +128,16 @@
             close_instance(mute=True)
 
         settings_file = instance_settings_file(name, owner)
 
         make_hub_request = True
         if settings_file.exists():
             isettings = load_instance_settings(settings_file)
+            # mimic instance_result from hub
+            instance_result = {"id": isettings.id.hex}
             # skip hub request for a purely local instance
             make_hub_request = isettings.is_remote
 
         if make_hub_request:
             # the following will return a string if the instance does not exist
             # on the hub
             hub_result = load_instance_from_hub(owner=owner, name=name)
@@ -135,45 +148,41 @@
                 db_updated = update_db_using_local(
                     instance_result, settings_file, db=db
                 )
                 ssettings = StorageSettings(
                     root=storage_result["root"],
                     region=storage_result["region"],
                     uid=storage_result["lnid"],
-                    is_hybrid=instance_result["storage_mode"] == "hybrid",
                 )
                 isettings = InstanceSettings(
                     id=UUID(instance_result["id"]),
                     owner=owner,
                     name=name,
                     storage=ssettings,
                     db=db_updated,
                     schema=instance_result["schema_str"],
                     git_repo=instance_result["git_repo"],
+                    local_storage=instance_result["storage_mode"] == "hybrid",
                 )
                 check_whether_migrations_in_sync(instance_result["lamindb_version"])
             else:
-                error_message = (
-                    f"'{owner}/{name}' not loadable:"
-                    f" '{hub_result}'\nCheck your permissions:"
-                    f" https://lamin.ai/{owner}/{name}?tab=collaborators"
+                message = INSTANCE_NOT_FOUND_MESSAGE.format(
+                    owner=owner, name=name, hub_result=hub_result
                 )
                 if settings_file.exists():
                     isettings = load_instance_settings(settings_file)
                     if isettings.is_remote:
                         if _raise_not_reachable_error:
-                            raise SystemExit(error_message)
+                            raise InstanceNotFoundError(message)
                         return "instance-not-reachable"
 
                 else:
                     if _raise_not_reachable_error:
-                        raise SystemExit(error_message)
+                        raise InstanceNotFoundError(message)
                     return "instance-not-reachable"
-                # mimic instance_result from hub
-                instance_result = {"id": isettings.id.hex}
 
         if storage is not None:
             update_isettings_with_storage(isettings, storage)
         isettings._persist()
         if _test:
             return None
         silence_loggers()
@@ -251,15 +260,15 @@
     return owner, name
 
 
 def update_isettings_with_storage(
     isettings: InstanceSettings, storage: UPathStr
 ) -> None:
     ssettings = StorageSettings(storage)
-    if ssettings.is_cloud:
+    if ssettings.type_is_cloud:
         try:  # triggering ssettings.id makes a lookup in the storage table
             logger.success(f"loaded storage: {ssettings.id} / {ssettings.root_as_str}")
         except RuntimeError as e:
             logger.error(
                 "storage not registered!\n"
                 "load instance without the `storage` arg and register storage root: "
                 f"`lamin set storage --storage {storage}`"
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_delete.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,107 @@
-import shutil
+import os
+from typing import Union, Optional
+from lamindb_setup.core import InstanceSettings, StorageSettings, UserSettings
+from lamindb_setup.core._settings_load import (
+    load_instance_settings,
+    load_or_create_user_settings,
+)
+from ._settings_store import current_instance_settings_file
 from pathlib import Path
-from lamin_utils import logger
-from typing import Optional
-from .core._settings_instance import InstanceSettings
-from .core._settings import settings
-from .core._settings_load import load_instance_settings
-from .core._settings_store import instance_settings_file
-
-
-def delete_cache(cache_dir: Path):
-    if cache_dir is not None and cache_dir.exists():
-        shutil.rmtree(cache_dir)
-
-
-def delete_by_isettings(isettings: InstanceSettings) -> None:
-    settings_file = isettings._get_settings_file()
-    if settings_file.exists():
-        settings_file.unlink()
-    delete_cache(isettings.storage.cache_dir)
-    if isettings.dialect == "sqlite":
+from ._settings_store import settings_dir
+
+
+class SetupSettings:
+    """Setup settings.
+
+    - :class:`~lamindb_setup.core.InstanceSettings`
+    - :class:`~lamindb_setup.core.StorageSettings`
+    - :class:`~lamindb_setup.core.UserSettings`
+    """
+
+    _using_key: Optional[str] = None  # set through lamindb.settings
+
+    _user_settings: Union[UserSettings, None] = None
+    _instance_settings: Union[InstanceSettings, None] = None
+
+    _user_settings_env: Union[str, None] = None
+    _instance_settings_env: Union[str, None] = None
+
+    _auto_connect_path: Path = settings_dir / "auto_connect"
+
+    @property
+    def _instance_settings_path(self) -> Path:
+        return current_instance_settings_file()
+
+    @property
+    def settings_dir(self) -> Path:
+        return settings_dir
+
+    @property
+    def auto_connect(self) -> bool:
+        """Auto-connect to loaded instance upon lamindb import."""
+        return self._auto_connect_path.exists()
+
+    @auto_connect.setter
+    def auto_connect(self, value: bool) -> None:
+        if value:
+            self._auto_connect_path.touch()
+        else:
+            self._auto_connect_path.unlink(missing_ok=True)
+
+    @property
+    def user(self) -> UserSettings:
+        """User."""
+        if (
+            self._user_settings is None
+            or self._user_settings_env != get_env_name()  # noqa
+        ):
+            self._user_settings = load_or_create_user_settings()
+            self._user_settings_env = get_env_name()
+            if self._user_settings and self._user_settings.uid is None:
+                raise RuntimeError("Need to login, first: lamin login <email>")
+        return self._user_settings  # type: ignore
+
+    @property
+    def instance(self) -> InstanceSettings:
+        """Instance."""
+        if (
+            self._instance_settings is None
+            or self._instance_settings_env != get_env_name()  # noqa
+        ):
+            self._instance_settings = load_instance_settings()
+            self._instance_settings_env = get_env_name()
+        return self._instance_settings  # type: ignore
+
+    @property
+    def storage(self) -> StorageSettings:
+        """Storage."""
+        return self.instance.storage
+
+    @property
+    def _instance_exists(self):
         try:
-            if isettings._sqlite_file.exists():
-                isettings._sqlite_file.unlink()
-            exclusion_dir = (
-                isettings.storage.root / f".lamindb/_exclusion/{isettings.id.hex}"
-            )
-            if exclusion_dir.exists():
-                exclusion_dir.rmdir()
-        except PermissionError:
-            logger.warning(
-                "Did not have permission to delete SQLite file:"
-                f" {isettings._sqlite_file}"
-            )
-            pass
-    if isettings.is_remote:
-        logger.warning("manually delete your remote instance on lamin.ai")
-    logger.warning(f"manually delete your stored data: {isettings.storage.root}")
-    # unset the global instance settings
-    if settings._instance_exists and isettings.slug == settings.instance.slug:
-        if settings._instance_settings_path.exists():
-            settings._instance_settings_path.unlink()
-        settings._instance_settings = None
-
-
-def delete(instance_name: str, force: bool = False) -> Optional[int]:
-    """Delete a LaminDB instance."""
-    if "/" in instance_name:
-        logger.warning(
-            "Deleting the instance of another user is currently not supported with the"
-            " CLI. Please provide only the instance name when deleting an instance ('/'"
-            " delimiter not allowed)."
-        )
-        raise ValueError("Invalid instance name: '/' delimiter not allowed.")
-    instance_slug = f"{settings.user.handle}/{instance_name}"
-    if not force:
-        valid_responses = ["y", "yes"]
-        user_input = (
-            input(f"Are you sure you want to delete instance {instance_slug}? (y/n) ")
-            .strip()
-            .lower()
-        )
-        if user_input not in valid_responses:
-            return -1
-    if settings._instance_exists and settings.instance.name == instance_name:
-        isettings = settings.instance
+            self.instance
+            return True
+        # this is implicit logic that catches if no instance is loaded
+        except SystemExit:
+            return False
+
+    def __repr__(self) -> str:
+        """Rich string representation."""
+        repr = self.user.__repr__()
+        repr += f"\nAuto-connect in Python: {self.auto_connect}\n"
+        if self._instance_exists:
+            repr += self.instance.__repr__()
+        else:
+            repr += "\nNo instance connected"
+        return repr
+
+
+def get_env_name():
+    if "LAMIN_ENV" in os.environ:
+        return os.environ["LAMIN_ENV"]
     else:
-        settings_file = instance_settings_file(instance_name, settings.user.handle)
-        if not settings_file.exists():
-            logger.warning(
-                "could not delete as instance settings do not exist locally. did you"
-                " provide a wrong instance name? could you try loading it?"
-            )
-            return None
-        isettings = load_instance_settings(settings_file)
-    logger.info(f"deleting instance {instance_slug}")
-    delete_by_isettings(isettings)
-    return None
+        return "prod"
+
+
+settings = SetupSettings()
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_django.py` & `lamindb_setup-0.70.0/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_exportdb.py` & `lamindb_setup-0.70.0/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_importdb.py` & `lamindb_setup-0.70.0/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_init_instance.py` & `lamindb_setup-0.70.0/lamindb_setup/_init_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         from .core._hub_core import delete_instance_record as delete_instance_record
 
         if isettings is not None:
             delete_by_isettings(isettings)
             delete_instance_record(isettings.id)
             isettings._get_settings_file().unlink(missing_ok=True)  # type: ignore
         if ssettings is not None:
-            delete_storage_record(ssettings.uuid)  # type: ignore
+            delete_storage_record(ssettings._uuid)  # type: ignore
         raise e
     return None
 
 
 def load_from_isettings(
     isettings: InstanceSettings,
     *,
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_migrate.py` & `lamindb_setup-0.70.0/lamindb_setup/_migrate.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 def check_whether_migrations_in_sync(db_version_str: str):
     from importlib import metadata
 
     try:
         installed_version_str = metadata.version("lamindb")
     except metadata.PackageNotFoundError:
         return None
+    if db_version_str is None:
+        logger.warning("no lamindb version stored to compare with installed version")
+        return None
     installed_version = version.parse(installed_version_str)
     db_version = version.parse(db_version_str)
     if (
         installed_version.major < db_version.major
         or installed_version.minor < db_version.minor
     ):
         db_version_lower = f"{db_version.major}.{db_version.minor}"
@@ -79,15 +82,15 @@
         instance_is_on_hub = instance is not None
         if instance_is_on_hub:
             # double check that user is an admin, otherwise will fail below
             # without idempotence
             collaborator = call_with_fallback_auth(
                 select_collaborator,
                 instance_id=instance_id_str,
-                account_id=settings.user.uuid,
+                account_id=settings.user._uuid,
             )
             if collaborator is None or collaborator["role"] != "admin":
                 raise SystemExit(
                     "❌ Only admins can deploy migrations, please ensure that you're an"
                     f" admin: https://lamin.ai/{settings.instance.slug}/settings"
                 )
             # we need lamindb to be installed, otherwise we can't populate the version
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_register_instance.py` & `lamindb_setup-0.70.0/lamindb_setup/_register_instance.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     if not _check_instance_setup() and not _test:
         setup_django(isettings)
 
     ssettings = settings.instance.storage
     if ssettings._uid is None and _test:
         # because django isn't up, we can't get it from the database
         ssettings._uid = base62(8)
-    ssettings._uuid = init_storage_hub(ssettings)
+    ssettings._uuid_ = init_storage_hub(ssettings)
     init_instance_hub(isettings)
     isettings._persist()
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_schema.py` & `lamindb_setup-0.70.0/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_setup_user.py` & `lamindb_setup-0.70.0/lamindb_setup/_setup_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     if handle is None:
         logger.success(f"logged in with handle {user_handle} (uid: {user_id})")
     else:
         logger.success(f"logged in with email {user_settings.email} (uid: {user_id})")
     user_settings.uid = user_id
     user_settings.handle = user_handle
     user_settings.name = user_name
-    user_settings.uuid = user_uuid
+    user_settings._uuid = user_uuid
     user_settings.access_token = access_token
     save_user_settings(user_settings)
 
     if settings._instance_exists and _check_instance_setup():
         register_user(user_settings)
 
     settings._user_settings = None
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.70.0/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_hub_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,22 @@
 def _delete_storage_record(storage_uuid: UUID, client: Client) -> None:
     if storage_uuid is None:
         return None
     logger.important(f"deleting storage {storage_uuid.hex}")
     client.table("storage").delete().eq("id", storage_uuid.hex).execute()
 
 
+def update_instance_record(instance_uuid: UUID, fields: Dict) -> None:
+    from ._hub_crud import update_instance
+
+    return call_with_fallback_auth(
+        update_instance, instance_id=instance_uuid.hex, instance_fields=fields
+    )
+
+
 def init_storage(
     ssettings: StorageSettings,
 ) -> UUID:
     return call_with_fallback_auth(
         _init_storage,
         ssettings=ssettings,
     )
@@ -66,32 +74,32 @@
     # in the future, we could also encode a prefix to model local storage
     # locations
     # f"{prefix}{root}"
     id = uuid.uuid5(uuid.NAMESPACE_URL, root)
     fields = dict(
         id=id.hex,
         lnid=ssettings.uid,
-        created_by=settings.user.uuid.hex,  # type: ignore
+        created_by=settings.user._uuid.hex,  # type: ignore
         root=root,
         region=ssettings.region,
         type=ssettings.type,
         aws_account_id=ssettings._aws_account_id,
         description=ssettings._description,
     )
     client.table("storage").upsert(fields).execute()
     return id
 
 
-def delete_instance(identifier: Union[UUID, str]):
+def delete_instance(identifier: Union[UUID, str], require_empty: bool = True) -> None:
     """Fully delete an instance in the hub.
 
     This function deletes the relevant instance and storage records in the hub,
     conditional on the emptiness of the storage location.
     """
-    from .upath import check_s3_storage_location_empty, create_path, hosted_buckets
+    from .upath import check_storage_is_empty, create_path
     from ._settings_storage import mark_storage_root
 
     if isinstance(identifier, UUID):
         instance_with_storage = call_with_fallback_auth(
             select_instance_by_id_with_storage,
             instance_id=identifier,
         )
@@ -99,27 +107,30 @@
         owner, name = identifier.split("/")
         instance_with_storage = call_with_fallback_auth(
             select_instance_by_owner_name,
             owner=owner,
             name=name,
         )
 
-    if instance_with_storage is not None:
+    if instance_with_storage is None:
+        logger.warning("instance not found")
+        return None
+
+    if require_empty:
         root_string = instance_with_storage["storage"]["root"]
         # gate storage and instance deletion on empty storage location for
-        # both hosted and non-hosted s3 instances
-        if root_string.startswith("s3://"):
-            root_path = create_path(root_string)
-            # only mark hosted instances
-            if root_string.startswith(hosted_buckets):
-                mark_storage_root(root_path)
-            check_s3_storage_location_empty(root_path)
-
-        delete_instance_record(UUID(instance_with_storage["id"]))
-        delete_storage_record(UUID(instance_with_storage["storage_id"]))
+        root_path = create_path(root_string)
+        mark_storage_root(root_path)  # address permission error
+        account_for_sqlite_file = instance_with_storage["db_scheme"] is None
+        check_storage_is_empty(
+            root_path, account_for_sqlite_file=account_for_sqlite_file
+        )
+    delete_instance_record(UUID(instance_with_storage["id"]))
+    delete_storage_record(UUID(instance_with_storage["storage_id"]))
+    return None
 
 
 def delete_instance_record(
     instance_id: UUID,
 ) -> None:
     return call_with_fallback_auth(
         _delete_instance_record,
@@ -136,17 +147,17 @@
 
     try:
         lamindb_version = metadata.version("lamindb")
     except metadata.PackageNotFoundError:
         lamindb_version = None
     fields = dict(
         id=isettings.id.hex,
-        account_id=settings.user.uuid.hex,  # type: ignore
+        account_id=settings.user._uuid.hex,  # type: ignore
         name=isettings.name,
-        storage_id=isettings.storage.uuid.hex,  # type: ignore
+        storage_id=isettings.storage._uuid.hex,  # type: ignore
         schema_str=isettings._schema_str,
         lamindb_version=lamindb_version,
         public=False,
     )
     if isettings.dialect != "sqlite":
         db_dsn = LaminDsnModel(db=isettings.db)
         fields.update(
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_settings_storage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,317 +1,317 @@
 import os
 import shutil
+from lamin_utils import logger
 from pathlib import Path
-from typing import Literal, Optional, Set, Tuple
+from typing import Any, Optional, Union, Literal
+from ._aws_storage import find_closest_aws_region
+from appdirs import AppDirs
+from ._settings_save import save_system_storage_settings
+from ._settings_store import system_storage_settings_file
+from .upath import LocalPathClasses, UPath, create_path, convert_pathlike
 from uuid import UUID
-from ._hub_client import call_with_fallback
-from ._hub_crud import select_account_handle_name_by_lnid
-from lamin_utils import logger
-from .cloud_sqlite_locker import (
-    InstanceLockedException,
-    EXPIRATION_TIME,
-)
-from ._hub_utils import LaminDsnModel, LaminDsn
-from ._settings_save import save_instance_settings
-from ._settings_storage import StorageSettings
-from ._settings_store import current_instance_settings_file, instance_settings_file
-from .upath import UPath
-
-
-def sanitize_git_repo_url(repo_url: str) -> str:
-    assert repo_url.startswith("https://")
-    return repo_url.replace(".git", "")
+import string
+import secrets
+from .types import UPathStr
+from .upath import hosted_regions
+
+
+DIRS = AppDirs("lamindb", "laminlabs")
+IS_INITIALIZED_KEY = ".lamindb/_is_initialized"
+
+
+def base62(n_char: int) -> str:
+    """Like nanoid without hyphen and underscore."""
+    alphabet = string.digits + string.ascii_letters.swapcase()
+    id = "".join(secrets.choice(alphabet) for i in range(n_char))
+    return id
+
+
+def get_storage_region(storage_root: UPathStr) -> Optional[str]:
+    storage_root_str = str(storage_root)
+    if storage_root_str.startswith("s3://"):
+        import botocore.session as session
+        from botocore.config import Config
+        from botocore.exceptions import NoCredentialsError
+
+        # strip the prefix and any suffixes of the bucket name
+        bucket = storage_root_str.replace("s3://", "").split("/")[0]
+        s3_session = session.get_session()
+        s3_client = s3_session.create_client("s3")
+        try:
+            response = s3_client.head_bucket(Bucket=bucket)
+        except NoCredentialsError:  # deal with anonymous access
+            s3_client = s3_session.create_client(
+                "s3", config=Config(signature_version=session.UNSIGNED)
+            )
+            response = s3_client.head_bucket(Bucket=bucket)
+        storage_region = response["ResponseMetadata"].get("HTTPHeaders", {})[
+            "x-amz-bucket-region"
+        ]
+        # if we want to except botcore.exceptions.ClientError to reformat an
+        # error message, this is how to do test for the "NoSuchBucket" error:
+        #     exc.response["Error"]["Code"] == "NoSuchBucket"
+    else:
+        storage_region = None
+    return storage_region
+
+
+def mark_storage_root(root: UPathStr):
+    # we need to touch a 0-byte object in folder-like storage location on S3 to avoid
+    # permission errors from leveraging s3fs on an empty hosted storage location
+    # for consistency, we write this file everywhere
+    root_upath = convert_pathlike(root)
+    mark_upath = root_upath / IS_INITIALIZED_KEY
+    mark_upath.touch()
+
+
+def init_storage(root: UPathStr) -> "StorageSettings":
+    if root is None:
+        raise ValueError("`storage` argument can't be `None`")
+    root_str = str(root)  # ensure we have a string
+    uid = base62(8)
+    region = None
+    lamin_env = os.getenv("LAMIN_ENV")
+    if root_str.startswith("create-s3"):
+        if root_str != "create-s3":
+            assert "--" in root_str, "example: `create-s3--eu-central-1`"
+            region = root_str.replace("create-s3--", "")
+        if region is None:
+            region = find_closest_aws_region()
+        else:
+            if region not in hosted_regions:
+                raise ValueError(f"region has to be one of {hosted_regions}")
+        if lamin_env is None or lamin_env == "prod":
+            root_str = f"s3://lamin-{region}/{uid}"
+        else:
+            root_str = f"s3://lamin-hosted-test/{uid}"
+    elif root_str.startswith(("gs://", "s3://")):
+        pass
+    else:  # local path
+        try:
+            _ = Path(root_str)
+        except Exception as e:
+            logger.error("`storage` is not a valid local, GCP storage or AWS S3 path")
+            raise e
+    ssettings = StorageSettings(uid=uid, root=root_str, region=region)
+    if ssettings.type_is_cloud:
+        from ._hub_core import init_storage as init_storage_hub
+
+        ssettings._description = f"Created as default storage for instance {uid}"
+        ssettings._uuid_ = init_storage_hub(ssettings)
+        logger.important(f"registered storage: {ssettings.root_as_str}")
+    mark_storage_root(ssettings.root)
+    return ssettings
+
+
+def _process_cache_path(cache_path: Union[str, Path, UPath, None]):
+    if cache_path is None or cache_path == "null":
+        return None
+    cache_dir = UPath(cache_path)
+    if not isinstance(cache_dir, LocalPathClasses):
+        raise ValueError("cache dir should be a local path.")
+    if cache_dir.exists() and not cache_dir.is_dir():
+        raise ValueError("cache dir should be a directory.")
+    return cache_dir
 
 
-class InstanceSettings:
-    """Instance settings."""
+class StorageSettings:
+    """Manage cloud or local storage settings."""
 
     def __init__(
         self,
-        id: UUID,  # instance id/uuid
-        owner: str,  # owner handle
-        name: str,  # instance name
-        storage: StorageSettings,  # storage location
-        uid: Optional[str] = None,  # instance uid/lnid
-        db: Optional[str] = None,  # DB URI
-        schema: Optional[str] = None,  # comma-separated string of schema names
-        git_repo: Optional[str] = None,  # a git repo URL
+        root: UPathStr,
+        region: Optional[str] = None,
+        uid: Optional[str] = None,
+        uuid: Optional[UUID] = None,
+        access_token: Optional[str] = None,
     ):
-        from ._hub_utils import validate_db_arg
-
-        self._id: UUID = id
-        self._owner: str = owner
-        self._name: str = name
-        self._uid: Optional[str] = uid
-        self._storage: StorageSettings = storage
-        validate_db_arg(db)
-        self._db: Optional[str] = db
-        self._schema_str: Optional[str] = schema
-        self._git_repo = None if git_repo is None else sanitize_git_repo_url(git_repo)
+        self._uid = uid
+        self._uuid_ = uuid
+        self._root_init = convert_pathlike(root)
+        if isinstance(self._root_init, LocalPathClasses):  # local paths
+            (self._root_init / ".lamindb").mkdir(parents=True, exist_ok=True)
+            self._root_init = self._root_init.resolve()
+        self._root = None
+        self._aws_account_id: Optional[int] = None
+        self._description: Optional[str] = None
+        # we don't yet infer region here to make init fast
+        self._region = region
+        # would prefer to type below as Registry, but need to think through import order
+        self._record: Optional[Any] = None
+        # cache settings
+        self._storage_settings_file = system_storage_settings_file()
+        if self._storage_settings_file.exists():
+            from dotenv import dotenv_values
+
+            cache_path = dotenv_values(self._storage_settings_file)[
+                "lamindb_cache_path"
+            ]
+            self._cache_dir = _process_cache_path(cache_path)
+        else:
+            self._cache_dir = None
+        # save access_token here for use in self.root
+        self.access_token = access_token
 
-    def __repr__(self):
-        """Rich string representation."""
-        representation = f"Current instance: {self.slug}"
-        attrs = ["owner", "name", "storage", "db", "schema", "git_repo"]
-        for attr in attrs:
-            value = getattr(self, attr)
-            if attr == "storage":
-                representation += f"\n- storage root: {value.root_as_str}"
-                representation += f"\n- storage region: {value.region}"
-            elif attr == "db":
-                if self.dialect != "sqlite":
-                    model = LaminDsnModel(db=value)
-                    db_print = LaminDsn.build(
-                        scheme=model.db.scheme,
-                        user=model.db.user,
-                        password="***",
-                        host="***",
-                        port=model.db.port,
-                        database=model.db.database,
-                    )
-                else:
-                    db_print = value
-                representation += f"\n- {attr}: {db_print}"
-            else:
-                representation += f"\n- {attr}: {value}"
-        return representation
-
-    @property
-    def owner(self) -> str:
-        """Instance owner. A user or organization account handle."""
-        return self._owner
-
-    @property
-    def name(self) -> str:
-        """Instance name."""
-        return self._name
-
-    @property
-    def identifier(self) -> str:
-        """Unique semantic identifier."""
-        logger.warning(
-            "InstanceSettings.identifier is deprecated and will be removed, use"
-            " InstanceSettings.slug instead"
-        )
-        return self.slug
-
-    @property
-    def slug(self) -> str:
-        """Unique semantic identifier of form `"{account_handle}/{instance_name}"`."""
-        return f"{self.owner}/{self.name}"
+        # local storage
+        self._has_local = False
+        self._local = None
 
     @property
-    def git_repo(self) -> Optional[str]:
-        """Sync transforms with scripts in git repository.
-
-        Provide the full git repo URL.
-        """
-        return self._git_repo
+    def id(self) -> int:
+        """Storage id."""
+        return self.record.id
 
     @property
-    def id(self) -> UUID:
-        """The internal instance id."""
-        return self._id
+    def _uuid(self) -> Optional[UUID]:
+        """Lamin's internal storage uuid."""
+        return self._uuid_
 
     @property
     def uid(self) -> Optional[str]:
-        """The user-facing instance id."""
+        """Storage id."""
+        if self._uid is None:
+            self._uid = self.record.uid
         return self._uid
 
     @property
-    def schema(self) -> Set[str]:
-        """Schema modules in addition to core schema."""
-        if self._schema_str is None:
-            return {}  # type: ignore
-        else:
-            return {schema for schema in self._schema_str.split(",") if schema != ""}
+    def _mark_storage_root(self) -> UPath:
+        return self.root / IS_INITIALIZED_KEY
 
     @property
-    def _sqlite_file(self) -> UPath:
-        """SQLite file."""
-        return self.storage.key_to_filepath(f"{self.id.hex}.lndb")
+    def record(self) -> Any:
+        """Storage record."""
+        if self._record is None:
+            # dynamic import because of import order
+            from lnschema_core.models import Storage
+            from ._settings import settings
 
-    @property
-    def _sqlite_file_local(self) -> Path:
-        """Local SQLite file."""
-        return self.storage.cloud_to_local_no_update(self._sqlite_file)
-
-    def _update_cloud_sqlite_file(self, unlock_cloud_sqlite: bool = True) -> None:
-        """Upload the local sqlite file to the cloud file."""
-        if self._is_cloud_sqlite:
-            sqlite_file = self._sqlite_file
-            logger.warning(
-                f"updating & unlocking cloud SQLite '{sqlite_file}' of instance"
-                f" '{self.slug}'"
-            )
-            cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
-            sqlite_file.upload_from(cache_file, print_progress=True)  # type: ignore
-            cloud_mtime = sqlite_file.modified.timestamp()  # type: ignore
-            # this seems to work even if there is an open connection
-            # to the cache file
-            os.utime(cache_file, times=(cloud_mtime, cloud_mtime))
-            if unlock_cloud_sqlite:
-                self._cloud_sqlite_locker.unlock()
-
-    def _update_local_sqlite_file(self, lock_cloud_sqlite: bool = True) -> None:
-        """Download the cloud sqlite file if it is newer than local."""
-        if self._is_cloud_sqlite:
-            logger.warning(
-                "updating local SQLite & locking cloud SQLite (sync back & unlock:"
-                " lamin close)"
-            )
-            if lock_cloud_sqlite:
-                self._cloud_sqlite_locker.lock()
-                self._check_sqlite_lock()
-            sqlite_file = self._sqlite_file
-            cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
-            sqlite_file.synchronize(cache_file, print_progress=True)  # type: ignore
-
-    def _check_sqlite_lock(self):
-        if not self._cloud_sqlite_locker.has_lock:
-            locked_by = self._cloud_sqlite_locker._locked_by
-            lock_msg = "Cannot load the instance, it is locked by "
-            user_info = call_with_fallback(
-                select_account_handle_name_by_lnid,
-                lnid=locked_by,
+            self._record = Storage.objects.using(settings._using_key).get(
+                root=self.root_as_str
             )
-            if user_info is None:
-                lock_msg += f"uid: '{locked_by}'."
-            else:
-                lock_msg += (
-                    f"'{user_info['handle']}' (uid: '{locked_by}', name:"
-                    f" '{user_info['name']}')."
-                )
-            lock_msg += (
-                " The instance will be automatically unlocked after"
-                f" {int(EXPIRATION_TIME/3600/24)}d of no activity."
-            )
-            raise InstanceLockedException(lock_msg)
+        return self._record
+
+    def __repr__(self):
+        """String rep."""
+        s = f"root='{self.root_as_str}', uid='{self.uid}'"
+        if self._uuid is not None:
+            s += f", uuid='{self._uuid.hex}'"
+        return f"StorageSettings({s})"
+
+    @property
+    def root(self) -> UPath:
+        """Root storage location."""
+        if self._root is None:
+            # below makes network requests to get credentials
+            self._root = create_path(self._root_init, access_token=self.access_token)
+        return self._root
+
+    def _set_fs_kwargs(self, **kwargs):
+        """Set additional fsspec arguments for cloud root.
+
+        Example:
+
+        >>> ln.setup.settings.storage._set_fs_kwargs(  # any fsspec args
+        >>>    profile="some_profile", cache_regions=True
+        >>> )
+        """
+        if not isinstance(self._root, LocalPathClasses) and kwargs != {}:
+            self._root = UPath(self.root, **kwargs)
 
     @property
-    def db(self) -> str:
-        """Database connection string (URI)."""
-        if self._db is None:
-            # here, we want the updated sqlite file
-            # hence, we don't use self._sqlite_file_local()
-            # error_no_origin=False because on instance init
-            # the sqlite file is not yet in the cloud
-            sqlite_filepath = self.storage.cloud_to_local(
-                self._sqlite_file, error_no_origin=False
-            )
-            return f"sqlite:///{sqlite_filepath}"
-        else:
-            return self._db
+    def root_as_str(self) -> str:
+        """Formatted root string."""
+        return self._root_init.as_posix().rstrip("/")
 
     @property
-    def dialect(self) -> Literal["sqlite", "postgresql"]:
-        """SQL dialect."""
-        if self._db is None or self._db.startswith("sqlite://"):
-            return "sqlite"
+    def cache_dir(
+        self,
+    ) -> UPath:
+        """Cache root, a local directory to cache cloud files."""
+        if "LAMIN_CACHE_DIR" in os.environ:
+            cache_dir = UPath(os.environ["LAMIN_CACHE_DIR"])
+        elif self._cache_dir is None:
+            cache_dir = UPath(DIRS.user_cache_dir)
         else:
-            assert self._db.startswith("postgresql"), f"Unexpected DB value: {self._db}"
-            return "postgresql"
+            cache_dir = self._cache_dir
+        cache_dir.mkdir(parents=True, exist_ok=True)
+        return cache_dir
+
+    @cache_dir.setter
+    def cache_dir(self, cache_dir: UPathStr):
+        """Set cache root."""
+        from lamindb_setup import settings
+
+        if settings.instance._is_cloud_sqlite:
+            src_sqlite_file = settings.instance._sqlite_file_local
+        else:
+            src_sqlite_file = None
+
+        save_cache_dir = self._cache_dir
+
+        new_cache_dir = _process_cache_path(cache_dir)
+        if new_cache_dir is not None:
+            new_cache_dir.mkdir(parents=True, exist_ok=True)
+            new_cache_dir = new_cache_dir.resolve()
+        self._cache_dir = new_cache_dir
+
+        try:
+            if src_sqlite_file is not None:
+                dst_sqlite_file = settings.instance._sqlite_file_local
+                dst_sqlite_file.parent.mkdir(parents=True, exist_ok=True)
+                if dst_sqlite_file.exists():
+                    dst_sqlite_file.unlink()
+                shutil.move(src_sqlite_file, dst_sqlite_file)  # type: ignore
+            save_system_storage_settings(self._cache_dir, self._storage_settings_file)
+        except Exception as e:
+            self._cache_dir = save_cache_dir
+            raise e
 
     @property
-    def session(self):
-        raise NotImplementedError
+    def type_is_cloud(self) -> bool:
+        """`True` if `storage_root` is in cloud, `False` otherwise."""
+        return self.type != "local"
 
     @property
-    def _is_cloud_sqlite(self) -> bool:
-        # can we make this a private property, Sergei?
-        # as it's not relevant to the user
-        """Is this a cloud instance with sqlite db."""
-        return self.dialect == "sqlite" and self.storage.is_cloud
+    def region(self) -> Optional[str]:
+        """Storage region."""
+        if self._region is None:
+            self._region = get_storage_region(self.root_as_str)
+        return self._region
 
     @property
-    def _cloud_sqlite_locker(self):
-        # avoid circular import
-        from .cloud_sqlite_locker import empty_locker, get_locker
+    def type(self) -> Literal["local", "s3", "gs"]:
+        """AWS S3 vs. Google Cloud vs. local.
 
-        if self._is_cloud_sqlite:
-            try:
-                return get_locker(self)
-            except PermissionError:
-                logger.warning("read-only access - did not access locker")
-                return empty_locker
-        else:
-            return empty_locker
+        Returns the protocol as a string: "local", "s3", "gs".
+        """
+        import fsspec
 
-    @property
-    def storage(self) -> StorageSettings:
-        """Low-level access to storage location."""
-        return self._storage
-
-    @property
-    def is_remote(self) -> bool:
-        """Boolean indicating if an instance has no local component."""
-        if not self.storage.is_cloud:
-            return False
-
-        def is_local_uri(uri: str):
-            if "@localhost:" in uri:
-                return True
-            if "@0.0.0.0:" in uri:
-                return True
-            if "@127.0.0.1" in uri:
-                return True
-            return False
-
-        if self.dialect == "postgresql":
-            if is_local_uri(self.db):
-                return False
-        # returns True for cloud SQLite
-        # and remote postgres
-        return True
-
-    def _get_settings_file(self) -> Path:
-        return instance_settings_file(self.name, self.owner)
-
-    def _persist(self) -> None:
-        assert self.name is not None
-
-        filepath = self._get_settings_file()
-        # persist under filepath for later reference
-        save_instance_settings(self, filepath)
-        # persist under current file for auto load
-        shutil.copy2(filepath, current_instance_settings_file())
-        # persist under settings class for same session reference
-        # need to import here to avoid circular import
-        from ._settings import settings
-
-        settings._instance_settings = self
-
-    def _init_db(self):
-        from .django import setup_django
-
-        setup_django(self, init=True)
-
-    def _load_db(
-        self, do_not_lock_for_laminapp_admin: bool = False
-    ) -> Tuple[bool, str]:
-        # Is the database available and initialized as LaminDB?
-        # returns a tuple of status code and message
-        if self.dialect == "sqlite" and not self._sqlite_file.exists():
-            legacy_file = self.storage.key_to_filepath(f"{self.name}.lndb")
-            if legacy_file.exists():
-                raise RuntimeError(
-                    "The SQLite file has been renamed!\nPlease rename your SQLite file"
-                    f" {legacy_file} to {self._sqlite_file}"
-                )
-            return False, f"SQLite file {self._sqlite_file} does not exist"
-        from lamindb_setup import settings  # to check user
-        from .django import setup_django
-
-        # lock in all cases except if do_not_lock_for_laminapp_admin is True and
-        # user is `laminapp-admin`
-        # value doesn't matter if not a cloud sqlite instance
-        lock_cloud_sqlite = self._is_cloud_sqlite and (
-            not do_not_lock_for_laminapp_admin
-            or settings.user.handle != "laminapp-admin"
-        )
-        # we need the local sqlite to setup django
-        self._update_local_sqlite_file(lock_cloud_sqlite=lock_cloud_sqlite)
-        # setting up django also performs a check for migrations & prints them
-        # as warnings
-        # this should fail, e.g., if the db is not reachable
-        setup_django(self)
-        return True, ""
+        convert = {"file": "local"}
+        protocol = fsspec.utils.get_protocol(self.root_as_str)
+        return convert.get(protocol, protocol)  # type: ignore
+
+    def key_to_filepath(self, filekey: Union[Path, UPath, str]) -> UPath:
+        """Cloud or local filepath from filekey."""
+        return self.root / filekey
+
+    def cloud_to_local(self, filepath: Union[Path, UPath], **kwargs) -> UPath:
+        """Local (cache) filepath from filepath."""
+        local_filepath = self.cloud_to_local_no_update(filepath)  # type: ignore
+        if isinstance(filepath, UPath) and not isinstance(filepath, LocalPathClasses):
+            local_filepath.parent.mkdir(parents=True, exist_ok=True)
+            filepath.synchronize(local_filepath, **kwargs)
+        return local_filepath
+
+    # conversion to Path via cloud_to_local() would trigger download
+    # of remote file to cache if there already is one
+    # in pure write operations that update the cloud, we don't want this
+    # hence, we manually construct the local file path
+    # using the `.parts` attribute in the following line
+    def cloud_to_local_no_update(self, filepath: UPath) -> UPath:
+        if isinstance(filepath, UPath) and not isinstance(filepath, LocalPathClasses):
+            return self.cache_dir.joinpath(filepath._url.netloc, *filepath.parts[1:])  # type: ignore # noqa
+        return filepath
+
+    def local_filepath(self, filekey: Union[Path, UPath, str]) -> UPath:
+        """Local (cache) filepath from filekey: `local(filepath(...))`."""
+        return self.cloud_to_local(self.key_to_filepath(filekey))
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_settings_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,9 +91,9 @@
     settings = UserSettings()
     settings.email = store.email
     settings.password = store.password if store.password != "null" else None
     settings.access_token = store.access_token
     settings.uid = store.uid
     settings.handle = store.handle if store.handle != "null" else "anonymous"
     settings.name = store.name if store.name != "null" else None
-    settings.uuid = UUID(store.uuid) if store.uuid != "null" else None
+    settings._uuid = UUID(store.uuid) if store.uuid != "null" else None
     return settings
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_settings_save.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 type = str
             if "__" not in store_key:
                 if store_key == "storage_root":
                     value = settings.storage.root_as_str
                 elif store_key == "storage_region":
                     value = settings.storage.region
                 else:
-                    if store_key in {"db", "schema_str", "name_"}:
+                    if store_key in {"db", "schema_str", "name_", "uuid"}:
                         settings_key = f"_{store_key.rstrip('_')}"
                     else:
                         settings_key = store_key
                     value = getattr(settings, settings_key)
                 if value is None:
                     value = "null"
                 elif isinstance(value, UUID):
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_settings_instance.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,349 +1,371 @@
+from __future__ import annotations
+
 import os
 import shutil
-from lamin_utils import logger
+from .upath import LocalPathClasses, convert_pathlike
 from pathlib import Path
-from typing import Any, Optional, Union, Literal
-from ._aws_storage import find_closest_aws_region
-from appdirs import AppDirs
-from ._settings_save import save_system_storage_settings
-from ._settings_store import system_storage_settings_file
-from .upath import LocalPathClasses, UPath, create_path, convert_pathlike
+from typing import Literal, Optional, Set, Tuple
 from uuid import UUID
-import string
-import secrets
-from .types import UPathStr
-from .upath import hosted_regions
-
-
-DIRS = AppDirs("lamindb", "laminlabs")
-IS_INITIALIZED_KEY = ".lamindb/_is_initialized"
-
-
-def base62(n_char: int) -> str:
-    """Like nanoid without hyphen and underscore."""
-    alphabet = string.digits + string.ascii_letters.swapcase()
-    id = "".join(secrets.choice(alphabet) for i in range(n_char))
-    return id
-
-
-def get_storage_region(storage_root: UPathStr) -> Optional[str]:
-    storage_root_str = str(storage_root)
-    if storage_root_str.startswith("s3://"):
-        import botocore.session as session
-        from botocore.config import Config
-        from botocore.exceptions import NoCredentialsError
-
-        # strip the prefix and any suffixes of the bucket name
-        bucket = storage_root_str.replace("s3://", "").split("/")[0]
-        s3_session = session.get_session()
-        s3_client = s3_session.create_client("s3")
-        try:
-            response = s3_client.head_bucket(Bucket=bucket)
-        except NoCredentialsError:  # deal with anonymous access
-            s3_client = s3_session.create_client(
-                "s3", config=Config(signature_version=session.UNSIGNED)
-            )
-            response = s3_client.head_bucket(Bucket=bucket)
-        storage_region = response["ResponseMetadata"].get("HTTPHeaders", {})[
-            "x-amz-bucket-region"
-        ]
-        # if we want to except botcore.exceptions.ClientError to reformat an
-        # error message, this is how to do test for the "NoSuchBucket" error:
-        #     exc.response["Error"]["Code"] == "NoSuchBucket"
-    else:
-        storage_region = None
-    return storage_region
-
-
-def mark_storage_root(root: UPathStr):
-    # we need to touch a 0-byte object in the storage location to avoid
-    # permission errors from leveraging s3fs on an empty hosted storage location
-    root_upath = convert_pathlike(root)
-    mark_upath = root_upath / IS_INITIALIZED_KEY
-    mark_upath.touch()
-
-
-def init_storage(root: UPathStr) -> "StorageSettings":
-    if root is None:
-        raise ValueError("`storage` argument can't be `None`")
-    root_str = str(root)  # ensure we have a string
-    uid = base62(8)
-    region = None
-    lamin_env = os.getenv("LAMIN_ENV")
-    if root_str.startswith("create-s3"):
-        if root_str != "create-s3":
-            assert "--" in root_str, "example: `create-s3--eu-central-1`"
-            region = root_str.replace("create-s3--", "")
-        if region is None:
-            region = find_closest_aws_region()
-        else:
-            if region not in hosted_regions:
-                raise ValueError(f"region has to be one of {hosted_regions}")
-        if lamin_env is None or lamin_env == "prod":
-            root_str = f"s3://lamin-{region}/{uid}"
-        else:
-            root_str = f"s3://lamin-hosted-test/{uid}"
-    elif root_str.startswith(("gs://", "s3://")):
-        pass
-    else:  # local path
-        try:
-            _ = Path(root_str)
-        except Exception as e:
-            logger.error("`storage` is not a valid local, GCP storage or AWS S3 path")
-            raise e
-    ssettings = StorageSettings(uid=uid, root=root_str, region=region)
-    if ssettings.is_cloud:
-        from ._hub_core import init_storage as init_storage_hub
-
-        ssettings._description = f"Created as default storage for instance {uid}"
-        ssettings._uuid = init_storage_hub(ssettings)
-        logger.important(f"registered storage: {ssettings.root_as_str}")
-    if ssettings.is_cloud and root_str.startswith("create-s3"):
-        mark_storage_root(ssettings.root)
-    return ssettings
-
-
-def _process_cache_path(cache_path: Union[str, Path, UPath, None]):
-    if cache_path is None or cache_path == "null":
-        return None
-    cache_dir = UPath(cache_path)
-    if not isinstance(cache_dir, LocalPathClasses):
-        raise ValueError("cache dir should be a local path.")
-    if cache_dir.exists() and not cache_dir.is_dir():
-        raise ValueError("cache dir should be a directory.")
-    return cache_dir
+from ._hub_client import call_with_fallback
+from ._hub_crud import select_account_handle_name_by_lnid
+from lamin_utils import logger
+from .cloud_sqlite_locker import (
+    InstanceLockedException,
+    EXPIRATION_TIME,
+)
+from ._hub_utils import LaminDsnModel, LaminDsn
+from ._settings_save import save_instance_settings
+from ._settings_storage import StorageSettings
+from ._settings_store import current_instance_settings_file, instance_settings_file
+from .upath import UPath
+
+LOCAL_STORAGE_ROOT_WARNING = (
+    "No local storage root found, set via `ln.setup.settings.instance.local_storage ="
+    " local_root`"
+)
+
+
+def sanitize_git_repo_url(repo_url: str) -> str:
+    assert repo_url.startswith("https://")
+    return repo_url.replace(".git", "")
 
 
-class StorageSettings:
-    """Manage cloud or local storage settings."""
+class InstanceSettings:
+    """Instance settings."""
 
     def __init__(
         self,
-        root: UPathStr,
-        region: Optional[str] = None,
-        is_hybrid: bool = False,  # refers to storage mode
-        uid: Optional[str] = None,
-        uuid: Optional[UUID] = None,
-        access_token: Optional[str] = None,
+        id: UUID,  # instance id/uuid
+        owner: str,  # owner handle
+        name: str,  # instance name
+        storage: StorageSettings,  # storage location
+        local_storage: bool = False,  # default to local storage
+        uid: Optional[str] = None,  # instance uid/lnid
+        db: Optional[str] = None,  # DB URI
+        schema: Optional[str] = None,  # comma-separated string of schema names
+        git_repo: Optional[str] = None,  # a git repo URL
     ):
-        self._uid = uid
-        self._uuid = uuid
-        self._is_hybrid = is_hybrid
-        self._root_init = convert_pathlike(root)
-        if isinstance(self._root_init, LocalPathClasses):  # local paths
-            self._root_init.mkdir(parents=True, exist_ok=True)
-            self._root_init = self._root_init.resolve()
-        self._root = None
-        self._remote_root = None
-        self._aws_account_id: Optional[int] = None
-        self._description: Optional[str] = None
-        # we don't yet infer region here to make init fast
-        self._region = region
-        # would prefer to type below as Registry, but need to think through import order
-        self._record: Optional[Any] = None
-        # cache settings
-        self._storage_settings_file = system_storage_settings_file()
-        if self._storage_settings_file.exists():
-            from dotenv import dotenv_values
-
-            cache_path = dotenv_values(self._storage_settings_file)[
-                "lamindb_cache_path"
-            ]
-            self._cache_dir = _process_cache_path(cache_path)
-        else:
-            self._cache_dir = None
-        # save access_token here for use in self.root
-        self.access_token = access_token
+        from ._hub_utils import validate_db_arg
 
-    @property
-    def id(self) -> int:
-        """Storage id."""
-        return self.record.id
+        self._id: UUID = id
+        self._owner: str = owner
+        self._name: str = name
+        self._uid: Optional[str] = uid
+        self._storage: StorageSettings = storage
+        validate_db_arg(db)
+        self._db: Optional[str] = db
+        self._schema_str: Optional[str] = schema
+        self._git_repo = None if git_repo is None else sanitize_git_repo_url(git_repo)
+        # local storage
+        self._local_storage_on = local_storage
+        self._local_storage = None
 
-    @property
-    def uuid(self) -> Optional[UUID]:
-        """Storage uuid."""
-        return self._uuid
+    def __repr__(self):
+        """Rich string representation."""
+        representation = f"Current instance: {self.slug}"
+        attrs = ["owner", "name", "storage", "db", "schema", "git_repo"]
+        for attr in attrs:
+            value = getattr(self, attr)
+            if attr == "storage":
+                representation += f"\n- storage root: {value.root_as_str}"
+                representation += f"\n- storage region: {value.region}"
+            elif attr == "db":
+                if self.dialect != "sqlite":
+                    model = LaminDsnModel(db=value)
+                    db_print = LaminDsn.build(
+                        scheme=model.db.scheme,
+                        user=model.db.user,
+                        password="***",
+                        host="***",
+                        port=model.db.port,
+                        database=model.db.database,
+                    )
+                else:
+                    db_print = value
+                representation += f"\n- {attr}: {db_print}"
+            else:
+                representation += f"\n- {attr}: {value}"
+        return representation
 
     @property
-    def uid(self) -> Optional[str]:
-        """Storage id."""
-        if self._uid is None:
-            self._uid = self.record.uid
-        return self._uid
+    def owner(self) -> str:
+        """Instance owner. A user or organization account handle."""
+        return self._owner
 
     @property
-    def record(self) -> Any:
-        """Storage record."""
-        if self._record is None:
-            # dynamic import because of import order
-            from lnschema_core.models import Storage
-            from ._settings import settings
-
-            if not self.is_hybrid:
-                self._record = Storage.objects.using(settings._using_key).get(
-                    root=self.root_as_str
-                )
-            else:
-                # this has to be redone
-                records = Storage.objects.filter(type="local").all()
-                for record in records:
-                    if Path(record.root).exists():
-                        self._record = record
-                        logger.warning("found local storage location")
-                        break
-        return self._record
+    def name(self) -> str:
+        """Instance name."""
+        return self._name
 
-    def __repr__(self):
-        """String rep."""
-        s = f"root='{self.root_as_str}', uid='{self.uid}'"
-        if self.uuid is not None:
-            s += f", uuid='{self.uuid.hex}'"
-        return f"StorageSettings({s})"
+    def _search_local_root(self):
+        from lnschema_core.models import Storage
+
+        records = Storage.objects.filter(type="local").all()
+        for record in records:
+            if Path(record.root).exists():
+                self._local_storage = StorageSettings(record.root)
+                logger.important(f"defaulting to local storage: {record}")
+                break
+        if self._local_storage is None:
+            logger.warning(LOCAL_STORAGE_ROOT_WARNING)
 
     @property
-    def is_hybrid(self) -> bool:
-        """Qualifies storage mode.
+    def local_storage(self) -> StorageSettings:
+        """Default local storage.
 
-        A storage location can be local, in the cloud, or hybrid. See
-        :attr:`~lamindb.setup.core.StorageSettings.type`.
+        Warning: Only enable if you're sure you want to use the more complicated
+        storage mode across local & cloud locations.
 
-        Hybrid means that a default local storage location is backed by an
-        optional cloud storage location.
-        """
-        return self._is_hybrid
+        As an admin, enable via: `ln.setup.settings.instance.local_storage =
+        local_root`.
 
-    @property
-    def root(self) -> UPath:
-        """Root storage location."""
-        if self._root is None:
-            if not self.is_hybrid:
-                # below makes network requests to get credentials
-                root_path = create_path(self._root_init, access_token=self.access_token)
-            else:
-                # this is a local path
-                root_path = create_path(self.record.root)
-            self._root = root_path
-        return self._root
+        If enabled, you'll save artifacts to a default local storage
+        location at :attr:`~lamindb.setup.settings.InstanceSettings.local_storage`.
 
-    @property
-    def remote_root(self) -> UPath:
-        """Remote storage location. Only needed for hybrid storage."""
-        if not self.is_hybrid:
-            raise ValueError("remote_root is only defined for hybrid storage")
-        if self._remote_root is None:
-            self._remote_root = create_path(
-                self._root_init, access_token=self.access_token
+        Upon passing `upload=True` in `artifact.save(upload=True)`, you upload the
+        artifact to the default cloud storage location:
+        :attr:`~lamindb.setup.core.InstanceSettings.storage`.
+        """
+        if not self._local_storage_on:
+            raise ValueError("Local storage is not enabled for this instance.")
+        if self._local_storage is None:
+            self._search_local_root()
+        if self._local_storage is None:
+            raise ValueError(LOCAL_STORAGE_ROOT_WARNING)
+        return self._local_storage
+
+    @local_storage.setter
+    def local_storage(self, local_root: Path):
+        from ._hub_core import update_instance_record
+        from .._init_instance import register_storage
+
+        self._search_local_root()
+        if self._local_storage is not None:
+            raise ValueError(
+                "You already configured a local storage root for this instance in this"
+                f" environment: {self.local_storage.root}"
             )
-        return self._remote_root
+        local_root = convert_pathlike(local_root)
+        assert isinstance(local_root, LocalPathClasses)
+        self._local_storage = StorageSettings(local_root)  # type: ignore
+        register_storage(self._local_storage)  # type: ignore
+        self._local_storage_on = True
+        update_instance_record(self.id, {"storage_mode": "hybrid"})
 
-    def _set_fs_kwargs(self, **kwargs):
-        """Set additional fsspec arguments for cloud root.
+    @property
+    def slug(self) -> str:
+        """Unique semantic identifier of form `"{account_handle}/{instance_name}"`."""
+        return f"{self.owner}/{self.name}"
 
-        Example:
+    @property
+    def git_repo(self) -> Optional[str]:
+        """Sync transforms with scripts in git repository.
 
-        >>> ln.setup.settings.storage._set_fs_kwargs(  # any fsspec args
-        >>>    profile="some_profile", cache_regions=True
-        >>> )
+        Provide the full git repo URL.
         """
-        if not isinstance(self._root, LocalPathClasses) and kwargs != {}:
-            self._root = UPath(self.root, **kwargs)
+        return self._git_repo
 
     @property
-    def root_as_str(self) -> str:
-        """Formatted root string."""
-        return self._root_init.as_posix().rstrip("/")
+    def id(self) -> UUID:
+        """The internal instance id."""
+        return self._id
 
     @property
-    def cache_dir(
-        self,
-    ) -> UPath:
-        """Cache root, a local directory to cache cloud files."""
-        if "LAMIN_CACHE_DIR" in os.environ:
-            cache_dir = UPath(os.environ["LAMIN_CACHE_DIR"])
-        elif self._cache_dir is None:
-            cache_dir = UPath(DIRS.user_cache_dir)
-        else:
-            cache_dir = self._cache_dir
-        cache_dir.mkdir(parents=True, exist_ok=True)
-        return cache_dir
-
-    @cache_dir.setter
-    def cache_dir(self, cache_dir: UPathStr):
-        """Set cache root."""
-        from lamindb_setup import settings
+    def uid(self) -> Optional[str]:
+        """The user-facing instance id."""
+        return self._uid
 
-        if settings.instance._is_cloud_sqlite:
-            src_sqlite_file = settings.instance._sqlite_file_local
+    @property
+    def schema(self) -> Set[str]:
+        """Schema modules in addition to core schema."""
+        if self._schema_str is None:
+            return {}  # type: ignore
         else:
-            src_sqlite_file = None
+            return {schema for schema in self._schema_str.split(",") if schema != ""}
 
-        save_cache_dir = self._cache_dir
+    @property
+    def _sqlite_file(self) -> UPath:
+        """SQLite file."""
+        return self.storage.key_to_filepath(f"{self.id.hex}.lndb")
 
-        new_cache_dir = _process_cache_path(cache_dir)
-        if new_cache_dir is not None:
-            new_cache_dir.mkdir(parents=True, exist_ok=True)
-            new_cache_dir = new_cache_dir.resolve()
-        self._cache_dir = new_cache_dir
+    @property
+    def _sqlite_file_local(self) -> Path:
+        """Local SQLite file."""
+        return self.storage.cloud_to_local_no_update(self._sqlite_file)
 
-        try:
-            if src_sqlite_file is not None:
-                dst_sqlite_file = settings.instance._sqlite_file_local
-                dst_sqlite_file.parent.mkdir(parents=True, exist_ok=True)
-                if dst_sqlite_file.exists():
-                    dst_sqlite_file.unlink()
-                shutil.move(src_sqlite_file, dst_sqlite_file)  # type: ignore
-            save_system_storage_settings(self._cache_dir, self._storage_settings_file)
-        except Exception as e:
-            self._cache_dir = save_cache_dir
-            raise e
+    def _update_cloud_sqlite_file(self, unlock_cloud_sqlite: bool = True) -> None:
+        """Upload the local sqlite file to the cloud file."""
+        if self._is_cloud_sqlite:
+            sqlite_file = self._sqlite_file
+            logger.warning(
+                f"updating & unlocking cloud SQLite '{sqlite_file}' of instance"
+                f" '{self.slug}'"
+            )
+            cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
+            sqlite_file.upload_from(cache_file, print_progress=True)  # type: ignore
+            cloud_mtime = sqlite_file.modified.timestamp()  # type: ignore
+            # this seems to work even if there is an open connection
+            # to the cache file
+            os.utime(cache_file, times=(cloud_mtime, cloud_mtime))
+            if unlock_cloud_sqlite:
+                self._cloud_sqlite_locker.unlock()
+
+    def _update_local_sqlite_file(self, lock_cloud_sqlite: bool = True) -> None:
+        """Download the cloud sqlite file if it is newer than local."""
+        if self._is_cloud_sqlite:
+            logger.warning(
+                "updating local SQLite & locking cloud SQLite (sync back & unlock:"
+                " lamin close)"
+            )
+            if lock_cloud_sqlite:
+                self._cloud_sqlite_locker.lock()
+                self._check_sqlite_lock()
+            sqlite_file = self._sqlite_file
+            cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
+            sqlite_file.synchronize(cache_file, print_progress=True)  # type: ignore
+
+    def _check_sqlite_lock(self):
+        if not self._cloud_sqlite_locker.has_lock:
+            locked_by = self._cloud_sqlite_locker._locked_by
+            lock_msg = "Cannot load the instance, it is locked by "
+            user_info = call_with_fallback(
+                select_account_handle_name_by_lnid,
+                lnid=locked_by,
+            )
+            if user_info is None:
+                lock_msg += f"uid: '{locked_by}'."
+            else:
+                lock_msg += (
+                    f"'{user_info['handle']}' (uid: '{locked_by}', name:"
+                    f" '{user_info['name']}')."
+                )
+            lock_msg += (
+                " The instance will be automatically unlocked after"
+                f" {int(EXPIRATION_TIME/3600/24)}d of no activity."
+            )
+            raise InstanceLockedException(lock_msg)
 
     @property
-    def is_cloud(self) -> bool:
-        """`True` if `storage_root` is in cloud, `False` otherwise."""
-        return self.type != "local"
+    def db(self) -> str:
+        """Database connection string (URI)."""
+        if self._db is None:
+            # here, we want the updated sqlite file
+            # hence, we don't use self._sqlite_file_local()
+            # error_no_origin=False because on instance init
+            # the sqlite file is not yet in the cloud
+            sqlite_filepath = self.storage.cloud_to_local(
+                self._sqlite_file, error_no_origin=False
+            )
+            return f"sqlite:///{sqlite_filepath}"
+        else:
+            return self._db
 
     @property
-    def region(self) -> Optional[str]:
-        """Storage region."""
-        if self._region is None:
-            self._region = get_storage_region(self.root_as_str)
-        return self._region
+    def dialect(self) -> Literal["sqlite", "postgresql"]:
+        """SQL dialect."""
+        if self._db is None or self._db.startswith("sqlite://"):
+            return "sqlite"
+        else:
+            assert self._db.startswith("postgresql"), f"Unexpected DB value: {self._db}"
+            return "postgresql"
 
     @property
-    def type(self) -> Literal["local", "s3", "gs"]:
-        """AWS S3 vs. Google Cloud vs. local.
-
-        Returns the protocol as a string: "local", "s3", "gs".
-        """
-        import fsspec
+    def _is_cloud_sqlite(self) -> bool:
+        # can we make this a private property, Sergei?
+        # as it's not relevant to the user
+        """Is this a cloud instance with sqlite db."""
+        return self.dialect == "sqlite" and self.storage.type_is_cloud
+
+    @property
+    def _cloud_sqlite_locker(self):
+        # avoid circular import
+        from .cloud_sqlite_locker import empty_locker, get_locker
+
+        if self._is_cloud_sqlite:
+            try:
+                return get_locker(self)
+            except PermissionError:
+                logger.warning("read-only access - did not access locker")
+                return empty_locker
+        else:
+            return empty_locker
 
-        convert = {"file": "local"}
-        protocol = fsspec.utils.get_protocol(self.root_as_str)
-        return convert.get(protocol, protocol)  # type: ignore
-
-    def key_to_filepath(self, filekey: Union[Path, UPath, str]) -> UPath:
-        """Cloud or local filepath from filekey."""
-        return self.root / filekey
-
-    def cloud_to_local(self, filepath: Union[Path, UPath], **kwargs) -> UPath:
-        """Local (cache) filepath from filepath."""
-        local_filepath = self.cloud_to_local_no_update(filepath)  # type: ignore
-        if isinstance(filepath, UPath) and not isinstance(filepath, LocalPathClasses):
-            local_filepath.parent.mkdir(parents=True, exist_ok=True)
-            filepath.synchronize(local_filepath, **kwargs)
-        return local_filepath
-
-    # conversion to Path via cloud_to_local() would trigger download
-    # of remote file to cache if there already is one
-    # in pure write operations that update the cloud, we don't want this
-    # hence, we manually construct the local file path
-    # using the `.parts` attribute in the following line
-    def cloud_to_local_no_update(self, filepath: UPath) -> UPath:
-        if isinstance(filepath, UPath) and not isinstance(filepath, LocalPathClasses):
-            return self.cache_dir.joinpath(filepath._url.netloc, *filepath.parts[1:])  # type: ignore # noqa
-        return filepath
-
-    def local_filepath(self, filekey: Union[Path, UPath, str]) -> UPath:
-        """Local (cache) filepath from filekey: `local(filepath(...))`."""
-        return self.cloud_to_local(self.key_to_filepath(filekey))
+    @property
+    def storage(self) -> StorageSettings:
+        """Low-level access to storage location."""
+        return self._storage
+
+    @property
+    def is_remote(self) -> bool:
+        """Boolean indicating if an instance has no local component."""
+        if not self.storage.type_is_cloud:
+            return False
+
+        def is_local_uri(uri: str):
+            if "@localhost:" in uri:
+                return True
+            if "@0.0.0.0:" in uri:
+                return True
+            if "@127.0.0.1" in uri:
+                return True
+            return False
+
+        if self.dialect == "postgresql":
+            if is_local_uri(self.db):
+                return False
+        # returns True for cloud SQLite
+        # and remote postgres
+        return True
+
+    def _get_settings_file(self) -> Path:
+        return instance_settings_file(self.name, self.owner)
+
+    def _persist(self) -> None:
+        assert self.name is not None
+
+        filepath = self._get_settings_file()
+        # persist under filepath for later reference
+        save_instance_settings(self, filepath)
+        # persist under current file for auto load
+        shutil.copy2(filepath, current_instance_settings_file())
+        # persist under settings class for same session reference
+        # need to import here to avoid circular import
+        from ._settings import settings
+
+        settings._instance_settings = self
+
+    def _init_db(self):
+        from .django import setup_django
+
+        setup_django(self, init=True)
+
+    def _load_db(
+        self, do_not_lock_for_laminapp_admin: bool = False
+    ) -> Tuple[bool, str]:
+        # Is the database available and initialized as LaminDB?
+        # returns a tuple of status code and message
+        if self.dialect == "sqlite" and not self._sqlite_file.exists():
+            legacy_file = self.storage.key_to_filepath(f"{self.name}.lndb")
+            if legacy_file.exists():
+                raise RuntimeError(
+                    "The SQLite file has been renamed!\nPlease rename your SQLite file"
+                    f" {legacy_file} to {self._sqlite_file}"
+                )
+            return False, f"SQLite file {self._sqlite_file} does not exist"
+        from lamindb_setup import settings  # to check user
+        from .django import setup_django
+
+        # lock in all cases except if do_not_lock_for_laminapp_admin is True and
+        # user is `laminapp-admin`
+        # value doesn't matter if not a cloud sqlite instance
+        lock_cloud_sqlite = self._is_cloud_sqlite and (
+            not do_not_lock_for_laminapp_admin
+            or settings.user.handle != "laminapp-admin"
+        )
+        # we need the local sqlite to setup django
+        self._update_local_sqlite_file(lock_cloud_sqlite=lock_cloud_sqlite)
+        # setting up django also performs a check for migrations & prints them
+        # as warnings
+        # this should fail, e.g., if the db is not reachable
+        setup_django(self)
+        return True, ""
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_settings_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """User email."""
     password: Optional[str] = None
     """API key or legacy password."""
     access_token: Optional[str] = None
     """User access token."""
     uid: str = "null"
     """Universal user ID."""
-    uuid: Optional[UUID] = None
+    _uuid: Optional[UUID] = None
     """Lamin's internal user ID."""
     name: Optional[str] = None
     """Full name."""
 
     def __repr__(self) -> str:
         """Rich string representation."""
         representation = f"Current user: {self.handle}"
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.70.0/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.70.0/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/django.py` & `lamindb_setup-0.70.0/lamindb_setup/core/django.py`

 * *Files 9% similar despite different names*

```diff
@@ -99,7 +99,10 @@
         call_command("migrate", verbosity=2)
         isettings._update_cloud_sqlite_file(unlock_cloud_sqlite=False)
     elif init:
         call_command("migrate", verbosity=0)
 
     global IS_SETUP
     IS_SETUP = True
+
+    if isettings._local_storage_on:
+        isettings._search_local_root()
```

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/hashing.py` & `lamindb_setup-0.70.0/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/lamindb_setup/core/upath.py` & `lamindb_setup-0.70.0/lamindb_setup/core/upath.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # we are not documenting UPath here because it's documented at lamindb.UPath
 """Paths & file systems."""
 
+from __future__ import annotations
+
 import os
 from datetime import datetime, timezone
 import botocore.session
 from pathlib import Path, PurePosixPath
 from typing import Literal, Dict
 import fsspec
 from itertools import islice
@@ -684,24 +686,38 @@
     return size, hash, hash_type, n_objects
 
 
 class InstanceNotEmpty(Exception):
     pass
 
 
-def check_s3_storage_location_empty(root: UPathStr) -> None:
+# is as fast as boto3: https://lamin.ai/laminlabs/lamindata/transform/krGp3hT1f78N5zKv
+def check_storage_is_empty(
+    root: UPathStr, *, raise_error: bool = True, account_for_sqlite_file: bool = False
+) -> int:
     root_upath = convert_pathlike(root)
     root_string = root_upath.as_posix()  # type: ignore
     # we currently touch a 0-byte file in the root of a hosted storage location
     # ({storage_root}/.lamindb/_is_initialized) during storage initialization
     # since path.fs.find raises a PermissionError on empty hosted
     # subdirectories (see lamindb_setup/core/_settings_storage/init_storage).
-    n_touched_objects = 0
-    if root_string.startswith(hosted_buckets):
-        n_touched_objects = 1
+    n_offset_objects = 1  # because of touched dummy file, see mark_storage_root()
+    if account_for_sqlite_file:
+        n_offset_objects += 1  # because of SQLite file
     objects = root_upath.fs.find(root_string)
     n_objects = len(objects)
-    if n_objects > n_touched_objects:
-        raise InstanceNotEmpty(
-            f"""storage location contains objects;
-            {compute_file_tree(root_upath)[0]}"""
-        )
+    n_diff = n_objects - n_offset_objects
+    ask_for_deletion = (
+        "delete them prior to deleting the instance"
+        if raise_error
+        else "consider deleting them"
+    )
+    message = (
+        f"Storage location contains {n_objects} objects "
+        f"({n_offset_objects} ignored) - {ask_for_deletion}\n{objects}"
+    )
+    if n_diff > 0:
+        if raise_error:
+            raise InstanceNotEmpty(message)
+        else:
+            logger.warning(message)
+    return n_diff
```

### Comparing `lamindb_setup-0.69.5/noxfile.py` & `lamindb_setup-0.70.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/pyproject.toml` & `lamindb_setup-0.70.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.70.0/tests/hub-cloud/test_connect_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,27 @@
 import os
 from postgrest.exceptions import APIError
 import pytest
 from laminhub_rest.core.collaborator._add_collaborator import add_collaborator
 from laminhub_rest.core.collaborator._delete_collaborator import delete_collaborator
-
+from lamindb_setup._connect_instance import InstanceNotFoundError
 import lamindb_setup as ln_setup
 from lamindb_setup.core._hub_client import connect_hub_with_auth
 from lamindb_setup.core._hub_crud import update_instance
 
 
-def test_load_remote_instance():
-    ln_setup.login("testuser1")
-    ln_setup.delete("load_remote_instance", force=True)
-    ln_setup.init(storage="s3://lamindb-ci/load_remote_instance", _test=True)
-    assert ln_setup.settings.instance.name == "load_remote_instance"
-    ln_setup.connect("testuser1/load_remote_instance", _test=True)
-    assert ln_setup.settings.instance.id is not None
-    assert ln_setup.settings.instance.storage.is_cloud
-    assert (
-        ln_setup.settings.instance.storage.root_as_str
-        == "s3://lamindb-ci/load_remote_instance"
-    )
-    assert (
-        ln_setup.settings.instance._sqlite_file.as_posix()
-        == f"s3://lamindb-ci/load_remote_instance/{ln_setup.settings.instance.id.hex}.lndb"  # noqa
-    )
-    ln_setup.close()
+# @pytest.fixture
+# def create_remote_test_instance():
+#     ln_setup.login("testuser1")
+#     ln_setup.init(storage="s3://lamindb-ci/load_remote_instance", _test=True)
+#     yield
+#     ln_setup.delete("load_remote_instance", force=True)
 
 
-def test_load_after_revoked_access():
+def test_connect_after_revoked_access():
     # can't currently test this on staging as I'm missing the accounts
     if os.getenv("LAMIN_ENV") == "prod":
         ln_setup.login("testuser1@lamin.ai")
         admin_hub = connect_hub_with_auth()
         try:
             # if a previous test run failed, this will
             # error with a violation of a unique constraint
@@ -52,33 +41,26 @@
         assert (
             ln_setup.settings.instance.storage.root_as_str
             == "s3://lamindb-setup-private-bucket"
         )
         delete_collaborator(
             "laminlabs",
             "static-test-instance-private-sqlite",
-            ln_setup.settings.user.uuid,
+            ln_setup.settings.user._uuid,
             admin_hub,
         )
         # make the instance private
-        with pytest.raises(SystemExit) as error:
+        with pytest.raises(InstanceNotFoundError):
             ln_setup.connect(
                 "https://lamin.ai/laminlabs/static-test-instance-private-sqlite",
                 _test=True,
             )
-        assert (
-            error.exconly()
-            == "SystemExit: 'laminlabs/static-test-instance-private-sqlite' not"
-            " loadable: 'instance-not-reachable'\n"
-            "Check your permissions:"
-            " https://lamin.ai/laminlabs/static-test-instance-private-sqlite?tab=collaborators"  # noqa
-        )
 
 
-def test_load_after_private_public_switch():
+def test_connect_after_private_public_switch():
     # can't currently test this on staging as I'm missing the accounts
     if os.getenv("LAMIN_ENV") == "prod":
         # this assumes that testuser1 is an admin of static-test-instance-private-sqlite
         ln_setup.login("testuser1@lamin.ai")
         ln_setup.connect(
             "https://lamin.ai/laminlabs/static-test-instance-private-sqlite", _test=True
         )
@@ -87,15 +69,15 @@
         update_instance(
             instance_id=ln_setup.settings.instance.id,
             instance_fields={"public": False},
             client=admin_hub,
         )
         # attempt to load instance with non-collaborator user
         ln_setup.login("testuser2")
-        with pytest.raises(SystemExit):
+        with pytest.raises(InstanceNotFoundError):
             ln_setup.connect(
                 "https://lamin.ai/laminlabs/static-test-instance-private-sqlite",
                 _test=True,
             )
         # make the instance public
         update_instance(
             instance_id=ln_setup.settings.instance.id,
@@ -110,15 +92,15 @@
         update_instance(
             instance_id=ln_setup.settings.instance.id,
             instance_fields={"public": False},
             client=admin_hub,
         )
 
 
-def test_load_with_db_parameter():
+def test_connect_with_db_parameter():
     if os.getenv("LAMIN_ENV") == "prod":
         # take a write-level access collaborator
         ln_setup.login("testuser1")
         # test load from hub
         ln_setup.connect("laminlabs/lamindata", _test=True)
         assert "root" in ln_setup.settings.instance.db
         # test load from provided db argument
```

### Comparing `lamindb_setup-0.69.5/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.70.0/tests/hub-cloud/test_init_instance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from pathlib import Path
-from typing import Dict, Optional, Tuple
 from uuid import UUID
 
 import pytest
 
 import lamindb_setup as ln_setup
 from lamindb_setup.core._hub_client import connect_hub_with_auth
+from lamindb_setup.core._hub_core import _connect_instance
 from lamindb_setup.core._hub_crud import (
     Client,
     select_account_by_handle,
-    select_db_user_by_instance,
     select_instance_by_name,
-    select_instance_by_owner_name,
 )
 
 pgurl = "postgresql://postgres:pwd@0.0.0.0:5432/pgtest"
 
 
 def delete_instance(
     id: str,
@@ -31,74 +29,52 @@
 def get_hub_client():
     ln_setup.login("testuser2")
     hub = connect_hub_with_auth()
     yield hub
     hub.auth.sign_out()
 
 
-def get_instance_and_dbuser_from_hub(
-    instance_name: str, hub: Client
-) -> Tuple[Optional[Dict[str, str]], Optional[Dict[str, str]]]:
-    assert ln_setup.settings.user.handle == "testuser2"
-    instance_account_storage = select_instance_by_owner_name(
-        "testuser2",
-        name=instance_name,
-        client=hub,
-    )
-    if instance_account_storage is not None:
-        _ = instance_account_storage.pop("account")
-        _ = instance_account_storage.pop("storage")
-        instance = instance_account_storage
-    else:
-        return None, None
-    db_user = select_db_user_by_instance(instance_id=instance["id"], client=hub)
-    return instance, db_user
-
-
 def test_init_instance_postgres_default_name(get_hub_client):
     hub = get_hub_client
     instance_name = "pgtest"
-    instance, _ = get_instance_and_dbuser_from_hub(instance_name, hub)
-    # if instance exists, delete it
-    if instance is not None:
-        delete_instance(instance["id"], hub)
-    ln_setup.delete("pgtest", force=True)
+    ln_setup.delete(instance_name, force=True)
     # now, run init
     ln_setup.init(storage="./mydatapg", db=pgurl, _test=True)
     assert ln_setup.settings.instance.slug == "testuser2/pgtest"
     ln_setup.register(_test=True)
     assert ln_setup.settings.instance.slug == "testuser2/pgtest"
     # and check
-    instance, db_user = get_instance_and_dbuser_from_hub(instance_name, hub)
+    instance, storage = _connect_instance(
+        owner="testuser2", name=instance_name, client=hub
+    )
     # hub checks
-    assert db_user is None
-    assert instance["name"] == "pgtest"
+    assert instance["db"].startswith("postgresql://none:none")
+    assert instance["name"] == instance_name
     assert instance["db_scheme"] == "postgresql"
     assert instance["db_host"] == "0.0.0.0"
     assert instance["db_port"] == 5432
     assert instance["db_database"] == "pgtest"
     # client checks
     assert ln_setup.settings.instance.id == UUID(instance["id"])
     assert ln_setup.settings.instance.name == "pgtest"
-    assert not ln_setup.settings.instance.storage.is_cloud
+    assert not ln_setup.settings.instance.storage.type_is_cloud
     assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
     assert ln_setup.settings.instance.dialect == "postgresql"
     assert ln_setup.settings.instance.db == pgurl
     assert (
         ln_setup.settings.instance.storage.root.as_posix()
         == Path("mydatapg").absolute().as_posix()
     )
-    delete_instance(instance["id"], hub)
-    ln_setup.delete("pgtest", force=True)
+    ln_setup.delete(instance_name, force=True)
 
 
 def test_init_instance_postgres_custom_name():
     ln_setup.init(storage="./mystorage", name="mydata2", db=pgurl, _test=True)
     assert ln_setup.settings.instance.name == "mydata2"
-    assert not ln_setup.settings.instance.storage.is_cloud
+    assert not ln_setup.settings.instance.storage.type_is_cloud
     assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
     assert ln_setup.settings.instance.dialect == "postgresql"
     assert ln_setup.settings.instance.db == pgurl
     assert (
         ln_setup.settings.instance.storage.root.as_posix()
         == Path("mystorage").absolute().as_posix()
     )
@@ -113,15 +89,15 @@
     )
     instance = select_instance_by_name(
         account_id=account["id"],
         name=ln_setup.settings.instance.name,
         client=hub,
     )
     assert ln_setup.settings.instance.id == UUID(instance["id"])
-    assert ln_setup.settings.storage.is_cloud
+    assert ln_setup.settings.storage.type_is_cloud
     assert (
         str(ln_setup.settings.storage.root)
         == "s3://lamindb-ci/init_instance_cloud_aws_us"
     )
     assert (
         ln_setup.settings.storage.root_as_str
         == "s3://lamindb-ci/init_instance_cloud_aws_us"
@@ -163,15 +139,15 @@
     instance = select_instance_by_name(
         account_id=account["id"],
         name=ln_setup.settings.instance.name,
         client=hub,
     )
     assert ln_setup.settings.instance.id == UUID(instance["id"])
     assert ln_setup.settings.instance.name == "local-sqlite-instance"
-    assert not ln_setup.settings.instance.storage.is_cloud
+    assert not ln_setup.settings.instance.storage.type_is_cloud
     assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
     assert ln_setup.settings.instance.dialect == "sqlite"
     ln_setup.delete("local-sqlite-instance", force=True)
     delete_instance(instance["id"], hub)
 
 
 def test_init_invalid_name():
```

### Comparing `lamindb_setup-0.69.5/tests/hub-local/conftest.py` & `lamindb_setup-0.70.0/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/tests/hub-local/test_all.py` & `lamindb_setup-0.70.0/tests/hub-local/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         return "user-exists"
     account_id = UUID(result_or_error[1])
     access_token = result_or_error[2]
     user_settings = UserSettings(
         handle=handle,
         email=email,
         password=result_or_error[0],
-        uuid=account_id,
+        _uuid=account_id,
         access_token=access_token,
     )
     if save_as_settings:
         save_user_settings(user_settings)
     return user_settings
 
 
@@ -73,15 +73,15 @@
 @pytest.fixture(scope="session")
 def create_testadmin1_session():  # -> Tuple[Client, UserSettings]
     email = "testadmin1@gmail.com"
     sign_up_user(email, "testadmin1", save_as_settings=True)
     with pytest.raises(AuthApiError):
         # test error with "User already registered"
         sign_up_user(email, "testadmin1")
-    account_id = ln_setup.settings.user.uuid
+    account_id = ln_setup.settings.user._uuid
     account = {
         "id": account_id.hex,
         "user_id": account_id.hex,
         "lnid": base62(8),
         "handle": "testadmin1",
     }
     # uses ln_setup.settings.user.access_token
@@ -92,16 +92,16 @@
 
 
 @pytest.fixture(scope="session")
 def create_testreader1_session():  # -> Tuple[Client, UserSettings]
     email = "testreader1@gmail.com"
     user_settings = sign_up_user(email, "testreader1")
     account = {
-        "id": user_settings.uuid.hex,
-        "user_id": user_settings.uuid.hex,
+        "id": user_settings._uuid.hex,
+        "user_id": user_settings._uuid.hex,
         "lnid": base62(8),
         "handle": "testreader1",
     }
     client = connect_hub_with_auth(access_token=user_settings.access_token)
     client.table("account").insert(account).execute()
     yield client, user_settings
     client.auth.sign_out()
@@ -124,15 +124,15 @@
     with pytest.raises(PermissionError) as error:
         ln_setup.connect("testadmin1/myinstance", _test=True)
     assert error.exconly().startswith(
         "PermissionError: No database access, please ask your admin"
     )
     db_collaborator = select_collaborator(
         instance_id=instance_id.hex,
-        account_id=ln_setup.settings.user.uuid.hex,
+        account_id=ln_setup.settings.user._uuid.hex,
         client=admin_client,
     )
     assert db_collaborator["role"] == "admin"
     assert db_collaborator["db_user_id"] is None
     db_dsn = LaminDsnModel(db=db_str)
     db_user_name = db_dsn.db.user
     db_user_password = db_dsn.db.password
@@ -140,30 +140,30 @@
         name="write",
         db_user_name=db_user_name,
         db_user_password=db_user_password,
         instance_id=instance_id,
         client=admin_client,
     )
     instance = select_instance_by_name(
-        account_id=ln_setup.settings.user.uuid,
+        account_id=ln_setup.settings.user._uuid,
         name="myinstance",
         client=admin_client,
     )
     yield instance
 
 
 def test_connection_string_decomp(create_myinstance, create_testadmin1_session):
     client, _ = create_testadmin1_session
     assert create_myinstance["db_scheme"] == "postgresql"
     assert create_myinstance["db_host"] == "fakeserver.xyz"
     assert create_myinstance["db_port"] == 5432
     assert create_myinstance["db_database"] == "mydb"
     db_collaborator = select_collaborator(
         instance_id=create_myinstance["id"],
-        account_id=ln_setup.settings.user.uuid.hex,
+        account_id=ln_setup.settings.user._uuid.hex,
         client=client,
     )
     assert db_collaborator["role"] == "admin"
     assert db_collaborator["db_user_id"] is None
 
 
 def test_db_user(
@@ -183,34 +183,34 @@
         instance_id=instance_id,
         client=reader_client,
     )
     assert db_user is None
     # check that testreader1 is not yet a collaborator
     db_collaborator = select_collaborator(
         instance_id=instance_id.hex,
-        account_id=reader_settings.uuid.hex,
+        account_id=reader_settings._uuid.hex,
         client=admin_client,
     )
     assert db_collaborator is None
     # now add testreader1 as a collaborator
     add_collaborator_by_ids(
-        account_id=reader_settings.uuid,
+        account_id=reader_settings._uuid,
         instance_id=instance_id,
         role="read",
         supabase_client=admin_client,
     )
     # check that this was successful and can be read by the reader
     db_collaborator = select_collaborator(
         instance_id=instance_id.hex,
-        account_id=reader_settings.uuid.hex,
+        account_id=reader_settings._uuid.hex,
         client=reader_client,
     )
     assert db_collaborator["role"] == "read"
     assert UUID(db_collaborator["instance_id"]) == instance_id
-    assert UUID(db_collaborator["account_id"]) == reader_settings.uuid
+    assert UUID(db_collaborator["account_id"]) == reader_settings._uuid
     assert db_collaborator["db_user_id"] is None
     # this alone doesn't set a db_user
     db_user = select_db_user_by_instance(
         instance_id=instance_id,
         client=reader_client,
     )
     assert db_user is None
```

### Comparing `lamindb_setup-0.69.5/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.70.0/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/tests/hub-prod/test_upath.py` & `lamindb_setup-0.70.0/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/tests/storage/test_hashing.py` & `lamindb_setup-0.70.0/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/tests/storage/test_storage_access.py` & `lamindb_setup-0.70.0/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/tests/storage/test_storage_basis.py` & `lamindb_setup-0.70.0/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/tests/storage/test_storage_stats.py` & `lamindb_setup-0.70.0/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.69.5/PKG-INFO` & `lamindb_setup-0.70.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.69.5
+Version: 0.70.0
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

