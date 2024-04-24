# Comparing `tmp/collective.listmonk-1.0.0a6.tar.gz` & `tmp/collective.listmonk-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.listmonk-1.0.0a6.tar", last modified: Mon Apr 22 20:49:49 2024, max compression
+gzip compressed data, was "collective.listmonk-1.0.0a7.tar", last modified: Wed Apr 24 17:56:59 2024, max compression
```

## Comparing `collective.listmonk-1.0.0a6.tar` & `collective.listmonk-1.0.0a7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.026454 collective.listmonk-1.0.0a6/
--rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/.editorconfig
--rw-r--r--   0 davisagli   (501) staff       (20)     1323 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/CHANGES.md
--rw-r--r--   0 davisagli   (501) staff       (20)       69 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/CONTRIBUTORS.md
--rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/LICENSE.GPL
--rw-r--r--   0 davisagli   (501) staff       (20)      665 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/LICENSE.md
--rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/MANIFEST.in
--rw-r--r--   0 davisagli   (501) staff       (20)     7321 2024-04-22 20:49:49.026209 collective.listmonk-1.0.0a6/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     4218 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/README.md
--rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/constraints.txt
--rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/docker-compose.yml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.018140 collective.listmonk-1.0.0a6/docs/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/docs/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/docs/dlr.svg
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.018443 collective.listmonk-1.0.0a6/news/
--rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/news/.changelog_template.jinja
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/news/.gitkeep
--rw-r--r--   0 davisagli   (501) staff       (20)     4793 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/pyproject.toml
--rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/requirements.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-22 20:49:49.026497 collective.listmonk-1.0.0a6/setup.cfg
--rw-r--r--   0 davisagli   (501) staff       (20)     2323 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/setup.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.014484 collective.listmonk-1.0.0a6/src/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.018589 collective.listmonk-1.0.0a6/src/collective/
--rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.020845 collective.listmonk-1.0.0a6/src/collective/listmonk/
--rw-r--r--   0 davisagli   (501) staff       (20)      199 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.021097 collective.listmonk-1.0.0a6/src/collective/listmonk/behaviors/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/behaviors/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/behaviors/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      465 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.021355 collective.listmonk-1.0.0a6/src/collective/listmonk/content/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/content/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3506 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/content/newsletter.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.021613 collective.listmonk-1.0.0a6/src/collective/listmonk/controlpanel/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/controlpanel/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      220 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/controlpanel/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      187 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/dependencies.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      232 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/interfaces.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1504 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/listmonk.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.022034 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3636 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/collective.listmonk.pot
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.015053 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/de/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.022176 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/de/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     3684 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.015209 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/en/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.022319 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/en/LC_MESSAGES/
--rw-r--r--   0 davisagli   (501) staff       (20)     3047 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po
--rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/locales/update.py
--rw-r--r--   0 davisagli   (501) staff       (20)      404 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/permissions.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.015528 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.022895 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      182 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/metadata.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      585 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/rolemap.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.023035 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/types/
--rw-r--r--   0 davisagli   (501) staff       (20)     2764 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/types/Newsletter.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      185 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/types.xml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.023182 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/uninstall/
--rw-r--r--   0 davisagli   (501) staff       (20)      122 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 davisagli   (501) staff       (20)      824 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/profiles.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.023873 collective.listmonk-1.0.0a6/src/collective/listmonk/services/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/services/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1592 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/services/base.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1261 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/services/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     6404 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/services/mailings.py
--rw-r--r--   0 davisagli   (501) staff       (20)     7495 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/services/subscriptions.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.024018 collective.listmonk-1.0.0a6/src/collective/listmonk/setuphandlers/
--rw-r--r--   0 davisagli   (501) staff       (20)      339 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/setuphandlers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3210 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/testing.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.024279 collective.listmonk-1.0.0a6/src/collective/listmonk/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/upgrades/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      140 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective/listmonk/upgrades/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.025566 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/
--rw-r--r--   0 davisagli   (501) staff       (20)     7321 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     2449 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/SOURCES.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/dependency_links.txt
--rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/entry_points.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/namespace_packages.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/not-zip-safe
--rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/requires.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/top_level.txt
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.024532 collective.listmonk-1.0.0a6/tests/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/tests/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.024923 collective.listmonk-1.0.0a6/tests/api/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/tests/api/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4966 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/tests/api/test_mailings.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5173 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/tests/api/test_subscriptions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3116 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/tests/conftest.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.025210 collective.listmonk-1.0.0a6/tests/setup/
--rw-r--r--   0 davisagli   (501) staff       (20)      917 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/tests/setup/test_setup_install.py
--rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/tests/setup/test_setup_uninstall.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-22 20:49:49.025351 collective.listmonk-1.0.0a6/tests/setup/upgrades/
--rw-r--r--   0 davisagli   (501) staff       (20)      645 2024-04-22 20:49:48.000000 collective.listmonk-1.0.0a6/tests/setup/upgrades/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.402063 collective.listmonk-1.0.0a7/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1363 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/.editorconfig
+-rw-r--r--   0 davisagli   (501) staff       (20)     1554 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/CHANGES.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       69 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/CONTRIBUTORS.md
+-rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/LICENSE.GPL
+-rw-r--r--   0 davisagli   (501) staff       (20)      665 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/LICENSE.md
+-rw-r--r--   0 davisagli   (501) staff       (20)      328 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/MANIFEST.in
+-rw-r--r--   0 davisagli   (501) staff       (20)     7552 2024-04-24 17:56:59.401757 collective.listmonk-1.0.0a7/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     4218 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/README.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       61 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/constraints.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)     1022 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/docker-compose.yml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.387557 collective.listmonk-1.0.0a7/docs/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/docs/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)    28415 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/docs/dlr.svg
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.387930 collective.listmonk-1.0.0a7/news/
+-rw-r--r--   0 davisagli   (501) staff       (20)      308 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/news/.changelog_template.jinja
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/news/.gitkeep
+-rw-r--r--   0 davisagli   (501) staff       (20)     4793 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/pyproject.toml
+-rw-r--r--   0 davisagli   (501) staff       (20)       32 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/requirements.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-24 17:56:59.402110 collective.listmonk-1.0.0a7/setup.cfg
+-rw-r--r--   0 davisagli   (501) staff       (20)     2323 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/setup.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.383144 collective.listmonk-1.0.0a7/src/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.388095 collective.listmonk-1.0.0a7/src/collective/
+-rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.390775 collective.listmonk-1.0.0a7/src/collective/listmonk/
+-rw-r--r--   0 davisagli   (501) staff       (20)      199 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.391077 collective.listmonk-1.0.0a7/src/collective/listmonk/behaviors/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/behaviors/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/behaviors/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      465 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.391345 collective.listmonk-1.0.0a7/src/collective/listmonk/content/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/content/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3514 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/content/newsletter.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.391618 collective.listmonk-1.0.0a7/src/collective/listmonk/controlpanel/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/controlpanel/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      220 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/controlpanel/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      187 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/dependencies.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      232 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/interfaces.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1504 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/listmonk.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.392072 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3636 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/collective.listmonk.pot
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.383734 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/de/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.392251 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/de/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     3684 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.383890 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/en/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.392436 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/en/LC_MESSAGES/
+-rw-r--r--   0 davisagli   (501) staff       (20)     3047 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po
+-rw-r--r--   0 davisagli   (501) staff       (20)     2487 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/locales/update.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      404 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/permissions.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.384347 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.393158 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      182 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/metadata.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      585 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/rolemap.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.393348 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/types/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2764 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/types/Newsletter.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      185 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/types.xml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.393540 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/uninstall/
+-rw-r--r--   0 davisagli   (501) staff       (20)      122 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 davisagli   (501) staff       (20)      824 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/profiles.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.396294 collective.listmonk-1.0.0a7/src/collective/listmonk/services/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/services/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1592 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/services/base.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1261 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/services/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     6404 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/services/mailings.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     7498 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/services/subscriptions.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.398755 collective.listmonk-1.0.0a7/src/collective/listmonk/setuphandlers/
+-rw-r--r--   0 davisagli   (501) staff       (20)      339 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/setuphandlers/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3210 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/testing.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.399146 collective.listmonk-1.0.0a7/src/collective/listmonk/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/upgrades/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      140 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/src/collective/listmonk/upgrades/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.401005 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/
+-rw-r--r--   0 davisagli   (501) staff       (20)     7552 2024-04-24 17:56:59.000000 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     2449 2024-04-24 17:56:59.000000 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/SOURCES.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-24 17:56:59.000000 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/dependency_links.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)      124 2024-04-24 17:56:59.000000 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/entry_points.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-24 17:56:59.000000 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/namespace_packages.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-24 17:56:59.000000 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/not-zip-safe
+-rw-r--r--   0 davisagli   (501) staff       (20)      264 2024-04-24 17:56:59.000000 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/requires.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       11 2024-04-24 17:56:59.000000 collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/top_level.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.399475 collective.listmonk-1.0.0a7/tests/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/tests/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.400030 collective.listmonk-1.0.0a7/tests/api/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/tests/api/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4966 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/tests/api/test_mailings.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     5173 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/tests/api/test_subscriptions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3116 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/tests/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.400359 collective.listmonk-1.0.0a7/tests/setup/
+-rw-r--r--   0 davisagli   (501) staff       (20)      917 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/tests/setup/test_setup_install.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/tests/setup/test_setup_uninstall.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-24 17:56:59.400699 collective.listmonk-1.0.0a7/tests/setup/upgrades/
+-rw-r--r--   0 davisagli   (501) staff       (20)      645 2024-04-24 17:56:58.000000 collective.listmonk-1.0.0a7/tests/setup/upgrades/conftest.py
```

### Comparing `collective.listmonk-1.0.0a6/.editorconfig` & `collective.listmonk-1.0.0a7/.editorconfig`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/CHANGES.md` & `collective.listmonk-1.0.0a7/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a7 (2024-04-24)
+
+
+### Bug fixes:
+
+- If a subscriber unsubscribes but still has an unconfirmed subscription to another list, don't delete the subscriber. @davisagli #16
+- Fix translation of unsubscribe link. @davisagli #17
+
 ## 1.0.0a6 (2024-04-22)
 
 
 ### New features:
 
 - Unsubscribe links now include a subscriber UUID, so it's not possible to unsubscribe a different subscriber.
   Also, if the user is unsubscribed from all lists, the listmonk subscriber will be deleted, to avoid retaining private data. @davisagli #14
```

### Comparing `collective.listmonk-1.0.0a6/LICENSE.GPL` & `collective.listmonk-1.0.0a7/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/LICENSE.md` & `collective.listmonk-1.0.0a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/PKG-INFO` & `collective.listmonk-1.0.0a7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.listmonk
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: A Listmonk newsletter integration for Plone.
 Home-page: https://github.com/collective/collective.listmonk
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.listmonk
 Project-URL: Source, https://github.com/collective/collective.listmonk
@@ -207,14 +207,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a7 (2024-04-24)
+
+
+### Bug fixes:
+
+- If a subscriber unsubscribes but still has an unconfirmed subscription to another list, don't delete the subscriber. @davisagli #16
+- Fix translation of unsubscribe link. @davisagli #17
+
 ## 1.0.0a6 (2024-04-22)
 
 
 ### New features:
 
 - Unsubscribe links now include a subscriber UUID, so it's not possible to unsubscribe a different subscriber.
   Also, if the user is unsubscribed from all lists, the listmonk subscriber will be deleted, to avoid retaining private data. @davisagli #14
```

### Comparing `collective.listmonk-1.0.0a6/README.md` & `collective.listmonk-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/docker-compose.yml` & `collective.listmonk-1.0.0a7/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/docs/dlr.svg` & `collective.listmonk-1.0.0a7/docs/dlr.svg`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/pyproject.toml` & `collective.listmonk-1.0.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/setup.py` & `collective.listmonk-1.0.0a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {Path("CONTRIBUTORS.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 
 setup(
     name="collective.listmonk",
-    version="1.0.0a6",
+    version="1.0.0a7",
     description="A Listmonk newsletter integration for Plone.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/content/newsletter.py` & `collective.listmonk-1.0.0a7/src/collective/listmonk/content/newsletter.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         parts.append(
             translate(
                 _(
                     "email_mailing_footer",
                     default="---\nTo unsubscribe, please click on the following link:\n${unsubscribe_link}",
                     mapping={"unsubscribe_link": self.get_unsubscribe_link()},
                 ),
-                request,
+                context=request,
             )
         )
 
         return "\n\n".join(parts)
 
     def get_unsubscribe_link(self):
         request = getRequest()
```

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/listmonk.py` & `collective.listmonk-1.0.0a7/src/collective/listmonk/listmonk.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/locales/collective.listmonk.pot` & `collective.listmonk-1.0.0a7/src/collective/listmonk/locales/collective.listmonk.pot`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po` & `collective.listmonk-1.0.0a7/src/collective/listmonk/locales/de/LC_MESSAGES/collective.listmonk.po`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po` & `collective.listmonk-1.0.0a7/src/collective/listmonk/locales/en/LC_MESSAGES/collective.listmonk.po`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/locales/update.py` & `collective.listmonk-1.0.0a7/src/collective/listmonk/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/rolemap.xml` & `collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/profiles/default/types/Newsletter.xml` & `collective.listmonk-1.0.0a7/src/collective/listmonk/profiles/default/types/Newsletter.xml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/profiles.zcml` & `collective.listmonk-1.0.0a7/src/collective/listmonk/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/services/base.py` & `collective.listmonk-1.0.0a7/src/collective/listmonk/services/base.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/services/configure.zcml` & `collective.listmonk-1.0.0a7/src/collective/listmonk/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/services/mailings.py` & `collective.listmonk-1.0.0a7/src/collective/listmonk/services/mailings.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/services/subscriptions.py` & `collective.listmonk-1.0.0a7/src/collective/listmonk/services/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
         subscriber = listmonk.find_subscriber(uuid=data.sub_uuid)
         if subscriber is None:
             raise BadRequest("Subscription not found")
         current_lists = [
             list["id"]
             for list in subscriber["lists"]
-            if list["subscription_status"] == "confirmed"
+            if list["subscription_status"] != "unsubscribed"
         ]
         if set(current_lists) - set(list_ids):
             # Some subscriptions will remain.
             # Unsubscribe from the others.
             listmonk.call_listmonk(
                 "put",
                 "/subscribers/lists",
```

### Comparing `collective.listmonk-1.0.0a6/src/collective/listmonk/testing.py` & `collective.listmonk-1.0.0a7/src/collective/listmonk/testing.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/PKG-INFO` & `collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.listmonk
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: A Listmonk newsletter integration for Plone.
 Home-page: https://github.com/collective/collective.listmonk
 Author: kitconcept GmbH
 Author-email: info@kitconcept.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.listmonk
 Project-URL: Source, https://github.com/collective/collective.listmonk
@@ -207,14 +207,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a7 (2024-04-24)
+
+
+### Bug fixes:
+
+- If a subscriber unsubscribes but still has an unconfirmed subscription to another list, don't delete the subscriber. @davisagli #16
+- Fix translation of unsubscribe link. @davisagli #17
+
 ## 1.0.0a6 (2024-04-22)
 
 
 ### New features:
 
 - Unsubscribe links now include a subscriber UUID, so it's not possible to unsubscribe a different subscriber.
   Also, if the user is unsubscribed from all lists, the listmonk subscriber will be deleted, to avoid retaining private data. @davisagli #14
```

### Comparing `collective.listmonk-1.0.0a6/src/collective.listmonk.egg-info/SOURCES.txt` & `collective.listmonk-1.0.0a7/src/collective.listmonk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/tests/api/test_mailings.py` & `collective.listmonk-1.0.0a7/tests/api/test_mailings.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/tests/api/test_subscriptions.py` & `collective.listmonk-1.0.0a7/tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/tests/conftest.py` & `collective.listmonk-1.0.0a7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/tests/setup/test_setup_install.py` & `collective.listmonk-1.0.0a7/tests/setup/test_setup_install.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/tests/setup/test_setup_uninstall.py` & `collective.listmonk-1.0.0a7/tests/setup/test_setup_uninstall.py`

 * *Files identical despite different names*

### Comparing `collective.listmonk-1.0.0a6/tests/setup/upgrades/conftest.py` & `collective.listmonk-1.0.0a7/tests/setup/upgrades/conftest.py`

 * *Files identical despite different names*

