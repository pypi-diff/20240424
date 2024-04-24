# Comparing `tmp/meta-edc-0.3.8.tar.gz` & `tmp/meta-edc-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta-edc-0.3.8.tar", last modified: Wed Mar 27 20:33:21 2024, max compression
+gzip compressed data, was "meta-edc-0.3.9.tar", last modified: Sun Mar 31 02:04:37 2024, max compression
```

## Comparing `meta-edc-0.3.8.tar` & `meta-edc-0.3.9.tar`

### file list

```diff
@@ -1,1195 +1,1195 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.179777 meta-edc-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       75 2022-04-11 18:27:09.000000 meta-edc-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)     4225 2024-02-13 23:41:07.000000 meta-edc-0.3.8/.env-tests
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.940134 meta-edc-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.957020 meta-edc-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2092 2024-02-13 23:44:08.000000 meta-edc-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1486 2024-02-13 23:41:07.000000 meta-edc-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1227 2024-02-15 06:32:55.000000 meta-edc-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-22 17:23:22.000000 meta-edc-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    13162 2024-03-27 20:33:11.000000 meta-edc-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 23:21:43.000000 meta-edc-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      199 2024-02-13 23:44:08.000000 meta-edc-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2687 2024-03-27 20:33:21.179695 meta-edc-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1798 2024-02-15 06:32:55.000000 meta-edc-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      893 2022-04-11 18:27:09.000000 meta-edc-0.3.8/TODO.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.941933 meta-edc-0.3.8/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.941414 meta-edc-0.3.8/bin/nginx/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.940439 meta-edc-0.3.8/bin/nginx/meta2/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.957974 meta-edc-0.3.8/bin/nginx/meta2/conf/
--rw-r--r--   0 erikvw     (501) staff       (20)      636 2021-08-09 19:25:30.000000 meta-edc-0.3.8/bin/nginx/meta2/conf/live.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      423 2021-08-09 19:25:30.000000 meta-edc-0.3.8/bin/nginx/meta2/conf/live_sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      281 2021-08-09 19:25:30.000000 meta-edc-0.3.8/bin/nginx/meta2/conf/meta.clinicedc.org.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      651 2021-08-09 19:25:30.000000 meta-edc-0.3.8/bin/nginx/meta2/conf/uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      426 2021-08-09 19:25:30.000000 meta-edc-0.3.8/bin/nginx/meta2/conf/uat_sites.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.940489 meta-edc-0.3.8/bin/nginx/meta2/www/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.958163 meta-edc-0.3.8/bin/nginx/meta2/www/html/
--rw-r--r--   0 erikvw     (501) staff       (20)     1439 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta2/www/html/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.958412 meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/
--rw-r--r--   0 erikvw     (501) staff       (20)     1432 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.958658 meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     1636 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.958847 meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/ug/
--rw-r--r--   0 erikvw     (501) staff       (20)     1236 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/ug/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.940869 meta-edc-0.3.8/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.959015 meta-edc-0.3.8/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     1863 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.959167 meta-edc-0.3.8/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/ug/
--rw-r--r--   0 erikvw     (501) staff       (20)     1237 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/ug/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.941057 meta-edc-0.3.8/bin/nginx/meta3/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.960078 meta-edc-0.3.8/bin/nginx/meta3/conf/
--rw-r--r--   0 erikvw     (501) staff       (20)      705 2021-08-09 19:25:29.000000 meta-edc-0.3.8/bin/nginx/meta3/conf/live.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      430 2021-08-09 19:25:29.000000 meta-edc-0.3.8/bin/nginx/meta3/conf/live_sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2021-08-09 19:25:29.000000 meta-edc-0.3.8/bin/nginx/meta3/conf/meta.clinicedc.org.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      728 2021-08-09 19:25:29.000000 meta-edc-0.3.8/bin/nginx/meta3/conf/uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      428 2021-08-09 19:25:29.000000 meta-edc-0.3.8/bin/nginx/meta3/conf/uat_sites.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.941109 meta-edc-0.3.8/bin/nginx/meta3/www/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.960263 meta-edc-0.3.8/bin/nginx/meta3/www/html/
--rw-r--r--   0 erikvw     (501) staff       (20)     1257 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta3/www/html/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.960471 meta-edc-0.3.8/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/
--rw-r--r--   0 erikvw     (501) staff       (20)     1257 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.960660 meta-edc-0.3.8/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     1845 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.941352 meta-edc-0.3.8/bin/nginx/meta3/www/html/uat.meta3.clinicedc.org/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.960861 meta-edc-0.3.8/bin/nginx/meta3/www/html/uat.meta3.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     1867 2021-08-09 19:25:29.000000 meta-edc-0.3.8/bin/nginx/meta3/www/html/uat.meta3.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.941522 meta-edc-0.3.8/bin/nginx/meta4/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.961909 meta-edc-0.3.8/bin/nginx/meta4/conf/
--rw-r--r--   0 erikvw     (501) staff       (20)      705 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/conf/live.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      430 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/conf/live_sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/conf/meta.clinicedc.org.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      728 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/conf/uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      428 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/conf/uat_sites.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.941570 meta-edc-0.3.8/bin/nginx/meta4/www/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.962081 meta-edc-0.3.8/bin/nginx/meta4/www/html/
--rw-r--r--   0 erikvw     (501) staff       (20)     1257 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/www/html/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.962256 meta-edc-0.3.8/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/
--rw-r--r--   0 erikvw     (501) staff       (20)     1257 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.962421 meta-edc-0.3.8/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     1845 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.941804 meta-edc-0.3.8/bin/nginx/meta4/www/html/uat.meta3.clinicedc.org/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.962596 meta-edc-0.3.8/bin/nginx/meta4/www/html/uat.meta3.clinicedc.org/tz/
--rw-r--r--   0 erikvw     (501) staff       (20)     1867 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/nginx/meta4/www/html/uat.meta3.clinicedc.org/tz/index.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.963129 meta-edc-0.3.8/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-04 23:21:43.000000 meta-edc-0.3.8/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-04 23:21:43.000000 meta-edc-0.3.8/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-08-22 17:23:22.000000 meta-edc-0.3.8/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.963840 meta-edc-0.3.8/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-04 23:21:43.000000 meta-edc-0.3.8/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-04 23:21:43.000000 meta-edc-0.3.8/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-04 23:21:43.000000 meta-edc-0.3.8/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-04 23:21:43.000000 meta-edc-0.3.8/bin/systemd/celerybeat.service
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.964540 meta-edc-0.3.8/bin/systemd/meta3/
--rw-r--r--   0 erikvw     (501) staff       (20)      425 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/systemd/meta3/gunicorn-live.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2021-08-09 19:25:30.000000 meta-edc-0.3.8/bin/systemd/meta3/gunicorn-live.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      418 2024-03-12 03:29:53.000000 meta-edc-0.3.8/bin/systemd/meta3/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2021-08-09 19:25:30.000000 meta-edc-0.3.8/bin/systemd/meta3/gunicorn-uat.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.964978 meta-edc-0.3.8/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      375 2020-03-04 23:21:43.000000 meta-edc-0.3.8/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   754498 2024-02-13 23:41:07.000000 meta-edc-0.3.8/docs/forms_reference.md
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.966749 meta-edc-0.3.8/docs/images/
--rw-r--r--   0 erikvw     (501) staff       (20)    86202 2020-03-04 23:21:43.000000 meta-edc-0.3.8/docs/images/user_groups.png
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.967403 meta-edc-0.3.8/docs/updates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.967886 meta-edc-0.3.8/docs/updates/0.1.65/
--rw-r--r--   0 erikvw     (501) staff       (20)    38460 2021-07-06 02:07:00.000000 meta-edc-0.3.8/docs/updates/0.1.65/renamed_fields.txt
--rw-r--r--   0 erikvw     (501) staff       (20)    29315 2021-07-05 21:18:11.000000 meta-edc-0.3.8/docs/updates/0.1.65/update_1_65_renamed_fields.py
--rw-r--r--   0 erikvw     (501) staff       (20)      289 2022-04-11 18:27:09.000000 meta-edc-0.3.8/docs/updates/pharmacy.sql
--rw-r--r--   0 erikvw     (501) staff       (20)     4680 2022-08-22 17:23:22.000000 meta-edc-0.3.8/env.sample
--rw-r--r--   0 erikvw     (501) staff       (20)     1019 2020-04-03 04:33:09.000000 meta-edc-0.3.8/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.942417 meta-edc-0.3.8/label_templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.968747 meta-edc-0.3.8/label_templates/2.25x1.25in/
--rw-r--r--   0 erikvw     (501) staff       (20)      588 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2.25x1.25in/aliquot.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      341 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2.25x1.25in/box.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      337 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2.25x1.25in/manifest.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      520 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2.25x1.25in/requisition.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      299 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2.25x1.25in/subject.lbl
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.969469 meta-edc-0.3.8/label_templates/2x1cm/
--rw-r--r--   0 erikvw     (501) staff       (20)      412 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2x1cm/aliquot.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      297 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2x1cm/box.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2x1cm/manifest.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      387 2020-03-04 23:21:43.000000 meta-edc-0.3.8/label_templates/2x1cm/requisition.lbl
--rwxr-xr-x   0 erikvw     (501) staff       (20)      634 2020-04-03 04:33:09.000000 meta-edc-0.3.8/manage.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.971809 meta-edc-0.3.8/meta_ae/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_ae/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11256 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.974555 meta-edc-0.3.8/meta_ae/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      400 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      484 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/ae_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      834 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/ae_initial_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      478 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/ae_local_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      488 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/ae_sponsor_review_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      463 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/ae_susar_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      449 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/ae_tmg_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2251 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/death_report_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      518 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/death_report_tmg_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      548 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/admin/death_report_tmg_second_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      525 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/admin/hospitalization_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4156 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      159 2021-07-02 03:53:00.000000 meta-edc-0.3.8/meta_ae/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-08-23 13:24:02.000000 meta-edc-0.3.8/meta_ae/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1184 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_ae/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)       36 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_ae/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.977431 meta-edc-0.3.8/meta_ae/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      492 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/forms/ae_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      292 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/forms/ae_initial_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-07-19 13:21:21.000000 meta-edc-0.3.8/meta_ae/forms/ae_local_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-07-19 13:21:21.000000 meta-edc-0.3.8/meta_ae/forms/ae_sponsor_review_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      280 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/forms/ae_susar_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      268 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/forms/ae_tmg_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1424 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/forms/death_report_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      322 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/forms/death_report_tmg_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      340 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/forms/death_report_tmg_second_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      365 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/forms/hospitalization_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      874 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/forms/modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1416 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.983451 meta-edc-0.3.8/meta_ae/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   140317 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2699 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0002_auto_20191024_1000.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2444 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0003_auto_20191102_0033.py
--rw-r--r--   0 erikvw     (501) staff       (20)      997 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0004_auto_20191114_0821.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18484 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0005_auto_20210624_0225.py
--rw-r--r--   0 erikvw     (501) staff       (20)    16966 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0006_aelocalreview_aesponsorreview.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2708 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0007_auto_20210911_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1240 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0008_auto_20211011_1657.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1151 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0009_auto_20220307_1929.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4214 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0010_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2827 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0011_alter_aefollowup_action_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2996 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0012_auto_20220826_0258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2841 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0013_auto_20220826_0322.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1857 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0014_auto_20220826_0406.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1238 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0015_auto_20220907_0157.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5278 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0016_rename_narrative_aetmg_investigator_narrative_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1013 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/migrations/0017_auto_20221130_2257.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1623 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/migrations/0018_alter_deathreporttmg_cause_of_death_agreed_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20955 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/migrations/0019_alter_aefollowup_managers_alter_aeinitial_managers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17482 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/migrations/0020_alter_aesusar_options_alter_aetmg_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4935 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/migrations/0021_alter_aefollowup_site_alter_aeinitial_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    24521 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/migrations/0022_historicalhospitalization_hospitalization.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_ae/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.984053 meta-edc-0.3.8/meta_ae/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2020-05-15 02:40:42.000000 meta-edc-0.3.8/meta_ae/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2666 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/model_mixins/ae_review_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1798 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/model_mixins/death_report_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.986933 meta-edc-0.3.8/meta_ae/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      402 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_ae/models/ae_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      422 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/models/ae_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_ae/models/ae_local_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      240 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_ae/models/ae_sponsor_review.py
--rw-r--r--   0 erikvw     (501) staff       (20)      208 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_ae/models/ae_susar.py
--rw-r--r--   0 erikvw     (501) staff       (20)      226 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_ae/models/ae_tmg.py
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/models/death_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2021-07-05 19:24:26.000000 meta-edc-0.3.8/meta_ae/models/death_report_tmg.py
--rw-r--r--   0 erikvw     (501) staff       (20)      564 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/models/death_report_tmg_second.py
--rw-r--r--   0 erikvw     (501) staff       (20)      802 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/models/hospitalization.py
--rw-r--r--   0 erikvw     (501) staff       (20)      620 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/models/managers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.987981 meta-edc-0.3.8/meta_ae/pdf_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)       84 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/pdf_reports/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      195 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/pdf_reports/ae_pdf_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      207 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/pdf_reports/death_pdf_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      585 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_ae/pdf_reports/meta_pdf_report_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.942952 meta-edc-0.3.8/meta_ae/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.943003 meta-edc-0.3.8/meta_ae/templates/meta_ae/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.988226 meta-edc-0.3.8/meta_ae/templates/meta_ae/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      885 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_ae/templates/meta_ae/bootstrap3/ae_initial_description.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.988636 meta-edc-0.3.8/meta_ae/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_ae/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1215 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_ae/templatetags/meta_ae_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.989220 meta-edc-0.3.8/meta_ae/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_ae/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_ae/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.989493 meta-edc-0.3.8/meta_ae/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_ae/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4915 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_ae/tests/tests/test_actions.py
--rw-r--r--   0 erikvw     (501) staff       (20)      260 2021-07-05 19:24:26.000000 meta-edc-0.3.8/meta_ae/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      197 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_ae/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.990611 meta-edc-0.3.8/meta_auth/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_auth/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-06-24 09:16:28.000000 meta-edc-0.3.8/meta_auth/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1729 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_auth/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2426 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_auth/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-24 09:16:34.000000 meta-edc-0.3.8/meta_auth/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.992404 meta-edc-0.3.8/meta_consent/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_consent/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-06-24 09:14:24.000000 meta-edc-0.3.8/meta_consent/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.993442 meta-edc-0.3.8/meta_consent/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      115 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/admin/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.994017 meta-edc-0.3.8/meta_consent/admin/actions/
--rw-r--r--   0 erikvw     (501) staff       (20)       70 2022-07-08 07:31:04.000000 meta-edc-0.3.8/meta_consent/admin/actions/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1474 2022-07-08 07:31:04.000000 meta-edc-0.3.8/meta_consent/admin/actions/create_missing_prescriptions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5362 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/admin/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      647 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/admin/subject_consent_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      657 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/admin/subject_consent_v1_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-06-24 09:14:27.000000 meta-edc-0.3.8/meta_consent/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      282 2022-08-23 13:24:02.000000 meta-edc-0.3.8/meta_consent/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1343 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_consent/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)      552 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_consent/consents.py
--rw-r--r--   0 erikvw     (501) staff       (20)       31 2022-06-24 09:14:43.000000 meta-edc-0.3.8/meta_consent/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.994384 meta-edc-0.3.8/meta_consent/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)       72 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1258 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/form_validators/subject_consent_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.995033 meta-edc-0.3.8/meta_consent/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1293 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/forms/subject_consent_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/forms/subject_consent_v1_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1306 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/forms/subject_reconsent_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.943663 meta-edc-0.3.8/meta_consent/locale/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.943711 meta-edc-0.3.8/meta_consent/locale/sw/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.995306 meta-edc-0.3.8/meta_consent/locale/sw/LC_MESSAGES/
--rw-r--r--   0 erikvw     (501) staff       (20)     1845 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_consent/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.995559 meta-edc-0.3.8/meta_consent/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_consent/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.995761 meta-edc-0.3.8/meta_consent/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_consent/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1438 2022-07-08 07:31:04.000000 meta-edc-0.3.8/meta_consent/management/commands/create_missing_prescriptions.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.001580 meta-edc-0.3.8/meta_consent/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    66732 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      590 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0002_auto_20191024_1000.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1610 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0003_auto_20200325_0901.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3509 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0004_auto_20210624_0225.py
--rw-r--r--   0 erikvw     (501) staff       (20)      790 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0005_alter_subjectconsent_options.py
--rw-r--r--   0 erikvw     (501) staff       (20)      637 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0006_auto_20210911_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3051 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0007_auto_20220128_1719.py
--rw-r--r--   0 erikvw     (501) staff       (20)      942 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0008_auto_20220412_2151.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1390 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0009_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)      647 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0010_alter_historicalsubjectreconsent_action_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      711 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0011_auto_20220826_0258.py
--rw-r--r--   0 erikvw     (501) staff       (20)      650 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0012_auto_20220826_0322.py
--rw-r--r--   0 erikvw     (501) staff       (20)      492 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0013_auto_20220826_0406.py
--rw-r--r--   0 erikvw     (501) staff       (20)      604 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/migrations/0014_alter_subjectconsent_managers.py
--rw-r--r--   0 erikvw     (501) staff       (20)      755 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0015_auto_20220914_0542.py
--rw-r--r--   0 erikvw     (501) staff       (20)      946 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_consent/migrations/0016_auto_20220914_0547.py
--rw-r--r--   0 erikvw     (501) staff       (20)      923 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/migrations/0017_auto_20220929_1742.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6458 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_consent/migrations/0018_alter_subjectconsent_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6441 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_consent/migrations/0019_alter_subjectconsent_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1110 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_consent/migrations/0020_historicalsubjectconsent_model_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      498 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_consent/migrations/0021_auto_20240111_0442.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1025 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_consent/migrations/0022_alter_historicalsubjectconsent_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2978 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/migrations/0023_subjectconsentv1_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25696 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/migrations/0024_historicalsubjectconsentv1.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6307 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_consent/migrations/0025_alter_historicalsubjectconsent_first_name_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_consent/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.002696 meta-edc-0.3.8/meta_consent/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      223 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-06-24 09:13:53.000000 meta-edc-0.3.8/meta_consent/models/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4557 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_consent/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3803 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/models/subject_consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)      458 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_consent/models/subject_consent_v1.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3595 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_consent/models/subject_reconsent.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.003340 meta-edc-0.3.8/meta_consent/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_consent/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_consent/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.003842 meta-edc-0.3.8/meta_consent/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_consent/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4651 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_consent/tests/tests/test_form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      376 2022-06-24 09:14:16.000000 meta-edc-0.3.8/meta_consent/tests/tests/test_subject_consent.py
--rw-r--r--   0 erikvw     (501) staff       (20)      857 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_consent/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-06-24 09:14:40.000000 meta-edc-0.3.8/meta_consent/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.004865 meta-edc-0.3.8/meta_dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      313 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.944248 meta-edc-0.3.8/meta_dashboard/locale/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.944297 meta-edc-0.3.8/meta_dashboard/locale/sw/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.005052 meta-edc-0.3.8/meta_dashboard/locale/sw/LC_MESSAGES/
--rw-r--r--   0 erikvw     (501) staff       (20)      698 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_dashboard/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.005305 meta-edc-0.3.8/meta_dashboard/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1168 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-06-24 09:14:59.000000 meta-edc-0.3.8/meta_dashboard/patterns.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.944690 meta-edc-0.3.8/meta_dashboard/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.944747 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.944950 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.006468 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/
--rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-08-22 17:23:22.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/add_consent_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      280 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/dashboard_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      401 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/eligibility_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-08-22 17:23:22.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/refusal_button.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1079 2022-08-22 17:23:22.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/screening_button.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.006698 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)     2671 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/screening/listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.007128 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.007303 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)      230 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/dashboard/top_bar.html
--rw-r--r--   0 erikvw     (501) staff       (20)      273 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/dashboard.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1403 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.007649 meta-edc-0.3.8/meta_dashboard/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3947 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/templatetags/meta_dashboard_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.008286 meta-edc-0.3.8/meta_dashboard/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      716 2021-07-05 19:24:26.000000 meta-edc-0.3.8/meta_dashboard/tests/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.008557 meta-edc-0.3.8/meta_dashboard/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2751 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_dashboard/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1193 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.008745 meta-edc-0.3.8/meta_dashboard/view_utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/view_utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3370 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/view_utils/subject_screening_button.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.009019 meta-edc-0.3.8/meta_dashboard/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-08-26 02:59:33.000000 meta-edc-0.3.8/meta_dashboard/views/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.009914 meta-edc-0.3.8/meta_dashboard/views/ae/
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/views/ae/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      452 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_dashboard/views/ae/ae_listboard_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      494 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_dashboard/views/ae/death_report_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.010346 meta-edc-0.3.8/meta_dashboard/views/screening/
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/views/screening/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      578 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_dashboard/views/screening/listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.010741 meta-edc-0.3.8/meta_dashboard/views/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-08-26 02:59:33.000000 meta-edc-0.3.8/meta_dashboard/views/subject/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.011261 meta-edc-0.3.8/meta_dashboard/views/subject/dashboard/
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_dashboard/views/subject/dashboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      344 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_dashboard/views/subject/dashboard/dashboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.011732 meta-edc-0.3.8/meta_dashboard/views/subject/listboard/
--rw-r--r--   0 erikvw     (501) staff       (20)       49 2022-08-26 02:59:33.000000 meta-edc-0.3.8/meta_dashboard/views/subject/listboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      601 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_dashboard/views/subject/listboard/listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.012766 meta-edc-0.3.8/meta_data_manager/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_data_manager/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      233 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_data_manager/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_data_manager/data_manager.py
--rw-r--r--   0 erikvw     (501) staff       (20)      952 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_data_manager/handlers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.016441 meta-edc-0.3.8/meta_edc/
--rw-r--r--   0 erikvw     (501) staff       (20)      186 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_edc/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2022-08-22 17:23:22.000000 meta-edc-0.3.8/meta_edc/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-24 09:07:19.000000 meta-edc-0.3.8/meta_edc/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_edc/asgi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      785 2020-03-04 23:21:43.000000 meta-edc-0.3.8/meta_edc/celery.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.017483 meta-edc-0.3.8/meta_edc/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_edc/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.017672 meta-edc-0.3.8/meta_edc/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_edc/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1003 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_edc/management/commands/update_forms_reference.py
--rw-r--r--   0 erikvw     (501) staff       (20)      211 2022-06-24 09:07:24.000000 meta-edc-0.3.8/meta_edc/meta_version.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1339 2022-07-19 13:21:21.000000 meta-edc-0.3.8/meta_edc/model_callers.py
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-04 23:21:43.000000 meta-edc-0.3.8/meta_edc/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1100 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_edc/navbars.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.018664 meta-edc-0.3.8/meta_edc/settings/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-03 04:33:09.000000 meta-edc-0.3.8/meta_edc/settings/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      911 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_edc/settings/debug.py
--rw-r--r--   0 erikvw     (501) staff       (20)    19233 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_edc/settings/defaults.py
--rw-r--r--   0 erikvw     (501) staff       (20)      216 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_edc/settings/live.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1938 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_edc/settings/logging.py
--rw-r--r--   0 erikvw     (501) staff       (20)      592 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_edc/settings/minimal.py
--rw-r--r--   0 erikvw     (501) staff       (20)      355 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_edc/settings/uat.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.946196 meta-edc-0.3.8/meta_edc/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.946253 meta-edc-0.3.8/meta_edc/templates/meta_edc/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.019094 meta-edc-0.3.8/meta_edc/templates/meta_edc/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/templates/meta_edc/bootstrap3/base.html
--rw-r--r--   0 erikvw     (501) staff       (20)     3780 2022-08-26 02:59:33.000000 meta-edc-0.3.8/meta_edc/templates/meta_edc/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.019435 meta-edc-0.3.8/meta_edc/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 meta-edc-0.3.8/meta_edc/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.020894 meta-edc-0.3.8/meta_edc/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)     5797 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/randomization_list_phase_three.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     6935 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_edc/tests/test_settings.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.021200 meta-edc-0.3.8/meta_edc/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_edc/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    23452 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_edc/tests/tests/test_endpoints.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3435 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_edc/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      342 2022-06-24 09:07:39.000000 meta-edc-0.3.8/meta_edc/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.021542 meta-edc-0.3.8/meta_edc/views/
--rw-r--r--   0 erikvw     (501) staff       (20)       32 2020-03-04 23:21:43.000000 meta-edc-0.3.8/meta_edc/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1006 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_edc/views/home_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)      175 2020-04-03 04:33:09.000000 meta-edc-0.3.8/meta_edc/wsgi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      174 2020-04-03 04:33:09.000000 meta-edc-0.3.8/meta_edc/wsgi_live.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2020-04-03 04:33:09.000000 meta-edc-0.3.8/meta_edc/wsgi_uat.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.179306 meta-edc-0.3.8/meta_edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2687 2024-03-27 20:33:20.000000 meta-edc-0.3.8/meta_edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    46153 2024-03-27 20:33:20.000000 meta-edc-0.3.8/meta_edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-27 20:33:20.000000 meta-edc-0.3.8/meta_edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:21:43.000000 meta-edc-0.3.8/meta_edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       42 2024-03-27 20:33:20.000000 meta-edc-0.3.8/meta_edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      229 2024-03-27 20:33:20.000000 meta-edc-0.3.8/meta_edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.022153 meta-edc-0.3.8/meta_export/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_export/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2021-07-02 03:53:00.000000 meta-edc-0.3.8/meta_export/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      226 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_export/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-06-24 09:12:54.000000 meta-edc-0.3.8/meta_export/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.023877 meta-edc-0.3.8/meta_labs/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-02 03:53:00.000000 meta-edc-0.3.8/meta_labs/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       87 2021-07-05 19:24:26.000000 meta-edc-0.3.8/meta_labs/aliquot_types.py
--rw-r--r--   0 erikvw     (501) staff       (20)      200 2022-08-23 13:24:02.000000 meta-edc-0.3.8/meta_labs/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      957 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_labs/lab_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)      128 2022-06-24 09:12:03.000000 meta-edc-0.3.8/meta_labs/labs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      477 2022-06-24 09:12:00.000000 meta-edc-0.3.8/meta_labs/list_data.py
--rw-r--r--   0 erikvw     (501) staff       (20)      500 2022-06-24 09:11:58.000000 meta-edc-0.3.8/meta_labs/processing_profiles.py
--rw-r--r--   0 erikvw     (501) staff       (20)      512 2022-07-19 19:44:25.000000 meta-edc-0.3.8/meta_labs/reportables.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.024823 meta-edc-0.3.8/meta_labs/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_labs/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      967 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_labs/tests/test_labs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      516 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_labs/tests/test_reportables.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_labs/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.026302 meta-edc-0.3.8/meta_lists/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_lists/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2157 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_lists/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-06-24 09:11:34.000000 meta-edc-0.3.8/meta_lists/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      278 2022-08-23 13:24:02.000000 meta-edc-0.3.8/meta_lists/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9702 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_lists/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.030612 meta-edc-0.3.8/meta_lists/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    13881 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4608 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0002_auto_20191026_2231.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2555 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0003_auto_20191102_0033.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2547 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0004_auto_20191102_1859.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2583 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0005_auto_20191104_0930.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4478 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0006_auto_20200514_1959.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2961 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0007_auto_20200516_2356.py
--rw-r--r--   0 erikvw     (501) staff       (20)      709 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_lists/migrations/0008_auto_20200528_1517.py
--rw-r--r--   0 erikvw     (501) staff       (20)      357 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0009_auto_20200613_2041.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1194 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0010_auto_20200617_1738.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1848 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0011_auto_20210624_0225.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2811 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0012_auto_20210728_1809.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2533 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0013_transferreasons_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2527 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_lists/migrations/0014_auto_20220913_2139.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2212 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_lists/migrations/0015_abnormalfootappearanceobservations_extra_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20692 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_lists/migrations/0016_alter_abnormalfootappearanceobservations_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13041 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_lists/migrations/0017_complications_dmmedications_dmtreatments_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2639 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_lists/migrations/0018_missedreferralreasons.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_lists/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3032 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_lists/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.030799 meta-edc-0.3.8/meta_lists/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_lists/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      212 2022-06-24 09:11:29.000000 meta-edc-0.3.8/meta_lists/tests/test_lists.py
--rw-r--r--   0 erikvw     (501) staff       (20)      204 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_lists/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.031756 meta-edc-0.3.8/meta_pharmacy/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_pharmacy/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      599 2022-08-23 13:24:02.000000 meta-edc-0.3.8/meta_pharmacy/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)       24 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_pharmacy/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.032184 meta-edc-0.3.8/meta_pharmacy/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     1115 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_pharmacy/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_pharmacy/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_pharmacy/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2945 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_pharmacy/prepare_meta_pharmacy.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.034415 meta-edc-0.3.8/meta_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_prn/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7485 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.036546 meta-edc-0.3.8/meta_prn/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      581 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5121 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/end_of_study_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1736 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/loss_to_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2377 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/off_study_medication_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1707 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/offschedule_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1621 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/offschedule_postnatal_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1703 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/offschedule_pregnancy_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1440 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/onschedule_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2144 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/pregnancy_notification_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      739 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/protocol_incident_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      723 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/admin/subject_transfer_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-06-24 09:09:37.000000 meta-edc-0.3.8/meta_prn/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      280 2022-08-23 13:24:02.000000 meta-edc-0.3.8/meta_prn/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      517 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_prn/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3153 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_prn/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      840 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.037170 meta-edc-0.3.8/meta_prn/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_prn/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11246 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/form_validators/end_of_study.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1068 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/form_validators/protocol_incident.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.038745 meta-edc-0.3.8/meta_prn/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      452 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      926 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/forms/end_of_study_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1333 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/forms/loss_to_followup_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2295 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/forms/off_study_medication_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      939 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/forms/offschedule_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1101 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/forms/offschedule_pregnancy_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4897 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/forms/pregnancy_notification_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      231 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/forms/protocol_incident_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      817 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/forms/subject_transfer_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2336 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.052227 meta-edc-0.3.8/meta_prn/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   108119 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2331 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0002_auto_20191024_1000.py
--rw-r--r--   0 erikvw     (501) staff       (20)      881 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0003_auto_20200120_2020.py
--rw-r--r--   0 erikvw     (501) staff       (20)      755 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0004_auto_20200403_0332.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4269 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0005_auto_20200524_1944.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13108 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0006_auto_20210624_0225.py
--rw-r--r--   0 erikvw     (501) staff       (20)      879 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0007_auto_20210721_0335.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3639 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0008_auto_20210910_0238.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2872 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0009_auto_20210910_0239.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2791 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0010_auto_20210910_1906.py
--rw-r--r--   0 erikvw     (501) staff       (20)      934 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/migrations/0011_auto_20210910_1911.py
--rw-r--r--   0 erikvw     (501) staff       (20)      796 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_prn/migrations/0012_auto_20210911_0004.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3117 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0013_auto_20210911_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0014_auto_20211003_1709.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5914 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0015_auto_20211104_1447.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5843 2024-03-07 19:17:25.000000 meta-edc-0.3.8/meta_prn/migrations/0016_auto_20220128_1719.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26858 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0017_auto_20220307_1929.py
--rw-r--r--   0 erikvw     (501) staff       (20)    34941 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0018_auto_20220309_2106.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1165 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0019_auto_20220309_2230.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2041 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0020_auto_20220310_0439.py
--rw-r--r--   0 erikvw     (501) staff       (20)    43328 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0021_auto_20220316_2147.py
--rw-r--r--   0 erikvw     (501) staff       (20)    27548 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0022_auto_20220318_0133.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2418 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0023_auto_20220415_1747.py
--rw-r--r--   0 erikvw     (501) staff       (20)      792 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0024_alter_protocoldeviationviolation_violation.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6264 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0025_alter_historicalprotocoldeviationviolation_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3925 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0026_remove_historicalprotocoldeviationviolation_violation_type_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1284 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0027_rename_historicalprotocoldeviationviolation_historicalprotocolincident_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1919 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0028_historicalpregnancynotification_bhcg_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      661 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0029_alter_historicalpregnancynotification_edd_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1254 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0030_auto_20220627_1119.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1840 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0031_alter_historicaloffschedule_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17575 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0032_historicalegfrnotification_egfrnotification.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1069 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0033_remove_historicalegfrnotification_action_item_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2075 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0034_auto_20220630_1110.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3456 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0035_auto_20220630_1140.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1391 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0036_remove_endofstudy_meta_prn_en_id_a50384_idx_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7338 2024-03-07 19:17:25.000000 meta-edc-0.3.8/meta_prn/migrations/0037_endofstudy_delivery_date_endofstudy_pregnancy_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    21785 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0038_alter_endofstudy_delivery_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1011 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0039_historicaloffstudymedication_reason_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4593 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0040_remove_historicaloffstudymedication_expected_restart_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26299 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0041_endofstudy_transfer_date_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6198 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0042_remove_endofstudy_investigator_decision_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7239 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0043_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3925 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0044_alter_endofstudy_action_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4149 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0045_auto_20220826_0258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3944 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0046_auto_20220826_0322.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2586 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0047_auto_20220826_0406.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2496 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0048_auto_20220922_2236.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3936 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0049_auto_20220929_1742.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1250 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0050_auto_20221004_0629.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1863 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0051_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      642 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/migrations/0052_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    38131 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/migrations/0053_alter_losstofollowup_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    27710 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/migrations/0054_alter_losstofollowup_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8878 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/migrations/0055_alter_endofstudy_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4089 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_prn/migrations/0056_alter_endofstudy_clinical_withdrawal_reason_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_prn/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.054318 meta-edc-0.3.8/meta_prn/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      594 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5316 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/models/end_of_study.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2436 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/models/loss_to_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1701 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/models/off_study_medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1336 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/models/offschedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      677 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/models/onschedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3129 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/models/pregnancy_notification.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1089 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/models/protocol_incident.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2443 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)      266 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/models/subject_transfer.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1018 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/pregnancy_action_item_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.055102 meta-edc-0.3.8/meta_prn/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_prn/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.058993 meta-edc-0.3.8/meta_prn/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_prn/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3811 2024-02-20 05:50:29.000000 meta-edc-0.3.8/meta_prn/tests/tests/test_actions.py
--rw-r--r--   0 erikvw     (501) staff       (20)      548 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_prn/tests/tests/test_manager_order.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3982 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_prn/tests/tests/test_pregnancy_notification.py
--rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-06-24 09:09:29.000000 meta-edc-0.3.8/meta_prn/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      202 2022-06-24 09:09:57.000000 meta-edc-0.3.8/meta_prn/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.060359 meta-edc-0.3.8/meta_rando/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_rando/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-23 13:24:02.000000 meta-edc-0.3.8/meta_rando/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.061555 meta-edc-0.3.8/meta_rando/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    13432 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_rando/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_rando/migrations/0002_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1225 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_rando/migrations/0003_auto_20220826_1640.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3572 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_rando/migrations/0004_alter_randomizationlist_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3248 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_rando/migrations/0005_alter_randomizationlist_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_rando/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      532 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_rando/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1591 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_rando/randomizers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.061653 meta-edc-0.3.8/meta_rando/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_rando/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.061836 meta-edc-0.3.8/meta_rando/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.8/meta_rando/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2278 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_rando/tests/tests/test_randomizers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.062858 meta-edc-0.3.8/meta_reports/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_reports/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_reports/ae_report.py
--rw-r--r--   0 erikvw     (501) staff       (20)      733 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_reports/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4713 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_reports/death_report.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.063013 meta-edc-0.3.8/meta_reports/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_reports/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_reports/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2395 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_reports/pdf_report.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.063626 meta-edc-0.3.8/meta_reports/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_reports/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_reports/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     1293 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_reports/tests/test_reports.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_reports/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.065948 meta-edc-0.3.8/meta_screening/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_screening/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.068086 meta-edc-0.3.8/meta_screening/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_screening/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5076 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/admin/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2534 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1067 2024-02-20 05:46:58.000000 meta-edc-0.3.8/meta_screening/admin/screening_part_one_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2592 2024-02-20 05:47:03.000000 meta-edc-0.3.8/meta_screening/admin/screening_part_three_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1278 2024-02-20 05:50:29.000000 meta-edc-0.3.8/meta_screening/admin/screening_part_two_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2244 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_screening/admin/subject_refusal_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6925 2024-02-20 05:50:29.000000 meta-edc-0.3.8/meta_screening/admin/subject_screening_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-10-18 02:37:22.000000 meta-edc-0.3.8/meta_screening/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      543 2022-08-23 13:24:02.000000 meta-edc-0.3.8/meta_screening/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1705 2022-06-24 09:06:35.000000 meta-edc-0.3.8/meta_screening/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1948 2022-06-24 09:06:38.000000 meta-edc-0.3.8/meta_screening/calculators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      789 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_screening/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      655 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_screening/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.069158 meta-edc-0.3.8/meta_screening/eligibility/
--rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-08-22 17:23:22.000000 meta-edc-0.3.8/meta_screening/eligibility/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7732 2022-07-08 07:31:04.000000 meta-edc-0.3.8/meta_screening/eligibility/eligibility.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1769 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_one.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.069954 meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_three/
--rw-r--r--   0 erikvw     (501) staff       (20)       79 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_three/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5405 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_three/base_eligibility_part_three.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4296 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_three/eligibility_part_three_phase_three.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1808 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_two.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.071343 meta-edc-0.3.8/meta_screening/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      308 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_screening/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1213 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_screening/form_validators/screening_part_one.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7606 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/form_validators/screening_part_three.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4738 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_screening/form_validators/screening_part_two.py
--rw-r--r--   0 erikvw     (501) staff       (20)      322 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/form_validators/subject_refusal.py
--rw-r--r--   0 erikvw     (501) staff       (20)      309 2022-06-24 09:04:37.000000 meta-edc-0.3.8/meta_screening/form_validators/subject_screening.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.072996 meta-edc-0.3.8/meta_screening/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      614 2022-07-19 13:21:21.000000 meta-edc-0.3.8/meta_screening/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3291 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/forms/field_lists.py
--rw-r--r--   0 erikvw     (501) staff       (20)      798 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_screening/forms/screening_part_one_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      987 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/forms/screening_part_three_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      701 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/forms/screening_part_two_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      624 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/forms/subject_refusal_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      643 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_screening/forms/subject_screening_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.091146 meta-edc-0.3.8/meta_screening/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   186855 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4467 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0002_auto_20191020_0612.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5513 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0003_auto_20191020_0627.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14316 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0004_auto_20191020_0738.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10372 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0005_auto_20191021_0353.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6710 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0006_auto_20191022_0134.py
--rw-r--r--   0 erikvw     (501) staff       (20)      950 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0007_auto_20191024_1000.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6148 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0008_auto_20191031_0745.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6108 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0009_auto_20191105_0122.py
--rw-r--r--   0 erikvw     (501) staff       (20)    36963 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0010_auto_20191106_0828.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7246 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_screening/migrations/0011_auto_20191107_0342.py
--rw-r--r--   0 erikvw     (501) staff       (20)      797 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_screening/migrations/0012_auto_20191107_0427.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7882 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0013_auto_20191107_0442.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17407 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0014_auto_20191107_0528.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1186 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0015_auto_20191107_2249.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4803 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0016_auto_20191119_2331.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2821 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0017_auto_20191213_0314.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5089 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0018_auto_20200118_1854.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4108 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0019_auto_20200120_2256.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8402 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0020_auto_20200524_1944.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25508 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0021_auto_20210628_2105.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2291 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0022_auto_20210702_0426.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2892 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0023_auto_20210702_0533.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4283 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0024_auto_20210710_1929.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4815 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0025_auto_20210710_2247.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2421 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0026_auto_20210712_0433.py
--rw-r--r--   0 erikvw     (501) staff       (20)      226 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0027_auto_20210804_0438.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14429 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0028_auto_20210823_2353.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25296 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0029_auto_20211123_1645.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1611 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0030_auto_20220128_1719.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10215 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0031_auto_20220304_0448.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5506 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0032_auto_20220304_0501.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2167 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0033_auto_20220304_0504.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6546 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0034_auto_20220304_0508.py
--rw-r--r--   0 erikvw     (501) staff       (20)    36492 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0035_auto_20220304_2233.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5609 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0036_auto_20220304_2307.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5029 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0037_auto_20220312_0339.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10872 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0038_auto_20220312_1929.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6642 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0039_auto_20220312_1938.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20940 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0040_auto_20220316_2147.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2662 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0041_auto_20220403_1227.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15665 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0042_auto_20220403_1402.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5504 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0043_auto_20220407_1713.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4908 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0044_alter_historicalscreeningpartone_severe_htn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1918 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0045_historicalscreeningpartone_contact_number_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1983 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0046_historicalscreeningpartone_hba1c_datetime_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2353 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0047_historicalscreeningpartone_appt_datetime_repeat_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1191 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0048_rename_appt_datetime_repeat_historicalscreeningpartone_repeat_appt_datetime_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9619 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0049_historicalscreeningpartone_p3_ltfu_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11994 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0050_historicalscreeningpartone_agree_to_p3_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11971 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0051_alter_historicalscreeningpartone_advised_to_fast_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3890 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0052_alter_historicalscreeningpartone_p3_ltfu_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3781 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0053_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6028 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0054_auto_20220722_2130.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18773 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0055_alter_historicalscreeningpartone_creatinine_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4224 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0056_alter_historicalscreeningpartone_agree_to_p3_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13643 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0057_alter_historicalscreeningpartone_calculated_egfr_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7511 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/migrations/0058_alter_historicalscreeningpartone_eligibility_datetime_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12718 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_screening/migrations/0059_alter_icpreferral_managers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6812 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_screening/migrations/0060_historicalicpreferral_locale_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4465 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_screening/migrations/0061_alter_historicalicpreferral_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      641 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_screening/migrations/0062_remove_icpreferral_site_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_screening/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.092421 meta-edc-0.3.8/meta_screening/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      315 2022-08-26 02:59:33.000000 meta-edc-0.3.8/meta_screening/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2761 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/model_mixins/calculated_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      592 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/model_mixins/creatinine_fields_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1360 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/model_mixins/eligibility_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3708 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/model_mixins/part_one_fields_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4974 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_screening/model_mixins/part_three_fields_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6692 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/model_mixins/part_two_fields_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.093543 meta-edc-0.3.8/meta_screening/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      262 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_screening/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3465 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_screening/models/icp_referral.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1175 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_screening/models/proxy_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      862 2022-08-26 02:59:33.000000 meta-edc-0.3.8/meta_screening/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2253 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_screening/models/subject_refusal.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2269 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_screening/models/subject_screening.py
--rw-r--r--   0 erikvw     (501) staff       (20)      131 2022-06-24 09:06:52.000000 meta-edc-0.3.8/meta_screening/offline_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.094335 meta-edc-0.3.8/meta_screening/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_screening/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_screening/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     8264 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_screening/tests/meta_test_case_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4097 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_screening/tests/options.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.095385 meta-edc-0.3.8/meta_screening/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-0.3.8/meta_screening/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    16710 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/tests/tests/test_forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4723 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_screening/tests/tests/test_screening_part_one.py
--rw-r--r--   0 erikvw     (501) staff       (20)    16774 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/tests/tests/test_screening_part_three.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3126 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_screening/tests/tests/test_screening_part_two.py
--rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-06-24 09:06:56.000000 meta-edc-0.3.8/meta_screening/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.096056 meta-edc-0.3.8/meta_sites/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_sites/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      278 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_sites/apps.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.096170 meta-edc-0.3.8/meta_sites/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-06-18 19:11:34.000000 meta-edc-0.3.8/meta_sites/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_sites/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1625 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_sites/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.096528 meta-edc-0.3.8/meta_sites/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_sites/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      415 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_sites/tests/test_sites.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-24 09:03:07.000000 meta-edc-0.3.8/meta_sites/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.097051 meta-edc-0.3.8/meta_stats/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_stats/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      540 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_stats/incidence.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_stats/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.097147 meta-edc-0.3.8/meta_stats/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_stats/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.097333 meta-edc-0.3.8/meta_stats/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_stats/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      313 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_stats/tests/tests/test_incidence.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.099537 meta-edc-0.3.8/meta_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5930 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.106421 meta-edc-0.3.8/meta_subject/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)     1714 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-06-24 08:59:56.000000 meta-edc-0.3.8/meta_subject/admin/autocomplete_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3189 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/birth_outcome_admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.107573 meta-edc-0.3.8/meta_subject/admin/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      356 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/admin/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      799 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_fbc_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      861 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_hba1c_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      822 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_ins_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      822 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_lft_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      836 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_lipid_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5120 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_rft_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1017 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/complications_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4069 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/complications_glycemia_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      824 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/concomitant_medication_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3426 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/admin/delivery_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2774 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/admin/dm_referral_followup_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      627 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/egfr_drop_notification_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      772 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/eq5d3l_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-06-24 09:00:25.000000 meta-edc-0.3.8/meta_subject/admin/fields.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1523 2022-06-24 09:00:28.000000 meta-edc-0.3.8/meta_subject/admin/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5153 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/admin/followup_examination_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1585 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/admin/followup_vitals_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2971 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/admin/glucose_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1716 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/admin/glucose_fbg_admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.108435 meta-edc-0.3.8/meta_subject/admin/health_economics/
--rw-r--r--   0 erikvw     (501) staff       (20)      140 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/admin/health_economics/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1037 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/admin/health_economics/health_economics_simple_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3889 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/admin/health_economics/health_economics_update_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1404 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/hepatitis_test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2264 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      492 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/malaria_test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      543 2024-03-11 21:08:18.000000 meta-edc-0.3.8/meta_subject/admin/medication_adherence_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1430 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/mnsi_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      510 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/modeladmin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1596 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/other_arv_regimens_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1763 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/patient_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1858 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/physical_exam_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      913 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/pregnancy_update_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      742 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/sf12_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5983 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/admin/study_medication_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1848 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/subject_requisition_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1314 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/admin/subject_visit_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1414 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/subject_visit_missed_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1144 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/urine_dipstick_test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1037 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/admin/urine_pregnancy_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-08-21 16:43:17.000000 meta-edc-0.3.8/meta_subject/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      289 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2618 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_subject/baker_recipes.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6610 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      662 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.110316 meta-edc-0.3.8/meta_subject/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      349 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/form_validators/birth_outcomes_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3193 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/form_validators/delivery_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6293 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/form_validators/dm_referral_followup_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      530 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/form_validators/egfr_drop_notification_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4241 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/form_validators/followup_examination_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3371 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/form_validators/glucose_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      250 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/form_validators/health_economics_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.116153 meta-edc-0.3.8/meta_subject/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)     1646 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      374 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/birth_outcomes_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.117229 meta-edc-0.3.8/meta_subject/forms/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      344 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      714 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_fbc_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_hba1c_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      722 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_ins_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      714 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_lft_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      730 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_lipid_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1362 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_rft_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      375 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/complications_glycemia_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      375 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/concomitant_medication_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      447 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/delivery_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      567 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/dm_referral_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      507 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/egfr_drop_notification_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/eq53d3l_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      502 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/followup_examination_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      354 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/followup_vitals_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1267 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/glucose_fbg_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      442 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/glucose_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.117693 meta-edc-0.3.8/meta_subject/forms/health_economics/
--rw-r--r--   0 erikvw     (501) staff       (20)      136 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/forms/health_economics/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      392 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/forms/health_economics/health_economics_simple_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      308 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/forms/health_economics/health_economics_update_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      794 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/hepatitis_test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      365 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/malaria_test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      865 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/medication_adherence_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2084 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_subject/forms/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      323 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/mnsi_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      962 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/other_arv_regimens_detail_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1687 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/other_arv_regimens_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1807 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/patient_history_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      786 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/physical_exam_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      559 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/pregnancy_update_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-06-24 08:54:57.000000 meta-edc-0.3.8/meta_subject/forms/sf12_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      821 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/slider_widget.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1481 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/study_medication_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      953 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/subject_requisition_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      791 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/forms/subject_visit_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2275 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/subject_visit_missed_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      827 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/urine_dipstick_test_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1267 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/forms/urine_pregnancy_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      325 2022-08-26 02:59:33.000000 meta-edc-0.3.8/meta_subject/identifiers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.949895 meta-edc-0.3.8/meta_subject/locale/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.949951 meta-edc-0.3.8/meta_subject/locale/sw/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.117840 meta-edc-0.3.8/meta_subject/locale/sw/LC_MESSAGES/
--rw-r--r--   0 erikvw     (501) staff       (20)     5685 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.950062 meta-edc-0.3.8/meta_subject/management/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.118477 meta-edc-0.3.8/meta_subject/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)     2432 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/management/commands/create_missing_refills.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1463 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_subject/management/commands/create_missing_rx.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8209 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/management/commands/missed.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.119155 meta-edc-0.3.8/meta_subject/metadata_rules/
--rw-r--r--   0 erikvw     (501) staff       (20)       53 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_subject/metadata_rules/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3438 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/metadata_rules/metadata_rules.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7117 2024-02-20 05:50:29.000000 meta-edc-0.3.8/meta_subject/metadata_rules/predicates.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.158437 meta-edc-0.3.8/meta_subject/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   408932 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    29351 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0002_auto_20191021_0353.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4024 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0003_auto_20191021_0534.py
--rw-r--r--   0 erikvw     (501) staff       (20)      739 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0004_auto_20191022_0134.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5818 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0005_auto_20191024_1000.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20050 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0006_auto_20191104_0756.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1141 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0007_auto_20191107_2249.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13943 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0008_auto_20191115_0132.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1129 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0009_auto_20191119_2331.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6879 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0010_auto_20191213_0314.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2779 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0011_auto_20200118_1854.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15554 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0012_auto_20200118_2334.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1829 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0013_auto_20200119_0013.py
--rw-r--r--   0 erikvw     (501) staff       (20)    32038 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0014_auto_20200120_1622.py
--rw-r--r--   0 erikvw     (501) staff       (20)      785 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0015_auto_20200120_1943.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2035 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0016_auto_20200123_1508.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7291 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0017_auto_20200325_0901.py
--rw-r--r--   0 erikvw     (501) staff       (20)    59621 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0018_coronakap_historicalcoronakap.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1560 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0019_auto_20200417_0315.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7013 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0020_auto_20200417_0329.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1177 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0021_auto_20200417_0332.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5512 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0022_auto_20200419_2223.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25415 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0023_auto_20200419_2305.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14715 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0024_auto_20200419_2331.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7347 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0025_auto_20200420_1455.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1091 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0026_auto_20200420_1524.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4755 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0027_auto_20200420_1645.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6449 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0028_auto_20200420_1732.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6003 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0029_auto_20200420_1751.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5045 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0030_auto_20200420_1816.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4609 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0031_auto_20200422_2039.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7735 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0032_auto_20200515_0307.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18672 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0033_auto_20200516_2356.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1004 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0034_auto_20200517_0125.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1316 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0035_auto_20200517_0128.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2987 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0036_auto_20200517_0150.py
--rw-r--r--   0 erikvw     (501) staff       (20)      587 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0037_auto_20200517_0207.py
--rw-r--r--   0 erikvw     (501) staff       (20)    26376 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0038_auto_20200520_0020.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6635 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0039_auto_20200524_1944.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18299 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0040_auto_20200527_2155.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12473 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0041_auto_20200528_0242.py
--rw-r--r--   0 erikvw     (501) staff       (20)      223 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0042_auto_20200528_0252.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1509 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0043_auto_20200528_1555.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2845 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0044_auto_20200528_1853.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1244 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0045_auto_20200530_1801.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3313 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0046_auto_20200530_1804.py
--rw-r--r--   0 erikvw     (501) staff       (20)      589 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0047_auto_20200530_1819.py
--rw-r--r--   0 erikvw     (501) staff       (20)      431 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0048_auto_20200530_1819.py
--rw-r--r--   0 erikvw     (501) staff       (20)      265 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0049_auto_20200613_2041.py
--rw-r--r--   0 erikvw     (501) staff       (20)      876 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0050_auto_20200614_1934.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20316 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0051_auto_20200617_2117.py
--rw-r--r--   0 erikvw     (501) staff       (20)    40851 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0052_auto_20210624_0225.py
--rw-r--r--   0 erikvw     (501) staff       (20)    27484 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0053_auto_20210628_2105.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3375 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0054_auto_20210628_2314.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2931 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0055_auto_20210628_2331.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3543 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0056_auto_20210702_0426.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2827 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0057_auto_20210702_0458.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1981 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0058_auto_20210702_0533.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14817 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0059_auto_20210709_2056.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1311 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0060_auto_20210709_2241.py
--rw-r--r--   0 erikvw     (501) staff       (20)    36061 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0061_auto_20210710_1929.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1007 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0062_auto_20210713_0616.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20740 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0063_auto_20210715_0337.py
--rw-r--r--   0 erikvw     (501) staff       (20)    31933 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0064_auto_20210715_2336.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10393 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0065_auto_20210716_0813.py
--rw-r--r--   0 erikvw     (501) staff       (20)    27932 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0066_auto_20210721_0335.py
--rw-r--r--   0 erikvw     (501) staff       (20)    47359 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0067_auto_20210726_0340.py
--rw-r--r--   0 erikvw     (501) staff       (20)    41022 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0068_auto_20210728_1809.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2083 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0069_auto_20210801_2021.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2865 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0070_auto_20210804_0438.py
--rw-r--r--   0 erikvw     (501) staff       (20)      995 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0071_auto_20210804_0715.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25832 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0072_auto_20210805_1545.py
--rw-r--r--   0 erikvw     (501) staff       (20)    41644 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0073_auto_20210809_0055.py
--rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_subject/migrations/0074_auto_20210809_1744.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1996 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0075_auto_20210809_1744.py
--rw-r--r--   0 erikvw     (501) staff       (20)      973 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0076_auto_20210809_1854.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8020 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0077_auto_20210809_2323.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1194 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0078_auto_20210810_0857.py
--rw-r--r--   0 erikvw     (501) staff       (20)    35483 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0079_auto_20210812_0335.py
--rw-r--r--   0 erikvw     (501) staff       (20)    17307 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0080_auto_20210812_0400.py
--rw-r--r--   0 erikvw     (501) staff       (20)    27695 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0081_auto_20210817_2306.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12293 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0082_auto_20210823_1612.py
--rw-r--r--   0 erikvw     (501) staff       (20)    14438 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0083_auto_20210823_1620.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15218 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0084_auto_20210910_0234.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2961 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0085_auto_20210911_2036.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15644 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0086_auto_20210920_0229.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2917 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0087_auto_20210922_2058.py
--rw-r--r--   0 erikvw     (501) staff       (20)    28868 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0088_auto_20210924_0027.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6593 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0089_auto_20210924_0121.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15971 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0090_auto_20210924_0424.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1875 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0091_auto_20210929_2324.py
--rw-r--r--   0 erikvw     (501) staff       (20)    16399 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0092_auto_20211013_0447.py
--rw-r--r--   0 erikvw     (501) staff       (20)    33887 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0093_auto_20211117_0352.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4811 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0094_auto_20211123_1645.py
--rw-r--r--   0 erikvw     (501) staff       (20)    22478 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0095_auto_20220128_1719.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3418 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0096_auto_20220304_0501.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2099 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0097_auto_20220304_2233.py
--rw-r--r--   0 erikvw     (501) staff       (20)    21282 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0098_auto_20220309_2106.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1908 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0099_auto_20220309_2218.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1090 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0100_auto_20220309_2238.py
--rw-r--r--   0 erikvw     (501) staff       (20)    61583 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0101_auto_20220316_2147.py
--rw-r--r--   0 erikvw     (501) staff       (20)    15290 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0102_auto_20220324_0304.py
--rw-r--r--   0 erikvw     (501) staff       (20)      868 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0103_auto_20220324_0326.py
--rw-r--r--   0 erikvw     (501) staff       (20)      966 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0104_auto_20220412_2151.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1290 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0105_auto_20220412_2310.py
--rw-r--r--   0 erikvw     (501) staff       (20)      772 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0106_auto_20220414_1741.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1492 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0107_auto_20220415_0043.py
--rw-r--r--   0 erikvw     (501) staff       (20)      688 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0108_auto_20220415_1747.py
--rw-r--r--   0 erikvw     (501) staff       (20)      556 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0109_auto_20220415_1758.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2516 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0110_auto_20220512_1811.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3010 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0111_alter_followupvitals_severe_htn_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1035 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0112_historicalsubjectvisit_document_status_comments_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      719 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0113_bloodresultsrft_egfr_percent_change_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      991 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0114_alter_bloodresultsrft_egfr_percent_change_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18446 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0115_historicalegfrnotification_egfrnotification.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1176 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0116_egfrnotification_report_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3278 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0117_alter_egfrnotification_managers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2049 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0118_delivery_crf_status_delivery_crf_status_comments_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0119_historicalstudymedication_roundup_divisible_by_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2887 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0120_alter_birthoutcomes_managers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    21740 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0121_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)      812 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0122_auto_20220708_2144.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8262 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0123_auto_20220714_2136.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1206 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0124_auto_20220714_2303.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1568 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0125_auto_20220719_2134.py
--rw-r--r--   0 erikvw     (501) staff       (20)      776 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0126_auto_20220719_2142.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5488 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0127_auto_20220720_0053.py
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0128_auto_20220720_0055.py
--rw-r--r--   0 erikvw     (501) staff       (20)      490 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0129_auto_20220720_0108.py
--rw-r--r--   0 erikvw     (501) staff       (20)      683 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0130_auto_20220720_0216.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1932 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0131_auto_20220722_0411.py
--rw-r--r--   0 erikvw     (501) staff       (20)      843 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0132_auto_20220722_1825.py
--rw-r--r--   0 erikvw     (501) staff       (20)    28130 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0133_auto_20220722_2140.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1806 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0134_auto_20220722_2211.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2263 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0135_auto_20220722_2212.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8660 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0136_egfrdropnotification_creatinine_quantifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1138 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0137_alter_egfrdropnotification_egfr_percent_change_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3531 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0138_alter_glucose_fbg_datetime_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      938 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0139_alter_bloodresultsins_ins_units_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4341 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0140_alter_bloodresultsfbc_action_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4570 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0141_auto_20220826_0258.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5196 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0142_auto_20220826_0322.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3810 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0143_auto_20220826_0406.py
--rw-r--r--   0 erikvw     (501) staff       (20)      964 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0144_auto_20220907_0157.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1785 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0145_auto_20220907_0202.py
--rw-r--r--   0 erikvw     (501) staff       (20)      618 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0146_auto_20220907_0207.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1906 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0147_auto_20220907_1505.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1814 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0148_auto_20220908_1826.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1000 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0149_auto_20220913_2139.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1222 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0150_auto_20220914_0039.py
--rw-r--r--   0 erikvw     (501) staff       (20)    52998 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0151_auto_20220918_0508.py
--rw-r--r--   0 erikvw     (501) staff       (20)      738 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0152_auto_20220925_0509.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1172 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0153_auto_20220928_0250.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1010 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0154_auto_20220928_0419.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9271 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0155_auto_20220929_1742.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5444 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0156_alter_bloodresultsfbc_assay_datetime_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    23251 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0157_remove_bloodresultsfbc_crf_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2191 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0158_alter_followupexamination_attended_clinic_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6479 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0159_alter_bloodresultsfbc_results_abnormal_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1614 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/migrations/0160_alter_healtheconomicssimple_education_certificate_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)   129780 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0161_alter_birthoutcomes_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2347 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/migrations/0162_alter_followupexamination_abdominal_tenderness_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)   114643 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0163_alter_birthoutcomes_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    29185 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0164_dmreferralfollowup_historicaldmreferralfollowup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      687 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0165_alter_dmreferralfollowup_healthcare_workers.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7299 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0166_rename_dm_medications_other_dmreferralfollowup_other_dm_medications_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      704 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0167_rename_healthcare_workers_other_dmreferralfollowup_other_healthcare_workers_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1926 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0168_alter_dmreferralfollowup_last_missed_pill_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3695 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0169_alter_dmreferralfollowup_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1748 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0170_remove_glucose_repeat_fbg_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2813 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0171_alter_glucose_endpoint_today_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2328 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0172_remove_historicalbloodresultsglu_action_item_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3429 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0173_alter_glucosefbg_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3274 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0174_remove_glucosefbg_glucose_abnormal_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      677 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0175_auto_20240214_2239.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1302 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/migrations/0176_alter_glucosefbg_glucose_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3001 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/migrations/0177_alter_bloodresultslft_alp_value_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    31556 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/migrations/0178_historicalhealtheconomicsupdate_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)    32903 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/migrations/0179_alter_birthoutcomes_consent_model_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2301 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/migrations/0180_dmreferralfollowup_missed_referral_reasons_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_subject/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.159704 meta-edc-0.3.8/meta_subject/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      286 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2904 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_subject/model_mixins/arv_history_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      248 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/model_mixins/crf_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      298 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/model_mixins/crf_with_action_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-06-24 08:52:03.000000 meta-edc-0.3.8/meta_subject/model_mixins/search_slug_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1160 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/model_mixins/vitals_fields_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.166431 meta-edc-0.3.8/meta_subject/models/
--rw-r--r--   0 erikvw     (501) staff       (20)     1715 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3033 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/birth_outcomes.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.167647 meta-edc-0.3.8/meta_subject/models/blood_results/
--rw-r--r--   0 erikvw     (501) staff       (20)      290 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/blood_results/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1252 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_fbc.py
--rw-r--r--   0 erikvw     (501) staff       (20)      958 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_hba1c.py
--rw-r--r--   0 erikvw     (501) staff       (20)      974 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_ins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1157 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_lft.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1090 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_lipid.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1568 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_rft.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1849 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/complications.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6056 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/complications_glycemia.py
--rw-r--r--   0 erikvw     (501) staff       (20)      368 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/concomitant_medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5100 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/delivery.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1063 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/models/diet_and_lifestyle.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5937 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/models/dm_referral_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      557 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/egfr_drop_notification.py
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/eq5d3l.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8116 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/models/followup_examination.py
--rw-r--r--   0 erikvw     (501) staff       (20)      903 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/models/followup_vitals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2539 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/glucose.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2101 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/glucose_fbg.py
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/glucose_review.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.169850 meta-edc-0.3.8/meta_subject/models/health_economics/
--rw-r--r--   0 erikvw     (501) staff       (20)      164 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/models/health_economics/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9715 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/models/health_economics/health_economics.py
--rw-r--r--   0 erikvw     (501) staff       (20)      741 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/models/health_economics/health_economics_simple.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3210 2024-03-08 06:41:57.000000 meta-edc-0.3.8/meta_subject/models/health_economics/health_economics_update.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1850 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/hepatitis_test.py
--rw-r--r--   0 erikvw     (501) staff       (20)      343 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/malaria_test.py
--rw-r--r--   0 erikvw     (501) staff       (20)      399 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)      284 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/mnsi.py
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/off_study_drug.py
--rw-r--r--   0 erikvw     (501) staff       (20)      607 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/other_arv_regimens.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1828 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/other_arv_regimens_detail.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4510 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/patient_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1971 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/models/physical_exam.py
--rw-r--r--   0 erikvw     (501) staff       (20)      949 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/pregnancy_update.py
--rw-r--r--   0 erikvw     (501) staff       (20)      283 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/models/sf12.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3989 2022-07-08 07:31:04.000000 meta-edc-0.3.8/meta_subject/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)      461 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/study_medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)      342 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/models/subject_requisition.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2152 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/models/subject_visit.py
--rw-r--r--   0 erikvw     (501) staff       (20)      747 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/subject_visit_missed.py
--rw-r--r--   0 erikvw     (501) staff       (20)      247 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_subject/models/todo.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1178 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/urine_dipstick_test.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1336 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/models/urine_pregnancy.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.950549 meta-edc-0.3.8/meta_subject/static/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.170324 meta-edc-0.3.8/meta_subject/static/meta_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)     1359 2022-08-22 17:23:22.000000 meta-edc-0.3.8/meta_subject/static/meta_subject/slider.css
--rw-r--r--   0 erikvw     (501) staff       (20)    10150 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_subject/static/meta_subject/slider.png
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:20.950655 meta-edc-0.3.8/meta_subject/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.170625 meta-edc-0.3.8/meta_subject/templates/meta_subject/
--rw-r--r--   0 erikvw     (501) staff       (20)      270 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/templates/meta_subject/endpoint_review_instructions.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.170799 meta-edc-0.3.8/meta_subject/templates/meta_subject/widgets/
--rw-r--r--   0 erikvw     (501) staff       (20)      913 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_subject/templates/meta_subject/widgets/slider.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.171282 meta-edc-0.3.8/meta_subject/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_subject/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_subject/tests/holidays.csv
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.173746 meta-edc-0.3.8/meta_subject/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-0.3.8/meta_subject/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9994 2024-03-27 20:33:11.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_egfr.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2454 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_fixes.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1871 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_followup.py
--rw-r--r--   0 erikvw     (501) staff       (20)      454 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_manager_order.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2517 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_medication_adherence.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4445 2022-08-22 17:23:22.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_metadata_rules.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9964 2024-02-20 05:50:29.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_mnsi.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2827 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_patient_history_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2947 2024-03-27 19:35:21.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_physical_exam.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7330 2024-02-20 05:50:29.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_sf12.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10161 2024-02-13 23:41:07.000000 meta-edc-0.3.8/meta_subject/tests/tests/test_study_medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1109 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_subject/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-06-24 09:02:28.000000 meta-edc-0.3.8/meta_subject/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.174611 meta-edc-0.3.8/meta_visit_schedule/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-07 23:18:25.000000 meta-edc-0.3.8/meta_visit_schedule/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      164 2021-07-02 03:53:00.000000 meta-edc-0.3.8/meta_visit_schedule/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      423 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_visit_schedule/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.174708 meta-edc-0.3.8/meta_visit_schedule/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_visit_schedule/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_visit_schedule/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.174898 meta-edc-0.3.8/meta_visit_schedule/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/meta_visit_schedule/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.175251 meta-edc-0.3.8/meta_visit_schedule/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-0.3.8/meta_visit_schedule/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7239 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_visit_schedule/tests/tests/test_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-0.3.8/meta_visit_schedule/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.175514 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/
--rw-r--r--   0 erikvw     (501) staff       (20)      339 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.176941 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-04-11 18:27:09.000000 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11947 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/crfs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/crfs_pregnancy.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3959 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/requisitions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6881 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1123 2024-02-15 06:32:55.000000 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/schedule_pregnancy.py
--rw-r--r--   0 erikvw     (501) staff       (20)      537 2024-02-13 23:44:08.000000 meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1734 2024-02-13 23:44:08.000000 meta-edc-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)      463 2022-08-23 13:24:02.000000 meta-edc-0.3.8/releases
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.177133 meta-edc-0.3.8/reports/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-06-18 19:11:34.000000 meta-edc-0.3.8/reports/20200603.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1006 2024-03-27 20:33:11.000000 meta-edc-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1183 2024-03-27 20:33:21.180128 meta-edc-0.3.8/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.177339 meta-edc-0.3.8/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:21.179062 meta-edc-0.3.8/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)     5307 2022-08-22 17:23:22.000000 meta-edc-0.3.8/tests/etc/randomization_list.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.8/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.901166 meta-edc-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       75 2022-04-11 18:27:09.000000 meta-edc-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)     4225 2024-02-13 23:41:07.000000 meta-edc-0.3.9/.env-tests
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.655761 meta-edc-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.676183 meta-edc-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2092 2024-02-13 23:44:08.000000 meta-edc-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1486 2024-02-13 23:41:07.000000 meta-edc-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1227 2024-02-15 06:32:55.000000 meta-edc-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-22 17:23:22.000000 meta-edc-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    13162 2024-03-27 20:33:11.000000 meta-edc-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 23:21:43.000000 meta-edc-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      199 2024-02-13 23:44:08.000000 meta-edc-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2687 2024-03-31 02:04:37.901093 meta-edc-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1798 2024-02-15 06:32:55.000000 meta-edc-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      893 2022-04-11 18:27:09.000000 meta-edc-0.3.9/TODO.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.660696 meta-edc-0.3.9/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.657063 meta-edc-0.3.9/bin/nginx/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.656063 meta-edc-0.3.9/bin/nginx/meta2/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.677086 meta-edc-0.3.9/bin/nginx/meta2/conf/
+-rw-r--r--   0 erikvw     (501) staff       (20)      636 2021-08-09 19:25:30.000000 meta-edc-0.3.9/bin/nginx/meta2/conf/live.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      423 2021-08-09 19:25:30.000000 meta-edc-0.3.9/bin/nginx/meta2/conf/live_sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      281 2021-08-09 19:25:30.000000 meta-edc-0.3.9/bin/nginx/meta2/conf/meta.clinicedc.org.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      651 2021-08-09 19:25:30.000000 meta-edc-0.3.9/bin/nginx/meta2/conf/uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      426 2021-08-09 19:25:30.000000 meta-edc-0.3.9/bin/nginx/meta2/conf/uat_sites.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.656123 meta-edc-0.3.9/bin/nginx/meta2/www/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.677234 meta-edc-0.3.9/bin/nginx/meta2/www/html/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1439 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta2/www/html/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.677429 meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1432 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.677624 meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1636 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.677786 meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/ug/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1236 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/ug/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.656512 meta-edc-0.3.9/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.677942 meta-edc-0.3.9/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1863 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.678135 meta-edc-0.3.9/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/ug/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1237 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/ug/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.656690 meta-edc-0.3.9/bin/nginx/meta3/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.678876 meta-edc-0.3.9/bin/nginx/meta3/conf/
+-rw-r--r--   0 erikvw     (501) staff       (20)      705 2021-08-09 19:25:29.000000 meta-edc-0.3.9/bin/nginx/meta3/conf/live.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      430 2021-08-09 19:25:29.000000 meta-edc-0.3.9/bin/nginx/meta3/conf/live_sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2021-08-09 19:25:29.000000 meta-edc-0.3.9/bin/nginx/meta3/conf/meta.clinicedc.org.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      728 2021-08-09 19:25:29.000000 meta-edc-0.3.9/bin/nginx/meta3/conf/uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      428 2021-08-09 19:25:29.000000 meta-edc-0.3.9/bin/nginx/meta3/conf/uat_sites.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.656737 meta-edc-0.3.9/bin/nginx/meta3/www/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.679021 meta-edc-0.3.9/bin/nginx/meta3/www/html/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1257 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta3/www/html/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.679166 meta-edc-0.3.9/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1257 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.679304 meta-edc-0.3.9/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1845 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.656992 meta-edc-0.3.9/bin/nginx/meta3/www/html/uat.meta3.clinicedc.org/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.679447 meta-edc-0.3.9/bin/nginx/meta3/www/html/uat.meta3.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1867 2021-08-09 19:25:29.000000 meta-edc-0.3.9/bin/nginx/meta3/www/html/uat.meta3.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.657192 meta-edc-0.3.9/bin/nginx/meta4/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.681662 meta-edc-0.3.9/bin/nginx/meta4/conf/
+-rw-r--r--   0 erikvw     (501) staff       (20)      705 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/conf/live.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      430 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/conf/live_sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/conf/meta.clinicedc.org.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      728 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/conf/uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      428 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/conf/uat_sites.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.660175 meta-edc-0.3.9/bin/nginx/meta4/www/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.681863 meta-edc-0.3.9/bin/nginx/meta4/www/html/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1257 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/www/html/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.682027 meta-edc-0.3.9/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1257 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.682202 meta-edc-0.3.9/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1845 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.660529 meta-edc-0.3.9/bin/nginx/meta4/www/html/uat.meta3.clinicedc.org/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.682374 meta-edc-0.3.9/bin/nginx/meta4/www/html/uat.meta3.clinicedc.org/tz/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1867 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/nginx/meta4/www/html/uat.meta3.clinicedc.org/tz/index.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.682860 meta-edc-0.3.9/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-04 23:21:43.000000 meta-edc-0.3.9/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-04 23:21:43.000000 meta-edc-0.3.9/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-08-22 17:23:22.000000 meta-edc-0.3.9/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.683643 meta-edc-0.3.9/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-04 23:21:43.000000 meta-edc-0.3.9/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-04 23:21:43.000000 meta-edc-0.3.9/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-04 23:21:43.000000 meta-edc-0.3.9/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-04 23:21:43.000000 meta-edc-0.3.9/bin/systemd/celerybeat.service
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.684280 meta-edc-0.3.9/bin/systemd/meta3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      425 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/systemd/meta3/gunicorn-live.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2021-08-09 19:25:30.000000 meta-edc-0.3.9/bin/systemd/meta3/gunicorn-live.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      418 2024-03-12 03:29:53.000000 meta-edc-0.3.9/bin/systemd/meta3/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2021-08-09 19:25:30.000000 meta-edc-0.3.9/bin/systemd/meta3/gunicorn-uat.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.684691 meta-edc-0.3.9/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      375 2020-03-04 23:21:43.000000 meta-edc-0.3.9/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   754498 2024-02-13 23:41:07.000000 meta-edc-0.3.9/docs/forms_reference.md
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.686033 meta-edc-0.3.9/docs/images/
+-rw-r--r--   0 erikvw     (501) staff       (20)    86202 2020-03-04 23:21:43.000000 meta-edc-0.3.9/docs/images/user_groups.png
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.686636 meta-edc-0.3.9/docs/updates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.687062 meta-edc-0.3.9/docs/updates/0.1.65/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38460 2021-07-06 02:07:00.000000 meta-edc-0.3.9/docs/updates/0.1.65/renamed_fields.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)    29315 2021-07-05 21:18:11.000000 meta-edc-0.3.9/docs/updates/0.1.65/update_1_65_renamed_fields.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      289 2022-04-11 18:27:09.000000 meta-edc-0.3.9/docs/updates/pharmacy.sql
+-rw-r--r--   0 erikvw     (501) staff       (20)     4680 2022-08-22 17:23:22.000000 meta-edc-0.3.9/env.sample
+-rw-r--r--   0 erikvw     (501) staff       (20)     1019 2020-04-03 04:33:09.000000 meta-edc-0.3.9/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.661336 meta-edc-0.3.9/label_templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.687891 meta-edc-0.3.9/label_templates/2.25x1.25in/
+-rw-r--r--   0 erikvw     (501) staff       (20)      588 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2.25x1.25in/aliquot.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      341 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2.25x1.25in/box.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      337 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2.25x1.25in/manifest.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      520 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2.25x1.25in/requisition.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      299 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2.25x1.25in/subject.lbl
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.688518 meta-edc-0.3.9/label_templates/2x1cm/
+-rw-r--r--   0 erikvw     (501) staff       (20)      412 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2x1cm/aliquot.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      297 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2x1cm/box.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2x1cm/manifest.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      387 2020-03-04 23:21:43.000000 meta-edc-0.3.9/label_templates/2x1cm/requisition.lbl
+-rwxr-xr-x   0 erikvw     (501) staff       (20)      634 2020-04-03 04:33:09.000000 meta-edc-0.3.9/manage.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.690574 meta-edc-0.3.9/meta_ae/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_ae/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11256 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.692912 meta-edc-0.3.9/meta_ae/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      400 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      484 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/ae_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      834 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/ae_initial_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      478 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/ae_local_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      488 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/ae_sponsor_review_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      463 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/ae_susar_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      449 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/ae_tmg_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2251 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/death_report_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      518 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/death_report_tmg_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      548 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/admin/death_report_tmg_second_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      525 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/admin/hospitalization_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4156 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      159 2021-07-02 03:53:00.000000 meta-edc-0.3.9/meta_ae/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-08-23 13:24:02.000000 meta-edc-0.3.9/meta_ae/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1184 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_ae/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       36 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_ae/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.695412 meta-edc-0.3.9/meta_ae/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      492 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/forms/ae_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      292 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/forms/ae_initial_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-07-19 13:21:21.000000 meta-edc-0.3.9/meta_ae/forms/ae_local_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-07-19 13:21:21.000000 meta-edc-0.3.9/meta_ae/forms/ae_sponsor_review_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      280 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/forms/ae_susar_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      268 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/forms/ae_tmg_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1424 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/forms/death_report_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      322 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/forms/death_report_tmg_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      340 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/forms/death_report_tmg_second_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      365 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/forms/hospitalization_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      874 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/forms/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1416 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.701385 meta-edc-0.3.9/meta_ae/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   140317 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2699 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0002_auto_20191024_1000.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2444 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0003_auto_20191102_0033.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      997 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0004_auto_20191114_0821.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18484 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0005_auto_20210624_0225.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    16966 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0006_aelocalreview_aesponsorreview.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2708 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0007_auto_20210911_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1240 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0008_auto_20211011_1657.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1151 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0009_auto_20220307_1929.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4214 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0010_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2827 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0011_alter_aefollowup_action_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2996 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0012_auto_20220826_0258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2841 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0013_auto_20220826_0322.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1857 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0014_auto_20220826_0406.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1238 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0015_auto_20220907_0157.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5278 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0016_rename_narrative_aetmg_investigator_narrative_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1013 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/migrations/0017_auto_20221130_2257.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1623 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/migrations/0018_alter_deathreporttmg_cause_of_death_agreed_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20955 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/migrations/0019_alter_aefollowup_managers_alter_aeinitial_managers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17482 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/migrations/0020_alter_aesusar_options_alter_aetmg_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4935 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/migrations/0021_alter_aefollowup_site_alter_aeinitial_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    24521 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/migrations/0022_historicalhospitalization_hospitalization.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_ae/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.701980 meta-edc-0.3.9/meta_ae/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2020-05-15 02:40:42.000000 meta-edc-0.3.9/meta_ae/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2666 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/model_mixins/ae_review_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1798 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/model_mixins/death_report_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.704403 meta-edc-0.3.9/meta_ae/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      402 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_ae/models/ae_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      422 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/models/ae_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_ae/models/ae_local_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      240 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_ae/models/ae_sponsor_review.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      208 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_ae/models/ae_susar.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      226 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_ae/models/ae_tmg.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/models/death_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2021-07-05 19:24:26.000000 meta-edc-0.3.9/meta_ae/models/death_report_tmg.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      564 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/models/death_report_tmg_second.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      802 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/models/hospitalization.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      620 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/models/managers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.705268 meta-edc-0.3.9/meta_ae/pdf_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)       84 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/pdf_reports/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      195 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/pdf_reports/ae_pdf_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      207 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/pdf_reports/death_pdf_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      585 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_ae/pdf_reports/meta_pdf_report_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.661986 meta-edc-0.3.9/meta_ae/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.662041 meta-edc-0.3.9/meta_ae/templates/meta_ae/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.705636 meta-edc-0.3.9/meta_ae/templates/meta_ae/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      885 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_ae/templates/meta_ae/bootstrap3/ae_initial_description.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.706000 meta-edc-0.3.9/meta_ae/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_ae/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1215 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_ae/templatetags/meta_ae_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.706455 meta-edc-0.3.9/meta_ae/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_ae/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_ae/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.706695 meta-edc-0.3.9/meta_ae/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_ae/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4915 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_ae/tests/tests/test_actions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      260 2021-07-05 19:24:26.000000 meta-edc-0.3.9/meta_ae/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      197 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_ae/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.709353 meta-edc-0.3.9/meta_auth/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_auth/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-06-24 09:16:28.000000 meta-edc-0.3.9/meta_auth/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1729 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_auth/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2426 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_auth/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-24 09:16:34.000000 meta-edc-0.3.9/meta_auth/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.712875 meta-edc-0.3.9/meta_consent/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_consent/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-06-24 09:14:24.000000 meta-edc-0.3.9/meta_consent/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.713821 meta-edc-0.3.9/meta_consent/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      115 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/admin/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.714355 meta-edc-0.3.9/meta_consent/admin/actions/
+-rw-r--r--   0 erikvw     (501) staff       (20)       70 2022-07-08 07:31:04.000000 meta-edc-0.3.9/meta_consent/admin/actions/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1474 2022-07-08 07:31:04.000000 meta-edc-0.3.9/meta_consent/admin/actions/create_missing_prescriptions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5362 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/admin/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      647 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/admin/subject_consent_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      657 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/admin/subject_consent_v1_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-06-24 09:14:27.000000 meta-edc-0.3.9/meta_consent/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      282 2022-08-23 13:24:02.000000 meta-edc-0.3.9/meta_consent/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1343 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_consent/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      552 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_consent/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       31 2022-06-24 09:14:43.000000 meta-edc-0.3.9/meta_consent/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.714696 meta-edc-0.3.9/meta_consent/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)       72 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1258 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/form_validators/subject_consent_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.715368 meta-edc-0.3.9/meta_consent/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1293 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/forms/subject_consent_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/forms/subject_consent_v1_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1306 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/forms/subject_reconsent_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.662893 meta-edc-0.3.9/meta_consent/locale/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.662953 meta-edc-0.3.9/meta_consent/locale/sw/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.715626 meta-edc-0.3.9/meta_consent/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1845 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_consent/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.715858 meta-edc-0.3.9/meta_consent/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_consent/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.716047 meta-edc-0.3.9/meta_consent/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_consent/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1438 2022-07-08 07:31:04.000000 meta-edc-0.3.9/meta_consent/management/commands/create_missing_prescriptions.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.722161 meta-edc-0.3.9/meta_consent/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    66732 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      590 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0002_auto_20191024_1000.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1610 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0003_auto_20200325_0901.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3509 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0004_auto_20210624_0225.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      790 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0005_alter_subjectconsent_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      637 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0006_auto_20210911_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3051 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0007_auto_20220128_1719.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      942 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0008_auto_20220412_2151.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1390 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0009_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      647 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0010_alter_historicalsubjectreconsent_action_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      711 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0011_auto_20220826_0258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      650 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0012_auto_20220826_0322.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      492 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0013_auto_20220826_0406.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      604 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/migrations/0014_alter_subjectconsent_managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      755 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0015_auto_20220914_0542.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      946 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_consent/migrations/0016_auto_20220914_0547.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      923 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/migrations/0017_auto_20220929_1742.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6458 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_consent/migrations/0018_alter_subjectconsent_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6441 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_consent/migrations/0019_alter_subjectconsent_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1110 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_consent/migrations/0020_historicalsubjectconsent_model_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      498 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_consent/migrations/0021_auto_20240111_0442.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1025 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_consent/migrations/0022_alter_historicalsubjectconsent_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2978 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/migrations/0023_subjectconsentv1_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    25696 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/migrations/0024_historicalsubjectconsentv1.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6307 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_consent/migrations/0025_alter_historicalsubjectconsent_first_name_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_consent/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.723349 meta-edc-0.3.9/meta_consent/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      223 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-06-24 09:13:53.000000 meta-edc-0.3.9/meta_consent/models/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4557 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_consent/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3803 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/models/subject_consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      458 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_consent/models/subject_consent_v1.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3595 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_consent/models/subject_reconsent.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.723865 meta-edc-0.3.9/meta_consent/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_consent/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_consent/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.724417 meta-edc-0.3.9/meta_consent/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_consent/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4651 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_consent/tests/tests/test_form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      376 2022-06-24 09:14:16.000000 meta-edc-0.3.9/meta_consent/tests/tests/test_subject_consent.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      857 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_consent/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-06-24 09:14:40.000000 meta-edc-0.3.9/meta_consent/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.725217 meta-edc-0.3.9/meta_dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      313 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.663611 meta-edc-0.3.9/meta_dashboard/locale/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.663668 meta-edc-0.3.9/meta_dashboard/locale/sw/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.725478 meta-edc-0.3.9/meta_dashboard/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 erikvw     (501) staff       (20)      698 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_dashboard/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.725667 meta-edc-0.3.9/meta_dashboard/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1168 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       47 2022-06-24 09:14:59.000000 meta-edc-0.3.9/meta_dashboard/patterns.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.663875 meta-edc-0.3.9/meta_dashboard/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.663949 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.664161 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.726798 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/
+-rw-r--r--   0 erikvw     (501) staff       (20)      447 2022-08-22 17:23:22.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/add_consent_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      280 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/dashboard_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      401 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/eligibility_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      429 2022-08-22 17:23:22.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/refusal_button.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1079 2022-08-22 17:23:22.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/screening_button.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.727002 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2671 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/screening/listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.727343 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.727486 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)      230 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/dashboard/top_bar.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      273 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/dashboard.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1403 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.727772 meta-edc-0.3.9/meta_dashboard/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3947 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/templatetags/meta_dashboard_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.728385 meta-edc-0.3.9/meta_dashboard/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      716 2021-07-05 19:24:26.000000 meta-edc-0.3.9/meta_dashboard/tests/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.728635 meta-edc-0.3.9/meta_dashboard/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2751 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_dashboard/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1193 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.728858 meta-edc-0.3.9/meta_dashboard/view_utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/view_utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3370 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/view_utils/subject_screening_button.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.729117 meta-edc-0.3.9/meta_dashboard/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-08-26 02:59:33.000000 meta-edc-0.3.9/meta_dashboard/views/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.729723 meta-edc-0.3.9/meta_dashboard/views/ae/
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/views/ae/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      452 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_dashboard/views/ae/ae_listboard_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      494 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_dashboard/views/ae/death_report_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.730063 meta-edc-0.3.9/meta_dashboard/views/screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/views/screening/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      578 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_dashboard/views/screening/listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.730318 meta-edc-0.3.9/meta_dashboard/views/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-08-26 02:59:33.000000 meta-edc-0.3.9/meta_dashboard/views/subject/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.730736 meta-edc-0.3.9/meta_dashboard/views/subject/dashboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_dashboard/views/subject/dashboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      344 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_dashboard/views/subject/dashboard/dashboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.732575 meta-edc-0.3.9/meta_dashboard/views/subject/listboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)       49 2022-08-26 02:59:33.000000 meta-edc-0.3.9/meta_dashboard/views/subject/listboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      601 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_dashboard/views/subject/listboard/listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.733503 meta-edc-0.3.9/meta_data_manager/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_data_manager/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      233 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_data_manager/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_data_manager/data_manager.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      952 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_data_manager/handlers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.736596 meta-edc-0.3.9/meta_edc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      186 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_edc/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2022-08-22 17:23:22.000000 meta-edc-0.3.9/meta_edc/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-06-24 09:07:19.000000 meta-edc-0.3.9/meta_edc/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      175 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_edc/asgi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      785 2020-03-04 23:21:43.000000 meta-edc-0.3.9/meta_edc/celery.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.737775 meta-edc-0.3.9/meta_edc/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_edc/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.737993 meta-edc-0.3.9/meta_edc/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_edc/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1003 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_edc/management/commands/update_forms_reference.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      211 2022-06-24 09:07:24.000000 meta-edc-0.3.9/meta_edc/meta_version.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1339 2022-07-19 13:21:21.000000 meta-edc-0.3.9/meta_edc/model_callers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-04 23:21:43.000000 meta-edc-0.3.9/meta_edc/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1100 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_edc/navbars.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.739630 meta-edc-0.3.9/meta_edc/settings/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-03 04:33:09.000000 meta-edc-0.3.9/meta_edc/settings/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      911 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_edc/settings/debug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    19233 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_edc/settings/defaults.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      216 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_edc/settings/live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1938 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_edc/settings/logging.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      592 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_edc/settings/minimal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      355 2024-03-31 02:03:21.000000 meta-edc-0.3.9/meta_edc/settings/uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.665437 meta-edc-0.3.9/meta_edc/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.665493 meta-edc-0.3.9/meta_edc/templates/meta_edc/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.740173 meta-edc-0.3.9/meta_edc/templates/meta_edc/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/templates/meta_edc/bootstrap3/base.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     3780 2022-08-26 02:59:33.000000 meta-edc-0.3.9/meta_edc/templates/meta_edc/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.740559 meta-edc-0.3.9/meta_edc/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:21:43.000000 meta-edc-0.3.9/meta_edc/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.742514 meta-edc-0.3.9/meta_edc/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5797 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/randomization_list_phase_three.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     6935 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_edc/tests/test_settings.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.742836 meta-edc-0.3.9/meta_edc/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_edc/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    23452 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_edc/tests/tests/test_endpoints.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3435 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_edc/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      342 2022-06-24 09:07:39.000000 meta-edc-0.3.9/meta_edc/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.743260 meta-edc-0.3.9/meta_edc/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)       32 2020-03-04 23:21:43.000000 meta-edc-0.3.9/meta_edc/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1006 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_edc/views/home_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      175 2020-04-03 04:33:09.000000 meta-edc-0.3.9/meta_edc/wsgi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      174 2020-04-03 04:33:09.000000 meta-edc-0.3.9/meta_edc/wsgi_live.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2020-04-03 04:33:09.000000 meta-edc-0.3.9/meta_edc/wsgi_uat.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.900609 meta-edc-0.3.9/meta_edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2687 2024-03-31 02:04:37.000000 meta-edc-0.3.9/meta_edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    46153 2024-03-31 02:04:37.000000 meta-edc-0.3.9/meta_edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-03-31 02:04:37.000000 meta-edc-0.3.9/meta_edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:21:43.000000 meta-edc-0.3.9/meta_edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       42 2024-03-31 02:04:37.000000 meta-edc-0.3.9/meta_edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      229 2024-03-31 02:04:37.000000 meta-edc-0.3.9/meta_edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.744079 meta-edc-0.3.9/meta_export/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_export/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2021-07-02 03:53:00.000000 meta-edc-0.3.9/meta_export/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      226 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_export/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      205 2022-06-24 09:12:54.000000 meta-edc-0.3.9/meta_export/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.745618 meta-edc-0.3.9/meta_labs/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-02 03:53:00.000000 meta-edc-0.3.9/meta_labs/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       87 2021-07-05 19:24:26.000000 meta-edc-0.3.9/meta_labs/aliquot_types.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      200 2022-08-23 13:24:02.000000 meta-edc-0.3.9/meta_labs/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      957 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_labs/lab_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      128 2022-06-24 09:12:03.000000 meta-edc-0.3.9/meta_labs/labs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      477 2022-06-24 09:12:00.000000 meta-edc-0.3.9/meta_labs/list_data.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      500 2022-06-24 09:11:58.000000 meta-edc-0.3.9/meta_labs/processing_profiles.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      512 2022-07-19 19:44:25.000000 meta-edc-0.3.9/meta_labs/reportables.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.746510 meta-edc-0.3.9/meta_labs/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_labs/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      967 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_labs/tests/test_labs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      516 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_labs/tests/test_reportables.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_labs/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.747933 meta-edc-0.3.9/meta_lists/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_lists/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2157 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_lists/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-06-24 09:11:34.000000 meta-edc-0.3.9/meta_lists/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      278 2022-08-23 13:24:02.000000 meta-edc-0.3.9/meta_lists/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9702 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_lists/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.752287 meta-edc-0.3.9/meta_lists/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    13881 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4608 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0002_auto_20191026_2231.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2555 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0003_auto_20191102_0033.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2547 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0004_auto_20191102_1859.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2583 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0005_auto_20191104_0930.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4478 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0006_auto_20200514_1959.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2961 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0007_auto_20200516_2356.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      709 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_lists/migrations/0008_auto_20200528_1517.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      357 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0009_auto_20200613_2041.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1194 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0010_auto_20200617_1738.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1848 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0011_auto_20210624_0225.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2811 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0012_auto_20210728_1809.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2533 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0013_transferreasons_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2527 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_lists/migrations/0014_auto_20220913_2139.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2212 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_lists/migrations/0015_abnormalfootappearanceobservations_extra_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20692 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_lists/migrations/0016_alter_abnormalfootappearanceobservations_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13041 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_lists/migrations/0017_complications_dmmedications_dmtreatments_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2639 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_lists/migrations/0018_missedreferralreasons.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_lists/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3032 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_lists/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.752481 meta-edc-0.3.9/meta_lists/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_lists/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      212 2022-06-24 09:11:29.000000 meta-edc-0.3.9/meta_lists/tests/test_lists.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      204 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_lists/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.753431 meta-edc-0.3.9/meta_pharmacy/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_pharmacy/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      599 2022-08-23 13:24:02.000000 meta-edc-0.3.9/meta_pharmacy/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       24 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_pharmacy/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.753815 meta-edc-0.3.9/meta_pharmacy/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1115 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_pharmacy/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_pharmacy/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_pharmacy/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2945 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_pharmacy/prepare_meta_pharmacy.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.755724 meta-edc-0.3.9/meta_prn/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_prn/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7485 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.757751 meta-edc-0.3.9/meta_prn/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      581 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5121 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/end_of_study_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1736 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/loss_to_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2377 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/off_study_medication_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1707 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/offschedule_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1621 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/offschedule_postnatal_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1703 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/offschedule_pregnancy_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1440 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/onschedule_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2144 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/pregnancy_notification_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      739 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/protocol_incident_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      723 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/admin/subject_transfer_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-06-24 09:09:37.000000 meta-edc-0.3.9/meta_prn/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      280 2022-08-23 13:24:02.000000 meta-edc-0.3.9/meta_prn/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      517 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_prn/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3153 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_prn/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      840 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.758302 meta-edc-0.3.9/meta_prn/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_prn/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11246 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/form_validators/end_of_study.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1068 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/form_validators/protocol_incident.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.759645 meta-edc-0.3.9/meta_prn/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      452 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      926 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/forms/end_of_study_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1333 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/forms/loss_to_followup_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2295 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/forms/off_study_medication_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      939 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/forms/offschedule_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1101 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/forms/offschedule_pregnancy_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4897 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/forms/pregnancy_notification_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      231 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/forms/protocol_incident_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      817 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/forms/subject_transfer_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2336 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.772496 meta-edc-0.3.9/meta_prn/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   108119 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2331 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0002_auto_20191024_1000.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      881 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0003_auto_20200120_2020.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      755 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0004_auto_20200403_0332.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4269 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0005_auto_20200524_1944.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13108 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0006_auto_20210624_0225.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      879 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0007_auto_20210721_0335.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3639 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0008_auto_20210910_0238.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2872 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0009_auto_20210910_0239.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2791 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0010_auto_20210910_1906.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      934 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/migrations/0011_auto_20210910_1911.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      796 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_prn/migrations/0012_auto_20210911_0004.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3117 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0013_auto_20210911_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0014_auto_20211003_1709.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5914 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0015_auto_20211104_1447.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5843 2024-03-07 19:17:25.000000 meta-edc-0.3.9/meta_prn/migrations/0016_auto_20220128_1719.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26858 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0017_auto_20220307_1929.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    34941 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0018_auto_20220309_2106.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1165 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0019_auto_20220309_2230.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2041 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0020_auto_20220310_0439.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    43328 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0021_auto_20220316_2147.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    27548 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0022_auto_20220318_0133.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2418 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0023_auto_20220415_1747.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      792 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0024_alter_protocoldeviationviolation_violation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6264 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0025_alter_historicalprotocoldeviationviolation_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3925 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0026_remove_historicalprotocoldeviationviolation_violation_type_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1284 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0027_rename_historicalprotocoldeviationviolation_historicalprotocolincident_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1919 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0028_historicalpregnancynotification_bhcg_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      661 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0029_alter_historicalpregnancynotification_edd_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1254 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0030_auto_20220627_1119.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1840 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0031_alter_historicaloffschedule_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17575 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0032_historicalegfrnotification_egfrnotification.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1069 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0033_remove_historicalegfrnotification_action_item_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2075 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0034_auto_20220630_1110.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3456 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0035_auto_20220630_1140.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1391 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0036_remove_endofstudy_meta_prn_en_id_a50384_idx_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7338 2024-03-07 19:17:25.000000 meta-edc-0.3.9/meta_prn/migrations/0037_endofstudy_delivery_date_endofstudy_pregnancy_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    21785 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0038_alter_endofstudy_delivery_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1011 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0039_historicaloffstudymedication_reason_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4593 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0040_remove_historicaloffstudymedication_expected_restart_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26299 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0041_endofstudy_transfer_date_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6198 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0042_remove_endofstudy_investigator_decision_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7239 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0043_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3925 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0044_alter_endofstudy_action_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4149 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0045_auto_20220826_0258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3944 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0046_auto_20220826_0322.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2586 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0047_auto_20220826_0406.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2496 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0048_auto_20220922_2236.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3936 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0049_auto_20220929_1742.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1250 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0050_auto_20221004_0629.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1863 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0051_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      642 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/migrations/0052_alter_historicalprotocolincident_reasons_withdrawn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    38131 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/migrations/0053_alter_losstofollowup_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    27710 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/migrations/0054_alter_losstofollowup_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8878 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/migrations/0055_alter_endofstudy_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4089 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_prn/migrations/0056_alter_endofstudy_clinical_withdrawal_reason_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_prn/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.774229 meta-edc-0.3.9/meta_prn/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      594 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5316 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/models/end_of_study.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2436 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/models/loss_to_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1701 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/models/off_study_medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1336 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/models/offschedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      677 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/models/onschedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3129 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/models/pregnancy_notification.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1089 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/models/protocol_incident.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2443 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      266 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/models/subject_transfer.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1018 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/pregnancy_action_item_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.774637 meta-edc-0.3.9/meta_prn/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_prn/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.775502 meta-edc-0.3.9/meta_prn/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_prn/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3811 2024-02-20 05:50:29.000000 meta-edc-0.3.9/meta_prn/tests/tests/test_actions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      548 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_prn/tests/tests/test_manager_order.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3982 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_prn/tests/tests/test_pregnancy_notification.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      270 2022-06-24 09:09:29.000000 meta-edc-0.3.9/meta_prn/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      202 2022-06-24 09:09:57.000000 meta-edc-0.3.9/meta_prn/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.776487 meta-edc-0.3.9/meta_rando/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_rando/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-23 13:24:02.000000 meta-edc-0.3.9/meta_rando/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.778094 meta-edc-0.3.9/meta_rando/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    13432 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_rando/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_rando/migrations/0002_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1225 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_rando/migrations/0003_auto_20220826_1640.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3572 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_rando/migrations/0004_alter_randomizationlist_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3248 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_rando/migrations/0005_alter_randomizationlist_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_rando/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      532 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_rando/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1591 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_rando/randomizers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.778223 meta-edc-0.3.9/meta_rando/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_rando/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.778478 meta-edc-0.3.9/meta_rando/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-0.3.9/meta_rando/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2278 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_rando/tests/tests/test_randomizers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.779475 meta-edc-0.3.9/meta_reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_reports/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_reports/ae_report.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      733 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_reports/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4713 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_reports/death_report.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.779631 meta-edc-0.3.9/meta_reports/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_reports/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_reports/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2395 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_reports/pdf_report.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.780263 meta-edc-0.3.9/meta_reports/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_reports/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_reports/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     1293 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_reports/tests/test_reports.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_reports/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.783670 meta-edc-0.3.9/meta_screening/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_screening/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.785531 meta-edc-0.3.9/meta_screening/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_screening/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5076 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/admin/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2534 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1067 2024-02-20 05:46:58.000000 meta-edc-0.3.9/meta_screening/admin/screening_part_one_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2592 2024-02-20 05:47:03.000000 meta-edc-0.3.9/meta_screening/admin/screening_part_three_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1278 2024-02-20 05:50:29.000000 meta-edc-0.3.9/meta_screening/admin/screening_part_two_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2244 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_screening/admin/subject_refusal_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6925 2024-02-20 05:50:29.000000 meta-edc-0.3.9/meta_screening/admin/subject_screening_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-10-18 02:37:22.000000 meta-edc-0.3.9/meta_screening/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      543 2022-08-23 13:24:02.000000 meta-edc-0.3.9/meta_screening/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1705 2022-06-24 09:06:35.000000 meta-edc-0.3.9/meta_screening/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1948 2022-06-24 09:06:38.000000 meta-edc-0.3.9/meta_screening/calculators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      789 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_screening/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      655 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_screening/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.786476 meta-edc-0.3.9/meta_screening/eligibility/
+-rw-r--r--   0 erikvw     (501) staff       (20)      284 2022-08-22 17:23:22.000000 meta-edc-0.3.9/meta_screening/eligibility/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7732 2022-07-08 07:31:04.000000 meta-edc-0.3.9/meta_screening/eligibility/eligibility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1769 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_one.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.787197 meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_three/
+-rw-r--r--   0 erikvw     (501) staff       (20)       79 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_three/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5405 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_three/base_eligibility_part_three.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4296 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_three/eligibility_part_three_phase_three.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1808 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_two.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.788640 meta-edc-0.3.9/meta_screening/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      308 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_screening/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1213 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_screening/form_validators/screening_part_one.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7606 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/form_validators/screening_part_three.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4738 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_screening/form_validators/screening_part_two.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      322 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/form_validators/subject_refusal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      309 2022-06-24 09:04:37.000000 meta-edc-0.3.9/meta_screening/form_validators/subject_screening.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.790233 meta-edc-0.3.9/meta_screening/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      614 2022-07-19 13:21:21.000000 meta-edc-0.3.9/meta_screening/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3291 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/forms/field_lists.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      798 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_screening/forms/screening_part_one_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      987 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/forms/screening_part_three_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      701 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/forms/screening_part_two_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      624 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/forms/subject_refusal_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      643 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_screening/forms/subject_screening_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.804421 meta-edc-0.3.9/meta_screening/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   186855 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4467 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0002_auto_20191020_0612.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5513 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0003_auto_20191020_0627.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14316 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0004_auto_20191020_0738.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10372 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0005_auto_20191021_0353.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6710 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0006_auto_20191022_0134.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      950 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0007_auto_20191024_1000.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6148 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0008_auto_20191031_0745.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6108 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0009_auto_20191105_0122.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    36963 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0010_auto_20191106_0828.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7246 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_screening/migrations/0011_auto_20191107_0342.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      797 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_screening/migrations/0012_auto_20191107_0427.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7882 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0013_auto_20191107_0442.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17407 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0014_auto_20191107_0528.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1186 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0015_auto_20191107_2249.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4803 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0016_auto_20191119_2331.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2821 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0017_auto_20191213_0314.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5089 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0018_auto_20200118_1854.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4108 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0019_auto_20200120_2256.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8402 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0020_auto_20200524_1944.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    25508 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0021_auto_20210628_2105.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2291 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0022_auto_20210702_0426.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2892 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0023_auto_20210702_0533.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4283 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0024_auto_20210710_1929.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4815 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0025_auto_20210710_2247.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2421 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0026_auto_20210712_0433.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      226 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0027_auto_20210804_0438.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14429 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0028_auto_20210823_2353.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    25296 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0029_auto_20211123_1645.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1611 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0030_auto_20220128_1719.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10215 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0031_auto_20220304_0448.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5506 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0032_auto_20220304_0501.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2167 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0033_auto_20220304_0504.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6546 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0034_auto_20220304_0508.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    36492 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0035_auto_20220304_2233.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5609 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0036_auto_20220304_2307.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5029 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0037_auto_20220312_0339.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10872 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0038_auto_20220312_1929.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6642 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0039_auto_20220312_1938.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20940 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0040_auto_20220316_2147.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2662 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0041_auto_20220403_1227.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15665 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0042_auto_20220403_1402.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5504 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0043_auto_20220407_1713.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4908 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0044_alter_historicalscreeningpartone_severe_htn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1918 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0045_historicalscreeningpartone_contact_number_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1983 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0046_historicalscreeningpartone_hba1c_datetime_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2353 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0047_historicalscreeningpartone_appt_datetime_repeat_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1191 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0048_rename_appt_datetime_repeat_historicalscreeningpartone_repeat_appt_datetime_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9619 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0049_historicalscreeningpartone_p3_ltfu_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11994 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0050_historicalscreeningpartone_agree_to_p3_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11971 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0051_alter_historicalscreeningpartone_advised_to_fast_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3890 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0052_alter_historicalscreeningpartone_p3_ltfu_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3781 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0053_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6028 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0054_auto_20220722_2130.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18773 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0055_alter_historicalscreeningpartone_creatinine_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4224 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0056_alter_historicalscreeningpartone_agree_to_p3_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13643 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0057_alter_historicalscreeningpartone_calculated_egfr_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7511 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/migrations/0058_alter_historicalscreeningpartone_eligibility_datetime_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12718 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_screening/migrations/0059_alter_icpreferral_managers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6812 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_screening/migrations/0060_historicalicpreferral_locale_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4465 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_screening/migrations/0061_alter_historicalicpreferral_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      641 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_screening/migrations/0062_remove_icpreferral_site_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_screening/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.805580 meta-edc-0.3.9/meta_screening/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      315 2022-08-26 02:59:33.000000 meta-edc-0.3.9/meta_screening/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2761 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/model_mixins/calculated_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      592 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/model_mixins/creatinine_fields_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1360 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/model_mixins/eligibility_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3708 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/model_mixins/part_one_fields_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4974 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_screening/model_mixins/part_three_fields_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6692 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/model_mixins/part_two_fields_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.806800 meta-edc-0.3.9/meta_screening/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      262 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_screening/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3465 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_screening/models/icp_referral.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1175 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_screening/models/proxy_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      862 2022-08-26 02:59:33.000000 meta-edc-0.3.9/meta_screening/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2253 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_screening/models/subject_refusal.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2269 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_screening/models/subject_screening.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      131 2022-06-24 09:06:52.000000 meta-edc-0.3.9/meta_screening/offline_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.807638 meta-edc-0.3.9/meta_screening/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_screening/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_screening/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     8264 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_screening/tests/meta_test_case_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4097 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_screening/tests/options.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.808760 meta-edc-0.3.9/meta_screening/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-0.3.9/meta_screening/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    16710 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/tests/tests/test_forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4723 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_screening/tests/tests/test_screening_part_one.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    16774 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/tests/tests/test_screening_part_three.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3126 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_screening/tests/tests/test_screening_part_two.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      208 2022-06-24 09:06:56.000000 meta-edc-0.3.9/meta_screening/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.809717 meta-edc-0.3.9/meta_sites/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_sites/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      278 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_sites/apps.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.809987 meta-edc-0.3.9/meta_sites/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-06-18 19:11:34.000000 meta-edc-0.3.9/meta_sites/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_sites/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1625 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_sites/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.810463 meta-edc-0.3.9/meta_sites/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_sites/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      415 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_sites/tests/test_sites.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-24 09:03:07.000000 meta-edc-0.3.9/meta_sites/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.811035 meta-edc-0.3.9/meta_stats/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_stats/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      540 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_stats/incidence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_stats/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.811139 meta-edc-0.3.9/meta_stats/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_stats/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.811337 meta-edc-0.3.9/meta_stats/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_stats/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      313 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_stats/tests/tests/test_incidence.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.813679 meta-edc-0.3.9/meta_subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5930 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.820728 meta-edc-0.3.9/meta_subject/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1714 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1158 2022-06-24 08:59:56.000000 meta-edc-0.3.9/meta_subject/admin/autocomplete_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3189 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/birth_outcome_admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.821883 meta-edc-0.3.9/meta_subject/admin/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      356 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/admin/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      799 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_fbc_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      861 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_hba1c_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      822 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_ins_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      822 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_lft_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      836 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_lipid_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5120 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_rft_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1017 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/complications_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4069 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/complications_glycemia_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      824 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/concomitant_medication_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3426 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/admin/delivery_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2774 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/admin/dm_referral_followup_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      627 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/egfr_drop_notification_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      772 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/eq5d3l_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      277 2022-06-24 09:00:25.000000 meta-edc-0.3.9/meta_subject/admin/fields.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1523 2022-06-24 09:00:28.000000 meta-edc-0.3.9/meta_subject/admin/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5153 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/admin/followup_examination_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1585 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/admin/followup_vitals_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2971 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/admin/glucose_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1716 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/admin/glucose_fbg_admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.822646 meta-edc-0.3.9/meta_subject/admin/health_economics/
+-rw-r--r--   0 erikvw     (501) staff       (20)      140 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/admin/health_economics/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1037 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/admin/health_economics/health_economics_simple_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3889 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/admin/health_economics/health_economics_update_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1404 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/hepatitis_test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2264 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      492 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/malaria_test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      543 2024-03-11 21:08:18.000000 meta-edc-0.3.9/meta_subject/admin/medication_adherence_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1430 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/mnsi_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      510 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/modeladmin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1596 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/other_arv_regimens_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1763 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/patient_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1858 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/physical_exam_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      913 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/pregnancy_update_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      742 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/sf12_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5983 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/admin/study_medication_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1848 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/subject_requisition_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1314 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/admin/subject_visit_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1414 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/subject_visit_missed_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1144 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/urine_dipstick_test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1037 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/admin/urine_pregnancy_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2022-08-21 16:43:17.000000 meta-edc-0.3.9/meta_subject/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      289 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2618 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_subject/baker_recipes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6610 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      662 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.824041 meta-edc-0.3.9/meta_subject/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      349 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/form_validators/birth_outcomes_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3193 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/form_validators/delivery_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6293 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/form_validators/dm_referral_followup_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      530 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/form_validators/egfr_drop_notification_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4241 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/form_validators/followup_examination_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3371 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/form_validators/glucose_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      250 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/form_validators/health_economics_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.829530 meta-edc-0.3.9/meta_subject/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1646 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      374 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/birth_outcomes_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.830544 meta-edc-0.3.9/meta_subject/forms/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      344 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      714 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_fbc_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_hba1c_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      722 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_ins_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      714 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_lft_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      730 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_lipid_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1362 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_rft_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      375 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/complications_glycemia_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      375 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/concomitant_medication_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      447 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/delivery_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      567 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/dm_referral_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      507 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/egfr_drop_notification_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/eq53d3l_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      502 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/followup_examination_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      354 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/followup_vitals_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1267 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/glucose_fbg_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      442 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/glucose_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.831040 meta-edc-0.3.9/meta_subject/forms/health_economics/
+-rw-r--r--   0 erikvw     (501) staff       (20)      136 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/forms/health_economics/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      392 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/forms/health_economics/health_economics_simple_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      308 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/forms/health_economics/health_economics_update_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      794 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/hepatitis_test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      365 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/malaria_test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      865 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/medication_adherence_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2084 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_subject/forms/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      323 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/mnsi_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      962 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/other_arv_regimens_detail_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1687 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/other_arv_regimens_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1807 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/patient_history_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      786 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/physical_exam_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      559 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/pregnancy_update_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-06-24 08:54:57.000000 meta-edc-0.3.9/meta_subject/forms/sf12_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      821 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/slider_widget.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1481 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/study_medication_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      953 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/subject_requisition_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      791 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/forms/subject_visit_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2275 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/subject_visit_missed_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      827 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/urine_dipstick_test_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1267 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/forms/urine_pregnancy_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      325 2022-08-26 02:59:33.000000 meta-edc-0.3.9/meta_subject/identifiers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.669479 meta-edc-0.3.9/meta_subject/locale/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.669547 meta-edc-0.3.9/meta_subject/locale/sw/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.831188 meta-edc-0.3.9/meta_subject/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5685 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.669701 meta-edc-0.3.9/meta_subject/management/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.831820 meta-edc-0.3.9/meta_subject/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2432 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/management/commands/create_missing_refills.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1463 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_subject/management/commands/create_missing_rx.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8209 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/management/commands/missed.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.832496 meta-edc-0.3.9/meta_subject/metadata_rules/
+-rw-r--r--   0 erikvw     (501) staff       (20)       53 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_subject/metadata_rules/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3438 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/metadata_rules/metadata_rules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7117 2024-02-20 05:50:29.000000 meta-edc-0.3.9/meta_subject/metadata_rules/predicates.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.878045 meta-edc-0.3.9/meta_subject/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   408932 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    29351 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0002_auto_20191021_0353.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4024 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0003_auto_20191021_0534.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      739 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0004_auto_20191022_0134.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5818 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0005_auto_20191024_1000.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20050 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0006_auto_20191104_0756.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1141 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0007_auto_20191107_2249.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13943 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0008_auto_20191115_0132.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1129 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0009_auto_20191119_2331.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6879 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0010_auto_20191213_0314.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2779 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0011_auto_20200118_1854.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15554 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0012_auto_20200118_2334.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1829 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0013_auto_20200119_0013.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    32038 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0014_auto_20200120_1622.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      785 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0015_auto_20200120_1943.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2035 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0016_auto_20200123_1508.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7291 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0017_auto_20200325_0901.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    59621 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0018_coronakap_historicalcoronakap.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1560 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0019_auto_20200417_0315.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7013 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0020_auto_20200417_0329.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1177 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0021_auto_20200417_0332.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5512 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0022_auto_20200419_2223.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    25415 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0023_auto_20200419_2305.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14715 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0024_auto_20200419_2331.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7347 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0025_auto_20200420_1455.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1091 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0026_auto_20200420_1524.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4755 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0027_auto_20200420_1645.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6449 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0028_auto_20200420_1732.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6003 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0029_auto_20200420_1751.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5045 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0030_auto_20200420_1816.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4609 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0031_auto_20200422_2039.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7735 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0032_auto_20200515_0307.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18672 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0033_auto_20200516_2356.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1004 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0034_auto_20200517_0125.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1316 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0035_auto_20200517_0128.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2987 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0036_auto_20200517_0150.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      587 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0037_auto_20200517_0207.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26376 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0038_auto_20200520_0020.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6635 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0039_auto_20200524_1944.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18299 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0040_auto_20200527_2155.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12473 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0041_auto_20200528_0242.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      223 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0042_auto_20200528_0252.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1509 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0043_auto_20200528_1555.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2845 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0044_auto_20200528_1853.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1244 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0045_auto_20200530_1801.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3313 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0046_auto_20200530_1804.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      589 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0047_auto_20200530_1819.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      431 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0048_auto_20200530_1819.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      265 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0049_auto_20200613_2041.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      876 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0050_auto_20200614_1934.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20316 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0051_auto_20200617_2117.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    40851 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0052_auto_20210624_0225.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    27484 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0053_auto_20210628_2105.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3375 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0054_auto_20210628_2314.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2931 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0055_auto_20210628_2331.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3543 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0056_auto_20210702_0426.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2827 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0057_auto_20210702_0458.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1981 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0058_auto_20210702_0533.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14817 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0059_auto_20210709_2056.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1311 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0060_auto_20210709_2241.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    36061 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0061_auto_20210710_1929.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1007 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0062_auto_20210713_0616.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20740 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0063_auto_20210715_0337.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    31933 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0064_auto_20210715_2336.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10393 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0065_auto_20210716_0813.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    27932 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0066_auto_20210721_0335.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    47359 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0067_auto_20210726_0340.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    41022 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0068_auto_20210728_1809.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2083 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0069_auto_20210801_2021.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2865 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0070_auto_20210804_0438.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      995 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0071_auto_20210804_0715.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    25832 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0072_auto_20210805_1545.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    41644 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0073_auto_20210809_0055.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      290 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_subject/migrations/0074_auto_20210809_1744.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1996 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0075_auto_20210809_1744.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      973 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0076_auto_20210809_1854.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8020 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0077_auto_20210809_2323.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1194 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0078_auto_20210810_0857.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    35483 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0079_auto_20210812_0335.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    17307 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0080_auto_20210812_0400.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    27695 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0081_auto_20210817_2306.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12293 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0082_auto_20210823_1612.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14438 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0083_auto_20210823_1620.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15218 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0084_auto_20210910_0234.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2961 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0085_auto_20210911_2036.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15644 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0086_auto_20210920_0229.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2917 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0087_auto_20210922_2058.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    28868 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0088_auto_20210924_0027.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6593 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0089_auto_20210924_0121.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15971 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0090_auto_20210924_0424.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1875 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0091_auto_20210929_2324.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    16399 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0092_auto_20211013_0447.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    33887 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0093_auto_20211117_0352.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4811 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0094_auto_20211123_1645.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    22478 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0095_auto_20220128_1719.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3418 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0096_auto_20220304_0501.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2099 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0097_auto_20220304_2233.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    21282 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0098_auto_20220309_2106.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1908 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0099_auto_20220309_2218.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1090 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0100_auto_20220309_2238.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    61583 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0101_auto_20220316_2147.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    15290 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0102_auto_20220324_0304.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      868 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0103_auto_20220324_0326.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      966 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0104_auto_20220412_2151.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1290 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0105_auto_20220412_2310.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      772 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0106_auto_20220414_1741.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1492 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0107_auto_20220415_0043.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      688 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0108_auto_20220415_1747.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      556 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0109_auto_20220415_1758.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2516 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0110_auto_20220512_1811.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3010 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0111_alter_followupvitals_severe_htn_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1035 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0112_historicalsubjectvisit_document_status_comments_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      719 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0113_bloodresultsrft_egfr_percent_change_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      991 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0114_alter_bloodresultsrft_egfr_percent_change_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18446 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0115_historicalegfrnotification_egfrnotification.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1176 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0116_egfrnotification_report_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3278 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0117_alter_egfrnotification_managers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2049 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0118_delivery_crf_status_delivery_crf_status_comments_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0119_historicalstudymedication_roundup_divisible_by_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2887 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0120_alter_birthoutcomes_managers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    21740 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0121_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      812 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0122_auto_20220708_2144.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8262 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0123_auto_20220714_2136.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1206 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0124_auto_20220714_2303.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1568 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0125_auto_20220719_2134.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      776 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0126_auto_20220719_2142.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5488 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0127_auto_20220720_0053.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0128_auto_20220720_0055.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      490 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0129_auto_20220720_0108.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      683 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0130_auto_20220720_0216.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1932 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0131_auto_20220722_0411.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      843 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0132_auto_20220722_1825.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    28130 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0133_auto_20220722_2140.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1806 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0134_auto_20220722_2211.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2263 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0135_auto_20220722_2212.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8660 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0136_egfrdropnotification_creatinine_quantifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1138 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0137_alter_egfrdropnotification_egfr_percent_change_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3531 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0138_alter_glucose_fbg_datetime_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      938 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0139_alter_bloodresultsins_ins_units_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4341 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0140_alter_bloodresultsfbc_action_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4570 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0141_auto_20220826_0258.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5196 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0142_auto_20220826_0322.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3810 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0143_auto_20220826_0406.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      964 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0144_auto_20220907_0157.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1785 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0145_auto_20220907_0202.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      618 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0146_auto_20220907_0207.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1906 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0147_auto_20220907_1505.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1814 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0148_auto_20220908_1826.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1000 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0149_auto_20220913_2139.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1222 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0150_auto_20220914_0039.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    52998 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0151_auto_20220918_0508.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      738 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0152_auto_20220925_0509.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1172 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0153_auto_20220928_0250.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1010 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0154_auto_20220928_0419.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9271 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0155_auto_20220929_1742.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5444 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0156_alter_bloodresultsfbc_assay_datetime_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    23251 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0157_remove_bloodresultsfbc_crf_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2191 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0158_alter_followupexamination_attended_clinic_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6479 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0159_alter_bloodresultsfbc_results_abnormal_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1614 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/migrations/0160_alter_healtheconomicssimple_education_certificate_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)   129780 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0161_alter_birthoutcomes_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2347 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/migrations/0162_alter_followupexamination_abdominal_tenderness_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)   114643 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0163_alter_birthoutcomes_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    29185 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0164_dmreferralfollowup_historicaldmreferralfollowup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      687 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0165_alter_dmreferralfollowup_healthcare_workers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7299 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0166_rename_dm_medications_other_dmreferralfollowup_other_dm_medications_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      704 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0167_rename_healthcare_workers_other_dmreferralfollowup_other_healthcare_workers_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1926 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0168_alter_dmreferralfollowup_last_missed_pill_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3695 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0169_alter_dmreferralfollowup_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1748 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0170_remove_glucose_repeat_fbg_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2813 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0171_alter_glucose_endpoint_today_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2328 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0172_remove_historicalbloodresultsglu_action_item_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3429 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0173_alter_glucosefbg_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3274 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0174_remove_glucosefbg_glucose_abnormal_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      677 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0175_auto_20240214_2239.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1302 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/migrations/0176_alter_glucosefbg_glucose_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3001 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/migrations/0177_alter_bloodresultslft_alp_value_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    31556 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/migrations/0178_historicalhealtheconomicsupdate_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    32903 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/migrations/0179_alter_birthoutcomes_consent_model_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2301 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/migrations/0180_dmreferralfollowup_missed_referral_reasons_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_subject/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.879508 meta-edc-0.3.9/meta_subject/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      286 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2904 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_subject/model_mixins/arv_history_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      248 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/model_mixins/crf_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      298 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/model_mixins/crf_with_action_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2022-06-24 08:52:03.000000 meta-edc-0.3.9/meta_subject/model_mixins/search_slug_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1160 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/model_mixins/vitals_fields_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.888360 meta-edc-0.3.9/meta_subject/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1715 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3033 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/birth_outcomes.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.889712 meta-edc-0.3.9/meta_subject/models/blood_results/
+-rw-r--r--   0 erikvw     (501) staff       (20)      290 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/blood_results/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1252 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_fbc.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      958 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_hba1c.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      974 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_ins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1157 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_lft.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1090 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_lipid.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1568 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_rft.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1849 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/complications.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6056 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/complications_glycemia.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      368 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/concomitant_medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5100 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/delivery.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1063 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/models/diet_and_lifestyle.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5937 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/models/dm_referral_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      557 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/egfr_drop_notification.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/eq5d3l.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8116 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/models/followup_examination.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      903 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/models/followup_vitals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2539 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/glucose.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2101 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/glucose_fbg.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/glucose_review.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.890659 meta-edc-0.3.9/meta_subject/models/health_economics/
+-rw-r--r--   0 erikvw     (501) staff       (20)      164 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/models/health_economics/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9715 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/models/health_economics/health_economics.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      741 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/models/health_economics/health_economics_simple.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3210 2024-03-08 06:41:57.000000 meta-edc-0.3.9/meta_subject/models/health_economics/health_economics_update.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1850 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/hepatitis_test.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      343 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/malaria_test.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      399 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      284 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/mnsi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/off_study_drug.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      607 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/other_arv_regimens.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1828 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/other_arv_regimens_detail.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4510 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/patient_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1971 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/models/physical_exam.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      949 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/pregnancy_update.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      283 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/models/sf12.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3989 2022-07-08 07:31:04.000000 meta-edc-0.3.9/meta_subject/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      461 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/study_medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      342 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/models/subject_requisition.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2152 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/models/subject_visit.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      747 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/subject_visit_missed.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      247 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_subject/models/todo.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1178 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/urine_dipstick_test.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1336 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/models/urine_pregnancy.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.670254 meta-edc-0.3.9/meta_subject/static/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.891101 meta-edc-0.3.9/meta_subject/static/meta_subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1359 2022-08-22 17:23:22.000000 meta-edc-0.3.9/meta_subject/static/meta_subject/slider.css
+-rw-r--r--   0 erikvw     (501) staff       (20)    10150 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_subject/static/meta_subject/slider.png
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.670363 meta-edc-0.3.9/meta_subject/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.891409 meta-edc-0.3.9/meta_subject/templates/meta_subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)      270 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/templates/meta_subject/endpoint_review_instructions.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.891561 meta-edc-0.3.9/meta_subject/templates/meta_subject/widgets/
+-rw-r--r--   0 erikvw     (501) staff       (20)      913 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_subject/templates/meta_subject/widgets/slider.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.892005 meta-edc-0.3.9/meta_subject/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_subject/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_subject/tests/holidays.csv
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.894692 meta-edc-0.3.9/meta_subject/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-0.3.9/meta_subject/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9994 2024-03-27 20:33:11.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_egfr.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2454 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_fixes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1871 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_followup.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      454 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_manager_order.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2517 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_medication_adherence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4445 2022-08-22 17:23:22.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_metadata_rules.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9964 2024-02-20 05:50:29.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_mnsi.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2827 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_patient_history_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2947 2024-03-27 19:35:21.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_physical_exam.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7330 2024-02-20 05:50:29.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_sf12.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10161 2024-02-13 23:41:07.000000 meta-edc-0.3.9/meta_subject/tests/tests/test_study_medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1109 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_subject/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      206 2022-06-24 09:02:28.000000 meta-edc-0.3.9/meta_subject/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.895619 meta-edc-0.3.9/meta_visit_schedule/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-07-07 23:18:25.000000 meta-edc-0.3.9/meta_visit_schedule/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      164 2021-07-02 03:53:00.000000 meta-edc-0.3.9/meta_visit_schedule/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      423 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_visit_schedule/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.895736 meta-edc-0.3.9/meta_visit_schedule/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_visit_schedule/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_visit_schedule/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.895960 meta-edc-0.3.9/meta_visit_schedule/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/meta_visit_schedule/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.896347 meta-edc-0.3.9/meta_visit_schedule/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-0.3.9/meta_visit_schedule/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7239 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_visit_schedule/tests/tests/test_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-0.3.9/meta_visit_schedule/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.896628 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/
+-rw-r--r--   0 erikvw     (501) staff       (20)      339 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.898204 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-04-11 18:27:09.000000 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11947 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/crfs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/crfs_pregnancy.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3959 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/requisitions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6881 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1123 2024-02-15 06:32:55.000000 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/schedule_pregnancy.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      537 2024-02-13 23:44:08.000000 meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1734 2024-02-13 23:44:08.000000 meta-edc-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)      463 2022-08-23 13:24:02.000000 meta-edc-0.3.9/releases
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.898415 meta-edc-0.3.9/reports/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-06-18 19:11:34.000000 meta-edc-0.3.9/reports/20200603.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1006 2024-03-27 20:33:11.000000 meta-edc-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1183 2024-03-31 02:04:37.901537 meta-edc-0.3.9/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.898629 meta-edc-0.3.9/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-03-31 02:04:37.900353 meta-edc-0.3.9/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)     5307 2022-08-22 17:23:22.000000 meta-edc-0.3.9/tests/etc/randomization_list.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      538 2020-03-15 03:34:20.000000 meta-edc-0.3.9/tests/holidays.csv
```

### Comparing `meta-edc-0.3.8/.env-tests` & `meta-edc-0.3.9/.env-tests`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/.github/workflows/build.yml` & `meta-edc-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/.gitignore` & `meta-edc-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/.pre-commit-config.yaml` & `meta-edc-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/CHANGES` & `meta-edc-0.3.9/CHANGES`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/LICENSE` & `meta-edc-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/PKG-INFO` & `meta-edc-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta-edc
-Version: 0.3.8
+Version: 0.3.9
 Summary: META Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 Home-page: https://github.com/meta-trial/meta-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc META EDC,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: edc==0.5.75
+Requires-Dist: edc==0.5.76
 Requires-Dist: edc-microscopy
 Requires-Dist: beautifulsoup4
 
 |pypi| |actions| |codecov| |downloads|
 
 
 META Edc
```

### Comparing `meta-edc-0.3.8/README.rst` & `meta-edc-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/TODO.txt` & `meta-edc-0.3.9/TODO.txt`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta2/conf/live.conf` & `meta-edc-0.3.9/bin/nginx/meta2/conf/live.conf`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta2/conf/uat.conf` & `meta-edc-0.3.9/bin/nginx/meta2/conf/uat.conf`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta2/www/html/index.html` & `meta-edc-0.3.9/bin/nginx/meta2/www/html/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/index.html` & `meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/tz/index.html` & `meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta2/www/html/live.meta.clinicedc.org/ug/index.html` & `meta-edc-0.3.9/bin/nginx/meta2/www/html/live.meta.clinicedc.org/ug/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/tz/index.html` & `meta-edc-0.3.9/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/ug/index.html` & `meta-edc-0.3.9/bin/nginx/meta2/www/html/uat.meta.clinicedc.org/ug/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta3/conf/live.conf` & `meta-edc-0.3.9/bin/nginx/meta3/conf/live.conf`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta3/conf/uat.conf` & `meta-edc-0.3.9/bin/nginx/meta3/conf/uat.conf`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta3/www/html/index.html` & `meta-edc-0.3.9/bin/nginx/meta3/www/html/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/index.html` & `meta-edc-0.3.9/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/tz/index.html` & `meta-edc-0.3.9/bin/nginx/meta3/www/html/live.meta3.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta3/www/html/uat.meta3.clinicedc.org/tz/index.html` & `meta-edc-0.3.9/bin/nginx/meta3/www/html/uat.meta3.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta4/conf/live.conf` & `meta-edc-0.3.9/bin/nginx/meta4/conf/live.conf`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta4/conf/uat.conf` & `meta-edc-0.3.9/bin/nginx/meta4/conf/uat.conf`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta4/www/html/index.html` & `meta-edc-0.3.9/bin/nginx/meta4/www/html/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/index.html` & `meta-edc-0.3.9/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/tz/index.html` & `meta-edc-0.3.9/bin/nginx/meta4/www/html/live.meta3.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/nginx/meta4/www/html/uat.meta3.clinicedc.org/tz/index.html` & `meta-edc-0.3.9/bin/nginx/meta4/www/html/uat.meta3.clinicedc.org/tz/index.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/scripts/update_edc.sh` & `meta-edc-0.3.9/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/systemd/celery-uat.service` & `meta-edc-0.3.9/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/bin/systemd/celery.service` & `meta-edc-0.3.9/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/docs/forms_reference.md` & `meta-edc-0.3.9/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/docs/images/user_groups.png` & `meta-edc-0.3.9/docs/images/user_groups.png`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/docs/updates/0.1.65/renamed_fields.txt` & `meta-edc-0.3.9/docs/updates/0.1.65/renamed_fields.txt`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/docs/updates/0.1.65/update_1_65_renamed_fields.py` & `meta-edc-0.3.9/docs/updates/0.1.65/update_1_65_renamed_fields.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/env.sample` & `meta-edc-0.3.9/env.sample`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/holidays.csv` & `meta-edc-0.3.9/holidays.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/label_templates/2.25x1.25in/aliquot.lbl` & `meta-edc-0.3.9/label_templates/2.25x1.25in/aliquot.lbl`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/label_templates/2.25x1.25in/requisition.lbl` & `meta-edc-0.3.9/label_templates/2.25x1.25in/requisition.lbl`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/manage.py` & `meta-edc-0.3.9/manage.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/action_items.py` & `meta-edc-0.3.9/meta_ae/action_items.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/admin/ae_initial_admin.py` & `meta-edc-0.3.9/meta_ae/admin/ae_initial_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/admin/death_report_admin.py` & `meta-edc-0.3.9/meta_ae/admin/death_report_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/admin/death_report_tmg_admin.py` & `meta-edc-0.3.9/meta_ae/admin/death_report_tmg_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/admin/death_report_tmg_second_admin.py` & `meta-edc-0.3.9/meta_ae/admin/death_report_tmg_second_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/admin/hospitalization_admin.py` & `meta-edc-0.3.9/meta_ae/admin/hospitalization_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/admin/modeladmin_mixins.py` & `meta-edc-0.3.9/meta_ae/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/baker_recipes.py` & `meta-edc-0.3.9/meta_ae/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/choices.py` & `meta-edc-0.3.9/meta_ae/choices.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/forms/death_report_form.py` & `meta-edc-0.3.9/meta_ae/forms/death_report_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/forms/modelform_mixins.py` & `meta-edc-0.3.9/meta_ae/forms/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/list_data.py` & `meta-edc-0.3.9/meta_ae/list_data.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0001_initial.py` & `meta-edc-0.3.9/meta_ae/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0002_auto_20191024_1000.py` & `meta-edc-0.3.9/meta_ae/migrations/0002_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0003_auto_20191102_0033.py` & `meta-edc-0.3.9/meta_ae/migrations/0003_auto_20191102_0033.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0004_auto_20191114_0821.py` & `meta-edc-0.3.9/meta_ae/migrations/0004_auto_20191114_0821.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0005_auto_20210624_0225.py` & `meta-edc-0.3.9/meta_ae/migrations/0005_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0006_aelocalreview_aesponsorreview.py` & `meta-edc-0.3.9/meta_ae/migrations/0006_aelocalreview_aesponsorreview.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0007_auto_20210911_2036.py` & `meta-edc-0.3.9/meta_ae/migrations/0007_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0008_auto_20211011_1657.py` & `meta-edc-0.3.9/meta_ae/migrations/0008_auto_20211011_1657.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0009_auto_20220307_1929.py` & `meta-edc-0.3.9/meta_ae/migrations/0009_auto_20220307_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0010_auto_20220704_1841.py` & `meta-edc-0.3.9/meta_ae/migrations/0010_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0011_alter_aefollowup_action_identifier_and_more.py` & `meta-edc-0.3.9/meta_ae/migrations/0011_alter_aefollowup_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0012_auto_20220826_0258.py` & `meta-edc-0.3.9/meta_ae/migrations/0012_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0013_auto_20220826_0322.py` & `meta-edc-0.3.9/meta_ae/migrations/0013_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0014_auto_20220826_0406.py` & `meta-edc-0.3.9/meta_ae/migrations/0014_auto_20220826_0406.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0015_auto_20220907_0157.py` & `meta-edc-0.3.9/meta_ae/migrations/0015_auto_20220907_0157.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0016_rename_narrative_aetmg_investigator_narrative_and_more.py` & `meta-edc-0.3.9/meta_ae/migrations/0016_rename_narrative_aetmg_investigator_narrative_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0017_auto_20221130_2257.py` & `meta-edc-0.3.9/meta_ae/migrations/0017_auto_20221130_2257.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0018_alter_deathreporttmg_cause_of_death_agreed_and_more.py` & `meta-edc-0.3.9/meta_ae/migrations/0018_alter_deathreporttmg_cause_of_death_agreed_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0019_alter_aefollowup_managers_alter_aeinitial_managers_and_more.py` & `meta-edc-0.3.9/meta_ae/migrations/0019_alter_aefollowup_managers_alter_aeinitial_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0020_alter_aesusar_options_alter_aetmg_options_and_more.py` & `meta-edc-0.3.9/meta_ae/migrations/0020_alter_aesusar_options_alter_aetmg_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0021_alter_aefollowup_site_alter_aeinitial_site_and_more.py` & `meta-edc-0.3.9/meta_ae/migrations/0021_alter_aefollowup_site_alter_aeinitial_site_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/migrations/0022_historicalhospitalization_hospitalization.py` & `meta-edc-0.3.9/meta_ae/migrations/0022_historicalhospitalization_hospitalization.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/model_mixins/ae_review_model_mixin.py` & `meta-edc-0.3.9/meta_ae/model_mixins/ae_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/model_mixins/death_report_model_mixin.py` & `meta-edc-0.3.9/meta_ae/model_mixins/death_report_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/models/death_report_tmg_second.py` & `meta-edc-0.3.9/meta_ae/models/death_report_tmg_second.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/models/hospitalization.py` & `meta-edc-0.3.9/meta_ae/models/hospitalization.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/models/managers.py` & `meta-edc-0.3.9/meta_ae/models/managers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/pdf_reports/meta_pdf_report_mixin.py` & `meta-edc-0.3.9/meta_ae/pdf_reports/meta_pdf_report_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/templates/meta_ae/bootstrap3/ae_initial_description.html` & `meta-edc-0.3.9/meta_ae/templates/meta_ae/bootstrap3/ae_initial_description.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/templatetags/meta_ae_extras.py` & `meta-edc-0.3.9/meta_ae/templatetags/meta_ae_extras.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/tests/holidays.csv` & `meta-edc-0.3.9/meta_ae/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_ae/tests/tests/test_actions.py` & `meta-edc-0.3.9/meta_ae/tests/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_auth/auth_objects.py` & `meta-edc-0.3.9/meta_auth/auth_objects.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_auth/auths.py` & `meta-edc-0.3.9/meta_auth/auths.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/action_items.py` & `meta-edc-0.3.9/meta_consent/action_items.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/admin/actions/create_missing_prescriptions.py` & `meta-edc-0.3.9/meta_consent/admin/actions/create_missing_prescriptions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/admin/modeladmin_mixins.py` & `meta-edc-0.3.9/meta_consent/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/admin/subject_consent_admin.py` & `meta-edc-0.3.9/meta_consent/admin/subject_consent_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/admin/subject_consent_v1_admin.py` & `meta-edc-0.3.9/meta_consent/admin/subject_consent_v1_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/baker_recipes.py` & `meta-edc-0.3.9/meta_consent/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/consents.py` & `meta-edc-0.3.9/meta_consent/consents.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/form_validators/subject_consent_form_validator.py` & `meta-edc-0.3.9/meta_consent/form_validators/subject_consent_form_validator.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/forms/subject_consent_form.py` & `meta-edc-0.3.9/meta_consent/forms/subject_consent_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/forms/subject_consent_v1_form.py` & `meta-edc-0.3.9/meta_consent/forms/subject_consent_v1_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/forms/subject_reconsent_form.py` & `meta-edc-0.3.9/meta_consent/forms/subject_reconsent_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/locale/sw/LC_MESSAGES/django.po` & `meta-edc-0.3.9/meta_consent/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/management/commands/create_missing_prescriptions.py` & `meta-edc-0.3.9/meta_consent/management/commands/create_missing_prescriptions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0001_initial.py` & `meta-edc-0.3.9/meta_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0002_auto_20191024_1000.py` & `meta-edc-0.3.9/meta_consent/migrations/0002_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0003_auto_20200325_0901.py` & `meta-edc-0.3.9/meta_consent/migrations/0003_auto_20200325_0901.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0004_auto_20210624_0225.py` & `meta-edc-0.3.9/meta_consent/migrations/0004_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0005_alter_subjectconsent_options.py` & `meta-edc-0.3.9/meta_consent/migrations/0005_alter_subjectconsent_options.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0006_auto_20210911_2036.py` & `meta-edc-0.3.9/meta_consent/migrations/0006_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0007_auto_20220128_1719.py` & `meta-edc-0.3.9/meta_consent/migrations/0007_auto_20220128_1719.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0008_auto_20220412_2151.py` & `meta-edc-0.3.9/meta_consent/migrations/0008_auto_20220412_2151.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0009_auto_20220704_1841.py` & `meta-edc-0.3.9/meta_consent/migrations/0009_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0010_alter_historicalsubjectreconsent_action_identifier_and_more.py` & `meta-edc-0.3.9/meta_consent/migrations/0010_alter_historicalsubjectreconsent_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0011_auto_20220826_0258.py` & `meta-edc-0.3.9/meta_consent/migrations/0011_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0012_auto_20220826_0322.py` & `meta-edc-0.3.9/meta_consent/migrations/0012_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0014_alter_subjectconsent_managers.py` & `meta-edc-0.3.9/meta_consent/migrations/0014_alter_subjectconsent_managers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0015_auto_20220914_0542.py` & `meta-edc-0.3.9/meta_consent/migrations/0015_auto_20220914_0542.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0016_auto_20220914_0547.py` & `meta-edc-0.3.9/meta_consent/migrations/0016_auto_20220914_0547.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0017_auto_20220929_1742.py` & `meta-edc-0.3.9/meta_consent/migrations/0017_auto_20220929_1742.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0018_alter_subjectconsent_options_and_more.py` & `meta-edc-0.3.9/meta_consent/migrations/0018_alter_subjectconsent_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0019_alter_subjectconsent_options_and_more.py` & `meta-edc-0.3.9/meta_consent/migrations/0019_alter_subjectconsent_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0020_historicalsubjectconsent_model_name_and_more.py` & `meta-edc-0.3.9/meta_consent/migrations/0020_historicalsubjectconsent_model_name_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0022_alter_historicalsubjectconsent_site_and_more.py` & `meta-edc-0.3.9/meta_consent/migrations/0022_alter_historicalsubjectconsent_site_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0023_subjectconsentv1_and_more.py` & `meta-edc-0.3.9/meta_consent/migrations/0023_subjectconsentv1_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0024_historicalsubjectconsentv1.py` & `meta-edc-0.3.9/meta_consent/migrations/0024_historicalsubjectconsentv1.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/migrations/0025_alter_historicalsubjectconsent_first_name_and_more.py` & `meta-edc-0.3.9/meta_consent/migrations/0025_alter_historicalsubjectconsent_first_name_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/models/signals.py` & `meta-edc-0.3.9/meta_consent/models/signals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/models/subject_consent.py` & `meta-edc-0.3.9/meta_consent/models/subject_consent.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/models/subject_reconsent.py` & `meta-edc-0.3.9/meta_consent/models/subject_reconsent.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/tests/holidays.csv` & `meta-edc-0.3.9/meta_consent/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/tests/tests/test_form_validators.py` & `meta-edc-0.3.9/meta_consent/tests/tests/test_form_validators.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_consent/tests/urls.py` & `meta-edc-0.3.9/meta_consent/tests/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/locale/sw/LC_MESSAGES/django.po` & `meta-edc-0.3.9/meta_dashboard/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/navbars.py` & `meta-edc-0.3.9/meta_dashboard/navbars.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/screening_button.html` & `meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/buttons/screening_button.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/screening/listboard.html` & `meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/screening/listboard.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/listboard.html` & `meta-edc-0.3.9/meta_dashboard/templates/meta_dashboard/bootstrap3/subject/listboard.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/templatetags/meta_dashboard_extras.py` & `meta-edc-0.3.9/meta_dashboard/templatetags/meta_dashboard_extras.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/tests/admin.py` & `meta-edc-0.3.9/meta_dashboard/tests/admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/tests/holidays.csv` & `meta-edc-0.3.9/meta_dashboard/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/tests/urls.py` & `meta-edc-0.3.9/meta_dashboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/urls.py` & `meta-edc-0.3.9/meta_dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/view_utils/subject_screening_button.py` & `meta-edc-0.3.9/meta_dashboard/view_utils/subject_screening_button.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/views/screening/listboard_view.py` & `meta-edc-0.3.9/meta_dashboard/views/screening/listboard_view.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_dashboard/views/subject/listboard/listboard_view.py` & `meta-edc-0.3.9/meta_dashboard/views/subject/listboard/listboard_view.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_data_manager/handlers.py` & `meta-edc-0.3.9/meta_data_manager/handlers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/admin.py` & `meta-edc-0.3.9/meta_edc/admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/celery.py` & `meta-edc-0.3.9/meta_edc/celery.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/management/commands/update_forms_reference.py` & `meta-edc-0.3.9/meta_edc/management/commands/update_forms_reference.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/model_callers.py` & `meta-edc-0.3.9/meta_edc/model_callers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/navbars.py` & `meta-edc-0.3.9/meta_edc/navbars.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/settings/debug.py` & `meta-edc-0.3.9/meta_edc/settings/debug.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/settings/defaults.py` & `meta-edc-0.3.9/meta_edc/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/settings/logging.py` & `meta-edc-0.3.9/meta_edc/settings/logging.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/settings/minimal.py` & `meta-edc-0.3.9/meta_edc/settings/minimal.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/templates/meta_edc/bootstrap3/home.html` & `meta-edc-0.3.9/meta_edc/templates/meta_edc/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/tests/etc/randomization_list_phase_three.csv` & `meta-edc-0.3.9/meta_edc/tests/etc/randomization_list_phase_three.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/tests/etc/user-rsa-local-private.pem` & `meta-edc-0.3.9/meta_edc/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/tests/etc/user-rsa-restricted-private.pem` & `meta-edc-0.3.9/meta_edc/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/tests/test_settings.py` & `meta-edc-0.3.9/meta_edc/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/tests/tests/test_endpoints.py` & `meta-edc-0.3.9/meta_edc/tests/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/urls.py` & `meta-edc-0.3.9/meta_edc/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc/views/home_view.py` & `meta-edc-0.3.9/meta_edc/views/home_view.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_edc.egg-info/PKG-INFO` & `meta-edc-0.3.9/meta_edc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta-edc
-Version: 0.3.8
+Version: 0.3.9
 Summary: META Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 Home-page: https://github.com/meta-trial/meta-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc META EDC,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: edc==0.5.75
+Requires-Dist: edc==0.5.76
 Requires-Dist: edc-microscopy
 Requires-Dist: beautifulsoup4
 
 |pypi| |actions| |codecov| |downloads|
 
 
 META Edc
```

### Comparing `meta-edc-0.3.8/meta_edc.egg-info/SOURCES.txt` & `meta-edc-0.3.9/meta_edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_labs/lab_profiles.py` & `meta-edc-0.3.9/meta_labs/lab_profiles.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_labs/reportables.py` & `meta-edc-0.3.9/meta_labs/reportables.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_labs/tests/test_labs.py` & `meta-edc-0.3.9/meta_labs/tests/test_labs.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_labs/tests/test_reportables.py` & `meta-edc-0.3.9/meta_labs/tests/test_reportables.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/admin.py` & `meta-edc-0.3.9/meta_lists/admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/list_data.py` & `meta-edc-0.3.9/meta_lists/list_data.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0001_initial.py` & `meta-edc-0.3.9/meta_lists/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0002_auto_20191026_2231.py` & `meta-edc-0.3.9/meta_lists/migrations/0002_auto_20191026_2231.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0003_auto_20191102_0033.py` & `meta-edc-0.3.9/meta_lists/migrations/0003_auto_20191102_0033.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0004_auto_20191102_1859.py` & `meta-edc-0.3.9/meta_lists/migrations/0004_auto_20191102_1859.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0005_auto_20191104_0930.py` & `meta-edc-0.3.9/meta_lists/migrations/0005_auto_20191104_0930.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0006_auto_20200514_1959.py` & `meta-edc-0.3.9/meta_lists/migrations/0006_auto_20200514_1959.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0007_auto_20200516_2356.py` & `meta-edc-0.3.9/meta_lists/migrations/0007_auto_20200516_2356.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0008_auto_20200528_1517.py` & `meta-edc-0.3.9/meta_lists/migrations/0008_auto_20200528_1517.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0010_auto_20200617_1738.py` & `meta-edc-0.3.9/meta_lists/migrations/0010_auto_20200617_1738.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0011_auto_20210624_0225.py` & `meta-edc-0.3.9/meta_lists/migrations/0011_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0012_auto_20210728_1809.py` & `meta-edc-0.3.9/meta_lists/migrations/0012_auto_20210728_1809.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0013_transferreasons_and_more.py` & `meta-edc-0.3.9/meta_lists/migrations/0013_transferreasons_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0014_auto_20220913_2139.py` & `meta-edc-0.3.9/meta_lists/migrations/0014_auto_20220913_2139.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0015_abnormalfootappearanceobservations_extra_value_and_more.py` & `meta-edc-0.3.9/meta_lists/migrations/0015_abnormalfootappearanceobservations_extra_value_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0016_alter_abnormalfootappearanceobservations_options_and_more.py` & `meta-edc-0.3.9/meta_lists/migrations/0016_alter_abnormalfootappearanceobservations_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0017_complications_dmmedications_dmtreatments_and_more.py` & `meta-edc-0.3.9/meta_lists/migrations/0017_complications_dmmedications_dmtreatments_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/migrations/0018_missedreferralreasons.py` & `meta-edc-0.3.9/meta_lists/migrations/0018_missedreferralreasons.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_lists/models.py` & `meta-edc-0.3.9/meta_lists/models.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_pharmacy/apps.py` & `meta-edc-0.3.9/meta_pharmacy/apps.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_pharmacy/migrations/0001_initial.py` & `meta-edc-0.3.9/meta_pharmacy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_pharmacy/prepare_meta_pharmacy.py` & `meta-edc-0.3.9/meta_pharmacy/prepare_meta_pharmacy.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/action_items.py` & `meta-edc-0.3.9/meta_prn/action_items.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/__init__.py` & `meta-edc-0.3.9/meta_prn/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/end_of_study_admin.py` & `meta-edc-0.3.9/meta_prn/admin/end_of_study_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/loss_to_followup_admin.py` & `meta-edc-0.3.9/meta_prn/admin/loss_to_followup_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/off_study_medication_admin.py` & `meta-edc-0.3.9/meta_prn/admin/off_study_medication_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/offschedule_admin.py` & `meta-edc-0.3.9/meta_prn/admin/offschedule_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/offschedule_postnatal_admin.py` & `meta-edc-0.3.9/meta_prn/admin/offschedule_postnatal_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/offschedule_pregnancy_admin.py` & `meta-edc-0.3.9/meta_prn/admin/offschedule_pregnancy_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/onschedule_admin.py` & `meta-edc-0.3.9/meta_prn/admin/onschedule_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/pregnancy_notification_admin.py` & `meta-edc-0.3.9/meta_prn/admin/pregnancy_notification_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/protocol_incident_admin.py` & `meta-edc-0.3.9/meta_prn/admin/protocol_incident_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/admin/subject_transfer_admin.py` & `meta-edc-0.3.9/meta_prn/admin/subject_transfer_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/baker_recipes.py` & `meta-edc-0.3.9/meta_prn/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/choices.py` & `meta-edc-0.3.9/meta_prn/choices.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/constants.py` & `meta-edc-0.3.9/meta_prn/constants.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/form_validators/end_of_study.py` & `meta-edc-0.3.9/meta_prn/form_validators/end_of_study.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/form_validators/protocol_incident.py` & `meta-edc-0.3.9/meta_prn/form_validators/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/forms/end_of_study_form.py` & `meta-edc-0.3.9/meta_prn/forms/end_of_study_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/forms/loss_to_followup_form.py` & `meta-edc-0.3.9/meta_prn/forms/loss_to_followup_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/forms/off_study_medication_form.py` & `meta-edc-0.3.9/meta_prn/forms/off_study_medication_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/forms/offschedule_form.py` & `meta-edc-0.3.9/meta_prn/forms/offschedule_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/forms/offschedule_pregnancy_form.py` & `meta-edc-0.3.9/meta_prn/forms/offschedule_pregnancy_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/forms/pregnancy_notification_form.py` & `meta-edc-0.3.9/meta_prn/forms/pregnancy_notification_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/forms/subject_transfer_form.py` & `meta-edc-0.3.9/meta_prn/forms/subject_transfer_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/list_data.py` & `meta-edc-0.3.9/meta_prn/list_data.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0001_initial.py` & `meta-edc-0.3.9/meta_prn/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0002_auto_20191024_1000.py` & `meta-edc-0.3.9/meta_prn/migrations/0002_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0003_auto_20200120_2020.py` & `meta-edc-0.3.9/meta_prn/migrations/0003_auto_20200120_2020.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0004_auto_20200403_0332.py` & `meta-edc-0.3.9/meta_prn/migrations/0004_auto_20200403_0332.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0005_auto_20200524_1944.py` & `meta-edc-0.3.9/meta_prn/migrations/0005_auto_20200524_1944.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0006_auto_20210624_0225.py` & `meta-edc-0.3.9/meta_prn/migrations/0006_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0007_auto_20210721_0335.py` & `meta-edc-0.3.9/meta_prn/migrations/0007_auto_20210721_0335.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0008_auto_20210910_0238.py` & `meta-edc-0.3.9/meta_prn/migrations/0008_auto_20210910_0238.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0009_auto_20210910_0239.py` & `meta-edc-0.3.9/meta_prn/migrations/0009_auto_20210910_0239.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0010_auto_20210910_1906.py` & `meta-edc-0.3.9/meta_prn/migrations/0010_auto_20210910_1906.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0011_auto_20210910_1911.py` & `meta-edc-0.3.9/meta_prn/migrations/0011_auto_20210910_1911.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0012_auto_20210911_0004.py` & `meta-edc-0.3.9/meta_prn/migrations/0012_auto_20210911_0004.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0013_auto_20210911_2036.py` & `meta-edc-0.3.9/meta_prn/migrations/0013_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0014_auto_20211003_1709.py` & `meta-edc-0.3.9/meta_prn/migrations/0014_auto_20211003_1709.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0015_auto_20211104_1447.py` & `meta-edc-0.3.9/meta_prn/migrations/0015_auto_20211104_1447.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0016_auto_20220128_1719.py` & `meta-edc-0.3.9/meta_prn/migrations/0016_auto_20220128_1719.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0017_auto_20220307_1929.py` & `meta-edc-0.3.9/meta_prn/migrations/0017_auto_20220307_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0018_auto_20220309_2106.py` & `meta-edc-0.3.9/meta_prn/migrations/0018_auto_20220309_2106.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0019_auto_20220309_2230.py` & `meta-edc-0.3.9/meta_prn/migrations/0019_auto_20220309_2230.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0020_auto_20220310_0439.py` & `meta-edc-0.3.9/meta_prn/migrations/0020_auto_20220310_0439.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0021_auto_20220316_2147.py` & `meta-edc-0.3.9/meta_prn/migrations/0021_auto_20220316_2147.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0022_auto_20220318_0133.py` & `meta-edc-0.3.9/meta_prn/migrations/0022_auto_20220318_0133.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0023_auto_20220415_1747.py` & `meta-edc-0.3.9/meta_prn/migrations/0023_auto_20220415_1747.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0024_alter_protocoldeviationviolation_violation.py` & `meta-edc-0.3.9/meta_prn/migrations/0024_alter_protocoldeviationviolation_violation.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0025_alter_historicalprotocoldeviationviolation_options_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0025_alter_historicalprotocoldeviationviolation_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0026_remove_historicalprotocoldeviationviolation_violation_type_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0026_remove_historicalprotocoldeviationviolation_violation_type_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0027_rename_historicalprotocoldeviationviolation_historicalprotocolincident_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0027_rename_historicalprotocoldeviationviolation_historicalprotocolincident_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0028_historicalpregnancynotification_bhcg_date_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0028_historicalpregnancynotification_bhcg_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0029_alter_historicalpregnancynotification_edd_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0029_alter_historicalpregnancynotification_edd_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0030_auto_20220627_1119.py` & `meta-edc-0.3.9/meta_prn/migrations/0030_auto_20220627_1119.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0031_alter_historicaloffschedule_options_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0031_alter_historicaloffschedule_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0032_historicalegfrnotification_egfrnotification.py` & `meta-edc-0.3.9/meta_prn/migrations/0032_historicalegfrnotification_egfrnotification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0033_remove_historicalegfrnotification_action_item_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0033_remove_historicalegfrnotification_action_item_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0034_auto_20220630_1110.py` & `meta-edc-0.3.9/meta_prn/migrations/0034_auto_20220630_1110.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0035_auto_20220630_1140.py` & `meta-edc-0.3.9/meta_prn/migrations/0035_auto_20220630_1140.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0036_remove_endofstudy_meta_prn_en_id_a50384_idx_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0036_remove_endofstudy_meta_prn_en_id_a50384_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0037_endofstudy_delivery_date_endofstudy_pregnancy_date_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0037_endofstudy_delivery_date_endofstudy_pregnancy_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0038_alter_endofstudy_delivery_date_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0038_alter_endofstudy_delivery_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0039_historicaloffstudymedication_reason_other_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0039_historicaloffstudymedication_reason_other_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0040_remove_historicaloffstudymedication_expected_restart_date_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0040_remove_historicaloffstudymedication_expected_restart_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0041_endofstudy_transfer_date_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0041_endofstudy_transfer_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0042_remove_endofstudy_investigator_decision_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0042_remove_endofstudy_investigator_decision_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0043_auto_20220704_1841.py` & `meta-edc-0.3.9/meta_prn/migrations/0043_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0044_alter_endofstudy_action_identifier_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0044_alter_endofstudy_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0045_auto_20220826_0258.py` & `meta-edc-0.3.9/meta_prn/migrations/0045_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0046_auto_20220826_0322.py` & `meta-edc-0.3.9/meta_prn/migrations/0046_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0047_auto_20220826_0406.py` & `meta-edc-0.3.9/meta_prn/migrations/0047_auto_20220826_0406.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0048_auto_20220922_2236.py` & `meta-edc-0.3.9/meta_prn/migrations/0048_auto_20220922_2236.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0049_auto_20220929_1742.py` & `meta-edc-0.3.9/meta_prn/migrations/0049_auto_20220929_1742.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0050_auto_20221004_0629.py` & `meta-edc-0.3.9/meta_prn/migrations/0050_auto_20221004_0629.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0051_historicalprotocolincident_reasons_withdrawn_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0051_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0052_alter_historicalprotocolincident_reasons_withdrawn_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0052_alter_historicalprotocolincident_reasons_withdrawn_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0053_alter_losstofollowup_options_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0053_alter_losstofollowup_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0054_alter_losstofollowup_options_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0054_alter_losstofollowup_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0055_alter_endofstudy_site_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0055_alter_endofstudy_site_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/migrations/0056_alter_endofstudy_clinical_withdrawal_reason_and_more.py` & `meta-edc-0.3.9/meta_prn/migrations/0056_alter_endofstudy_clinical_withdrawal_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/__init__.py` & `meta-edc-0.3.9/meta_prn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/end_of_study.py` & `meta-edc-0.3.9/meta_prn/models/end_of_study.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/loss_to_followup.py` & `meta-edc-0.3.9/meta_prn/models/loss_to_followup.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/off_study_medication.py` & `meta-edc-0.3.9/meta_prn/models/off_study_medication.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/offschedule.py` & `meta-edc-0.3.9/meta_prn/models/offschedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/onschedule.py` & `meta-edc-0.3.9/meta_prn/models/onschedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/pregnancy_notification.py` & `meta-edc-0.3.9/meta_prn/models/pregnancy_notification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/protocol_incident.py` & `meta-edc-0.3.9/meta_prn/models/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/models/signals.py` & `meta-edc-0.3.9/meta_prn/models/signals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/pregnancy_action_item_mixin.py` & `meta-edc-0.3.9/meta_prn/pregnancy_action_item_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/tests/tests/test_actions.py` & `meta-edc-0.3.9/meta_prn/tests/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/tests/tests/test_manager_order.py` & `meta-edc-0.3.9/meta_prn/tests/tests/test_manager_order.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_prn/tests/tests/test_pregnancy_notification.py` & `meta-edc-0.3.9/meta_prn/tests/tests/test_pregnancy_notification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_rando/migrations/0001_initial.py` & `meta-edc-0.3.9/meta_rando/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_rando/migrations/0002_auto_20220704_1841.py` & `meta-edc-0.3.9/meta_rando/migrations/0002_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_rando/migrations/0003_auto_20220826_1640.py` & `meta-edc-0.3.9/meta_rando/migrations/0003_auto_20220826_1640.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_rando/migrations/0004_alter_randomizationlist_options_and_more.py` & `meta-edc-0.3.9/meta_rando/migrations/0004_alter_randomizationlist_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_rando/migrations/0005_alter_randomizationlist_options_and_more.py` & `meta-edc-0.3.9/meta_rando/migrations/0005_alter_randomizationlist_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_rando/models.py` & `meta-edc-0.3.9/meta_rando/models.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_rando/randomizers.py` & `meta-edc-0.3.9/meta_rando/randomizers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_rando/tests/tests/test_randomizers.py` & `meta-edc-0.3.9/meta_rando/tests/tests/test_randomizers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_reports/apps.py` & `meta-edc-0.3.9/meta_reports/apps.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_reports/death_report.py` & `meta-edc-0.3.9/meta_reports/death_report.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_reports/pdf_report.py` & `meta-edc-0.3.9/meta_reports/pdf_report.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_reports/tests/holidays.csv` & `meta-edc-0.3.9/meta_reports/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_reports/tests/test_reports.py` & `meta-edc-0.3.9/meta_reports/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/admin/fieldsets.py` & `meta-edc-0.3.9/meta_screening/admin/fieldsets.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/admin/list_filters.py` & `meta-edc-0.3.9/meta_screening/admin/list_filters.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/admin/screening_part_one_admin.py` & `meta-edc-0.3.9/meta_screening/admin/screening_part_one_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/admin/screening_part_three_admin.py` & `meta-edc-0.3.9/meta_screening/admin/screening_part_three_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/admin/screening_part_two_admin.py` & `meta-edc-0.3.9/meta_screening/admin/screening_part_two_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/admin/subject_refusal_admin.py` & `meta-edc-0.3.9/meta_screening/admin/subject_refusal_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/admin/subject_screening_admin.py` & `meta-edc-0.3.9/meta_screening/admin/subject_screening_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/apps.py` & `meta-edc-0.3.9/meta_screening/apps.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/baker_recipes.py` & `meta-edc-0.3.9/meta_screening/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/calculators.py` & `meta-edc-0.3.9/meta_screening/calculators.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/choices.py` & `meta-edc-0.3.9/meta_screening/choices.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/constants.py` & `meta-edc-0.3.9/meta_screening/constants.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/eligibility/eligibility.py` & `meta-edc-0.3.9/meta_screening/eligibility/eligibility.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_one.py` & `meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_one.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_three/base_eligibility_part_three.py` & `meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_three/base_eligibility_part_three.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_three/eligibility_part_three_phase_three.py` & `meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_three/eligibility_part_three_phase_three.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/eligibility/eligibility_part_two.py` & `meta-edc-0.3.9/meta_screening/eligibility/eligibility_part_two.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/form_validators/screening_part_one.py` & `meta-edc-0.3.9/meta_screening/form_validators/screening_part_one.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/form_validators/screening_part_three.py` & `meta-edc-0.3.9/meta_screening/form_validators/screening_part_three.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/form_validators/screening_part_two.py` & `meta-edc-0.3.9/meta_screening/form_validators/screening_part_two.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/forms/__init__.py` & `meta-edc-0.3.9/meta_screening/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/forms/field_lists.py` & `meta-edc-0.3.9/meta_screening/forms/field_lists.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/forms/screening_part_one_form.py` & `meta-edc-0.3.9/meta_screening/forms/screening_part_one_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/forms/screening_part_three_form.py` & `meta-edc-0.3.9/meta_screening/forms/screening_part_three_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/forms/screening_part_two_form.py` & `meta-edc-0.3.9/meta_screening/forms/screening_part_two_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/forms/subject_refusal_form.py` & `meta-edc-0.3.9/meta_screening/forms/subject_refusal_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/forms/subject_screening_form.py` & `meta-edc-0.3.9/meta_screening/forms/subject_screening_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0001_initial.py` & `meta-edc-0.3.9/meta_screening/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0002_auto_20191020_0612.py` & `meta-edc-0.3.9/meta_screening/migrations/0002_auto_20191020_0612.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0003_auto_20191020_0627.py` & `meta-edc-0.3.9/meta_screening/migrations/0003_auto_20191020_0627.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0004_auto_20191020_0738.py` & `meta-edc-0.3.9/meta_screening/migrations/0004_auto_20191020_0738.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0005_auto_20191021_0353.py` & `meta-edc-0.3.9/meta_screening/migrations/0005_auto_20191021_0353.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0006_auto_20191022_0134.py` & `meta-edc-0.3.9/meta_screening/migrations/0006_auto_20191022_0134.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0007_auto_20191024_1000.py` & `meta-edc-0.3.9/meta_screening/migrations/0007_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0008_auto_20191031_0745.py` & `meta-edc-0.3.9/meta_screening/migrations/0008_auto_20191031_0745.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0009_auto_20191105_0122.py` & `meta-edc-0.3.9/meta_screening/migrations/0009_auto_20191105_0122.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0010_auto_20191106_0828.py` & `meta-edc-0.3.9/meta_screening/migrations/0010_auto_20191106_0828.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0011_auto_20191107_0342.py` & `meta-edc-0.3.9/meta_screening/migrations/0011_auto_20191107_0342.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0012_auto_20191107_0427.py` & `meta-edc-0.3.9/meta_screening/migrations/0012_auto_20191107_0427.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0013_auto_20191107_0442.py` & `meta-edc-0.3.9/meta_screening/migrations/0013_auto_20191107_0442.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0014_auto_20191107_0528.py` & `meta-edc-0.3.9/meta_screening/migrations/0014_auto_20191107_0528.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0015_auto_20191107_2249.py` & `meta-edc-0.3.9/meta_screening/migrations/0015_auto_20191107_2249.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0016_auto_20191119_2331.py` & `meta-edc-0.3.9/meta_screening/migrations/0016_auto_20191119_2331.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0017_auto_20191213_0314.py` & `meta-edc-0.3.9/meta_screening/migrations/0017_auto_20191213_0314.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0018_auto_20200118_1854.py` & `meta-edc-0.3.9/meta_screening/migrations/0018_auto_20200118_1854.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0019_auto_20200120_2256.py` & `meta-edc-0.3.9/meta_screening/migrations/0019_auto_20200120_2256.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0020_auto_20200524_1944.py` & `meta-edc-0.3.9/meta_screening/migrations/0020_auto_20200524_1944.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0021_auto_20210628_2105.py` & `meta-edc-0.3.9/meta_screening/migrations/0021_auto_20210628_2105.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0022_auto_20210702_0426.py` & `meta-edc-0.3.9/meta_screening/migrations/0022_auto_20210702_0426.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0023_auto_20210702_0533.py` & `meta-edc-0.3.9/meta_screening/migrations/0023_auto_20210702_0533.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0024_auto_20210710_1929.py` & `meta-edc-0.3.9/meta_screening/migrations/0024_auto_20210710_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0025_auto_20210710_2247.py` & `meta-edc-0.3.9/meta_screening/migrations/0025_auto_20210710_2247.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0026_auto_20210712_0433.py` & `meta-edc-0.3.9/meta_screening/migrations/0026_auto_20210712_0433.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0028_auto_20210823_2353.py` & `meta-edc-0.3.9/meta_screening/migrations/0028_auto_20210823_2353.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0029_auto_20211123_1645.py` & `meta-edc-0.3.9/meta_screening/migrations/0029_auto_20211123_1645.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0030_auto_20220128_1719.py` & `meta-edc-0.3.9/meta_screening/migrations/0030_auto_20220128_1719.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0031_auto_20220304_0448.py` & `meta-edc-0.3.9/meta_screening/migrations/0031_auto_20220304_0448.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0032_auto_20220304_0501.py` & `meta-edc-0.3.9/meta_screening/migrations/0032_auto_20220304_0501.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0033_auto_20220304_0504.py` & `meta-edc-0.3.9/meta_screening/migrations/0033_auto_20220304_0504.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0034_auto_20220304_0508.py` & `meta-edc-0.3.9/meta_screening/migrations/0034_auto_20220304_0508.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0035_auto_20220304_2233.py` & `meta-edc-0.3.9/meta_screening/migrations/0035_auto_20220304_2233.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0036_auto_20220304_2307.py` & `meta-edc-0.3.9/meta_screening/migrations/0036_auto_20220304_2307.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0037_auto_20220312_0339.py` & `meta-edc-0.3.9/meta_screening/migrations/0037_auto_20220312_0339.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0038_auto_20220312_1929.py` & `meta-edc-0.3.9/meta_screening/migrations/0038_auto_20220312_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0039_auto_20220312_1938.py` & `meta-edc-0.3.9/meta_screening/migrations/0039_auto_20220312_1938.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0040_auto_20220316_2147.py` & `meta-edc-0.3.9/meta_screening/migrations/0040_auto_20220316_2147.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0041_auto_20220403_1227.py` & `meta-edc-0.3.9/meta_screening/migrations/0041_auto_20220403_1227.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0042_auto_20220403_1402.py` & `meta-edc-0.3.9/meta_screening/migrations/0042_auto_20220403_1402.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0043_auto_20220407_1713.py` & `meta-edc-0.3.9/meta_screening/migrations/0043_auto_20220407_1713.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0044_alter_historicalscreeningpartone_severe_htn_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0044_alter_historicalscreeningpartone_severe_htn_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0045_historicalscreeningpartone_contact_number_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0045_historicalscreeningpartone_contact_number_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0046_historicalscreeningpartone_hba1c_datetime_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0046_historicalscreeningpartone_hba1c_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0047_historicalscreeningpartone_appt_datetime_repeat_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0047_historicalscreeningpartone_appt_datetime_repeat_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0048_rename_appt_datetime_repeat_historicalscreeningpartone_repeat_appt_datetime_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0048_rename_appt_datetime_repeat_historicalscreeningpartone_repeat_appt_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0049_historicalscreeningpartone_p3_ltfu_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0049_historicalscreeningpartone_p3_ltfu_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0050_historicalscreeningpartone_agree_to_p3_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0050_historicalscreeningpartone_agree_to_p3_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0051_alter_historicalscreeningpartone_advised_to_fast_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0051_alter_historicalscreeningpartone_advised_to_fast_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0052_alter_historicalscreeningpartone_p3_ltfu_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0052_alter_historicalscreeningpartone_p3_ltfu_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0053_auto_20220704_1841.py` & `meta-edc-0.3.9/meta_screening/migrations/0053_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0054_auto_20220722_2130.py` & `meta-edc-0.3.9/meta_screening/migrations/0054_auto_20220722_2130.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0055_alter_historicalscreeningpartone_creatinine_value_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0055_alter_historicalscreeningpartone_creatinine_value_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0056_alter_historicalscreeningpartone_agree_to_p3_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0056_alter_historicalscreeningpartone_agree_to_p3_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0057_alter_historicalscreeningpartone_calculated_egfr_value_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0057_alter_historicalscreeningpartone_calculated_egfr_value_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0058_alter_historicalscreeningpartone_eligibility_datetime_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0058_alter_historicalscreeningpartone_eligibility_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0059_alter_icpreferral_managers_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0059_alter_icpreferral_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0060_historicalicpreferral_locale_created_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0060_historicalicpreferral_locale_created_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0061_alter_historicalicpreferral_site_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0061_alter_historicalicpreferral_site_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/migrations/0062_remove_icpreferral_site_and_more.py` & `meta-edc-0.3.9/meta_screening/migrations/0062_remove_icpreferral_site_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/model_mixins/calculated_model_mixin.py` & `meta-edc-0.3.9/meta_screening/model_mixins/calculated_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/model_mixins/creatinine_fields_model_mixin.py` & `meta-edc-0.3.9/meta_screening/model_mixins/creatinine_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/model_mixins/eligibility_model_mixin.py` & `meta-edc-0.3.9/meta_screening/model_mixins/eligibility_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/model_mixins/part_one_fields_model_mixin.py` & `meta-edc-0.3.9/meta_screening/model_mixins/part_one_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/model_mixins/part_three_fields_model_mixin.py` & `meta-edc-0.3.9/meta_screening/model_mixins/part_three_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/model_mixins/part_two_fields_model_mixin.py` & `meta-edc-0.3.9/meta_screening/model_mixins/part_two_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/models/icp_referral.py` & `meta-edc-0.3.9/meta_screening/models/icp_referral.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/models/proxy_models.py` & `meta-edc-0.3.9/meta_screening/models/proxy_models.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/models/signals.py` & `meta-edc-0.3.9/meta_screening/models/signals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/models/subject_refusal.py` & `meta-edc-0.3.9/meta_screening/models/subject_refusal.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/models/subject_screening.py` & `meta-edc-0.3.9/meta_screening/models/subject_screening.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/tests/holidays.csv` & `meta-edc-0.3.9/meta_screening/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/tests/meta_test_case_mixin.py` & `meta-edc-0.3.9/meta_screening/tests/meta_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/tests/options.py` & `meta-edc-0.3.9/meta_screening/tests/options.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/tests/tests/test_forms.py` & `meta-edc-0.3.9/meta_screening/tests/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/tests/tests/test_screening_part_one.py` & `meta-edc-0.3.9/meta_screening/tests/tests/test_screening_part_one.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/tests/tests/test_screening_part_three.py` & `meta-edc-0.3.9/meta_screening/tests/tests/test_screening_part_three.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_screening/tests/tests/test_screening_part_two.py` & `meta-edc-0.3.9/meta_screening/tests/tests/test_screening_part_two.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_sites/sites.py` & `meta-edc-0.3.9/meta_sites/sites.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_stats/incidence.py` & `meta-edc-0.3.9/meta_stats/incidence.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/action_items.py` & `meta-edc-0.3.9/meta_subject/action_items.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/__init__.py` & `meta-edc-0.3.9/meta_subject/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/autocomplete_admin.py` & `meta-edc-0.3.9/meta_subject/admin/autocomplete_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/birth_outcome_admin.py` & `meta-edc-0.3.9/meta_subject/admin/birth_outcome_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_fbc_admin.py` & `meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_fbc_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_hba1c_admin.py` & `meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_hba1c_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_ins_admin.py` & `meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_ins_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_lft_admin.py` & `meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_lft_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_lipid_admin.py` & `meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_lipid_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/blood_results/blood_results_rft_admin.py` & `meta-edc-0.3.9/meta_subject/admin/blood_results/blood_results_rft_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/complications_admin.py` & `meta-edc-0.3.9/meta_subject/admin/complications_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/complications_glycemia_admin.py` & `meta-edc-0.3.9/meta_subject/admin/complications_glycemia_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/concomitant_medication_admin.py` & `meta-edc-0.3.9/meta_subject/admin/concomitant_medication_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/delivery_admin.py` & `meta-edc-0.3.9/meta_subject/admin/delivery_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/dm_referral_followup_admin.py` & `meta-edc-0.3.9/meta_subject/admin/dm_referral_followup_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/egfr_drop_notification_admin.py` & `meta-edc-0.3.9/meta_subject/admin/egfr_drop_notification_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/eq5d3l_admin.py` & `meta-edc-0.3.9/meta_subject/admin/eq5d3l_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/fieldsets.py` & `meta-edc-0.3.9/meta_subject/admin/fieldsets.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/followup_examination_admin.py` & `meta-edc-0.3.9/meta_subject/admin/followup_examination_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/followup_vitals_admin.py` & `meta-edc-0.3.9/meta_subject/admin/followup_vitals_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/glucose_admin.py` & `meta-edc-0.3.9/meta_subject/admin/glucose_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/glucose_fbg_admin.py` & `meta-edc-0.3.9/meta_subject/admin/glucose_fbg_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/health_economics/health_economics_simple_admin.py` & `meta-edc-0.3.9/meta_subject/admin/health_economics/health_economics_simple_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/health_economics/health_economics_update_admin.py` & `meta-edc-0.3.9/meta_subject/admin/health_economics/health_economics_update_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/hepatitis_test_admin.py` & `meta-edc-0.3.9/meta_subject/admin/hepatitis_test_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/list_filters.py` & `meta-edc-0.3.9/meta_subject/admin/list_filters.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/medication_adherence_admin.py` & `meta-edc-0.3.9/meta_subject/admin/medication_adherence_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/mnsi_admin.py` & `meta-edc-0.3.9/meta_subject/admin/mnsi_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/other_arv_regimens_admin.py` & `meta-edc-0.3.9/meta_subject/admin/other_arv_regimens_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/patient_history_admin.py` & `meta-edc-0.3.9/meta_subject/admin/patient_history_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/physical_exam_admin.py` & `meta-edc-0.3.9/meta_subject/admin/physical_exam_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/pregnancy_update_admin.py` & `meta-edc-0.3.9/meta_subject/admin/pregnancy_update_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/sf12_admin.py` & `meta-edc-0.3.9/meta_subject/admin/sf12_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/study_medication_admin.py` & `meta-edc-0.3.9/meta_subject/admin/study_medication_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/subject_requisition_admin.py` & `meta-edc-0.3.9/meta_subject/admin/subject_requisition_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/subject_visit_admin.py` & `meta-edc-0.3.9/meta_subject/admin/subject_visit_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/subject_visit_missed_admin.py` & `meta-edc-0.3.9/meta_subject/admin/subject_visit_missed_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/urine_dipstick_test_admin.py` & `meta-edc-0.3.9/meta_subject/admin/urine_dipstick_test_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/admin/urine_pregnancy_admin.py` & `meta-edc-0.3.9/meta_subject/admin/urine_pregnancy_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/baker_recipes.py` & `meta-edc-0.3.9/meta_subject/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/choices.py` & `meta-edc-0.3.9/meta_subject/choices.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/constants.py` & `meta-edc-0.3.9/meta_subject/constants.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/form_validators/delivery_form_validator.py` & `meta-edc-0.3.9/meta_subject/form_validators/delivery_form_validator.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/form_validators/dm_referral_followup_form_validator.py` & `meta-edc-0.3.9/meta_subject/form_validators/dm_referral_followup_form_validator.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/form_validators/egfr_drop_notification_form_validator.py` & `meta-edc-0.3.9/meta_subject/form_validators/egfr_drop_notification_form_validator.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/form_validators/followup_examination_form_validator.py` & `meta-edc-0.3.9/meta_subject/form_validators/followup_examination_form_validator.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/form_validators/glucose_form_validator.py` & `meta-edc-0.3.9/meta_subject/form_validators/glucose_form_validator.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/__init__.py` & `meta-edc-0.3.9/meta_subject/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_fbc_form.py` & `meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_fbc_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_hba1c_form.py` & `meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_hba1c_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_ins_form.py` & `meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_ins_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_lft_form.py` & `meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_lft_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_lipid_form.py` & `meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_lipid_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/blood_results/blood_results_rft_form.py` & `meta-edc-0.3.9/meta_subject/forms/blood_results/blood_results_rft_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/dm_referral_followup.py` & `meta-edc-0.3.9/meta_subject/forms/dm_referral_followup.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/glucose_fbg_form.py` & `meta-edc-0.3.9/meta_subject/forms/glucose_fbg_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/hepatitis_test_form.py` & `meta-edc-0.3.9/meta_subject/forms/hepatitis_test_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/medication_adherence_form.py` & `meta-edc-0.3.9/meta_subject/forms/medication_adherence_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/mixins.py` & `meta-edc-0.3.9/meta_subject/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/other_arv_regimens_detail_form.py` & `meta-edc-0.3.9/meta_subject/forms/other_arv_regimens_detail_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/other_arv_regimens_form.py` & `meta-edc-0.3.9/meta_subject/forms/other_arv_regimens_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/patient_history_form.py` & `meta-edc-0.3.9/meta_subject/forms/patient_history_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/physical_exam_form.py` & `meta-edc-0.3.9/meta_subject/forms/physical_exam_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/pregnancy_update_form.py` & `meta-edc-0.3.9/meta_subject/forms/pregnancy_update_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/slider_widget.py` & `meta-edc-0.3.9/meta_subject/forms/slider_widget.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/study_medication_form.py` & `meta-edc-0.3.9/meta_subject/forms/study_medication_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/subject_requisition_form.py` & `meta-edc-0.3.9/meta_subject/forms/subject_requisition_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/subject_visit_form.py` & `meta-edc-0.3.9/meta_subject/forms/subject_visit_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/subject_visit_missed_form.py` & `meta-edc-0.3.9/meta_subject/forms/subject_visit_missed_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/urine_dipstick_test_form.py` & `meta-edc-0.3.9/meta_subject/forms/urine_dipstick_test_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/forms/urine_pregnancy_form.py` & `meta-edc-0.3.9/meta_subject/forms/urine_pregnancy_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/locale/sw/LC_MESSAGES/django.po` & `meta-edc-0.3.9/meta_subject/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/management/commands/create_missing_refills.py` & `meta-edc-0.3.9/meta_subject/management/commands/create_missing_refills.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/management/commands/create_missing_rx.py` & `meta-edc-0.3.9/meta_subject/management/commands/create_missing_rx.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/management/commands/missed.py` & `meta-edc-0.3.9/meta_subject/management/commands/missed.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/metadata_rules/metadata_rules.py` & `meta-edc-0.3.9/meta_subject/metadata_rules/metadata_rules.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/metadata_rules/predicates.py` & `meta-edc-0.3.9/meta_subject/metadata_rules/predicates.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0001_initial.py` & `meta-edc-0.3.9/meta_subject/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0002_auto_20191021_0353.py` & `meta-edc-0.3.9/meta_subject/migrations/0002_auto_20191021_0353.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0003_auto_20191021_0534.py` & `meta-edc-0.3.9/meta_subject/migrations/0003_auto_20191021_0534.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0004_auto_20191022_0134.py` & `meta-edc-0.3.9/meta_subject/migrations/0004_auto_20191022_0134.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0005_auto_20191024_1000.py` & `meta-edc-0.3.9/meta_subject/migrations/0005_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0006_auto_20191104_0756.py` & `meta-edc-0.3.9/meta_subject/migrations/0006_auto_20191104_0756.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0007_auto_20191107_2249.py` & `meta-edc-0.3.9/meta_subject/migrations/0007_auto_20191107_2249.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0008_auto_20191115_0132.py` & `meta-edc-0.3.9/meta_subject/migrations/0008_auto_20191115_0132.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0009_auto_20191119_2331.py` & `meta-edc-0.3.9/meta_subject/migrations/0009_auto_20191119_2331.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0010_auto_20191213_0314.py` & `meta-edc-0.3.9/meta_subject/migrations/0010_auto_20191213_0314.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0011_auto_20200118_1854.py` & `meta-edc-0.3.9/meta_subject/migrations/0011_auto_20200118_1854.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0012_auto_20200118_2334.py` & `meta-edc-0.3.9/meta_subject/migrations/0012_auto_20200118_2334.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0013_auto_20200119_0013.py` & `meta-edc-0.3.9/meta_subject/migrations/0013_auto_20200119_0013.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0014_auto_20200120_1622.py` & `meta-edc-0.3.9/meta_subject/migrations/0014_auto_20200120_1622.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0015_auto_20200120_1943.py` & `meta-edc-0.3.9/meta_subject/migrations/0015_auto_20200120_1943.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0016_auto_20200123_1508.py` & `meta-edc-0.3.9/meta_subject/migrations/0016_auto_20200123_1508.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0017_auto_20200325_0901.py` & `meta-edc-0.3.9/meta_subject/migrations/0017_auto_20200325_0901.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0018_coronakap_historicalcoronakap.py` & `meta-edc-0.3.9/meta_subject/migrations/0018_coronakap_historicalcoronakap.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0019_auto_20200417_0315.py` & `meta-edc-0.3.9/meta_subject/migrations/0019_auto_20200417_0315.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0020_auto_20200417_0329.py` & `meta-edc-0.3.9/meta_subject/migrations/0020_auto_20200417_0329.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0021_auto_20200417_0332.py` & `meta-edc-0.3.9/meta_subject/migrations/0021_auto_20200417_0332.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0022_auto_20200419_2223.py` & `meta-edc-0.3.9/meta_subject/migrations/0022_auto_20200419_2223.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0023_auto_20200419_2305.py` & `meta-edc-0.3.9/meta_subject/migrations/0023_auto_20200419_2305.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0024_auto_20200419_2331.py` & `meta-edc-0.3.9/meta_subject/migrations/0024_auto_20200419_2331.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0025_auto_20200420_1455.py` & `meta-edc-0.3.9/meta_subject/migrations/0025_auto_20200420_1455.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0026_auto_20200420_1524.py` & `meta-edc-0.3.9/meta_subject/migrations/0026_auto_20200420_1524.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0027_auto_20200420_1645.py` & `meta-edc-0.3.9/meta_subject/migrations/0027_auto_20200420_1645.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0028_auto_20200420_1732.py` & `meta-edc-0.3.9/meta_subject/migrations/0028_auto_20200420_1732.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0029_auto_20200420_1751.py` & `meta-edc-0.3.9/meta_subject/migrations/0029_auto_20200420_1751.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0030_auto_20200420_1816.py` & `meta-edc-0.3.9/meta_subject/migrations/0030_auto_20200420_1816.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0031_auto_20200422_2039.py` & `meta-edc-0.3.9/meta_subject/migrations/0031_auto_20200422_2039.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0032_auto_20200515_0307.py` & `meta-edc-0.3.9/meta_subject/migrations/0032_auto_20200515_0307.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0033_auto_20200516_2356.py` & `meta-edc-0.3.9/meta_subject/migrations/0033_auto_20200516_2356.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0034_auto_20200517_0125.py` & `meta-edc-0.3.9/meta_subject/migrations/0034_auto_20200517_0125.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0035_auto_20200517_0128.py` & `meta-edc-0.3.9/meta_subject/migrations/0035_auto_20200517_0128.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0036_auto_20200517_0150.py` & `meta-edc-0.3.9/meta_subject/migrations/0036_auto_20200517_0150.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0037_auto_20200517_0207.py` & `meta-edc-0.3.9/meta_subject/migrations/0037_auto_20200517_0207.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0038_auto_20200520_0020.py` & `meta-edc-0.3.9/meta_subject/migrations/0038_auto_20200520_0020.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0039_auto_20200524_1944.py` & `meta-edc-0.3.9/meta_subject/migrations/0039_auto_20200524_1944.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0040_auto_20200527_2155.py` & `meta-edc-0.3.9/meta_subject/migrations/0040_auto_20200527_2155.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0041_auto_20200528_0242.py` & `meta-edc-0.3.9/meta_subject/migrations/0041_auto_20200528_0242.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0043_auto_20200528_1555.py` & `meta-edc-0.3.9/meta_subject/migrations/0043_auto_20200528_1555.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0044_auto_20200528_1853.py` & `meta-edc-0.3.9/meta_subject/migrations/0044_auto_20200528_1853.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0045_auto_20200530_1801.py` & `meta-edc-0.3.9/meta_subject/migrations/0045_auto_20200530_1801.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0046_auto_20200530_1804.py` & `meta-edc-0.3.9/meta_subject/migrations/0046_auto_20200530_1804.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0047_auto_20200530_1819.py` & `meta-edc-0.3.9/meta_subject/migrations/0047_auto_20200530_1819.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0050_auto_20200614_1934.py` & `meta-edc-0.3.9/meta_subject/migrations/0050_auto_20200614_1934.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0051_auto_20200617_2117.py` & `meta-edc-0.3.9/meta_subject/migrations/0051_auto_20200617_2117.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0052_auto_20210624_0225.py` & `meta-edc-0.3.9/meta_subject/migrations/0052_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0053_auto_20210628_2105.py` & `meta-edc-0.3.9/meta_subject/migrations/0053_auto_20210628_2105.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0054_auto_20210628_2314.py` & `meta-edc-0.3.9/meta_subject/migrations/0054_auto_20210628_2314.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0055_auto_20210628_2331.py` & `meta-edc-0.3.9/meta_subject/migrations/0055_auto_20210628_2331.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0056_auto_20210702_0426.py` & `meta-edc-0.3.9/meta_subject/migrations/0056_auto_20210702_0426.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0057_auto_20210702_0458.py` & `meta-edc-0.3.9/meta_subject/migrations/0057_auto_20210702_0458.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0058_auto_20210702_0533.py` & `meta-edc-0.3.9/meta_subject/migrations/0058_auto_20210702_0533.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0059_auto_20210709_2056.py` & `meta-edc-0.3.9/meta_subject/migrations/0059_auto_20210709_2056.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0060_auto_20210709_2241.py` & `meta-edc-0.3.9/meta_subject/migrations/0060_auto_20210709_2241.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0061_auto_20210710_1929.py` & `meta-edc-0.3.9/meta_subject/migrations/0061_auto_20210710_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0062_auto_20210713_0616.py` & `meta-edc-0.3.9/meta_subject/migrations/0062_auto_20210713_0616.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0063_auto_20210715_0337.py` & `meta-edc-0.3.9/meta_subject/migrations/0063_auto_20210715_0337.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0064_auto_20210715_2336.py` & `meta-edc-0.3.9/meta_subject/migrations/0064_auto_20210715_2336.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0065_auto_20210716_0813.py` & `meta-edc-0.3.9/meta_subject/migrations/0065_auto_20210716_0813.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0066_auto_20210721_0335.py` & `meta-edc-0.3.9/meta_subject/migrations/0066_auto_20210721_0335.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0067_auto_20210726_0340.py` & `meta-edc-0.3.9/meta_subject/migrations/0067_auto_20210726_0340.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0068_auto_20210728_1809.py` & `meta-edc-0.3.9/meta_subject/migrations/0068_auto_20210728_1809.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0069_auto_20210801_2021.py` & `meta-edc-0.3.9/meta_subject/migrations/0069_auto_20210801_2021.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0070_auto_20210804_0438.py` & `meta-edc-0.3.9/meta_subject/migrations/0070_auto_20210804_0438.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0071_auto_20210804_0715.py` & `meta-edc-0.3.9/meta_subject/migrations/0071_auto_20210804_0715.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0072_auto_20210805_1545.py` & `meta-edc-0.3.9/meta_subject/migrations/0072_auto_20210805_1545.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0073_auto_20210809_0055.py` & `meta-edc-0.3.9/meta_subject/migrations/0073_auto_20210809_0055.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0075_auto_20210809_1744.py` & `meta-edc-0.3.9/meta_subject/migrations/0075_auto_20210809_1744.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0076_auto_20210809_1854.py` & `meta-edc-0.3.9/meta_subject/migrations/0076_auto_20210809_1854.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0077_auto_20210809_2323.py` & `meta-edc-0.3.9/meta_subject/migrations/0077_auto_20210809_2323.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0078_auto_20210810_0857.py` & `meta-edc-0.3.9/meta_subject/migrations/0078_auto_20210810_0857.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0079_auto_20210812_0335.py` & `meta-edc-0.3.9/meta_subject/migrations/0079_auto_20210812_0335.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0080_auto_20210812_0400.py` & `meta-edc-0.3.9/meta_subject/migrations/0080_auto_20210812_0400.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0081_auto_20210817_2306.py` & `meta-edc-0.3.9/meta_subject/migrations/0081_auto_20210817_2306.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0082_auto_20210823_1612.py` & `meta-edc-0.3.9/meta_subject/migrations/0082_auto_20210823_1612.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0083_auto_20210823_1620.py` & `meta-edc-0.3.9/meta_subject/migrations/0083_auto_20210823_1620.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0084_auto_20210910_0234.py` & `meta-edc-0.3.9/meta_subject/migrations/0084_auto_20210910_0234.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0085_auto_20210911_2036.py` & `meta-edc-0.3.9/meta_subject/migrations/0085_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0086_auto_20210920_0229.py` & `meta-edc-0.3.9/meta_subject/migrations/0086_auto_20210920_0229.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0087_auto_20210922_2058.py` & `meta-edc-0.3.9/meta_subject/migrations/0087_auto_20210922_2058.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0088_auto_20210924_0027.py` & `meta-edc-0.3.9/meta_subject/migrations/0088_auto_20210924_0027.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0089_auto_20210924_0121.py` & `meta-edc-0.3.9/meta_subject/migrations/0089_auto_20210924_0121.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0090_auto_20210924_0424.py` & `meta-edc-0.3.9/meta_subject/migrations/0090_auto_20210924_0424.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0091_auto_20210929_2324.py` & `meta-edc-0.3.9/meta_subject/migrations/0091_auto_20210929_2324.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0092_auto_20211013_0447.py` & `meta-edc-0.3.9/meta_subject/migrations/0092_auto_20211013_0447.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0093_auto_20211117_0352.py` & `meta-edc-0.3.9/meta_subject/migrations/0093_auto_20211117_0352.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0094_auto_20211123_1645.py` & `meta-edc-0.3.9/meta_subject/migrations/0094_auto_20211123_1645.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0095_auto_20220128_1719.py` & `meta-edc-0.3.9/meta_subject/migrations/0095_auto_20220128_1719.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0096_auto_20220304_0501.py` & `meta-edc-0.3.9/meta_subject/migrations/0096_auto_20220304_0501.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0097_auto_20220304_2233.py` & `meta-edc-0.3.9/meta_subject/migrations/0097_auto_20220304_2233.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0098_auto_20220309_2106.py` & `meta-edc-0.3.9/meta_subject/migrations/0098_auto_20220309_2106.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0099_auto_20220309_2218.py` & `meta-edc-0.3.9/meta_subject/migrations/0099_auto_20220309_2218.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0100_auto_20220309_2238.py` & `meta-edc-0.3.9/meta_subject/migrations/0100_auto_20220309_2238.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0101_auto_20220316_2147.py` & `meta-edc-0.3.9/meta_subject/migrations/0101_auto_20220316_2147.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0102_auto_20220324_0304.py` & `meta-edc-0.3.9/meta_subject/migrations/0102_auto_20220324_0304.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0103_auto_20220324_0326.py` & `meta-edc-0.3.9/meta_subject/migrations/0103_auto_20220324_0326.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0104_auto_20220412_2151.py` & `meta-edc-0.3.9/meta_subject/migrations/0104_auto_20220412_2151.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0105_auto_20220412_2310.py` & `meta-edc-0.3.9/meta_subject/migrations/0105_auto_20220412_2310.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0106_auto_20220414_1741.py` & `meta-edc-0.3.9/meta_subject/migrations/0106_auto_20220414_1741.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0107_auto_20220415_0043.py` & `meta-edc-0.3.9/meta_subject/migrations/0107_auto_20220415_0043.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0108_auto_20220415_1747.py` & `meta-edc-0.3.9/meta_subject/migrations/0108_auto_20220415_1747.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0109_auto_20220415_1758.py` & `meta-edc-0.3.9/meta_subject/migrations/0109_auto_20220415_1758.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0110_auto_20220512_1811.py` & `meta-edc-0.3.9/meta_subject/migrations/0110_auto_20220512_1811.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0111_alter_followupvitals_severe_htn_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0111_alter_followupvitals_severe_htn_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0112_historicalsubjectvisit_document_status_comments_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0112_historicalsubjectvisit_document_status_comments_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0113_bloodresultsrft_egfr_percent_change_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0113_bloodresultsrft_egfr_percent_change_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0114_alter_bloodresultsrft_egfr_percent_change_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0114_alter_bloodresultsrft_egfr_percent_change_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0115_historicalegfrnotification_egfrnotification.py` & `meta-edc-0.3.9/meta_subject/migrations/0115_historicalegfrnotification_egfrnotification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0116_egfrnotification_report_status_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0116_egfrnotification_report_status_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0117_alter_egfrnotification_managers_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0117_alter_egfrnotification_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0118_delivery_crf_status_delivery_crf_status_comments_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0118_delivery_crf_status_delivery_crf_status_comments_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0119_historicalstudymedication_roundup_divisible_by_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0119_historicalstudymedication_roundup_divisible_by_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0120_alter_birthoutcomes_managers_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0120_alter_birthoutcomes_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0121_auto_20220704_1841.py` & `meta-edc-0.3.9/meta_subject/migrations/0121_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0122_auto_20220708_2144.py` & `meta-edc-0.3.9/meta_subject/migrations/0122_auto_20220708_2144.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0123_auto_20220714_2136.py` & `meta-edc-0.3.9/meta_subject/migrations/0123_auto_20220714_2136.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0124_auto_20220714_2303.py` & `meta-edc-0.3.9/meta_subject/migrations/0124_auto_20220714_2303.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0125_auto_20220719_2134.py` & `meta-edc-0.3.9/meta_subject/migrations/0125_auto_20220719_2134.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0126_auto_20220719_2142.py` & `meta-edc-0.3.9/meta_subject/migrations/0126_auto_20220719_2142.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0127_auto_20220720_0053.py` & `meta-edc-0.3.9/meta_subject/migrations/0127_auto_20220720_0053.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0128_auto_20220720_0055.py` & `meta-edc-0.3.9/meta_subject/migrations/0128_auto_20220720_0055.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0130_auto_20220720_0216.py` & `meta-edc-0.3.9/meta_subject/migrations/0130_auto_20220720_0216.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0131_auto_20220722_0411.py` & `meta-edc-0.3.9/meta_subject/migrations/0131_auto_20220722_0411.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0132_auto_20220722_1825.py` & `meta-edc-0.3.9/meta_subject/migrations/0132_auto_20220722_1825.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0133_auto_20220722_2140.py` & `meta-edc-0.3.9/meta_subject/migrations/0133_auto_20220722_2140.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0134_auto_20220722_2211.py` & `meta-edc-0.3.9/meta_subject/migrations/0134_auto_20220722_2211.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0135_auto_20220722_2212.py` & `meta-edc-0.3.9/meta_subject/migrations/0135_auto_20220722_2212.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0136_egfrdropnotification_creatinine_quantifier_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0136_egfrdropnotification_creatinine_quantifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0137_alter_egfrdropnotification_egfr_percent_change_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0137_alter_egfrdropnotification_egfr_percent_change_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0138_alter_glucose_fbg_datetime_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0138_alter_glucose_fbg_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0139_alter_bloodresultsins_ins_units_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0139_alter_bloodresultsins_ins_units_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0140_alter_bloodresultsfbc_action_identifier_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0140_alter_bloodresultsfbc_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0141_auto_20220826_0258.py` & `meta-edc-0.3.9/meta_subject/migrations/0141_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0142_auto_20220826_0322.py` & `meta-edc-0.3.9/meta_subject/migrations/0142_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0143_auto_20220826_0406.py` & `meta-edc-0.3.9/meta_subject/migrations/0143_auto_20220826_0406.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0144_auto_20220907_0157.py` & `meta-edc-0.3.9/meta_subject/migrations/0144_auto_20220907_0157.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0145_auto_20220907_0202.py` & `meta-edc-0.3.9/meta_subject/migrations/0145_auto_20220907_0202.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0146_auto_20220907_0207.py` & `meta-edc-0.3.9/meta_subject/migrations/0146_auto_20220907_0207.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0147_auto_20220907_1505.py` & `meta-edc-0.3.9/meta_subject/migrations/0147_auto_20220907_1505.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0148_auto_20220908_1826.py` & `meta-edc-0.3.9/meta_subject/migrations/0148_auto_20220908_1826.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0149_auto_20220913_2139.py` & `meta-edc-0.3.9/meta_subject/migrations/0149_auto_20220913_2139.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0150_auto_20220914_0039.py` & `meta-edc-0.3.9/meta_subject/migrations/0150_auto_20220914_0039.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0151_auto_20220918_0508.py` & `meta-edc-0.3.9/meta_subject/migrations/0151_auto_20220918_0508.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0152_auto_20220925_0509.py` & `meta-edc-0.3.9/meta_subject/migrations/0152_auto_20220925_0509.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0153_auto_20220928_0250.py` & `meta-edc-0.3.9/meta_subject/migrations/0153_auto_20220928_0250.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0154_auto_20220928_0419.py` & `meta-edc-0.3.9/meta_subject/migrations/0154_auto_20220928_0419.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0155_auto_20220929_1742.py` & `meta-edc-0.3.9/meta_subject/migrations/0155_auto_20220929_1742.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0156_alter_bloodresultsfbc_assay_datetime_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0156_alter_bloodresultsfbc_assay_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0157_remove_bloodresultsfbc_crf_status_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0157_remove_bloodresultsfbc_crf_status_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0158_alter_followupexamination_attended_clinic_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0158_alter_followupexamination_attended_clinic_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0159_alter_bloodresultsfbc_results_abnormal_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0159_alter_bloodresultsfbc_results_abnormal_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0160_alter_healtheconomicssimple_education_certificate_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0160_alter_healtheconomicssimple_education_certificate_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0161_alter_birthoutcomes_options_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0161_alter_birthoutcomes_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0162_alter_followupexamination_abdominal_tenderness_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0162_alter_followupexamination_abdominal_tenderness_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0163_alter_birthoutcomes_options_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0163_alter_birthoutcomes_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0164_dmreferralfollowup_historicaldmreferralfollowup.py` & `meta-edc-0.3.9/meta_subject/migrations/0164_dmreferralfollowup_historicaldmreferralfollowup.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0165_alter_dmreferralfollowup_healthcare_workers.py` & `meta-edc-0.3.9/meta_subject/migrations/0165_alter_dmreferralfollowup_healthcare_workers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0166_rename_dm_medications_other_dmreferralfollowup_other_dm_medications_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0166_rename_dm_medications_other_dmreferralfollowup_other_dm_medications_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0167_rename_healthcare_workers_other_dmreferralfollowup_other_healthcare_workers_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0167_rename_healthcare_workers_other_dmreferralfollowup_other_healthcare_workers_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0168_alter_dmreferralfollowup_last_missed_pill_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0168_alter_dmreferralfollowup_last_missed_pill_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0169_alter_dmreferralfollowup_options_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0169_alter_dmreferralfollowup_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0170_remove_glucose_repeat_fbg_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0170_remove_glucose_repeat_fbg_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0171_alter_glucose_endpoint_today_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0171_alter_glucose_endpoint_today_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0172_remove_historicalbloodresultsglu_action_item_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0172_remove_historicalbloodresultsglu_action_item_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0173_alter_glucosefbg_options_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0173_alter_glucosefbg_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0174_remove_glucosefbg_glucose_abnormal_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0174_remove_glucosefbg_glucose_abnormal_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0175_auto_20240214_2239.py` & `meta-edc-0.3.9/meta_subject/migrations/0175_auto_20240214_2239.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0176_alter_glucosefbg_glucose_value_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0176_alter_glucosefbg_glucose_value_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0177_alter_bloodresultslft_alp_value_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0177_alter_bloodresultslft_alp_value_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0178_historicalhealtheconomicsupdate_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0178_historicalhealtheconomicsupdate_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0179_alter_birthoutcomes_consent_model_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0179_alter_birthoutcomes_consent_model_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/migrations/0180_dmreferralfollowup_missed_referral_reasons_and_more.py` & `meta-edc-0.3.9/meta_subject/migrations/0180_dmreferralfollowup_missed_referral_reasons_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/model_mixins/arv_history_model_mixin.py` & `meta-edc-0.3.9/meta_subject/model_mixins/arv_history_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/model_mixins/vitals_fields_model_mixin.py` & `meta-edc-0.3.9/meta_subject/model_mixins/vitals_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/__init__.py` & `meta-edc-0.3.9/meta_subject/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/birth_outcomes.py` & `meta-edc-0.3.9/meta_subject/models/birth_outcomes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_fbc.py` & `meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_fbc.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_hba1c.py` & `meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_hba1c.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_ins.py` & `meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_ins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_lft.py` & `meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_lft.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_lipid.py` & `meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_lipid.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/blood_results/blood_results_rft.py` & `meta-edc-0.3.9/meta_subject/models/blood_results/blood_results_rft.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/complications.py` & `meta-edc-0.3.9/meta_subject/models/complications.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/complications_glycemia.py` & `meta-edc-0.3.9/meta_subject/models/complications_glycemia.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/delivery.py` & `meta-edc-0.3.9/meta_subject/models/delivery.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/diet_and_lifestyle.py` & `meta-edc-0.3.9/meta_subject/models/diet_and_lifestyle.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/dm_referral_followup.py` & `meta-edc-0.3.9/meta_subject/models/dm_referral_followup.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/egfr_drop_notification.py` & `meta-edc-0.3.9/meta_subject/models/egfr_drop_notification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/followup_examination.py` & `meta-edc-0.3.9/meta_subject/models/followup_examination.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/followup_vitals.py` & `meta-edc-0.3.9/meta_subject/models/followup_vitals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/glucose.py` & `meta-edc-0.3.9/meta_subject/models/glucose.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/glucose_fbg.py` & `meta-edc-0.3.9/meta_subject/models/glucose_fbg.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/health_economics/health_economics.py` & `meta-edc-0.3.9/meta_subject/models/health_economics/health_economics.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/health_economics/health_economics_simple.py` & `meta-edc-0.3.9/meta_subject/models/health_economics/health_economics_simple.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/health_economics/health_economics_update.py` & `meta-edc-0.3.9/meta_subject/models/health_economics/health_economics_update.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/hepatitis_test.py` & `meta-edc-0.3.9/meta_subject/models/hepatitis_test.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/off_study_drug.py` & `meta-edc-0.3.9/meta_subject/models/off_study_drug.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/other_arv_regimens.py` & `meta-edc-0.3.9/meta_subject/models/other_arv_regimens.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/other_arv_regimens_detail.py` & `meta-edc-0.3.9/meta_subject/models/other_arv_regimens_detail.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/patient_history.py` & `meta-edc-0.3.9/meta_subject/models/patient_history.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/physical_exam.py` & `meta-edc-0.3.9/meta_subject/models/physical_exam.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/pregnancy_update.py` & `meta-edc-0.3.9/meta_subject/models/pregnancy_update.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/signals.py` & `meta-edc-0.3.9/meta_subject/models/signals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/subject_visit.py` & `meta-edc-0.3.9/meta_subject/models/subject_visit.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/subject_visit_missed.py` & `meta-edc-0.3.9/meta_subject/models/subject_visit_missed.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/urine_dipstick_test.py` & `meta-edc-0.3.9/meta_subject/models/urine_dipstick_test.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/models/urine_pregnancy.py` & `meta-edc-0.3.9/meta_subject/models/urine_pregnancy.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/static/meta_subject/slider.css` & `meta-edc-0.3.9/meta_subject/static/meta_subject/slider.css`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/static/meta_subject/slider.png` & `meta-edc-0.3.9/meta_subject/static/meta_subject/slider.png`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/templates/meta_subject/widgets/slider.html` & `meta-edc-0.3.9/meta_subject/templates/meta_subject/widgets/slider.html`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/holidays.csv` & `meta-edc-0.3.9/meta_subject/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_egfr.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_egfr.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_fixes.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_fixes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_followup.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_followup.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_medication_adherence.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_medication_adherence.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_metadata_rules.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_metadata_rules.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_mnsi.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_mnsi.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_patient_history_form.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_patient_history_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_physical_exam.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_physical_exam.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_sf12.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_sf12.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/tests/test_study_medication.py` & `meta-edc-0.3.9/meta_subject/tests/tests/test_study_medication.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_subject/tests/urls.py` & `meta-edc-0.3.9/meta_subject/tests/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_visit_schedule/tests/tests/test_schedule.py` & `meta-edc-0.3.9/meta_visit_schedule/tests/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/crfs.py` & `meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/crfs.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/requisitions.py` & `meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/requisitions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/schedule.py` & `meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/schedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/schedule_pregnancy.py` & `meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/schedule_pregnancy.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/meta_visit_schedule/visit_schedules/phase_three/visit_schedule.py` & `meta-edc-0.3.9/meta_visit_schedule/visit_schedules/phase_three/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/pyproject.toml` & `meta-edc-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/runtests.py` & `meta-edc-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/setup.cfg` & `meta-edc-0.3.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [options]
 python_requires = >=3.11
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	edc==0.5.75
+	edc==0.5.76
 	edc-microscopy
 	beautifulsoup4
 
 [options.packages.find]
 exclude = 
 	examples*
 	tools*
```

### Comparing `meta-edc-0.3.8/tests/etc/randomization_list.csv` & `meta-edc-0.3.9/tests/etc/randomization_list.csv`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/tests/etc/user-rsa-local-private.pem` & `meta-edc-0.3.9/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/tests/etc/user-rsa-restricted-private.pem` & `meta-edc-0.3.9/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `meta-edc-0.3.8/tests/holidays.csv` & `meta-edc-0.3.9/tests/holidays.csv`

 * *Files identical despite different names*

