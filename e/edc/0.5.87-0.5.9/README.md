# Comparing `tmp/edc-0.5.87.tar.gz` & `tmp/edc-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.5.87.tar", last modified: Tue Apr 23 23:41:04 2024, max compression
+gzip compressed data, was "edc-0.5.9.tar", last modified: Thu Jul 20 02:51:26 2023, max compression
```

## Comparing `edc-0.5.87.tar` & `edc-0.5.9.tar`

### file list

```diff
@@ -1,82 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.077779 edc-0.5.87/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.87/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2024-02-13 18:05:12.000000 edc-0.5.87/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.87/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.87/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    67482 2024-04-23 23:40:55.000000 edc-0.5.87/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.87/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.87/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    44485 2024-04-23 23:41:04.077669 edc-0.5.87/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    40358 2024-02-13 18:05:12.000000 edc-0.5.87/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.057693 edc-0.5.87/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.061160 edc-0.5.87/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.87/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.87/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.87/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.061957 edc-0.5.87/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.87/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.87/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.87/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.87/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.063415 edc-0.5.87/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.87/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.87/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.87/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.87/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.87/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.87/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.87/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.87/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.068873 edc-0.5.87/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.87/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12978 2023-12-15 03:23:19.000000 edc-0.5.87/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)    15486 2023-11-13 00:42:59.000000 edc-0.5.87/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.87/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1531 2024-03-27 20:17:30.000000 edc-0.5.87/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.87/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6596 2023-11-13 00:42:59.000000 edc-0.5.87/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.87/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     9565 2023-08-04 04:47:01.000000 edc-0.5.87/docs/disaster_recovery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.87/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.87/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.87/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.87/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      643 2023-11-01 13:29:41.000000 edc-0.5.87/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.87/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.87/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.87/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.87/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.87/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.077061 edc-0.5.87/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    44485 2024-04-23 23:41:04.000000 edc-0.5.87/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1719 2024-04-23 23:41:04.000000 edc-0.5.87/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-04-23 23:41:04.000000 edc-0.5.87/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-27 20:17:39.000000 edc-0.5.87/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1929 2024-04-23 23:41:04.000000 edc-0.5.87/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2024-04-23 23:41:04.000000 edc-0.5.87/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.073047 edc-0.5.87/image/
--rw-r--r--   0 erikvw     (501) staff       (20)    34744 2023-11-22 02:41:32.000000 edc-0.5.87/image/administration_appointment.png
--rw-r--r--   0 erikvw     (501) staff       (20)    14449 2023-11-22 02:41:32.000000 edc-0.5.87/image/administration_button.png
--rw-r--r--   0 erikvw     (501) staff       (20)     4335 2023-11-22 02:41:32.000000 edc-0.5.87/image/administration_icon.png
--rw-r--r--   0 erikvw     (501) staff       (20)   157606 2023-11-22 02:41:32.000000 edc-0.5.87/image/appointments.png
--rw-r--r--   0 erikvw     (501) staff       (20)   157606 2023-11-22 02:41:32.000000 edc-0.5.87/image/appointments_annotated_top.png
--rw-r--r--   0 erikvw     (501) staff       (20)    15845 2023-11-22 02:41:32.000000 edc-0.5.87/image/appointments_changelist.png
--rw-r--r--   0 erikvw     (501) staff       (20)     4708 2023-11-22 02:41:32.000000 edc-0.5.87/image/down_arrow.png
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.87/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2023-09-26 19:26:40.000000 edc-0.5.87/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.076423 edc-0.5.87/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.87/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.87/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1158 2024-04-09 00:56:42.000000 edc-0.5.87/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4027 2024-02-11 18:40:59.000000 edc-0.5.87/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.87/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       55 2024-02-13 18:05:12.000000 edc-0.5.87/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.87/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.87/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      159 2024-03-27 20:17:30.000000 edc-0.5.87/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.87/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.87/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2933 2024-04-23 23:41:04.078202 edc-0.5.87/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-04-23 23:41:04.076751 edc-0.5.87/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.87/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.87/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.717582 edc-0.5.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    43780 2023-07-20 02:51:18.000000 edc-0.5.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-20 02:51:26.717726 edc-0.5.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37646 2023-07-12 23:55:42.000000 edc-0.5.9/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.704697 edc-0.5.9/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.707540 edc-0.5.9/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.9/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.9/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.9/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.708212 edc-0.5.9/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.9/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.9/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.9/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.9/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.709308 edc-0.5.9/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.713077 edc-0.5.9/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.9/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.9/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.9/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.9/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.9/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.9/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.9/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.9/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.9/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.9/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.9/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.9/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.9/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.9/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.9/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.9/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.9/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.9/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.9/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.714023 edc-0.5.9/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.9/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1917 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.714126 edc-0.5.9/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.9/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.9/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.716982 edc-0.5.9/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.9/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.9/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.9/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.9/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.9/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.9/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.9/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.9/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.9/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.9/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.9/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2960 2023-07-20 02:51:26.718140 edc-0.5.9/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.717373 edc-0.5.9/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.9/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.9/utils/get_edc_requirements.py
```

### Comparing `edc-0.5.87/.gitignore` & `edc-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/.pre-commit-config.yaml` & `edc-0.5.9/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.7
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 23.1.0
     hooks:
       - id: black
-        language_version: python3.11
+        language_version: python3.9
 
   - repo: https://github.com/pycqa/flake8
-    rev: 7.0.0
+    rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.13.2
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.4.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.34.0
+    rev: v1.30.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-0.5.87/CHANGES` & `edc-0.5.9/CHANGES`

 * *Files 22% similar despite different names*

```diff
@@ -1,707 +1,29 @@
 Changes
 -------
 
-0.5.87
-------
-- fix issue to prevent appointment creator from resetting appointment
-  datetime for appointments that are not NEW. (edc-appointment)
-
-0.5.86
-------
-- refresh medata on each render of subject dashboard is current.
-  Performance penalty is negligible (edc-metadata)
-- catch ObjectDoesNotExist and pass when validating ae_initial
-  outcome date if AeInitial relation does not exist.
-  (edc-adverse-event)
-
-0.5.85
-------
-- fix regression in site_consents where consent definitions were not
-  filtered by site before querying for consent model instances. This
-  resulted in irrelevant links to consents showing on the subject
-  dashboard. (edc-consent)
-- fix syntax error in popover templates.
-  (edc-prn, edc-subject-dashboard)
-- fix regression where action item button was not passing parent
-  reference model instance id to new form. For example, given the
-  sequence aeinitial->aefolllowup->aefollowup, the last aefollowup
-  action item pop over list item link was not passing the aeinitial
-  id to the add form for AeFollowup. (edc-action-item)
-
-0.5.84
-------
-- add gettext wrappers to field validator messages. (edc-model)
-- minor, allow import of show_urls from root __init__. (edc-utils)
-- remove edc-next-appointment as a default module
-
-0.5.83
------
-- improve consent definition validity period comparisons (edc-consent)
-
-0.5.82
------
- - allow action_identifier to be passed when creating an ActionItem
-   (edc-action-item)
- - also skip get_site_on_create() if self.site_id (edc-sites)
-
-0.5.81
-------
-- add `site` to signatures for get_consent_or_raise, etc
-  (edc-consent, edc-appointment, edc-crf)
-
-0.5.80
-------
-- fix issue where requisition rule group incorrectly tries to run rules
-  when appointment is missed. (edc-metadata)
-
-0.5.79
-------
-- minor, separate age from dob on subject dashboard (edc-subject-dashboard)
-
-0.5.78
-------
-- fix outdated call in view mixin to site_consents from
-  'get_consent_or_raise' to 'get_consents'. (edc-consent)
-- (edc-action-item)
-  - fix search field list not finding subject_identifier;
-  - check for action_identifier before looking up reference_obj.
-- bump to django-audit-fields 0.3.17
-- bump to django-multisite2 2.0.1
-- add management command `sync_sites` to manually sync and review
-  site related models from edc_sites, django_sites and multisite.
-  Also review ALLOWED_HOSTS for current settings file. (edc-sites)
-
-0.5.76
-------
-- fix regression where dynamic site middleware incorrectly tried to
-  determine site after calling get_response in __call__.
-  (django-multisite2)
-
-0.5.75
-------
-- fix export_model management command incorrectly enumerating model
-  names (edc-pdutils)
-- prefix regex strings with 'r' (edc-identifier, edc-lab)
-- (django-crypto-fields) 0.4.1
-  - major refactor
-  - use cache framework for encryption keys
-- (edc-consent)
-  - remove 'updates_by' from ConsentDefinition init and instead set
-    when registering the ConsentDefinition with site_consents.register.
-  - change 'updates' to only accept a ConsentDefinition
-  - update system checks that warn of duplicate versions
-    and period overlap when using the same proxy_for_model.
- - (django-multisite2)
-   - switch to django-multisite2
-   - major refactor
-   - add MULTISITE_REGISTER_POST_MIGRATE_SYNC_ALIAS settings attr
- - (edc-sites)
-   - require --settings when running migrate
-   - require MULTISITE_REGISTER_POST_MIGRATE_SYNC_ALIAS = False so
-     multisite post-migrate signal NOT be registered by multisite2
- - connect multisite2 post-migrate signal AFTER edc-site post migrate
-   signal (edc-appconfig)
-
-0.5.74
-------
-yanked because of edc-consent
-
-0.5.73
-------
-- Move fieldsets to modeladmin mixin (edc-adherence)
-- Django 4.2.11
-
-0.5.72
-------
-- add missing migrations (edc-locator, edc-visit-tracking)
-- replace deprecated dataframe manipulation for pandas v2.2. Add
-  ValueError exception if remove_illegal_characters() operates
-  on a non-str Series (edc-pdutils)
-- rename data dictionary field from "default" to "default_value"
-  (edc-data-dictionary)
-- change site_consent system checks that look for duration overlap
-  from errors to warnings (edc-consent)
- - get consent definition directly from site_consents on PRN
-   models that do not have access to a schedule (edc-prn)
-
-0.5.71
-------
-- refactor to handle multiple versions of consents and consents that
-  update previous versions (edc-consent)
-- query consent attr thru consent definition (edc-crf, edc-screening,
-  edc-visit-schedule)
-- use RequiresConsentModelAdminMixin for modeladmin classes that
-  require consent (edc-model-admin)
-
-0.5.70
-------
-- show field_cls.metadata in reference document (edc-form-describer)
-- use 'custom_name' to capture 3rd element of tuple in list_data,
-  if it exists. Add ListModelMixin2 and class to convert a choices
-  tuple to something the list_data loader can handle
-  (edc-list-data)
-- add iter to custom Choices class (edc-model-field)
-- change precision for ALP to 2 places, ALT to 2 places, magnesium to
-  2 places (edc-lab-results)
-- update precision on equalities for magnsium, uric acid, neutrophils
-  (edc-reportable)
-
-0.5.69
-------
-- fix timeuntil on aefollowup "description" template
-  (edc-adverse-event)
-
-0.5.68
-------
-- add missing action_identifier to extra kwargs coming from popover
-  (edc-action-item)
-- fix issue where runner fails if no fieldset defined in ModelAdmin.
-  Check get_related_visit_model_attr has value before calling.
-  (edc-form-runners)
-- check creatinine has value before attempting to calculate eGFR drop
-  (edc-egfr)
-- fix signature on get_next_related_visit to include
-  `include_interim=True` (edc-pharmacy, edc-visit-tracking)
-- change form validation error to use message from
-  ScheduledVisitWindowError when date is outside window period
-  (edc-appointment)
-- skip some form validation until report_datetime has value
-  (edc-visit-schedule)
-- get ConsentDefinition from Screening model if not enough
-  data to get from schedule.get_consent_definition
-  (edc-consent)
-
-0.5.67
-------
-- add `is_required_by_date` method to allow a metadata_rule user to
-  hardcode a date before which the rule always returns not_required
-  (edc-he)
-- fix issue where the action item popover template incorrectly gets
-  the color style from the Action instance instead of the Action
-  class (edc-action-item)
-
-0.5.66
-------
-- minor changes to system checks
-- update pre-commit config
-- force metadata_handler to create missing metadata,
-  allow_create=True (edc-metadata)
-- fix regression where visit_code and visit_code sequence are
-  incorrectly saved as booleans on the Issues model
-  (edc-form-runners)
-- fix timezone setting on to_local, to_utc (edc-utils)
-- check value of creatinine before calculating drop (edc-egfr)
-- fix how refill_end_datetime is set (edc-pharmacy)
-
-0.5.65
-------
-- remove fields reference_model and related_reference_model from ActionItem.
-  Fields already appear on ActionType. (edc-action_item)
-- display window period boundaries on changelist (edc-appointment)
-- skip system check if migrating (edc-sites)
-- fix run_form_runners command incorrectly including skipped models
-  (edc-form-runners)
-- bump to Django 4.2.10
-
-0.5.64
-------
-- remove redundant check from Holiday model (edc-facility)
-- fix render TmgButton when reference_obj is None by passing
-  subject_identifier (edc-adverse-event)
-- remove edc-model-wrapper, edc-subject-model-wrapper from
-  requirements
-- fix issue where missing CRF/Requisition metadata is not
-  created using subject dashboard's refresh button
-  (edc-metadata)
-- rework TMG dashboard, add navigation for TMG Role members
-  to navigate to new, open, closed TMG summaries from subject
-  dashboard and subject review dashboard (edc-adverse-event,
-  edc-subject-dashboard, edc-review-dashboard)
-- add Choices class and custom fields to accept standardized field
-  names and standardized categorical field values in choices as
-  metadata when building model classes for standardized forms.
-  (edc-model-fields)
-
-0.5.63
-------
-- minor fixes to templates (edc-dashboard, edc-subject-dashboard,
-  edc-navbar)
-- add system check against SubjectScheduleHistory and the OnSchedule
-  model (edc-visit-schedule, edc-appconfig)
-- management command to delete invalid onschedule instances
-  (edc-visit-schedule)
-- fix issue where form runner fails on PRN forms that do not
-  have visit schedule fields (edc-form-runners)
-
-0.5.62
-------
-- add checks to confirm reference_model matches (edc-action_item)
-- skip admin classes without custom modelform classes
-  (edc-form-runner)
-- fix modelform not finding site for PRN forms (edc-site)
-
-0.5.61
-------
-- add related_visit_model_cls attr to form validator mixin
-  (edc-visit-tracking)
--
-0.5.60
-------
-- fix regression on updating missed appointments in signal
-  (edc-appointment)
-- fix query on userprofile.role raising exception
-  (edc-auth)
-
-0.5.59
-------
-- use get_locator_model to access SUBJECT_LOCATOR_MODEL
-  settings attribute (edc_locator)
-
-0.5.58
-------
-- disabled refresh appointments and refresh data collection schedule
-  if multisite viewer or auditor (edc-subject-dashboard)
-
-0.5.57
-------
-- add `is_multisite_viewer` boolean to UserProfile model. This field
-  value replaces the use of a special codename for multisite data
-  view (edc-auth)
-- redirect to screening_listboard if not a registered subject in
-  view_on_site (edc-model-admin)
-- move refresh_appointments to utils, check appt_datetime is not
-  before previous appt (edc-appointment)
-- change DeathReportTmgSecond mixin to be used with a proxy of death
-  report tmg (edc-adverse-event)
-- Add subject consent buttons for listboards and subject-dashboards
-  (edc-subject-dashboard)
-- Rework resequencing when visit code sequences and dates not
-  correctly ordered (edc-appointment)
-- add schedule button to review listboard (edc-review-listboard)
-
-0.5.56
-------
-- add new app edc_appconfigs
-  - call all site global autodiscover() in ready
-  - register system checks that access site globals in ready
-  - register post-migrate signals that access site globals in ready
-- move NavbarItem class validation to system_checks. Rename
-  NavbarItem.append_item method to register (edc-navbar)
-- refactor edc_protocol, rename class to ResearchProtocolConfig
-  (edc-protocol)
-- minor changes to subject dashboard template (edc-subject-dashboard)
-- require consent definition as class attr on screening models
-  (edc-screening)
-- refactor notification, raise exception any entries, referred to
-  by Action classes, are missing from EMAIL_CONTACTS
-- wrap search form in button div (edc-listboard)
-
-0.5.55 yanked
--------------
-
-0.5.54 yanked
--------------
-- refactor to remove modelwrappers and other listboard and
-  dashboard improvements
-- refactor TMG listboard
-- refactor subject dashboard, screening and subject listboards
-
-0.5.53
-------
-- refactor edc-consent
-- AE PDF reports for changes in edc_pdf_reports:
-    - set `pdf_report_cls` on AE models (death report, AE initial)
-    - update modeladmin changelist (death report, AE initial)
-    - add urls from edc_pdf_reports
-    - See edc_pdf_reports README
-- user is now redirected to effect_ae changelists instead of AE
-  listboards. Remove effect_ae from administration section.
-  (changes from edc-adverse-event)
-- migrations for indexes triggered from other modules e.g.
-  edc-list-data, edc-model, etc
-- remove redundant edc-sites post-migrate signal
-- update edc_sites import paths
-
-0.5.51
-------
-- reset migrations. may need to review existing migrations before
-  updating (edc-form-runners)
-- split index migrations to avoid mem issues during migrations.
-  may need to review existing migrations before updating
-  (edc-data-manager)
-- fix decimal_places==0 treated as falsy (edc-lab-panel)
-- pass current site and locale into form_validator (edc-form-validators)
-- SodiumModelMixin (edc-lab-results)
-- add inclusive option to report_datetime validators (edc-form-validators)
-- major refactor of edc_sites:
-    - register sites from sites.py. sites must be registered
-      with the new sites global. ``sites`` uses autodiscover
-      to find ``sites.py`` in root of an app.
-    - move most functionality related to sites onto the
-      `sites`` global instance.
-    - add funcs to allow a configuration where an auditor type
-      user, with view only access, is able to view data from
-      other sites while logged into the current site.
-    - set current site and locale from request object in get_forms
-- update dashboard apps to accommodate expanded auditor type
-  role using funcs from edc_sites (edc-dashboard, edc-listboard,
-  edc-subject-dashboard, edc-review-dashboard)
-- update tests to either register a default site or add sites.py
-  to the test setup (most modules)
-- add DJ50 to testing matrix, drop DJ41.
-
-0.5.50 (yanked)
-------
-  ** skip this release, goto 0.5.51
-- bump django-audit-fields
-
-0.5.49 (yanked)
-------
-  ** skip this release, goto 0.5.51
-- bump django-audit-fields, django-crypto-fields
-- track locale on model instance add/change (django-audit-fields)
-- convert Meta.unique_together to new Meta.constraints
-- review index inheritance and fix where not working
-- add indexes to improve performance (edc-metadata, edc-action-item)
-
-0.5.48
-------
-- remove invalid permissions codename (edc-data-manager)
-
-0.5.47 (yanked)
-------
-  ** skip this release, goto 0.5.48
-- require module `edc_form_runners`
-- fix missing model name in breadcrumbs (edc-model-admin)
-- use self.subject_identifier from base class when looking up
-  ``action_cls`` in `ActionItemModelFormMixin` (edc-action-item)
-- add custom form_runner (edc_appointment)
-- use proxy model to make custom admin class for edc_form_runner
-  Issue model (edc-data-manager)
-- add link to edc_data_manager.Issue changelist from subject
-  dashboard and issue badge with hover text on subject dashboard
-  CRF/Requisitions (edc-subject-dashboard,
-  edc-subject-model-wrappers)
-
-0.5.46
-------
-- minor, updates to translation files (edc-he)
-
-0.5.45
-------
-- updates to HE 'PropertyModelMixin' (edc-he)
-    - add 'calculated_land_surface_area' field (standardised to m2)
-    - add additional units: Decimals (1/100th of Acre), Sq. feet
-    - convert 'land_surface_area' to decimal field
-- minor, remove additional refs to edc_reference in tests (edc-utils)
-
-0.5.44
-------
-- fix issue where appointment creator may lose the site id
-  for funcs run from the django console on a multisite
-  installation (edc-appointment, edc-visit-schedule, edc-sites)
-
-0.5.43
-------
-- method to calculated relative previous appt with a subject visit
-  report (edc_appointment)
-
-0.5.42 (invalid)
-------
-- fix where scheduled crf collection incorrectly combines
-  crfs_unscheduled + crfs_prn instead of crfs + crfs_prn
-  (edc-metadata)
-
-0.5.41
-------
-- docs (edc)
-- add 'appt_status' property to form validation, trivial
-  (edc-appointment)
-
-0.5.40
-------
-- remove `edc_reference` from setup.cfg
-- fix additional exceptions not caught in modelform
-  (edc-appointment, edc-visit-tracking)
-- fix prn metadata not updating (edc-metadata)
-- refactor form collections in visit class (edc-visit-tracking)
-
-0.5.39
-------
-- fix minor typos in fieldsets (edc-lab-results)
-- catch exception into form when unscheduled appointment not allowed
-  (edc-appointment)
-- remove additional refs to edc_reference in tests
-
-0.5.38
-------
-- add further validation to death report model and form validation
-  mixins (edc-adverse-event)
-- minor doc updates
-
-0.5.37
-------
-- remove dependency `edc_reference`. `edc-reference` maintained a
-  single table, "edc_reference.Reference", with values needed for
-  metadata-rules. The table was updated on a `post_save` signal
-  for CRF/Requisition and other models using the
-  `ReferenceModelMixin`. By removing `edc_reference`, `edc-metadata` now
-  directly queries CRF/Requisition models instead of querying model
-  "edc_reference.Reference". This change has bumped most edc modules. The
-  dependency was required for a few modules or, as in most cases, just for
-  tests. The model mixin `ReferenceModelMixin` and the site controller
-  `site_reference_configs` are no longer required. You may remove from
-  your app any reference to `edc-reference` and the file
-  `reference_model_configs`.
-
-0.5.36
-------
-- add missing migrations (edc-data-manager)
-
-0.5.35
-------
-- remove imports from base constructor (edc-visit-schedule)
-- update imports for changes to edc-visit-schedule
-  and drop 3.10/DJ4.1 (all)
-
-0.5.34
-------
-- add import path for ScreeningManager to model_mixins (edc-screening)
-
-0.5.33
-------
-- merge edc-next-appointment into edc-appointment.
-  edc-next-appointment is now deprecated.
-- refactor mixin paths (edc-appointment)
-- update modules to reflect path changes in edc-appointment
-  (edc-crf, edc-timepoint, edc-visit-tracking, edc-facility)
-
-0.5.32
-------
-- add site to SubjectScheduleHistory model (edc-visit-schedule)
-- change signature on UnscheduledAppointmentCreator; allow signal
-  to create unscheduled/interim appointment when using next
-  appointment CRF based on `allow_create_interim` field value.
-  (edc-appointment)
-- update mixins with `allow_create_interim` field.
-  (edc-next-appointment)
-- allow proxy models but use the proxy_for_model model name to
-  update and get references (edc-reference).
-- add data manager to recipients list (edc-data-manager)
-- use title case for "Data Collection Status" app name (edc-metadata)
-
-0.5.31
-------
-- refactor update_skipped_appointments management command
-  (edc-appointment)
-- add SiteModelAdminMixin to SubjectRefusalAdmin to filter by site
-  (edc-refusal)
-- change to use non-ISO numbering (edc-facility)
-- fix administration page template failing if app_list is None.
-  (edc-model-admin)
-
-0.5.30
-------
-- fix issues when setting appointments as skipped, resetting
-  appointments (edc-appointment, edc-next-appointment)
-- (edc-visit-tracking)
-    - use Django's get_model_related to determine `related_visit` and
-      other similar properties.
-    - enforce appointment sequence when saving CRFs in model save.
-
-0.5.29
-------
-- reset migrations. You need to drop the `edc_visit_tracking`
-  models and delete any migrations under django_migrations
-  where app="edc_visit_tracking" before running
-  `migrate`. (edc_visit_tracking)
-- add SKIPPED_APPT appointment status; update admin, form classes;
-  Add settings.EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING.
-  (edc-appointment, edc-next-appointment, edc-visit-tracking)
-- minor change to admin (edc-he)
-
-0.5.28
-------
-- fix import and minor typos (edc-crf)
-- add custom language internationalization constants (edc-constants)
-- refactor SingleSite interface to accept list of `language_codes`
-  instead of a dict of `languages` (edc-sites)
-    - NOTE: this is a "breaking" change.  Protocol specific sites.py
-      modules that already declare `languages` will need to be
-      updated use 'language_codes' instead.
-
-0.5.27
-------
-- add constants (edc-constants)
-- use django_apps to get model to prevent circular
-  import in tests (edc-sites)
-
-0.5.26
-------
-- change from 'confirm' to 'transcribe' (edc-adherence)
-- add proxy_models to list of models to be used by consent
-  object (edc-consent)
-- removed `PiiModelAdminMixin` (edc-consent)
-- use getters for some class attributes (changelist_url,
-  post_full_url_on_delete,  post_url_on_delete_name) to make
-  it easier to override and to access request object
-  (edc-model-admin)
-- add `country` templatetag; change signature for
-  `get_current_country` to accept both `site` and `request`
-  (edc-sites)
-
-0.5.25
-------
-- include django.mo file in MANIFEST.IN for modules with
-  locale messages (django-audit-fields, edc-adverse-event,
-  edc-constants, edc-crf, edc-dashboard, edc-he, edc-model-admin,
-  edc-protocol, edc-qol, edc-review-dashboard, edc-subject-dashboard,
-  edc-visit-tracking)
-
-0.5.24
-------
-- ICECAP-A sw translation (edc-qol)
-- add translation funcs, sw translation (edc-visit-tracking
-  and others)
-- slight refactor PiiModelAdminMixin (edc-model-admin)
-
-0.5.23
-------
-- fix filter_fieldsets_for_pii_permissions (edc-consent)
-
-0.5.22
-------
-- setup apps for translation, add partially updated po files for
-  locale sw.
-- add set language template (edc-navbar)
-- expect default settings of USE_I18N and USE_L10N to be `True`
-  on main project apps
-
-0.5.21
-------
-- edc-adverse-event
-  - check for pdf report class on model class as well as on view mixin;
-  - rename reports as `AePdfReport` and `DeathPdfReport`;
-  - Check for "susar" model instance field attribute in `signal` before
-    updating.
-  - add hospitalization codenames for auth
-  - use get_edc_adverse_event_app_label() (edc-transfer)
-  - add migration; update tests (edc-he)
-  - access ADVERSE_EVENT_APP_LABEL settings attr through function
-    get_adverse_event_app_label
-
-0.5.20
-------
-- remove default contact date from subject visit missed
-  (edc-visit-tracking)
-
-0.5.19
-------
-- use related visit attr for singleton model mixin lookup
-  (edc-crf)
-- fix spelling error in constant (edc-he)
-
-0.5.18
-------
-- modify metadata rules to update the CrfMetadata of previous
-  timepoints if HE forms are filled in over more than one timepoint;
-  fix minor validation issues; improve test coverage (edc-he)
-- add `time-machine` to testing dependencies
-
-0.5.17
-------
-- add Meta option to declare PredicateCollection on a RuleGroup;
-  update README (edc-metadata)
-- add models and other classes (edc-he)
-- and method `get_models` to list all models associated with a visit
-  (edc-visit-schedule)
-- add model_mixin method `update_references_on_save` to update ALL
-  references on save (edc-reference)
-
-0.5.16
-------
-- move model, admin, form, etc from intecomm to edc-he (edc-he)
-- add extra_value column to ListModelMixin to inspect in
-  admin class (edc-list-data)
-- set instance attr in get() instead of get_context_data()
-  (edc-listboard, edc-appointment, edc-registration)
-- add disaster recovery (from backup) docs (edc)
-- minor updates to backup docs (edc)
-
-0.5.15
-------
-- minor updates to email subject and body for new/changed user
-  accounts (edc-auth)
-- update backup docs (edc)
-- add SubjectVisit concrete model/admin; raise exception if related
-  visit model, or SubjectVisit, is a proxy model; deprecate
-  func get_subject_visit_model_cls (edc-visit-tracking)
-- raise exception if attempting to get an invalid visit_code from
-  the visit schedule (edc-visit-schedule)
-- add related_visit_model to RuleGroups to allow related visit model
-  to be from an outside app; fix issue where Rule runner relied on
-  related visit model for the app_label to get rules from site global
-  (edc-metadata)
-- use `get_appointment_model_cls` instead of directly importing
-  Appointment model; add tests for admin class (edc-appointment)
-- add missing mixins to QueryRule admin class (edc-data-manager)
-- add checks to form validator (edc-facility)
-- update tests to use SubjectVisit from edc-visit-tracking (all)
-- add more typing hints (all)
-
-0.5.14
-------
-- raise if locator model in settings does not match visit schedule
-  (edc-locator, edc-visit-schedule)
-
-0.5.13
-------
-- 0.5.12 has wrong version of edc-facility, bump to  0.3.16
-
-0.5.12
-------
-- add missing edc-next-appointment
-
-0.5.11
-------
-- add HealthFacility model/form/admin (edc-facility)
-- rename func get_clinic_codenames to get_app_codenames,
-  deprecate get_clinic_codenames (edc-auth)
-- fix issue where unable to read selected models from the
-  post/session (edc-export)
-- improve SubjectLocator changelist (edc-locator)
-- Add additional date filters to custom ListFilter class,
-  yes_no_coloring templatetag (edc-model-admin)
-- new module with mixins for NextAppointment CRF
-  (edc-next-appointment)
-
-0.5.10
-------
-- 0.5.9 has wrong version of django-crypto-fields,
-  bump to 0.3.7
-
 0.5.9
-------
-- limit data export to the sites listed in userprofile; use
-  protocol name for zip archive `base_dir`; update modeladmin
-  classes (edc-export)
+-----
+- limit data export to the sites listed in userprofile; use protocol
+  name for zip archive `base_dir`; update modeladmin classes
+  (edc-export)
 - add func to get all sites for user (edc-sites)
 - filter data by site using sites param (edc-pdutils)
 - add unregister method for site_action_items (edc-action-item)
 - add verbose_name_plural; move ModelAdmin functionality to
   SubjectLocatorModelAdminMixin (edc-locator)
 - add ModelAdmin mixin to remove PII/encrypted fields from changelist
   and search for users not in PII/PII_VIEW permission groups;
   move dashboard functionality to ModelAdminDashboardMixin.
   (edc-model-admin)
 - add unregister method for site_prn_forms (edc-prn)
 - use `get_locator_model` instead of hardcoded locator model
   (edc-subject-dashboard, edc-subject-model-wrappers)
 
+
 0.5.8
 -----
 - use SQLAlchemy to prepare sql text for pandas, upgrade pandas
   to latest, require SQLAlchemy (edc-pdutils)
 - typing hints (edc-pdutils, edc-export)
 - check settings before loading load_data (edc-list-data)
 - add func to get all sites for country (edc-sites)
@@ -711,16 +33,15 @@
 - change field `return_in_days` to `rx_days` (edc-rx)
 
 0.5.6
 -----
 - major refactor; eliminated use of TargetHandler classes; removed
   post processing validation checks no longer necessary with
   these fixes (edc-metadata)
-- raise addition exception if field not on source model
-  (edc-reference)
+- raise addition exception if field not on source model (edc-reference)
 
 0.5.5
 -----
 - refactor options for get and create; wrap create in transaction
   (edc-reference)
 - wrap site lookup in transaction (edc-sites)
 - fix sidebar template metadata panel href (edc-subject-dashboard)
@@ -745,42 +66,42 @@
  - link changelist to subject_dashboard; refactor ReferenceGetter to
    respect site. Customize ModelAdmin class. (edc-reference)
  - add link to edc_metadata from dashboard (edc-subject-dashboard)
  - remove unique constraint on legal_name (edc-model)
 
 0.5.3
 -----
-- accept FieldError on get_queryset if using SiteModelAdminMixin for
-  model without field `site`. (edc-sites)
+- accept FieldError on get_queryset if using SiteModelAdminMixin for model
+  without field `site`. (edc-sites)
 
 0.5.2
 -----
 - force all models to use `objects` as default manager (edc-model)
 - add new mixins to handle redirects, delete button (edc-model-admin)
 - update admin mixin to handle fks/m2ms in modelform (edc-site)
-- move managers from fields mixin to screening_model_mixin
-  (edc-screening)
+- move managers from fields mixin to screening_model_mixin (edc-screening)
+
 
 0.5.1
 ------
-- add additional validation to check screening identifier and the
-  screening eligibility boolean. (edc-consent)
-- add mixin to redirect all forms to a selected changelist
-  (edc-model-admin)
+- add additional validation to check screening identifier and the screening
+  eligibility boolean. (edc-consent)
+- add mixin to redirect all forms to a selected changelist (edc-model-admin)
 - improve redirect on delete (edc-model-admin)
 
+
+
 0.4.99
 ------
-- fix rounding issue with md section numbers, allow opt out of
-  timestamp on every form rendered (edc-form-describer)
+- fix rounding issue with md section numbers, allow opt out of timestamp on
+  every form rendered (edc-form-describer)
 
 0.4.98
 ------
-- allow fbg date to be 'on or after' report date instead of only after
-  (edc-glucose)
+- allow fbg date to be 'on or after' report date instead of only after (edc-glucose)
 - minor fix in date_is_after_or_raise validation message when using
   inclusive=True (edc-form-validators)
 
 0.4.97
 ------
 - raise incorrectly skipped exception in form validator (edc-dx-review)
 - specify action type when querying death report actions
```

### Comparing `edc-0.5.87/LICENSE` & `edc-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/README.rst` & `edc-0.5.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,65 @@
-|pypi| |downloads| |black|
+Metadata-Version: 2.1
+Name: edc
+Version: 0.5.9
+Summary: EDC core modules for clinicedc/edc projects.
+Home-page: https://github.com/clinicedc/edc
+Author: Erik van Widenfelt
+Author-email: ew2789@gmail.com
+License: GPL license, see LICENSE
+Keywords: django edc clinical trials research
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS
+
+|pypi| |downloads|
 
 clinicedc
 =========
 
 Here are a set of python modules that extend Django to empower you to build an EDC / eSource system to handle data
 collection and management for multi-site longitudinal clinical trials.
 
 Refer to the specific open projects listed below for example EDC systems built with these modules.
 The more recent the trial the better the example.
 
 The codebase continues to evolve over many years of conducting clinical trials for mostly NIH-funded clinical trials through
 the `Harvard T Chan School of Public Health <https://aids.harvard.edu>`__, the
 `Botswana-Harvard AIDS Institute Partnership <https://aids.harvard.edu/research/bhp>`__
 in Gaborone, Botswana and the `London School of Hygiene and Tropical Medicine <https://lshtm.ac.uk>`__.
-Almost all trials were originally related to HIV/AIDS research.
-
-More recent work with the `RESPOND Africa Group <https://www.ucl.ac.uk/global-health/respond-africa>`__ formerly at the
-`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ and now with the `University College London Institute for Global Health <https://www.ucl.ac.uk/global-health/>`__ has expanded into Diabetes (DM),
+Almost all trials were originally related to HIV/AIDS research. More recent work with the `RESPOND Africa Group <https://www.lstmed.ac.uk/RespondAfrica>`__ at both the
+`Liverpool School of Tropical Medicine <https://lstm.ac.uk>`__ and the `University College London Institute for Global Health <https://www.ucl.ac.uk/global-health/>`__ has expanded into Diabetes (DM),
 Hypertension (HTN) and models of integrating care in Africa (https://inteafrica.org) for the
 three main chronic conditions -- HIV/DM/HTN.
 
-See also https://www.ucl.ac.uk/global-health/respond-africa
+See also https://www.lstmed.ac.uk/RespondAfrica
 
 The implementations we have developed are mostly eSource systems rather than the traditional EDCs.
 
 The ``clinicedc`` for each trial consists of a subset of trial-specific modules that reference this module.
 
 (python 3.11, Django 4.2, MySQL 8+, see setup.cfg)
 
 
 Projects that use ``clinicedc``
 -------------------------------
 Recent examples of ``clinicedc`` applications using this codebase:
 
 INTECOMM
 --------
-Controlling chronic diseases in Africa: Development and evaluation of an integrated community-based management model for HIV, Diabetes and Hypertension in Tanzania and Uganda
 
 https://github.com/intecomm-trial/intecomm-edc (2022- )
 
 EFFECT
 ------
 Fluconazole plus flucytosine vs. fluconazole alone for cryptococcal antigen-positive patients identified through screening:
 
@@ -60,53 +80,49 @@
 http://www.isrctn.com/ISRCTN77382043
 
 Mapitio
 ~~~~~~~
 
 Retrospective HIV/Diabetes/Hypertension Cohort (Tanzania)
 
-https://github.com/mapitio/mapitio-edc (2020-2022)
+https://github.com/mapitio/mapitio-edc (2020- )
 
 MOCCA
 ~~~~~
 
 Integrated care for HIV and non-communicable diseases in Africa: a pilot study to inform a large-scale trial (MOCCA and MOCCA Extension Study)
 
-https://github.com/mocca-trail/mocca-edc (2020-2022)
+https://github.com/mocca-trail/mocca-edc (2020- )
 
 http://www.isrctn.com/ISRCTN71437522
 
 INTE Africa Trial
 ~~~~~~~~~~~~~~~~~
-Evaluating the integration of health services for chronic diseases in Africa
 
 (32 sites in Uganda and Tanzania)
 
-https://github.com/inte-africa-trial/inte-edc (2020-2022)
+https://github.com/inte-africa-trial/inte-edc (2020- )
 
 https://inteafrica.org
 
 http://www.isrctn.com/ISRCTN43896688
 
 META Trial (Phase II)
 ~~~~~~~~~~~~~~~~~~~~~
-A randomised placebo-controlled double-blind phase II trial to determine the effects of metformin versus placebo on the incidence of diabetes in HIV-infected persons with pre-diabetes in Tanzania.
 
 (3 sites in Tanzania)
 
 https://github.com/meta-trial/meta-edc (2019-2021)
 
 http://www.isrctn.com/ISRCTN76157257
 
 
 The Ambition Trial
 ~~~~~~~~~~~~~~~~~~
 
-High dose AMBISOME on a fluconazole backbone for cryptococcal meningitis induction therapy in sub-Saharan Africa
-
 (7 sites in Botswana, Malawi, South Africa, Uganda, Zimbabwe)
 
 https://github.com/ambition-trial/ambition-edc (2018-2021)
 
 http://www.isrctn.com/ISRCTN72509687
 
 Start with main repo `ambition-edc`
@@ -132,65 +148,63 @@
 For further information go to https://github.com/erikvw.
 
 |django| |jet-brains|
 
 =========================== ============================= ==================================
 edc-action-item_            |edc-action-item|             |pypi-edc-action-item|
 edc-adverse-event_          |edc-adverse-event|           |pypi-edc-adverse-event|
-edc-appconfig_              |edc-appconfig|               |pypi-edc-appconfig|
 edc-appointment_            |edc-appointment|             |pypi-edc-appointment|
 edc-auth_                   |edc-auth|                    |pypi-edc-auth|
+edc-call-manager_           |edc-call-manager|
 edc-consent_                |edc-consent|                 |pypi-edc-consent|
 edc-constants_                                            |pypi-edc-constants|
 edc-crf_                    |edc-crf|                     |pypi-edc-crf|
 edc-dashboard_              |edc-dashboard|               |pypi-edc-dashboard|
 edc-data-manager_           |edc-data-manager|            |pypi-edc-data-manager|
 edc-device_                 |edc-device|                  |pypi-edc-device|
-edc-document-status_        |edc-document-status|         |pypi-edc-document-status|
 edc-egfr_                   |edc-egfr|                    |pypi-edc-egfr|
 edc-export_                 |edc-export|                  |pypi-edc-export|
 edc-facility_               |edc-facility|                |pypi-edc-facility|
 edc-fieldsets_              |edc-fieldsets|               |pypi-edc-fieldsets|
 edc-form-describer_         |edc-form-describer|          |pypi-edc-form-describer|
 edc-form-label_             |edc-form-label|              |pypi-edc-form-label|
-edc-form-runners_           |edc-form-runners|            |pypi-edc-form-runners|
 edc-form-validators_        |edc-form-validators|         |pypi-edc-form-validators|
 edc-identifier_             |edc-identifier|              |pypi-edc-identifier|
 edc-lab_                    |edc-lab|                     |pypi-edc-lab|
-edc-lab-dashboard_          |edc-lab-dashboard|           |pypi-edc-lab-dashboard|
 edc-lab-panel_              |edc-lab-panel|               |pypi-edc-lab-panel|
-edc-lab-results_            |edc-lab-results|             |pypi-edc-lab-panel|
+edc-lab-dashboard_          |edc-lab-dashboard|           |pypi-edc-lab-dashboard|
+edc-lab-results_            |edc-lab-results|               |pypi-edc-lab-panel|
 edc-label_                  |edc-label|                   |pypi-edc-label|
 edc-list-data_              |edc-list-data|               |pypi-edc-list-data|
-edc-listboard_              |edc-listboard|               |pypi-edc-listboard|
 edc-locator_                |edc-locator|                 |pypi-edc-locator|
 edc-ltfu_                   |edc-ltfu|                    |pypi-edc-ltfu|
 edc-metadata_               |edc-metadata|                |pypi-edc-metadata|
 edc-model_                  |edc-model|                   |pypi-edc-model|
 edc-model-admin_            |edc-model-admin|             |pypi-edc-model-admin|
 edc-model-fields_           |edc-model-fields|            |pypi-edc-model-fields|
 edc-model-form_             |edc-model-form|              |pypi-edc-model-form|
+edc-model-wrapper_          |edc-model-wrapper|           |pypi-edc-model-wrapper|
 edc-navbar_                 |edc-navbar|                  |pypi-edc-navbar|
-edc-next-appointment_       |edc-next-appointment|        |pypi-edc-next-appointment|
 edc-notification_           |edc-notification|            |pypi-edc-notification|
 edc-offstudy_               |edc-offstudy|                |pypi-edc-offstudy|
-edc-pdf-reports_            |edc-pdf-reports|             |pypi-edc-pdf-reports|
 edc-pdutils_                |edc-pdutils|                 |pypi-edc-pdutils|
 edc-prn_                    |edc-prn|                     |pypi-edc-prn|
 edc-protocol_               |edc-protocol|                |pypi-edc-protocol|
 edc-protocol-incident_      |edc-protocol-incident|       |pypi-edc-protocol-incident|
 edc-randomization_          |edc-randomization|           |pypi-edc-randomization|
-edc-refusal_                |edc-refusal|                 |pypi-edc-refusal|
+edc-reference_              |edc-reference|               |pypi-edc-reference|
 edc-registration_           |edc-registration|            |pypi-edc-registration|
 edc-reportable_             |edc-reportable|              |pypi-edc-reportable|
+edc-reports_                |edc-reports|                 |pypi-edc-reports|
 edc-review-dashboard_       |edc-review-dashboard|        |pypi-edc-review-dashboard|
 edc-screening_              |edc-screening|               |pypi-edc-screening|
 edc-search_                 |edc-search|                  |pypi-edc-search|
 edc-sites_                  |edc-sites|                   |pypi-edc-sites|
 edc-subject-dashboard_      |edc-subject-dashboard|       |pypi-edc-subject-dashboard|
+edc-subject-model-wrappers_ |edc-subject-model-wrappers|  |pypi-edc-subject-model-wrappers|
 edc-test-utils_             |edc-test-utils|              |pypi-edc-test-utils|
 edc-timepoint_              |edc-timepoint|               |pypi-edc-timepoint|
 edc-transfer_               |edc-transfer|                |pypi-edc-transfer|
 edc-unblinding_             |edc-unblinding|              |pypi-edc-unblinding|
 edc-utils_                  |edc-utils|                   |pypi-edc-utils|
 edc-visit-schedule_         |edc-visit-schedule|          |pypi-edc-visit-schedule|
 edc-visit-tracking_         |edc-visit-tracking|          |pypi-edc-visit-tracking|
@@ -202,22 +216,19 @@
 
 ========================== ============================== ==================================
 edc-adherence_              |edc-adherence|               |pypi-edc-adherence|
 edc-csf_                    |edc-csf|                     |pypi-edc-csf|
 edc-dx_                     |edc-dx|                      |pypi-edc-dx|
 edc-dx-review_              |edc-dx-review|               |pypi-edc-dx-review|
 edc-glucose_                |edc-glucose|                 |pypi-edc-glucose|
-edc-he_                     |edc-he|                      |pypi-edc-he|
 edc-mnsi_                   |edc-mnsi|                    |pypi-edc-mnsi|
 edc-microbiology_           |edc-microbiology|            |pypi-edc-microbiology|
 edc-microscopy_             |edc-microscopy|              |pypi-edc-microscopy|
 edc-pharmacy_               |edc-pharmacy|                |pypi-edc-pharmacy|
 edc-pharmacy-dashboard_     |edc-pharmacy-dashboard|      |pypi-edc-pharmacy-dashboard|
-edc-qol_                    |edc-qol|                     |pypi-edc-qol|
-edc-rx_                     |edc-rx|                      |pypi-edc-rx|
 edc-vitals_                 |edc-vitals|                  |pypi-edc-vitals|
 ========================== ============================== ==================================
 
 Thanks to JetBrains for support with an opensource PyCharm IDE license. |jet-brains|
 
 .. |pypi| image:: https://img.shields.io/pypi/v/edc.svg
     :target: https://pypi.python.org/pypi/edc
@@ -230,246 +241,230 @@
    :alt: Made with Django
 
 
 .. _edc-action-item: https://github.com/clinicedc/edc-action-item
 .. _edc-adherence: https://github.com/clinicedc/edc-adherence
 .. _edc-adverse-event: https://github.com/clinicedc/edc-adverse-event
 .. _edc-appointment: https://github.com/clinicedc/edc-appointment
-.. _edc-appconfig: https://github.com/clinicedc/edc-appconfig
 .. _edc-auth: https://github.com/clinicedc/edc-auth
+.. _edc-call-manager: https://github.com/clinicedc/edc-call-manager
 .. _edc-consent: https://github.com/clinicedc/edc-consent
 .. _edc-constants: https://github.com/clinicedc/edc-constants
 .. _edc-crf: https://github.com/clinicedc/edc-crf
 .. _edc-csf: https://github.com/clinicedc/edc-csf
 .. _edc-dashboard: https://github.com/clinicedc/edc-dashboard
 .. _edc-data-manager: https://github.com/clinicedc/edc-data-manager
 .. _edc-device: https://github.com/clinicedc/edc-device
-.. _edc-document-status: https://github.com/clinicedc/edc-document-status
 .. _edc-dx: https://github.com/clinicedc/edc-dx
 .. _edc-dx-review: https://github.com/clinicedc/edc-dx-review
 .. _edc-egfr: https://github.com/clinicedc/edc-egfr
 .. _edc-export: https://github.com/clinicedc/edc-export
 .. _edc-facility: https://github.com/clinicedc/edc-facility
 .. _edc-fieldsets: https://github.com/clinicedc/edc-fieldsets
 .. _edc-form-describer: https://github.com/clinicedc/edc-form-describer
 .. _edc-form-label: https://github.com/clinicedc/edc-form-label
-.. _edc-form-runners: https://github.com/clinicedc/edc-form-runners
 .. _edc-form-validators: https://github.com/clinicedc/edc-form-validators
 .. _edc-glucose: https://github.com/clinicedc/edc-glucose
-.. _edc-he: https://github.com/clinicedc/edc-he
 .. _edc-identifier: https://github.com/clinicedc/edc-identifier
 .. _edc-lab: https://github.com/clinicedc/edc-lab
 .. _edc-lab-dashboard: https://github.com/clinicedc/edc-lab-dashboard
 .. _edc-lab-panel: https://github.com/clinicedc/edc-lab-panel
 .. _edc-lab-results: https://github.com/clinicedc/edc-lab-results
 .. _edc-label: https://github.com/clinicedc/edc-label
 .. _edc-list-data: https://github.com/clinicedc/edc-list-data
-.. _edc-listboard: https://github.com/clinicedc/edc-listboard
 .. _edc-locator: https://github.com/clinicedc/edc-locator
 .. _edc-ltfu: https://github.com/clinicedc/edc-ltfu
 .. _edc-metadata: https://github.com/clinicedc/edc-metadata
 .. _edc-mnsi: https://github.com/clinicedc/edc-mnsi
 .. _edc-microbiology: https://github.com/clinicedc/edc-microbiology
 .. _edc-microscopy: https://github.com/clinicedc/edc-microscopy
 .. _edc-model: https://github.com/clinicedc/edc-model
 .. _edc-model-admin: https://github.com/clinicedc/edc-model-admin
 .. _edc-model-fields: https://github.com/clinicedc/edc-model-fields
 .. _edc-model-form: https://github.com/clinicedc/edc-model-form
+.. _edc-model-wrapper: https://github.com/clinicedc/edc-model-wrapper
 .. _edc-navbar: https://github.com/clinicedc/edc-navbar
-.. _edc-next-appointment: https://github.com/clinicedc/edc-next-appointment
 .. _edc-notification: https://github.com/clinicedc/edc-notification
 .. _edc-offstudy: https://github.com/clinicedc/edc-offstudy
 .. _edc-pdutils: https://github.com/clinicedc/edc-pdutils
 .. _edc-pharmacy: https://github.com/clinicedc/edc-pharmacy
 .. _edc-pharmacy-dashboard: https://github.com/clinicedc/edc-pharmacy-dashboard
 .. _edc-prn: https://github.com/clinicedc/edc-prn
 .. _edc-protocol: https://github.com/clinicedc/edc-protocol
 .. _edc-protocol-incident: https://github.com/clinicedc/edc-protocol-incident
-.. _edc-qol: https://github.com/clinicedc/edc-qol
 .. _edc-randomization: https://github.com/clinicedc/edc-randomization
+.. _edc-reference: https://github.com/clinicedc/edc-reference
 .. _edc-refusal: https://github.com/clinicedc/edc-refusal
 .. _edc-registration: https://github.com/clinicedc/edc-registration
 .. _edc-reportable: https://github.com/clinicedc/edc-reportable
-.. _edc-pdf-reports: https://github.com/clinicedc/edc-reports
+.. _edc-reports: https://github.com/clinicedc/edc-reports
 .. _edc-review-dashboard: https://github.com/clinicedc/edc-review-dashboard
-.. _edc-rx: https://github.com/clinicedc/edc-rx
 .. _edc-screening: https://github.com/clinicedc/edc-screening
 .. _edc-search: https://github.com/clinicedc/edc-search
 .. _edc-sites: https://github.com/clinicedc/edc-sites
 .. _edc-subject-dashboard: https://github.com/clinicedc/edc-subject-dashboard
+.. _edc-subject-model-wrappers: https://github.com/clinicedc/edc-subject-model-wrappers
 .. _edc-test-utils: https://github.com/clinicedc/edc-test-utils
 .. _edc-timepoint: https://github.com/clinicedc/edc-timepoint
 .. _edc-transfer: https://github.com/clinicedc/edc-transfer
 .. _edc-unblinding: https://github.com/clinicedc/edc-unblinding
 .. _edc-utils: https://github.com/clinicedc/edc-utils
 .. _edc-visit-schedule: https://github.com/clinicedc/edc-visit-schedule
 .. _edc-visit-tracking: https://github.com/clinicedc/edc-visit-tracking
 .. _edc-vitals: https://github.com/clinicedc/edc-vitals
 
-.. |edc-action-item| image:: https://github.com/clinicedc/edc-action-item/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-action-item/actions/workflows/build.yml
-.. |edc-adherence| image:: https://github.com/clinicedc/edc-adherence/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-adherence/actions/workflows/build.yml
-.. |edc-adverse-event| image:: https://github.com/clinicedc/edc-adverse-event/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-adverse-event/actions/workflows/build.yml
-.. |edc-appointment| image:: https://github.com/clinicedc/edc-appointment/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-appointment/actions/workflows/build.yml
-.. |edc-appconfig| image:: https://github.com/clinicedc/edc-appconfig/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-appconfig/actions/workflows/build.yml
-.. |edc-auth| image:: https://github.com/clinicedc/edc-auth/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-auth/actions/workflows/build.yml
-.. |edc-lab-results| image:: https://github.com/clinicedc/edc-lab-results/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-lab-results/actions/workflows/build.yml
-.. |edc-clinic| image:: https://github.com/clinicedc/edc-clinic/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-clinic/actions/workflows/build.yml
-.. |edc-consent| image:: https://github.com/clinicedc/edc-consent/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-consent/actions/workflows/build.yml
-.. |edc-crf| image:: https://github.com/clinicedc/edc-crf/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-crf/actions/workflows/build.yml
-.. |edc-csf| image:: https://github.com/clinicedc/edc-csf/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-csf/actions/workflows/build.yml
-.. |edc-dashboard| image:: https://github.com/clinicedc/edc-dashboard/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-dashboard/actions/workflows/build.yml
-.. |edc-data-manager| image:: https://github.com/clinicedc/edc-data-manager/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-data-manager/actions/workflows/build.yml
-.. |edc-device| image:: https://github.com/clinicedc/edc-device/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-device/actions/workflows/build.yml
-.. |edc-document-status| image:: https://github.com/clinicedc/edc-document-status/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-document-status/actions/workflows/build.yml
-.. |edc-dx| image:: https://github.com/clinicedc/edc-dx/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-dx/actions/workflows/build.yml
-.. |edc-dx-review| image:: https://github.com/clinicedc/edc-dx-review/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-dx-review/actions/workflows/build.yml
-.. |edc-egfr| image:: https://github.com/clinicedc/edc-egfr/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-egfr/actions/workflows/build.yml
-.. |edc-export| image:: https://github.com/clinicedc/edc-export/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-export/actions/workflows/build.yml
-.. |edc-facility| image:: https://github.com/clinicedc/edc-facility/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-facility/actions/workflows/build.yml
-.. |edc-fieldsets| image:: https://github.com/clinicedc/edc-fieldsets/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-fieldsets/actions/workflows/build.yml
-.. |edc-form-describer| image:: https://github.com/clinicedc/edc-form-describer/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-form-describer/actions/workflows/build.yml
-.. |edc-form-label| image:: https://github.com/clinicedc/edc-form-label/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-form-label/actions/workflows/build.yml
-.. |edc-form-runners| image:: https://github.com/clinicedc/edc-form-runners/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-form-runners/actions/workflows/build.yml
-.. |edc-form-validators| image:: https://github.com/clinicedc/edc-form-validators/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-form-validators/actions/workflows/build.yml
-.. |edc-glucose| image:: https://github.com/clinicedc/edc-glucose/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-glucose/actions/workflows/build.yml
-.. |edc-he| image:: https://github.com/clinicedc/edc-he/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-he/actions/workflows/build.yml
-.. |edc-identifier| image:: https://github.com/clinicedc/edc-identifier/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-identifier/actions/workflows/build.yml
-.. |edc-lab| image:: https://github.com/clinicedc/edc-lab/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-lab/actions/workflows/build.yml
-.. |edc-lab-panel| image:: https://github.com/clinicedc/edc-lab-panel/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-lab-panel/actions/workflows/build.yml
-.. |edc-lab-dashboard| image:: https://github.com/clinicedc/edc-lab-dashboard/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-lab-dashboard/actions/workflows/build.yml
-.. |edc-label| image:: https://github.com/clinicedc/edc-label/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-label/actions/workflows/build.yml
-.. |edc-list-data| image:: https://github.com/clinicedc/edc-list-data/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-list-data/actions/workflows/build.yml
-.. |edc-listboard| image:: https://github.com/clinicedc/edc-listboard/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-listboard/actions/workflows/build.yml
-.. |edc-locator| image:: https://github.com/clinicedc/edc-locator/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-locator/actions/workflows/build.yml
-.. |edc-ltfu| image:: https://github.com/clinicedc/edc-ltfu/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-ltfu/actions/workflows/build.yml
-.. |edc-metadata| image:: https://github.com/clinicedc/edc-metadata/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-metadata/actions/workflows/build.yml
-.. |edc-metadata-rules| image:: https://github.com/clinicedc/edc-metadata-rules/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-metadata-rules/actions/workflows/build.yml
-.. |edc-mnsi| image:: https://github.com/clinicedc/edc-mnsi/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-mnsi/actions/workflows/build.yml
-.. |edc-microbiology| image:: https://github.com/clinicedc/edc-microbiology/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-microbiology/actions/workflows/build.yml
-.. |edc-microscopy| image:: https://github.com/clinicedc/edc-microscopy/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-microscopy/actions/workflows/build.yml
-.. |edc-model| image:: https://github.com/clinicedc/edc-model/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-model/actions/workflows/build.yml
-.. |edc-model-admin| image:: https://github.com/clinicedc/edc-model-admin/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-model-admin/actions/workflows/build.yml
-.. |edc-model-fields| image:: https://github.com/clinicedc/edc-model-fields/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-model-fields/actions/workflows/build.yml
-.. |edc-model-form| image:: https://github.com/clinicedc/edc-model-form/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-model-form/actions/workflows/build.yml
-.. |edc-navbar| image:: https://github.com/clinicedc/edc-navbar/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-navbar/actions/workflows/build.yml
-.. |edc-next-appointment| image:: https://github.com/clinicedc/edc-next-appointment/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-next-appointment/actions/workflows/build.yml
-.. |edc-notification| image:: https://github.com/clinicedc/edc-notification/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-notification/actions/workflows/build.yml
-.. |edc-offstudy| image:: https://github.com/clinicedc/edc-offstudy/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-offstudy/actions/workflows/build.yml
-.. |edc-pdutils| image:: https://github.com/clinicedc/edc-pdutils/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-pdutils/actions/workflows/build.yml
-.. |edc-pharmacy| image:: https://github.com/clinicedc/edc-pharmacy/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-pharmacy/actions/workflows/build.yml
-.. |edc-pharmacy-dashboard| image:: https://github.com/clinicedc/edc-pharmacy-dashboard/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-pharmacy-dashboard/actions/workflows/build.yml
-.. |edc-prn| image:: https://github.com/clinicedc/edc-prn/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-prn/actions/workflows/build.yml
-.. |edc-protocol| image:: https://github.com/clinicedc/edc-protocol/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-protocol/actions/workflows/build.yml
-.. |edc-protocol-incident| image:: https://github.com/clinicedc/edc-protocol-incident/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-protocol-incident/actions/workflows/build.yml
-.. |edc-randomization| image:: https://github.com/clinicedc/edc-randomization/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-randomization/actions/workflows/build.yml
-.. |edc-refusal| image:: https://github.com/clinicedc/edc-refusal/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-refusal/actions/workflows/build.yml
-.. |edc-registration| image:: https://github.com/clinicedc/edc-registration/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-registration/actions/workflows/build.yml
-.. |edc-reportable| image:: https://github.com/clinicedc/edc-reportable/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-reportable/actions/workflows/build.yml
-.. |edc-pdf-reports| image:: https://github.com/clinicedc/edc-pdf-reports/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-pdf-reports/actions/workflows/build.yml
-.. |edc-qol| image:: https://github.com/clinicedc/edc-qol/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-qol/actions/workflows/build.yml
-.. |edc-review-dashboard| image:: https://github.com/clinicedc/edc-review-dashboard/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-review-dashboard/actions/workflows/build.yml
-.. |edc-rx| image:: https://github.com/clinicedc/edc-rx/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-rx/actions/workflows/build.yml
-.. |edc-screening| image:: https://github.com/clinicedc/edc-screening/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-screening/actions/workflows/build.yml
-.. |edc-search| image:: https://github.com/clinicedc/edc-search/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-search/actions/workflows/build.yml
-.. |edc-sites| image:: https://github.com/clinicedc/edc-sites/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-sites/actions/workflows/build.yml
-.. |edc-subject-dashboard| image:: https://github.com/clinicedc/edc-subject-dashboard/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-subject-dashboard/actions/workflows/build.yml
-.. |edc-test-utils| image:: https://github.com/clinicedc/edc-test-utils/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-test-utils/actions/workflows/build.yml
-.. |edc-timepoint| image:: https://github.com/clinicedc/edc-timepoint/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-timepoint/actions/workflows/build.yml
-.. |edc-transfer| image:: https://github.com/clinicedc/edc-transfer/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-transfer/actions/workflows/build.yml
-.. |edc-unblinding| image:: https://github.com/clinicedc/edc-unblinding/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-unblinding/actions/workflows/build.yml
-.. |edc-utils| image:: https://github.com/clinicedc/edc-utils/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-utils/actions/workflows/build.yml
-.. |edc-visit-schedule| image:: https://github.com/clinicedc/edc-visit-schedule/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-visit-schedule/actions/workflows/build.yml
-.. |edc-visit-tracking| image:: https://github.com/clinicedc/edc-visit-tracking/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-visit-tracking/actions/workflows/build.yml
-.. |edc-vitals| image:: https://github.com/clinicedc/edc-vitals/actions/workflows/build.yml/badge.svg
-  :target: https://github.com/clinicedc/edc-vitals/actions/workflows/build.yml
+.. |edc-action-item| image:: https://github.com/clinicedc/edc-action-item/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-action-item/actions?query=workflow:build
+.. |edc-adherence| image:: https://github.com/clinicedc/edc-adherence/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-adherence/actions?query=workflow:build
+.. |edc-adverse-event| image:: https://github.com/clinicedc/edc-adverse-event/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-adverse-event/actions?query=workflow:build
+.. |edc-appointment| image:: https://github.com/clinicedc/edc-appointment/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-appointment/actions?query=workflow:build
+.. |edc-auth| image:: https://github.com/clinicedc/edc-auth/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-auth/actions?query=workflow:build
+.. |edc-lab-results| image:: https://github.com/clinicedc/edc-lab-results/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-lab-results/actions?query=workflow:build
+.. |edc-call-manager| image:: https://github.com/clinicedc/edc-call-manager/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-call-manager/actions?query=workflow:build
+.. |edc-clinic| image:: https://github.com/clinicedc/edc-clinic/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-clinic/actions?query=workflow:build
+.. |edc-consent| image:: https://github.com/clinicedc/edc-consent/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-consent/actions?query=workflow:build
+.. |edc-crf| image:: https://github.com/clinicedc/edc-crf/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-crf/actions?query=workflow:build
+.. |edc-csf| image:: https://github.com/clinicedc/edc-csf/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-csf/actions?query=workflow:build
+.. |edc-dashboard| image:: https://github.com/clinicedc/edc-dashboard/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-dashboard/actions?query=workflow:build
+.. |edc-data-manager| image:: https://github.com/clinicedc/edc-data-manager/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-data-manager/actions?query=workflow:build
+.. |edc-device| image:: https://github.com/clinicedc/edc-device/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-device/actions?query=workflow:build
+.. |edc-dx| image:: https://github.com/clinicedc/edc-dx/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-dx/actions?query=workflow:build
+.. |edc-dx-review| image:: https://github.com/clinicedc/edc-dx-review/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-dx-review/actions?query=workflow:build
+.. |edc-egfr| image:: https://github.com/clinicedc/edc-egfr/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-egfr/actions?query=workflow:build
+.. |edc-export| image:: https://github.com/clinicedc/edc-export/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-export/actions?query=workflow:build
+.. |edc-facility| image:: https://github.com/clinicedc/edc-facility/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-facility/actions?query=workflow:build
+.. |edc-fieldsets| image:: https://github.com/clinicedc/edc-fieldsets/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-fieldsets/actions?query=workflow:build
+.. |edc-form-describer| image:: https://github.com/clinicedc/edc-form-describer/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-form-describer/actions?query=workflow:build
+.. |edc-form-label| image:: https://github.com/clinicedc/edc-form-label/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-form-label/actions?query=workflow:build
+.. |edc-form-validators| image:: https://github.com/clinicedc/edc-form-validators/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-form-validators/actions?query=workflow:build
+.. |edc-glucose| image:: https://github.com/clinicedc/edc-glucose/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-glucose/actions?query=workflow:build
+.. |edc-identifier| image:: https://github.com/clinicedc/edc-identifier/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-identifier/actions?query=workflow:build
+.. |edc-lab| image:: https://github.com/clinicedc/edc-lab/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-lab/actions?query=workflow:build
+.. |edc-lab-panel| image:: https://github.com/clinicedc/edc-lab-panel/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-lab-panel/actions?query=workflow:build
+.. |edc-lab-dashboard| image:: https://github.com/clinicedc/edc-lab-dashboard/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-lab-dashboard/actions?query=workflow:build
+.. |edc-label| image:: https://github.com/clinicedc/edc-label/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-label/actions?query=workflow:build
+.. |edc-list-data| image:: https://github.com/clinicedc/edc-list-data/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-list-data/actions?query=workflow:build
+.. |edc-locator| image:: https://github.com/clinicedc/edc-locator/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-locator/actions?query=workflow:build
+.. |edc-ltfu| image:: https://github.com/clinicedc/edc-ltfu/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-ltfu/actions?query=workflow:build
+.. |edc-metadata| image:: https://github.com/clinicedc/edc-metadata/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-metadata/actions?query=workflow:build
+.. |edc-metadata-rules| image:: https://github.com/clinicedc/edc-metadata-rules/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-metadata-rules/actions?query=workflow:build
+.. |edc-mnsi| image:: https://github.com/clinicedc/edc-mnsi/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-mnsi/actions?query=workflow:build
+.. |edc-microbiology| image:: https://github.com/clinicedc/edc-microbiology/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-microbiology/actions?query=workflow:build
+.. |edc-microscopy| image:: https://github.com/clinicedc/edc-microscopy/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-microscopy/actions?query=workflow:build
+.. |edc-model| image:: https://github.com/clinicedc/edc-model/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-model/actions?query=workflow:build
+.. |edc-model-admin| image:: https://github.com/clinicedc/edc-model-admin/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-model-admin/actions?query=workflow:build
+.. |edc-model-fields| image:: https://github.com/clinicedc/edc-model-fields/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-model-fields/actions?query=workflow:build
+.. |edc-model-form| image:: https://github.com/clinicedc/edc-model-form/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-model-form/actions?query=workflow:build
+.. |edc-model-wrapper| image:: https://github.com/clinicedc/edc-model-wrapper/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-model-wrapper/actions?query=workflow:build
+.. |edc-navbar| image:: https://github.com/clinicedc/edc-navbar/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-navbar/actions?query=workflow:build
+.. |edc-notification| image:: https://github.com/clinicedc/edc-notification/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-notification/actions?query=workflow:build
+.. |edc-offstudy| image:: https://github.com/clinicedc/edc-offstudy/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-offstudy/actions?query=workflow:build
+.. |edc-pdutils| image:: https://github.com/clinicedc/edc-pdutils/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-pdutils/actions?query=workflow:build
+.. |edc-pharmacy| image:: https://github.com/clinicedc/edc-pharmacy/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-pharmacy/actions?query=workflow:build
+.. |edc-pharmacy-dashboard| image:: https://github.com/clinicedc/edc-pharmacy-dashboard/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-pharmacy-dashboard/actions?query=workflow:build
+.. |edc-prn| image:: https://github.com/clinicedc/edc-prn/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-prn/actions?query=workflow:build
+.. |edc-protocol| image:: https://github.com/clinicedc/edc-protocol/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-protocol/actions?query=workflow:build
+.. |edc-protocol-incident| image:: https://github.com/clinicedc/edc-protocol-incident/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-protocol-incident/actions?query=workflow:build
+.. |edc-randomization| image:: https://github.com/clinicedc/edc-randomization/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-randomization/actions?query=workflow:build
+.. |edc-reference| image:: https://github.com/clinicedc/edc-reference/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-reference/actions?query=workflow:build
+.. |edc-registration| image:: https://github.com/clinicedc/edc-registration/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-registration/actions?query=workflow:build
+.. |edc-reportable| image:: https://github.com/clinicedc/edc-reportable/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-reportable/actions?query=workflow:build
+.. |edc-reports| image:: https://github.com/clinicedc/edc-reports/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-reports/actions?query=workflow:build
+.. |edc-review-dashboard| image:: https://github.com/clinicedc/edc-review-dashboard/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-review-dashboard/actions?query=workflow:build
+.. |edc-screening| image:: https://github.com/clinicedc/edc-screening/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-screening/actions?query=workflow:build
+.. |edc-search| image:: https://github.com/clinicedc/edc-search/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-search/actions?query=workflow:build
+.. |edc-sites| image:: https://github.com/clinicedc/edc-sites/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-sites/actions?query=workflow:build
+.. |edc-subject-dashboard| image:: https://github.com/clinicedc/edc-subject-dashboard/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-subject-dashboard/actions?query=workflow:build
+.. |edc-subject-model-wrappers| image:: https://github.com/clinicedc/edc-subject-model-wrappers/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-subject-model-wrappers/actions?query=workflow:build
+.. |edc-test-utils| image:: https://github.com/clinicedc/edc-test-utils/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-test-utils/actions?query=workflow:build
+.. |edc-timepoint| image:: https://github.com/clinicedc/edc-timepoint/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-timepoint/actions?query=workflow:build
+.. |edc-transfer| image:: https://github.com/clinicedc/edc-transfer/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-transfer/actions?query=workflow:build
+.. |edc-unblinding| image:: https://github.com/clinicedc/edc-unblinding/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-unblinding/actions?query=workflow:build
+.. |edc-utils| image:: https://github.com/clinicedc/edc-utils/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-utils/actions?query=workflow:build
+.. |edc-visit-schedule| image:: https://github.com/clinicedc/edc-visit-schedule/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-visit-schedule/actions?query=workflow:build
+.. |edc-visit-tracking| image:: https://github.com/clinicedc/edc-visit-tracking/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-visit-tracking/actions?query=workflow:build
+.. |edc-vitals| image:: https://github.com/clinicedc/edc-vitals/workflows/build/badge.svg?branch=develop
+  :target: https://github.com/clinicedc/edc-vitals/actions?query=workflow:build
 
 .. |pypi-edc-action-item| image:: https://img.shields.io/pypi/v/edc-action-item.svg
     :target: https://pypi.python.org/pypi/edc-action-item
 .. |pypi-edc-adherence| image:: https://img.shields.io/pypi/v/edc-adherence.svg
     :target: https://pypi.python.org/pypi/edc-adherence
 .. |pypi-edc-adverse-event| image:: https://img.shields.io/pypi/v/edc-adverse-event.svg
     :target: https://pypi.python.org/pypi/edc-adverse-event
 .. |pypi-edc-appointment| image:: https://img.shields.io/pypi/v/edc-appointment.svg
     :target: https://pypi.python.org/pypi/edc-appointment
-.. |pypi-edc-appconfig| image:: https://img.shields.io/pypi/v/edc-appconfig.svg
-    :target: https://pypi.python.org/pypi/edc-appconfig
 .. |pypi-edc-auth| image:: https://img.shields.io/pypi/v/edc-auth.svg
     :target: https://pypi.python.org/pypi/edc-auth
 .. |pypi-edc-blood-results| image:: https://img.shields.io/pypi/v/edc-blood-results.svg
     :target: https://pypi.python.org/pypi/edc-blood-results
 .. |pypi-edc-consent| image:: https://img.shields.io/pypi/v/edc-consent.svg
     :target: https://pypi.python.org/pypi/edc-consent
 .. |pypi-edc-constants| image:: https://img.shields.io/pypi/v/edc-constants.svg
@@ -480,16 +475,14 @@
     :target: https://pypi.python.org/pypi/edc-csf
 .. |pypi-edc-dashboard| image:: https://img.shields.io/pypi/v/edc-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-dashboard
 .. |pypi-edc-data-manager| image:: https://img.shields.io/pypi/v/edc-data-manager.svg
     :target: https://pypi.python.org/pypi/edc-data-manager
 .. |pypi-edc-device| image:: https://img.shields.io/pypi/v/edc-device.svg
     :target: https://pypi.python.org/pypi/edc-device
-.. |pypi-edc-document-status| image:: https://img.shields.io/pypi/v/edc-document-status.svg
-    :target: https://pypi.python.org/pypi/edc-document-status
 .. |pypi-edc-dx| image:: https://img.shields.io/pypi/v/edc-dx.svg
     :target: https://pypi.python.org/pypi/edc-dx
 .. |pypi-edc-dx-review| image:: https://img.shields.io/pypi/v/edc-dx-review.svg
     :target: https://pypi.python.org/pypi/edc-dx-review
 .. |pypi-edc-egfr| image:: https://img.shields.io/pypi/v/edc-egfr.svg
     :target: https://pypi.python.org/pypi/edc-egfr
 .. |pypi-edc-export| image:: https://img.shields.io/pypi/v/edc-export.svg
@@ -498,36 +491,30 @@
     :target: https://pypi.python.org/pypi/edc-facility
 .. |pypi-edc-fieldsets| image:: https://img.shields.io/pypi/v/edc-fieldsets.svg
     :target: https://pypi.python.org/pypi/edc-fieldsets
 .. |pypi-edc-form-describer| image:: https://img.shields.io/pypi/v/edc-form-describer.svg
     :target: https://pypi.python.org/pypi/edc-form-describer
 .. |pypi-edc-form-label| image:: https://img.shields.io/pypi/v/edc-form-label.svg
     :target: https://pypi.python.org/pypi/edc-form-label
-.. |pypi-edc-form-runners| image:: https://img.shields.io/pypi/v/edc-form-runners.svg
-    :target: https://pypi.python.org/pypi/edc-form-runners
 .. |pypi-edc-form-validators| image:: https://img.shields.io/pypi/v/edc-form-validators.svg
     :target: https://pypi.python.org/pypi/edc-form-validators
 .. |pypi-edc-glucose| image:: https://img.shields.io/pypi/v/edc-glucose.svg
     :target: https://pypi.python.org/pypi/edc-glucose
-.. |pypi-edc-he| image:: https://img.shields.io/pypi/v/edc-he.svg
-    :target: https://pypi.python.org/pypi/edc-he
 .. |pypi-edc-identifier| image:: https://img.shields.io/pypi/v/edc-identifier.svg
     :target: https://pypi.python.org/pypi/edc-identifier
 .. |pypi-edc-lab| image:: https://img.shields.io/pypi/v/edc-lab.svg
     :target: https://pypi.python.org/pypi/edc-lab
 .. |pypi-edc-lab-panel| image:: https://img.shields.io/pypi/v/edc-lab-panel.svg
     :target: https://pypi.python.org/pypi/edc-lab-panel
 .. |pypi-edc-lab-dashboard| image:: https://img.shields.io/pypi/v/edc-lab-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-lab-dashboard
 .. |pypi-edc-label| image:: https://img.shields.io/pypi/v/edc-label.svg
     :target: https://pypi.python.org/pypi/edc-label
 .. |pypi-edc-list-data| image:: https://img.shields.io/pypi/v/edc-list-data.svg
     :target: https://pypi.python.org/pypi/edc-list-data
-.. |pypi-edc-listboard| image:: https://img.shields.io/pypi/v/edc-listboard.svg
-    :target: https://pypi.python.org/pypi/edc-listboard
 .. |pypi-edc-locator| image:: https://img.shields.io/pypi/v/edc-locator.svg
     :target: https://pypi.python.org/pypi/edc-locator
 .. |pypi-edc-ltfu| image:: https://img.shields.io/pypi/v/edc-ltfu.svg
     :target: https://pypi.python.org/pypi/edc-ltfu
 .. |pypi-edc-metadata| image:: https://img.shields.io/pypi/v/edc-metadata.svg
     :target: https://pypi.python.org/pypi/edc-metadata
 .. |pypi-edc-mnsi| image:: https://img.shields.io/pypi/v/edc-mnsi.svg
@@ -540,18 +527,18 @@
     :target: https://pypi.python.org/pypi/edc-model
 .. |pypi-edc-model-admin| image:: https://img.shields.io/pypi/v/edc-model-admin.svg
     :target: https://pypi.python.org/pypi/edc-model-admin
 .. |pypi-edc-model-fields| image:: https://img.shields.io/pypi/v/edc-model-fields.svg
     :target: https://pypi.python.org/pypi/edc-model-fields
 .. |pypi-edc-model-form| image:: https://img.shields.io/pypi/v/edc-model-form.svg
     :target: https://pypi.python.org/pypi/edc-model-form
+.. |pypi-edc-model-wrapper| image:: https://img.shields.io/pypi/v/edc-model-wrapper.svg
+    :target: https://pypi.python.org/pypi/edc-model-wrapper
 .. |pypi-edc-navbar| image:: https://img.shields.io/pypi/v/edc-navbar.svg
     :target: https://pypi.python.org/pypi/edc-navbar
-.. |pypi-edc-next-appointment| image:: https://img.shields.io/pypi/v/edc-next-appointment.svg
-    :target: https://pypi.python.org/pypi/edc-next-appointment
 .. |pypi-edc-notification| image:: https://img.shields.io/pypi/v/edc-notification.svg
     :target: https://pypi.python.org/pypi/edc-notification
 .. |pypi-edc-offstudy| image:: https://img.shields.io/pypi/v/edc-offstudy.svg
     :target: https://pypi.python.org/pypi/edc-offstudy
 .. |pypi-edc-pdutils| image:: https://img.shields.io/pypi/v/edc-pdutils.svg
     :target: https://pypi.python.org/pypi/edc-pdutils
 .. |pypi-edc-pharmacy| image:: https://img.shields.io/pypi/v/edc-pharmacy.svg
@@ -560,38 +547,36 @@
     :target: https://pypi.python.org/pypi/edc-pharmacy-dashboard
 .. |pypi-edc-prn| image:: https://img.shields.io/pypi/v/edc-prn.svg
     :target: https://pypi.python.org/pypi/edc-prn
 .. |pypi-edc-protocol| image:: https://img.shields.io/pypi/v/edc-protocol.svg
     :target: https://pypi.python.org/pypi/edc-protocol
 .. |pypi-edc-protocol-incident| image:: https://img.shields.io/pypi/v/edc-protocol-incident.svg
     :target: https://pypi.python.org/pypi/edc-protocol-incident
-.. |pypi-edc-qol| image:: https://img.shields.io/pypi/v/edc-qol.svg
-    :target: https://pypi.python.org/pypi/edc-qol
 .. |pypi-edc-randomization| image:: https://img.shields.io/pypi/v/edc-randomization.svg
     :target: https://pypi.python.org/pypi/edc-randomization
-.. |pypi-edc-refusal| image:: https://img.shields.io/pypi/v/edc-refusal.svg
-    :target: https://pypi.python.org/pypi/edc-refusal
+.. |pypi-edc-reference| image:: https://img.shields.io/pypi/v/edc-reference.svg
+    :target: https://pypi.python.org/pypi/edc-reference
 .. |pypi-edc-registration| image:: https://img.shields.io/pypi/v/edc-registration.svg
     :target: https://pypi.python.org/pypi/edc-registration
 .. |pypi-edc-reportable| image:: https://img.shields.io/pypi/v/edc-reportable.svg
     :target: https://pypi.python.org/pypi/edc-reportable
-.. |pypi-edc-pdf-reports| image:: https://img.shields.io/pypi/v/edc-pdf-reports.svg
-    :target: https://pypi.python.org/pypi/edc-pdf-reports
+.. |pypi-edc-reports| image:: https://img.shields.io/pypi/v/edc-reports.svg
+    :target: https://pypi.python.org/pypi/edc-reports
 .. |pypi-edc-review-dashboard| image:: https://img.shields.io/pypi/v/edc-review-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-review-dashboard
-.. |pypi-edc-rx| image:: https://img.shields.io/pypi/v/edc-rx.svg
-    :target: https://pypi.python.org/pypi/edc-rx
 .. |pypi-edc-screening| image:: https://img.shields.io/pypi/v/edc-screening.svg
     :target: https://pypi.python.org/pypi/edc-screening
 .. |pypi-edc-search| image:: https://img.shields.io/pypi/v/edc-search.svg
     :target: https://pypi.python.org/pypi/edc-search
 .. |pypi-edc-sites| image:: https://img.shields.io/pypi/v/edc-sites.svg
     :target: https://pypi.python.org/pypi/edc-sites
 .. |pypi-edc-subject-dashboard| image:: https://img.shields.io/pypi/v/edc-subject-dashboard.svg
     :target: https://pypi.python.org/pypi/edc-subject-dashboard
+.. |pypi-edc-subject-model-wrappers| image:: https://img.shields.io/pypi/v/edc-subject-model-wrappers.svg
+    :target: https://pypi.python.org/pypi/edc-subject-model-wrappers
 .. |pypi-edc-test-utils| image:: https://img.shields.io/pypi/v/edc-test-utils.svg
     :target: https://pypi.python.org/pypi/edc-test-utils
 .. |pypi-edc-timepoint| image:: https://img.shields.io/pypi/v/edc-timepoint.svg
     :target: https://pypi.python.org/pypi/edc-timepoint
 .. |pypi-edc-transfer| image:: https://img.shields.io/pypi/v/edc-transfer.svg
     :target: https://pypi.python.org/pypi/edc-transfer
 .. |pypi-edc-unblinding| image:: https://img.shields.io/pypi/v/edc-utils.svg
@@ -604,10 +589,7 @@
     :target: https://pypi.python.org/pypi/edc-visit-tracking
 .. |pypi-edc-vitals| image:: https://img.shields.io/pypi/v/edc-vitals.svg
     :target: https://pypi.python.org/pypi/edc-vitals
 .. |jet-brains| image:: https://resources.jetbrains.com/storage/products/company/brand/logos/PyCharm_icon.png
     :target: https://jb.gg/OpenSource
     :width: 25
     :alt: JetBrains PyCharm
-
-.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
```

### Comparing `edc-0.5.87/bin/nginx/edc-uat.conf` & `edc-0.5.9/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/bin/nginx/edc.conf` & `edc-0.5.9/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/bin/scripts/dev_repos.sh` & `edc-0.5.9/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/bin/scripts/update_edc.sh` & `edc-0.5.9/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/bin/systemd/celery-uat.service` & `edc-0.5.9/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/bin/systemd/celery.service` & `edc-0.5.9/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/Makefile` & `edc-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/README.rst` & `edc-0.5.9/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 Login as non-root account ``ambition`` and install dependencies.
 
 .. code-block:: bash
 
     sudo apt-get update
     sudo apt-get -y upgrade
     sudo apt-get -y install mysql-server-5.7 # if needed
-    sudo apt-get -y install mysql-client-5.7 libmysqlclient-dev libcups2-dev ipython3 python3-pip python3-dev python3-venv python3-cups python3-venv redis-server nginx curl wbritish
+    sudo apt-get -y install mysql-client-5.7 libmysqlclient-dev libcups2-dev ipython3 python3-pip python3-dev python3-venv python3-cups python3-venv redis-server nginx curl
 
 
 As of Feb 2019 ``ambition`` and ``edc`` modules are tested on python versions 3.7 and above. Ubuntu 18.04 LTS uses python 3.6.7.
 
 To upgrade to python3.7:
 
 .. code-block:: bash
```

### Comparing `edc-0.5.87/docs/celery.rst` & `edc-0.5.9/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/conf.py` & `edc-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/configure_web_services.rst` & `edc-0.5.9/docs/configure_web_services.rst`

 * *Files 18% similar despite different names*

```diff
@@ -93,31 +93,31 @@
 	$ sudo systemctl daemon-reload
 	$ sudo systemctl restart gunicorn
 
 If needed to reset ...
 
 .. code-block:: bash
 
-	$ sudo systemctl stop gunicorn-live.socket \
-		&& sudo systemctl stop gunicorn-live \
-		&& sudo systemctl disable gunicorn-live.socket
+	$ sudo systemctl stop gunicorn.socket \
+		&& sudo systemctl stop gunicorn \
+		&& sudo systemctl disable gunicorn.socket
 
 	$ sudo systemctl stop gunicorn-uat.socket \
 		&& sudo systemctl stop gunicorn-uat \
 		&& sudo systemctl disable gunicorn-uat.socket
 
 
 Nginx
 =====
 
 Copy the configurations to ``/etc/nginx/sites-available``
 
 .. code-block:: bash
 
-	$ sudo cp -R ~/app/bin/nginx/conf/* /etc/nginx/sites-available/
+	$ sudo cp -R ~/app/bin/nginx/* /etc/nginx/sites-available/
 
 
 Replace town referred to in server name
 
 .. code-block:: bash
 
 	# for example
@@ -128,135 +128,64 @@
 
 Enable each site:
 
 .. code-block:: bash
 
 	$ sudo ln -s /etc/nginx/sites-available/ambition.conf /etc/nginx/sites-enabled
 
-Inspect:
 
-.. code-block:: bash
+Inspect::
 
 	$ ls -la /etc/nginx/sites-enabled
 
-Output:
-
-.. code-block:: bash
+Output::
 
 	ambition-uat.conf -> /etc/nginx/sites-available/ambition-uat.conf
 	ambition.conf -> /etc/nginx/sites-available/ambition.conf
 
+
 Disable the default site, if enabled:
 
 .. code-block:: bash
 
 	$ sudo unlink /etc/nginx/sites-enabled/default
 
-Test the new configuration:
-
 .. code-block:: bash
 
 	$ sudo nginx -t
 
-Output:
-
-.. code-block:: bash
-
-	nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
-	nginx: configuration file /etc/nginx/nginx.conf test is successful
-
-Restart Nginx service:
-
 .. code-block:: bash
 
 	$ sudo systemctl restart nginx
 
 Firewall
 ========
 
-On application/web-server, check ``ufw`` to open ``openSSH``, ``http``, ``https``
-
-e.g.
-
-.. code-block:: bash
-
-	# review ports opened by application firewall rules
-	$ sudo ufw app info 'OpenSSH'
-	$ sudo ufw app info 'Nginx Full'
-
-	# configure application firewall rules
-	$ sudo ufw allow 'OpenSSH'
-	$ sudo ufw allow 'Nginx Full'
-
-	# review ports opened by application firewall rule
-	$ sudo ufw app info 'Nginx Full'
-
-	# enable the firewall, and check
-	$ sudo ufw enable
-	$ sudo ufw status
-
+Check ``ufw`` to open ``openSSH``, ``http``, ``https``, ``631``
 
 Also check cloud firewall to ensure these ports are open
 
-If not already done, on DB server, ensure application server has access to ``3306`` from it's private IP
-
-e.g.
-
-.. code-block:: bash
-
-	$ sudo ufw allow from <app.server.private.ip> to any port 3306
-
 
 Certificates and HTTPS configuration
 ====================================
 
-see https://certbot.eff.org or more specifically `Certbot Instructions for Nginx on Ubuntu 20 <https://certbot.eff.org/instructions?ws=nginx&os=ubuntufocal&tab=standard/>`_ (or later)
-
-Remove certbot-auto and any Certbot OS packages:
-
-.. code-block:: bash
-
-	$ sudo apt-get remove certbot
-
-Install certbot and prepare command:
-
-.. code-block:: bash
-
-	$ sudo snap install --classic certbot
-	$ sudo ln -s /snap/bin/certbot /usr/bin/certbot
-
-
-Get and install certificates:
+see  https://certbot.eff.org
 
 .. code-block:: bash
 
 	$ sudo certbot --nginx
 
-    Saving debug log to /var/log/letsencrypt/letsencrypt.log
-
-    Which names would you like to activate HTTPS for?
-    We recommend selecting either all domains, or all domains in a VirtualHost/server block.
-    - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
-    # select blank for all
-
-Test automatic certificate renewal
-
-.. code-block:: bash
-
-	$ sudo certbot renew --dry-run
-
-Confirm Nginx config still valid:
-
 .. code-block:: bash
 
 	$ sudo nginx -t
 
 .. code-block:: bash
 
 	$ sudo systemctl restart nginx
 
 Now check that the DB server will allow access
 
 * check the firewall (under DO)
 * check mysql user for this account (edc@privateIP)
 
 See document ``prepare_database``
+
```

### Comparing `edc-0.5.87/docs/deploy_new_droplet.rst` & `edc-0.5.9/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/exporting_encrypted_data.rst` & `edc-0.5.9/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/forms_reference.md` & `edc-0.5.9/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/make.bat` & `edc-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/prepare_database.rst` & `edc-0.5.9/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/printing.rst` & `edc-0.5.9/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/docs/update_deployment.rst` & `edc-0.5.9/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/edc.egg-info/SOURCES.txt` & `edc-0.5.9/edc.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -27,38 +27,31 @@
 docs/README.rst
 docs/backup.rst
 docs/celery.rst
 docs/conda.rst
 docs/conf.py
 docs/configure_web_services.rst
 docs/deploy_new_droplet.rst
-docs/disaster_recovery.rst
 docs/dump_users.rst
 docs/exporting_encrypted_data.rst
 docs/forms_reference.md
 docs/index.rst
 docs/landing_page.rst
 docs/make.bat
+docs/multisite_deployment.rst
 docs/prepare_database.rst
 docs/printing.rst
 docs/redis.rst
 docs/update_deployment.rst
 edc.egg-info/PKG-INFO
 edc.egg-info/SOURCES.txt
 edc.egg-info/dependency_links.txt
 edc.egg-info/not-zip-safe
 edc.egg-info/requires.txt
 edc.egg-info/top_level.txt
-image/administration_appointment.png
-image/administration_button.png
-image/administration_icon.png
-image/appointments.png
-image/appointments_annotated_top.png
-image/appointments_changelist.png
-image/down_arrow.png
 image/icon-pycharm.png
 requirements.tests/coverage.txt
 requirements.tests/docs.txt
 requirements.tests/edc.txt
 requirements.tests/edc_dev.txt
 requirements.tests/edc_offline.txt
 requirements.tests/lint.txt
```

### Comparing `edc-0.5.87/edc.egg-info/requires.txt` & `edc-0.5.9/edc.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,90 +6,89 @@
 pycups
 pyrabbit
 python-dateutil
 python-memcached
 reportlab
 tqdm
 fontawesomefree
-djangorestframework
 django-environ
 django-redis
+django-audit-fields==0.3.9
+django-crypto-fields==0.3.5
 django-defender
+django-extensions
+django-logentry-admin
+django-multisite-edc==2.0.0
+django-revision==0.3.6
+django-simple-history>=3.1.1
 django-storages
-django-logentry-admin==1.1.0
-django-extensions==3.2.3
-django-simple-history==3.5.0
-django-audit-fields==0.3.17
-django-crypto-fields==0.4.1
-django-logentry-admin==1.1.0
-django-multisite2==2.0.1
-django-revision==0.3.7
-edc-action-item==0.3.89
-edc-adherence==0.3.13
-edc-adverse-event==0.3.83
-edc-appconfig==0.1.8
-edc-appointment==0.4.28
-edc-auth==0.3.86
-edc-consent==0.3.83
-edc-constants==0.3.62
-edc-crf==0.3.74
-edc-dashboard==0.3.61
-edc-data-manager==0.3.77
-edc-device==0.3.17
-edc-document-status==0.3.2
-edc-dx==0.3.7
-edc-dx-review==0.3.2
-edc-egfr==0.3.8
-edc-export==0.3.49
-edc-facility==0.3.37
-edc-fieldsets==0.3.21
-edc-form-describer==0.3.22
-edc-form-label==0.3.18
-edc-form-runners==0.3.10
-edc-form-validators==0.3.40
-edc-glucose==0.3.6
-edc-he==0.3.12
-edc-identifier==0.3.36
-edc-lab==0.3.60
-edc-lab-dashboard==0.3.23
-edc-lab-panel==0.3.5
-edc-lab-results==0.3.11
-edc-label==0.3.19
-edc-list-data==0.3.26
-edc-listboard==0.3.13
-edc-locator==0.3.45
-edc-ltfu==0.3.34
-edc-metadata==0.3.95
-edc-mnsi==0.3.5
-edc-model==0.3.40
-edc-model-admin==0.3.73
-edc-model-fields==0.3.12
-edc-model-form==0.3.2
-edc-navbar==0.3.28
-edc-notification==0.3.26
-edc-offstudy==0.3.47
-edc-pdf-reports==0.3.20
-edc-pdutils==0.3.37
-edc-pharmacy==0.3.9
-edc-pharmacy-dashboard==0.1.8
-edc-prn==0.3.24
-edc-protocol==0.3.16
-edc-protocol-incident==0.3.5
-edc-qol==0.3.6
-edc-randomization==0.3.56
-edc-refusal==0.3.10
-edc-registration==0.3.41
-edc-reportable==0.3.38
-edc-review-dashboard==0.3.38
-edc-rx==0.3.1
-edc-screening==0.3.52
-edc-search==0.3.11
-edc-sites==0.3.56
-edc-subject-dashboard==0.3.71
-edc-timepoint==0.3.21
-edc-transfer==0.3.22
-edc-unblinding==0.3.9
-edc-utils==0.3.33
-edc-visit-schedule==0.3.97
-edc-visit-tracking==0.3.91
-edc-vitals==0.1.13
-Django>=4.2.11
+djangorestframework
+edc-action-item==0.3.55
+edc-adherence==0.1.21
+edc-adverse-event==0.3.55
+edc-appointment==0.3.74
+edc-auth==0.3.63
+edc-consent==0.3.47
+edc-constants==0.3.49
+edc-crf==0.3.44
+edc-dashboard==0.3.45
+edc-data-manager==0.3.56
+edc-device==0.3.11
+edc-document-status==0.1.4
+edc-dx==0.1.20
+edc-dx-review==0.1.39
+edc-egfr==0.1.11
+edc-export==0.3.31
+edc-facility==0.3.15
+edc-fieldsets==0.3.13
+edc-form-describer==0.3.16
+edc-form-label==0.3.9
+edc-form-validators==0.3.34
+edc-glucose==0.1.30
+edc-he==0.1.9
+edc-identifier==0.3.24
+edc-lab==0.3.44
+edc-lab-dashboard==0.3.11
+edc-lab-panel==0.1.15
+edc-lab-results==0.1.38
+edc-label==0.3.13
+edc-list-data==0.3.19
+edc-listboard==0.1.11
+edc-locator==0.3.25
+edc-ltfu==0.3.24
+edc-metadata==0.3.54
+edc-mnsi==0.1.17
+edc-model==0.3.32
+edc-model-admin==0.3.48
+edc-model-fields==0.3.7
+edc-model-form==0.1.12
+edc-model-wrapper==0.3.10
+edc-navbar==0.3.16
+edc-notification==0.3.18
+edc-offstudy==0.3.33
+edc-pdf-reports==0.3.14
+edc-pdutils==0.3.24
+edc-pharmacy==0.1.39
+edc-pharmacy-dashboard==0.1.3
+edc-prn==0.3.14
+edc-protocol==0.3.10
+edc-protocol-incident==0.1.26
+edc-qol==0.1.15
+edc-randomization==0.3.47
+edc-reference==0.3.20
+edc-refusal==0.1.13
+edc-registration==0.3.30
+edc-reportable==0.3.31
+edc-review-dashboard==0.3.19
+edc-rx==0.1.7
+edc-screening==0.3.35
+edc-search==0.3.7
+edc-sites==0.3.27
+edc-subject-dashboard==0.3.39
+edc-subject-model-wrappers==0.3.16
+edc-timepoint==0.3.11
+edc-transfer==0.3.14
+edc-unblinding==0.1.15
+edc-utils==0.3.20
+edc-visit-schedule==0.3.62
+edc-visit-tracking==0.3.53
+edc-vitals==0.1.11
```

### Comparing `edc-0.5.87/image/icon-pycharm.png` & `edc-0.5.9/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.5.87/requirements.tests/edc.txt` & `edc-0.5.9/requirements.tests/edc.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,14 @@
-django-environ
-django-storages
-fontawesomefree
-bs4
-mysqlclient
-django-logentry-admin
-django-simple-history
+canned-views
 django-audit-fields
 django-crypto-fields
 django-revision
-django-multisite2
 edc-action-item
 edc-adherence
 edc-adverse-event
-edc-appconfig
 edc-appointment
 edc-auth
 edc-consent
 edc-constants
 edc-crf
 edc-dashboard
 edc-data-manager
@@ -26,15 +18,14 @@
 edc-dx-review
 edc-egfr
 edc-export
 edc-facility
 edc-fieldsets
 edc-form-describer
 edc-form-label
-edc-form-runners
 edc-form-validators
 edc-glucose
 edc-he
 edc-identifier
 edc-lab
 edc-lab-dashboard
 edc-lab-panel
@@ -46,36 +37,38 @@
 edc-ltfu
 edc-metadata
 edc-mnsi
 edc-model
 edc-model-admin
 edc-model-fields
 edc-model-form
+edc-model-wrapper
 edc-navbar
-edc-next-appointment
 edc-notification
 edc-offstudy
 edc-pdf-reports
 edc-pdutils
 edc-pharmacy
 edc-pharmacy-dashboard
 edc-prn
 edc-protocol
 edc-protocol-incident
 edc-qol
 edc-randomization
+edc-reference
 edc-refusal
 edc-registration
 edc-reportable
 edc-review-dashboard
 edc-rx
 edc-screening
 edc-search
 edc-sites
 edc-subject-dashboard
+edc-subject-model-wrappers
 edc-timepoint
 edc-transfer
 edc-unblinding
 edc-utils
 edc-visit-schedule
 edc-visit-tracking
 edc-vitals
```

### Comparing `edc-0.5.87/requirements.tests/edc_dev.txt` & `edc-0.5.9/requirements.tests/edc_dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 https://github.com/erikvw/django-crypto-fields/tarball/develop
 https://github.com/erikvw/django-revision/tarball/develop
 https://github.com/clinicedc/edc-action-item/tarball/develop
 https://github.com/clinicedc/edc-adherence/tarball/develop
 https://github.com/clinicedc/edc-adverse-event/tarball/develop
 https://github.com/clinicedc/edc-appointment/tarball/develop
 https://github.com/clinicedc/edc-auth/tarball/develop
-https://github.com/clinicedc/edc-appconfig/tarball/develop
 https://github.com/clinicedc/edc-consent/tarball/develop
 https://github.com/clinicedc/edc-constants/tarball/develop
 https://github.com/clinicedc/edc-crf/tarball/develop
 https://github.com/clinicedc/edc-dashboard/tarball/develop
 https://github.com/clinicedc/edc-data-manager/tarball/develop
 https://github.com/clinicedc/edc-device/tarball/develop
 https://github.com/clinicedc/edc-document-status/tarball/develop
@@ -19,15 +18,14 @@
 https://github.com/clinicedc/edc-dx-review/tarball/develop
 https://github.com/clinicedc/edc-egfr/tarball/develop
 https://github.com/clinicedc/edc-export/tarball/develop
 https://github.com/clinicedc/edc-facility/tarball/develop
 https://github.com/clinicedc/edc-fieldsets/tarball/develop
 https://github.com/clinicedc/edc-form-describer/tarball/develop
 https://github.com/clinicedc/edc-form-label/tarball/develop
-https://github.com/clinicedc/edc-form-runners/tarball/develop
 https://github.com/clinicedc/edc-form-validators/tarball/develop
 https://github.com/clinicedc/edc-glucose/tarball/develop
 https://github.com/clinicedc/edc-identifier/tarball/develop
 https://github.com/clinicedc/edc-lab/tarball/develop
 https://github.com/clinicedc/edc-lab-dashboard/tarball/develop
 https://github.com/clinicedc/edc-lab-panel/tarball/develop
 https://github.com/clinicedc/edc-lab-results/tarball/develop
@@ -36,33 +34,36 @@
 https://github.com/clinicedc/edc-locator/tarball/develop
 https://github.com/clinicedc/edc-ltfu/tarball/develop
 https://github.com/clinicedc/edc-metadata/tarball/develop
 https://github.com/clinicedc/edc-model/tarball/develop
 https://github.com/clinicedc/edc-model-admin/tarball/develop
 https://github.com/clinicedc/edc-model-fields/tarball/develop
 https://github.com/clinicedc/edc-model-form/tarball/develop
+https://github.com/clinicedc/edc-model-wrapper/tarball/develop
 https://github.com/clinicedc/edc-navbar/tarball/develop
 https://github.com/clinicedc/edc-notification/tarball/develop
 https://github.com/clinicedc/edc-offstudy/tarball/develop
 https://github.com/clinicedc/edc-pdf-reports/tarball/develop
 https://github.com/clinicedc/edc-pdutils/tarball/develop
 https://github.com/clinicedc/edc-pharmacy/tarball/develop
 https://github.com/clinicedc/edc-pharmacy-dashboard/tarball/develop
 https://github.com/clinicedc/edc-prn/tarball/develop
 https://github.com/clinicedc/edc-protocol/tarball/develop
 https://github.com/clinicedc/edc-protocol-incident/tarball/develop
 https://github.com/clinicedc/edc-randomization/tarball/develop
+https://github.com/clinicedc/edc-reference/tarball/develop
 https://github.com/clinicedc/edc-refusal/tarball/develop
 https://github.com/clinicedc/edc-registration/tarball/develop
 https://github.com/clinicedc/edc-reportable/tarball/develop
 https://github.com/clinicedc/edc-review-dashboard/tarball/develop
 https://github.com/clinicedc/edc-screening/tarball/develop
 https://github.com/clinicedc/edc-search/tarball/develop
 https://github.com/clinicedc/edc-sites/tarball/develop
 https://github.com/clinicedc/edc-subject-dashboard/tarball/develop
+https://github.com/clinicedc/edc-subject-model-wrappers/tarball/develop
 https://github.com/clinicedc/edc-timepoint/tarball/develop
 https://github.com/clinicedc/edc-transfer/tarball/develop
 https://github.com/clinicedc/edc-unblinding/tarball/develop
 https://github.com/clinicedc/edc-utils/tarball/develop
 https://github.com/clinicedc/edc-visit-schedule/tarball/develop
 https://github.com/clinicedc/edc-visit-tracking/tarball/develop
 https://github.com/clinicedc/edc-vitals/tarball/develop
```

### Comparing `edc-0.5.87/setup.cfg` & `edc-0.5.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.11
+python_requires = >=3.10
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	argon2-cffi
 	boto3
 	celery
@@ -33,97 +34,96 @@
 	pycups
 	pyrabbit
 	python-dateutil
 	python-memcached
 	reportlab
 	tqdm
 	fontawesomefree
-	djangorestframework
 	django-environ
 	django-redis
+	django-audit-fields==0.3.9
+	django-crypto-fields==0.3.5
 	django-defender
+	django-extensions
+	django-logentry-admin
+	django-multisite-edc==2.0.0
+	django-revision==0.3.6
+	django-simple-history>=3.1.1
 	django-storages
-	django-logentry-admin==1.1.0
-	django-extensions==3.2.3
-	django-simple-history==3.5.0
-	django-audit-fields==0.3.17
-	django-crypto-fields==0.4.1
-	django-logentry-admin==1.1.0
-	django-multisite2==2.0.1
-	django-revision==0.3.7
-	edc-action-item==0.3.89
-	edc-adherence==0.3.13
-	edc-adverse-event==0.3.83
-	edc-appconfig==0.1.8
-	edc-appointment==0.4.28
-	edc-auth==0.3.86
-	edc-consent==0.3.83
-	edc-constants==0.3.62
-	edc-crf==0.3.74
-	edc-dashboard==0.3.61
-	edc-data-manager==0.3.77
-	edc-device==0.3.17
-	edc-document-status==0.3.2
-	edc-dx==0.3.7
-	edc-dx-review==0.3.2
-	edc-egfr==0.3.8
-	edc-export==0.3.49
-	edc-facility==0.3.37
-	edc-fieldsets==0.3.21
-	edc-form-describer==0.3.22
-	edc-form-label==0.3.18
-	edc-form-runners==0.3.10
-	edc-form-validators==0.3.40
-	edc-glucose==0.3.6
-	edc-he==0.3.12
-	edc-identifier==0.3.36
-	edc-lab==0.3.60
-	edc-lab-dashboard==0.3.23
-	edc-lab-panel==0.3.5
-	edc-lab-results==0.3.11
-	edc-label==0.3.19
-	edc-list-data==0.3.26
-	edc-listboard==0.3.13
-	edc-locator==0.3.45
-	edc-ltfu==0.3.34
-	edc-metadata==0.3.95
-	edc-mnsi==0.3.5
-	edc-model==0.3.40
-	edc-model-admin==0.3.73
-	edc-model-fields==0.3.12
-	edc-model-form==0.3.2
-	edc-navbar==0.3.28
-	edc-notification==0.3.26
-	edc-offstudy==0.3.47
-	edc-pdf-reports==0.3.20
-	edc-pdutils==0.3.37
-	edc-pharmacy==0.3.9
-	edc-pharmacy-dashboard==0.1.8
-	edc-prn==0.3.24
-	edc-protocol==0.3.16
-	edc-protocol-incident==0.3.5
-	edc-qol==0.3.6
-	edc-randomization==0.3.56
-	edc-refusal==0.3.10
-	edc-registration==0.3.41
-	edc-reportable==0.3.38
-	edc-review-dashboard==0.3.38
-	edc-rx==0.3.1
-	edc-screening==0.3.52
-	edc-search==0.3.11
-	edc-sites==0.3.56
-	edc-subject-dashboard==0.3.71
-	edc-timepoint==0.3.21
-	edc-transfer==0.3.22
-	edc-unblinding==0.3.9
-	edc-utils==0.3.33
-	edc-visit-schedule==0.3.97
-	edc-visit-tracking==0.3.91
-	edc-vitals==0.1.13
-	Django>=4.2.11
+	djangorestframework
+	edc-action-item==0.3.55
+	edc-adherence==0.1.21
+	edc-adverse-event==0.3.55
+	edc-appointment==0.3.74
+	edc-auth==0.3.63
+	edc-consent==0.3.47
+	edc-constants==0.3.49
+	edc-crf==0.3.44
+	edc-dashboard==0.3.45
+	edc-data-manager==0.3.56
+	edc-device==0.3.11
+	edc-document-status==0.1.4
+	edc-dx==0.1.20
+	edc-dx-review==0.1.39
+	edc-egfr==0.1.11
+	edc-export==0.3.31
+	edc-facility==0.3.15
+	edc-fieldsets==0.3.13
+	edc-form-describer==0.3.16
+	edc-form-label==0.3.9
+	edc-form-validators==0.3.34
+	edc-glucose==0.1.30
+	edc-he==0.1.9
+	edc-identifier==0.3.24
+	edc-lab==0.3.44
+	edc-lab-dashboard==0.3.11
+	edc-lab-panel==0.1.15
+	edc-lab-results==0.1.38
+	edc-label==0.3.13
+	edc-list-data==0.3.19
+	edc-listboard==0.1.11
+	edc-locator==0.3.25
+	edc-ltfu==0.3.24
+	edc-metadata==0.3.54
+	edc-mnsi==0.1.17
+	edc-model==0.3.32
+	edc-model-admin==0.3.48
+	edc-model-fields==0.3.7
+	edc-model-form==0.1.12
+	edc-model-wrapper==0.3.10
+	edc-navbar==0.3.16
+	edc-notification==0.3.18
+	edc-offstudy==0.3.33
+	edc-pdf-reports==0.3.14
+	edc-pdutils==0.3.24
+	edc-pharmacy==0.1.39
+	edc-pharmacy-dashboard==0.1.3
+	edc-prn==0.3.14
+	edc-protocol==0.3.10
+	edc-protocol-incident==0.1.26
+	edc-qol==0.1.15
+	edc-randomization==0.3.47
+	edc-reference==0.3.20
+	edc-refusal==0.1.13
+	edc-registration==0.3.30
+	edc-reportable==0.3.31
+	edc-review-dashboard==0.3.19
+	edc-rx==0.1.7
+	edc-screening==0.3.35
+	edc-search==0.3.7
+	edc-sites==0.3.27
+	edc-subject-dashboard==0.3.39
+	edc-subject-model-wrappers==0.3.16
+	edc-timepoint==0.3.11
+	edc-transfer==0.3.14
+	edc-unblinding==0.1.15
+	edc-utils==0.3.20
+	edc-visit-schedule==0.3.62
+	edc-visit-tracking==0.3.53
+	edc-vitals==0.1.11
 
 [options.packages.find]
 exclude = 
 	examples*
 	tools*
 	docs*
 	bin*
```

### Comparing `edc-0.5.87/utils/get_edc_requirements.py` & `edc-0.5.9/utils/get_edc_requirements.py`

 * *Files identical despite different names*

