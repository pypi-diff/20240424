# Comparing `tmp/redturtle.voltoplugin.editablefooter-1.3.2.tar.gz` & `tmp/redturtle.voltoplugin.editablefooter-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.voltoplugin.editablefooter-1.3.2.tar", last modified: Thu Mar 14 10:48:20 2024, max compression
+gzip compressed data, was "redturtle.voltoplugin.editablefooter-1.3.3.tar", last modified: Wed Apr 24 07:40:57 2024, max compression
```

## Comparing `redturtle.voltoplugin.editablefooter-1.3.2.tar` & `redturtle.voltoplugin.editablefooter-1.3.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.766507 redturtle.voltoplugin.editablefooter-1.3.2/
--rw-r--r--   0 cekk       (501) staff       (20)     1926 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/.gitlab-ci.yml
--rw-r--r--   0 cekk       (501) staff       (20)     1003 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       73 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      687 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      108 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     4470 2024-03-14 10:48:20.766574 redturtle.voltoplugin.editablefooter-1.3.2/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2218 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/constraints_plone52.txt
--rw-r--r--   0 cekk       (501) staff       (20)       62 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/constraints_plone60.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.760381 redturtle.voltoplugin.editablefooter-1.3.2/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     8032 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)      119 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)       33 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      439 2024-03-14 10:48:20.766822 redturtle.voltoplugin.editablefooter-1.3.2/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2676 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.757125 redturtle.voltoplugin.editablefooter-1.3.2/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.760511 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.761711 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.762515 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/
--rw-r--r--   0 cekk       (501) staff       (20)      153 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.762908 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      533 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      612 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)     1482 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      771 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.763534 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.757609 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.763811 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/en/LC_MESSAGES/redturtle.volto_editablefooter.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1770 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/en/LC_MESSAGES/redturtle.volto_editablefooter.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.757755 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.764075 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     1119 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/redturtle.volto_editablefooter.mo
--rw-r--r--   0 cekk       (501) staff       (20)     2067 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/redturtle.volto_editablefooter.po
--rw-r--r--   0 cekk       (501) staff       (20)     1912 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/redturtle.volto_editablefooter.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1613 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      545 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      273 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.757990 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.764839 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      227 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      606 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      182 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)      255 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.765219 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      146 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      384 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      268 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/uninstall/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.765966 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1037 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      622 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)     1262 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/deserializer.py
--rw-r--r--   0 cekk       (501) staff       (20)     2296 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/get.py
--rw-r--r--   0 cekk       (501) staff       (20)      760 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/serializer.py
--rw-r--r--   0 cekk       (501) staff       (20)      613 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     2370 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.766364 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3672 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/tests/test_controlpanel_api.py
--rw-r--r--   0 cekk       (501) staff       (20)     4146 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/tests/test_footer_columns_route.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-14 10:48:20.761580 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4470 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3293 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      141 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       32 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      200 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       10 2024-03-14 10:48:20.000000 redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.913345 redturtle.voltoplugin.editablefooter-1.3.3/
+-rw-r--r--   0 cekk       (501) staff       (20)     1926 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/.gitlab-ci.yml
+-rw-r--r--   0 cekk       (501) staff       (20)     1138 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       73 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      687 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      108 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     4605 2024-04-24 07:40:57.913400 redturtle.voltoplugin.editablefooter-1.3.3/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2218 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/constraints_plone52.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       62 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/constraints_plone60.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.907785 redturtle.voltoplugin.editablefooter-1.3.3/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     8032 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)      119 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       33 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      340 2024-04-24 07:40:57.913615 redturtle.voltoplugin.editablefooter-1.3.3/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2652 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.905187 redturtle.voltoplugin.editablefooter-1.3.3/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.907880 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.908826 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.909467 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/
+-rw-r--r--   0 cekk       (501) staff       (20)      153 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.909772 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      533 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      603 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1482 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      771 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.910291 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.905595 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.910552 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/en/LC_MESSAGES/redturtle.volto_editablefooter.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1770 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/en/LC_MESSAGES/redturtle.volto_editablefooter.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.905715 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.910817 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     1119 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/redturtle.volto_editablefooter.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     2067 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/redturtle.volto_editablefooter.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1912 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/redturtle.volto_editablefooter.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1613 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      545 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.905905 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.911634 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      227 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      606 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      182 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      255 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.912006 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      146 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      384 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      268 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/uninstall/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.912837 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)      488 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1037 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      677 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2508 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/deserializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2774 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1346 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/serializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)      613 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2370 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.913214 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     7718 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/tests/test_controlpanel_api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6015 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/tests/test_footer_columns_route.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:40:57.908725 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     4605 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3293 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      141 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       32 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      187 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2024-04-24 07:40:57.000000 redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/top_level.txt
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/.gitlab-ci.yml` & `redturtle.voltoplugin.editablefooter-1.3.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/CHANGES.rst` & `redturtle.voltoplugin.editablefooter-1.3.3/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.3.3 (2024-04-24)
+------------------
+
+- Fix serializer/deserializer for footerTop blocks: use blocks handlers to fix data.
+  [cekk]
+
+
 1.3.2 (2024-03-14)
 ------------------
 
 - Revert changes to 1.2.1 branch. We haven't deleted 1.3.0 and 1.3.1 branches because there are some releases on pypi.
   [cekk]
 
 1.3.1 (2024-03-14)
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/DEVELOP.rst` & `redturtle.voltoplugin.editablefooter-1.3.3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/LICENSE.GPL` & `redturtle.voltoplugin.editablefooter-1.3.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/LICENSE.rst` & `redturtle.voltoplugin.editablefooter-1.3.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/PKG-INFO` & `redturtle.voltoplugin.editablefooter-1.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.voltoplugin.editablefooter
-Version: 1.3.2
+Version: 1.3.3
 Summary: Add-on for Volto to manage four-columns footer
 Home-page: https://github.com/collective/redturtle.voltoplugin.editablefooter
 Author: RedTurtle Techonolgy
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.voltoplugin.editablefooter
 Project-URL: Source, https://github.com/collective/redturtle.voltoplugin.editablefooter
@@ -130,14 +130,21 @@
 
 - RedTurtle Techonolgy, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+1.3.3 (2024-04-24)
+------------------
+
+- Fix serializer/deserializer for footerTop blocks: use blocks handlers to fix data.
+  [cekk]
+
+
 1.3.2 (2024-03-14)
 ------------------
 
 - Revert changes to 1.2.1 branch. We haven't deleted 1.3.0 and 1.3.1 branches because there are some releases on pypi.
   [cekk]
 
 1.3.1 (2024-03-14)
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/README.rst` & `redturtle.voltoplugin.editablefooter-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/docs/conf.py` & `redturtle.voltoplugin.editablefooter-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/setup.py` & `redturtle.voltoplugin.editablefooter-1.3.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.voltoplugin.editablefooter",
-    version="1.3.2",
+    version="1.3.3",
     description="Add-on for Volto to manage four-columns footer",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
@@ -48,16 +48,15 @@
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.6",
     install_requires=[
         "setuptools",
         "plone.api >= 1.8.4",
-        "plone.restapi",
-        "plone.app.dexterity",
+        "plone.restapi>=9.5.0",
         "plone.volto",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/browser/configure.zcml` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/browser/controlpanel.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/browser/controlpanel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
 from plone.app.registry.browser import controlpanel
-from redturtle.voltoplugin.editablefooter.interfaces import (
-    IEditableFooterSettings,
-)
 from redturtle.voltoplugin.editablefooter import _
+from redturtle.voltoplugin.editablefooter.interfaces import IEditableFooterSettings
 
 
 class EditableFooterForm(controlpanel.RegistryEditForm):
     schema = IEditableFooterSettings
     label = _("editable_footer_settings_label", default="Editable Footer Settings")
     description = _(
         "editable_footer_settings_help",
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/configure.zcml` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/interfaces.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/README.rst` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/en/LC_MESSAGES/redturtle.volto_editablefooter.po` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/en/LC_MESSAGES/redturtle.volto_editablefooter.po`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/redturtle.volto_editablefooter.mo` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/redturtle.volto_editablefooter.mo`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/redturtle.volto_editablefooter.po` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/it/LC_MESSAGES/redturtle.volto_editablefooter.po`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/redturtle.volto_editablefooter.pot` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/redturtle.volto_editablefooter.pot`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/update.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/locales/update.sh` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/locales/update.sh`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/profiles/default/controlpanel.xml` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/configure.zcml` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/controlpanel.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/controlpanel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from plone.restapi.controlpanels import RegistryConfigletPanel
+from redturtle.voltoplugin.editablefooter.interfaces import IEditableFooterSettings
 from redturtle.voltoplugin.editablefooter.interfaces import (
     IRedturtleVoltoEditablefooterLayer,
-    IEditableFooterSettings,
 )
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 @adapter(Interface, IRedturtleVoltoEditablefooterLayer)
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/deserializer.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/serializer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # -*- coding: utf-8 -*-
-from plone.restapi.deserializer import json_body
-from plone.restapi.deserializer.controlpanels import (
-    ControlpanelDeserializeFromJson,
-)
-from plone.restapi.interfaces import IDeserializeFromJson
-from redturtle.voltoplugin.editablefooter.interfaces import (
-    IEditableFooterSettings,
-)
-from zExceptions import BadRequest
+from plone import api
+from plone.restapi.interfaces import IBlockFieldSerializationTransformer
+from plone.restapi.interfaces import ISerializeToJson
+from plone.restapi.serializer.controlpanels import ControlpanelSerializeToJson
+from redturtle.voltoplugin.editablefooter.interfaces import IEditableFooterSettings
+from redturtle.voltoplugin.editablefooter.restapi import fix_footer_top_blocks
 from zope.component import adapter
 from zope.interface import implementer
 
 import json
 
 
-@implementer(IDeserializeFromJson)
+@implementer(ISerializeToJson)
 @adapter(IEditableFooterSettings)
-class EditableFooterControlpanelDeserializeFromJson(ControlpanelDeserializeFromJson):
+class EditableFooterControlpanelSerializeToJson(ControlpanelSerializeToJson):
     def __call__(self):
-        req = json_body(self.controlpanel.request)
-        proxy = self.registry.forInterface(self.schema, prefix=self.schema_prefix)
-        errors = []
-        data = req.get("footer_columns", {})
-        if not data:
-            errors.append({"message": "Missing data", "field": "footer_columns"})
-            raise BadRequest(errors)
-        try:
-            # later we need to do some validations
-            setattr(proxy, "footer_columns", json.dumps(data))
-        except ValueError as e:
-            errors.append({"message": str(e), "field": "footer_columns", "error": e})
+        json_data = super().__call__()
+        conf = json_data["data"].get("footer_columns", "")
+        if not conf:
+            return json_data
+        footer_columns = json.loads(conf)
 
-        if errors:
-            raise BadRequest(errors)
+        for path_setting in footer_columns:
+            footer_top = path_setting.get("footerTop", {}).get("blocks", {})
+            if footer_top:
+                path_setting["footerTop"]["blocks"] = fix_footer_top_blocks(
+                    context=api.portal.get(),
+                    blocks=footer_top,
+                    transformer=IBlockFieldSerializationTransformer,
+                )
+
+        json_data["data"]["footer_columns"] = footer_columns
+        return json_data
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/restapi/get.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/restapi/get.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 # -*- coding: utf-8 -*-
-from redturtle.voltoplugin.editablefooter.interfaces import (
-    IEditableFooterSettings,
-)
 from plone import api
 from plone.registry.interfaces import IRegistry
+from plone.restapi.interfaces import IBlockFieldSerializationTransformer
+from plone.restapi.serializer.converters import json_compatible
 from plone.restapi.services import Service
+from redturtle.voltoplugin.editablefooter.interfaces import IEditableFooterSettings
+from redturtle.voltoplugin.editablefooter.restapi import fix_footer_top_blocks
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.publisher.interfaces import IPublishTraverse
 
+
 try:
     from plone.volto.interfaces import IVoltoSettings
 
     HAS_PLONE_VOLTO = True
 except ImportError:
     HAS_PLONE_VOLTO = False
 
 import json
 
 
 @implementer(IPublishTraverse)
 class FooterColumns(Service):
-    def __init__(self, context, request):
-        super(FooterColumns, self).__init__(context, request)
-
     def reply(self):
         record = api.portal.get_registry_record(
             "footer_columns", interface=IEditableFooterSettings, default=""
         )
         if not record:
             return []
         data = json.loads(record)
         portal_url = self.get_portal_url()
         for el in data or []:
             if isinstance(el, dict):
+                footer_top = el.get("footerTop", {}).get("blocks", {})
+                if footer_top:
+                    el["footerTop"]["blocks"] = fix_footer_top_blocks(
+                        context=self.context,
+                        blocks=footer_top,
+                        transformer=IBlockFieldSerializationTransformer,
+                    )
+
                 for item in el.get("items") or []:
                     if (
                         isinstance(item, dict)
                         and item.get("text")  # noqa: W503
                         and isinstance(item.get("text"), dict)  # noqa: W503
                         and item.get("text").get("data")  # noqa: W503
                     ):
                         item["text"]["data"] = item["text"]["data"].replace(
                             'href="/', f'href="{portal_url}/'
                         )
-        return data
+        return json_compatible(data)
 
     def get_portal_url(self):
         portal_url = api.portal.get().absolute_url()
         # BBB
         if portal_url.endswith("/api"):
             portal_url = portal_url[:4]
         if not HAS_PLONE_VOLTO:
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/setuphandlers.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/testing.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/testing.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneSandboxLayer
 from plone.restapi.testing import PloneRestApiDXLayer
 from plone.testing import z2
 
-import redturtle.voltoplugin.editablefooter
 import plone.restapi
 import plone.volto
+import redturtle.voltoplugin.editablefooter
 
 
 class VoltoEditableFooterLayer(PloneSandboxLayer):
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle/voltoplugin/editablefooter/tests/test_footer_columns_route.py` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle/voltoplugin/editablefooter/tests/test_footer_columns_route.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from redturtle.voltoplugin.editablefooter.interfaces import IEditableFooterSettings
 from redturtle.voltoplugin.editablefooter.testing import (
     VOLTO_EDITABLEFOOTER_API_FUNCTIONAL_TESTING,
 )
 from transaction import commit
 from zope.component import getUtility
 
-
 import json
 import unittest
 
 
 class FooterColumnsEndpointTest(unittest.TestCase):
     layer = VOLTO_EDITABLEFOOTER_API_FUNCTIONAL_TESTING
 
@@ -40,14 +39,19 @@
                     {"text": {"data": '<a href="https://site.com/">Link 1</a>'}},
                     {"text": {"data": '<a href="/relative/to/this/site">Link 1</a>'}},
                 ]
             }
         ]
         self.set_record_value(field="footer_columns", value=json.dumps(self.value))
 
+        self.document = api.content.create(
+            container=self.portal, type="Document", title="document"
+        )
+        commit()
+
     def tearDown(self):
         self.api_session.close()
 
     def set_record_value(self, field, value):
         api.portal.set_registry_record(field, value, interface=IEditableFooterSettings)
         commit()
 
@@ -63,14 +67,57 @@
         # self.value has relative links, but the result should have absolute links
         self.assertNotEqual(result, self.value)
         self.assertEqual(
             json.dumps(result),
             json.dumps(self.value).replace('href=\\"/', f'href=\\"{self.portal_url}/'),
         )
 
+    def test_return_expanded_resolveuid_in_footerTop_internal_links(self):
+        data = [
+            {
+                "footerTop": {
+                    "blocks": {
+                        "2955de0f-ea5e-475f-8efd-34c7060b99b9": {
+                            "@type": "slate",
+                            "plaintext": " link ",
+                            "value": [
+                                {
+                                    "children": [
+                                        {
+                                            "type": "link",
+                                            "data": {
+                                                "url": self.document.absolute_url(),
+                                                "dataElement": "",
+                                            },
+                                            "children": [{"text": "link"}],
+                                        },
+                                    ],
+                                    "type": "p",
+                                }
+                            ],
+                        }
+                    },
+                    "blocks_layout": {
+                        "items": ["2955de0f-ea5e-475f-8efd-34c7060b99b9"]
+                    },
+                },
+                "rootPath": "/",
+            }
+        ]
+        self.set_record_value(field="footer_columns", value=json.dumps(data))
+
+        response = self.api_session.get("/@footer-columns").json()
+
+        self.assertEqual(
+            response[0]["footerTop"]["blocks"]["2955de0f-ea5e-475f-8efd-34c7060b99b9"][
+                "value"
+            ][0]["children"][0]["data"]["url"],
+            self.document.absolute_url(),
+        )
+
 
 class FooterColumnsEndpointTestWithPloneVolto(FooterColumnsEndpointTest):
     layer = VOLTO_EDITABLEFOOTER_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         super().setUp()
         applyProfile(self.portal, "plone.volto:default")
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/PKG-INFO` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.voltoplugin.editablefooter
-Version: 1.3.2
+Version: 1.3.3
 Summary: Add-on for Volto to manage four-columns footer
 Home-page: https://github.com/collective/redturtle.voltoplugin.editablefooter
 Author: RedTurtle Techonolgy
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.voltoplugin.editablefooter
 Project-URL: Source, https://github.com/collective/redturtle.voltoplugin.editablefooter
@@ -130,14 +130,21 @@
 
 - RedTurtle Techonolgy, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+1.3.3 (2024-04-24)
+------------------
+
+- Fix serializer/deserializer for footerTop blocks: use blocks handlers to fix data.
+  [cekk]
+
+
 1.3.2 (2024-03-14)
 ------------------
 
 - Revert changes to 1.2.1 branch. We haven't deleted 1.3.0 and 1.3.1 branches because there are some releases on pypi.
   [cekk]
 
 1.3.1 (2024-03-14)
```

### Comparing `redturtle.voltoplugin.editablefooter-1.3.2/src/redturtle.voltoplugin.editablefooter.egg-info/SOURCES.txt` & `redturtle.voltoplugin.editablefooter-1.3.3/src/redturtle.voltoplugin.editablefooter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

