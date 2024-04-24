# Comparing `tmp/django-listing-0.7.8.tar.gz` & `tmp/django-listing-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-listing-0.7.8.tar", last modified: Wed Feb 21 11:57:38 2024, max compression
+gzip compressed data, was "django-listing-0.7.9.tar", last modified: Mon Feb 26 14:07:11 2024, max compression
```

## Comparing `django-listing-0.7.8.tar` & `django-listing-0.7.9.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.514133 django-listing-0.7.8/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2885 2024-02-21 11:51:13.000000 django-listing-0.7.8/CHANGES.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      982 2021-04-01 07:22:20.000000 django-listing-0.7.8/LICENSE.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      215 2020-05-30 19:21:14.000000 django-listing-0.7.8/MANIFEST.in
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7666 2024-02-21 11:57:38.514133 django-listing-0.7.8/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3742 2023-05-08 12:05:07.000000 django-listing-0.7.8/README.rst
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.498133 django-listing-0.7.8/django_listing/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      893 2024-02-21 11:48:02.000000 django-listing-0.7.8/django_listing/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15629 2023-07-05 10:36:54.000000 django-listing-0.7.8/django_listing/actions_buttons_column.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7260 2023-04-27 22:59:09.000000 django-listing-0.7.8/django_listing/aggregations.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3524 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/apps.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    14693 2024-02-16 12:10:54.000000 django-listing-0.7.8/django_listing/attached_form.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    65019 2024-02-20 17:16:31.000000 django-listing-0.7.8/django_listing/columns.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1230 2023-04-27 22:59:09.000000 django-listing-0.7.8/django_listing/context.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      751 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/exceptions.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32527 2024-02-05 09:57:45.000000 django-listing-0.7.8/django_listing/filters.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2317 2024-02-01 13:26:13.000000 django-listing-0.7.8/django_listing/html_attributes.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    57447 2024-02-21 11:23:57.000000 django-listing-0.7.8/django_listing/listing.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.494132 django-listing-0.7.8/django_listing/locale/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.494132 django-listing-0.7.8/django_listing/locale/en/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.498133 django-listing-0.7.8/django_listing/locale/en/LC_MESSAGES/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      527 2024-02-21 11:46:41.000000 django-listing-0.7.8/django_listing/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10535 2024-02-21 11:45:33.000000 django-listing-0.7.8/django_listing/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.494132 django-listing-0.7.8/django_listing/locale/fr/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.498133 django-listing-0.7.8/django_listing/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6419 2024-02-21 11:47:14.000000 django-listing-0.7.8/django_listing/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13982 2024-02-21 11:47:13.000000 django-listing-0.7.8/django_listing/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     9727 2024-02-08 09:25:05.000000 django-listing-0.7.8/django_listing/paginators.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16818 2024-02-18 01:30:08.000000 django-listing-0.7.8/django_listing/record.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.494132 django-listing-0.7.8/django_listing/static/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.498133 django-listing-0.7.8/django_listing/static/django_listing/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.494132 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.502133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/animation.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing-codes.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing-embedded.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7-codes.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32396 2024-02-14 08:22:19.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing.css
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.502133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74488 2020-05-06 06:54:52.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.eot
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    99231 2020-05-06 06:54:52.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74296 2020-05-06 06:54:52.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.ttf
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    40228 2020-05-06 06:54:52.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.woff
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32996 2020-05-06 06:54:52.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.woff2
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.502133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/csv.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/dbf.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/html.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/json.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/ods.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/pdf.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/tsv.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/xls.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/xlsx.svg
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.498133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.502133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    20290 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/_fonts.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16940 2024-02-14 14:20:07.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/_main.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/animation.css
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.506133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4790 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_accordion.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2126 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_alert.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1118 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_badge.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      911 2023-05-03 12:10:03.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_bootstrap.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1751 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_breadcrumb.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3073 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_button-group.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6685 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_buttons.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6736 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_card.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5580 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_carousel.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1127 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_close.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1201 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_containers.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8018 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_dropdown.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      256 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_forms.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10554 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_functions.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      575 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_grid.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      294 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_helpers.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1158 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_images.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6475 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_list-group.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1648 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_maps.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      899 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_mixins.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7762 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_modal.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4665 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_nav.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8936 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_navbar.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4555 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_offcanvas.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3940 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_pagination.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      859 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_placeholders.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6907 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_popover.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1875 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_progress.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12311 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_reboot.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2395 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_root.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2429 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_spinners.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4358 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tables.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2490 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_toasts.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3939 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tooltip.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      425 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_transitions.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1420 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_type.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    14817 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_utilities.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    68610 2023-05-03 10:46:06.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_variables.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1198 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-grid.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      163 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-reboot.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      280 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-utilities.scss
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.506133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2030 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_floating-labels.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4287 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-check.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5695 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-control.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2796 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-range.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2316 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-select.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      219 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-text.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3835 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_input-group.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1142 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_labels.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      478 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_validation.scss
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.506133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       37 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_clearfix.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      454 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_color-bg.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      450 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_colored-links.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      621 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_position.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      399 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_ratio.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      245 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_stacks.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      223 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_stretched-link.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       73 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_text-truncation.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      136 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_visually-hidden.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      147 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_vr.scss
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      393 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_alert.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      328 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_backdrop.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      263 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_banner.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2031 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_border-radius.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      398 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_box-shadow.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4580 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_breakpoints.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3220 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_buttons.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1473 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_caret.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      147 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_clearfix.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      167 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_color-scheme.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      410 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_container.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      613 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_deprecate.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4122 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_forms.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1956 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_gradients.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4726 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_grid.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      395 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_image.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      509 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_list-group.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      168 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_lists.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      387 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_pagination.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      495 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_reset-text.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_resize.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1101 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_table-variants.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      168 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_text-truncate.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      661 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_transition.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3380 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_utilities.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1012 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_visually-hidden.scss
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/utilities/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1737 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/utilities/_api.scss
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/vendor/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10029 2022-11-21 18:19:01.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/vendor/_rfs.scss
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing-codes.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing-embedded.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7-codes.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    39216 2024-02-21 11:53:53.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8120 2024-02-21 11:53:53.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing.css.map
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    39216 2024-02-21 11:53:53.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing.min.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      391 2024-02-01 13:26:13.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing.scss
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74236 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.eot
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)   103859 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74044 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.ttf
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    41044 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.woff
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    33536 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.woff2
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/csv.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/dbf.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/html.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/json.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/ods.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/pdf.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/tsv.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/xls.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/xlsx.svg
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/static/django_listing/css/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     9678 2020-07-23 13:29:12.000000 django-listing-0.7.8/django_listing/static/django_listing/css/dropzone.min.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1722 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/static/django_listing/css/dual-listbox.min.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16503 2020-05-04 16:11:45.000000 django-listing-0.7.8/django_listing/static/django_listing/css/jquery.datetimepicker.min.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16264 2023-06-26 06:53:59.000000 django-listing-0.7.8/django_listing/static/django_listing/css/select2.min.css
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/static/django_listing/js/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    24272 2024-02-21 11:53:51.000000 django-listing-0.7.8/django_listing/static/django_listing/js/django_listing.js
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    24272 2024-02-21 11:53:53.000000 django-listing-0.7.8/django_listing/static/django_listing/js/django_listing.min.js
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    47430 2020-07-23 13:29:13.000000 django-listing-0.7.8/django_listing/static/django_listing/js/dropzone.min.js
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    21613 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/static/django_listing/js/dual-listbox.js
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    21613 2024-02-21 11:53:53.000000 django-listing-0.7.8/django_listing/static/django_listing/js/dual-listbox.min.js
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    60579 2020-05-04 16:11:45.000000 django-listing-0.7.8/django_listing/static/django_listing/js/jquery.datetimepicker.full.min.js
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1681 2021-09-20 13:59:03.000000 django-listing-0.7.8/django_listing/static/django_listing/js/js.cookie.min.js
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    73163 2023-06-26 06:53:10.000000 django-listing-0.7.8/django_listing/static/django_listing/js/select2.min.js
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.498133 django-listing-0.7.8/django_listing/templates/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.498133 django-listing-0.7.8/django_listing/templates/django_listing/
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap4/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      181 2023-02-05 10:40:51.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap4/readme.txt
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.510133 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3309 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/attached_form.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2024-02-01 13:26:13.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/filters_form.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      818 2023-02-05 16:44:01.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_dropdown.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1581 2024-02-21 11:53:51.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_export.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      370 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_group_by.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      583 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_invert_selection.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1497 2023-02-05 16:44:01.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_select.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      571 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_select_all.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      575 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_unselect_all.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      384 2023-02-05 16:44:01.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_update.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2023-02-05 16:44:01.000000 django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_variations.html
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.514133 django-listing-0.7.8/django_listing/templates/django_listing/default/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1785 2020-08-13 07:02:47.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/action_footer.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      809 2023-04-28 23:01:05.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/action_header.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1804 2023-07-05 09:51:43.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/actions_buttons.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3299 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/attached_form.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        9 2018-05-13 07:49:23.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/div_row.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      226 2020-08-13 07:02:47.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/empty_listing.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2028 2024-02-01 13:26:13.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/filters_form.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3052 2024-02-21 09:12:12.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/footer.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2026 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/group_by.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1212 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/header.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7022 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/listing.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1175 2023-02-05 16:17:41.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/listing_div.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13292 2021-08-19 06:39:39.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/paginator.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      277 2019-04-09 10:09:14.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/selection_overlay.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      815 2023-02-02 17:30:06.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_dropdown.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1613 2024-02-21 11:53:51.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_export.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      370 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_group_by.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      583 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_invert_selection.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1557 2020-05-19 13:04:19.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_select.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      571 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_select_all.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      575 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_unselect_all.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      384 2020-08-13 07:02:47.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_update.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_variations.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/toolbar.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1338 2023-06-21 16:08:14.000000 django-listing-0.7.8/django_listing/templates/django_listing/default/view_object_popup.html
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.514133 django-listing-0.7.8/django_listing/templatetags/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2018-04-20 16:44:23.000000 django-listing-0.7.8/django_listing/templatetags/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12357 2024-02-12 10:36:30.000000 django-listing-0.7.8/django_listing/templatetags/django_listing.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5355 2024-02-01 13:26:29.000000 django-listing-0.7.8/django_listing/theme_config.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11116 2024-02-06 15:25:03.000000 django-listing-0.7.8/django_listing/toolbar.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2147 2023-04-27 22:59:09.000000 django-listing-0.7.8/django_listing/utils.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    28777 2024-02-21 09:29:48.000000 django-listing-0.7.8/django_listing/views.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-21 11:57:38.498133 django-listing-0.7.8/django_listing.egg-info/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7666 2024-02-21 11:57:38.000000 django-listing-0.7.8/django_listing.egg-info/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    14488 2024-02-21 11:57:38.000000 django-listing-0.7.8/django_listing.egg-info/SOURCES.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2024-02-21 11:57:38.000000 django-listing-0.7.8/django_listing.egg-info/dependency_links.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2024-02-21 11:57:38.000000 django-listing-0.7.8/django_listing.egg-info/not-zip-safe
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       55 2024-02-21 11:57:38.000000 django-listing-0.7.8/django_listing.egg-info/requires.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       15 2024-02-21 11:57:38.000000 django-listing-0.7.8/django_listing.egg-info/top_level.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2024-02-21 11:57:38.514133 django-listing-0.7.8/setup.cfg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2138 2023-04-27 22:59:09.000000 django-listing-0.7.8/setup.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.687950 django-listing-0.7.9/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2963 2024-02-26 14:06:32.000000 django-listing-0.7.9/CHANGES.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      982 2021-04-01 07:22:20.000000 django-listing-0.7.9/LICENSE.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      215 2020-05-30 19:21:14.000000 django-listing-0.7.9/MANIFEST.in
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7726 2024-02-26 14:07:11.687950 django-listing-0.7.9/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3742 2023-05-08 12:05:07.000000 django-listing-0.7.9/README.rst
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.663950 django-listing-0.7.9/django_listing/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      893 2024-02-26 14:06:32.000000 django-listing-0.7.9/django_listing/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15629 2023-07-05 10:36:54.000000 django-listing-0.7.9/django_listing/actions_buttons_column.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7260 2023-04-27 22:59:09.000000 django-listing-0.7.9/django_listing/aggregations.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3524 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/apps.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    14693 2024-02-16 12:10:54.000000 django-listing-0.7.9/django_listing/attached_form.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    65019 2024-02-20 17:16:31.000000 django-listing-0.7.9/django_listing/columns.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1230 2023-04-27 22:59:09.000000 django-listing-0.7.9/django_listing/context.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      751 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/exceptions.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32527 2024-02-05 09:57:45.000000 django-listing-0.7.9/django_listing/filters.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2317 2024-02-01 13:26:13.000000 django-listing-0.7.9/django_listing/html_attributes.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    57597 2024-02-26 14:03:24.000000 django-listing-0.7.9/django_listing/listing.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/locale/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/locale/en/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.663950 django-listing-0.7.9/django_listing/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      527 2024-02-21 11:46:41.000000 django-listing-0.7.9/django_listing/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10535 2024-02-21 11:45:33.000000 django-listing-0.7.9/django_listing/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/locale/fr/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.663950 django-listing-0.7.9/django_listing/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6419 2024-02-21 11:47:14.000000 django-listing-0.7.9/django_listing/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13982 2024-02-21 11:47:13.000000 django-listing-0.7.9/django_listing/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     9727 2024-02-08 09:25:05.000000 django-listing-0.7.9/django_listing/paginators.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16818 2024-02-18 01:30:08.000000 django-listing-0.7.9/django_listing/record.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/static/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/static/django_listing/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.663950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/animation.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing-embedded.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32396 2024-02-14 08:22:19.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing.css
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.667950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74488 2020-05-06 06:54:52.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.eot
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    99231 2020-05-06 06:54:52.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74296 2020-05-06 06:54:52.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.ttf
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    40228 2020-05-06 06:54:52.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.woff
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32996 2020-05-06 06:54:52.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.woff2
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.671950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/csv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/dbf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/html.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/json.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/ods.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/pdf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/tsv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/xls.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/xlsx.svg
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.671950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    20290 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/_fonts.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16940 2024-02-14 14:20:07.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/_main.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/animation.css
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.675950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4790 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_accordion.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2126 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_alert.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1118 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_badge.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      911 2023-05-03 12:10:03.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_bootstrap.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1751 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_breadcrumb.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3073 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_button-group.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6685 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_buttons.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6736 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_card.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5580 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_carousel.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1127 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_close.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1201 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_containers.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8018 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_dropdown.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      256 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_forms.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10554 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_functions.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      575 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_grid.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      294 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_helpers.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1158 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_images.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6475 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_list-group.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1648 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_maps.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      899 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_mixins.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7762 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_modal.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4665 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_nav.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8936 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_navbar.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4555 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_offcanvas.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3940 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_pagination.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      859 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_placeholders.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6907 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_popover.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1875 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_progress.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12311 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_reboot.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2395 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_root.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2429 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_spinners.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4358 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tables.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2490 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_toasts.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3939 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tooltip.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      425 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_transitions.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1420 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_type.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    14817 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_utilities.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    68610 2023-05-03 10:46:06.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_variables.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1198 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-grid.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      163 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-reboot.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      280 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-utilities.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.675950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2030 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_floating-labels.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4287 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-check.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5695 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-control.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2796 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-range.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2316 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-select.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      219 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-text.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3835 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_input-group.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1142 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_labels.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      478 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_validation.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.675950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       37 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_clearfix.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      454 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_color-bg.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      450 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_colored-links.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      621 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_position.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      399 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_ratio.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      245 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_stacks.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      223 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_stretched-link.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       73 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_text-truncation.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      136 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_visually-hidden.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      147 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_vr.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.679950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      393 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_alert.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      328 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_backdrop.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      263 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_banner.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2031 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_border-radius.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      398 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_box-shadow.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4580 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_breakpoints.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3220 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_buttons.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1473 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_caret.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      147 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_clearfix.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      167 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_color-scheme.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      410 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_container.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      613 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_deprecate.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4122 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_forms.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1956 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_gradients.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4726 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_grid.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      395 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_image.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      509 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_list-group.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      168 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_lists.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      387 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_pagination.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      495 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_reset-text.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_resize.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1101 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_table-variants.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      168 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_text-truncate.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      661 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_transition.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3380 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_utilities.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1012 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_visually-hidden.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.679950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/utilities/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1737 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/utilities/_api.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.679950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/vendor/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10029 2022-11-21 18:19:01.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/vendor/_rfs.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing-embedded.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    39216 2024-02-21 11:53:53.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8120 2024-02-21 11:53:53.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing.css.map
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    39216 2024-02-21 11:53:53.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing.min.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      391 2024-02-01 13:26:13.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.679950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74236 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.eot
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)   103859 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74044 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.ttf
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    41044 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.woff
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    33536 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.woff2
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.679950 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/csv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/dbf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/html.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/json.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/ods.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/pdf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/tsv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/xls.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/xlsx.svg
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.679950 django-listing-0.7.9/django_listing/static/django_listing/css/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     9678 2020-07-23 13:29:12.000000 django-listing-0.7.9/django_listing/static/django_listing/css/dropzone.min.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1722 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/static/django_listing/css/dual-listbox.min.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16503 2020-05-04 16:11:45.000000 django-listing-0.7.9/django_listing/static/django_listing/css/jquery.datetimepicker.min.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16264 2023-06-26 06:53:59.000000 django-listing-0.7.9/django_listing/static/django_listing/css/select2.min.css
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.683951 django-listing-0.7.9/django_listing/static/django_listing/js/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    24272 2024-02-21 11:53:51.000000 django-listing-0.7.9/django_listing/static/django_listing/js/django_listing.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    24272 2024-02-21 11:53:53.000000 django-listing-0.7.9/django_listing/static/django_listing/js/django_listing.min.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    47430 2020-07-23 13:29:13.000000 django-listing-0.7.9/django_listing/static/django_listing/js/dropzone.min.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    21613 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/static/django_listing/js/dual-listbox.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    21613 2024-02-21 11:53:53.000000 django-listing-0.7.9/django_listing/static/django_listing/js/dual-listbox.min.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    60579 2020-05-04 16:11:45.000000 django-listing-0.7.9/django_listing/static/django_listing/js/jquery.datetimepicker.full.min.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1681 2021-09-20 13:59:03.000000 django-listing-0.7.9/django_listing/static/django_listing/js/js.cookie.min.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    73163 2023-06-26 06:53:10.000000 django-listing-0.7.9/django_listing/static/django_listing/js/select2.min.js
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/templates/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.659950 django-listing-0.7.9/django_listing/templates/django_listing/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.683951 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap4/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      181 2023-02-05 10:40:51.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap4/readme.txt
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.683951 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3309 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/attached_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2024-02-01 13:26:13.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/filters_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      818 2023-02-05 16:44:01.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_dropdown.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1802 2024-02-26 13:45:57.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_export.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      370 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_group_by.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      583 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_invert_selection.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1497 2023-02-05 16:44:01.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_select.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      571 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_select_all.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      575 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_unselect_all.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      384 2023-02-05 16:44:01.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_update.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2023-02-05 16:44:01.000000 django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_variations.html
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.687950 django-listing-0.7.9/django_listing/templates/django_listing/default/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1785 2020-08-13 07:02:47.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/action_footer.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      809 2023-04-28 23:01:05.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/action_header.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1804 2023-07-05 09:51:43.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/actions_buttons.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3299 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/attached_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        9 2018-05-13 07:49:23.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/div_row.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      226 2020-08-13 07:02:47.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/empty_listing.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2028 2024-02-01 13:26:13.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/filters_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3052 2024-02-21 09:12:12.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/footer.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2026 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/group_by.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1212 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/header.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7022 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/listing.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1175 2023-02-05 16:17:41.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/listing_div.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13292 2021-08-19 06:39:39.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/paginator.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      277 2019-04-09 10:09:14.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/selection_overlay.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      815 2023-02-02 17:30:06.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_dropdown.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1842 2024-02-26 14:04:16.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_export.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      370 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_group_by.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      583 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_invert_selection.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1557 2020-05-19 13:04:19.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_select.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      571 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_select_all.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      575 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_unselect_all.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      384 2020-08-13 07:02:47.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_update.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_variations.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/toolbar.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1338 2023-06-21 16:08:14.000000 django-listing-0.7.9/django_listing/templates/django_listing/default/view_object_popup.html
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.687950 django-listing-0.7.9/django_listing/templatetags/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2018-04-20 16:44:23.000000 django-listing-0.7.9/django_listing/templatetags/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12357 2024-02-12 10:36:30.000000 django-listing-0.7.9/django_listing/templatetags/django_listing.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5355 2024-02-01 13:26:29.000000 django-listing-0.7.9/django_listing/theme_config.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11117 2024-02-25 13:16:31.000000 django-listing-0.7.9/django_listing/toolbar.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2147 2023-04-27 22:59:09.000000 django-listing-0.7.9/django_listing/utils.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    28777 2024-02-21 09:29:48.000000 django-listing-0.7.9/django_listing/views.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2024-02-26 14:07:11.663950 django-listing-0.7.9/django_listing.egg-info/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7726 2024-02-26 14:07:11.000000 django-listing-0.7.9/django_listing.egg-info/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    14488 2024-02-26 14:07:11.000000 django-listing-0.7.9/django_listing.egg-info/SOURCES.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2024-02-26 14:07:11.000000 django-listing-0.7.9/django_listing.egg-info/dependency_links.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2024-02-26 14:07:11.000000 django-listing-0.7.9/django_listing.egg-info/not-zip-safe
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       55 2024-02-26 14:07:11.000000 django-listing-0.7.9/django_listing.egg-info/requires.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       15 2024-02-26 14:07:11.000000 django-listing-0.7.9/django_listing.egg-info/top_level.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2024-02-26 14:07:11.687950 django-listing-0.7.9/setup.cfg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2138 2023-04-27 22:59:09.000000 django-listing-0.7.9/setup.py
```

### Comparing `django-listing-0.7.8/CHANGES.rst` & `django-listing-0.7.9/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.7.9 (2024-02-26)
+------------------
+- Add export toolbar button permission
+
 0.7.8 (2024-02-21)
 ------------------
 - Add spinner while exporting listing to file
 - Check export select file format to not be empty
 - Better default listing name
 - Exported file name has now a timestamp
```

### Comparing `django-listing-0.7.8/LICENSE.rst` & `django-listing-0.7.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/PKG-INFO` & `django-listing-0.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-listing
-Version: 0.7.8
+Version: 0.7.9
 Summary: Library for creating HTML listing / table / data grid
 Home-page: https://github.com/elapouya/django-listing
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: GPLv3+
 Keywords: table,datatable,listing,data grid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -102,14 +101,18 @@
 -------------
 
 Please, `read the doc <http://django-listing.readthedocs.org>`_  (Work in progress)
 
 News
 ----
 
+0.7.9 (2024-02-26)
+------------------
+- Add export toolbar button permission
+
 0.7.8 (2024-02-21)
 ------------------
 - Add spinner while exporting listing to file
 - Check export select file format to not be empty
 - Better default listing name
 - Exported file name has now a timestamp
```

### Comparing `django-listing-0.7.8/README.rst` & `django-listing-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/__init__.py` & `django-listing-0.7.9/django_listing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ django_listing root __init__.py file
 
    isort:skip_file
 """
 
-__version__ = "0.7.8"
+__version__ = "0.7.9"
 __author__ = "Eric Lapouyade"
 __copyright__ = "Copyright 2018, The Django listing Project"
 __credits__ = ["Eric Lapouyade"]
 __license__ = "Dual licensing"
 __maintainer__ = "Eric Lapouyade"
 __status__ = "Beta"
```

### Comparing `django-listing-0.7.8/django_listing/actions_buttons_column.py` & `django-listing-0.7.9/django_listing/actions_buttons_column.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/aggregations.py` & `django-listing-0.7.9/django_listing/aggregations.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/apps.py` & `django-listing-0.7.9/django_listing/apps.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/attached_form.py` & `django-listing-0.7.9/django_listing/attached_form.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/columns.py` & `django-listing-0.7.9/django_listing/columns.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/context.py` & `django-listing-0.7.9/django_listing/context.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/exceptions.py` & `django-listing-0.7.9/django_listing/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/filters.py` & `django-listing-0.7.9/django_listing/filters.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/html_attributes.py` & `django-listing-0.7.9/django_listing/html_attributes.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/listing.py` & `django-listing-0.7.9/django_listing/listing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1023,14 +1023,16 @@
         response = self.render_init(context)
         if response is not None:
             return response
         return self.render_template()
 
     def export_data(self):
         if self.export:
+            if not self.has_permission_for_action("export"):
+                raise ListingException(_("[You do not have permission to export data]"))
             export_format = self.export.upper()
             if export_format in EXPORT_FORMATS:
                 use_col_name = export_format in EXPORT_FORMATS_USE_COL_NAME
                 headers = self.exported_headers(use_col_name)
                 if export_format == "DBF":
                     headers = list(map(lambda h: h[:10], headers))
                 data = tablib.Dataset()
```

### Comparing `django-listing-0.7.8/django_listing/locale/en/LC_MESSAGES/django.mo` & `django-listing-0.7.9/django_listing/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/locale/en/LC_MESSAGES/django.po` & `django-listing-0.7.9/django_listing/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/locale/fr/LC_MESSAGES/django.mo` & `django-listing-0.7.9/django_listing/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/locale/fr/LC_MESSAGES/django.po` & `django-listing-0.7.9/django_listing/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/paginators.py` & `django-listing-0.7.9/django_listing/paginators.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/record.py` & `django-listing-0.7.9/django_listing/record.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/animation.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/animation.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing-codes.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing-codes.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing-embedded.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing-embedded.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7-codes.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7-codes.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/css/django_listing.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/css/django_listing.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.eot` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.eot`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.ttf` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.ttf`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.woff` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.woff`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/font/django_listing.woff2` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/font/django_listing.woff2`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/csv.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/csv.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/dbf.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/dbf.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/html.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/html.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/json.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/json.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/ods.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/ods.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/pdf.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/tsv.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/tsv.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/xls.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/xls.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap4/icons/xlsx.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap4/icons/xlsx.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/_fonts.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/_fonts.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/_main.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/_main.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/animation.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/animation.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_accordion.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_alert.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_badge.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_bootstrap.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_bootstrap.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_breadcrumb.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_button-group.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_buttons.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_card.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_carousel.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_close.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_containers.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_dropdown.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_functions.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_grid.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_images.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_list-group.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_maps.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_maps.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_mixins.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_modal.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_nav.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_navbar.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_offcanvas.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_pagination.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_placeholders.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_popover.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_progress.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_reboot.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_root.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_spinners.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tables.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_toasts.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tooltip.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_type.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_utilities.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/_variables.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-grid.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_floating-labels.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-check.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-control.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-range.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-select.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_input-group.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_labels.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_position.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_border-radius.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_breakpoints.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_buttons.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_caret.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_deprecate.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_forms.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_gradients.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_grid.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_table-variants.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_transition.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_utilities.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_visually-hidden.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/utilities/_api.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/bootstrap/vendor/_rfs.scss` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing-codes.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing-codes.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing-embedded.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing-embedded.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7-codes.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7-codes.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing.css.map` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing.css.map`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/css/django_listing.min.css` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/css/django_listing.min.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.eot` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.eot`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.ttf` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.ttf`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.woff` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.woff`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/font/django_listing.woff2` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/font/django_listing.woff2`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/csv.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/csv.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/dbf.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/dbf.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/html.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/html.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/json.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/json.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/ods.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/ods.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/pdf.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/tsv.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/tsv.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/xls.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/xls.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/bootstrap5/icons/xlsx.svg` & `django-listing-0.7.9/django_listing/static/django_listing/bootstrap5/icons/xlsx.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/css/dropzone.min.css` & `django-listing-0.7.9/django_listing/static/django_listing/css/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/css/dual-listbox.min.css` & `django-listing-0.7.9/django_listing/static/django_listing/css/dual-listbox.min.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/css/jquery.datetimepicker.min.css` & `django-listing-0.7.9/django_listing/static/django_listing/css/jquery.datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/css/select2.min.css` & `django-listing-0.7.9/django_listing/static/django_listing/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/js/django_listing.js` & `django-listing-0.7.9/django_listing/static/django_listing/js/django_listing.js`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/js/django_listing.min.js` & `django-listing-0.7.9/django_listing/static/django_listing/js/django_listing.min.js`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/js/dropzone.min.js` & `django-listing-0.7.9/django_listing/static/django_listing/js/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/js/dual-listbox.js` & `django-listing-0.7.9/django_listing/static/django_listing/js/dual-listbox.js`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/js/dual-listbox.min.js` & `django-listing-0.7.9/django_listing/static/django_listing/js/dual-listbox.min.js`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/js/jquery.datetimepicker.full.min.js` & `django-listing-0.7.9/django_listing/static/django_listing/js/jquery.datetimepicker.full.min.js`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/js/js.cookie.min.js` & `django-listing-0.7.9/django_listing/static/django_listing/js/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/static/django_listing/js/select2.min.js` & `django-listing-0.7.9/django_listing/static/django_listing/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/attached_form.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/attached_form.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/filters_form.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/filters_form.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_dropdown.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_dropdown.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_export.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_export.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 {% load django_listing i18n %}
 {% get_uniq_id as uniq_id %}
-<div class="btn-group me-2 toolbar_item {{ item.css_class }}" role="group">
-    <form id="toolbar-item-{{ uniq_id }}-form-id" class="form-inline">
-        {% gethiddens_listing listing without=item.select_name %}
-        {% if item.label %}
-            <label class="visually-hidden" for="toolbar-item-{{ uniq_id }}-select-id">{{ item.label }}</label>
-        {% endif %}
-        <div class="input-group input-group-sm me-sm-2">
-        {% if item.label %}
-            <span class="input-group-text">{{ item.label }}</span>
-        {% endif %}
-            <select id="toolbar-item-{{ uniq_id }}-select-id"
-                    name="{{ item.select_name}}{{ listing.suffix }}"
-                    class="custom-select form-select pr-4"
-                    {% if not listing.accept_ajax and not item.has_submit_button %}
-                    onchange="document.getElementById('toolbar-item-{{ uniq_id }}-form-id').submit()"
-                    {% endif %}
-            >
-                {% for key,label,selected in item.selected_choices %}
-                    <option value="{{ key }}" class="listing-icon-up-open"{% if selected %} selected{% endif %}>{{ label }}</option>
-                {% endfor %}
-            </select>
-            {% if item.has_submit_button %}
-                <button type="submit" class="btn btn-secondary btn-sm ms-1 file-generation-button" data-empty-select-msg="{% trans "Please select a file format !" %}">{{ item.button_label }}</button>
+{% listing_has_permission_for_action listing "export" as has_export_perm %}
+{% if has_export_perm %}
+    <div class="btn-group me-2 toolbar_item {{ item.css_class }}" role="group">
+        <form id="toolbar-item-{{ uniq_id }}-form-id" class="form-inline">
+            {% gethiddens_listing listing without=item.select_name %}
+            {% if item.label %}
+                <label class="visually-hidden" for="toolbar-item-{{ uniq_id }}-select-id">{{ item.label }}</label>
             {% endif %}
-        </div>
-    </form>
-</div>
+            <div class="input-group input-group-sm me-sm-2">
+            {% if item.label %}
+                <span class="input-group-text">{{ item.label }}</span>
+            {% endif %}
+                <select id="toolbar-item-{{ uniq_id }}-select-id"
+                        name="{{ item.select_name}}{{ listing.suffix }}"
+                        class="custom-select form-select pr-4"
+                        {% if not listing.accept_ajax and not item.has_submit_button %}
+                        onchange="document.getElementById('toolbar-item-{{ uniq_id }}-form-id').submit()"
+                        {% endif %}
+                >
+                    {% for key,label,selected in item.selected_choices %}
+                        <option value="{{ key }}" class="listing-icon-up-open"{% if selected %} selected{% endif %}>{{ label }}</option>
+                    {% endfor %}
+                </select>
+                {% if item.has_submit_button %}
+                    <button type="submit" class="btn btn-secondary btn-sm ms-1 file-generation-button" data-empty-select-msg="{% trans "Please select a file format !" %}">{{ item.button_label }}</button>
+                {% endif %}
+            </div>
+        </form>
+    </div>
+{% endif %}
```

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_invert_selection.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_invert_selection.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_select.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_select.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_select_all.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_select_all.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_unselect_all.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_unselect_all.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/bootstrap5/tbi_variations.html` & `django-listing-0.7.9/django_listing/templates/django_listing/bootstrap5/tbi_variations.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/action_footer.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/action_footer.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/action_header.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/action_header.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/actions_buttons.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/actions_buttons.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/attached_form.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/attached_form.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/filters_form.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/filters_form.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/footer.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/footer.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/group_by.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/group_by.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/header.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/header.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/listing.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/listing.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/listing_div.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/listing_div.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/paginator.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/paginator.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_dropdown.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_dropdown.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_export.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_select.html`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,22 @@
         {% if item.label %}
             <div class="input-group-prepend">
                 <div class="input-group-text">{{ item.label }}</div>
             </div>
         {% endif %}
             <select id="toolbar-item-{{ uniq_id }}-select-id"
                     name="{{ item.select_name}}{{ listing.suffix }}"
-                    class="custom-select form-control pr-4"
+                    class="listing-nav custom-select form-control pr-4"
                     {% if not listing.accept_ajax and not item.has_submit_button %}
                     onchange="document.getElementById('toolbar-item-{{ uniq_id }}-form-id').submit()"
                     {% endif %}
             >
                 {% for key,label,selected in item.selected_choices %}
                     <option value="{{ key }}" class="listing-icon-up-open"{% if selected %} selected{% endif %}>{{ label }}</option>
                 {% endfor %}
             </select>
             {% if item.has_submit_button %}
-                <button type="submit" class="btn btn-secondary btn-sm ml-1" data-empty-select-msg="{% trans "Please select a file format !" %}">{{ item.button_label }}</button>
+                <button type="submit" class="btn btn-secondary btn-sm ml-1">{{ item.button_label }}</button>
             {% endif %}
         </div>
     </form>
 </div>
```

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_invert_selection.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_invert_selection.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_select.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_export.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 {% load django_listing %}
 {% get_uniq_id as uniq_id %}
-<div class="btn-group mr-2 toolbar_item {{ item.css_class }}" role="group">
-    <form id="toolbar-item-{{ uniq_id }}-form-id" class="form-inline">
-        {% gethiddens_listing listing without=item.select_name %}
-        {% if item.label %}
-            <label class="sr-only" for="toolbar-item-{{ uniq_id }}-select-id">{{ item.label }}</label>
-        {% endif %}
-        <div class="input-group input-group-sm mr-sm-2">
-        {% if item.label %}
-            <div class="input-group-prepend">
-                <div class="input-group-text">{{ item.label }}</div>
-            </div>
-        {% endif %}
-            <select id="toolbar-item-{{ uniq_id }}-select-id"
-                    name="{{ item.select_name}}{{ listing.suffix }}"
-                    class="listing-nav custom-select form-control pr-4"
-                    {% if not listing.accept_ajax and not item.has_submit_button %}
-                    onchange="document.getElementById('toolbar-item-{{ uniq_id }}-form-id').submit()"
-                    {% endif %}
-            >
-                {% for key,label,selected in item.selected_choices %}
-                    <option value="{{ key }}" class="listing-icon-up-open"{% if selected %} selected{% endif %}>{{ label }}</option>
-                {% endfor %}
-            </select>
-            {% if item.has_submit_button %}
-                <button type="submit" class="btn btn-secondary btn-sm ml-1">{{ item.button_label }}</button>
+{% listing_has_permission_for_action listing "export" as has_export_perm %}
+{% if has_export_perm %}
+    <div class="btn-group mr-2 toolbar_item {{ item.css_class }}" role="group">
+        <form id="toolbar-item-{{ uniq_id }}-form-id" class="form-inline">
+            {% gethiddens_listing listing without=item.select_name %}
+            {% if item.label %}
+                <label class="sr-only" for="toolbar-item-{{ uniq_id }}-select-id">{{ item.label }}</label>
+            {% endif %}
+            <div class="input-group input-group-sm mr-sm-2">
+            {% if item.label %}
+                <div class="input-group-prepend">
+                    <div class="input-group-text">{{ item.label }}</div>
+                </div>
             {% endif %}
-        </div>
-    </form>
-</div>
+                <select id="toolbar-item-{{ uniq_id }}-select-id"
+                        name="{{ item.select_name}}{{ listing.suffix }}"
+                        class="custom-select form-control pr-4"
+                        {% if not listing.accept_ajax and not item.has_submit_button %}
+                        onchange="document.getElementById('toolbar-item-{{ uniq_id }}-form-id').submit()"
+                        {% endif %}
+                >
+                    {% for key,label,selected in item.selected_choices %}
+                        <option value="{{ key }}" class="listing-icon-up-open"{% if selected %} selected{% endif %}>{{ label }}</option>
+                    {% endfor %}
+                </select>
+                {% if item.has_submit_button %}
+                    <button type="submit" class="btn btn-secondary btn-sm ml-1" data-empty-select-msg="{% trans "Please select a file format !" %}">{{ item.button_label }}</button>
+                {% endif %}
+            </div>
+        </form>
+    </div>
+{% endif %}
```

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_select_all.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_select_all.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_unselect_all.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_unselect_all.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/tbi_variations.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/tbi_variations.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templates/django_listing/default/view_object_popup.html` & `django-listing-0.7.9/django_listing/templates/django_listing/default/view_object_popup.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/templatetags/django_listing.py` & `django-listing-0.7.9/django_listing/templatetags/django_listing.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/theme_config.py` & `django-listing-0.7.9/django_listing/theme_config.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/toolbar.py` & `django-listing-0.7.9/django_listing/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self._params = params
         self.name2item = {}
         if items:
             if isinstance(items[0], str):
                 items_name = map(str.strip, items[0].split(","))
                 items = []
                 for name in items_name:
-                    slug = re.sub("[_\d]+$", "", name)
+                    slug = re.sub(r"[_\d]+$", "", name)
                     cls = ToolbarItemMeta.get_class(slug)
                     item = cls(name)
                     item.set_listing(listing)
                     items.append(cls(name))
             elif isinstance(items[0], (list, tuple)):
                 items = items[0]
             elif isinstance(items[0], GeneratorType):
```

### Comparing `django-listing-0.7.8/django_listing/utils.py` & `django-listing-0.7.9/django_listing/utils.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing/views.py` & `django-listing-0.7.9/django_listing/views.py`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/django_listing.egg-info/PKG-INFO` & `django-listing-0.7.9/django_listing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: django-listing
-Version: 0.7.8
+Version: 0.7.9
 Summary: Library for creating HTML listing / table / data grid
 Home-page: https://github.com/elapouya/django-listing
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: GPLv3+
 Keywords: table,datatable,listing,data grid
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -102,14 +101,18 @@
 -------------
 
 Please, `read the doc <http://django-listing.readthedocs.org>`_  (Work in progress)
 
 News
 ----
 
+0.7.9 (2024-02-26)
+------------------
+- Add export toolbar button permission
+
 0.7.8 (2024-02-21)
 ------------------
 - Add spinner while exporting listing to file
 - Check export select file format to not be empty
 - Better default listing name
 - Exported file name has now a timestamp
```

### Comparing `django-listing-0.7.8/django_listing.egg-info/SOURCES.txt` & `django-listing-0.7.9/django_listing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-listing-0.7.8/setup.py` & `django-listing-0.7.9/setup.py`

 * *Files identical despite different names*

