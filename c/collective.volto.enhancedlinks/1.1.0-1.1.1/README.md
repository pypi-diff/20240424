# Comparing `tmp/collective.volto.enhancedlinks-1.1.0.tar.gz` & `tmp/collective.volto.enhancedlinks-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.volto.enhancedlinks-1.1.0.tar", last modified: Mon Mar 18 14:16:27 2024, max compression
+gzip compressed data, was "collective.volto.enhancedlinks-1.1.1.tar", last modified: Wed Apr 24 07:10:40 2024, max compression
```

## Comparing `collective.volto.enhancedlinks-1.1.0.tar` & `collective.volto.enhancedlinks-1.1.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.413579 collective.volto.enhancedlinks-1.1.0/
--rw-r--r--   0 cekk       (501) staff       (20)       27 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/.isort.cfg
--rw-r--r--   0 cekk       (501) staff       (20)      413 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       73 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1338 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      681 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      233 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     4870 2024-03-18 14:16:27.413640 collective.volto.enhancedlinks-1.1.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3011 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)     2091 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/base.cfg
--rw-r--r--   0 cekk       (501) staff       (20)       79 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/bobtemplate.cfg
--rw-r--r--   0 cekk       (501) staff       (20)      215 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/buildout.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     3573 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/pyproject.toml
--rw-r--r--   0 cekk       (501) staff       (20)      340 2024-03-18 14:16:27.413877 collective.volto.enhancedlinks-1.1.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2791 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.405182 collective.volto.enhancedlinks-1.1.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.407904 collective.volto.enhancedlinks-1.1.0/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       56 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.408935 collective.volto.enhancedlinks-1.1.0/src/collective/volto/
--rw-r--r--   0 cekk       (501) staff       (20)       56 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.410139 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/
--rw-r--r--   0 cekk       (501) staff       (20)      123 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1074 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/adapters.py
--rw-r--r--   0 cekk       (501) staff       (20)      502 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/behaviors.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1733 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.410457 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/events/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/events/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      381 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/events/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      291 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/events/invalidate_cache.py
--rw-r--r--   0 cekk       (501) staff       (20)      213 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/indexer.py
--rw-r--r--   0 cekk       (501) staff       (20)      383 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.410966 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/collective.volto.enhancedlinks.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.405563 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.411202 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)       28 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/en/LC_MESSAGES/collective.volto.enhancedlinks.mo
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/en/LC_MESSAGES/collective.volto.enhancedlinks.po
--rw-r--r--   0 cekk       (501) staff       (20)     1742 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      527 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/update.sh
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.405805 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.411514 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      301 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      180 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)      188 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/default/toolset.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.411734 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/default/types/
--rw-r--r--   0 cekk       (501) staff       (20)      290 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/default/types/File.xml
--rw-r--r--   0 cekk       (501) staff       (20)      291 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/default/types/Image.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.411843 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      113 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/profiles/uninstall/toolset.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.412040 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      447 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.412354 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/deserializer/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/deserializer/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      841 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/deserializer/blocks.py
--rw-r--r--   0 cekk       (501) staff       (20)      525 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/deserializer/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.412683 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/serializer/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/serializer/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2861 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/serializer/blocks.py
--rw-r--r--   0 cekk       (501) staff       (20)      521 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/serializer/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      850 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1246 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.413020 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.413440 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/files/
--rw-r--r--   0 cekk       (501) staff       (20)     8561 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/files/file.pdf
--rw-r--r--   0 cekk       (501) staff       (20)       39 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/files/file_csv.csv
--rw-r--r--   0 cekk       (501) staff       (20)     5131 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/files/image.jpg
--rw-r--r--   0 cekk       (501) staff       (20)     5797 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/test_serializer.py
--rw-r--r--   0 cekk       (501) staff       (20)     5989 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/test_summary_serializer.py
--rw-r--r--   0 cekk       (501) staff       (20)     1734 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tool.py
--rw-r--r--   0 cekk       (501) staff       (20)      914 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)      371 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/upgrades.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-03-18 14:16:27.408829 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4870 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3179 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      135 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       28 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)       85 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)      344 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/test_plone52.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     1303 2024-03-18 14:16:27.000000 collective.volto.enhancedlinks-1.1.0/test_plone60.cfg
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.606403 collective.volto.enhancedlinks-1.1.1/
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/.isort.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)      506 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       73 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     1338 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      681 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      233 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     4963 2024-04-24 07:10:40.606457 collective.volto.enhancedlinks-1.1.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3011 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     2091 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/base.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)       79 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/bobtemplate.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)      215 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/buildout.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     3573 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/pyproject.toml
+-rw-r--r--   0 cekk       (501) staff       (20)      340 2024-04-24 07:10:40.606723 collective.volto.enhancedlinks-1.1.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2791 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.596221 collective.volto.enhancedlinks-1.1.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.599540 collective.volto.enhancedlinks-1.1.1/src/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)       56 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.600819 collective.volto.enhancedlinks-1.1.1/src/collective/volto/
+-rw-r--r--   0 cekk       (501) staff       (20)       56 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.602312 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/
+-rw-r--r--   0 cekk       (501) staff       (20)      123 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1074 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/adapters.py
+-rw-r--r--   0 cekk       (501) staff       (20)      502 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/behaviors.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1733 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.602686 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/events/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/events/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      381 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/events/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      291 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/events/invalidate_cache.py
+-rw-r--r--   0 cekk       (501) staff       (20)      213 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/indexer.py
+-rw-r--r--   0 cekk       (501) staff       (20)      383 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.603335 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/collective.volto.enhancedlinks.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.596630 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.603632 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)       28 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/en/LC_MESSAGES/collective.volto.enhancedlinks.mo
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/en/LC_MESSAGES/collective.volto.enhancedlinks.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1742 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      527 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/update.sh
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.596889 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.604037 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      301 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      180 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      188 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/default/toolset.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.604311 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)      290 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/default/types/File.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      291 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/default/types/Image.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.604442 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      113 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/profiles/uninstall/toolset.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.604695 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      447 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.605105 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/deserializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/deserializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      841 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/deserializer/blocks.py
+-rw-r--r--   0 cekk       (501) staff       (20)      525 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/deserializer/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.605495 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/serializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/serializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2861 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/serializer/blocks.py
+-rw-r--r--   0 cekk       (501) staff       (20)      521 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/serializer/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      850 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1246 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.605880 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.606271 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/files/
+-rw-r--r--   0 cekk       (501) staff       (20)     8561 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/files/file.pdf
+-rw-r--r--   0 cekk       (501) staff       (20)       39 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/files/file_csv.csv
+-rw-r--r--   0 cekk       (501) staff       (20)     5131 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/files/image.jpg
+-rw-r--r--   0 cekk       (501) staff       (20)     5797 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/test_serializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5989 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/test_summary_serializer.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1738 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tool.py
+-rw-r--r--   0 cekk       (501) staff       (20)      914 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)      371 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-04-24 07:10:40.600685 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     4963 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3179 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      135 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       28 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)       85 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      344 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/test_plone52.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     1303 2024-04-24 07:10:40.000000 collective.volto.enhancedlinks-1.1.1/test_plone60.cfg
```

### Comparing `collective.volto.enhancedlinks-1.1.0/DEVELOP.rst` & `collective.volto.enhancedlinks-1.1.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/LICENSE.GPL` & `collective.volto.enhancedlinks-1.1.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/LICENSE.rst` & `collective.volto.enhancedlinks-1.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/PKG-INFO` & `collective.volto.enhancedlinks-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.volto.enhancedlinks
-Version: 1.1.0
+Version: 1.1.1
 Summary: Enhance Volto text blocks to automatically append file size and mimetype to internal links
 Home-page: https://github.com/collective/RegioneER.volto.enhancedlinks
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.volto.enhancedlinks/
 Project-URL: Source, https://github.com/collective/RegioneER.volto.enhancedlinks
@@ -143,14 +143,21 @@
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
 
+1.1.1 (2024-04-24)
+------------------
+
+- Prevent write-on-read to each tool call.
+  [cekk]
+
+
 1.1.0 (2024-03-18)
 ------------------
 
 - Add tool to manage infos, removed memoize machinery
   [mamico]
 
 1.0.1 (2024-01-30)
```

### Comparing `collective.volto.enhancedlinks-1.1.0/README.rst` & `collective.volto.enhancedlinks-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/base.cfg` & `collective.volto.enhancedlinks-1.1.1/base.cfg`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/pyproject.toml` & `collective.volto.enhancedlinks-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/setup.py` & `collective.volto.enhancedlinks-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.volto.enhancedlinks",
-    version="1.1.0",
+    version="1.1.1",
     description="Enhance Volto text blocks to automatically append file size and mimetype to internal links",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/adapters.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/adapters.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/configure.zcml` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/README.rst` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/update.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/locales/update.sh` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/deserializer/blocks.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/deserializer/blocks.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/deserializer/configure.zcml` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/deserializer/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/serializer/blocks.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/serializer/blocks.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/restapi/serializer/configure.zcml` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/restapi/serializer/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/setuphandlers.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/testing.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/testing.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/files/file.pdf` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/files/file.pdf`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/files/image.jpg` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/files/image.jpg`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/test_serializer.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tests/test_summary_serializer.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tests/test_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/tool.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,12 +46,12 @@
                     # not a link to file/image
                     info = {}
                 else:
                     info = {
                         "getObjSize": brain.getObjSize,
                         "mime_type": brain.mime_type,
                     }
-        self._enhanced_links[uid] = info
+            self._enhanced_links[uid] = info
         return info
 
 
 InitializeClass(EnhancedLinksTool)
```

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective/volto/enhancedlinks/upgrades.py` & `collective.volto.enhancedlinks-1.1.1/src/collective/volto/enhancedlinks/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/PKG-INFO` & `collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.volto.enhancedlinks
-Version: 1.1.0
+Version: 1.1.1
 Summary: Enhance Volto text blocks to automatically append file size and mimetype to internal links
 Home-page: https://github.com/collective/RegioneER.volto.enhancedlinks
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/collective.volto.enhancedlinks/
 Project-URL: Source, https://github.com/collective/RegioneER.volto.enhancedlinks
@@ -143,14 +143,21 @@
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
 
+1.1.1 (2024-04-24)
+------------------
+
+- Prevent write-on-read to each tool call.
+  [cekk]
+
+
 1.1.0 (2024-03-18)
 ------------------
 
 - Add tool to manage infos, removed memoize machinery
   [mamico]
 
 1.0.1 (2024-01-30)
```

### Comparing `collective.volto.enhancedlinks-1.1.0/src/collective.volto.enhancedlinks.egg-info/SOURCES.txt` & `collective.volto.enhancedlinks-1.1.1/src/collective.volto.enhancedlinks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.volto.enhancedlinks-1.1.0/test_plone60.cfg` & `collective.volto.enhancedlinks-1.1.1/test_plone60.cfg`

 * *Files identical despite different names*

