# Comparing `tmp/odoo14-addon-sale_order_mitxelena-14.0.1.0.6.tar.gz` & `tmp/odoo14-addon-sale_order_mitxelena-14.0.1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-sale_order_mitxelena-14.0.1.0.6.tar", last modified: Mon Mar 18 07:44:49 2024, max compression
+gzip compressed data, was "odoo14-addon-sale_order_mitxelena-14.0.1.0.7.tar", last modified: Wed Apr 24 09:33:16 2024, max compression
```

## Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6.tar` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.465553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/
--rw-r--r--   0 root         (0) root         (0)      393 2024-03-18 07:44:49.465553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.457553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.457553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.457553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-03-18 07:44:47.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.457553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3039 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/controllers/zip_reports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.461553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    14758 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/ca.po
--rw-rw-rw-   0 root         (0) root         (0)    16279 2024-03-18 07:44:47.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)    16211 2024-03-18 07:44:47.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/eu.po
--rw-rw-rw-   0 root         (0) root         (0)    14688 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/sale_order_mitxelena.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.461553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/models/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1725 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/models/sale_order.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.461553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/mitxelena_sale_order_report.py
--rw-rw-rw-   0 root         (0) root         (0)     8809 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/mitxelena_sale_order_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1434 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/mitxelena_standar_layout.xml
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/sale_order_report_template.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.461553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/security/
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.457553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.457553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.461553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/
--rw-rw-rw-   0 root         (0) root         (0)    69697 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/AS-9100-bw.tm.jpg
--rw-rw-rw-   0 root         (0) root         (0)   264537 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/UKAS-AND-ISO-9001-bw.tm.png
--rw-rw-rw-   0 root         (0) root         (0)     2846 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/logo-mitxelena.png
--rw-rw-rw-   0 root         (0) root         (0)     5059 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/zerbitzua-euskaraz-zb.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.457553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.461553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/src/js/
--rw-rw-rw-   0 root         (0) root         (0)     1114 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/src/js/sale_order_line.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.461553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/views/
--rw-rw-rw-   0 root         (0) root         (0)     4130 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/views/sale_order_line_views.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.465553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/wizard/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/wizard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1733 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/wizard/sale_order_report_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2024-03-18 06:12:03.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/wizard/sale_order_report_wizard_view.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 07:44:49.465553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo14_addon_sale_order_mitxelena.egg-info/
--rw-r--r--   0 root         (0) root         (0)      393 2024-03-18 07:44:49.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo14_addon_sale_order_mitxelena.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1884 2024-03-18 07:44:49.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo14_addon_sale_order_mitxelena.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 07:44:49.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo14_addon_sale_order_mitxelena.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 07:44:49.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo14_addon_sale_order_mitxelena.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-18 07:44:49.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo14_addon_sale_order_mitxelena.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-18 07:44:49.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo14_addon_sale_order_mitxelena.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-18 07:44:49.465553 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-03-18 07:44:47.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.938017 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      393 2024-04-24 09:33:16.938017 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3039 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/controllers/zip_reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    14758 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/ca.po
+-rw-rw-rw-   0 root         (0) root         (0)    16274 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)    16211 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/eu.po
+-rw-rw-rw-   0 root         (0) root         (0)    14688 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/sale_order_mitxelena.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/models/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1872 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/models/sale_order.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/mitxelena_sale_order_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     8809 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/mitxelena_sale_order_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/mitxelena_standar_layout.xml
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/sale_order_report_template.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/security/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/
+-rw-rw-rw-   0 root         (0) root         (0)    69697 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/AS-9100-bw.tm.jpg
+-rw-rw-rw-   0 root         (0) root         (0)   264537 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/UKAS-AND-ISO-9001-bw.tm.png
+-rw-rw-rw-   0 root         (0) root         (0)     2846 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/logo-mitxelena.png
+-rw-rw-rw-   0 root         (0) root         (0)     5059 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/zerbitzua-euskaraz-zb.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.934016 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/src/js/sale_order_line.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.938017 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/views/
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/views/sale_order_line_views.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.938017 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/wizard/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/wizard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/wizard/sale_order_report_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/wizard/sale_order_report_wizard_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 09:33:16.938017 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo14_addon_sale_order_mitxelena.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      393 2024-04-24 09:33:16.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo14_addon_sale_order_mitxelena.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-24 09:33:16.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo14_addon_sale_order_mitxelena.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 09:33:16.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo14_addon_sale_order_mitxelena.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 09:33:16.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo14_addon_sale_order_mitxelena.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 09:33:16.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo14_addon_sale_order_mitxelena.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-24 09:33:16.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo14_addon_sale_order_mitxelena.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 09:33:16.938017 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-24 09:33:15.000000 odoo14-addon-sale_order_mitxelena-14.0.1.0.7/setup.py
```

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/__manifest__.py` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/__manifest__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Sale Order Mitxelena Custom',
-    'version': '14.0.1.0.6',
+    'version': '14.0.1.0.7',
     "license": "AGPL-3",
     'category': 'Sales',
     'summary': 'Customization for sale order',
     'depends': ['sale', 
                 'base'],
     'data': [
         'views/sale_order_line_views.xml',
```

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/controllers/zip_reports.py` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/controllers/zip_reports.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/ca.po` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/ca.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/es.po` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 	* sale_order_mitxelena
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-15 10:25+0000\n"
-"PO-Revision-Date: 2024-03-18 07:42+0000\n"
+"PO-Revision-Date: 2024-03-19 08:58+0000\n"
 "Last-Translator: Unai Gorrotxategi <unai@talaios.coop>\n"
 "Language-Team: Spanish <https://weblate.devs.coop/projects/odoo-mitxelena/"
 "sale-order-mitxelena/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
@@ -331,15 +331,15 @@
 #: model:ir.model,name:sale_order_mitxelena.model_product_template
 msgid "Product Template"
 msgstr "Plantilla de Producto"
 
 #. module: sale_order_mitxelena
 #: model_terms:ir.ui.view,arch_db:sale_order_mitxelena.report_saleorder_template
 msgid "QUOTATION"
-msgstr "PRESUPUESTO"
+msgstr "OFERTA"
 
 #. module: sale_order_mitxelena
 #: model_terms:ir.ui.view,arch_db:sale_order_mitxelena.report_saleorder_template
 msgid "Quantity"
 msgstr "Cantidad"
 
 #. module: sale_order_mitxelena
```

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/eu.po` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/eu.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/i18n/sale_order_mitxelena.pot` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/i18n/sale_order_mitxelena.pot`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/models/sale_order.py` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/models/sale_order.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from odoo import models, fields, api, _
 from odoo.exceptions import UserError, ValidationError
 
 class SaleOrderLine(models.Model):
     _inherit = 'sale.order.line'
-    
-    dimensions = fields.Char(string="Dimensions")
-    materials = fields.Char(string="Materials")    
+
+    dimensions = fields.Char(related="product_id.dimensions", string="Dimensions")
+    materials = fields.Char(related="product_id.materials", string="Materials")
     date_order = fields.Datetime(related="order_id.date_order")
-    client_order_ref = fields.Char(related='order_id.client_order_ref', string="Client ref.")    
+    client_order_ref = fields.Char(related='order_id.client_order_ref', string="Client ref.")
     plan = fields.Binary(string="Plan", related="product_id.plan")
     plan_fname = fields.Char(string="Plan", related="product_id.plan_fname")    
         
 class SaleOrder(models.Model):
     _inherit = 'sale.order'
     mecanization = fields.Boolean(string="Mecanization")
     welding = fields.Boolean(string="Welding")
@@ -22,11 +22,13 @@
                                                 ('energy', _('Energy')), ('aeronautic', _('Aeronautic')), ('petrochemical', _('Petrochemical')),
                                                 ('press', _('Press')),('others', _('Others'))])
     urgency = fields.Boolean(string="Urgency")
     reparation = fields.Boolean(string="Reparation")
     estimated_date = fields.Char(string="Estimated date")
 
 class Product(models.Model):
-    _inherit = ["product.template"]    
+    _inherit = ["product.template"]
+    dimensions = fields.Char(string="Dimensions")
+    materials = fields.Char(string="Materials")
     plan = fields.Binary(string="Plan file")
     plan_fname = fields.Char(string='File name')
     special_processes_treatments = fields.Text(string='Treatments / Processes')
```

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/mitxelena_sale_order_report.py` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/mitxelena_sale_order_report.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/mitxelena_sale_order_template.xml` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/mitxelena_sale_order_template.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/reports/mitxelena_standar_layout.xml` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/reports/mitxelena_standar_layout.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/AS-9100-bw.tm.jpg` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/AS-9100-bw.tm.jpg`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/UKAS-AND-ISO-9001-bw.tm.png` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/UKAS-AND-ISO-9001-bw.tm.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/logo-mitxelena.png` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/logo-mitxelena.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/report/img/zerbitzua-euskaraz-zb.png` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/report/img/zerbitzua-euskaraz-zb.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/static/src/js/sale_order_line.js` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/static/src/js/sale_order_line.js`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/views/sale_order_line_views.xml` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/views/sale_order_line_views.xml`

 * *Files 2% similar despite different names*

#### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/views/sale_order_line_views.xml` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/views/sale_order_line_views.xml`

```diff
@@ -19,19 +19,19 @@
         <field name="client_order_ref"/>
         <field name="order_partner_id"/>
         <field name="qty_invoiced"/>
         <field name="state"/>
       </tree>
     </field>
   </record>
-  <template id="sale_order_mitxelena.sale_order_line_assets" name="sale_order_line_assets" inherit_id="web.assets_backend">
-    <xpath expr="." position="inside">
-      <script type="text/javascript" src="/sale_order_mitxelena/static/src/js/sale_order_line.js"/>
-    </xpath>
-  </template>
+  <!-- <template id="sale_order_mitxelena.sale_order_line_assets" name="sale_order_line_assets" inherit_id="web.assets_backend">
+        <xpath expr="." position="inside">
+            <script type="text/javascript" src="/sale_order_mitxelena/static/src/js/sale_order_line.js"></script>
+        </xpath>
+    </template> -->
   <!-- Form view for sale order -->
   <record id="view_order_form_custom" model="ir.ui.view">
     <field name="name">sale.order.form.custom</field>
     <field name="model">sale.order</field>
     <field name="inherit_id" ref="sale.view_order_form"/>
     <field name="arch" type="xml">
       <xpath expr="//field[@name='order_line']/tree/field[@name='product_uom_qty']" position="after">
@@ -61,14 +61,16 @@
   <!-- Form view for product -->
   <record id="view_product_form_custom" model="ir.ui.view">
     <field name="name">product.template.form.custom</field>
     <field name="model">product.template</field>
     <field name="inherit_id" ref="product.product_template_only_form_view"/>
     <field name="arch" type="xml">
       <xpath expr="//field[@name='company_id']" position="after">
+        <field name="dimensions"/>
+        <field name="materials"/>
         <field name="plan" widget="binary" filename="plan_fname"/>
         <field name="plan_fname" invisible="1"/>
       </xpath>
       <xpath expr="//field[@name='barcode']" position="after">
         <field name="special_processes_treatments" widget="text"/>
       </xpath>
     </field>
```

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/wizard/sale_order_report_wizard.py` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/wizard/sale_order_report_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo/addons/sale_order_mitxelena/wizard/sale_order_report_wizard_view.xml` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo/addons/sale_order_mitxelena/wizard/sale_order_report_wizard_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-sale_order_mitxelena-14.0.1.0.6/odoo14_addon_sale_order_mitxelena.egg-info/SOURCES.txt` & `odoo14-addon-sale_order_mitxelena-14.0.1.0.7/odoo14_addon_sale_order_mitxelena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

