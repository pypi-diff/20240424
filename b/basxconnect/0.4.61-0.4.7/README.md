# Comparing `tmp/basxconnect-0.4.61.tar.gz` & `tmp/basxconnect-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basxconnect-0.4.61.tar", last modified: Wed Apr 24 04:53:33 2024, max compression
+gzip compressed data, was "basxconnect-0.4.7.tar", last modified: Sun Jul 24 08:58:22 2022, max compression
```

## Comparing `basxconnect-0.4.61.tar` & `basxconnect-0.4.7.tar`

### file list

```diff
@@ -1,275 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.313243 basxconnect-0.4.61/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 04:53:19.000000 basxconnect-0.4.61/.bandit
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 04:53:19.000000 basxconnect-0.4.61/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.269243 basxconnect-0.4.61/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 04:53:19.000000 basxconnect-0.4.61/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 04:53:19.000000 basxconnect-0.4.61/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 04:53:19.000000 basxconnect-0.4.61/.github/workflows/automated_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-24 04:53:19.000000 basxconnect-0.4.61/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 04:53:19.000000 basxconnect-0.4.61/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 04:53:19.000000 basxconnect-0.4.61/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-24 04:53:19.000000 basxconnect-0.4.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 04:53:19.000000 basxconnect-0.4.61/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-24 04:53:33.313243 basxconnect-0.4.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-24 04:53:19.000000 basxconnect-0.4.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/basxconnect/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/basxconnect/contributions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/dynamic_preferences_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/contributions/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/contributions/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/basxconnect/contributions/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/contributions/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/basxconnect/contributions/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/contributions/locale/nb_NO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/basxconnect/contributions/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/locale/nb_NO/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/contributions/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/basxconnect/contributions/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/contributions/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.281243 basxconnect-0.4.61/basxconnect/contributions/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.285243 basxconnect-0.4.61/basxconnect/contributions/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)    16506 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/migrations/0002_alter_contribution_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/migrations/0003_alter_contribution__import.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/migrations/0004_auto_20211030_0955.py
--rw-r--r--   0 runner    (1001) docker     (127)    16516 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/migrations/0005_alter_contribution_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.285243 basxconnect-0.4.61/basxconnect/contributions/wizards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/wizards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12215 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/contributions/wizards/contributionsimport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.285243 basxconnect-0.4.61/basxconnect/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/dynamic_preferences_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.285243 basxconnect-0.4.61/basxconnect/core/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.285243 basxconnect-0.4.61/basxconnect/core/layouts/editperson/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.285243 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/base_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/contributions_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/documenttemplates_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/head.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/history_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/relationships_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.285243 basxconnect-0.4.61/basxconnect/core/layouts/editperson/legalperson/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/legalperson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/legalperson/base_data_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/legalperson/mailing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.289243 basxconnect-0.4.61/basxconnect/core/layouts/editperson/naturalperson/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/naturalperson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/naturalperson/mailing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.289243 basxconnect-0.4.61/basxconnect/core/layouts/editperson/personassociation/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/personassociation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/personassociation/base_data_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/editperson/personassociation/mailing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/layouts/settings_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/core/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/core/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.289243 basxconnect-0.4.61/basxconnect/core/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    24299 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/core/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.289243 basxconnect-0.4.61/basxconnect/core/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    26217 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/core/locale/nb_NO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.289243 basxconnect-0.4.61/basxconnect/core/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/locale/nb_NO/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/core/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.289243 basxconnect-0.4.61/basxconnect/core/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    26428 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.273243 basxconnect-0.4.61/basxconnect/core/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.289243 basxconnect-0.4.61/basxconnect/core/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    32849 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.297243 basxconnect-0.4.61/basxconnect/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)  2061154 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0002_auto_20210309_1750.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0003_auto_20210309_2221.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0004_auto_20210311_1851.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0005_auto_20210311_1851.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0006_auto_20210312_0016.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0007_auto_20210312_0054.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0008_auto_20210323_1456.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0009_auto_20210522_1817.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0010_auto_20210523_1140.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0011_auto_20210726_2047.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0012_auto_20210928_1158.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0013_auto_20210928_1445.py
--rw-r--r--   0 runner    (1001) docker     (127)    10894 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0014_auto_20210928_1512.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0015_rename_category_to_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0016_auto_20210928_1534.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0017_remove_person_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0018_term_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0019_alter_term_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0020_auto_20211005_1630.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0021_auto_20211007_0932.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0022_auto_20211018_1644.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0023_auto_20211030_0955.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0024_alter_term_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0025_alter_term_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0026_auto_20211216_0946.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0027_auto_20211223_1948.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0028_auto_20220404_1058.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0029_auto_20220429_1138.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0030_auto_20220602_1434.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0031_alter_email_person_alter_email_type_alter_fax_person_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0032_alter_historicallegalperson_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0033_historicalnaturalperson_maiden_name_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0034_term_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/0035_alter_email_type_alter_fax_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.297243 basxconnect-0.4.61/basxconnect/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/models/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/models/persons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/models/relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/search_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.297243 basxconnect-0.4.61/basxconnect/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/tests/test_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.297243 basxconnect-0.4.61/basxconnect/core/views/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/menu_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/core/views/person/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/person/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/person/person_browse_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/person/person_details_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/person/person_modals_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/person/search_person_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/relationship_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/settings_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/tag_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/term.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/views/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/core/wizards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/wizards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/core/wizards/add_person.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/invoicing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/dynamic_preferences_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/invoicing/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/invoicing/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/invoicing/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/invoicing/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/invoicing/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/invoicing/locale/nb_NO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/invoicing/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/locale/nb_NO/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/invoicing/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/invoicing/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/invoicing/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/invoicing/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.301243 basxconnect-0.4.61/basxconnect/invoicing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/migrations/0002_alter_invoice_note.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/migrations/0003_invoice_receipt_sent.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/invoicing/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.305243 basxconnect-0.4.61/basxconnect/mailer_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.305243 basxconnect-0.4.61/basxconnect/mailer_integration/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/abstract/mailer.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/dynamic_preferences_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.305243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.305243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/nb_NO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.305243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/nb_NO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/locale/nb_NO/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.305243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.277243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.305243 basxconnect-0.4.61/basxconnect/mailer_integration/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.305243 basxconnect-0.4.61/basxconnect/mailer_integration/mailchimp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/mailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/mailchimp/mailer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/mailchimp/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.309243 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0002_interest_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0003_alter_interest_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0004_auto_20210823_1424.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0005_alter_mailingpreferences_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0006_alter_mailingpreferences_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0007_alter_mailingpreferences_interests.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0008_alter_mailingpreferences_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0009_alter_mailingpreferences_email.py
--rw-r--r--   0 runner    (1001) docker     (127)   338885 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0010_mailingpreferences_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0011_invalidperson_newperson_synchronizationresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0012_auto_20211119_0830.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0013_mailingpreferences_latest_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0014_rename_mailingpreferences_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0015_synchronizationperson_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0016_remove_synchronizationperson_successfully_added.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0017_auto_20211122_1219.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0018_alter_synchronizationperson_sync_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0019_auto_20211210_1602.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0020_subscription_deleted.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0021_auto_20220106_0917.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0022_auto_20220118_1308.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0023_auto_20220517_1700.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0024_synchronizationperson_maybe_duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/signal_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/synchronize.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/mailer_integration/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.309243 basxconnect-0.4.61/basxconnect/projects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/projects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.309243 basxconnect-0.4.61/basxconnect/projects/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/projects/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/projects/migrations/0002_alter_project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/projects/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/projects/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 04:53:19.000000 basxconnect-0.4.61/basxconnect/projects/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:53:33.309243 basxconnect-0.4.61/basxconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-24 04:53:33.000000 basxconnect-0.4.61/basxconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-04-24 04:53:33.000000 basxconnect-0.4.61/basxconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:53:33.000000 basxconnect-0.4.61/basxconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:53:33.000000 basxconnect-0.4.61/basxconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 04:53:33.000000 basxconnect-0.4.61/basxconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 04:53:33.000000 basxconnect-0.4.61/basxconnect.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1033 2024-04-24 04:53:19.000000 basxconnect-0.4.61/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:53:33.313243 basxconnect-0.4.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-24 04:53:19.000000 basxconnect-0.4.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.488048 basxconnect-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-24 08:58:00.000000 basxconnect-0.4.7/.bandit
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-07-24 08:58:00.000000 basxconnect-0.4.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-07-24 08:58:00.000000 basxconnect-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2022-07-24 08:58:00.000000 basxconnect-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2022-07-24 08:58:00.000000 basxconnect-0.4.7/.github/workflows/automated_release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-07-24 08:58:00.000000 basxconnect-0.4.7/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-07-24 08:58:00.000000 basxconnect-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-24 08:58:00.000000 basxconnect-0.4.7/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-07-24 08:58:00.000000 basxconnect-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-07-24 08:58:00.000000 basxconnect-0.4.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-07-24 08:58:22.488048 basxconnect-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2703 2022-07-24 08:58:00.000000 basxconnect-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/basxconnect/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/basxconnect/contributions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/dynamic_preferences_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/contributions/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/contributions/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/basxconnect/contributions/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5968 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/contributions/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/basxconnect/contributions/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     6137 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/contributions/locale/nb_NO/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/basxconnect/contributions/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5963 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/locale/nb_NO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/contributions/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/basxconnect/contributions/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     6168 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/contributions/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.460048 basxconnect-0.4.7/basxconnect/contributions/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     7308 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.460048 basxconnect-0.4.7/basxconnect/contributions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)    14479 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16506 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/migrations/0002_alter_contribution_currency.py
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/migrations/0003_alter_contribution__import.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/migrations/0004_auto_20211030_0955.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.460048 basxconnect-0.4.7/basxconnect/contributions/wizards/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/wizards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12132 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/contributions/wizards/contributionsimport.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.460048 basxconnect-0.4.7/basxconnect/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/dynamic_preferences_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.460048 basxconnect-0.4.7/basxconnect/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)     6176 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/fixtures/base.de.json
+-rw-r--r--   0 runner    (1001) docker     (121)     5718 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/fixtures/base.en.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.460048 basxconnect-0.4.7/basxconnect/core/layouts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.460048 basxconnect-0.4.7/basxconnect/core/layouts/editperson/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.460048 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9361 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/base_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/contributions_tab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/documenttemplates_tab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/head.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4996 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/history_tab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4817 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/relationships_tab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4394 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.468048 basxconnect-0.4.7/basxconnect/core/layouts/editperson/legalperson/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/legalperson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/legalperson/base_data_tab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/legalperson/mailing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.472048 basxconnect-0.4.7/basxconnect/core/layouts/editperson/naturalperson/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/naturalperson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/naturalperson/mailing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.472048 basxconnect-0.4.7/basxconnect/core/layouts/editperson/personassociation/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/personassociation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/personassociation/base_data_tab.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/editperson/personassociation/mailing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/layouts/settings_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/core/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/core/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.472048 basxconnect-0.4.7/basxconnect/core/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    23605 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/core/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.472048 basxconnect-0.4.7/basxconnect/core/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    25765 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/core/locale/nb_NO/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.472048 basxconnect-0.4.7/basxconnect/core/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    24305 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/locale/nb_NO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/core/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.472048 basxconnect-0.4.7/basxconnect/core/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    25863 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/core/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.472048 basxconnect-0.4.7/basxconnect/core/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    32017 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.480048 basxconnect-0.4.7/basxconnect/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)  2061155 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0002_auto_20210309_1750.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0003_auto_20210309_2221.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0004_auto_20210311_1851.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0005_auto_20210311_1851.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0006_auto_20210312_0016.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0007_auto_20210312_0054.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0008_auto_20210323_1456.py
+-rw-r--r--   0 runner    (1001) docker     (121)      877 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0009_auto_20210522_1817.py
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0010_auto_20210523_1140.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0011_auto_20210726_2047.py
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0012_auto_20210928_1158.py
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0013_auto_20210928_1445.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10895 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0014_auto_20210928_1512.py
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0015_rename_category_to_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0016_auto_20210928_1534.py
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0017_remove_person_categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0018_term_slug.py
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0019_alter_term_slug.py
+-rw-r--r--   0 runner    (1001) docker     (121)      603 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0020_auto_20211005_1630.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0021_auto_20211007_0932.py
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0022_auto_20211018_1644.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3881 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0023_auto_20211030_0955.py
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0024_alter_term_slug.py
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0025_alter_term_slug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0026_auto_20211216_0946.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0027_auto_20211223_1948.py
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0028_auto_20220404_1058.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0029_auto_20220429_1138.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0030_auto_20220602_1434.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3106 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/0031_alter_email_person_alter_email_type_alter_fax_person_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.480048 basxconnect-0.4.7/basxconnect/core/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4337 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/models/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12893 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/models/persons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/models/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/search_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.480048 basxconnect-0.4.7/basxconnect/core/static/
+-rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.480048 basxconnect-0.4.7/basxconnect/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/tests/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7539 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.480048 basxconnect-0.4.7/basxconnect/core/views/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/menu_views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.480048 basxconnect-0.4.7/basxconnect/core/views/person/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/person/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19672 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/person/person_browse_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7446 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/person/person_details_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8560 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/person/person_modals_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/person/search_person_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/relationship_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/settings_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4532 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/tag_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/term.py
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/views/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.480048 basxconnect-0.4.7/basxconnect/core/wizards/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/wizards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13732 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/core/wizards/add_person.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.484048 basxconnect-0.4.7/basxconnect/mailer_integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.484048 basxconnect-0.4.7/basxconnect/mailer_integration/abstract/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2160 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/abstract/mailer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/dynamic_preferences_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/help.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5751 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.484048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     6512 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.484048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5619 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/nb_NO/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.484048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5573 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/locale/nb_NO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.484048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     5620 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.452048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.484048 basxconnect-0.4.7/basxconnect/mailer_integration/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     7182 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.484048 basxconnect-0.4.7/basxconnect/mailer_integration/mailchimp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/mailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5344 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/mailchimp/mailer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/mailchimp/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.488048 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0002_interest_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0003_alter_interest_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0004_auto_20210823_1424.py
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0005_alter_mailingpreferences_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0006_alter_mailingpreferences_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0007_alter_mailingpreferences_interests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0008_alter_mailingpreferences_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0009_alter_mailingpreferences_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)   338886 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0010_mailingpreferences_language.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2457 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0011_invalidperson_newperson_synchronizationresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0012_auto_20211119_0830.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0013_mailingpreferences_latest_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0014_rename_mailingpreferences_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0015_synchronizationperson_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0016_remove_synchronizationperson_successfully_added.py
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0017_auto_20211122_1219.py
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0018_alter_synchronizationperson_sync_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0019_auto_20211210_1602.py
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0020_subscription_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0021_auto_20220106_0917.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0022_auto_20220118_1308.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0023_auto_20220517_1700.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/signal_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5704 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/synchronize.py
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6373 2022-07-24 08:58:00.000000 basxconnect-0.4.7/basxconnect/mailer_integration/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-24 08:58:22.456048 basxconnect-0.4.7/basxconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-07-24 08:58:22.000000 basxconnect-0.4.7/basxconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8804 2022-07-24 08:58:22.000000 basxconnect-0.4.7/basxconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-24 08:58:22.000000 basxconnect-0.4.7/basxconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-24 08:58:22.000000 basxconnect-0.4.7/basxconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-07-24 08:58:22.000000 basxconnect-0.4.7/basxconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-24 08:58:22.000000 basxconnect-0.4.7/basxconnect.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      968 2022-07-24 08:58:00.000000 basxconnect-0.4.7/manage.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-24 08:58:22.488048 basxconnect-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-07-24 08:58:00.000000 basxconnect-0.4.7/setup.py
```

### Comparing `basxconnect-0.4.61/.github/ISSUE_TEMPLATE/bug_report.md` & `basxconnect-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/.github/ISSUE_TEMPLATE/feature_request.md` & `basxconnect-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/.github/workflows/automated_release.yml` & `basxconnect-0.4.7/.github/workflows/automated_release.yml`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/.github/workflows/main.yml` & `basxconnect-0.4.7/.github/workflows/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     - name: Run bandit
       run: bandit -c .bandit -r basxconnect
 
     - name: Run safety
       run: safety check
 
     - name: Test basxconnect
-      run: python manage.py test basxbread .
+      run: python manage.py test bread .
```

### Comparing `basxconnect-0.4.61/LICENSE` & `basxconnect-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/Makefile` & `basxconnect-0.4.7/Makefile`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/PKG-INFO` & `basxconnect-0.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 Metadata-Version: 2.1
 Name: basxconnect
-Version: 0.4.61
+Version: 0.4.7
 Summary: CRM application for non-profit organizations
 Home-page: https://github.com/basxsoftwareassociation/basxconnect
 Author: basx Software Association
 Author-email: sam@basx.dev
 License: New BSD License
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: basx-bread
-Requires-Dist: django-formtools==2.3
-Requires-Dist: djangorestframework
-Requires-Dist: chardet
-Requires-Dist: tablib
-Requires-Dist: dateparser
 Provides-Extra: testing
-Requires-Dist: basx-bread[testing]; extra == "testing"
 Provides-Extra: mailer-integration
-Requires-Dist: mailchimp_marketing; extra == "mailer-integration"
+License-File: LICENSE
 
 [![basxconnect-ci](https://github.com/basxsoftwareassociation/basxconnect/actions/workflows/main.yml/badge.svg)](https://github.com/basxsoftwareassociation/basxconnect/actions/workflows/main.yml)
 [![Translation status](https://hosted.weblate.org/widgets/basxconnect/-/svg-badge.svg)](https://hosted.weblate.org/engage/basxconnect/)
 
 basxconnect
 ===========
 
@@ -58,31 +51,26 @@
 What we have so far
 -------------------
 
 - Integration of the core parts of carbon design in django (*"like bootstrap for django"*)
 - CRUD-framework (*"Quick generation of create/read/update/delete views"*)
 - HTML-layout framework which allows a more flexible hooking-in than the standard HTML-rendering mechanisms (*"DOM on the server side"*)
 - Core model to manage people, communication and relationships
-- Additional modules for:
-  - Generating reports
-  - Generating documents and PDFs from word templates
-  - Custom add/edit forms
-  - Data import from PDFs with form-fields
-  - Customiable Database triggers to send notification emails
-  - Invoicing module
 - Demo project which implements a bare-bone version of a *product* (this repository)
 
 What we still need to do
 ------------------------
 
+- Adding a workflow engine which allows code-based configuration of manual and automated workflows (e.g. uploading a file, waiting for approval from a certain role, sending out an email automatically, etc.)
 - Improving the existing code base to have better support for extendability
 - Write documentation where necessary and add code-examples and how-to's
 - Implement revisions completely to allow going to a certain date and maybe display diffs
 
 Other TODOs:
 - Explain more why basxConnect is necessary and the difference to alternative solutions
 
 We would like to thank the following projects for their work, they provide a valuable base for basxConnect:
 
 - Translation: https://weblate.org/
 - Design System: https://www.carbondesignsystem.com/
 
+
```

### Comparing `basxconnect-0.4.61/README.md` & `basxconnect-0.4.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -30,31 +30,24 @@
 What we have so far
 -------------------
 
 - Integration of the core parts of carbon design in django (*"like bootstrap for django"*)
 - CRUD-framework (*"Quick generation of create/read/update/delete views"*)
 - HTML-layout framework which allows a more flexible hooking-in than the standard HTML-rendering mechanisms (*"DOM on the server side"*)
 - Core model to manage people, communication and relationships
-- Additional modules for:
-  - Generating reports
-  - Generating documents and PDFs from word templates
-  - Custom add/edit forms
-  - Data import from PDFs with form-fields
-  - Customiable Database triggers to send notification emails
-  - Invoicing module
 - Demo project which implements a bare-bone version of a *product* (this repository)
 
 What we still need to do
 ------------------------
 
+- Adding a workflow engine which allows code-based configuration of manual and automated workflows (e.g. uploading a file, waiting for approval from a certain role, sending out an email automatically, etc.)
 - Improving the existing code base to have better support for extendability
 - Write documentation where necessary and add code-examples and how-to's
 - Implement revisions completely to allow going to a certain date and maybe display diffs
 
 Other TODOs:
 - Explain more why basxConnect is necessary and the difference to alternative solutions
 
 We would like to thank the following projects for their work, they provide a valuable base for basxConnect:
 
 - Translation: https://weblate.org/
 - Design System: https://www.carbondesignsystem.com/
-
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/dynamic_preferences_registry.py` & `basxconnect-0.4.7/basxconnect/contributions/dynamic_preferences_registry.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/contributions/locale/de/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/contributions/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
-"PO-Revision-Date: 2023-04-05 02:46+0000\n"
-"Last-Translator: Sam <saemideluxe@gmx.ch>\n"
-"Language-Team: German <https://hosted.weblate.org/projects/basxconnect/"
-"basxconnect-contributions/de/>\n"
-"Language: de\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.17-dev\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: basxconnect/contributions/dynamic_preferences_registry.py:7
 #: basxconnect/contributions/models.py:89 basxconnect/contributions/urls.py:53
 msgid "Contributions"
 msgstr "Zuwendungen"
 
 #: basxconnect/contributions/dynamic_preferences_registry.py:15
 msgid "Preferred Currency"
 msgstr "Bevorzute Währung"
 
 #: basxconnect/contributions/models.py:18
 #: basxconnect/contributions/models.py:71
-#: basxconnect/contributions/wizards/contributionsimport.py:142
+#: basxconnect/contributions/wizards/contributionsimport.py:140
 msgid "Date"
 msgstr "Datum"
 
 #: basxconnect/contributions/models.py:19 basxconnect/contributions/urls.py:25
 msgid "Importfile"
 msgstr "Importdatei"
 
@@ -48,15 +47,15 @@
 
 #: basxconnect/contributions/models.py:33
 msgid "Number of bookings"
 msgstr "Anzahl Buchungen"
 
 #: basxconnect/contributions/models.py:46
 msgid "Total amount"
-msgstr "Betrag Total"
+msgstr "Gesamtbetrag"
 
 #: basxconnect/contributions/models.py:52
 msgid "Contribution Import"
 msgstr "Zuwendungsimport"
 
 #: basxconnect/contributions/models.py:53
 msgid "Contributions Imports"
@@ -67,29 +66,29 @@
 msgstr "Import"
 
 #: basxconnect/contributions/models.py:69
 msgid "Person"
 msgstr "Person"
 
 #: basxconnect/contributions/models.py:72
-#: basxconnect/contributions/wizards/contributionsimport.py:143
+#: basxconnect/contributions/wizards/contributionsimport.py:141
 msgid "Note"
 msgstr "Buchungstext"
 
 #: basxconnect/contributions/models.py:73
 msgid "Debit Account"
 msgstr "Konto"
 
 #: basxconnect/contributions/models.py:74
 msgid "Credit Account"
 msgstr "Kostenstelle"
 
 #: basxconnect/contributions/models.py:75
 #: basxconnect/contributions/models.py:82
-#: basxconnect/contributions/wizards/contributionsimport.py:174
+#: basxconnect/contributions/wizards/contributionsimport.py:172
 msgid "Amount"
 msgstr "Betrag"
 
 #: basxconnect/contributions/models.py:76
 msgid "Currency"
 msgstr "Währung"
 
@@ -101,108 +100,108 @@
 msgid "Import date"
 msgstr "Importdatum"
 
 #: basxconnect/contributions/urls.py:47
 msgid "Imports"
 msgstr "Importe"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:90
+#: basxconnect/contributions/wizards/contributionsimport.py:88
 msgid "Upload a file"
 msgstr "Datei heraufladen"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:92
+#: basxconnect/contributions/wizards/contributionsimport.py:90
 msgid "File to import"
 msgstr "Zu importierende Datei"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:92
+#: basxconnect/contributions/wizards/contributionsimport.py:90
 msgid "Choose a CSV file"
 msgstr "CSV Datei auswählen"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:95
+#: basxconnect/contributions/wizards/contributionsimport.py:93
 msgid "First line is header"
 msgstr "Erste Zeile ist Kopfzeile"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:98
+#: basxconnect/contributions/wizards/contributionsimport.py:96
 msgid "Filter out duplicates"
 msgstr "Duplikate herausfiltern"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:103
+#: basxconnect/contributions/wizards/contributionsimport.py:101
 msgid "Import options"
 msgstr "Importoptionen"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:112
+#: basxconnect/contributions/wizards/contributionsimport.py:110
 msgid "Required field"
 msgstr "Erforderliches Feld"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:133
+#: basxconnect/contributions/wizards/contributionsimport.py:131
 msgid "CSV import problem: "
 msgstr "Problem beim CSV import: "
 
-#: basxconnect/contributions/wizards/contributionsimport.py:138
+#: basxconnect/contributions/wizards/contributionsimport.py:136
 msgid "Assignment"
 msgstr "Zuweisung"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:145
+#: basxconnect/contributions/wizards/contributionsimport.py:143
 msgid "Account"
 msgstr "Konto"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:148
+#: basxconnect/contributions/wizards/contributionsimport.py:146
 msgid "Cost Center"
 msgstr "Kostenstelle"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:151
+#: basxconnect/contributions/wizards/contributionsimport.py:149
 msgid "Person Number"
 msgstr "Personennummer"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:154
+#: basxconnect/contributions/wizards/contributionsimport.py:152
 msgid "Donor Number"
 msgstr "Spendernummer"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:157
+#: basxconnect/contributions/wizards/contributionsimport.py:155
 msgid "Assignment state"
 msgstr "Zuweisungsstatus"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:178
+#: basxconnect/contributions/wizards/contributionsimport.py:176
 msgid "Overview of contributions to import"
 msgstr "Überblick der zu importierenden Buchungen"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:184
+#: basxconnect/contributions/wizards/contributionsimport.py:182
 msgid "contributions"
 msgstr "Zuwendungen"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:188
+#: basxconnect/contributions/wizards/contributionsimport.py:186
 msgid "Sum"
 msgstr "Summe"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:219
+#: basxconnect/contributions/wizards/contributionsimport.py:217
 msgid " contributions could not been assigned"
 msgstr " Zuwendungen konnten nicht zugewiesen werden"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:222
+#: basxconnect/contributions/wizards/contributionsimport.py:220
 msgid ""
 "Please make sure that each entry has contributor number which matches with a "
 "person number and do the import again"
 msgstr ""
 "Bitte stellen Sie sicher, dass jeder Eintrag eine Spenennummer hat welche "
 "mit der Stammnummer einer Person aus der Datenbank übereinstimmt und "
 "versuchen Sie erneut zu importieren"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:228
+#: basxconnect/contributions/wizards/contributionsimport.py:226
 msgid "Cancel import"
 msgstr "Import abbrechen"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:234
+#: basxconnect/contributions/wizards/contributionsimport.py:232
 msgid "Assignment complete"
 msgstr "Zuweisung vollstängid"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:235
+#: basxconnect/contributions/wizards/contributionsimport.py:233
 msgid "Continue in order to complete the import"
 msgstr "Weiterfahren um den Import abzuschliessen"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:296
+#: basxconnect/contributions/wizards/contributionsimport.py:294
 msgid "Import contributions"
 msgstr "Zuwendungen importieren"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:311
+#: basxconnect/contributions/wizards/contributionsimport.py:309
 #, python-format
 msgid "Successfully imported %d contributions"
 msgstr "%d Zuwendungen wurden erfolgreich importiert"
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/locale/fr/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/contributions/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: 2021-03-25 02:49+0000\n"
 "Last-Translator: Nathan <bonnemainsnathan@gmail.com>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/basxconnect/"
 "basxconnect-contributions/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -26,15 +26,15 @@
 
 #: basxconnect/contributions/dynamic_preferences_registry.py:15
 msgid "Preferred Currency"
 msgstr "Devise de préférence"
 
 #: basxconnect/contributions/models.py:18
 #: basxconnect/contributions/models.py:71
-#: basxconnect/contributions/wizards/contributionsimport.py:142
+#: basxconnect/contributions/wizards/contributionsimport.py:140
 msgid "Date"
 msgstr "Date"
 
 #: basxconnect/contributions/models.py:19 basxconnect/contributions/urls.py:25
 msgid "Importfile"
 msgstr "Fichier d'import"
 
@@ -67,29 +67,29 @@
 msgstr "Importer"
 
 #: basxconnect/contributions/models.py:69
 msgid "Person"
 msgstr "Personne"
 
 #: basxconnect/contributions/models.py:72
-#: basxconnect/contributions/wizards/contributionsimport.py:143
+#: basxconnect/contributions/wizards/contributionsimport.py:141
 msgid "Note"
 msgstr "Remarque"
 
 #: basxconnect/contributions/models.py:73
 msgid "Debit Account"
 msgstr "Compte débiteur"
 
 #: basxconnect/contributions/models.py:74
 msgid "Credit Account"
 msgstr "Compte créditeur"
 
 #: basxconnect/contributions/models.py:75
 #: basxconnect/contributions/models.py:82
-#: basxconnect/contributions/wizards/contributionsimport.py:174
+#: basxconnect/contributions/wizards/contributionsimport.py:172
 msgid "Amount"
 msgstr "Montant"
 
 #: basxconnect/contributions/models.py:76
 msgid "Currency"
 msgstr "Devise"
 
@@ -101,107 +101,107 @@
 msgid "Import date"
 msgstr "Date d'import"
 
 #: basxconnect/contributions/urls.py:47
 msgid "Imports"
 msgstr "Imports"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:90
+#: basxconnect/contributions/wizards/contributionsimport.py:88
 msgid "Upload a file"
 msgstr "Importer un fichier"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:92
+#: basxconnect/contributions/wizards/contributionsimport.py:90
 msgid "File to import"
 msgstr "Fichier à importer"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:92
+#: basxconnect/contributions/wizards/contributionsimport.py:90
 msgid "Choose a CSV file"
 msgstr "Sélectionnez un fichier CSV"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:95
+#: basxconnect/contributions/wizards/contributionsimport.py:93
 msgid "First line is header"
 msgstr "La première ligne correspond à l'en-tête"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:98
+#: basxconnect/contributions/wizards/contributionsimport.py:96
 msgid "Filter out duplicates"
 msgstr "Filtrer les doublons"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:103
+#: basxconnect/contributions/wizards/contributionsimport.py:101
 msgid "Import options"
 msgstr "Options d'import"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:112
+#: basxconnect/contributions/wizards/contributionsimport.py:110
 msgid "Required field"
 msgstr "Champ requis"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:133
+#: basxconnect/contributions/wizards/contributionsimport.py:131
 msgid "CSV import problem: "
 msgstr "Problème d'import du fichier CSV : "
 
-#: basxconnect/contributions/wizards/contributionsimport.py:138
+#: basxconnect/contributions/wizards/contributionsimport.py:136
 msgid "Assignment"
 msgstr "Affectation"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:145
+#: basxconnect/contributions/wizards/contributionsimport.py:143
 msgid "Account"
 msgstr "Compte"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:148
+#: basxconnect/contributions/wizards/contributionsimport.py:146
 msgid "Cost Center"
 msgstr "Centre de coûts"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:151
+#: basxconnect/contributions/wizards/contributionsimport.py:149
 msgid "Person Number"
 msgstr "Numéro de personne"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:154
+#: basxconnect/contributions/wizards/contributionsimport.py:152
 msgid "Donor Number"
 msgstr "Numéro de donateur"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:157
+#: basxconnect/contributions/wizards/contributionsimport.py:155
 msgid "Assignment state"
 msgstr "État de l'affectation"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:178
+#: basxconnect/contributions/wizards/contributionsimport.py:176
 msgid "Overview of contributions to import"
 msgstr "Aperçu des contributions à importer"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:184
+#: basxconnect/contributions/wizards/contributionsimport.py:182
 msgid "contributions"
 msgstr "contributions"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:188
+#: basxconnect/contributions/wizards/contributionsimport.py:186
 msgid "Sum"
 msgstr "Somme"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:219
+#: basxconnect/contributions/wizards/contributionsimport.py:217
 msgid " contributions could not been assigned"
 msgstr " contributions n'ont pas pu être affectées"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:222
+#: basxconnect/contributions/wizards/contributionsimport.py:220
 msgid ""
 "Please make sure that each entry has contributor number which matches with a "
 "person number and do the import again"
 msgstr ""
 "Veuillez vérifier que chaque entrée contienne un numéro de contributeur "
 "correspondant à un numéro de personne et recommencez l'importation"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:228
+#: basxconnect/contributions/wizards/contributionsimport.py:226
 msgid "Cancel import"
 msgstr "Annuler l'import"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:234
+#: basxconnect/contributions/wizards/contributionsimport.py:232
 msgid "Assignment complete"
 msgstr "Affectation terminée"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:235
+#: basxconnect/contributions/wizards/contributionsimport.py:233
 msgid "Continue in order to complete the import"
 msgstr "Continuez afin de compléter l'import"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:296
+#: basxconnect/contributions/wizards/contributionsimport.py:294
 msgid "Import contributions"
 msgstr "Importer des contibutions"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:311
+#: basxconnect/contributions/wizards/contributionsimport.py:309
 #, python-format
 msgid "Successfully imported %d contributions"
 msgstr "%d contributions ont bien été importées"
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/locale/pt/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/contributions/locale/pt/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: 2021-05-08 22:32+0000\n"
 "Last-Translator: ssantos <ssantos@web.de>\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/basxconnect/"
 "basxconnect-contributions/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -26,15 +26,15 @@
 
 #: basxconnect/contributions/dynamic_preferences_registry.py:15
 msgid "Preferred Currency"
 msgstr "Moeda de preferência"
 
 #: basxconnect/contributions/models.py:18
 #: basxconnect/contributions/models.py:71
-#: basxconnect/contributions/wizards/contributionsimport.py:142
+#: basxconnect/contributions/wizards/contributionsimport.py:140
 msgid "Date"
 msgstr "Data"
 
 #: basxconnect/contributions/models.py:19 basxconnect/contributions/urls.py:25
 msgid "Importfile"
 msgstr "Importar ficheiro"
 
@@ -67,29 +67,29 @@
 msgstr "Importação"
 
 #: basxconnect/contributions/models.py:69
 msgid "Person"
 msgstr "Pessoa"
 
 #: basxconnect/contributions/models.py:72
-#: basxconnect/contributions/wizards/contributionsimport.py:143
+#: basxconnect/contributions/wizards/contributionsimport.py:141
 msgid "Note"
 msgstr "Nota"
 
 #: basxconnect/contributions/models.py:73
 msgid "Debit Account"
 msgstr "Conta de débito"
 
 #: basxconnect/contributions/models.py:74
 msgid "Credit Account"
 msgstr "Conta de crédito"
 
 #: basxconnect/contributions/models.py:75
 #: basxconnect/contributions/models.py:82
-#: basxconnect/contributions/wizards/contributionsimport.py:174
+#: basxconnect/contributions/wizards/contributionsimport.py:172
 msgid "Amount"
 msgstr "Montante"
 
 #: basxconnect/contributions/models.py:76
 msgid "Currency"
 msgstr "Moeda"
 
@@ -101,107 +101,107 @@
 msgid "Import date"
 msgstr "Data de Importação"
 
 #: basxconnect/contributions/urls.py:47
 msgid "Imports"
 msgstr "Importações"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:90
+#: basxconnect/contributions/wizards/contributionsimport.py:88
 msgid "Upload a file"
 msgstr "Carregue um ficheiro"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:92
+#: basxconnect/contributions/wizards/contributionsimport.py:90
 msgid "File to import"
 msgstr "Ficheiro para importar"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:92
+#: basxconnect/contributions/wizards/contributionsimport.py:90
 msgid "Choose a CSV file"
 msgstr "Escolha um ficheiro CSV"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:95
+#: basxconnect/contributions/wizards/contributionsimport.py:93
 msgid "First line is header"
 msgstr "Primeira linha é o cabeçalho"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:98
+#: basxconnect/contributions/wizards/contributionsimport.py:96
 msgid "Filter out duplicates"
 msgstr "Filtrar duplicados"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:103
+#: basxconnect/contributions/wizards/contributionsimport.py:101
 msgid "Import options"
 msgstr "Opções de importação"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:112
+#: basxconnect/contributions/wizards/contributionsimport.py:110
 msgid "Required field"
 msgstr "Campo obrigatório"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:133
+#: basxconnect/contributions/wizards/contributionsimport.py:131
 msgid "CSV import problem: "
 msgstr "Problema de importação do CSV: "
 
-#: basxconnect/contributions/wizards/contributionsimport.py:138
+#: basxconnect/contributions/wizards/contributionsimport.py:136
 msgid "Assignment"
 msgstr "Assinatura"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:145
+#: basxconnect/contributions/wizards/contributionsimport.py:143
 msgid "Account"
 msgstr "Conta"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:148
+#: basxconnect/contributions/wizards/contributionsimport.py:146
 msgid "Cost Center"
 msgstr "Centro de Custos"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:151
+#: basxconnect/contributions/wizards/contributionsimport.py:149
 msgid "Person Number"
 msgstr "Número da Pessoa"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:154
+#: basxconnect/contributions/wizards/contributionsimport.py:152
 msgid "Donor Number"
 msgstr "Número de Doador"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:157
+#: basxconnect/contributions/wizards/contributionsimport.py:155
 msgid "Assignment state"
 msgstr "Estado de atribuição"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:178
+#: basxconnect/contributions/wizards/contributionsimport.py:176
 msgid "Overview of contributions to import"
 msgstr "Visão geral das contribuições para a importação"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:184
+#: basxconnect/contributions/wizards/contributionsimport.py:182
 msgid "contributions"
 msgstr "contribuições"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:188
+#: basxconnect/contributions/wizards/contributionsimport.py:186
 msgid "Sum"
 msgstr "Soma"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:219
+#: basxconnect/contributions/wizards/contributionsimport.py:217
 msgid " contributions could not been assigned"
 msgstr " as contribuições não puderam ser atribuídas"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:222
+#: basxconnect/contributions/wizards/contributionsimport.py:220
 msgid ""
 "Please make sure that each entry has contributor number which matches with a "
 "person number and do the import again"
 msgstr ""
 "Certifique-se de que cada entrada tem um número de contribuinte que coincide "
 "com um número da pessoa e faça novamente a importação"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:228
+#: basxconnect/contributions/wizards/contributionsimport.py:226
 msgid "Cancel import"
 msgstr "Cancelar importação"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:234
+#: basxconnect/contributions/wizards/contributionsimport.py:232
 msgid "Assignment complete"
 msgstr "Cessão completa"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:235
+#: basxconnect/contributions/wizards/contributionsimport.py:233
 msgid "Continue in order to complete the import"
 msgstr "Continuar de forma a completar a importação"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:296
+#: basxconnect/contributions/wizards/contributionsimport.py:294
 msgid "Import contributions"
 msgstr "Importação de contribuições"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:311
+#: basxconnect/contributions/wizards/contributionsimport.py:309
 #, python-format
 msgid "Successfully imported %d contributions"
 msgstr "Contribuições %d importadas com sucesso"
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/locale/th/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/contributions/locale/th/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
-"PO-Revision-Date: 2023-04-05 02:46+0000\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
+"PO-Revision-Date: 2021-10-20 02:32+0000\n"
 "Last-Translator: Tidaphan <tida@basx.dev>\n"
 "Language-Team: Thai <https://hosted.weblate.org/projects/basxconnect/"
 "basxconnect-contributions/th/>\n"
 "Language: th\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.17-dev\n"
+"X-Generator: Weblate 4.9-dev\n"
 
 #: basxconnect/contributions/dynamic_preferences_registry.py:7
 #: basxconnect/contributions/models.py:89 basxconnect/contributions/urls.py:53
 msgid "Contributions"
 msgstr "เงินบริจาค"
 
 #: basxconnect/contributions/dynamic_preferences_registry.py:15
 msgid "Preferred Currency"
 msgstr "สกุลเงิน"
 
 #: basxconnect/contributions/models.py:18
 #: basxconnect/contributions/models.py:71
-#: basxconnect/contributions/wizards/contributionsimport.py:142
+#: basxconnect/contributions/wizards/contributionsimport.py:140
 msgid "Date"
 msgstr "วันที่"
 
 #: basxconnect/contributions/models.py:19 basxconnect/contributions/urls.py:25
 msgid "Importfile"
 msgstr "นำเข้าไฟล์"
 
@@ -48,15 +48,15 @@
 
 #: basxconnect/contributions/models.py:33
 msgid "Number of bookings"
 msgstr "หมายเลขการจอง"
 
 #: basxconnect/contributions/models.py:46
 msgid "Total amount"
-msgstr "ยอดรวมจำนวน"
+msgstr "จำนวนรวม"
 
 #: basxconnect/contributions/models.py:52
 msgid "Contribution Import"
 msgstr "นำเข้าเงินบริจาค"
 
 #: basxconnect/contributions/models.py:53
 msgid "Contributions Imports"
@@ -67,29 +67,29 @@
 msgstr "นำเข้า"
 
 #: basxconnect/contributions/models.py:69
 msgid "Person"
 msgstr "บุคคล"
 
 #: basxconnect/contributions/models.py:72
-#: basxconnect/contributions/wizards/contributionsimport.py:143
+#: basxconnect/contributions/wizards/contributionsimport.py:141
 msgid "Note"
 msgstr "บันทึกเพิ่ม"
 
 #: basxconnect/contributions/models.py:73
 msgid "Debit Account"
 msgstr "บัญชีเดบิต"
 
 #: basxconnect/contributions/models.py:74
 msgid "Credit Account"
 msgstr "บัญชีเครดิต"
 
 #: basxconnect/contributions/models.py:75
 #: basxconnect/contributions/models.py:82
-#: basxconnect/contributions/wizards/contributionsimport.py:174
+#: basxconnect/contributions/wizards/contributionsimport.py:172
 msgid "Amount"
 msgstr "จำนวน"
 
 #: basxconnect/contributions/models.py:76
 msgid "Currency"
 msgstr "สกุลเงิน"
 
@@ -101,108 +101,108 @@
 msgid "Import date"
 msgstr "วันที่นำเข้า"
 
 #: basxconnect/contributions/urls.py:47
 msgid "Imports"
 msgstr "นำเข้า"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:90
+#: basxconnect/contributions/wizards/contributionsimport.py:88
 msgid "Upload a file"
 msgstr "อัพโหลดไฟล์"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:92
+#: basxconnect/contributions/wizards/contributionsimport.py:90
 msgid "File to import"
 msgstr "ไฟล์สำหรับนำเข้า"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:92
+#: basxconnect/contributions/wizards/contributionsimport.py:90
 msgid "Choose a CSV file"
 msgstr "เลือกไฟล์ CSV"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:95
+#: basxconnect/contributions/wizards/contributionsimport.py:93
 msgid "First line is header"
 msgstr "หัวเรื่องบรรทัดแรก"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:98
+#: basxconnect/contributions/wizards/contributionsimport.py:96
 msgid "Filter out duplicates"
 msgstr "คัดกรองรายการที่ซ้ำกัน"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:103
+#: basxconnect/contributions/wizards/contributionsimport.py:101
 msgid "Import options"
 msgstr "ตัวเลือกการนำเข้า"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:112
+#: basxconnect/contributions/wizards/contributionsimport.py:110
 msgid "Required field"
 msgstr "จำเป็น"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:133
+#: basxconnect/contributions/wizards/contributionsimport.py:131
 msgid "CSV import problem: "
 msgstr "เกิดปัญหาการนำเข้าCVS "
 
-#: basxconnect/contributions/wizards/contributionsimport.py:138
+#: basxconnect/contributions/wizards/contributionsimport.py:136
 msgid "Assignment"
 msgstr "การมอบหมาย"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:145
+#: basxconnect/contributions/wizards/contributionsimport.py:143
 msgid "Account"
 msgstr "บัญชี"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:148
+#: basxconnect/contributions/wizards/contributionsimport.py:146
 msgid "Cost Center"
 msgstr "ศูนย์ต้นทุน"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:151
+#: basxconnect/contributions/wizards/contributionsimport.py:149
 msgid "Person Number"
 msgstr "หมายเลขประจำตัว"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:154
+#: basxconnect/contributions/wizards/contributionsimport.py:152
 msgid "Donor Number"
 msgstr "หมายเลขผู้บริจาค"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:157
+#: basxconnect/contributions/wizards/contributionsimport.py:155
 msgid "Assignment state"
 msgstr "สถานะการมอบหมาย"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:178
+#: basxconnect/contributions/wizards/contributionsimport.py:176
 msgid "Overview of contributions to import"
 msgstr "ภาพรวมของเงินบริจาคที่จะนำเข้า"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:184
+#: basxconnect/contributions/wizards/contributionsimport.py:182
 msgid "contributions"
 msgstr "เงินบริจาค"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:188
+#: basxconnect/contributions/wizards/contributionsimport.py:186
 msgid "Sum"
 msgstr "ผลรวม"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:219
+#: basxconnect/contributions/wizards/contributionsimport.py:217
 msgid " contributions could not been assigned"
 msgstr " ไม่สามารถมอบหมายเงินบริจาคได้"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:222
+#: basxconnect/contributions/wizards/contributionsimport.py:220
 msgid ""
 "Please make sure that each entry has contributor number which matches with a "
 "person number and do the import again"
 msgstr "โปรดตรวจสอบให้แน่ใจว่าแต่ละรายการมีหมายเลขผู้สนับสนุนซึ่งตรงกับหมายเลขบุคคลและทำการนำเข้าอีกครั้ง"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:228
+#: basxconnect/contributions/wizards/contributionsimport.py:226
 msgid "Cancel import"
 msgstr "ยกเลิกการนำเข้า"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:234
+#: basxconnect/contributions/wizards/contributionsimport.py:232
 msgid "Assignment complete"
 msgstr "การมอบหมายเรียบร้อย"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:235
+#: basxconnect/contributions/wizards/contributionsimport.py:233
 msgid "Continue in order to complete the import"
 msgstr "ดำเนินการต่อเพื่อดำเนินการนำเข้าให้เสร็จสมบูรณ์"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:296
+#: basxconnect/contributions/wizards/contributionsimport.py:294
 msgid "Import contributions"
 msgstr "นำเข้าเงินบริจาค"
 
-#: basxconnect/contributions/wizards/contributionsimport.py:311
+#: basxconnect/contributions/wizards/contributionsimport.py:309
 #, python-format
 msgid "Successfully imported %d contributions"
 msgstr "นำเข้าเงินบริจาค%d สำเร็จแล้ว"
 
 #~ msgid "Contribution imports"
 #~ msgstr "นำเข้าเงินบริจาค"
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/migrations/0001_initial.py` & `basxconnect-0.4.7/basxconnect/contributions/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import django.db.models.deletion
 import djmoney.models.fields
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = [
         ("core", "0001_initial"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/migrations/0002_alter_contribution_currency.py` & `basxconnect-0.4.7/basxconnect/contributions/migrations/0002_alter_contribution_currency.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/contributions/migrations/0003_alter_contribution__import.py` & `basxconnect-0.4.7/basxconnect/contributions/migrations/0003_alter_contribution__import.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.5 on 2021-10-29 13:55
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("contributions", "0002_alter_contribution_currency"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="contribution",
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/migrations/0004_auto_20211030_0955.py` & `basxconnect-0.4.7/basxconnect/contributions/migrations/0004_auto_20211030_0955.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.5 on 2021-10-30 02:55
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("contributions", "0003_alter_contribution__import"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="contribution",
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/models.py` & `basxconnect-0.4.7/basxconnect/contributions/models.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/contributions/urls.py` & `basxconnect-0.4.7/basxconnect/contributions/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         model_urlname(models.ContributionImport, "add"),
     ),
     *default_model_paths(
         models.ContributionImport,
         browseview=views.BrowseView._with(
             columns=(
                 layout.datatable.DataTableColumn(
-                    _("Import date"), layout.ObjectFieldValue("date.date", "row"), None
+                    _("Import date"), layout.FC("row.date.date"), None
                 ),
                 layout.datatable.DataTableColumn(
                     _("Importfile"),
                     hg.BaseElement(
                         layout.ObjectFieldValue(
                             "importfile", "row", formatter=format_value
                         ),
```

### Comparing `basxconnect-0.4.61/basxconnect/contributions/wizards/contributionsimport.py` & `basxconnect-0.4.7/basxconnect/contributions/wizards/contributionsimport.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,17 @@
     encoding = chardet.detect(filedata).get("encoding") or "utf8"
     data = filedata.decode(encoding).splitlines()
     if has_header:
         data = data[1:]
 
     ret = []
     for row in csv.reader(data, delimiter=delimiter):
-        if len(row) == 0:
-            continue
         data = {k: row[mapping[k]] for k in mapping.keys() if mapping[k] is not None}
         data.setdefault("currency", global_preferences["contributions__currency"])
-        data["date"] = dateparser.parse(
-            data["date"], languages=[get_language().split("-")[0]]
-        )
+        data["date"] = dateparser.parse(data["date"], languages=[get_language()])
 
         externalnumber = data.pop("donornumber")
         person = Person.objects.filter(personnumber=externalnumber)
         if person.exists():
             data["person"] = person.get()
         contribution = models.Contribution(**data)
         contribution.full_clean(exclude=["_import", "person"])
```

### Comparing `basxconnect-0.4.61/basxconnect/core/apps.py` & `basxconnect-0.4.7/basxconnect/core/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 
 
 class CoreConfig(AppConfig):
     name = "basxconnect.core"
     default_auto_field = "django.db.models.BigAutoField"
-    verbose_name = _("BasxConnect Core")
 
     def ready(self):
         from django.db.models.signals import post_save
 
         from .models import Address, Phone, Vocabulary
 
         shared_task(base=RepeatedTask, run_every=timedelta(hours=6))(update_addresses)
```

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/addresses.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/addresses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import django.db.models
 import htmlgenerator as hg
 from basxbread import layout
 from basxbread.layout import ObjectFieldValue
 from basxbread.layout.components.datatable import DataTableColumn
 from basxbread.layout.components.icon import Icon
 from basxbread.layout.components.modal import modal_with_trigger
-from basxbread.utils import ModelHref, reverse_model
+from basxbread.utils import Link, ModelHref, reverse_model
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 from htmlgenerator import mark_safe
 
 from basxconnect.core import models
 from basxconnect.core.layouts.editperson.common.utils import tile_with_icon, tiling_col
 
 R = layout.grid.Row
 C = layout.grid.Col
 
 
-def numbers():
+def numbers(request):
     return tile_with_datatable(
         models.Phone,
         hg.F(lambda c: c["object"].core_phone_list.all()),
-        ["number", "type"],
+        ["type", "number"],
+        request,
     )
 
 
-def tile_with_datatable(model, queryset, columns):
+def tile_with_datatable(model, queryset, columns, request):
     addmodal = layout.modal.Modal.with_ajax_content(
         _("Add"),
         ModelHref(
             model,
             "add",
             query=hg.F(lambda c: {"person": c["object"].pk, "asajax": True}),
         ),
@@ -37,15 +38,15 @@
     )
 
     def editmodal():
         return hg.F(
             lambda c: modal_with_trigger(
                 layout.modal.Modal.with_ajax_content(
                     _("Edit"),
-                    ModelHref(hg.C("row"), "edit", query={"asajax": True}),
+                    ModelHref.from_object(hg.C("row"), "edit", query={"asajax": True}),
                     submitlabel=_("Save"),
                 ),
                 layout.button.Button,
                 notext=True,
                 small=True,
                 buttontype="ghost",
                 icon="edit",
@@ -58,65 +59,64 @@
         layout.datatable.DataTable.from_queryset(
             queryset,
             model=model,
             prevent_automatic_sortingnames=True,
             columns=columns,
             rowactions=[
                 editmodal(),
-                layout.button.Button(
-                    _("Delete"),
-                    icon="trash-can",
-                    notext=True,
-                    small=True,
-                    buttontype="ghost",
-                ).as_submit(
+                Link(
                     href=ModelHref(
                         model,
                         "delete",
                         kwargs={"pk": hg.C("row.pk")},
+                        query={"next": request.get_full_path()},
                     ),
+                    iconname="trash-can",
+                    label=_("Delete"),
                 ),
             ],
             primary_button=layout.button.Button(
                 _("Add"), buttontype="primary", **addmodal.openerattributes
             ),
             style="border-top: none;",
         ),
         addmodal,
     )
 
 
-def email():
+def email(request):
     return tile_with_datatable(
         models.Email,
         hg.F(lambda c: c["object"].core_email_list.all()),
         [
-            "email",
             DataTableColumn(
                 layout.ObjectFieldLabel("type", models.Email),
                 hg.SPAN(
                     hg.C("row.type"),
                     hg.If(
                         hg.F(
                             lambda c: c["row"] == c["row"].person.primary_email_address
                         ),
                         hg.BaseElement(" (", _("primary"), ")"),
                         "",
                     ),
                 ),
             ),
+            "email",
         ],
+        request,
     )
 
 
-def urls():
+def urls(request):
     return tile_with_datatable(
         models.Web,
         hg.F(lambda c: c["object"].core_web_list.all()),
-        ["url", "type"],
+        ["type", "url"],
+        request,
     )
 
 
 def edit_heading(model: type):
     return _("Edit %s") % model._meta.verbose_name
 
 
@@ -222,23 +222,21 @@
     return tile_with_icon(
         Icon("map"),
         hg.H4(_("Address(es)")),
         R(
             C(
                 hg.Iterator(
                     hg.F(
-                        lambda c: (
-                            getattr(c["object"], "core_postal_list")
-                            .order_by(
-                                django.db.models.F("valid_until").desc(nulls_first=True)
-                            )
-                            .all()
-                            if hasattr(c["object"], "core_postal_list")
-                            else []
+                        lambda c: getattr(c["object"], "core_postal_list")
+                        .order_by(
+                            django.db.models.F("valid_until").desc(nulls_first=True)
                         )
+                        .all()
+                        if hasattr(c["object"], "core_postal_list")
+                        else []
                     ),
                     "i",
                     display_postal(),
                 )
             )
         ),
         R(
```

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/base_data.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/base_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,27 +10,27 @@
     open_modal_popup_button,
     tile_with_icon,
 )
 
 R = layout.grid.Row
 
 
-def common_tiles():
+def common_tiles(request):
     return hg.BaseElement(
         R(
             tags(),
-            addresses.email(),
+            addresses.email(request),
         ),
         R(
             addresses.postals(),
-            addresses.numbers(),
+            addresses.numbers(request),
         ),
         R(
             other(),
-            addresses.urls(),
+            addresses.urls(request),
         ),
     )
 
 
 def other():
     return utils.tile_with_icon(
         Icon("add-comment"),
```

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/contributions_tab.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/contributions_tab.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/head.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/head.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 import htmlgenerator as hg
 from basxbread import layout
-from basxbread.utils import ModelHref
 from django.utils.translation import gettext_lazy as _
 
 R = layout.grid.Row
 C = layout.grid.Col
 
 
-def editperson_toolbar():
+def editperson_toolbar(request):
     deletebutton = layout.button.Button(
         _("Delete"),
         buttontype="ghost",
         icon="trash-can",
         notext=True,
-    ).as_submit(
-        ModelHref(hg.C("object"), "delete"),
-        confirm_text=hg.format(
-            _("Are you sure you want to delete {}?"), hg.EM(hg.C("object"))
+        **layout.aslink_attributes(
+            hg.F(lambda c: layout.objectaction(c["object"], "delete"))
         ),
     )
     restorebutton = layout.button.Button(
         _("Restore"),
         buttontype="ghost",
         icon="undo",
         notext=True,
-    ).as_submit(
-        ModelHref(hg.C("object"), "delete", query={"restore": True}),
-        confirm_text=hg.format(
-            _("Are you sure you want to restore {}?"), hg.EM(hg.C("object"))
+        **layout.aslink_attributes(
+            hg.F(
+                lambda c: layout.objectaction(
+                    c["object"], "delete", query={"restore": True}
+                )
+            )
         ),
     )
     copybutton = layout.button.Button(
         _("Copy"),
         buttontype="ghost",
         icon="copy",
         notext=True,
-    ).as_submit(
-        ModelHref(hg.C("object"), "copy"),
-        confirm_text=hg.format(
-            _("Are you sure you want to copy {}?"), hg.EM(hg.C("object"))
+        **layout.aslink_attributes(
+            hg.F(lambda c: layout.objectaction(c["object"], "copy"))
         ),
     )
 
     return hg.SPAN(
         hg.If(hg.C("object.deleted"), restorebutton, deletebutton),
         copybutton,
         layout.button.PrintPageButton(buttontype="ghost"),
         _class="no-print",
         style="margin-bottom: 1rem; margin-left: 1rem",
         width=3,
     )
 
 
-def editperson_head():
+def editperson_head(request):
     return hg.BaseElement(
         R(
             C(
                 hg.H3(
                     hg.SPAN(
                         hg.C("object"),
                         style=hg.If(
                             hg.C("object.deleted"), "text-decoration: line-through"
                         ),
                     ),
-                    editperson_toolbar(),
+                    editperson_toolbar(request),
                 ),
                 width=12,
             ),
             style="padding-top: 1rem",
         ),
     )
```

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/relationships_tab.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/relationships_tab.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/common/utils.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/common/utils.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/legalperson/base_data_tab.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/legalperson/base_data_tab.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     tile_col_edit_modal,
 )
 
 R = layout.grid.Row
 C = layout.grid.Col
 
 
-def base_data_tab():
+def base_data_tab(request):
     return layout.tabs.Tab(
         _("Base data"),
         hg.BaseElement(
             grid_inside_tab(
                 R(
                     tile_col_edit_modal(
                         _("Base Data"),
@@ -29,11 +29,11 @@
                         [
                             "name",
                             "name_addition",
                         ],
                     ),
                     person_metadata(models.LegalPerson),
                 ),
-                common_tiles(),
+                common_tiles(request),
             ),
         ),
     )
```

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/legalperson/mailing.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/legalperson/mailing.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,74 +11,55 @@
     person_metadata,
 )
 
 R = layout.grid.Row
 C = layout.grid.Col
 
 
-def base_data_tab():
+def base_data_tab(request):
+
     return layout.tabs.Tab(
         _("Personal data"),
         utils.grid_inside_tab(
             R(
                 personal_data(),
                 person_metadata(models.NaturalPerson),
             ),
-            base_data.common_tiles(),
+            base_data.common_tiles(request),
         ),
     )
 
 
 def personal_data():
-    displayed_fields = (
-        [
-            utils.display_field_label_and_value(field)
-            for field in [
-                "salutation",
-                "title",
-                "name",
-                "first_name",
-                "last_name",
-            ]
-        ]
-        + [
-            hg.If(
-                hg.C("object.middle_name"),
-                utils.display_field_label_and_value("middle_name"),
-            )
-        ]
-        + [
-            hg.If(
-                hg.C("object.maiden_name"),
-                utils.display_field_label_and_value("maiden_name"),
-            )
+    displayed_fields = [
+        utils.display_field_label_and_value(field)
+        for field in [
+            "salutation",
+            "title",
+            "name",
+            "first_name",
+            "last_name",
+            "gender",
+            "date_of_birth",
+            "place_of_birth",
+            "profession",
         ]
-        + [
-            utils.display_field_label_and_value(field)
-            for field in [
-                "gender",
-                "date_of_birth",
-                "place_of_birth",
-                "profession",
-            ]
-        ]
-        + [
-            hg.If(
-                hg.C("object.deceased"),
-                display_label_and_value(
-                    ObjectFieldLabel("deceased"),
-                    hg.If(hg.C("object.deceased"), _("Yes"), _("No")),
-                ),
-            ),
-            hg.If(
-                hg.C("object.deceased"),
-                utils.display_field_label_and_value("decease_date"),
+    ] + [
+        hg.If(
+            hg.C("object.deceased"),
+            display_label_and_value(
+                ObjectFieldLabel("deceased"),
+                hg.If(hg.C("object.deceased"), _("Yes"), _("No")),
             ),
-        ]
-    )
+        ),
+        hg.If(
+            hg.C("object.deceased"),
+            utils.display_field_label_and_value("decease_date"),
+        ),
+    ]
     return utils.tile_col_edit_modal_displayed_fields(
         _("Personal Data"),
         models.NaturalPerson,
         "ajax_edit_personal_data",
         Icon("user--profile"),
         displayed_fields,
     )
```

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/naturalperson/mailing.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/naturalperson/mailing.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/layouts/editperson/personassociation/mailing.py` & `basxconnect-0.4.7/basxconnect/core/layouts/editperson/personassociation/mailing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from basxconnect.core.layouts.editperson.common.utils import grid_inside_tab, tiling_col
 
 R = layout.grid.Row
 
 
 def mailings_tab(request):
+
     from django.apps import apps
 
     if apps.is_installed("basxconnect.mailer_integration"):
         from basxconnect.mailer_integration.layouts import mailer_integration_tile
 
         mailer_tile = mailer_integration_tile(request)
     else:
```

### Comparing `basxconnect-0.4.61/basxconnect/core/locale/de/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/core/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,142 +3,155 @@
 # This file is distributed under the same license as the basxconnect package.
 # basx GmbH <info@basx.ch>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-04 10:14+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: 2021-04-08 02:26+0000\n"
 "Last-Translator: Frederik Bugglin <bugglin@basx.ch>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/basxconnect/"
 "basxconnect/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.6-dev\n"
 
-#: basxconnect/core/apps.py:13
-msgid "BasxConnect Core"
-msgstr ""
-
-#: basxconnect/core/apps.py:29
+#: basxconnect/core/apps.py:28
 #: basxconnect/core/layouts/editperson/common/base_data.py:53
 #: basxconnect/core/models/persons.py:73
 msgid "Tags"
 msgstr "Tags"
 
-#: basxconnect/core/apps.py:30
+#: basxconnect/core/apps.py:29
 msgid "Titles"
 msgstr "Titel"
 
-#: basxconnect/core/apps.py:31
+#: basxconnect/core/apps.py:30
 msgid "Salutations"
 msgstr "Anreden"
 
-#: basxconnect/core/apps.py:32
+#: basxconnect/core/apps.py:31
 msgid "Forms Of Address"
 msgstr "Anredeform"
 
-#: basxconnect/core/apps.py:33
+#: basxconnect/core/apps.py:32
 msgid "Genders"
 msgstr "Geschlechter"
 
-#: basxconnect/core/apps.py:34
+#: basxconnect/core/apps.py:33
 msgid "Natural Person Types"
 msgstr "Natürliche Personen Typen"
 
-#: basxconnect/core/apps.py:35
+#: basxconnect/core/apps.py:34
 msgid "Legal Person Types"
 msgstr "Juristische Personen Typen"
 
-#: basxconnect/core/apps.py:36
+#: basxconnect/core/apps.py:35
 msgid "Association Person Types"
 msgstr "Personenverbindungen Typen"
 
-#: basxconnect/core/apps.py:37
+#: basxconnect/core/apps.py:36
 msgid "Address statuses"
 msgstr "Adressen Stati"
 
-#: basxconnect/core/apps.py:38
+#: basxconnect/core/apps.py:37
 msgid "Email Types"
 msgstr "Email Typen"
 
-#: basxconnect/core/apps.py:39
+#: basxconnect/core/apps.py:38
 msgid "URL Types"
 msgstr "URL Typen"
 
-#: basxconnect/core/apps.py:40
+#: basxconnect/core/apps.py:39
 msgid "Phone Types"
 msgstr "Telefon Typen"
 
-#: basxconnect/core/apps.py:41
+#: basxconnect/core/apps.py:40
 msgid "Address Types"
 msgstr "Adressen Typen"
 
-#: basxconnect/core/dynamic_preferences_registry.py:8
+#: basxconnect/core/dynamic_preferences_registry.py:14
+#: basxconnect/core/views/menu_views.py:55
+#: basxconnect/core/views/settings_views.py:30
 msgid "General"
 msgstr "Allgemein"
 
-#: basxconnect/core/dynamic_preferences_registry.py:9
-#: basxconnect/core/models/persons.py:244
-#: basxconnect/core/views/menu_views.py:28
-#: basxconnect/core/views/menu_views.py:34
+#: basxconnect/core/dynamic_preferences_registry.py:15
+#: basxconnect/core/layouts/settings_layout.py:78
+#: basxconnect/core/models/persons.py:242
+#: basxconnect/core/views/menu_views.py:42
+#: basxconnect/core/views/menu_views.py:46
+#: basxconnect/core/views/menu_views.py:65
 msgid "Persons"
 msgstr "Personen"
 
-#: basxconnect/core/dynamic_preferences_registry.py:18
+#: basxconnect/core/dynamic_preferences_registry.py:23
+msgid "Sender letterhead"
+msgstr "Absender Briefkopf"
+
+#: basxconnect/core/dynamic_preferences_registry.py:32
+msgid "Logo"
+msgstr "Logo"
+
+#: basxconnect/core/dynamic_preferences_registry.py:44
+msgid "Organization Name"
+msgstr "Name der Organisation"
+
+#: basxconnect/core/dynamic_preferences_registry.py:53
 msgid "Default type of natural persons"
 msgstr "Standart-Typ für Natürliche Personen"
 
-#: basxconnect/core/dynamic_preferences_registry.py:27
+#: basxconnect/core/dynamic_preferences_registry.py:62
 msgid "Default type of person associations"
 msgstr "Standart-Typ für Personenverbindungen"
 
-#: basxconnect/core/dynamic_preferences_registry.py:36
+#: basxconnect/core/dynamic_preferences_registry.py:71
 msgid "Default type of legal persons"
 msgstr "Standart-Typ für juristische Personen"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:30
-#: basxconnect/core/layouts/editperson/common/addresses.py:80
+#: basxconnect/core/layouts/editperson/common/addresses.py:31
+#: basxconnect/core/layouts/editperson/common/addresses.py:78
 #: basxconnect/core/layouts/editperson/common/addresses.py:267
 msgid "Add"
 msgstr "Hinzufügen"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:36
-#: basxconnect/core/layouts/editperson/common/addresses.py:45
+#: basxconnect/core/layouts/editperson/common/addresses.py:37
+#: basxconnect/core/layouts/editperson/common/addresses.py:46
 #: basxconnect/core/layouts/editperson/common/addresses.py:134
 #: basxconnect/core/layouts/editperson/common/addresses.py:306
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:114
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:125
 #: basxconnect/core/layouts/editperson/common/utils.py:116
 #: basxconnect/core/views/tag_views.py:109
 msgid "Save"
 msgstr "Speichern"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:43
-#: basxconnect/core/layouts/editperson/common/addresses.py:52
+#: basxconnect/core/layouts/editperson/common/addresses.py:44
+#: basxconnect/core/layouts/editperson/common/addresses.py:53
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:77
 #: basxconnect/core/layouts/editperson/common/utils.py:98
 #: basxconnect/core/layouts/settings_layout.py:39
 msgid "Edit"
 msgstr "Bearbeiten"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:66
+#: basxconnect/core/layouts/editperson/common/addresses.py:74
 #: basxconnect/core/layouts/editperson/common/addresses.py:204
-#: basxconnect/core/layouts/editperson/common/head.py:12
+#: basxconnect/core/layouts/editperson/common/head.py:11
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:87
 #: basxconnect/core/layouts/settings_layout.py:53
-#: basxconnect/core/views/person/person_browse_views.py:186
+#: basxconnect/core/layouts/settings_layout.py:123
+#: basxconnect/core/views/person/person_browse_views.py:187
 msgid "Delete"
 msgstr "Löschen"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:102
+#: basxconnect/core/layouts/editperson/common/addresses.py:99
 #: basxconnect/core/layouts/editperson/common/addresses.py:148
 msgid "primary"
 msgstr "primär"
 
 #: basxconnect/core/layouts/editperson/common/addresses.py:120
 #, python-format
 msgid "Edit %s"
@@ -178,75 +191,60 @@
 
 #: basxconnect/core/layouts/editperson/common/contributions_tab.py:17
 msgid "Contributions"
 msgstr "Zuwendungen"
 
 #: basxconnect/core/layouts/editperson/common/contributions_tab.py:37
 #: basxconnect/core/layouts/settings_layout.py:33
-#: basxconnect/core/layouts/settings_layout.py:90
-#: basxconnect/core/views/term.py:27 basxconnect/core/wizards/add_person.py:386
+#: basxconnect/core/layouts/settings_layout.py:115
+#: basxconnect/core/views/term.py:26 basxconnect/core/wizards/add_person.py:379
 #, python-format
 msgid "Add %s"
 msgstr "%s hinzufügen"
 
-#: basxconnect/core/layouts/editperson/common/documenttemplates_tab.py:30
-msgid "Series letters"
-msgstr "Serienbriefe"
-
-#: basxconnect/core/layouts/editperson/common/head.py:19
-msgid "Are you sure you want to delete {}?"
-msgstr "Sind Sie sicher, dass Sie {} löschen möchten?"
+#: basxconnect/core/layouts/editperson/common/documenttemplates_tab.py:19
+msgid "Documents"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/head.py:23
-#: basxconnect/core/views/person/person_browse_views.py:192
+#: basxconnect/core/layouts/editperson/common/head.py:20
+#: basxconnect/core/views/person/person_browse_views.py:193
 msgid "Restore"
 msgstr "Wiederherstellen"
 
-#: basxconnect/core/layouts/editperson/common/head.py:30
-msgid "Are you sure you want to restore {}?"
-msgstr "Sind Sie sicher, dass Sie {} wiederherstellen möchten?"
-
-#: basxconnect/core/layouts/editperson/common/head.py:34
+#: basxconnect/core/layouts/editperson/common/head.py:33
 msgid "Copy"
 msgstr "Kopieren"
 
-#: basxconnect/core/layouts/editperson/common/head.py:41
-msgid "Are you sure you want to copy {}?"
-msgstr "Sind Sie sicher, dass Sie {} kopieren möchten?"
-
-#: basxconnect/core/layouts/editperson/common/history_tab.py:65
-#: basxconnect/core/layouts/editperson/common/history_tab.py:77
-msgid "<Value has been deleted>"
-msgstr "<Wert wurde gelöscht>"
-
-#: basxconnect/core/layouts/editperson/common/history_tab.py:83
+#: basxconnect/core/layouts/editperson/common/history_tab.py:68
 msgid "History"
-msgstr "Historie"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:91
+#: basxconnect/core/layouts/editperson/common/history_tab.py:78
 msgid "Date"
-msgstr "Datum"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:97
+#: basxconnect/core/layouts/editperson/common/history_tab.py:84
 msgid "Time"
-msgstr "Zeit"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:103
+#: basxconnect/core/layouts/editperson/common/history_tab.py:90
 msgid "User"
-msgstr "Benutzer"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:107
-#: basxconnect/core/layouts/editperson/common/history_tab.py:139
+#: basxconnect/core/layouts/editperson/common/history_tab.py:94
+#: basxconnect/core/layouts/editperson/common/history_tab.py:126
+#, fuzzy
+#| msgid "Changed"
 msgid "Changes"
-msgstr "Geändert"
+msgstr "Zuletzt geändert"
 
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:22
 #: basxconnect/core/layouts/settings_layout.py:16
 #: basxconnect/core/models/relationships.py:55
-#: basxconnect/core/views/menu_views.py:59
+#: basxconnect/core/views/menu_views.py:75
 msgid "Relationships"
 msgstr "Verknüpfungen"
 
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:28
 msgid "Relationships to person"
 msgstr "Beziehungen zu Personen"
 
@@ -278,25 +276,25 @@
 msgstr "Erstellt"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:44
 msgid "Meta data"
 msgstr "Metadaten"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:52
-#: basxconnect/core/views/person/person_browse_views.py:114
-#: basxconnect/core/views/person/person_browse_views.py:244
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_browse_views.py:115
+#: basxconnect/core/views/person/person_browse_views.py:245
+#: basxconnect/core/views/person/person_details_views.py:161
 msgid "Inactive"
 msgstr "Inaktiv"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:52
 #: basxconnect/core/models/persons.py:58
-#: basxconnect/core/views/person/person_browse_views.py:113
-#: basxconnect/core/views/person/person_browse_views.py:244
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_browse_views.py:114
+#: basxconnect/core/views/person/person_browse_views.py:245
+#: basxconnect/core/views/person/person_details_views.py:161
 msgid "Active"
 msgstr "Aktiv"
 
 #: basxconnect/core/layouts/editperson/legalperson/base_data_tab.py:20
 #: basxconnect/core/layouts/editperson/personassociation/base_data_tab.py:18
 msgid "Base data"
 msgstr "Stammdaten"
@@ -304,143 +302,144 @@
 #: basxconnect/core/layouts/editperson/legalperson/base_data_tab.py:25
 #: basxconnect/core/layouts/editperson/personassociation/base_data_tab.py:22
 msgid "Base Data"
 msgstr "Stammdaten"
 
 #: basxconnect/core/layouts/editperson/legalperson/mailing.py:27
 #: basxconnect/core/layouts/editperson/naturalperson/mailing.py:27
-#: basxconnect/core/layouts/editperson/personassociation/mailing.py:20
+#: basxconnect/core/layouts/editperson/personassociation/mailing.py:21
 msgid "Mailings"
 msgstr "Versand"
 
 #: basxconnect/core/layouts/editperson/legalperson/mailing.py:31
 #: basxconnect/core/layouts/editperson/naturalperson/mailing.py:31
 #: basxconnect/core/views/person/person_modals_views.py:28
+#: basxconnect/core/views/settings_views.py:29
 msgid "Settings"
 msgstr "Einstellungen"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:20
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:21
 msgid "Personal data"
 msgstr "Persönliche Daten"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:69
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:51
 msgid "Yes"
 msgstr "Ja"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:69
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:51
 msgid "No"
 msgstr "Nein"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:79
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:60
 msgid "Personal Data"
 msgstr "Persönliche Daten"
 
 #: basxconnect/core/migrations/0015_rename_category_to_tag.py:13
 msgid "Tag"
 msgstr "Tag"
 
 #: basxconnect/core/migrations/0015_rename_category_to_tag.py:21
 msgid "Category"
 msgstr "Kategorie"
 
-#: basxconnect/core/models/addresses.py:20
-#: basxconnect/core/models/persons.py:243
+#: basxconnect/core/models/addresses.py:18
+#: basxconnect/core/models/persons.py:241
 msgid "Person"
 msgstr "Person"
 
-#: basxconnect/core/models/addresses.py:32
-#: basxconnect/core/models/addresses.py:57
-#: basxconnect/core/views/person/person_browse_views.py:157
-#: basxconnect/core/wizards/add_person.py:69
+#: basxconnect/core/models/addresses.py:30
+#: basxconnect/core/models/addresses.py:54
+#: basxconnect/core/views/person/person_browse_views.py:158
+#: basxconnect/core/wizards/add_person.py:67
 msgid "Email"
 msgstr "E-Mail"
 
-#: basxconnect/core/models/addresses.py:40
-#: basxconnect/core/models/addresses.py:76
-#: basxconnect/core/models/addresses.py:96
-#: basxconnect/core/models/addresses.py:118
-#: basxconnect/core/models/addresses.py:144
-#: basxconnect/core/models/persons.py:359
-#: basxconnect/core/models/persons.py:383
+#: basxconnect/core/models/addresses.py:39
+#: basxconnect/core/models/addresses.py:74
+#: basxconnect/core/models/addresses.py:93
+#: basxconnect/core/models/addresses.py:114
+#: basxconnect/core/models/addresses.py:139
+#: basxconnect/core/models/persons.py:350
+#: basxconnect/core/models/persons.py:374
 #: basxconnect/core/models/relationships.py:36
-#: basxconnect/core/wizards/add_person.py:280
+#: basxconnect/core/wizards/add_person.py:273
 msgid "Type"
 msgstr "Typ"
 
-#: basxconnect/core/models/addresses.py:63
+#: basxconnect/core/models/addresses.py:60
 msgid "Email address"
 msgstr "E-Mail-Adresse"
 
-#: basxconnect/core/models/addresses.py:64
+#: basxconnect/core/models/addresses.py:61
 msgid "Email addresses"
 msgstr "E-Mail-Adressen"
 
-#: basxconnect/core/models/addresses.py:68
+#: basxconnect/core/models/addresses.py:65
 msgid "Url"
 msgstr "URL"
 
-#: basxconnect/core/models/addresses.py:84
+#: basxconnect/core/models/addresses.py:80
 msgid "Web address"
 msgstr "Webadresse"
 
-#: basxconnect/core/models/addresses.py:85
+#: basxconnect/core/models/addresses.py:81
 msgid "Web addresses"
 msgstr "Webadressen"
 
-#: basxconnect/core/models/addresses.py:89
-#: basxconnect/core/models/addresses.py:111
+#: basxconnect/core/models/addresses.py:85
+#: basxconnect/core/models/addresses.py:106
 msgid "Number"
 msgstr "Nummer"
 
-#: basxconnect/core/models/addresses.py:106
+#: basxconnect/core/models/addresses.py:101
 msgid "Phone number"
 msgstr "Telefonnummer"
 
-#: basxconnect/core/models/addresses.py:107
+#: basxconnect/core/models/addresses.py:102
 msgid "Phone numbers"
 msgstr "Telefonnummern"
 
-#: basxconnect/core/models/addresses.py:128
+#: basxconnect/core/models/addresses.py:122
 msgid "Fax number"
 msgstr "Faxnummer"
 
-#: basxconnect/core/models/addresses.py:129
+#: basxconnect/core/models/addresses.py:123
 msgid "Fax numbers"
 msgstr "Faxnummern"
 
-#: basxconnect/core/models/addresses.py:133
+#: basxconnect/core/models/addresses.py:127
 msgid "Country"
 msgstr "Land"
 
-#: basxconnect/core/models/addresses.py:134
-#: basxconnect/core/wizards/add_person.py:48
+#: basxconnect/core/models/addresses.py:128
+#: basxconnect/core/wizards/add_person.py:46
 msgid "Address"
 msgstr "Adresse"
 
-#: basxconnect/core/models/addresses.py:135
+#: basxconnect/core/models/addresses.py:129
 msgid "Post Code"
 msgstr "PLZ"
 
-#: basxconnect/core/models/addresses.py:136
+#: basxconnect/core/models/addresses.py:130
 msgid "City"
 msgstr "Ort"
 
-#: basxconnect/core/models/addresses.py:148
+#: basxconnect/core/models/addresses.py:140
 msgid "Valid from"
 msgstr "Gültig von"
 
-#: basxconnect/core/models/addresses.py:149
+#: basxconnect/core/models/addresses.py:141
 msgid "Valid until"
 msgstr "Gültig bis"
 
-#: basxconnect/core/models/addresses.py:164
+#: basxconnect/core/models/addresses.py:153
 msgid "Postal address"
 msgstr "Anschrift"
 
-#: basxconnect/core/models/addresses.py:165
+#: basxconnect/core/models/addresses.py:154
 msgid "Postal addresses"
 msgstr "Anschriften"
 
 #: basxconnect/core/models/persons.py:43
 msgid "Deleted"
 msgstr "Gelöscht"
 
@@ -477,16 +476,16 @@
 msgstr "Primäre Telefonnummer"
 
 #: basxconnect/core/models/persons.py:115
 msgid "Remarks"
 msgstr "Bemerkungen"
 
 #: basxconnect/core/models/persons.py:132
-#: basxconnect/core/models/persons.py:316
-#: basxconnect/core/views/person/person_browse_views.py:371
+#: basxconnect/core/models/persons.py:307
+#: basxconnect/core/views/person/person_browse_views.py:372
 msgid "Person Type"
 msgstr "Personentyp"
 
 #: basxconnect/core/models/persons.py:142
 msgid "Main Type"
 msgstr "Personen-Typ"
 
@@ -494,102 +493,98 @@
 msgid "active"
 msgstr "aktiv"
 
 #: basxconnect/core/models/persons.py:149
 msgid "inactive"
 msgstr "Inaktiv"
 
-#: basxconnect/core/models/persons.py:248
+#: basxconnect/core/models/persons.py:246
 msgid "First Name"
 msgstr "Vorname"
 
-#: basxconnect/core/models/persons.py:249
+#: basxconnect/core/models/persons.py:247
 msgid "Middle Name"
 msgstr "Mittelname(n)"
 
-#: basxconnect/core/models/persons.py:250
+#: basxconnect/core/models/persons.py:248
 msgid "Last Name"
 msgstr "Nachname"
 
-#: basxconnect/core/models/persons.py:251
-msgid "Maiden Name"
-msgstr "Mädchenname"
-
-#: basxconnect/core/models/persons.py:254
+#: basxconnect/core/models/persons.py:250
 msgid "Autogenerate Display Name"
 msgstr "Anzeigenamen automatisch erstellen"
 
-#: basxconnect/core/models/persons.py:263
+#: basxconnect/core/models/persons.py:260
 msgid "Title"
 msgstr "Titel"
 
-#: basxconnect/core/models/persons.py:274
+#: basxconnect/core/models/persons.py:269
 msgid "Salutation"
 msgstr "Anrede"
 
-#: basxconnect/core/models/persons.py:285
+#: basxconnect/core/models/persons.py:279
 msgid "Form of address"
 msgstr "Anredeform"
 
-#: basxconnect/core/models/persons.py:290
+#: basxconnect/core/models/persons.py:282
 msgid "Profession"
 msgstr "Beruf"
 
-#: basxconnect/core/models/persons.py:294
+#: basxconnect/core/models/persons.py:286
 msgid "Date of Birth"
 msgstr "Geburtsdatum"
 
-#: basxconnect/core/models/persons.py:295
+#: basxconnect/core/models/persons.py:287
 msgid "Place of Birth"
 msgstr "Geburtsort"
 
-#: basxconnect/core/models/persons.py:296
+#: basxconnect/core/models/persons.py:288
 msgid "Deceased"
 msgstr "Verstorben"
 
-#: basxconnect/core/models/persons.py:297
+#: basxconnect/core/models/persons.py:289
 msgid "Deceased Date"
 msgstr "Todesdatum"
 
-#: basxconnect/core/models/persons.py:305
+#: basxconnect/core/models/persons.py:298
 msgid "Gender"
 msgstr "Geschlecht"
 
-#: basxconnect/core/models/persons.py:329
+#: basxconnect/core/models/persons.py:320
 msgid "Age"
 msgstr "Alter"
 
-#: basxconnect/core/models/persons.py:346
-#: basxconnect/core/views/person/person_browse_views.py:210
+#: basxconnect/core/models/persons.py:337
+#: basxconnect/core/views/person/person_browse_views.py:211
 msgid "Natural Person"
 msgstr "Natürliche Person"
 
-#: basxconnect/core/models/persons.py:347
+#: basxconnect/core/models/persons.py:338
 msgid "Natural Persons"
 msgstr "Natürliche Personen"
 
-#: basxconnect/core/models/persons.py:351
+#: basxconnect/core/models/persons.py:342
 msgid "Addition name"
 msgstr "Zusatz"
 
-#: basxconnect/core/models/persons.py:371
-#: basxconnect/core/views/person/person_browse_views.py:211
+#: basxconnect/core/models/persons.py:362
+#: basxconnect/core/views/person/person_browse_views.py:212
 msgid "Legal Person"
 msgstr "Juristische Person"
 
-#: basxconnect/core/models/persons.py:372
+#: basxconnect/core/models/persons.py:363
 msgid "Legal Persons"
 msgstr "Juristische Personen"
 
-#: basxconnect/core/models/persons.py:395
-#: basxconnect/core/views/person/person_browse_views.py:213
+#: basxconnect/core/models/persons.py:386
+#: basxconnect/core/views/person/person_browse_views.py:214
 msgid "Person Association"
 msgstr "Personenverbindung"
 
-#: basxconnect/core/models/persons.py:396
+#: basxconnect/core/models/persons.py:387
 msgid "Person Associations"
 msgstr "Personenverbindungen"
 
 #: basxconnect/core/models/relationships.py:9
 msgid "Name for relationship type"
 msgstr "Name des Beziehungstypes"
 
@@ -621,127 +616,115 @@
 msgid "Ends on"
 msgstr "Endet am"
 
 #: basxconnect/core/models/relationships.py:54
 msgid "Relationship"
 msgstr "Beziehung"
 
-#: basxconnect/core/models/utils.py:19 basxconnect/core/models/utils.py:75
-msgid "Terms"
-msgstr "Begriffe"
-
-#: basxconnect/core/models/utils.py:26
-#: basxconnect/core/views/person/person_browse_views.py:129
+#: basxconnect/core/models/utils.py:13
+#: basxconnect/core/views/person/person_browse_views.py:130
 msgid "Name"
 msgstr "Name"
 
-#: basxconnect/core/models/utils.py:28 basxconnect/core/models/utils.py:56
+#: basxconnect/core/models/utils.py:15 basxconnect/core/models/utils.py:33
 msgid "Slug"
 msgstr "Slug"
 
-#: basxconnect/core/models/utils.py:30
+#: basxconnect/core/models/utils.py:17
 msgid "slug is human-readable, to make referencing easier"
 msgstr "Slug ist eine interne Id welche einfach lesbar ist"
 
-#: basxconnect/core/models/utils.py:40 basxconnect/core/models/utils.py:54
+#: basxconnect/core/models/utils.py:25 basxconnect/core/models/utils.py:31
 msgid "Vocabulary"
 msgstr "Vokabular"
 
-#: basxconnect/core/models/utils.py:41
+#: basxconnect/core/models/utils.py:26
 msgid "Vocabularies"
 msgstr "Vokabulare"
 
-#: basxconnect/core/models/utils.py:55 basxconnect/core/models/utils.py:74
+#: basxconnect/core/models/utils.py:32 basxconnect/core/models/utils.py:44
 msgid "Term"
 msgstr "Begriff"
 
-#: basxconnect/core/models/utils.py:58
-msgid "Disabled"
-msgstr "Deaktiviert"
-
-#: basxconnect/core/models/utils.py:60
-msgid "Do not allow this term to be selected"
-msgstr "Verbiete die Nutzung dieses Begriffes"
-
-#: basxconnect/core/views/menu_views.py:46
-msgid "Taxonomy"
-msgstr "Taxonomie"
+#: basxconnect/core/models/utils.py:45
+msgid "Terms"
+msgstr "Begriffe"
 
-#: basxconnect/core/views/person/person_browse_views.py:174
+#: basxconnect/core/views/person/person_browse_views.py:175
 msgid "Add tag"
 msgstr "Tag hinzufügen"
 
-#: basxconnect/core/views/person/person_browse_views.py:180
+#: basxconnect/core/views/person/person_browse_views.py:181
 msgid "Remove tag"
 msgstr "Tag entfernen"
 
-#: basxconnect/core/views/person/person_browse_views.py:198
+#: basxconnect/core/views/person/person_browse_views.py:199
 msgid "Excel"
 msgstr "Excel"
 
-#: basxconnect/core/views/person/person_browse_views.py:248
+#: basxconnect/core/views/person/person_browse_views.py:249
 msgid "Trash"
 msgstr "Papierkorb"
 
-#: basxconnect/core/views/person/person_browse_views.py:445
-#: basxconnect/core/views/person/person_details_views.py:214
+#: basxconnect/core/views/person/person_browse_views.py:446
+#: basxconnect/core/views/person/person_details_views.py:233
 msgid "Cancel"
 msgstr "Abbrechen"
 
-#: basxconnect/core/views/person/person_browse_views.py:451
+#: basxconnect/core/views/person/person_browse_views.py:452
 msgid "Reset"
 msgstr "Zurücksetzen"
 
-#: basxconnect/core/views/person/person_browse_views.py:458
+#: basxconnect/core/views/person/person_browse_views.py:459
 msgctxt "apply filter"
 msgid "Filter"
 msgstr "Anwenden"
 
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_details_views.py:161
 #, python-format
 msgid "%s is %s"
 msgstr "%s ist %s"
 
-#: basxconnect/core/views/person/person_details_views.py:159
+#: basxconnect/core/views/person/person_details_views.py:178
 #, python-format
 msgid "Delete linked %s subscription as well"
 msgstr "Verknüpfte Email-Abonnemente %s auch löschen"
 
-#: basxconnect/core/views/person/person_details_views.py:205
+#: basxconnect/core/views/person/person_details_views.py:224
 #, python-format
 msgid "Delete email %s"
 msgstr "Email %s löschen"
 
-#: basxconnect/core/views/person/person_details_views.py:220
+#: basxconnect/core/views/person/person_details_views.py:239
 msgid "Confirm"
 msgstr "Bestätigen"
 
 #: basxconnect/core/views/person/person_modals_views.py:32
 msgid "Edit mailing settings"
 msgstr "Versand-Einstellungen bearbeiten"
 
-#: basxconnect/core/views/person/person_modals_views.py:153
+#: basxconnect/core/views/person/person_modals_views.py:149
 msgid "Use as primary postal address"
 msgstr "Als primäre Postadresse verwenden"
 
-#: basxconnect/core/views/person/person_modals_views.py:216
+#: basxconnect/core/views/person/person_modals_views.py:213
 msgid "Use as primary email address"
 msgstr "Als primäre Email Adresse verwenden"
 
-#: basxconnect/core/views/person/person_modals_views.py:224
+#: basxconnect/core/views/person/person_modals_views.py:221
 #, python-format
 msgid "Propagate change of email address to %s"
 msgstr "Email Adresse auch in %s ändern"
 
-#: basxconnect/core/views/person/person_modals_views.py:253
+#: basxconnect/core/views/person/person_modals_views.py:250
 msgid "Edit Email"
 msgstr "E-Mail bearbeiten"
 
 #: basxconnect/core/views/person/search_person_view.py:21
-#: basxconnect/core/wizards/add_person.py:151
+#: basxconnect/core/wizards/add_person.py:147
 msgid "Search person"
 msgstr "Suche"
 
 #: basxconnect/core/views/person/search_person_view.py:62
 msgid "No results"
 msgstr "Keine Ergebnisse gefunden"
 
@@ -754,14 +737,18 @@
 msgid "Edit Relationship"
 msgstr "Beziehung editieren"
 
 #: basxconnect/core/views/relationship_views.py:61
 msgid "Add Relationship"
 msgstr "Beziehung hinzufügen"
 
+#: basxconnect/core/views/settings_views.py:31
+msgid "Information about our organization"
+msgstr "Angaben zu unserer Organisation"
+
 #: basxconnect/core/views/tag_views.py:67
 #, python-format
 msgid "Add tag to %(count)d person"
 msgid_plural "Add tag to %(count)d persons"
 msgstr[0] "Tag zu %(count)d Person hinzufügen"
 msgstr[1] "Tag zu %(count)d Personen hinzufügen"
 
@@ -781,101 +768,89 @@
 msgid "Submit"
 msgstr "Absenden"
 
 #: basxconnect/core/views/vocabulary.py:14
 msgid "Terms of vocabulary"
 msgstr "Begriffe von Vokabular"
 
-#: basxconnect/core/wizards/add_person.py:105
+#: basxconnect/core/wizards/add_person.py:101
 msgid "Back"
 msgstr "Zurück"
 
-#: basxconnect/core/wizards/add_person.py:116
+#: basxconnect/core/wizards/add_person.py:112
 msgid "Complete"
 msgstr "Fertigstellen"
 
-#: basxconnect/core/wizards/add_person.py:119
+#: basxconnect/core/wizards/add_person.py:115
 msgid "Continue"
 msgstr "Weiter"
 
-#: basxconnect/core/wizards/add_person.py:131
+#: basxconnect/core/wizards/add_person.py:127
 msgid "Check for existing people before continuing"
 msgstr "Auf existierende Einträge prüfen bevor es weitergehen kann"
 
-#: basxconnect/core/wizards/add_person.py:139
+#: basxconnect/core/wizards/add_person.py:135
 msgid "Start typing to search for a person..."
 msgstr "Tippen um nach Personen zu suchen..."
 
-#: basxconnect/core/wizards/add_person.py:155
+#: basxconnect/core/wizards/add_person.py:151
 msgid ""
 "Before a new person can be added it must be confirmed that the person does "
 "not exists yet."
 msgstr ""
 "Bevor eine neue Person hinzugefügt wird muss überprüft werden, ob die Person "
 "nicht bereits existiert"
 
-#: basxconnect/core/wizards/add_person.py:171
+#: basxconnect/core/wizards/add_person.py:167
 msgid "Type of person"
 msgstr "Personentyp"
 
-#: basxconnect/core/wizards/add_person.py:177
+#: basxconnect/core/wizards/add_person.py:173
 msgid "Choose person main type"
 msgstr "Hauptyp auswählen"
 
-#: basxconnect/core/wizards/add_person.py:180
+#: basxconnect/core/wizards/add_person.py:176
 msgid "Please choose what type of person you want to add:"
 msgstr "Bitte den Personentyp wählen"
 
-#: basxconnect/core/wizards/add_person.py:195
+#: basxconnect/core/wizards/add_person.py:191
 msgid "Subtype of person"
 msgstr "Art der Person"
 
-#: basxconnect/core/wizards/add_person.py:211
+#: basxconnect/core/wizards/add_person.py:207
 msgid "Choose person type"
 msgstr "Bitte den Personentyp wählen"
 
-#: basxconnect/core/wizards/add_person.py:219
+#: basxconnect/core/wizards/add_person.py:215
 msgid "Add person"
 msgstr "Person hinzufügen"
 
-#: basxconnect/core/wizards/add_person.py:227
+#: basxconnect/core/wizards/add_person.py:223
 msgid "Finish"
 msgstr "Beenden"
 
-#: basxconnect/core/wizards/add_person.py:279
+#: basxconnect/core/wizards/add_person.py:272
 msgid "Search"
 msgstr "Suche"
 
-#: basxconnect/core/wizards/add_person.py:281
+#: basxconnect/core/wizards/add_person.py:274
 msgid "Subtype"
 msgstr "Art"
 
-#: basxconnect/core/wizards/add_person.py:282
+#: basxconnect/core/wizards/add_person.py:275
 msgid "Information"
 msgstr "Informationen"
 
-#: basxconnect/core/wizards/add_person.py:283
+#: basxconnect/core/wizards/add_person.py:276
 msgid "Confirmation"
 msgstr "Bestätigung"
 
-#: basxconnect/core/wizards/add_person.py:307
+#: basxconnect/core/wizards/add_person.py:300
 msgid "Add new person"
 msgstr "Neue Person hinzufügen"
 
-#: basxconnect/core/wizards/add_person.py:378
+#: basxconnect/core/wizards/add_person.py:371
 msgid "Review and confirm the entered information"
 msgstr "Überprüfen und bestätigen Sie die eingetragenen Informationen"
 
-#~ msgid "Sender letterhead"
-#~ msgstr "Absender Briefkopf"
-
-#~ msgid "Logo"
-#~ msgstr "Logo"
-
-#~ msgid "Organization Name"
-#~ msgstr "Name der Organisation"
-
-#~ msgid "Information about our organization"
-#~ msgstr "Angaben zu unserer Organisation"
-
 #~ msgid "Languages"
 #~ msgstr "Sprachen"
```

### Comparing `basxconnect-0.4.61/basxconnect/core/locale/fr/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/core/locale/fr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,142 +3,155 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-04 10:14+0700\n"
-"PO-Revision-Date: 2022-08-04 05:15+0000\n"
-"Last-Translator: Maxime Leroy <lisacintosh@gmail.com>\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
+"PO-Revision-Date: 2022-02-12 10:55+0000\n"
+"Last-Translator: Nathan <bonnemainsnathan@gmail.com>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/basxconnect/"
 "basxconnect/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.14-dev\n"
+"X-Generator: Weblate 4.11-dev\n"
 
-#: basxconnect/core/apps.py:13
-msgid "BasxConnect Core"
-msgstr ""
-
-#: basxconnect/core/apps.py:29
+#: basxconnect/core/apps.py:28
 #: basxconnect/core/layouts/editperson/common/base_data.py:53
 #: basxconnect/core/models/persons.py:73
 msgid "Tags"
 msgstr "Étiquettes"
 
-#: basxconnect/core/apps.py:30
+#: basxconnect/core/apps.py:29
 msgid "Titles"
 msgstr "Titres"
 
-#: basxconnect/core/apps.py:31
+#: basxconnect/core/apps.py:30
 msgid "Salutations"
 msgstr "Salutations"
 
-#: basxconnect/core/apps.py:32
+#: basxconnect/core/apps.py:31
 msgid "Forms Of Address"
 msgstr "Formulaires d'adresse"
 
-#: basxconnect/core/apps.py:33
+#: basxconnect/core/apps.py:32
 msgid "Genders"
 msgstr "Genres"
 
-#: basxconnect/core/apps.py:34
+#: basxconnect/core/apps.py:33
 msgid "Natural Person Types"
 msgstr "Type des personnes physiques"
 
-#: basxconnect/core/apps.py:35
+#: basxconnect/core/apps.py:34
 msgid "Legal Person Types"
 msgstr "Type des personnes morales"
 
-#: basxconnect/core/apps.py:36
+#: basxconnect/core/apps.py:35
 msgid "Association Person Types"
 msgstr "Types des associations de personnes"
 
-#: basxconnect/core/apps.py:37
+#: basxconnect/core/apps.py:36
 msgid "Address statuses"
 msgstr "Status de l'adresse"
 
-#: basxconnect/core/apps.py:38
+#: basxconnect/core/apps.py:37
 msgid "Email Types"
 msgstr "Types d'e-mail"
 
-#: basxconnect/core/apps.py:39
+#: basxconnect/core/apps.py:38
 msgid "URL Types"
 msgstr "Types d'URL"
 
-#: basxconnect/core/apps.py:40
+#: basxconnect/core/apps.py:39
 msgid "Phone Types"
 msgstr "Types de téléphone"
 
-#: basxconnect/core/apps.py:41
+#: basxconnect/core/apps.py:40
 msgid "Address Types"
 msgstr "Types d'adresses"
 
-#: basxconnect/core/dynamic_preferences_registry.py:8
+#: basxconnect/core/dynamic_preferences_registry.py:14
+#: basxconnect/core/views/menu_views.py:55
+#: basxconnect/core/views/settings_views.py:30
 msgid "General"
 msgstr "Général"
 
-#: basxconnect/core/dynamic_preferences_registry.py:9
-#: basxconnect/core/models/persons.py:244
-#: basxconnect/core/views/menu_views.py:28
-#: basxconnect/core/views/menu_views.py:34
+#: basxconnect/core/dynamic_preferences_registry.py:15
+#: basxconnect/core/layouts/settings_layout.py:78
+#: basxconnect/core/models/persons.py:242
+#: basxconnect/core/views/menu_views.py:42
+#: basxconnect/core/views/menu_views.py:46
+#: basxconnect/core/views/menu_views.py:65
 msgid "Persons"
 msgstr "Personnes"
 
-#: basxconnect/core/dynamic_preferences_registry.py:18
+#: basxconnect/core/dynamic_preferences_registry.py:23
+msgid "Sender letterhead"
+msgstr "En-tête de l'expéditeur"
+
+#: basxconnect/core/dynamic_preferences_registry.py:32
+msgid "Logo"
+msgstr "Logo"
+
+#: basxconnect/core/dynamic_preferences_registry.py:44
+msgid "Organization Name"
+msgstr "Nom de l'organisation"
+
+#: basxconnect/core/dynamic_preferences_registry.py:53
 msgid "Default type of natural persons"
 msgstr "Type par défaut des personnes physiques"
 
-#: basxconnect/core/dynamic_preferences_registry.py:27
+#: basxconnect/core/dynamic_preferences_registry.py:62
 msgid "Default type of person associations"
 msgstr "Type par défaut des associations de personnes"
 
-#: basxconnect/core/dynamic_preferences_registry.py:36
+#: basxconnect/core/dynamic_preferences_registry.py:71
 msgid "Default type of legal persons"
 msgstr "Type par défaut des personnes morales"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:30
-#: basxconnect/core/layouts/editperson/common/addresses.py:80
+#: basxconnect/core/layouts/editperson/common/addresses.py:31
+#: basxconnect/core/layouts/editperson/common/addresses.py:78
 #: basxconnect/core/layouts/editperson/common/addresses.py:267
 msgid "Add"
 msgstr "Ajouter"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:36
-#: basxconnect/core/layouts/editperson/common/addresses.py:45
+#: basxconnect/core/layouts/editperson/common/addresses.py:37
+#: basxconnect/core/layouts/editperson/common/addresses.py:46
 #: basxconnect/core/layouts/editperson/common/addresses.py:134
 #: basxconnect/core/layouts/editperson/common/addresses.py:306
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:114
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:125
 #: basxconnect/core/layouts/editperson/common/utils.py:116
 #: basxconnect/core/views/tag_views.py:109
 msgid "Save"
 msgstr "Enregistrer"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:43
-#: basxconnect/core/layouts/editperson/common/addresses.py:52
+#: basxconnect/core/layouts/editperson/common/addresses.py:44
+#: basxconnect/core/layouts/editperson/common/addresses.py:53
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:77
 #: basxconnect/core/layouts/editperson/common/utils.py:98
 #: basxconnect/core/layouts/settings_layout.py:39
 msgid "Edit"
 msgstr "Modifier"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:66
+#: basxconnect/core/layouts/editperson/common/addresses.py:74
 #: basxconnect/core/layouts/editperson/common/addresses.py:204
-#: basxconnect/core/layouts/editperson/common/head.py:12
+#: basxconnect/core/layouts/editperson/common/head.py:11
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:87
 #: basxconnect/core/layouts/settings_layout.py:53
-#: basxconnect/core/views/person/person_browse_views.py:186
+#: basxconnect/core/layouts/settings_layout.py:123
+#: basxconnect/core/views/person/person_browse_views.py:187
 msgid "Delete"
 msgstr "Supprimer"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:102
+#: basxconnect/core/layouts/editperson/common/addresses.py:99
 #: basxconnect/core/layouts/editperson/common/addresses.py:148
 msgid "primary"
 msgstr "principal"
 
 #: basxconnect/core/layouts/editperson/common/addresses.py:120
 #, python-format
 msgid "Edit %s"
@@ -178,77 +191,60 @@
 
 #: basxconnect/core/layouts/editperson/common/contributions_tab.py:17
 msgid "Contributions"
 msgstr "Contributions"
 
 #: basxconnect/core/layouts/editperson/common/contributions_tab.py:37
 #: basxconnect/core/layouts/settings_layout.py:33
-#: basxconnect/core/layouts/settings_layout.py:90
-#: basxconnect/core/views/term.py:27 basxconnect/core/wizards/add_person.py:386
+#: basxconnect/core/layouts/settings_layout.py:115
+#: basxconnect/core/views/term.py:26 basxconnect/core/wizards/add_person.py:379
 #, python-format
 msgid "Add %s"
 msgstr "Ajouter %s"
 
-#: basxconnect/core/layouts/editperson/common/documenttemplates_tab.py:30
-#, fuzzy
-#| msgid "Sender letterhead"
-msgid "Series letters"
-msgstr "En-tête de l'expéditeur"
-
-#: basxconnect/core/layouts/editperson/common/head.py:19
-msgid "Are you sure you want to delete {}?"
+#: basxconnect/core/layouts/editperson/common/documenttemplates_tab.py:19
+msgid "Documents"
 msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/head.py:23
-#: basxconnect/core/views/person/person_browse_views.py:192
+#: basxconnect/core/layouts/editperson/common/head.py:20
+#: basxconnect/core/views/person/person_browse_views.py:193
 msgid "Restore"
 msgstr "Restaurer"
 
-#: basxconnect/core/layouts/editperson/common/head.py:30
-msgid "Are you sure you want to restore {}?"
-msgstr ""
-
-#: basxconnect/core/layouts/editperson/common/head.py:34
+#: basxconnect/core/layouts/editperson/common/head.py:33
 msgid "Copy"
 msgstr "Copier"
 
-#: basxconnect/core/layouts/editperson/common/head.py:41
-msgid "Are you sure you want to copy {}?"
-msgstr ""
-
-#: basxconnect/core/layouts/editperson/common/history_tab.py:65
-#: basxconnect/core/layouts/editperson/common/history_tab.py:77
-msgid "<Value has been deleted>"
-msgstr ""
-
-#: basxconnect/core/layouts/editperson/common/history_tab.py:83
+#: basxconnect/core/layouts/editperson/common/history_tab.py:68
 msgid "History"
-msgstr "Historique"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:91
+#: basxconnect/core/layouts/editperson/common/history_tab.py:78
 msgid "Date"
 msgstr "Date"
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:97
+#: basxconnect/core/layouts/editperson/common/history_tab.py:84
 msgid "Time"
-msgstr "Heure"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:103
+#: basxconnect/core/layouts/editperson/common/history_tab.py:90
 msgid "User"
 msgstr "Utilisateur"
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:107
-#: basxconnect/core/layouts/editperson/common/history_tab.py:139
+#: basxconnect/core/layouts/editperson/common/history_tab.py:94
+#: basxconnect/core/layouts/editperson/common/history_tab.py:126
+#, fuzzy
+#| msgid "Change"
 msgid "Changes"
-msgstr "Modifications"
+msgstr "Modifier"
 
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:22
 #: basxconnect/core/layouts/settings_layout.py:16
 #: basxconnect/core/models/relationships.py:55
-#: basxconnect/core/views/menu_views.py:59
+#: basxconnect/core/views/menu_views.py:75
 msgid "Relationships"
 msgstr "Relations"
 
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:28
 msgid "Relationships to person"
 msgstr "Les relations de la personne"
 
@@ -269,36 +265,38 @@
 #: basxconnect/core/layouts/editperson/common/utils.py:26
 #: basxconnect/core/models/persons.py:152
 msgid "Status"
 msgstr "État"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:28
 msgid "Changed"
-msgstr "Modifié"
+msgstr "Modifié le"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:36
 msgid "Created"
 msgstr "Créé le"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:44
+#, fuzzy
+#| msgid "Base data"
 msgid "Meta data"
-msgstr "Méta-données"
+msgstr "Données de la base"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:52
-#: basxconnect/core/views/person/person_browse_views.py:114
-#: basxconnect/core/views/person/person_browse_views.py:244
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_browse_views.py:115
+#: basxconnect/core/views/person/person_browse_views.py:245
+#: basxconnect/core/views/person/person_details_views.py:161
 msgid "Inactive"
 msgstr "Inactif"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:52
 #: basxconnect/core/models/persons.py:58
-#: basxconnect/core/views/person/person_browse_views.py:113
-#: basxconnect/core/views/person/person_browse_views.py:244
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_browse_views.py:114
+#: basxconnect/core/views/person/person_browse_views.py:245
+#: basxconnect/core/views/person/person_details_views.py:161
 msgid "Active"
 msgstr "Actif"
 
 #: basxconnect/core/layouts/editperson/legalperson/base_data_tab.py:20
 #: basxconnect/core/layouts/editperson/personassociation/base_data_tab.py:18
 msgid "Base data"
 msgstr "Données de la base"
@@ -306,143 +304,146 @@
 #: basxconnect/core/layouts/editperson/legalperson/base_data_tab.py:25
 #: basxconnect/core/layouts/editperson/personassociation/base_data_tab.py:22
 msgid "Base Data"
 msgstr "Données de la Base"
 
 #: basxconnect/core/layouts/editperson/legalperson/mailing.py:27
 #: basxconnect/core/layouts/editperson/naturalperson/mailing.py:27
-#: basxconnect/core/layouts/editperson/personassociation/mailing.py:20
+#: basxconnect/core/layouts/editperson/personassociation/mailing.py:21
 msgid "Mailings"
 msgstr "Envois"
 
 #: basxconnect/core/layouts/editperson/legalperson/mailing.py:31
 #: basxconnect/core/layouts/editperson/naturalperson/mailing.py:31
 #: basxconnect/core/views/person/person_modals_views.py:28
+#: basxconnect/core/views/settings_views.py:29
 msgid "Settings"
 msgstr "Paramètres"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:20
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:21
+#, fuzzy
+#| msgid "Personal Data"
 msgid "Personal data"
 msgstr "Données personnelles"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:69
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:51
 msgid "Yes"
 msgstr "Oui"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:69
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:51
 msgid "No"
 msgstr "Non"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:79
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:60
 msgid "Personal Data"
 msgstr "Données personnelles"
 
 #: basxconnect/core/migrations/0015_rename_category_to_tag.py:13
 msgid "Tag"
 msgstr "Étiquette"
 
 #: basxconnect/core/migrations/0015_rename_category_to_tag.py:21
 msgid "Category"
 msgstr "Catégorie"
 
-#: basxconnect/core/models/addresses.py:20
-#: basxconnect/core/models/persons.py:243
+#: basxconnect/core/models/addresses.py:18
+#: basxconnect/core/models/persons.py:241
 msgid "Person"
 msgstr "Personne"
 
-#: basxconnect/core/models/addresses.py:32
-#: basxconnect/core/models/addresses.py:57
-#: basxconnect/core/views/person/person_browse_views.py:157
-#: basxconnect/core/wizards/add_person.py:69
+#: basxconnect/core/models/addresses.py:30
+#: basxconnect/core/models/addresses.py:54
+#: basxconnect/core/views/person/person_browse_views.py:158
+#: basxconnect/core/wizards/add_person.py:67
 msgid "Email"
 msgstr "E-mail"
 
-#: basxconnect/core/models/addresses.py:40
-#: basxconnect/core/models/addresses.py:76
-#: basxconnect/core/models/addresses.py:96
-#: basxconnect/core/models/addresses.py:118
-#: basxconnect/core/models/addresses.py:144
-#: basxconnect/core/models/persons.py:359
-#: basxconnect/core/models/persons.py:383
+#: basxconnect/core/models/addresses.py:39
+#: basxconnect/core/models/addresses.py:74
+#: basxconnect/core/models/addresses.py:93
+#: basxconnect/core/models/addresses.py:114
+#: basxconnect/core/models/addresses.py:139
+#: basxconnect/core/models/persons.py:350
+#: basxconnect/core/models/persons.py:374
 #: basxconnect/core/models/relationships.py:36
-#: basxconnect/core/wizards/add_person.py:280
+#: basxconnect/core/wizards/add_person.py:273
 msgid "Type"
 msgstr "Type"
 
-#: basxconnect/core/models/addresses.py:63
+#: basxconnect/core/models/addresses.py:60
 msgid "Email address"
 msgstr "Adresse e-mail"
 
-#: basxconnect/core/models/addresses.py:64
+#: basxconnect/core/models/addresses.py:61
 msgid "Email addresses"
 msgstr "Adresses e-mail"
 
-#: basxconnect/core/models/addresses.py:68
+#: basxconnect/core/models/addresses.py:65
 msgid "Url"
 msgstr "URL"
 
-#: basxconnect/core/models/addresses.py:84
+#: basxconnect/core/models/addresses.py:80
 msgid "Web address"
 msgstr "Adresse Web"
 
-#: basxconnect/core/models/addresses.py:85
+#: basxconnect/core/models/addresses.py:81
 msgid "Web addresses"
 msgstr "Adresses Web"
 
-#: basxconnect/core/models/addresses.py:89
-#: basxconnect/core/models/addresses.py:111
+#: basxconnect/core/models/addresses.py:85
+#: basxconnect/core/models/addresses.py:106
 msgid "Number"
 msgstr "Numéro"
 
-#: basxconnect/core/models/addresses.py:106
+#: basxconnect/core/models/addresses.py:101
 msgid "Phone number"
 msgstr "Numéro de téléphone"
 
-#: basxconnect/core/models/addresses.py:107
+#: basxconnect/core/models/addresses.py:102
 msgid "Phone numbers"
 msgstr "Numéros de téléphone"
 
-#: basxconnect/core/models/addresses.py:128
+#: basxconnect/core/models/addresses.py:122
 msgid "Fax number"
 msgstr "Numéro de télécopie"
 
-#: basxconnect/core/models/addresses.py:129
+#: basxconnect/core/models/addresses.py:123
 msgid "Fax numbers"
 msgstr "Numéros de télécopie"
 
-#: basxconnect/core/models/addresses.py:133
+#: basxconnect/core/models/addresses.py:127
 msgid "Country"
 msgstr "Pays"
 
-#: basxconnect/core/models/addresses.py:134
-#: basxconnect/core/wizards/add_person.py:48
+#: basxconnect/core/models/addresses.py:128
+#: basxconnect/core/wizards/add_person.py:46
 msgid "Address"
 msgstr "Adresse"
 
-#: basxconnect/core/models/addresses.py:135
+#: basxconnect/core/models/addresses.py:129
 msgid "Post Code"
 msgstr "Code postal"
 
-#: basxconnect/core/models/addresses.py:136
+#: basxconnect/core/models/addresses.py:130
 msgid "City"
 msgstr "Ville"
 
-#: basxconnect/core/models/addresses.py:148
+#: basxconnect/core/models/addresses.py:140
 msgid "Valid from"
 msgstr "Valide à partir de"
 
-#: basxconnect/core/models/addresses.py:149
+#: basxconnect/core/models/addresses.py:141
 msgid "Valid until"
 msgstr "Valide jusqu'à"
 
-#: basxconnect/core/models/addresses.py:164
+#: basxconnect/core/models/addresses.py:153
 msgid "Postal address"
 msgstr "Adresse postale"
 
-#: basxconnect/core/models/addresses.py:165
+#: basxconnect/core/models/addresses.py:154
 msgid "Postal addresses"
 msgstr "Adresses postales"
 
 #: basxconnect/core/models/persons.py:43
 msgid "Deleted"
 msgstr "Supprimé"
 
@@ -460,35 +461,37 @@
 
 #: basxconnect/core/models/persons.py:60
 msgid "Salutation Letter"
 msgstr "Message de salutation"
 
 #: basxconnect/core/models/persons.py:64
 msgid "Preferred Language"
-msgstr "Langue préférée"
+msgstr "Langue de préférence"
 
 #: basxconnect/core/models/persons.py:82
 msgid "Primary postal address"
 msgstr "Adresse postale principale"
 
 #: basxconnect/core/models/persons.py:95
 msgid "Primary email address"
 msgstr "Adresse e-mail principale"
 
 #: basxconnect/core/models/persons.py:108
+#, fuzzy
+#| msgid "Phone number"
 msgid "Primary phonenumber"
-msgstr "Numéro de téléphone principal"
+msgstr "Numéro de téléphone"
 
 #: basxconnect/core/models/persons.py:115
 msgid "Remarks"
 msgstr "Remarques"
 
 #: basxconnect/core/models/persons.py:132
-#: basxconnect/core/models/persons.py:316
-#: basxconnect/core/views/person/person_browse_views.py:371
+#: basxconnect/core/models/persons.py:307
+#: basxconnect/core/views/person/person_browse_views.py:372
 msgid "Person Type"
 msgstr "Type de personne"
 
 #: basxconnect/core/models/persons.py:142
 msgid "Main Type"
 msgstr "Type principal"
 
@@ -496,104 +499,100 @@
 msgid "active"
 msgstr "actif"
 
 #: basxconnect/core/models/persons.py:149
 msgid "inactive"
 msgstr "inactif"
 
-#: basxconnect/core/models/persons.py:248
+#: basxconnect/core/models/persons.py:246
 msgid "First Name"
 msgstr "Prénom"
 
-#: basxconnect/core/models/persons.py:249
+#: basxconnect/core/models/persons.py:247
 msgid "Middle Name"
 msgstr "Deuxième prénom"
 
-#: basxconnect/core/models/persons.py:250
+#: basxconnect/core/models/persons.py:248
 msgid "Last Name"
 msgstr "Nom"
 
-#: basxconnect/core/models/persons.py:251
-#, fuzzy
-#| msgid "Middle Name"
-msgid "Maiden Name"
-msgstr "Deuxième prénom"
-
-#: basxconnect/core/models/persons.py:254
+#: basxconnect/core/models/persons.py:250
 msgid "Autogenerate Display Name"
 msgstr "Générer automatiquement le nom affiché"
 
-#: basxconnect/core/models/persons.py:263
+#: basxconnect/core/models/persons.py:260
 msgid "Title"
 msgstr "Titre"
 
-#: basxconnect/core/models/persons.py:274
+#: basxconnect/core/models/persons.py:269
 msgid "Salutation"
 msgstr "Salutation"
 
-#: basxconnect/core/models/persons.py:285
+#: basxconnect/core/models/persons.py:279
 msgid "Form of address"
 msgstr "Formulaire d'adresse"
 
-#: basxconnect/core/models/persons.py:290
+#: basxconnect/core/models/persons.py:282
 msgid "Profession"
 msgstr "Profession"
 
-#: basxconnect/core/models/persons.py:294
+#: basxconnect/core/models/persons.py:286
 msgid "Date of Birth"
 msgstr "Date de naissance"
 
-#: basxconnect/core/models/persons.py:295
+#: basxconnect/core/models/persons.py:287
+#, fuzzy
+#| msgid "Date of Birth"
 msgid "Place of Birth"
-msgstr "Lieu de naissance"
+msgstr "Date de naissance"
 
-#: basxconnect/core/models/persons.py:296
+#: basxconnect/core/models/persons.py:288
 msgid "Deceased"
 msgstr "Décédé"
 
-#: basxconnect/core/models/persons.py:297
+#: basxconnect/core/models/persons.py:289
 msgid "Deceased Date"
 msgstr "Date de décès"
 
-#: basxconnect/core/models/persons.py:305
+#: basxconnect/core/models/persons.py:298
 msgid "Gender"
 msgstr "Genre"
 
-#: basxconnect/core/models/persons.py:329
+#: basxconnect/core/models/persons.py:320
 msgid "Age"
 msgstr "Âge"
 
-#: basxconnect/core/models/persons.py:346
-#: basxconnect/core/views/person/person_browse_views.py:210
+#: basxconnect/core/models/persons.py:337
+#: basxconnect/core/views/person/person_browse_views.py:211
 msgid "Natural Person"
 msgstr "Personne physique"
 
-#: basxconnect/core/models/persons.py:347
+#: basxconnect/core/models/persons.py:338
 msgid "Natural Persons"
 msgstr "Personnes physiques"
 
-#: basxconnect/core/models/persons.py:351
+#: basxconnect/core/models/persons.py:342
 msgid "Addition name"
 msgstr "Nom supplémentaire"
 
-#: basxconnect/core/models/persons.py:371
-#: basxconnect/core/views/person/person_browse_views.py:211
+#: basxconnect/core/models/persons.py:362
+#: basxconnect/core/views/person/person_browse_views.py:212
 msgid "Legal Person"
 msgstr "Personne morale"
 
-#: basxconnect/core/models/persons.py:372
+#: basxconnect/core/models/persons.py:363
 msgid "Legal Persons"
 msgstr "Personnes morales"
 
-#: basxconnect/core/models/persons.py:395
-#: basxconnect/core/views/person/person_browse_views.py:213
+#: basxconnect/core/models/persons.py:386
+#: basxconnect/core/views/person/person_browse_views.py:214
 msgid "Person Association"
 msgstr "Association"
 
-#: basxconnect/core/models/persons.py:396
+#: basxconnect/core/models/persons.py:387
 msgid "Person Associations"
 msgstr "Associations de personnes"
 
 #: basxconnect/core/models/relationships.py:9
 msgid "Name for relationship type"
 msgstr "Nom du type de relation"
 
@@ -625,127 +624,118 @@
 msgid "Ends on"
 msgstr "Se termine le"
 
 #: basxconnect/core/models/relationships.py:54
 msgid "Relationship"
 msgstr "Relation"
 
-#: basxconnect/core/models/utils.py:19 basxconnect/core/models/utils.py:75
-msgid "Terms"
-msgstr "Termes"
-
-#: basxconnect/core/models/utils.py:26
-#: basxconnect/core/views/person/person_browse_views.py:129
+#: basxconnect/core/models/utils.py:13
+#: basxconnect/core/views/person/person_browse_views.py:130
 msgid "Name"
 msgstr "Nom"
 
-#: basxconnect/core/models/utils.py:28 basxconnect/core/models/utils.py:56
+#: basxconnect/core/models/utils.py:15 basxconnect/core/models/utils.py:33
 msgid "Slug"
 msgstr "Slug"
 
-#: basxconnect/core/models/utils.py:30
+#: basxconnect/core/models/utils.py:17
 msgid "slug is human-readable, to make referencing easier"
 msgstr "Le slug est lisible par les hommes, pour faciliter le référencement"
 
-#: basxconnect/core/models/utils.py:40 basxconnect/core/models/utils.py:54
+#: basxconnect/core/models/utils.py:25 basxconnect/core/models/utils.py:31
 msgid "Vocabulary"
 msgstr "Vocabulaire"
 
-#: basxconnect/core/models/utils.py:41
+#: basxconnect/core/models/utils.py:26
 msgid "Vocabularies"
 msgstr "Vocabulaires"
 
-#: basxconnect/core/models/utils.py:55 basxconnect/core/models/utils.py:74
+#: basxconnect/core/models/utils.py:32 basxconnect/core/models/utils.py:44
 msgid "Term"
 msgstr "Terme"
 
-#: basxconnect/core/models/utils.py:58
-msgid "Disabled"
-msgstr ""
-
-#: basxconnect/core/models/utils.py:60
-msgid "Do not allow this term to be selected"
-msgstr ""
-
-#: basxconnect/core/views/menu_views.py:46
-msgid "Taxonomy"
-msgstr ""
+#: basxconnect/core/models/utils.py:45
+msgid "Terms"
+msgstr "Termes"
 
-#: basxconnect/core/views/person/person_browse_views.py:174
+#: basxconnect/core/views/person/person_browse_views.py:175
+#, fuzzy
+#| msgid "Add %s"
 msgid "Add tag"
-msgstr "Ajouter une étiquette"
+msgstr "Ajouter %s"
 
-#: basxconnect/core/views/person/person_browse_views.py:180
+#: basxconnect/core/views/person/person_browse_views.py:181
 msgid "Remove tag"
-msgstr "Retirer l'étiquette"
+msgstr ""
 
-#: basxconnect/core/views/person/person_browse_views.py:198
+#: basxconnect/core/views/person/person_browse_views.py:199
 msgid "Excel"
 msgstr "Excel"
 
-#: basxconnect/core/views/person/person_browse_views.py:248
+#: basxconnect/core/views/person/person_browse_views.py:249
 msgid "Trash"
 msgstr "Corbeille"
 
-#: basxconnect/core/views/person/person_browse_views.py:445
-#: basxconnect/core/views/person/person_details_views.py:214
+#: basxconnect/core/views/person/person_browse_views.py:446
+#: basxconnect/core/views/person/person_details_views.py:233
 msgid "Cancel"
 msgstr "Annuler"
 
-#: basxconnect/core/views/person/person_browse_views.py:451
+#: basxconnect/core/views/person/person_browse_views.py:452
 msgid "Reset"
 msgstr "Réinitialiser"
 
-#: basxconnect/core/views/person/person_browse_views.py:458
+#: basxconnect/core/views/person/person_browse_views.py:459
 msgctxt "apply filter"
 msgid "Filter"
 msgstr "Filtrer"
 
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_details_views.py:161
 #, python-format
 msgid "%s is %s"
 msgstr "%s est %s"
 
-#: basxconnect/core/views/person/person_details_views.py:159
-#, python-format
+#: basxconnect/core/views/person/person_details_views.py:178
+#, fuzzy, python-format
+#| msgid "Delete linked email subscriptions as well"
 msgid "Delete linked %s subscription as well"
-msgstr "Supprimer également les %s souscriptions liés"
+msgstr "Supprimer également les abonnements e-mail liés"
 
-#: basxconnect/core/views/person/person_details_views.py:205
+#: basxconnect/core/views/person/person_details_views.py:224
 #, python-format
 msgid "Delete email %s"
 msgstr "Supprimer l'e-mail %s"
 
-#: basxconnect/core/views/person/person_details_views.py:220
+#: basxconnect/core/views/person/person_details_views.py:239
 msgid "Confirm"
 msgstr "Confirmer"
 
 #: basxconnect/core/views/person/person_modals_views.py:32
 msgid "Edit mailing settings"
 msgstr "Modifier les préférences du courrier"
 
-#: basxconnect/core/views/person/person_modals_views.py:153
+#: basxconnect/core/views/person/person_modals_views.py:149
 msgid "Use as primary postal address"
 msgstr "Utiliser comme adresse principale"
 
-#: basxconnect/core/views/person/person_modals_views.py:216
+#: basxconnect/core/views/person/person_modals_views.py:213
 msgid "Use as primary email address"
 msgstr "Utiliser comme adresse e-mail principale"
 
-#: basxconnect/core/views/person/person_modals_views.py:224
+#: basxconnect/core/views/person/person_modals_views.py:221
 #, python-format
 msgid "Propagate change of email address to %s"
 msgstr "Propager les modifications d'adresse e-mail vers %s"
 
-#: basxconnect/core/views/person/person_modals_views.py:253
+#: basxconnect/core/views/person/person_modals_views.py:250
 msgid "Edit Email"
 msgstr "Modifier e-mail"
 
 #: basxconnect/core/views/person/search_person_view.py:21
-#: basxconnect/core/wizards/add_person.py:151
+#: basxconnect/core/wizards/add_person.py:147
 msgid "Search person"
 msgstr "Rechercher une personne"
 
 #: basxconnect/core/views/person/search_person_view.py:62
 msgid "No results"
 msgstr "Aucun résultat"
 
@@ -758,150 +748,144 @@
 msgid "Edit Relationship"
 msgstr "Modifier la relation"
 
 #: basxconnect/core/views/relationship_views.py:61
 msgid "Add Relationship"
 msgstr "Ajouter une relation"
 
+#: basxconnect/core/views/settings_views.py:31
+msgid "Information about our organization"
+msgstr "Informations sur votre organisation"
+
 #: basxconnect/core/views/tag_views.py:67
-#, python-format
+#, fuzzy, python-format
+#| msgid "Add relationship to person"
 msgid "Add tag to %(count)d person"
 msgid_plural "Add tag to %(count)d persons"
-msgstr[0] "Ajouter une étiquette à %(count)d personne"
-msgstr[1] "Ajouter une étiquette à %(count)d personnes"
+msgstr[0] "Ajouter une relation vers cette personne"
+msgstr[1] "Ajouter une relation vers cette personne"
 
 #: basxconnect/core/views/tag_views.py:73
 #, python-format
 msgid "Remove tag from %(count)d person"
 msgid_plural "Remove tag from %(count)d persons"
-msgstr[0] "Retirer l'étiquette à %(count)d personne"
-msgstr[1] "Retirer l'étiquette à %(count)d personnes"
+msgstr[0] ""
+msgstr[1] ""
 
 #: basxconnect/core/views/tag_views.py:90
 #: basxconnect/core/views/tag_views.py:112
 msgid "Create new tag"
-msgstr "Créer une nouvelle étiquette"
+msgstr ""
 
 #: basxconnect/core/views/tag_views.py:121
 msgid "Submit"
-msgstr "Soumettre"
+msgstr ""
 
 #: basxconnect/core/views/vocabulary.py:14
+#, fuzzy
+#| msgid "Vocabulary"
 msgid "Terms of vocabulary"
-msgstr "Conditions du vocabulaire"
+msgstr "Vocabulaire"
 
-#: basxconnect/core/wizards/add_person.py:105
+#: basxconnect/core/wizards/add_person.py:101
 msgid "Back"
 msgstr "Retour"
 
-#: basxconnect/core/wizards/add_person.py:116
+#: basxconnect/core/wizards/add_person.py:112
 msgid "Complete"
 msgstr "Terminer"
 
-#: basxconnect/core/wizards/add_person.py:119
+#: basxconnect/core/wizards/add_person.py:115
 msgid "Continue"
 msgstr "Continuer"
 
-#: basxconnect/core/wizards/add_person.py:131
+#: basxconnect/core/wizards/add_person.py:127
 msgid "Check for existing people before continuing"
 msgstr "Vérifier s'il existe des personnes avant de continuer"
 
-#: basxconnect/core/wizards/add_person.py:139
+#: basxconnect/core/wizards/add_person.py:135
 msgid "Start typing to search for a person..."
 msgstr "Commencez à taper pour rechercher une personne…"
 
-#: basxconnect/core/wizards/add_person.py:155
+#: basxconnect/core/wizards/add_person.py:151
 msgid ""
 "Before a new person can be added it must be confirmed that the person does "
 "not exists yet."
 msgstr ""
 "Avant de pouvoir ajouter une nouvelle personne, il faut confirmer qu'elle "
 "n'existe pas encore."
 
-#: basxconnect/core/wizards/add_person.py:171
+#: basxconnect/core/wizards/add_person.py:167
 msgid "Type of person"
 msgstr "Type de personne"
 
-#: basxconnect/core/wizards/add_person.py:177
+#: basxconnect/core/wizards/add_person.py:173
 msgid "Choose person main type"
 msgstr "Sélectionnez le type principal de la personne"
 
-#: basxconnect/core/wizards/add_person.py:180
+#: basxconnect/core/wizards/add_person.py:176
 msgid "Please choose what type of person you want to add:"
 msgstr "Veuillez sélectionner le type de personne que vous souhaitez ajouter :"
 
-#: basxconnect/core/wizards/add_person.py:195
+#: basxconnect/core/wizards/add_person.py:191
 msgid "Subtype of person"
 msgstr "Sous-type de personne"
 
-#: basxconnect/core/wizards/add_person.py:211
+#: basxconnect/core/wizards/add_person.py:207
 msgid "Choose person type"
 msgstr "Sélectionnez le type de personne"
 
-#: basxconnect/core/wizards/add_person.py:219
+#: basxconnect/core/wizards/add_person.py:215
 msgid "Add person"
 msgstr "Ajouter une personne"
 
-#: basxconnect/core/wizards/add_person.py:227
+#: basxconnect/core/wizards/add_person.py:223
 msgid "Finish"
 msgstr "Terminer"
 
-#: basxconnect/core/wizards/add_person.py:279
+#: basxconnect/core/wizards/add_person.py:272
 msgid "Search"
 msgstr "Rechercher"
 
-#: basxconnect/core/wizards/add_person.py:281
+#: basxconnect/core/wizards/add_person.py:274
 msgid "Subtype"
 msgstr "Sous-type"
 
-#: basxconnect/core/wizards/add_person.py:282
+#: basxconnect/core/wizards/add_person.py:275
 msgid "Information"
 msgstr "Information"
 
-#: basxconnect/core/wizards/add_person.py:283
+#: basxconnect/core/wizards/add_person.py:276
 msgid "Confirmation"
 msgstr "Confirmation"
 
-#: basxconnect/core/wizards/add_person.py:307
+#: basxconnect/core/wizards/add_person.py:300
 msgid "Add new person"
 msgstr "Ajouter une nouvelle personne"
 
-#: basxconnect/core/wizards/add_person.py:378
+#: basxconnect/core/wizards/add_person.py:371
 msgid "Review and confirm the entered information"
 msgstr "Valider et confirmer les informations saisies"
 
-#~ msgid "Sender letterhead"
-#~ msgstr "En-tête de l'expéditeur"
-
-#~ msgid "Logo"
-#~ msgstr "Logo"
-
-#~ msgid "Organization Name"
-#~ msgstr "Nom de l'organisation"
-
-#~ msgid "Information about our organization"
-#~ msgstr "Informations sur votre organisation"
-
-#~ msgid "Documents"
-#~ msgstr "Documents"
-
 #~ msgid "Languages"
 #~ msgstr "Langues"
 
 #~ msgid "Revisions"
 #~ msgstr "Révisions"
 
 #, fuzzy
+#~| msgid "Person category"
 #~ msgid "Person Category"
 #~ msgstr "Catégorie de personne"
 
 #~ msgid "Categories"
 #~ msgstr "Catégories"
 
 #, fuzzy
+#~| msgid "Categories"
 #~ msgid "Edit Categories"
 #~ msgstr "Catégories"
 
 #~ msgid "Unsaved changes"
 #~ msgstr "Modifications non enregistrées"
 
 #~ msgid "Discard"
@@ -945,15 +929,13 @@
 #~ "Le paramètre django BASXCONNECT.OWNER_PERSON_ID doit être défini à une "
 #~ "personne existante afin de pourvoir modifier cet écran"
 
 #~ msgid "Include trash"
 #~ msgstr "Inclure les éléments supprimés"
 
 #, fuzzy
+#~| msgid "Person B"
 #~ msgid "to \"person B\""
 #~ msgstr "Personne B"
 
 #~ msgid "No address"
 #~ msgstr "Aucune adresse"
-
-#~ msgid "Change"
-#~ msgstr "Modifier"
```

### Comparing `basxconnect-0.4.61/basxconnect/core/locale/pt/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/core/locale/pt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,174 +3,189 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-04 10:14+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: 2021-05-08 22:32+0000\n"
 "Last-Translator: ssantos <ssantos@web.de>\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/basxconnect/"
 "basxconnect/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.7-dev\n"
 
-#: basxconnect/core/apps.py:13
-msgid "BasxConnect Core"
-msgstr ""
-
-#: basxconnect/core/apps.py:29
+#: basxconnect/core/apps.py:28
 #: basxconnect/core/layouts/editperson/common/base_data.py:53
 #: basxconnect/core/models/persons.py:73
 msgid "Tags"
 msgstr "Marcadores"
 
-#: basxconnect/core/apps.py:30
+#: basxconnect/core/apps.py:29
 #, fuzzy
 #| msgid "Title"
 msgid "Titles"
 msgstr "Título"
 
-#: basxconnect/core/apps.py:31
+#: basxconnect/core/apps.py:30
 #, fuzzy
 #| msgid "Salutation"
 msgid "Salutations"
 msgstr "Saudação"
 
-#: basxconnect/core/apps.py:32
+#: basxconnect/core/apps.py:31
 #, fuzzy
 #| msgid "Form of address"
 msgid "Forms Of Address"
 msgstr "Forma de endereço"
 
-#: basxconnect/core/apps.py:33
+#: basxconnect/core/apps.py:32
 #, fuzzy
 #| msgid "Gender"
 msgid "Genders"
 msgstr "Sexo"
 
-#: basxconnect/core/apps.py:34
+#: basxconnect/core/apps.py:33
 #, fuzzy
 #| msgid "Natural Persons"
 msgid "Natural Person Types"
 msgstr "Pessoais Naturais"
 
-#: basxconnect/core/apps.py:35
+#: basxconnect/core/apps.py:34
 #, fuzzy
 #| msgid "Legal Persons"
 msgid "Legal Person Types"
 msgstr "Pessoas Legais"
 
-#: basxconnect/core/apps.py:36
+#: basxconnect/core/apps.py:35
 #, fuzzy
 #| msgid "Person A"
 msgid "Association Person Types"
 msgstr "Pessoa A"
 
-#: basxconnect/core/apps.py:37
+#: basxconnect/core/apps.py:36
 #, fuzzy
 #| msgid "Address"
 msgid "Address statuses"
 msgstr "Endereço"
 
-#: basxconnect/core/apps.py:38
+#: basxconnect/core/apps.py:37
 #, fuzzy
 #| msgid "Main Type"
 msgid "Email Types"
 msgstr "Tipo principal"
 
-#: basxconnect/core/apps.py:39
+#: basxconnect/core/apps.py:38
 #, fuzzy
 #| msgid "Type"
 msgid "URL Types"
 msgstr "Escrever"
 
-#: basxconnect/core/apps.py:40
+#: basxconnect/core/apps.py:39
 #, fuzzy
 #| msgid "Person A"
 msgid "Phone Types"
 msgstr "Pessoa A"
 
-#: basxconnect/core/apps.py:41
+#: basxconnect/core/apps.py:40
 #, fuzzy
 #| msgid "Address"
 msgid "Address Types"
 msgstr "Endereço"
 
-#: basxconnect/core/dynamic_preferences_registry.py:8
+#: basxconnect/core/dynamic_preferences_registry.py:14
+#: basxconnect/core/views/menu_views.py:55
+#: basxconnect/core/views/settings_views.py:30
 msgid "General"
 msgstr "Geral"
 
-#: basxconnect/core/dynamic_preferences_registry.py:9
-#: basxconnect/core/models/persons.py:244
-#: basxconnect/core/views/menu_views.py:28
-#: basxconnect/core/views/menu_views.py:34
+#: basxconnect/core/dynamic_preferences_registry.py:15
+#: basxconnect/core/layouts/settings_layout.py:78
+#: basxconnect/core/models/persons.py:242
+#: basxconnect/core/views/menu_views.py:42
+#: basxconnect/core/views/menu_views.py:46
+#: basxconnect/core/views/menu_views.py:65
 msgid "Persons"
 msgstr "Pessoas"
 
-#: basxconnect/core/dynamic_preferences_registry.py:18
+#: basxconnect/core/dynamic_preferences_registry.py:23
+msgid "Sender letterhead"
+msgstr "Papel timbrado do transmissor"
+
+#: basxconnect/core/dynamic_preferences_registry.py:32
+msgid "Logo"
+msgstr "Logótipo"
+
+#: basxconnect/core/dynamic_preferences_registry.py:44
+#, fuzzy
+#| msgid "Addition name"
+msgid "Organization Name"
+msgstr "Adicionar nome"
+
+#: basxconnect/core/dynamic_preferences_registry.py:53
 #, fuzzy
 #| msgid "Subtype of person"
 msgid "Default type of natural persons"
 msgstr "Subtipo de pessoa"
 
-#: basxconnect/core/dynamic_preferences_registry.py:27
+#: basxconnect/core/dynamic_preferences_registry.py:62
 #, fuzzy
 #| msgid "Person Associations"
 msgid "Default type of person associations"
 msgstr "Associações de Pessoas"
 
-#: basxconnect/core/dynamic_preferences_registry.py:36
+#: basxconnect/core/dynamic_preferences_registry.py:71
 #, fuzzy
 #| msgid "Subtype of person"
 msgid "Default type of legal persons"
 msgstr "Subtipo de pessoa"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:30
-#: basxconnect/core/layouts/editperson/common/addresses.py:80
+#: basxconnect/core/layouts/editperson/common/addresses.py:31
+#: basxconnect/core/layouts/editperson/common/addresses.py:78
 #: basxconnect/core/layouts/editperson/common/addresses.py:267
 #, fuzzy
 #| msgid "Add %s"
 msgid "Add"
 msgstr "Adicionar %s"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:36
-#: basxconnect/core/layouts/editperson/common/addresses.py:45
+#: basxconnect/core/layouts/editperson/common/addresses.py:37
+#: basxconnect/core/layouts/editperson/common/addresses.py:46
 #: basxconnect/core/layouts/editperson/common/addresses.py:134
 #: basxconnect/core/layouts/editperson/common/addresses.py:306
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:114
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:125
 #: basxconnect/core/layouts/editperson/common/utils.py:116
 #: basxconnect/core/views/tag_views.py:109
 msgid "Save"
 msgstr "Guardar"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:43
-#: basxconnect/core/layouts/editperson/common/addresses.py:52
+#: basxconnect/core/layouts/editperson/common/addresses.py:44
+#: basxconnect/core/layouts/editperson/common/addresses.py:53
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:77
 #: basxconnect/core/layouts/editperson/common/utils.py:98
 #: basxconnect/core/layouts/settings_layout.py:39
 msgid "Edit"
 msgstr "Editar"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:66
+#: basxconnect/core/layouts/editperson/common/addresses.py:74
 #: basxconnect/core/layouts/editperson/common/addresses.py:204
-#: basxconnect/core/layouts/editperson/common/head.py:12
+#: basxconnect/core/layouts/editperson/common/head.py:11
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:87
 #: basxconnect/core/layouts/settings_layout.py:53
-#: basxconnect/core/views/person/person_browse_views.py:186
+#: basxconnect/core/layouts/settings_layout.py:123
+#: basxconnect/core/views/person/person_browse_views.py:187
 msgid "Delete"
 msgstr "Apagar"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:102
+#: basxconnect/core/layouts/editperson/common/addresses.py:99
 #: basxconnect/core/layouts/editperson/common/addresses.py:148
 msgid "primary"
 msgstr ""
 
 #: basxconnect/core/layouts/editperson/common/addresses.py:120
 #, fuzzy, python-format
 #| msgid "Edit"
@@ -219,79 +234,60 @@
 #, fuzzy
 #| msgid "Confirmation"
 msgid "Contributions"
 msgstr "Confirmação"
 
 #: basxconnect/core/layouts/editperson/common/contributions_tab.py:37
 #: basxconnect/core/layouts/settings_layout.py:33
-#: basxconnect/core/layouts/settings_layout.py:90
-#: basxconnect/core/views/term.py:27 basxconnect/core/wizards/add_person.py:386
+#: basxconnect/core/layouts/settings_layout.py:115
+#: basxconnect/core/views/term.py:26 basxconnect/core/wizards/add_person.py:379
 #, python-format
 msgid "Add %s"
 msgstr "Adicionar %s"
 
-#: basxconnect/core/layouts/editperson/common/documenttemplates_tab.py:30
-#, fuzzy
-#| msgid "Sender letterhead"
-msgid "Series letters"
-msgstr "Papel timbrado do transmissor"
-
-#: basxconnect/core/layouts/editperson/common/head.py:19
-msgid "Are you sure you want to delete {}?"
+#: basxconnect/core/layouts/editperson/common/documenttemplates_tab.py:19
+msgid "Documents"
 msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/head.py:23
-#: basxconnect/core/views/person/person_browse_views.py:192
+#: basxconnect/core/layouts/editperson/common/head.py:20
+#: basxconnect/core/views/person/person_browse_views.py:193
 msgid "Restore"
 msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/head.py:30
-msgid "Are you sure you want to restore {}?"
-msgstr ""
-
-#: basxconnect/core/layouts/editperson/common/head.py:34
+#: basxconnect/core/layouts/editperson/common/head.py:33
 msgid "Copy"
 msgstr "Copiar"
 
-#: basxconnect/core/layouts/editperson/common/head.py:41
-msgid "Are you sure you want to copy {}?"
-msgstr ""
-
-#: basxconnect/core/layouts/editperson/common/history_tab.py:65
-#: basxconnect/core/layouts/editperson/common/history_tab.py:77
-msgid "<Value has been deleted>"
-msgstr ""
-
-#: basxconnect/core/layouts/editperson/common/history_tab.py:83
+#: basxconnect/core/layouts/editperson/common/history_tab.py:68
 msgid "History"
 msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:91
+#: basxconnect/core/layouts/editperson/common/history_tab.py:78
 msgid "Date"
 msgstr "Data"
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:97
+#: basxconnect/core/layouts/editperson/common/history_tab.py:84
 msgid "Time"
 msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:103
+#: basxconnect/core/layouts/editperson/common/history_tab.py:90
 msgid "User"
 msgstr "Utilizador"
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:107
-#: basxconnect/core/layouts/editperson/common/history_tab.py:139
+#: basxconnect/core/layouts/editperson/common/history_tab.py:94
+#: basxconnect/core/layouts/editperson/common/history_tab.py:126
 #, fuzzy
 #| msgid "Change"
 msgid "Changes"
 msgstr "Alterar"
 
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:22
 #: basxconnect/core/layouts/settings_layout.py:16
 #: basxconnect/core/models/relationships.py:55
-#: basxconnect/core/views/menu_views.py:59
+#: basxconnect/core/views/menu_views.py:75
 msgid "Relationships"
 msgstr "Relações"
 
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:28
 #, fuzzy
 #| msgid "Relationship types"
 msgid "Relationships to person"
@@ -333,25 +329,25 @@
 #: basxconnect/core/layouts/editperson/common/utils.py:44
 #, fuzzy
 #| msgid "Base data"
 msgid "Meta data"
 msgstr "Base de dados"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:52
-#: basxconnect/core/views/person/person_browse_views.py:114
-#: basxconnect/core/views/person/person_browse_views.py:244
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_browse_views.py:115
+#: basxconnect/core/views/person/person_browse_views.py:245
+#: basxconnect/core/views/person/person_details_views.py:161
 msgid "Inactive"
 msgstr "Inactivo"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:52
 #: basxconnect/core/models/persons.py:58
-#: basxconnect/core/views/person/person_browse_views.py:113
-#: basxconnect/core/views/person/person_browse_views.py:244
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_browse_views.py:114
+#: basxconnect/core/views/person/person_browse_views.py:245
+#: basxconnect/core/views/person/person_details_views.py:161
 msgid "Active"
 msgstr "Ativo"
 
 #: basxconnect/core/layouts/editperson/legalperson/base_data_tab.py:20
 #: basxconnect/core/layouts/editperson/personassociation/base_data_tab.py:18
 msgid "Base data"
 msgstr "Base de dados"
@@ -361,39 +357,40 @@
 #, fuzzy
 #| msgid "Base data"
 msgid "Base Data"
 msgstr "Base de dados"
 
 #: basxconnect/core/layouts/editperson/legalperson/mailing.py:27
 #: basxconnect/core/layouts/editperson/naturalperson/mailing.py:27
-#: basxconnect/core/layouts/editperson/personassociation/mailing.py:20
+#: basxconnect/core/layouts/editperson/personassociation/mailing.py:21
 msgid "Mailings"
 msgstr ""
 
 #: basxconnect/core/layouts/editperson/legalperson/mailing.py:31
 #: basxconnect/core/layouts/editperson/naturalperson/mailing.py:31
 #: basxconnect/core/views/person/person_modals_views.py:28
+#: basxconnect/core/views/settings_views.py:29
 msgid "Settings"
 msgstr "Definições"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:20
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:21
 #, fuzzy
 #| msgid "Person"
 msgid "Personal data"
 msgstr "Pessoa"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:69
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:51
 msgid "Yes"
 msgstr ""
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:69
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:51
 msgid "No"
 msgstr ""
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:79
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:60
 #, fuzzy
 #| msgid "Person"
 msgid "Personal Data"
 msgstr "Pessoa"
 
 #: basxconnect/core/migrations/0015_rename_category_to_tag.py:13
 #, fuzzy
@@ -401,109 +398,109 @@
 msgid "Tag"
 msgstr "Marcadores"
 
 #: basxconnect/core/migrations/0015_rename_category_to_tag.py:21
 msgid "Category"
 msgstr "Categoria"
 
-#: basxconnect/core/models/addresses.py:20
-#: basxconnect/core/models/persons.py:243
+#: basxconnect/core/models/addresses.py:18
+#: basxconnect/core/models/persons.py:241
 msgid "Person"
 msgstr "Pessoa"
 
-#: basxconnect/core/models/addresses.py:32
-#: basxconnect/core/models/addresses.py:57
-#: basxconnect/core/views/person/person_browse_views.py:157
-#: basxconnect/core/wizards/add_person.py:69
+#: basxconnect/core/models/addresses.py:30
+#: basxconnect/core/models/addresses.py:54
+#: basxconnect/core/views/person/person_browse_views.py:158
+#: basxconnect/core/wizards/add_person.py:67
 msgid "Email"
 msgstr "E-mail"
 
-#: basxconnect/core/models/addresses.py:40
-#: basxconnect/core/models/addresses.py:76
-#: basxconnect/core/models/addresses.py:96
-#: basxconnect/core/models/addresses.py:118
-#: basxconnect/core/models/addresses.py:144
-#: basxconnect/core/models/persons.py:359
-#: basxconnect/core/models/persons.py:383
+#: basxconnect/core/models/addresses.py:39
+#: basxconnect/core/models/addresses.py:74
+#: basxconnect/core/models/addresses.py:93
+#: basxconnect/core/models/addresses.py:114
+#: basxconnect/core/models/addresses.py:139
+#: basxconnect/core/models/persons.py:350
+#: basxconnect/core/models/persons.py:374
 #: basxconnect/core/models/relationships.py:36
-#: basxconnect/core/wizards/add_person.py:280
+#: basxconnect/core/wizards/add_person.py:273
 msgid "Type"
 msgstr "Escrever"
 
-#: basxconnect/core/models/addresses.py:63
+#: basxconnect/core/models/addresses.py:60
 msgid "Email address"
 msgstr "Endereço do E-mail"
 
-#: basxconnect/core/models/addresses.py:64
+#: basxconnect/core/models/addresses.py:61
 msgid "Email addresses"
 msgstr "Endereço do E-mail"
 
-#: basxconnect/core/models/addresses.py:68
+#: basxconnect/core/models/addresses.py:65
 msgid "Url"
 msgstr "Url"
 
-#: basxconnect/core/models/addresses.py:84
+#: basxconnect/core/models/addresses.py:80
 msgid "Web address"
 msgstr "Endereço web"
 
-#: basxconnect/core/models/addresses.py:85
+#: basxconnect/core/models/addresses.py:81
 msgid "Web addresses"
 msgstr "Endereços web"
 
-#: basxconnect/core/models/addresses.py:89
-#: basxconnect/core/models/addresses.py:111
+#: basxconnect/core/models/addresses.py:85
+#: basxconnect/core/models/addresses.py:106
 msgid "Number"
 msgstr "Número"
 
-#: basxconnect/core/models/addresses.py:106
+#: basxconnect/core/models/addresses.py:101
 msgid "Phone number"
 msgstr "Número de Telemóvel"
 
-#: basxconnect/core/models/addresses.py:107
+#: basxconnect/core/models/addresses.py:102
 msgid "Phone numbers"
 msgstr "Números de Telemóveis"
 
-#: basxconnect/core/models/addresses.py:128
+#: basxconnect/core/models/addresses.py:122
 msgid "Fax number"
 msgstr "Número de Fax"
 
-#: basxconnect/core/models/addresses.py:129
+#: basxconnect/core/models/addresses.py:123
 msgid "Fax numbers"
 msgstr "Números de Fax"
 
-#: basxconnect/core/models/addresses.py:133
+#: basxconnect/core/models/addresses.py:127
 msgid "Country"
 msgstr "Pais"
 
-#: basxconnect/core/models/addresses.py:134
-#: basxconnect/core/wizards/add_person.py:48
+#: basxconnect/core/models/addresses.py:128
+#: basxconnect/core/wizards/add_person.py:46
 msgid "Address"
 msgstr "Endereço"
 
-#: basxconnect/core/models/addresses.py:135
+#: basxconnect/core/models/addresses.py:129
 msgid "Post Code"
 msgstr "Código-Postal"
 
-#: basxconnect/core/models/addresses.py:136
+#: basxconnect/core/models/addresses.py:130
 msgid "City"
 msgstr "Cidade"
 
-#: basxconnect/core/models/addresses.py:148
+#: basxconnect/core/models/addresses.py:140
 msgid "Valid from"
 msgstr ""
 
-#: basxconnect/core/models/addresses.py:149
+#: basxconnect/core/models/addresses.py:141
 msgid "Valid until"
 msgstr ""
 
-#: basxconnect/core/models/addresses.py:164
+#: basxconnect/core/models/addresses.py:153
 msgid "Postal address"
 msgstr "Endereço Postal"
 
-#: basxconnect/core/models/addresses.py:165
+#: basxconnect/core/models/addresses.py:154
 msgid "Postal addresses"
 msgstr "Endereços Postais"
 
 #: basxconnect/core/models/persons.py:43
 msgid "Deleted"
 msgstr "Eliminado"
 
@@ -542,16 +539,16 @@
 msgstr "Número de Telemóvel"
 
 #: basxconnect/core/models/persons.py:115
 msgid "Remarks"
 msgstr "Observações"
 
 #: basxconnect/core/models/persons.py:132
-#: basxconnect/core/models/persons.py:316
-#: basxconnect/core/views/person/person_browse_views.py:371
+#: basxconnect/core/models/persons.py:307
+#: basxconnect/core/views/person/person_browse_views.py:372
 #, fuzzy
 #| msgid "Person A"
 msgid "Person Type"
 msgstr "Pessoa A"
 
 #: basxconnect/core/models/persons.py:142
 msgid "Main Type"
@@ -561,106 +558,100 @@
 msgid "active"
 msgstr "Ativo"
 
 #: basxconnect/core/models/persons.py:149
 msgid "inactive"
 msgstr "Inativo"
 
-#: basxconnect/core/models/persons.py:248
+#: basxconnect/core/models/persons.py:246
 msgid "First Name"
 msgstr "Primeiro Nome"
 
-#: basxconnect/core/models/persons.py:249
+#: basxconnect/core/models/persons.py:247
 msgid "Middle Name"
 msgstr "Nome do Meio"
 
-#: basxconnect/core/models/persons.py:250
+#: basxconnect/core/models/persons.py:248
 msgid "Last Name"
 msgstr "Último Nome"
 
-#: basxconnect/core/models/persons.py:251
-#, fuzzy
-#| msgid "Middle Name"
-msgid "Maiden Name"
-msgstr "Nome do Meio"
-
-#: basxconnect/core/models/persons.py:254
+#: basxconnect/core/models/persons.py:250
 msgid "Autogenerate Display Name"
 msgstr ""
 
-#: basxconnect/core/models/persons.py:263
+#: basxconnect/core/models/persons.py:260
 msgid "Title"
 msgstr "Título"
 
-#: basxconnect/core/models/persons.py:274
+#: basxconnect/core/models/persons.py:269
 msgid "Salutation"
 msgstr "Saudação"
 
-#: basxconnect/core/models/persons.py:285
+#: basxconnect/core/models/persons.py:279
 msgid "Form of address"
 msgstr "Forma de endereço"
 
-#: basxconnect/core/models/persons.py:290
+#: basxconnect/core/models/persons.py:282
 msgid "Profession"
 msgstr "Profissão"
 
-#: basxconnect/core/models/persons.py:294
+#: basxconnect/core/models/persons.py:286
 msgid "Date of Birth"
 msgstr "Data de nascimento"
 
-#: basxconnect/core/models/persons.py:295
+#: basxconnect/core/models/persons.py:287
 #, fuzzy
 #| msgid "Date of Birth"
 msgid "Place of Birth"
 msgstr "Data de nascimento"
 
-#: basxconnect/core/models/persons.py:296
+#: basxconnect/core/models/persons.py:288
 msgid "Deceased"
 msgstr "Falecido"
 
-#: basxconnect/core/models/persons.py:297
+#: basxconnect/core/models/persons.py:289
 msgid "Deceased Date"
 msgstr "Data de Falecimento"
 
-#: basxconnect/core/models/persons.py:305
+#: basxconnect/core/models/persons.py:298
 msgid "Gender"
 msgstr "Sexo"
 
-#: basxconnect/core/models/persons.py:329
+#: basxconnect/core/models/persons.py:320
 msgid "Age"
 msgstr ""
 
-#: basxconnect/core/models/persons.py:346
-#: basxconnect/core/views/person/person_browse_views.py:210
+#: basxconnect/core/models/persons.py:337
+#: basxconnect/core/views/person/person_browse_views.py:211
 msgid "Natural Person"
 msgstr "Pessoa Natural"
 
-#: basxconnect/core/models/persons.py:347
+#: basxconnect/core/models/persons.py:338
 msgid "Natural Persons"
 msgstr "Pessoais Naturais"
 
-#: basxconnect/core/models/persons.py:351
+#: basxconnect/core/models/persons.py:342
 msgid "Addition name"
 msgstr "Adicionar nome"
 
-#: basxconnect/core/models/persons.py:371
-#: basxconnect/core/views/person/person_browse_views.py:211
+#: basxconnect/core/models/persons.py:362
+#: basxconnect/core/views/person/person_browse_views.py:212
 msgid "Legal Person"
 msgstr "Pessoa Legal"
 
-#: basxconnect/core/models/persons.py:372
+#: basxconnect/core/models/persons.py:363
 msgid "Legal Persons"
 msgstr "Pessoas Legais"
 
-#: basxconnect/core/models/persons.py:395
-#: basxconnect/core/views/person/person_browse_views.py:213
+#: basxconnect/core/models/persons.py:386
+#: basxconnect/core/views/person/person_browse_views.py:214
 msgid "Person Association"
 msgstr "Associação de Pessoa"
 
-#: basxconnect/core/models/persons.py:396
+#: basxconnect/core/models/persons.py:387
 msgid "Person Associations"
 msgstr "Associações de Pessoas"
 
 #: basxconnect/core/models/relationships.py:9
 msgid "Name for relationship type"
 msgstr "Nome do tipo de relação"
 
@@ -692,139 +683,127 @@
 msgid "Ends on"
 msgstr "Terminar"
 
 #: basxconnect/core/models/relationships.py:54
 msgid "Relationship"
 msgstr "Relação"
 
-#: basxconnect/core/models/utils.py:19 basxconnect/core/models/utils.py:75
-msgid "Terms"
-msgstr "Termos"
-
-#: basxconnect/core/models/utils.py:26
-#: basxconnect/core/views/person/person_browse_views.py:129
+#: basxconnect/core/models/utils.py:13
+#: basxconnect/core/views/person/person_browse_views.py:130
 msgid "Name"
 msgstr "Nome"
 
-#: basxconnect/core/models/utils.py:28 basxconnect/core/models/utils.py:56
+#: basxconnect/core/models/utils.py:15 basxconnect/core/models/utils.py:33
 msgid "Slug"
 msgstr "Slug"
 
-#: basxconnect/core/models/utils.py:30
+#: basxconnect/core/models/utils.py:17
 msgid "slug is human-readable, to make referencing easier"
 msgstr "slug é legível por humanos, para facilitar a referenciação"
 
-#: basxconnect/core/models/utils.py:40 basxconnect/core/models/utils.py:54
+#: basxconnect/core/models/utils.py:25 basxconnect/core/models/utils.py:31
 msgid "Vocabulary"
 msgstr ""
 
-#: basxconnect/core/models/utils.py:41
+#: basxconnect/core/models/utils.py:26
 msgid "Vocabularies"
 msgstr ""
 
-#: basxconnect/core/models/utils.py:55 basxconnect/core/models/utils.py:74
+#: basxconnect/core/models/utils.py:32 basxconnect/core/models/utils.py:44
 msgid "Term"
 msgstr "Termo"
 
-#: basxconnect/core/models/utils.py:58
-msgid "Disabled"
-msgstr ""
-
-#: basxconnect/core/models/utils.py:60
-msgid "Do not allow this term to be selected"
-msgstr ""
-
-#: basxconnect/core/views/menu_views.py:46
-msgid "Taxonomy"
-msgstr ""
+#: basxconnect/core/models/utils.py:45
+msgid "Terms"
+msgstr "Termos"
 
-#: basxconnect/core/views/person/person_browse_views.py:174
+#: basxconnect/core/views/person/person_browse_views.py:175
 #, fuzzy
 #| msgid "Add %s"
 msgid "Add tag"
 msgstr "Adicionar %s"
 
-#: basxconnect/core/views/person/person_browse_views.py:180
+#: basxconnect/core/views/person/person_browse_views.py:181
 msgid "Remove tag"
 msgstr ""
 
-#: basxconnect/core/views/person/person_browse_views.py:198
+#: basxconnect/core/views/person/person_browse_views.py:199
 msgid "Excel"
 msgstr ""
 
-#: basxconnect/core/views/person/person_browse_views.py:248
+#: basxconnect/core/views/person/person_browse_views.py:249
 msgid "Trash"
 msgstr ""
 
-#: basxconnect/core/views/person/person_browse_views.py:445
-#: basxconnect/core/views/person/person_details_views.py:214
+#: basxconnect/core/views/person/person_browse_views.py:446
+#: basxconnect/core/views/person/person_details_views.py:233
 msgid "Cancel"
 msgstr "Cancelar"
 
-#: basxconnect/core/views/person/person_browse_views.py:451
+#: basxconnect/core/views/person/person_browse_views.py:452
 msgid "Reset"
 msgstr "Reiniciar"
 
-#: basxconnect/core/views/person/person_browse_views.py:458
+#: basxconnect/core/views/person/person_browse_views.py:459
 msgctxt "apply filter"
 msgid "Filter"
 msgstr "Filtrar"
 
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_details_views.py:161
 #, python-format
 msgid "%s is %s"
 msgstr "%s é %s"
 
-#: basxconnect/core/views/person/person_details_views.py:159
+#: basxconnect/core/views/person/person_details_views.py:178
 #, python-format
 msgid "Delete linked %s subscription as well"
 msgstr ""
 
-#: basxconnect/core/views/person/person_details_views.py:205
+#: basxconnect/core/views/person/person_details_views.py:224
 #, python-format
 msgid "Delete email %s"
 msgstr ""
 
-#: basxconnect/core/views/person/person_details_views.py:220
+#: basxconnect/core/views/person/person_details_views.py:239
 #, fuzzy
 #| msgid "Confirmation"
 msgid "Confirm"
 msgstr "Confirmação"
 
 #: basxconnect/core/views/person/person_modals_views.py:32
 #, fuzzy
 #| msgid "Edit"
 msgid "Edit mailing settings"
 msgstr "Editar"
 
-#: basxconnect/core/views/person/person_modals_views.py:153
+#: basxconnect/core/views/person/person_modals_views.py:149
 #, fuzzy
 #| msgid "Primary postal address"
 msgid "Use as primary postal address"
 msgstr "Endereço postal principal"
 
-#: basxconnect/core/views/person/person_modals_views.py:216
+#: basxconnect/core/views/person/person_modals_views.py:213
 #, fuzzy
 #| msgid "Primary postal address"
 msgid "Use as primary email address"
 msgstr "Endereço postal principal"
 
-#: basxconnect/core/views/person/person_modals_views.py:224
+#: basxconnect/core/views/person/person_modals_views.py:221
 #, python-format
 msgid "Propagate change of email address to %s"
 msgstr ""
 
-#: basxconnect/core/views/person/person_modals_views.py:253
+#: basxconnect/core/views/person/person_modals_views.py:250
 #, fuzzy
 #| msgid "Email"
 msgid "Edit Email"
 msgstr "E-mail"
 
 #: basxconnect/core/views/person/search_person_view.py:21
-#: basxconnect/core/wizards/add_person.py:151
+#: basxconnect/core/wizards/add_person.py:147
 msgid "Search person"
 msgstr "Procurar pessoa"
 
 #: basxconnect/core/views/person/search_person_view.py:62
 msgid "No results"
 msgstr "Nenhum resultado"
 
@@ -841,14 +820,18 @@
 
 #: basxconnect/core/views/relationship_views.py:61
 #, fuzzy
 #| msgid "Relationship"
 msgid "Add Relationship"
 msgstr "Relação"
 
+#: basxconnect/core/views/settings_views.py:31
+msgid "Information about our organization"
+msgstr "Informação sobre a nossa organização"
+
 #: basxconnect/core/views/tag_views.py:67
 #, fuzzy, python-format
 #| msgid "Relationship types"
 msgid "Add tag to %(count)d person"
 msgid_plural "Add tag to %(count)d persons"
 msgstr[0] "Tipos de Relações"
 msgstr[1] "Tipos de Relações"
@@ -869,108 +852,94 @@
 msgid "Submit"
 msgstr ""
 
 #: basxconnect/core/views/vocabulary.py:14
 msgid "Terms of vocabulary"
 msgstr ""
 
-#: basxconnect/core/wizards/add_person.py:105
+#: basxconnect/core/wizards/add_person.py:101
 msgid "Back"
 msgstr "Voltar"
 
-#: basxconnect/core/wizards/add_person.py:116
+#: basxconnect/core/wizards/add_person.py:112
 msgid "Complete"
 msgstr "Completo"
 
-#: basxconnect/core/wizards/add_person.py:119
+#: basxconnect/core/wizards/add_person.py:115
 msgid "Continue"
 msgstr "Continuar"
 
-#: basxconnect/core/wizards/add_person.py:131
+#: basxconnect/core/wizards/add_person.py:127
 msgid "Check for existing people before continuing"
 msgstr "Verificar as pessoas existentes antes de continuar"
 
-#: basxconnect/core/wizards/add_person.py:139
+#: basxconnect/core/wizards/add_person.py:135
 msgid "Start typing to search for a person..."
 msgstr "Comece a digitar para procurar uma pessoa..."
 
-#: basxconnect/core/wizards/add_person.py:155
+#: basxconnect/core/wizards/add_person.py:151
 msgid ""
 "Before a new person can be added it must be confirmed that the person does "
 "not exists yet."
 msgstr ""
 "Antes que uma nova pessoa possa ser acrescentada, deve ser confirmado que a "
 "pessoa ainda não existe."
 
-#: basxconnect/core/wizards/add_person.py:171
+#: basxconnect/core/wizards/add_person.py:167
 msgid "Type of person"
 msgstr "Tipo de pessoa"
 
-#: basxconnect/core/wizards/add_person.py:177
+#: basxconnect/core/wizards/add_person.py:173
 msgid "Choose person main type"
 msgstr "Escolha o tipo de pessoa principal"
 
-#: basxconnect/core/wizards/add_person.py:180
+#: basxconnect/core/wizards/add_person.py:176
 msgid "Please choose what type of person you want to add:"
 msgstr "Por favor selecione o tipo de pessoa quer adicionar:"
 
-#: basxconnect/core/wizards/add_person.py:195
+#: basxconnect/core/wizards/add_person.py:191
 msgid "Subtype of person"
 msgstr "Subtipo de pessoa"
 
-#: basxconnect/core/wizards/add_person.py:211
+#: basxconnect/core/wizards/add_person.py:207
 msgid "Choose person type"
 msgstr "Escolher o tipo de pessoa"
 
-#: basxconnect/core/wizards/add_person.py:219
+#: basxconnect/core/wizards/add_person.py:215
 msgid "Add person"
 msgstr "Adicionar pessoa"
 
-#: basxconnect/core/wizards/add_person.py:227
+#: basxconnect/core/wizards/add_person.py:223
 msgid "Finish"
 msgstr "Concluir"
 
-#: basxconnect/core/wizards/add_person.py:279
+#: basxconnect/core/wizards/add_person.py:272
 msgid "Search"
 msgstr "Pesquisar"
 
-#: basxconnect/core/wizards/add_person.py:281
+#: basxconnect/core/wizards/add_person.py:274
 msgid "Subtype"
 msgstr "Subtipo"
 
-#: basxconnect/core/wizards/add_person.py:282
+#: basxconnect/core/wizards/add_person.py:275
 msgid "Information"
 msgstr "Informação"
 
-#: basxconnect/core/wizards/add_person.py:283
+#: basxconnect/core/wizards/add_person.py:276
 msgid "Confirmation"
 msgstr "Confirmação"
 
-#: basxconnect/core/wizards/add_person.py:307
+#: basxconnect/core/wizards/add_person.py:300
 msgid "Add new person"
 msgstr "Adicionar nova pessoa"
 
-#: basxconnect/core/wizards/add_person.py:378
+#: basxconnect/core/wizards/add_person.py:371
 msgid "Review and confirm the entered information"
 msgstr "Rever e confirmar informação introduzida"
 
-#~ msgid "Sender letterhead"
-#~ msgstr "Papel timbrado do transmissor"
-
-#~ msgid "Logo"
-#~ msgstr "Logótipo"
-
-#, fuzzy
-#~| msgid "Addition name"
-#~ msgid "Organization Name"
-#~ msgstr "Adicionar nome"
-
-#~ msgid "Information about our organization"
-#~ msgstr "Informação sobre a nossa organização"
-
 #~ msgid "Languages"
 #~ msgstr "Línguas"
 
 #~ msgid "Revisions"
 #~ msgstr "Revisões"
 
 #, fuzzy
```

### Comparing `basxconnect-0.4.61/basxconnect/core/locale/th/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/core/locale/th/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,142 +3,155 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-08 16:43+0700\n"
-"PO-Revision-Date: 2023-04-05 02:46+0000\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
+"PO-Revision-Date: 2022-03-30 10:08+0000\n"
 "Last-Translator: Tidaphan <tida@basx.dev>\n"
 "Language-Team: Thai <https://hosted.weblate.org/projects/basxconnect/"
 "basxconnect/th/>\n"
 "Language: th\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.17-dev\n"
+"X-Generator: Weblate 4.12-dev\n"
 
-#: basxconnect/core/apps.py:13
-msgid "BasxConnect Core"
-msgstr "BasxConnect Core"
-
-#: basxconnect/core/apps.py:29
+#: basxconnect/core/apps.py:28
 #: basxconnect/core/layouts/editperson/common/base_data.py:53
 #: basxconnect/core/models/persons.py:73
 msgid "Tags"
 msgstr "แท็ก"
 
-#: basxconnect/core/apps.py:30
+#: basxconnect/core/apps.py:29
 msgid "Titles"
 msgstr "หัวเรื่อง"
 
-#: basxconnect/core/apps.py:31
+#: basxconnect/core/apps.py:30
 msgid "Salutations"
 msgstr "คำนำหน้านาม"
 
-#: basxconnect/core/apps.py:32
+#: basxconnect/core/apps.py:31
 msgid "Forms Of Address"
 msgstr "ประเภทที่อยู่อาศัย"
 
-#: basxconnect/core/apps.py:33
+#: basxconnect/core/apps.py:32
 msgid "Genders"
 msgstr "เพศ"
 
-#: basxconnect/core/apps.py:34
+#: basxconnect/core/apps.py:33
 msgid "Natural Person Types"
 msgstr "บุคคลธรรมดา"
 
-#: basxconnect/core/apps.py:35
+#: basxconnect/core/apps.py:34
 msgid "Legal Person Types"
 msgstr "นิติบุคคล"
 
-#: basxconnect/core/apps.py:36
+#: basxconnect/core/apps.py:35
 msgid "Association Person Types"
 msgstr "กลุ่มบุคคล สมาคม"
 
-#: basxconnect/core/apps.py:37
+#: basxconnect/core/apps.py:36
 msgid "Address statuses"
 msgstr "ประเภทที่อยู่"
 
-#: basxconnect/core/apps.py:38
+#: basxconnect/core/apps.py:37
 msgid "Email Types"
 msgstr "อีเมล์"
 
-#: basxconnect/core/apps.py:39
+#: basxconnect/core/apps.py:38
 msgid "URL Types"
 msgstr "ประเภทของ URL"
 
-#: basxconnect/core/apps.py:40
+#: basxconnect/core/apps.py:39
 msgid "Phone Types"
 msgstr "ประเภทโทรศัพท์"
 
-#: basxconnect/core/apps.py:41
+#: basxconnect/core/apps.py:40
 msgid "Address Types"
 msgstr "ประเภทที่อยู่"
 
-#: basxconnect/core/dynamic_preferences_registry.py:8
+#: basxconnect/core/dynamic_preferences_registry.py:14
+#: basxconnect/core/views/menu_views.py:55
+#: basxconnect/core/views/settings_views.py:30
 msgid "General"
 msgstr "ทั่วไป"
 
-#: basxconnect/core/dynamic_preferences_registry.py:9
-#: basxconnect/core/models/persons.py:244
-#: basxconnect/core/views/menu_views.py:28
-#: basxconnect/core/views/menu_views.py:34
+#: basxconnect/core/dynamic_preferences_registry.py:15
+#: basxconnect/core/layouts/settings_layout.py:78
+#: basxconnect/core/models/persons.py:242
+#: basxconnect/core/views/menu_views.py:42
+#: basxconnect/core/views/menu_views.py:46
+#: basxconnect/core/views/menu_views.py:65
 msgid "Persons"
 msgstr "บุคคล"
 
-#: basxconnect/core/dynamic_preferences_registry.py:18
+#: basxconnect/core/dynamic_preferences_registry.py:23
+msgid "Sender letterhead"
+msgstr "หัวจดหมาย"
+
+#: basxconnect/core/dynamic_preferences_registry.py:32
+msgid "Logo"
+msgstr "โลโก้"
+
+#: basxconnect/core/dynamic_preferences_registry.py:44
+msgid "Organization Name"
+msgstr "ชื่อองค์กร"
+
+#: basxconnect/core/dynamic_preferences_registry.py:53
 msgid "Default type of natural persons"
 msgstr "ค่าเริ่มต้นประเภทบุคคลธรรมดา"
 
-#: basxconnect/core/dynamic_preferences_registry.py:27
+#: basxconnect/core/dynamic_preferences_registry.py:62
 msgid "Default type of person associations"
 msgstr "ค่าเริ่มต้นประเภทกลุ่มบุคคล"
 
-#: basxconnect/core/dynamic_preferences_registry.py:36
+#: basxconnect/core/dynamic_preferences_registry.py:71
 msgid "Default type of legal persons"
 msgstr "ค่าเริ่มต้นประเภทนิติบุคคล"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:30
-#: basxconnect/core/layouts/editperson/common/addresses.py:80
+#: basxconnect/core/layouts/editperson/common/addresses.py:31
+#: basxconnect/core/layouts/editperson/common/addresses.py:78
 #: basxconnect/core/layouts/editperson/common/addresses.py:267
 msgid "Add"
 msgstr "เพิ่ม"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:36
-#: basxconnect/core/layouts/editperson/common/addresses.py:45
+#: basxconnect/core/layouts/editperson/common/addresses.py:37
+#: basxconnect/core/layouts/editperson/common/addresses.py:46
 #: basxconnect/core/layouts/editperson/common/addresses.py:134
 #: basxconnect/core/layouts/editperson/common/addresses.py:306
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:114
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:125
 #: basxconnect/core/layouts/editperson/common/utils.py:116
 #: basxconnect/core/views/tag_views.py:109
 msgid "Save"
 msgstr "บันทึก"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:43
-#: basxconnect/core/layouts/editperson/common/addresses.py:52
+#: basxconnect/core/layouts/editperson/common/addresses.py:44
+#: basxconnect/core/layouts/editperson/common/addresses.py:53
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:77
 #: basxconnect/core/layouts/editperson/common/utils.py:98
 #: basxconnect/core/layouts/settings_layout.py:39
 msgid "Edit"
 msgstr "แก้ไข"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:66
+#: basxconnect/core/layouts/editperson/common/addresses.py:74
 #: basxconnect/core/layouts/editperson/common/addresses.py:204
-#: basxconnect/core/layouts/editperson/common/head.py:12
+#: basxconnect/core/layouts/editperson/common/head.py:11
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:87
 #: basxconnect/core/layouts/settings_layout.py:53
-#: basxconnect/core/views/person/person_browse_views.py:186
+#: basxconnect/core/layouts/settings_layout.py:123
+#: basxconnect/core/views/person/person_browse_views.py:187
 msgid "Delete"
 msgstr "ลบ"
 
-#: basxconnect/core/layouts/editperson/common/addresses.py:102
+#: basxconnect/core/layouts/editperson/common/addresses.py:99
 #: basxconnect/core/layouts/editperson/common/addresses.py:148
 msgid "primary"
 msgstr "ข้อมูลหลัก"
 
 #: basxconnect/core/layouts/editperson/common/addresses.py:120
 #, python-format
 msgid "Edit %s"
@@ -178,75 +191,60 @@
 
 #: basxconnect/core/layouts/editperson/common/contributions_tab.py:17
 msgid "Contributions"
 msgstr "เงินบริจาค"
 
 #: basxconnect/core/layouts/editperson/common/contributions_tab.py:37
 #: basxconnect/core/layouts/settings_layout.py:33
-#: basxconnect/core/layouts/settings_layout.py:90
-#: basxconnect/core/views/term.py:27 basxconnect/core/wizards/add_person.py:386
+#: basxconnect/core/layouts/settings_layout.py:115
+#: basxconnect/core/views/term.py:26 basxconnect/core/wizards/add_person.py:379
 #, python-format
 msgid "Add %s"
 msgstr "เพิ่ม %s"
 
-#: basxconnect/core/layouts/editperson/common/documenttemplates_tab.py:30
-msgid "Series letters"
-msgstr "ชุดตัวอักษร"
-
-#: basxconnect/core/layouts/editperson/common/head.py:19
-msgid "Are you sure you want to delete {}?"
-msgstr "คุณแน่ใจหรือว่าต้องการลบ {}?"
+#: basxconnect/core/layouts/editperson/common/documenttemplates_tab.py:19
+msgid "Documents"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/head.py:23
-#: basxconnect/core/views/person/person_browse_views.py:192
+#: basxconnect/core/layouts/editperson/common/head.py:20
+#: basxconnect/core/views/person/person_browse_views.py:193
 msgid "Restore"
 msgstr "เรียกคืนค่า"
 
-#: basxconnect/core/layouts/editperson/common/head.py:30
-msgid "Are you sure you want to restore {}?"
-msgstr "คุณแน่ใจหรือไม่ว่าต้องการกู้คืน {}?"
-
-#: basxconnect/core/layouts/editperson/common/head.py:34
+#: basxconnect/core/layouts/editperson/common/head.py:33
 msgid "Copy"
 msgstr "คัดลอก"
 
-#: basxconnect/core/layouts/editperson/common/head.py:41
-msgid "Are you sure you want to copy {}?"
-msgstr "คุณแน่ใจหรือไม่ว่าต้องการคัดลอก {}?"
-
-#: basxconnect/core/layouts/editperson/common/history_tab.py:65
-#: basxconnect/core/layouts/editperson/common/history_tab.py:77
-msgid "<Value has been deleted>"
-msgstr "<ค่าถูกลบ>"
-
-#: basxconnect/core/layouts/editperson/common/history_tab.py:83
+#: basxconnect/core/layouts/editperson/common/history_tab.py:68
 msgid "History"
-msgstr "ประวัติ"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:91
+#: basxconnect/core/layouts/editperson/common/history_tab.py:78
 msgid "Date"
 msgstr "วันที่"
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:97
+#: basxconnect/core/layouts/editperson/common/history_tab.py:84
 msgid "Time"
-msgstr "เวลา"
+msgstr ""
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:103
+#: basxconnect/core/layouts/editperson/common/history_tab.py:90
 msgid "User"
 msgstr "ชื่อผู้ใช้งาน"
 
-#: basxconnect/core/layouts/editperson/common/history_tab.py:107
-#: basxconnect/core/layouts/editperson/common/history_tab.py:139
+#: basxconnect/core/layouts/editperson/common/history_tab.py:94
+#: basxconnect/core/layouts/editperson/common/history_tab.py:126
+#, fuzzy
+#| msgid "Change"
 msgid "Changes"
 msgstr "เปลี่ยน"
 
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:22
 #: basxconnect/core/layouts/settings_layout.py:16
 #: basxconnect/core/models/relationships.py:55
-#: basxconnect/core/views/menu_views.py:59
+#: basxconnect/core/views/menu_views.py:75
 msgid "Relationships"
 msgstr "ความสัมพันธ์"
 
 #: basxconnect/core/layouts/editperson/common/relationships_tab.py:28
 msgid "Relationships to person"
 msgstr "สถานะความสัมพันธ์ที่เกี่ยวข้องเป็น"
 
@@ -274,29 +272,31 @@
 msgstr "เปลี่ยน"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:36
 msgid "Created"
 msgstr "สร้าง"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:44
+#, fuzzy
+#| msgid "Base data"
 msgid "Meta data"
-msgstr "โครงสร้างข้อมูลข้อมูล"
+msgstr "ฐานข้อมูล"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:52
-#: basxconnect/core/views/person/person_browse_views.py:114
-#: basxconnect/core/views/person/person_browse_views.py:244
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_browse_views.py:115
+#: basxconnect/core/views/person/person_browse_views.py:245
+#: basxconnect/core/views/person/person_details_views.py:161
 msgid "Inactive"
 msgstr "ไม่ใช้งาน"
 
 #: basxconnect/core/layouts/editperson/common/utils.py:52
 #: basxconnect/core/models/persons.py:58
-#: basxconnect/core/views/person/person_browse_views.py:113
-#: basxconnect/core/views/person/person_browse_views.py:244
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_browse_views.py:114
+#: basxconnect/core/views/person/person_browse_views.py:245
+#: basxconnect/core/views/person/person_details_views.py:161
 msgid "Active"
 msgstr "ใช้งาน"
 
 #: basxconnect/core/layouts/editperson/legalperson/base_data_tab.py:20
 #: basxconnect/core/layouts/editperson/personassociation/base_data_tab.py:18
 msgid "Base data"
 msgstr "ฐานข้อมูล"
@@ -304,143 +304,146 @@
 #: basxconnect/core/layouts/editperson/legalperson/base_data_tab.py:25
 #: basxconnect/core/layouts/editperson/personassociation/base_data_tab.py:22
 msgid "Base Data"
 msgstr "ฐานข้อมูล"
 
 #: basxconnect/core/layouts/editperson/legalperson/mailing.py:27
 #: basxconnect/core/layouts/editperson/naturalperson/mailing.py:27
-#: basxconnect/core/layouts/editperson/personassociation/mailing.py:20
+#: basxconnect/core/layouts/editperson/personassociation/mailing.py:21
 msgid "Mailings"
 msgstr "การส่งจดหมาย"
 
 #: basxconnect/core/layouts/editperson/legalperson/mailing.py:31
 #: basxconnect/core/layouts/editperson/naturalperson/mailing.py:31
 #: basxconnect/core/views/person/person_modals_views.py:28
+#: basxconnect/core/views/settings_views.py:29
 msgid "Settings"
 msgstr "ตั้งค่า"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:20
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:21
+#, fuzzy
+#| msgid "Personal Data"
 msgid "Personal data"
 msgstr "ข้อมูลบุคคล"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:69
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:51
 msgid "Yes"
 msgstr "ใช่"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:69
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:51
 msgid "No"
 msgstr "ไม่ใช่"
 
-#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:79
+#: basxconnect/core/layouts/editperson/naturalperson/base_data_tab.py:60
 msgid "Personal Data"
 msgstr "ข้อมูลบุคคล"
 
 #: basxconnect/core/migrations/0015_rename_category_to_tag.py:13
 msgid "Tag"
 msgstr "แท็ก"
 
 #: basxconnect/core/migrations/0015_rename_category_to_tag.py:21
 msgid "Category"
 msgstr "หมวดหมู่"
 
-#: basxconnect/core/models/addresses.py:20
-#: basxconnect/core/models/persons.py:243
+#: basxconnect/core/models/addresses.py:18
+#: basxconnect/core/models/persons.py:241
 msgid "Person"
 msgstr "บุคคล"
 
-#: basxconnect/core/models/addresses.py:32
-#: basxconnect/core/models/addresses.py:57
-#: basxconnect/core/views/person/person_browse_views.py:157
-#: basxconnect/core/wizards/add_person.py:69
+#: basxconnect/core/models/addresses.py:30
+#: basxconnect/core/models/addresses.py:54
+#: basxconnect/core/views/person/person_browse_views.py:158
+#: basxconnect/core/wizards/add_person.py:67
 msgid "Email"
 msgstr "อีเมล์"
 
-#: basxconnect/core/models/addresses.py:40
-#: basxconnect/core/models/addresses.py:76
-#: basxconnect/core/models/addresses.py:96
-#: basxconnect/core/models/addresses.py:118
-#: basxconnect/core/models/addresses.py:144
-#: basxconnect/core/models/persons.py:359
-#: basxconnect/core/models/persons.py:383
+#: basxconnect/core/models/addresses.py:39
+#: basxconnect/core/models/addresses.py:74
+#: basxconnect/core/models/addresses.py:93
+#: basxconnect/core/models/addresses.py:114
+#: basxconnect/core/models/addresses.py:139
+#: basxconnect/core/models/persons.py:350
+#: basxconnect/core/models/persons.py:374
 #: basxconnect/core/models/relationships.py:36
-#: basxconnect/core/wizards/add_person.py:280
+#: basxconnect/core/wizards/add_person.py:273
 msgid "Type"
 msgstr "ประเภท"
 
-#: basxconnect/core/models/addresses.py:63
+#: basxconnect/core/models/addresses.py:60
 msgid "Email address"
 msgstr "ที่อยู่อีเมล์"
 
-#: basxconnect/core/models/addresses.py:64
+#: basxconnect/core/models/addresses.py:61
 msgid "Email addresses"
 msgstr "ที่อยู่อีเมล์"
 
-#: basxconnect/core/models/addresses.py:68
+#: basxconnect/core/models/addresses.py:65
 msgid "Url"
 msgstr "URL เว็บไซต์ / เฟซบุคเพจ"
 
-#: basxconnect/core/models/addresses.py:84
+#: basxconnect/core/models/addresses.py:80
 msgid "Web address"
 msgstr "เว็บไซต์"
 
-#: basxconnect/core/models/addresses.py:85
+#: basxconnect/core/models/addresses.py:81
 msgid "Web addresses"
 msgstr "เว็บไซต์"
 
-#: basxconnect/core/models/addresses.py:89
-#: basxconnect/core/models/addresses.py:111
+#: basxconnect/core/models/addresses.py:85
+#: basxconnect/core/models/addresses.py:106
 msgid "Number"
 msgstr "ลำดับที่"
 
-#: basxconnect/core/models/addresses.py:106
+#: basxconnect/core/models/addresses.py:101
 msgid "Phone number"
 msgstr "เบอร์โทรศัพท์"
 
-#: basxconnect/core/models/addresses.py:107
+#: basxconnect/core/models/addresses.py:102
 msgid "Phone numbers"
 msgstr "เบอร์โทรศัพท์"
 
-#: basxconnect/core/models/addresses.py:128
+#: basxconnect/core/models/addresses.py:122
 msgid "Fax number"
 msgstr "แฟกซ์"
 
-#: basxconnect/core/models/addresses.py:129
+#: basxconnect/core/models/addresses.py:123
 msgid "Fax numbers"
 msgstr "แฟกซ์"
 
-#: basxconnect/core/models/addresses.py:133
+#: basxconnect/core/models/addresses.py:127
 msgid "Country"
 msgstr "ประเทศ"
 
-#: basxconnect/core/models/addresses.py:134
-#: basxconnect/core/wizards/add_person.py:48
+#: basxconnect/core/models/addresses.py:128
+#: basxconnect/core/wizards/add_person.py:46
 msgid "Address"
 msgstr "ที่อยู่"
 
-#: basxconnect/core/models/addresses.py:135
+#: basxconnect/core/models/addresses.py:129
 msgid "Post Code"
 msgstr "รหัสไปรษณีย์"
 
-#: basxconnect/core/models/addresses.py:136
+#: basxconnect/core/models/addresses.py:130
 msgid "City"
 msgstr "จังหวัด"
 
-#: basxconnect/core/models/addresses.py:148
+#: basxconnect/core/models/addresses.py:140
 msgid "Valid from"
 msgstr "ใช้ได้ตั้งแต่"
 
-#: basxconnect/core/models/addresses.py:149
+#: basxconnect/core/models/addresses.py:141
 msgid "Valid until"
 msgstr "ใช้ได้จนถึง"
 
-#: basxconnect/core/models/addresses.py:164
+#: basxconnect/core/models/addresses.py:153
 msgid "Postal address"
 msgstr "ไปรษณีย์พื้นที่"
 
-#: basxconnect/core/models/addresses.py:165
+#: basxconnect/core/models/addresses.py:154
 msgid "Postal addresses"
 msgstr "ไปรษณีย์พื้นที่"
 
 #: basxconnect/core/models/persons.py:43
 msgid "Deleted"
 msgstr "ลบ"
 
@@ -469,24 +472,26 @@
 msgstr "ที่อยู่สำหรับติดต่อ"
 
 #: basxconnect/core/models/persons.py:95
 msgid "Primary email address"
 msgstr "อีเมล์สำหรับติดต่อ"
 
 #: basxconnect/core/models/persons.py:108
+#, fuzzy
+#| msgid "Phone number"
 msgid "Primary phonenumber"
-msgstr "เบอร์โทรศัพท์ติดต่อ"
+msgstr "เบอร์โทรศัพท์"
 
 #: basxconnect/core/models/persons.py:115
 msgid "Remarks"
 msgstr "หมายเหตุ"
 
 #: basxconnect/core/models/persons.py:132
-#: basxconnect/core/models/persons.py:316
-#: basxconnect/core/views/person/person_browse_views.py:371
+#: basxconnect/core/models/persons.py:307
+#: basxconnect/core/views/person/person_browse_views.py:372
 msgid "Person Type"
 msgstr "ประเภทของบุคคล"
 
 #: basxconnect/core/models/persons.py:142
 msgid "Main Type"
 msgstr "ประเภท"
 
@@ -494,102 +499,100 @@
 msgid "active"
 msgstr "ใช้งาน"
 
 #: basxconnect/core/models/persons.py:149
 msgid "inactive"
 msgstr "ไม่ใช้งาน"
 
-#: basxconnect/core/models/persons.py:248
+#: basxconnect/core/models/persons.py:246
 msgid "First Name"
 msgstr "ชื่อ"
 
-#: basxconnect/core/models/persons.py:249
+#: basxconnect/core/models/persons.py:247
 msgid "Middle Name"
 msgstr "ชื่อกลาง"
 
-#: basxconnect/core/models/persons.py:250
+#: basxconnect/core/models/persons.py:248
 msgid "Last Name"
 msgstr "นามสกุล"
 
-#: basxconnect/core/models/persons.py:251
-msgid "Maiden Name"
-msgstr "นามสกุลเดิม"
-
-#: basxconnect/core/models/persons.py:254
+#: basxconnect/core/models/persons.py:250
 msgid "Autogenerate Display Name"
 msgstr "สร้างชื่อที่แสดงโดยอัตโนมัติ"
 
-#: basxconnect/core/models/persons.py:263
+#: basxconnect/core/models/persons.py:260
 msgid "Title"
 msgstr "เรื่อง"
 
-#: basxconnect/core/models/persons.py:274
+#: basxconnect/core/models/persons.py:269
 msgid "Salutation"
 msgstr "คำนำหน้านาม"
 
-#: basxconnect/core/models/persons.py:285
+#: basxconnect/core/models/persons.py:279
 msgid "Form of address"
 msgstr "ประเภทที่อยู่อาศัย"
 
-#: basxconnect/core/models/persons.py:290
+#: basxconnect/core/models/persons.py:282
 msgid "Profession"
 msgstr "อาชีพ"
 
-#: basxconnect/core/models/persons.py:294
+#: basxconnect/core/models/persons.py:286
 msgid "Date of Birth"
 msgstr "วันเดือนปีเกิด"
 
-#: basxconnect/core/models/persons.py:295
+#: basxconnect/core/models/persons.py:287
+#, fuzzy
+#| msgid "Date of Birth"
 msgid "Place of Birth"
-msgstr "สถานที่เกิด"
+msgstr "วันเดือนปีเกิด"
 
-#: basxconnect/core/models/persons.py:296
+#: basxconnect/core/models/persons.py:288
 msgid "Deceased"
 msgstr "เสียชีวิต"
 
-#: basxconnect/core/models/persons.py:297
+#: basxconnect/core/models/persons.py:289
 msgid "Deceased Date"
 msgstr "วันที่เสียชีวิต"
 
-#: basxconnect/core/models/persons.py:305
+#: basxconnect/core/models/persons.py:298
 msgid "Gender"
 msgstr "เพศ"
 
-#: basxconnect/core/models/persons.py:329
+#: basxconnect/core/models/persons.py:320
 msgid "Age"
 msgstr "อายุ"
 
-#: basxconnect/core/models/persons.py:346
-#: basxconnect/core/views/person/person_browse_views.py:210
+#: basxconnect/core/models/persons.py:337
+#: basxconnect/core/views/person/person_browse_views.py:211
 msgid "Natural Person"
 msgstr "บุคคลธรรมดา"
 
-#: basxconnect/core/models/persons.py:347
+#: basxconnect/core/models/persons.py:338
 msgid "Natural Persons"
 msgstr "บุคคลธรรมดา"
 
-#: basxconnect/core/models/persons.py:351
+#: basxconnect/core/models/persons.py:342
 msgid "Addition name"
 msgstr "ชื่อองค์กร"
 
-#: basxconnect/core/models/persons.py:371
-#: basxconnect/core/views/person/person_browse_views.py:211
+#: basxconnect/core/models/persons.py:362
+#: basxconnect/core/views/person/person_browse_views.py:212
 msgid "Legal Person"
 msgstr "นิติบุคคล"
 
-#: basxconnect/core/models/persons.py:372
+#: basxconnect/core/models/persons.py:363
 msgid "Legal Persons"
 msgstr "นิติบุคคล"
 
-#: basxconnect/core/models/persons.py:395
-#: basxconnect/core/views/person/person_browse_views.py:213
+#: basxconnect/core/models/persons.py:386
+#: basxconnect/core/views/person/person_browse_views.py:214
 msgid "Person Association"
 msgstr "กลุ่มบุคคล"
 
-#: basxconnect/core/models/persons.py:396
+#: basxconnect/core/models/persons.py:387
 msgid "Person Associations"
 msgstr "กลุ่มบุคคล"
 
 #: basxconnect/core/models/relationships.py:9
 msgid "Name for relationship type"
 msgstr "ประเภทความสัมพันธ์"
 
@@ -621,127 +624,118 @@
 msgid "Ends on"
 msgstr "สิ้นสุดวันที่"
 
 #: basxconnect/core/models/relationships.py:54
 msgid "Relationship"
 msgstr "ความสัมพันธ์"
 
-#: basxconnect/core/models/utils.py:19 basxconnect/core/models/utils.py:75
-msgid "Terms"
-msgstr "ข้อกำหนด"
-
-#: basxconnect/core/models/utils.py:26
-#: basxconnect/core/views/person/person_browse_views.py:129
+#: basxconnect/core/models/utils.py:13
+#: basxconnect/core/views/person/person_browse_views.py:130
 msgid "Name"
 msgstr "ชื่อ"
 
-#: basxconnect/core/models/utils.py:28 basxconnect/core/models/utils.py:56
+#: basxconnect/core/models/utils.py:15 basxconnect/core/models/utils.py:33
 msgid "Slug"
 msgstr "Slug"
 
-#: basxconnect/core/models/utils.py:30
+#: basxconnect/core/models/utils.py:17
 msgid "slug is human-readable, to make referencing easier"
-msgstr "slugสามารถอ่านได้โดยมนุษย์ เพื่อให้การอ้างอิงง่ายขึ้น"
+msgstr "Slug คือสิ่งที่ทำให้การค้นหา ระบุตัวตนง่ายขึ้น"
 
-#: basxconnect/core/models/utils.py:40 basxconnect/core/models/utils.py:54
+#: basxconnect/core/models/utils.py:25 basxconnect/core/models/utils.py:31
 msgid "Vocabulary"
 msgstr "คำศัพท์"
 
-#: basxconnect/core/models/utils.py:41
+#: basxconnect/core/models/utils.py:26
 msgid "Vocabularies"
 msgstr "คำศัพท์"
 
-#: basxconnect/core/models/utils.py:55 basxconnect/core/models/utils.py:74
+#: basxconnect/core/models/utils.py:32 basxconnect/core/models/utils.py:44
 msgid "Term"
-msgstr "ข้อกำหนด"
-
-#: basxconnect/core/models/utils.py:58
-msgid "Disabled"
-msgstr "ไม่มีสิทธิ์"
-
-#: basxconnect/core/models/utils.py:60
-msgid "Do not allow this term to be selected"
-msgstr "ไม่อนุญาตให้เลือกคำนี้"
+msgstr "หมวดหมู่"
 
-#: basxconnect/core/views/menu_views.py:46
-msgid "Taxonomy"
-msgstr "อนุกรมวิธาน"
+#: basxconnect/core/models/utils.py:45
+msgid "Terms"
+msgstr "หมวดหมู่"
 
-#: basxconnect/core/views/person/person_browse_views.py:174
+#: basxconnect/core/views/person/person_browse_views.py:175
+#, fuzzy
+#| msgid "Add %s"
 msgid "Add tag"
-msgstr "เพิ่ม แท็ก"
+msgstr "เพิ่ม %s"
 
-#: basxconnect/core/views/person/person_browse_views.py:180
+#: basxconnect/core/views/person/person_browse_views.py:181
 msgid "Remove tag"
-msgstr "ลบแท็ก"
+msgstr ""
 
-#: basxconnect/core/views/person/person_browse_views.py:198
+#: basxconnect/core/views/person/person_browse_views.py:199
 msgid "Excel"
 msgstr "Excel"
 
-#: basxconnect/core/views/person/person_browse_views.py:248
+#: basxconnect/core/views/person/person_browse_views.py:249
 msgid "Trash"
 msgstr "ลบทิ้ง"
 
-#: basxconnect/core/views/person/person_browse_views.py:445
-#: basxconnect/core/views/person/person_details_views.py:214
+#: basxconnect/core/views/person/person_browse_views.py:446
+#: basxconnect/core/views/person/person_details_views.py:233
 msgid "Cancel"
 msgstr "ยกเลิก"
 
-#: basxconnect/core/views/person/person_browse_views.py:451
+#: basxconnect/core/views/person/person_browse_views.py:452
 msgid "Reset"
-msgstr "รีเซ็ต"
+msgstr "ตั้งค่าใหม่"
 
-#: basxconnect/core/views/person/person_browse_views.py:458
+#: basxconnect/core/views/person/person_browse_views.py:459
 msgctxt "apply filter"
 msgid "Filter"
-msgstr "กรอง"
+msgstr "เลือก"
 
-#: basxconnect/core/views/person/person_details_views.py:143
+#: basxconnect/core/views/person/person_details_views.py:161
 #, python-format
 msgid "%s is %s"
 msgstr "%s คือ %s"
 
-#: basxconnect/core/views/person/person_details_views.py:159
-#, python-format
+#: basxconnect/core/views/person/person_details_views.py:178
+#, fuzzy, python-format
+#| msgid "Delete linked email subscriptions as well"
 msgid "Delete linked %s subscription as well"
-msgstr "ลบการสมัครสมาชิก %s ที่แบบต่อเนื่อง"
+msgstr "ลบการอีเมลที่เชื่อมโยงด้วยการสมัครสมาชิก"
 
-#: basxconnect/core/views/person/person_details_views.py:205
+#: basxconnect/core/views/person/person_details_views.py:224
 #, python-format
 msgid "Delete email %s"
 msgstr "ลบอีเมล์%s"
 
-#: basxconnect/core/views/person/person_details_views.py:220
+#: basxconnect/core/views/person/person_details_views.py:239
 msgid "Confirm"
 msgstr "ยืนยัน"
 
 #: basxconnect/core/views/person/person_modals_views.py:32
 msgid "Edit mailing settings"
 msgstr "แก้ไขการตั้งค่าการส่งจดหมาย"
 
-#: basxconnect/core/views/person/person_modals_views.py:153
+#: basxconnect/core/views/person/person_modals_views.py:149
 msgid "Use as primary postal address"
 msgstr "ใช้เป็นที่อยู่หลักสำหรับติดต่อ"
 
-#: basxconnect/core/views/person/person_modals_views.py:216
+#: basxconnect/core/views/person/person_modals_views.py:213
 msgid "Use as primary email address"
 msgstr "ใช้เป็นที่อยู่หลักสำหรับติดต่อ"
 
-#: basxconnect/core/views/person/person_modals_views.py:224
+#: basxconnect/core/views/person/person_modals_views.py:221
 #, python-format
 msgid "Propagate change of email address to %s"
 msgstr "เผยแพร่การเปลี่ยนแปลงที่อยู่อีเมลไปยัง %s"
 
-#: basxconnect/core/views/person/person_modals_views.py:253
+#: basxconnect/core/views/person/person_modals_views.py:250
 msgid "Edit Email"
 msgstr "แก้ไขอีเมล์"
 
 #: basxconnect/core/views/person/search_person_view.py:21
-#: basxconnect/core/wizards/add_person.py:151
+#: basxconnect/core/wizards/add_person.py:147
 msgid "Search person"
 msgstr "ค้นหาบุคคล"
 
 #: basxconnect/core/views/person/search_person_view.py:62
 msgid "No results"
 msgstr "ไม่มีผลลัพท์"
 
@@ -754,132 +748,124 @@
 msgid "Edit Relationship"
 msgstr "แก้ไขความสัมพันธ์"
 
 #: basxconnect/core/views/relationship_views.py:61
 msgid "Add Relationship"
 msgstr "เพิ่มความสัมพันธ์"
 
+#: basxconnect/core/views/settings_views.py:31
+msgid "Information about our organization"
+msgstr "ข้อมูลเกี่ยวกับองค์กร"
+
 #: basxconnect/core/views/tag_views.py:67
-#, python-format
+#, fuzzy, python-format
+#| msgid "Add relationship to person"
 msgid "Add tag to %(count)d person"
 msgid_plural "Add tag to %(count)d persons"
-msgstr[0] "เพิ่มแท็กเพื่อ%(count)dบุคคล"
+msgstr[0] "เพิ่มสถานะความสัมพันธ์ของตนเองกับบุคคลอื่น"
 
 #: basxconnect/core/views/tag_views.py:73
 #, python-format
 msgid "Remove tag from %(count)d person"
 msgid_plural "Remove tag from %(count)d persons"
-msgstr[0] "ลบแท็กจาก %(count)dบุคคล"
+msgstr[0] ""
 
 #: basxconnect/core/views/tag_views.py:90
 #: basxconnect/core/views/tag_views.py:112
 msgid "Create new tag"
-msgstr "สร้างแท็กใหม่"
+msgstr ""
 
 #: basxconnect/core/views/tag_views.py:121
 msgid "Submit"
-msgstr "ยืนยัน"
+msgstr ""
 
 #: basxconnect/core/views/vocabulary.py:14
+#, fuzzy
+#| msgid "Vocabulary"
 msgid "Terms of vocabulary"
-msgstr "ศัพท์บัญญัติ"
+msgstr "คำศัพท์"
 
-#: basxconnect/core/wizards/add_person.py:105
+#: basxconnect/core/wizards/add_person.py:101
 msgid "Back"
 msgstr "กลับ"
 
-#: basxconnect/core/wizards/add_person.py:116
+#: basxconnect/core/wizards/add_person.py:112
 msgid "Complete"
 msgstr "เรียบร้อย"
 
-#: basxconnect/core/wizards/add_person.py:119
+#: basxconnect/core/wizards/add_person.py:115
 msgid "Continue"
 msgstr "ต่อไป"
 
-#: basxconnect/core/wizards/add_person.py:131
+#: basxconnect/core/wizards/add_person.py:127
 msgid "Check for existing people before continuing"
 msgstr "ตรวจสอบข้อมูลก่อนดำเนินการต่อ"
 
-#: basxconnect/core/wizards/add_person.py:139
+#: basxconnect/core/wizards/add_person.py:135
 msgid "Start typing to search for a person..."
 msgstr "พิมพ์เพื่อค้นหาบุคคล"
 
-#: basxconnect/core/wizards/add_person.py:155
+#: basxconnect/core/wizards/add_person.py:151
 msgid ""
 "Before a new person can be added it must be confirmed that the person does "
 "not exists yet."
 msgstr "ก่อนที่จะเพิ่มบุคคลใหม่จะต้องได้รับการยืนยันว่าบุคคลนั้นยังไม่ปรากฏ"
 
-#: basxconnect/core/wizards/add_person.py:171
+#: basxconnect/core/wizards/add_person.py:167
 msgid "Type of person"
 msgstr "ประเภทบุคคล"
 
-#: basxconnect/core/wizards/add_person.py:177
+#: basxconnect/core/wizards/add_person.py:173
 msgid "Choose person main type"
 msgstr "เลือกประเภทบุคคลหลัก"
 
-#: basxconnect/core/wizards/add_person.py:180
+#: basxconnect/core/wizards/add_person.py:176
 msgid "Please choose what type of person you want to add:"
 msgstr "โปรดเลือกประเภทของบุคคลที่คุณต้องการเพิ่ม:"
 
-#: basxconnect/core/wizards/add_person.py:195
+#: basxconnect/core/wizards/add_person.py:191
 msgid "Subtype of person"
 msgstr "ประเภทบุคคลรายย่อย"
 
-#: basxconnect/core/wizards/add_person.py:211
+#: basxconnect/core/wizards/add_person.py:207
 msgid "Choose person type"
 msgstr "เลือกประเภทบุคคล"
 
-#: basxconnect/core/wizards/add_person.py:219
+#: basxconnect/core/wizards/add_person.py:215
 msgid "Add person"
 msgstr "เพิ่มบุคคล"
 
-#: basxconnect/core/wizards/add_person.py:227
+#: basxconnect/core/wizards/add_person.py:223
 msgid "Finish"
-msgstr "เสร็จสิ้น"
+msgstr "เสร็จเรียบร้อย"
 
-#: basxconnect/core/wizards/add_person.py:279
+#: basxconnect/core/wizards/add_person.py:272
 msgid "Search"
 msgstr "ค้นหา"
 
-#: basxconnect/core/wizards/add_person.py:281
+#: basxconnect/core/wizards/add_person.py:274
 msgid "Subtype"
 msgstr "ประเภทย่อย"
 
-#: basxconnect/core/wizards/add_person.py:282
+#: basxconnect/core/wizards/add_person.py:275
 msgid "Information"
 msgstr "ข้อมูลเบื้องต้น"
 
-#: basxconnect/core/wizards/add_person.py:283
+#: basxconnect/core/wizards/add_person.py:276
 msgid "Confirmation"
 msgstr "ยืนยัน"
 
-#: basxconnect/core/wizards/add_person.py:307
+#: basxconnect/core/wizards/add_person.py:300
 msgid "Add new person"
 msgstr "เพิ่มบุคคลใหม่"
 
-#: basxconnect/core/wizards/add_person.py:378
+#: basxconnect/core/wizards/add_person.py:371
 msgid "Review and confirm the entered information"
 msgstr "ตรวจสอบและยืนยันข้อมูล"
 
-#~ msgid "Sender letterhead"
-#~ msgstr "หัวจดหมาย"
-
-#~ msgid "Logo"
-#~ msgstr "โลโก้"
-
-#~ msgid "Organization Name"
-#~ msgstr "ชื่อองค์กร"
-
-#~ msgid "Information about our organization"
-#~ msgstr "ข้อมูลเกี่ยวกับองค์กร"
-
-#~ msgid "Documents"
-#~ msgstr "เอกสาร"
-
 #~ msgid "Administration"
 #~ msgstr "ผู้ดูแลระบบ"
 
 #~ msgid "System Information"
 #~ msgstr "ข้อมูลระบบ"
 
 #~ msgid "Maintenance"
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0001_initial.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import simple_history.models
 from basxbread.contrib import languages
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = [
         ("contenttypes", "0002_remove_content_type_name"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0003_auto_20210309_2221.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0003_auto_20210309_2221.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.1.5 on 2021-03-09 15:21
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0002_auto_20210309_1750"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicallegalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0004_auto_20210311_1851.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0004_auto_20210311_1851.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.1.5 on 2021-03-11 11:51
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0003_auto_20210309_2221"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="historicalnaturalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0005_auto_20210311_1851.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0005_auto_20210311_1851.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.1.5 on 2021-03-11 11:51
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0004_auto_20210311_1851"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicalnaturalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0006_auto_20210312_0016.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0006_auto_20210312_0016.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.1.5 on 2021-03-11 17:16
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0005_auto_20210311_1851"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicalnaturalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0007_auto_20210312_0054.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0007_auto_20210312_0054.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.1.5 on 2021-03-11 17:54
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0006_auto_20210312_0016"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicallegalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0008_auto_20210323_1456.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0008_auto_20210323_1456.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.1.7 on 2021-03-23 07:56
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0007_auto_20210312_0054"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicallegalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0009_auto_20210522_1817.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0009_auto_20210522_1817.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.1.7 on 2021-05-22 11:17
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0008_auto_20210323_1456"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="relationship",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0010_auto_20210523_1140.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0010_auto_20210523_1140.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.1.7 on 2021-05-23 04:40
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0009_auto_20210522_1817"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="email",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0011_auto_20210726_2047.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0011_auto_20210726_2047.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.db import migrations, models
 
 import basxconnect.core.models.persons
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0010_auto_20210523_1140"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicallegalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0012_auto_20210928_1158.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0012_auto_20210928_1158.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.5 on 2021-09-28 04:58
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0011_auto_20210726_2047"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicalnaturalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0013_auto_20210928_1445.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0013_auto_20210928_1445.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.5 on 2021-09-28 07:45
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0012_auto_20210928_1158"),
     ]
 
     operations = [
         migrations.RenameModel(
             old_name="Category",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0014_auto_20210928_1512.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0014_auto_20210928_1512.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.5 on 2021-09-28 08:12
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0013_auto_20210928_1445"),
     ]
 
     operations = [
         migrations.RenameField(
             model_name="term",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0015_rename_category_to_tag.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0015_rename_category_to_tag.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0016_auto_20210928_1534.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0016_auto_20210928_1534.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0018_term_slug.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0018_term_slug.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0020_auto_20211005_1630.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0020_auto_20211005_1630.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.4 on 2021-10-05 14:30
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0019_alter_term_slug"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="postal",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0021_auto_20211007_0932.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0021_auto_20211007_0932.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.4 on 2021-10-07 07:32
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0020_auto_20211005_1630"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="postal",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0022_auto_20211018_1644.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0022_auto_20211018_1644.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.5 on 2021-10-18 09:44
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0021_auto_20211007_0932"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="email",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0023_auto_20211030_0955.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0023_auto_20211030_0955.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.5 on 2021-10-30 02:55
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0022_auto_20211018_1644"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="email",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0026_auto_20211216_0946.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0026_auto_20211216_0946.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0027_auto_20211223_1948.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0027_auto_20211223_1948.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.10 on 2021-12-23 12:48
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0026_auto_20211216_0946"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="historicallegalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0029_auto_20220429_1138.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0029_auto_20220429_1138.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.13 on 2022-04-29 04:38
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0028_auto_20220404_1058"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicallegalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0030_auto_20220602_1434.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0030_auto_20220602_1434.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.13 on 2022-06-02 07:34
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0029_auto_20220429_1138"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="historicalnaturalperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0031_alter_email_person_alter_email_type_alter_fax_person_and_more.py` & `basxconnect-0.4.7/basxconnect/core/migrations/0031_alter_email_person_alter_email_type_alter_fax_person_and_more.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 4.0.5 on 2022-06-02 10:03
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0030_auto_20220602_1434"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="email",
```

### Comparing `basxconnect-0.4.61/basxconnect/core/migrations/0034_term_disabled.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0021_auto_20220106_0917.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# Generated by Django 4.0.6 on 2022-11-25 08:13
+# Generated by Django 3.2.4 on 2022-01-06 08:17
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
-        ("core", "0033_historicalnaturalperson_maiden_name_and_more"),
+        ("mailer_integration", "0020_subscription_deleted"),
     ]
 
     operations = [
+        migrations.RemoveField(
+            model_name="subscription",
+            name="deleted",
+        ),
         migrations.AddField(
-            model_name="term",
-            name="disabled",
+            model_name="subscription",
+            name="active",
             field=models.BooleanField(
-                default=False,
-                help_text="Do not allow this term to be selected",
-                verbose_name="Disabled",
+                blank=True, default=True, editable=False, verbose_name="Deleted"
             ),
         ),
     ]
```

### Comparing `basxconnect-0.4.61/basxconnect/core/models/addresses.py` & `basxconnect-0.4.7/basxconnect/core/models/addresses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import htmlgenerator as hg
 from basxbread.layout import button
-from django import forms
 from django.db import models
-from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 from django_countries.fields import CountryField
 from phonenumber_field.modelfields import PhoneNumberField
 
 from .persons import Person
 from .utils import Term
 
@@ -33,17 +31,16 @@
     type = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         related_name="type_%(app_label)s_%(class)s_list",
         limit_choices_to={"vocabulary__slug": "emailtype"},
-        verbose_name=_("Type"),
     )
-    type.formfield_kwargs = {"widget": forms.RadioSelect()}
+    type.verbose_name = _("Type")
 
     def asbutton(self):
         return hg.DIV(
             hg.SPAN(self.email, style="margin-right: 0.25rem"),
             hg.SPAN(style="flex-grow: 1"),
             button.Button(
                 icon="email",
@@ -69,17 +66,16 @@
     type = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         related_name="type_%(app_label)s_%(class)s_list",
         limit_choices_to={"vocabulary__slug": "urltype"},
-        verbose_name=_("Type"),
     )
-    type.formfield_kwargs = {"widget": forms.RadioSelect()}
+    type.verbose_name = _("Type")
 
     def __str__(self):
         return str(self.url)
 
     class Meta:
         verbose_name = _("Web address")
         verbose_name_plural = _("Web addresses")
@@ -89,17 +85,16 @@
     number = PhoneNumberField(_("Number"))
     type = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         limit_choices_to={"vocabulary__slug": "phonetype"},
-        verbose_name=_("Type"),
     )
-    type.formfield_kwargs = {"widget": forms.RadioSelect()}
+    type.verbose_name = _("Type")
 
     def __str__(self):
         if self.type:
             return f"{self.number} ({self.type})"
         return str(self.number)
 
     class Meta:
@@ -111,17 +106,16 @@
     number = PhoneNumberField(_("Number"))
     type = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         limit_choices_to={"vocabulary__slug": "phonetype"},
-        verbose_name=_("Type"),
     )
-    type.formfield_kwargs = {"widget": forms.RadioSelect()}
+    type.verbose_name = _("Type")
 
     def __str__(self):
         if self.type:
             return f"{self.number} ({self.type})"
         return str(self.number)
 
     class Meta:
@@ -137,24 +131,19 @@
     type = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         related_name="type_%(app_label)s_%(class)s_list",
         limit_choices_to={"vocabulary__slug": "addresstype"},
-        verbose_name=_("Type"),
     )
-    type.formfield_kwargs = {"widget": forms.RadioSelect()}
-
+    type.verbose_name = _("Type")
     valid_from = models.DateField(_("Valid from"), blank=True, null=True)
     valid_until = models.DateField(_("Valid until"), blank=True, null=True)
 
-    def is_active(self):
-        return self.valid_from <= now.date() <= self.valid_until
-
     def __str__(self):
         ret = [self.address]
         if self.postcode:
             ret.append(f"{self.postcode} {self.city}")
         else:
             ret.append(self.city)
         ret.append(self.country.name)
```

### Comparing `basxconnect-0.4.61/basxconnect/core/models/persons.py` & `basxconnect-0.4.7/basxconnect/core/models/persons.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import datetime
 import random
 
 from basxbread import layout
 from basxbread.contrib.languages.fields import LanguageField
 from basxbread.utils import get_concrete_instance
 from basxbread.utils.inheritancemanager import InheritanceManager
-from django import forms
 from django.contrib.contenttypes.fields import GenericRelation
 from django.db import models
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 from dynamic_preferences.registries import global_preferences_registry
 from simple_history.models import HistoricalRecords
 
@@ -76,40 +76,44 @@
         "core.Postal",
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
         related_name="primary_address_for",
     )
     primary_postal_address.verbose_name = _("Primary postal address")
-    primary_postal_address.lazy_choices = lambda field, request, instance: (
-        instance.core_postal_list.all()
+    primary_postal_address.lazy_choices = (
+        lambda field, request, instance: instance.core_postal_list.all()
         if hasattr(instance, "core_postal_list")
         else None
     )
     primary_email_address = models.ForeignKey(
         "core.Email",
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
         related_name="primary_email_for",
     )
     primary_email_address.verbose_name = _("Primary email address")
-    primary_email_address.lazy_choices = lambda field, request, instance: (
-        instance.core_email_list.all() if hasattr(instance, "core_email_list") else None
+    primary_email_address.lazy_choices = (
+        lambda field, request, instance: instance.core_email_list.all()
+        if hasattr(instance, "core_email_list")
+        else None
     )
     primary_phonenumber = models.ForeignKey(
         "core.Phone",
         null=True,
         blank=True,
         on_delete=models.SET_NULL,
         related_name="primary_phone_for",
     )
     primary_phonenumber.verbose_name = _("Primary phonenumber")
-    primary_phonenumber.lazy_choices = lambda field, request, instance: (
-        instance.core_phone_list.all() if hasattr(instance, "core_phone_list") else None
+    primary_phonenumber.lazy_choices = (
+        lambda field, request, instance: instance.core_phone_list.all()
+        if hasattr(instance, "core_phone_list")
+        else None
     )
 
     remarks = models.TextField(_("Remarks"), blank=True)
     notes = GenericRelation(Note)
     history = HistoricalRecords(inherit=True)
     _maintype = models.CharField(  # only used internally for filtering or sorting
         max_length=32,
@@ -156,55 +160,53 @@
         # to do the same thing again after a call to super.save
         # and then save again
         # the random-things is a bit ugly but if we want to enforce uniqueness
         # on the database level we have to use this one during creation
 
         if not self._maintype:
             self._maintype = "person"
-        if self.pk is not None:
-            if hasattr(self, "core_postal_list"):
-                active_postals = [
-                    postal
-                    for postal in self.core_postal_list.all()
-                    if postal.valid_until is None
-                    or postal.valid_until >= timezone.now().date()
-                ]
-                if len(active_postals) == 0:
-                    self.primary_postal_address = None
-                elif (
-                    len(active_postals) == 1
-                    or self.primary_postal_address is None
-                    or (
-                        self.primary_postal_address.valid_until
-                        and self.primary_postal_address.valid_until
-                        < timezone.now().date()
-                    )
-                ):
-                    self.primary_postal_address = active_postals[0]
-
-            else:
+        if hasattr(self, "core_postal_list"):
+            active_postals = [
+                postal
+                for postal in self.core_postal_list.all()
+                if postal.valid_until is None
+                or postal.valid_until >= timezone.now().date()
+            ]
+            if len(active_postals) == 0:
                 self.primary_postal_address = None
-
-            if hasattr(self, "core_email_list"):
-                if self.core_email_list.all().count() == 1 or (
-                    self.core_email_list.all().count() > 0
-                    and self.primary_email_address is None
-                ):
-                    self.primary_email_address = self.core_email_list.first()
-            else:
-                self.primary_email_address = None
-
-            if hasattr(self, "core_phone_list"):
-                if (
-                    self.core_phone_list.all().count() == 1
-                    or self.primary_phonenumber is None
-                ):
-                    self.primary_phonenumber = self.core_phone_list.first()
-            else:
-                self.primary_phonenumber = None
+            elif (
+                len(active_postals) == 1
+                or self.primary_postal_address is None
+                or (
+                    self.primary_postal_address.valid_until
+                    and self.primary_postal_address.valid_until < timezone.now().date()
+                )
+            ):
+                self.primary_postal_address = active_postals[0]
+
+        else:
+            self.primary_postal_address = None
+
+        if hasattr(self, "core_email_list"):
+            if (
+                self.core_email_list.all().count() == 1
+                or self.primary_email_address is None
+            ):
+                self.primary_email_address = self.core_email_list.first()
+        else:
+            self.primary_email_address = None
+
+        if hasattr(self, "core_phone_list"):
+            if (
+                self.core_phone_list.all().count() == 1
+                or self.primary_phonenumber is None
+            ):
+                self.primary_phonenumber = self.core_phone_list.first()
+        else:
+            self.primary_phonenumber = None
 
         super().save(*args, **kwargs)
         if self.personnumber.startswith("__placeholder__"):
             self.personnumber = str(self.pk)
             super().save(update_fields=["personnumber"])
 
         self.default_sorting_name = self.name
@@ -240,51 +242,45 @@
         verbose_name_plural = _("Persons")
 
 
 class NaturalPerson(Person):
     first_name = models.CharField(_("First Name"), max_length=255, blank=True)
     middle_name = models.CharField(_("Middle Name"), max_length=255, blank=True)
     last_name = models.CharField(_("Last Name"), max_length=255, blank=True)
-    maiden_name = models.CharField(_("Maiden Name"), max_length=255, blank=True)
-
     autogenerate_displayname = models.BooleanField(
         _("Autogenerate Display Name"), default=True
     )
     title = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         limit_choices_to={"vocabulary__slug": "title"},
         related_name="title_persons",
-        verbose_name=_("Title"),
     )
-    title.formfield_kwargs = {"widget": forms.RadioSelect()}
-
+    title.verbose_name = _("Title")
     salutation = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         limit_choices_to={"vocabulary__slug": "salutation"},
         related_name="+",
-        verbose_name=_("Salutation"),
     )
-    salutation.formfield_kwargs = {"widget": forms.RadioSelect()}
+    salutation.verbose_name = _("Salutation")
 
     form_of_address = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         limit_choices_to={"vocabulary__slug": "form_of_address"},
         related_name="+",
-        verbose_name=_("Form of address"),
     )
-    form_of_address.formfield_kwargs = {"widget": forms.RadioSelect()}
+    form_of_address.verbose_name = _("Form of address")
 
     profession = models.CharField(
         _("Profession"),
         max_length=255,
         blank=True,
     )
     date_of_birth = models.DateField(_("Date of Birth"), blank=True, null=True)
@@ -294,31 +290,30 @@
     gender = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         limit_choices_to={"vocabulary__slug": "gender"},
         related_name="gender_persons",
-        verbose_name=_("Gender"),
     )
-    gender.formfield_kwargs = {"widget": forms.RadioSelect()}
+    gender.verbose_name = _("Gender")
 
     type = models.ForeignKey(
         Term,
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         limit_choices_to={"vocabulary__slug": "naturaltype"},
     )
     type.verbose_name = _("Person Type")
 
     def age(self):
         if not self.date_of_birth:
             return None
-        today = timezone.now().date()
+        today = datetime.date.today()
         birth = self.date_of_birth
         return (
             today.year
             - birth.year
             - ((today.month, today.day) < (birth.month, birth.day))
         )
```

### Comparing `basxconnect-0.4.61/basxconnect/core/models/relationships.py` & `basxconnect-0.4.7/basxconnect/core/models/relationships.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/models/utils.py` & `basxconnect-0.4.7/basxconnect/core/models/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,66 +5,36 @@
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.utils.html import mark_safe
 from django.utils.text import slugify
 from django.utils.translation import gettext_lazy as _
 
 
-class VocabularyManager(models.Manager):
-    def get_queryset(self):
-        return (
-            super()
-            .get_queryset()
-            .annotate(
-                termcount=models.Count(
-                    "term", output_field=models.IntegerField(_("Terms"))
-                )
-            )
-        )
-
-
 class Vocabulary(models.Model):
     name = models.CharField(_("Name"), max_length=255, unique=True)
     slug = models.SlugField(
         _("Slug"),
         unique=True,
         help_text=_("slug is human-readable, to make referencing easier"),
     )
 
-    objects = VocabularyManager()
-
     def __str__(self):
         return self.name
 
     class Meta:
         ordering = ["name"]
         verbose_name = _("Vocabulary")
         verbose_name_plural = _("Vocabularies")
 
 
-class TermManager(models.Manager):
-    def get_queryset(self):
-        return super().get_queryset().filter(disabled=False)
-
-    def including_disabled(self):
-        return super().get_queryset()
-
-
 class Term(models.Model):
     vocabulary = models.ForeignKey(Vocabulary, null=False, on_delete=models.CASCADE)
     vocabulary.verbose_name = _("Vocabulary")
     term = models.CharField(_("Term"), max_length=255)
     slug = models.CharField(_("Slug"), max_length=255, unique=True, blank=True)
-    disabled = models.BooleanField(
-        _("Disabled"),
-        default=False,
-        help_text=_("Do not allow this term to be selected"),
-    )
-
-    objects = TermManager()
 
     def save(self, *args, **kwargs):
         if not self.slug:
             self.slug = self.vocabulary.slug + "__" + slugify(self.term)
         super().save(*args, **kwargs)
 
     def __str__(self):
```

### Comparing `basxconnect-0.4.61/basxconnect/core/search_indexes.py` & `basxconnect-0.4.7/basxconnect/core/search_indexes.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/tests/settings.py` & `basxconnect-0.4.7/basxconnect/core/tests/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = "test"  # nosec # can ignore security check for testing key
 
 ALLOWED_HOSTS = ["*"]
 
 # BASXBREAD_DEPENDENCIES are imported in the start import at the top
 INSTALLED_APPS = [
-    "basxconnect.core",
+    "basxconnect.core.apps.CoreConfig",
     "basxconnect.contributions.apps.ContributionsConfig",
 ] + BASXBREAD_DEPENDENCIES
 
 TEMPLATES[0]["OPTIONS"]["context_processors"].append(
     "basxconnect.core.context_processors.basxconnect_core"
 )
```

### Comparing `basxconnect-0.4.61/basxconnect/core/tests/test_person.py` & `basxconnect-0.4.7/basxconnect/core/tests/test_person.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/urls.py` & `basxconnect-0.4.7/basxconnect/core/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from basxbread import views as breadviews
 from basxbread.utils.urls import (
     autopath,
     default_model_paths,
     model_urlname,
     reverse_model,
 )
-from basxbread.views import AddView, EditView
+from basxbread.views import AddView, BrowseView, EditView
 from django.views.generic import RedirectView
 
 import basxconnect.core.views.tag_views
 from basxconnect.core.views import settings_views
 from basxconnect.core.views.person import (
     person_browse_views,
     person_details_views,
@@ -122,28 +122,32 @@
         editview=EditRelationshipView,
         addview=AddRelationshipView,
     ),
     *default_model_paths(models.RelationshipType),
     *default_model_paths(
         models.Term,
         addview=AddView._with(fields=["term", "vocabulary"]),
-        editview=EditView._with(fields=["term", "slug", "disabled"]),
-        browseview=TermsBrowseView,
+        editview=EditView._with(fields=["term", "slug"]),
+        browseview=TermsBrowseView._with(
+            rowclickaction=BrowseView.gen_rowclickaction("edit", return_to_current=True)
+        ),
     ),
     *default_model_paths(
         models.Vocabulary,
         browseview=VocabularyBrowseView,
     ),
     *default_model_paths(models.Postal),
     *default_model_paths(models.Phone),
     *default_model_paths(models.Web),
+    autopath(settings_views.generalsettings),
     autopath(
         person_details_views.togglepersonstatus,
         model_urlname(models.Person, "togglestatus"),
     ),
+    autopath(settings_views.personsettings),
     autopath(settings_views.relationshipssettings),
     autopath(search_person_view.searchperson),
     autopath(
         person_modals_views.NaturalPersonEditMailingsView.as_view(),
         urlname=model_urlname(models.NaturalPerson, "ajax_edit_mailings"),
     ),
     autopath(
```

### Comparing `basxconnect-0.4.61/basxconnect/core/views/person/person_browse_views.py` & `basxconnect-0.4.7/basxconnect/core/views/person/person_browse_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 
 def export(request, queryset):
     # Fields which are filtered should also be displayed in columns
     form = PersonBrowseView.FilterForm({"status": ["active"], **request.GET})
     columns = list(PersonBrowseView.columns)
     if form.is_valid():
+
         # only the tags selected in the filter should be visible in the export
         tags = models.Term.objects.all()
         if form.cleaned_data.get("tags"):
             tags = form.cleaned_data.get("tags")
 
         def render_matching_tags(context):
             return ", ".join(str(i) for i in set(tags) & set(context["row"].tags.all()))
@@ -100,15 +101,15 @@
     columns = [
         DataTableColumn(
             layout.ObjectFieldLabel("personnumber", models.Person),
             hg.DIV(
                 hg.C("row.personnumber"),
                 style=hg.If(hg.C("row.deleted"), "text-decoration:line-through"),
             ),
-            sortingname="personnumber__int",
+            "personnumber__int",
         ),
         DataTableColumn(
             hg.DIV(
                 layout.tooltip.IconTooltip(
                     hg.UL(
                         hg.LI(hg.SPAN("●", style="color: green"), " ", _("Active")),
                         hg.LI(hg.SPAN("●", style="color: red"), " ", _("Inactive")),
```

### Comparing `basxconnect-0.4.61/basxconnect/core/views/person/person_details_views.py` & `basxconnect-0.4.7/basxconnect/core/views/person/person_details_views.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import basxbread
 import django
 import htmlgenerator as hg
 from basxbread import layout, menu
 from basxbread.layout.components.button import Button
 from basxbread.layout.components.forms import Form
 from basxbread.utils import Link, reverse_model
-from basxbread.views import EditView, ReadView
+from basxbread.views import EditView, ReadView, layoutasreadonly
 from django.apps import apps
+from django.conf import settings
 from django.forms import forms
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
+from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.csrf import csrf_exempt
 
 from ... import models
 from ...layouts.editperson import legalperson, naturalperson, personassociation
 from ...layouts.editperson.common import history_tab
 from ...layouts.editperson.common.head import editperson_head
@@ -24,49 +26,65 @@
 R = layout.grid.Row
 C = layout.grid.Col
 
 
 class NaturalPersonEditView(EditView):
     def get_layout(self):
         return personform_shortcut(
+            self.request,
             editnaturalperson_form(self.request),
         )
 
 
 class NaturalPersonReadView(ReadView):
     def get_layout(self):
         return personform_shortcut(
+            self.request,
             editnaturalperson_form(self.request),
         )
 
 
 class LegalPersonEditView(EditView):
     def get_layout(self):
-        return personform_shortcut(editlegalperson_form(self.request))
+        return personform_shortcut(
+            self.request,
+            editlegalperson_form(self.request),
+        )
 
 
 class LegalPersonReadView(ReadView):
     def get_layout(self):
-        return personform_shortcut(editlegalperson_form(self.request))
+        return layoutasreadonly(
+            personform_shortcut(
+                self.request,
+                editlegalperson_form(self.request),
+            )
+        )
 
 
 class PersonAssociationEditView(EditView):
     def get_layout(self):
-        return personform_shortcut(editpersonassociation_form(self.request))
+        return personform_shortcut(
+            self.request,
+            editpersonassociation_form(self.request),
+        )
 
 
 class PersonAssociationReadView(ReadView):
     def get_layout(self):
-        return personform_shortcut(editpersonassociation_form(self.request))
+        return personform_shortcut(
+            self.request,
+            editpersonassociation_form(self.request),
+        )
 
 
-def personform_shortcut(formlayout):
+def personform_shortcut(request, formlayout):
     return hg.BaseElement(
         layout.grid.Grid(
-            editperson_head(),
+            editperson_head(request),
             formlayout,
             gutter=False,
         )
     )
 
 
 def editnaturalperson_form(request):
@@ -112,15 +130,15 @@
             ),
         ),
     )
 
 
 def editperson_tabs(base_data_tab, mailing_tab, request):
     ret = [
-        base_data_tab(),
+        base_data_tab(request),
         relationshipstab(request),
         mailing_tab(request),
     ]
 
     if apps.is_installed("basxconnect.contributions"):
         from ...layouts.editperson.common import contributions_tab
 
@@ -148,14 +166,15 @@
     email = models.Email.objects.get(id=pk)
     enable_delete_mailer_contact_checkbox = apps.is_installed(
         "basxconnect.mailer_integration"
     ) and hasattr(email, "subscription")
 
     fields = []
     if enable_delete_mailer_contact_checkbox:
+
         from basxconnect.mailer_integration.settings import MAILER
 
         class DeleteMailerSubscriptionForm(forms.Form):
             delete_mailer_contact = django.forms.BooleanField(
                 label=_("Delete linked %s subscription as well") % MAILER.name(),
                 required=False,
             )
@@ -193,15 +212,15 @@
                     reverse_model(email.person, "read", kwargs={"pk": email.person.pk})
                 )
         else:
             form = forms.Form()
 
     return layout.render(
         request,
-        layout.skeleton.default_page_layout(
+        import_string(settings.DEFAULT_PAGE_LAYOUT)(
             menu.main,
             Form(
                 form,
                 hg.BaseElement(
                     hg.H3(_("Delete email %s") % email.email),
                     *(basxbread.layout.forms.FormField(field) for field in fields),
                 ),
```

### Comparing `basxconnect-0.4.61/basxconnect/core/views/person/person_modals_views.py` & `basxconnect-0.4.7/basxconnect/core/views/person/person_modals_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,14 @@
     fields = [
         "salutation",
         "title",
         "name",
         "autogenerate_displayname",
         "first_name",
         "last_name",
-        "middle_name",
-        "maiden_name",
         "gender",
         "date_of_birth",
         "place_of_birth",
         "profession",
         "deceased",
         "decease_date",
     ]
@@ -85,16 +83,14 @@
                         width=6,
                         breakpoint="lg",
                         style="align-self: flex-end;",
                     ),
                 ),
                 R(C(F("first_name"))),
                 R(C(F("last_name"))),
-                R(C(F("middle_name"))),
-                R(C(F("maiden_name"))),
                 R(C(F("gender"))),
                 R(C(F("date_of_birth"))),
                 R(C(F("place_of_birth"))),
                 R(C(F("profession"))),
                 R(C(F("deceased"))),
                 R(C(F("decease_date"))),
             )
@@ -126,19 +122,19 @@
         "salutation_letter",
     ]
 
 
 class EditPostalAddressView(EditView):
     model = models.Postal
     fields = [
+        "type",
         "address",
         "postcode",
         "city",
         "country",
-        "type",
         "valid_from",
         "valid_until",
     ]
 
     def form_valid(self, form, *args, **kwargs):
         ret = super().form_valid(form, *args, **kwargs)
         is_primary = form.cleaned_data["is_primary"]
@@ -176,17 +172,18 @@
         ret = super().form_valid(request, *args, **kwargs)
         self.object.person.save()
         return ret
 
 
 class EditEmailAddressView(EditView):
     model = models.Email
-    fields = ["email", "type"]
+    fields = ["type", "email"]
 
     def form_valid(self, form, *args, **kwargs):
+
         ret = super().form_valid(form, *args, **kwargs)
         is_primary = form.cleaned_data["is_primary"]
         if is_primary:
             self.object.person.primary_email_address = self.object
         self.object.person.save()
 
         if apps.is_installed("basxconnect.mailer_integration"):
```

### Comparing `basxconnect-0.4.61/basxconnect/core/views/person/search_person_view.py` & `basxconnect-0.4.7/basxconnect/core/views/person/search_person_view.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/views/relationship_views.py` & `basxconnect-0.4.7/basxconnect/core/views/relationship_views.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/views/tag_views.py` & `basxconnect-0.4.7/basxconnect/core/views/tag_views.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/core/views/term.py` & `basxconnect-0.4.7/basxconnect/core/views/term.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from basxbread import layout
-from basxbread.utils import Link, ModelHref, permissionname
-from basxbread.views import BrowseView, deletelink
+from basxbread.utils import Link, ModelHref
+from basxbread.views import BrowseView
 from django.utils.translation import gettext_lazy as _
 
 from basxconnect.core.models import Term, Vocabulary
 
 
 class TermsBrowseView(BrowseView):
-    rowclickaction = BrowseView.gen_rowclickaction("edit", return_to_current=True)
-    rowactions = [deletelink()]
-    columns = ["term", "slug"]
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
     def get(self, *args, **kwargs):
         vocabulary = Vocabulary.objects.filter(
             slug=self.request.GET.get("vocabulary_slug")
         ).first()
         if vocabulary:
             self.primary_button = layout.button.Button.from_link(
@@ -21,22 +20,18 @@
                     href=ModelHref(
                         Term,
                         "add",
                         query={"vocabulary": vocabulary.id},
                         return_to_current=True,
                     ),
                     label=_("Add %s") % Term._meta.verbose_name,
-                    permissions=[permissionname(Term, "add")],
                 ),
                 icon=layout.icon.Icon("add", size=20),
             )
-            self.title = Vocabulary.objects.get(
-                slug=self.request.GET.get("vocabulary_slug")
-            ).name
         return super().get(*args, **kwargs)
 
     def get_queryset(self):
-        qs = Term.objects.including_disabled()
+        qs = super().get_queryset()
         vocabulary_slug = self.request.GET.get("vocabulary_slug")
         if vocabulary_slug:
             qs = qs.filter(vocabulary__slug=vocabulary_slug)
         return qs
```

### Comparing `basxconnect-0.4.61/basxconnect/core/wizards/add_person.py` & `basxconnect-0.4.7/basxconnect/core/wizards/add_person.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,22 @@
 ADD_FORM_LAYOUTS = {
     NaturalPerson: lambda: hg.BaseElement(
         layout.grid.Row(
             layout.grid.Col(layout.forms.FormField("first_name")),
             layout.grid.Col(layout.forms.FormField("last_name")),
         ),
         layout.grid.Row(
-            layout.grid.Col(layout.forms.FormField("salutation"), width=2),
-            layout.grid.Col(layout.forms.FormField("gender"), width=2),
-            layout.grid.Col(width=4),
-            layout.grid.Col(layout.forms.FormField("preferred_language")),
+            layout.grid.Col(layout.forms.FormField("salutation")),
+            layout.grid.Col(layout.forms.FormField("gender")),
         ),
     ),
     LegalPerson: lambda: hg.DIV(
         layout.forms.FormField("name"), layout.forms.FormField("name_addition")
     ),
-    PersonAssociation: lambda: hg.DIV(layout.forms.FormField("name")),
+    PersonAssociation: hg.DIV(layout.forms.FormField("name")),
 }
 
 
 def ADD_ADDRESS_LAYOUT():
     return layout.grid.Grid(
         layout.grid.Row(
             layout.grid.Col(_("Address"), style="font-weight: 700; margin-bottom: 2rem")
@@ -68,16 +66,14 @@
         layout.grid.Row(
             layout.grid.Col(_("Email"), style="font-weight: 700; margin-bottom: 2rem")
         ),
         layout.grid.Row(
             layout.grid.Col(
                 layout.forms.FormField("email", elementattributes={"required": False})
             ),
-        ),
-        layout.grid.Row(
             layout.grid.Col(layout.forms.FormField("type")),
         ),
         gutter=False,
     )
 
 
 def generate_wizard_form(formlayout):
@@ -232,22 +228,19 @@
     form = modelform_factory(
         request=request, model=model, layout=ADD_FORM_LAYOUTS[model]()
     )(data, files, initial=initial)
 
     for fieldname, field in modelform_factory(
         request, Postal, ADD_ADDRESS_LAYOUT()
     )().fields.items():
-        if fieldname == "country":
-            field.required = False
         form.fields[fieldname] = field
 
     for fieldname, field in modelform_factory(
         request, Email, ADD_EMAIL_LAYOUT()
     )().fields.items():
-        field.required = False
         form.fields[fieldname] = field
 
     formlayout = hg.BaseElement(
         layout.grid.Grid(
             ADD_FORM_LAYOUTS[model](), style="margin-bottom: 2rem", gutter=False
         ),
         layout.grid.Grid(
@@ -309,15 +302,15 @@
             layout.progress_indicator.ProgressIndicator(
                 self.get_steps(),
                 style="margin-bottom: 2rem",
             ),
             layout.grid.Grid(
                 layout.grid.Row(
                     layout.grid.Col(
-                        generate_wizard_form(self.get_form()._layout), width=12
+                        generate_wizard_form(self.get_form()._layout), width=8
                     )
                 ),
                 gutter=False,
             ),
             hg.SCRIPT(
                 hg.mark_safe(
                     r"""
@@ -389,24 +382,22 @@
     def done(self, form_list, **kwargs):
         personform = list(form_list)[-1]
         # in case the new person had a subtype set, we need to set the attribute here
         subtype = (self.get_cleaned_data_for_step("Subtype") or {}).get("subtype")
         if subtype:
             personform.instance.type = subtype
         newperson = personform.save()
-
-        if personform.cleaned_data["country"] != "":
-            newperson.core_postal_list.create(
-                **{
-                    k: v
-                    for k, v in personform.cleaned_data.items()
-                    if k in ("address", "city", "postcode", "country")
-                }
-            )
-        if "email" in personform.cleaned_data and personform.cleaned_data["email"]:
+        newperson.core_postal_list.create(
+            **{
+                k: v
+                for k, v in personform.cleaned_data.items()
+                if k in ("address", "city", "postcode", "country")
+            }
+        )
+        if "email" in personform.cleaned_data:
             newperson.core_email_list.create(
                 email=personform.cleaned_data["email"],
                 type=personform.cleaned_data["type"],
             )
 
         newperson.save()
         return redirect(
```

### Comparing `basxconnect-0.4.61/basxconnect/invoicing/migrations/0002_alter_invoice_note.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0004_auto_20210823_1424.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-# Generated by Django 4.1.7 on 2023-04-05 04:19
+# Generated by Django 3.2.4 on 2021-08-23 14:24
 
+import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
-        ("basxconnect_invoicing", "0001_initial"),
+        ("core", "0011_auto_20210726_2047"),
+        ("mailer_integration", "0003_alter_interest_external_id"),
     ]
 
     operations = [
-        migrations.AlterField(
-            model_name="invoice",
-            name="note",
-            field=models.TextField(
-                blank=True,
-                help_text="Can be displayed on invoice and/or receipt",
-                verbose_name="Note to client",
+        migrations.RemoveField(
+            model_name="mailingpreferences",
+            name="person",
+        ),
+        migrations.AddField(
+            model_name="mailingpreferences",
+            name="email",
+            field=models.OneToOneField(
+                default=None,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="core.person",
             ),
+            preserve_default=False,
         ),
     ]
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/abstract/mailer.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/abstract/mailer.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             ),
             email=preferences.email.email,
             interests_ids=[
                 interest.external_id for interest in preferences.interests.all()
             ],
             status=preferences.status,
             language=preferences.language,
-            persontype=person.type.slug if hasattr(person, "type") else "",
         )
 
 
 class MailingInterest(NamedTuple):
     id: str
     name: str
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/dynamic_preferences_registry.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/dynamic_preferences_registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from django.utils.translation import gettext_lazy as _
 from dynamic_preferences.preferences import Section
 from dynamic_preferences.registries import global_preferences_registry
-from dynamic_preferences.types import (
-    BooleanPreference,
-    LongStringPreference,
-    StringPreference,
-)
+from dynamic_preferences.types import LongStringPreference, StringPreference
 
 mailchimp_integration = Section("mailchimp", _("Mailchimp"))
 
 
 @global_preferences_registry.register
 class MailchimpServer(StringPreference):
     section = mailchimp_integration
@@ -60,31 +56,7 @@
 
 @global_preferences_registry.register
 class MailchimpApiKey(LongStringPreference):
     section = mailchimp_integration
     name = "api_key"
     default = ""
     verbose_name = _("Mailchimp API key")
-
-
-@global_preferences_registry.register
-class MailchimpDisableInterestsKey(BooleanPreference):
-    section = mailchimp_integration
-    name = "disable_interests"
-    default = False
-    verbose_name = _("Disable mailing interests")
-
-
-@global_preferences_registry.register
-class MailchimpSynchronizeLanguage(BooleanPreference):
-    section = mailchimp_integration
-    name = "synchronize_language"
-    default = False
-    verbose_name = _("Synchronize language with Mailchimp")
-
-
-@global_preferences_registry.register
-class MailchimpAutomaticallySubscribeNewPersons(BooleanPreference):
-    section = mailchimp_integration
-    name = "automatically_subscribe_new_persons"
-    default = False
-    verbose_name = _("Automatically subscribe new persons")
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/help.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/help.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/layouts.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/layouts.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from basxbread.layout.components.icon import Icon
 from basxbread.utils import ModelHref
 from django.conf import settings
 from django.shortcuts import get_object_or_404
 from django.utils.formats import localize
 from django.utils.timezone import localtime
 from django.utils.translation import gettext_lazy as _
-from dynamic_preferences.registries import global_preferences_registry
 
 from basxconnect.core import models
 from basxconnect.core.layouts.editperson.common.utils import tile_with_icon
 from basxconnect.core.models import Person
 from basxconnect.mailer_integration.models import Interest, Subscription
 
 R = basxbread.layout.grid.Row
@@ -24,19 +23,17 @@
     person = get_object_or_404(Person, pk=request.resolver_match.kwargs["pk"])
     addresses = person.core_email_list.all()
     return tile_with_icon(
         Icon("email--new"),
         hg.H4(
             _("Email Subscriptions"),
         ),
-        *(
-            [_display_subscription(email) for email in addresses]
-            if hasattr(person, "core_email_list") and person.core_email_list.count() > 0
-            else C(_("Person has no email addresses"))
-        ),
+        *[_display_subscription(email) for email in addresses]
+        if hasattr(person, "core_email_list") and person.core_email_list.count() > 0
+        else C(_("Person has no email addresses")),
     )
 
 
 def _display_subscription(email):
     if not hasattr(email, "subscription"):
         return _display_email_without_subscription(email)
     subscription = email.subscription
@@ -83,22 +80,20 @@
                 style="padding-bottom: 24px;",
             ),
         ),
         *interests,
         R(
             C(_("Last synchronized"), width=6, breakpoint="lg"),
             C(
-                (
-                    localize(
-                        localtime(subscription.latest_sync.sync_completed_datetime),
-                        use_l10n=settings.USE_L10N,
-                    )
-                    if hasattr(subscription.latest_sync, "sync_completed_datetime")
-                    else ""
-                ),
+                localize(
+                    localtime(subscription.latest_sync.sync_completed_datetime),
+                    use_l10n=settings.USE_L10N,
+                )
+                if hasattr(subscription.latest_sync, "sync_completed_datetime")
+                else "",
                 breakpoint="lg",
             ),
             style="padding-bottom: 24px;",
         ),
         R(
             C(
                 layout.button.Button(
@@ -168,33 +163,19 @@
     )
     modal[0][1].attributes["style"] = "overflow: visible"
     modal[0].attributes["style"] = "overflow: visible"
     return modal
 
 
 def modal_add_subscription(email: models.Email):
-    preferred_language = email.person.preferred_language
-    set_language = (
-        global_preferences_registry.manager()["mailchimp__synchronize_language"]
-        and preferred_language
-    )
-    disable_interests = global_preferences_registry.manager()[
-        "mailchimp__disable_interests"
-    ]
     ret = layout.modal.Modal.with_ajax_content(
         heading=_("Add subscription"),
         url=ModelHref(
             Subscription,
             "ajax_add",
-            query={
-                "asajax": True,
-                "email": email.pk,
-                "status": "subscribed",
-                **({"language": preferred_language} if set_language else {}),
-                **({"interests": ""} if disable_interests else {}),
-            },
+            query={"asajax": True, "email": email.pk, "status": "subscribed"},
         ),
         submitlabel=_("Save"),
     )
     ret[0][1].attributes["style"] = "overflow: visible"
     ret[0].attributes["style"] = "overflow: visible"
     return ret
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/locale/de/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/mailer_integration/locale/de/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,72 +4,60 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:10
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:6
 msgid "Mailchimp"
-msgstr "Mailchimp"
+msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:18
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:14
 msgid "Mailchimp server"
-msgstr "Mailchimp Server"
+msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:26
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:22
 msgid "Mailchimp list ID"
-msgstr "Mailchimp Listen-ID"
+msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:34
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:30
 msgid "Mailchimp segment ID"
-msgstr "Mailchimp Segment-ID"
+msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:42
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:38
 msgid "Mailchimp interests category ID"
-msgstr "Mailchimp Interessenskategorie-ID"
+msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:50
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:46
 msgid "Mailchimp tag"
-msgstr "Mailchimp-Tag"
+msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:58
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:54
 msgid "BasxConnect Mailchimp tag"
-msgstr "BasxConnect Mailchimp-Tag"
+msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:66
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:62
 msgid "Mailchimp API key"
-msgstr "Mailchimp API-Key"
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:74
-msgid "Disable mailing interests"
-msgstr "Mailing Interessen deaktivieren"
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:82
-msgid "Synchronize language with Mailchimp"
-msgstr "Synchronisiere Sprache mit Mailchimp"
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:90
-msgid "Automatically subscribe new persons"
-msgstr "Füge automatisch Abonements für neue Personen hinzu"
+msgstr ""
 
 #: basxconnect/mailer_integration/help.py:8
-#: basxconnect/mailer_integration/views.py:84
+#: basxconnect/mailer_integration/views.py:69
 msgid "Help"
-msgstr "Hilfe"
+msgstr ""
 
 #: basxconnect/mailer_integration/help.py:10
 msgid ""
 "The button below is currently the only way of getting new subcribers from "
 "the mailer into our system. Is it also the only way of getting updates for "
 "subscribers that we already have in our system. This is what happens when "
 "the button is pressed:"
@@ -90,54 +78,54 @@
 
 #: basxconnect/mailer_integration/help.py:28
 msgid ""
 "If an email address is not yet in BasxConnect, a new person will be created "
 "with that email address."
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:29
+#: basxconnect/mailer_integration/layouts.py:28
 msgid "Email Subscriptions"
 msgstr "Email Abonnemente"
 
-#: basxconnect/mailer_integration/layouts.py:33
+#: basxconnect/mailer_integration/layouts.py:32
 msgid "Person has no email addresses"
 msgstr "Person hat keine Email Adressen"
 
-#: basxconnect/mailer_integration/layouts.py:76
+#: basxconnect/mailer_integration/layouts.py:75
 msgid "Status before archiving"
-msgstr "Status vor dem Archivieren"
+msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:86
+#: basxconnect/mailer_integration/layouts.py:85
 msgid "Last synchronized"
 msgstr "Zuletzt synchronisiert"
 
-#: basxconnect/mailer_integration/layouts.py:121
+#: basxconnect/mailer_integration/layouts.py:120
 msgid "No subscription yet for "
 msgstr "Noch kein Abonnement für "
 
-#: basxconnect/mailer_integration/layouts.py:123
-#: basxconnect/mailer_integration/layouts.py:180
+#: basxconnect/mailer_integration/layouts.py:122
+#: basxconnect/mailer_integration/layouts.py:171
 msgid "Add subscription"
 msgstr "Abonnement hinzufügen"
 
-#: basxconnect/mailer_integration/layouts.py:140
-#: basxconnect/mailer_integration/layouts.py:143
+#: basxconnect/mailer_integration/layouts.py:139
+#: basxconnect/mailer_integration/layouts.py:142
 msgid "active"
 msgstr "Aktiv"
 
-#: basxconnect/mailer_integration/layouts.py:146
+#: basxconnect/mailer_integration/layouts.py:145
 msgid "inactive"
 msgstr "Inaktiv"
 
-#: basxconnect/mailer_integration/layouts.py:156
+#: basxconnect/mailer_integration/layouts.py:155
 msgid "Edit subscription"
 msgstr "Abonnement bearbeiten"
 
-#: basxconnect/mailer_integration/layouts.py:163
-#: basxconnect/mailer_integration/layouts.py:192
+#: basxconnect/mailer_integration/layouts.py:162
+#: basxconnect/mailer_integration/layouts.py:177
 msgid "Save"
 msgstr "Speichern"
 
 #: basxconnect/mailer_integration/models.py:24
 msgid "Number of persons in the mailer segment"
 msgstr "Anzahl Personen im Mailer-Segment"
 
@@ -158,99 +146,83 @@
 msgstr "Vorname"
 
 #: basxconnect/mailer_integration/models.py:74
 msgid "Last Name"
 msgstr "Nachname"
 
 #: basxconnect/mailer_integration/models.py:76
+#, fuzzy
+#| msgid "Add subscription"
 msgid "Old subscription status"
-msgstr "Alter Abonnement-Status"
+msgstr "Abonnement hinzufügen"
 
 #: basxconnect/mailer_integration/models.py:79
+#, fuzzy
+#| msgid "No subscription yet for "
 msgid "New subscription status"
-msgstr "Neuer Abonnement-Status"
+msgstr "Noch kein Abonnement für "
 
 #: basxconnect/mailer_integration/models.py:87
-#: basxconnect/mailer_integration/views.py:104
+#: basxconnect/mailer_integration/views.py:89
 msgid "Newly added to BasxConnect"
 msgstr "Neu zu BasxConnect hinzugefügt"
 
 #: basxconnect/mailer_integration/models.py:88
 msgid "Not added to BasxConnect"
 msgstr "Nicht zu BasxConnect hinzugefügt"
 
 #: basxconnect/mailer_integration/models.py:89
 msgid "Synchronized previously but not this time"
 msgstr "Schon mal synchronisiert, aber nicht diesmal"
 
 #: basxconnect/mailer_integration/models.py:90
-#: basxconnect/mailer_integration/views.py:108
+#: basxconnect/mailer_integration/views.py:93
 msgid "Subscription status changed"
-msgstr "Abonement-Status geändert"
+msgstr ""
 
 #: basxconnect/mailer_integration/models.py:93
 msgid "Synchronization Status"
 msgstr "Synchronisationsstatus"
 
-#: basxconnect/mailer_integration/models.py:99
-#: basxconnect/mailer_integration/views.py:53
-msgid "Possible duplicate"
-msgstr "Mögliche Duplikate"
-
-#: basxconnect/mailer_integration/models.py:101
-msgid "Other person with same first and last name already exists"
-msgstr "Andere Person mit dem selben Vor- und Nachnamen exisiert schon"
-
-#: basxconnect/mailer_integration/views.py:36
+#: basxconnect/mailer_integration/views.py:34
 msgid "Sychronization successful"
 msgstr "Synchronisation erfolgreich"
 
-#: basxconnect/mailer_integration/views.py:38
+#: basxconnect/mailer_integration/views.py:36
 #, python-format
 msgid ""
 "Synchronized with mailer segment containing %s contacts. %s new persons were "
 "added to BasxConnect."
 msgstr ""
 "Das synchronisierte Segment auf dem Mailer beinhhaltet %s Kontakte. %s neue "
 "personen wurden zu BasxConnect hinzugefügt."
 
-#: basxconnect/mailer_integration/views.py:55
-#, python-brace-format
-msgid ""
-"New person '{person.first_name} {person.last_name}' might be a duplicate, "
-"there is another person with the same name."
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:64
-msgid "Error"
-msgstr "Fehler"
-
-#: basxconnect/mailer_integration/views.py:75
+#: basxconnect/mailer_integration/views.py:60
 msgid "Synchronization of Email Subcriptions"
 msgstr "Synchronisation von Email Abonnementen"
 
-#: basxconnect/mailer_integration/views.py:81
+#: basxconnect/mailer_integration/views.py:66
 msgid "Download subscriptions"
 msgstr "Abonnemente herunterladen"
 
-#: basxconnect/mailer_integration/views.py:112
+#: basxconnect/mailer_integration/views.py:97
 msgid "Previous Executions"
 msgstr "Vergangene Ausführungen"
 
-#: basxconnect/mailer_integration/views.py:123
+#: basxconnect/mailer_integration/views.py:108
 msgid "Delete"
 msgstr "Löschen"
 
-#: basxconnect/mailer_integration/views.py:161
+#: basxconnect/mailer_integration/views.py:146
 msgid "Old"
-msgstr "Alt"
+msgstr ""
 
-#: basxconnect/mailer_integration/views.py:163
+#: basxconnect/mailer_integration/views.py:148
 msgid "New"
-msgstr "Neu"
+msgstr ""
 
-#: basxconnect/mailer_integration/views.py:170
+#: basxconnect/mailer_integration/views.py:155
 msgid "Tools"
 msgstr "Werkzeuge"
 
 #~ msgid "In mailer segment but not added to BasxConnect"
 #~ msgstr "Im Mailer-Segment aber nicht zu BasxConnect hinzugefügt"
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/locale/fr/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/mailer_integration/locale/fr/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,70 +4,58 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:10
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:6
 msgid "Mailchimp"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:18
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:14
 msgid "Mailchimp server"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:26
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:22
 msgid "Mailchimp list ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:34
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:30
 msgid "Mailchimp segment ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:42
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:38
 msgid "Mailchimp interests category ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:50
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:46
 msgid "Mailchimp tag"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:58
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:54
 msgid "BasxConnect Mailchimp tag"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:66
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:62
 msgid "Mailchimp API key"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:74
-msgid "Disable mailing interests"
-msgstr ""
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:82
-msgid "Synchronize language with Mailchimp"
-msgstr ""
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:90
-msgid "Automatically subscribe new persons"
-msgstr ""
-
 #: basxconnect/mailer_integration/help.py:8
-#: basxconnect/mailer_integration/views.py:84
+#: basxconnect/mailer_integration/views.py:69
 msgid "Help"
 msgstr ""
 
 #: basxconnect/mailer_integration/help.py:10
 msgid ""
 "The button below is currently the only way of getting new subcribers from "
 "the mailer into our system. Is it also the only way of getting updates for "
@@ -90,54 +78,54 @@
 
 #: basxconnect/mailer_integration/help.py:28
 msgid ""
 "If an email address is not yet in BasxConnect, a new person will be created "
 "with that email address."
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:29
+#: basxconnect/mailer_integration/layouts.py:28
 msgid "Email Subscriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:33
+#: basxconnect/mailer_integration/layouts.py:32
 msgid "Person has no email addresses"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:76
+#: basxconnect/mailer_integration/layouts.py:75
 msgid "Status before archiving"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:86
+#: basxconnect/mailer_integration/layouts.py:85
 msgid "Last synchronized"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:121
+#: basxconnect/mailer_integration/layouts.py:120
 msgid "No subscription yet for "
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:123
-#: basxconnect/mailer_integration/layouts.py:180
+#: basxconnect/mailer_integration/layouts.py:122
+#: basxconnect/mailer_integration/layouts.py:171
 msgid "Add subscription"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:140
-#: basxconnect/mailer_integration/layouts.py:143
+#: basxconnect/mailer_integration/layouts.py:139
+#: basxconnect/mailer_integration/layouts.py:142
 msgid "active"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:146
+#: basxconnect/mailer_integration/layouts.py:145
 msgid "inactive"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:156
+#: basxconnect/mailer_integration/layouts.py:155
 msgid "Edit subscription"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:163
-#: basxconnect/mailer_integration/layouts.py:192
+#: basxconnect/mailer_integration/layouts.py:162
+#: basxconnect/mailer_integration/layouts.py:177
 msgid "Save"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:24
 msgid "Number of persons in the mailer segment"
 msgstr ""
 
@@ -166,86 +154,66 @@
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:79
 msgid "New subscription status"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:87
-#: basxconnect/mailer_integration/views.py:104
+#: basxconnect/mailer_integration/views.py:89
 msgid "Newly added to BasxConnect"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:88
 msgid "Not added to BasxConnect"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:89
 msgid "Synchronized previously but not this time"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:90
-#: basxconnect/mailer_integration/views.py:108
+#: basxconnect/mailer_integration/views.py:93
 msgid "Subscription status changed"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:93
 msgid "Synchronization Status"
 msgstr ""
 
-#: basxconnect/mailer_integration/models.py:99
-#: basxconnect/mailer_integration/views.py:53
-msgid "Possible duplicate"
-msgstr ""
-
-#: basxconnect/mailer_integration/models.py:101
-msgid "Other person with same first and last name already exists"
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:36
+#: basxconnect/mailer_integration/views.py:34
 msgid "Sychronization successful"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:38
+#: basxconnect/mailer_integration/views.py:36
 #, python-format
 msgid ""
 "Synchronized with mailer segment containing %s contacts. %s new persons were "
 "added to BasxConnect."
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:55
-#, python-brace-format
-msgid ""
-"New person '{person.first_name} {person.last_name}' might be a duplicate, "
-"there is another person with the same name."
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:64
-msgid "Error"
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:75
+#: basxconnect/mailer_integration/views.py:60
 msgid "Synchronization of Email Subcriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:81
+#: basxconnect/mailer_integration/views.py:66
 msgid "Download subscriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:112
+#: basxconnect/mailer_integration/views.py:97
 msgid "Previous Executions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:123
+#: basxconnect/mailer_integration/views.py:108
 msgid "Delete"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:161
+#: basxconnect/mailer_integration/views.py:146
 msgid "Old"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:163
+#: basxconnect/mailer_integration/views.py:148
 msgid "New"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:170
+#: basxconnect/mailer_integration/views.py:155
 msgid "Tools"
 msgstr ""
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/locale/nb_NO/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/mailer_integration/locale/pt/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,69 +4,58 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:10
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:6
 msgid "Mailchimp"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:18
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:14
 msgid "Mailchimp server"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:26
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:22
 msgid "Mailchimp list ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:34
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:30
 msgid "Mailchimp segment ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:42
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:38
 msgid "Mailchimp interests category ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:50
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:46
 msgid "Mailchimp tag"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:58
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:54
 msgid "BasxConnect Mailchimp tag"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:66
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:62
 msgid "Mailchimp API key"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:74
-msgid "Disable mailing interests"
-msgstr ""
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:82
-msgid "Synchronize language with Mailchimp"
-msgstr ""
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:90
-msgid "Automatically subscribe new persons"
-msgstr ""
-
 #: basxconnect/mailer_integration/help.py:8
-#: basxconnect/mailer_integration/views.py:84
+#: basxconnect/mailer_integration/views.py:69
 msgid "Help"
 msgstr ""
 
 #: basxconnect/mailer_integration/help.py:10
 msgid ""
 "The button below is currently the only way of getting new subcribers from "
 "the mailer into our system. Is it also the only way of getting updates for "
@@ -89,54 +78,54 @@
 
 #: basxconnect/mailer_integration/help.py:28
 msgid ""
 "If an email address is not yet in BasxConnect, a new person will be created "
 "with that email address."
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:29
+#: basxconnect/mailer_integration/layouts.py:28
 msgid "Email Subscriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:33
+#: basxconnect/mailer_integration/layouts.py:32
 msgid "Person has no email addresses"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:76
+#: basxconnect/mailer_integration/layouts.py:75
 msgid "Status before archiving"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:86
+#: basxconnect/mailer_integration/layouts.py:85
 msgid "Last synchronized"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:121
+#: basxconnect/mailer_integration/layouts.py:120
 msgid "No subscription yet for "
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:123
-#: basxconnect/mailer_integration/layouts.py:180
+#: basxconnect/mailer_integration/layouts.py:122
+#: basxconnect/mailer_integration/layouts.py:171
 msgid "Add subscription"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:140
-#: basxconnect/mailer_integration/layouts.py:143
+#: basxconnect/mailer_integration/layouts.py:139
+#: basxconnect/mailer_integration/layouts.py:142
 msgid "active"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:146
+#: basxconnect/mailer_integration/layouts.py:145
 msgid "inactive"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:156
+#: basxconnect/mailer_integration/layouts.py:155
 msgid "Edit subscription"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:163
-#: basxconnect/mailer_integration/layouts.py:192
+#: basxconnect/mailer_integration/layouts.py:162
+#: basxconnect/mailer_integration/layouts.py:177
 msgid "Save"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:24
 msgid "Number of persons in the mailer segment"
 msgstr ""
 
@@ -165,86 +154,66 @@
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:79
 msgid "New subscription status"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:87
-#: basxconnect/mailer_integration/views.py:104
+#: basxconnect/mailer_integration/views.py:89
 msgid "Newly added to BasxConnect"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:88
 msgid "Not added to BasxConnect"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:89
 msgid "Synchronized previously but not this time"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:90
-#: basxconnect/mailer_integration/views.py:108
+#: basxconnect/mailer_integration/views.py:93
 msgid "Subscription status changed"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:93
 msgid "Synchronization Status"
 msgstr ""
 
-#: basxconnect/mailer_integration/models.py:99
-#: basxconnect/mailer_integration/views.py:53
-msgid "Possible duplicate"
-msgstr ""
-
-#: basxconnect/mailer_integration/models.py:101
-msgid "Other person with same first and last name already exists"
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:36
+#: basxconnect/mailer_integration/views.py:34
 msgid "Sychronization successful"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:38
+#: basxconnect/mailer_integration/views.py:36
 #, python-format
 msgid ""
 "Synchronized with mailer segment containing %s contacts. %s new persons were "
 "added to BasxConnect."
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:55
-#, python-brace-format
-msgid ""
-"New person '{person.first_name} {person.last_name}' might be a duplicate, "
-"there is another person with the same name."
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:64
-msgid "Error"
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:75
+#: basxconnect/mailer_integration/views.py:60
 msgid "Synchronization of Email Subcriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:81
+#: basxconnect/mailer_integration/views.py:66
 msgid "Download subscriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:112
+#: basxconnect/mailer_integration/views.py:97
 msgid "Previous Executions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:123
+#: basxconnect/mailer_integration/views.py:108
 msgid "Delete"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:161
+#: basxconnect/mailer_integration/views.py:146
 msgid "Old"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:163
+#: basxconnect/mailer_integration/views.py:148
 msgid "New"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:170
+#: basxconnect/mailer_integration/views.py:155
 msgid "Tools"
 msgstr ""
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/locale/pt/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/mailer_integration/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -4,70 +4,57 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:10
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:6
 msgid "Mailchimp"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:18
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:14
 msgid "Mailchimp server"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:26
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:22
 msgid "Mailchimp list ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:34
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:30
 msgid "Mailchimp segment ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:42
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:38
 msgid "Mailchimp interests category ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:50
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:46
 msgid "Mailchimp tag"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:58
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:54
 msgid "BasxConnect Mailchimp tag"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:66
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:62
 msgid "Mailchimp API key"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:74
-msgid "Disable mailing interests"
-msgstr ""
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:82
-msgid "Synchronize language with Mailchimp"
-msgstr ""
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:90
-msgid "Automatically subscribe new persons"
-msgstr ""
-
 #: basxconnect/mailer_integration/help.py:8
-#: basxconnect/mailer_integration/views.py:84
+#: basxconnect/mailer_integration/views.py:69
 msgid "Help"
 msgstr ""
 
 #: basxconnect/mailer_integration/help.py:10
 msgid ""
 "The button below is currently the only way of getting new subcribers from "
 "the mailer into our system. Is it also the only way of getting updates for "
@@ -90,54 +77,54 @@
 
 #: basxconnect/mailer_integration/help.py:28
 msgid ""
 "If an email address is not yet in BasxConnect, a new person will be created "
 "with that email address."
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:29
+#: basxconnect/mailer_integration/layouts.py:28
 msgid "Email Subscriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:33
+#: basxconnect/mailer_integration/layouts.py:32
 msgid "Person has no email addresses"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:76
+#: basxconnect/mailer_integration/layouts.py:75
 msgid "Status before archiving"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:86
+#: basxconnect/mailer_integration/layouts.py:85
 msgid "Last synchronized"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:121
+#: basxconnect/mailer_integration/layouts.py:120
 msgid "No subscription yet for "
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:123
-#: basxconnect/mailer_integration/layouts.py:180
+#: basxconnect/mailer_integration/layouts.py:122
+#: basxconnect/mailer_integration/layouts.py:171
 msgid "Add subscription"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:140
-#: basxconnect/mailer_integration/layouts.py:143
+#: basxconnect/mailer_integration/layouts.py:139
+#: basxconnect/mailer_integration/layouts.py:142
 msgid "active"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:146
+#: basxconnect/mailer_integration/layouts.py:145
 msgid "inactive"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:156
+#: basxconnect/mailer_integration/layouts.py:155
 msgid "Edit subscription"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:163
-#: basxconnect/mailer_integration/layouts.py:192
+#: basxconnect/mailer_integration/layouts.py:162
+#: basxconnect/mailer_integration/layouts.py:177
 msgid "Save"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:24
 msgid "Number of persons in the mailer segment"
 msgstr ""
 
@@ -166,86 +153,66 @@
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:79
 msgid "New subscription status"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:87
-#: basxconnect/mailer_integration/views.py:104
+#: basxconnect/mailer_integration/views.py:89
 msgid "Newly added to BasxConnect"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:88
 msgid "Not added to BasxConnect"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:89
 msgid "Synchronized previously but not this time"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:90
-#: basxconnect/mailer_integration/views.py:108
+#: basxconnect/mailer_integration/views.py:93
 msgid "Subscription status changed"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:93
 msgid "Synchronization Status"
 msgstr ""
 
-#: basxconnect/mailer_integration/models.py:99
-#: basxconnect/mailer_integration/views.py:53
-msgid "Possible duplicate"
-msgstr ""
-
-#: basxconnect/mailer_integration/models.py:101
-msgid "Other person with same first and last name already exists"
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:36
+#: basxconnect/mailer_integration/views.py:34
 msgid "Sychronization successful"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:38
+#: basxconnect/mailer_integration/views.py:36
 #, python-format
 msgid ""
 "Synchronized with mailer segment containing %s contacts. %s new persons were "
 "added to BasxConnect."
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:55
-#, python-brace-format
-msgid ""
-"New person '{person.first_name} {person.last_name}' might be a duplicate, "
-"there is another person with the same name."
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:64
-msgid "Error"
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:75
+#: basxconnect/mailer_integration/views.py:60
 msgid "Synchronization of Email Subcriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:81
+#: basxconnect/mailer_integration/views.py:66
 msgid "Download subscriptions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:112
+#: basxconnect/mailer_integration/views.py:97
 msgid "Previous Executions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:123
+#: basxconnect/mailer_integration/views.py:108
 msgid "Delete"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:161
+#: basxconnect/mailer_integration/views.py:146
 msgid "Old"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:163
+#: basxconnect/mailer_integration/views.py:148
 msgid "New"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:170
+#: basxconnect/mailer_integration/views.py:155
 msgid "Tools"
 msgstr ""
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/locale/th/LC_MESSAGES/django.po` & `basxconnect-0.4.7/basxconnect/mailer_integration/locale/th/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,82 +4,68 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 11:33+0700\n"
+"POT-Creation-Date: 2022-07-24 15:47+0700\n"
 "PO-Revision-Date: 2021-11-01 12:38+0700\n"
 "Last-Translator: Saksinkarn Petchkuljinda <dward.the.2nd@gmail.com>\n"
 "Language-Team: Thai <LL@li.org>\n"
 "Language: th\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:10
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:6
 msgid "Mailchimp"
 msgstr "Mailchimp"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:18
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:14
 #, fuzzy
 #| msgid "Mailchimp"
 msgid "Mailchimp server"
 msgstr "Mailchimp"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:26
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:22
 #, fuzzy
 #| msgid "Mailchimp"
 msgid "Mailchimp list ID"
 msgstr "Mailchimp"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:34
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:30
 #, fuzzy
 #| msgid "Mailchimp"
 msgid "Mailchimp segment ID"
 msgstr "Mailchimp"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:42
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:38
 msgid "Mailchimp interests category ID"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:50
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:46
 #, fuzzy
 #| msgid "Mailchimp"
 msgid "Mailchimp tag"
 msgstr "Mailchimp"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:58
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:54
 msgid "BasxConnect Mailchimp tag"
 msgstr ""
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:66
+#: basxconnect/mailer_integration/dynamic_preferences_registry.py:62
 #, fuzzy
 #| msgid "Mailchimp"
 msgid "Mailchimp API key"
 msgstr "Mailchimp"
 
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:74
-#, fuzzy
-#| msgid "Mailing Interests"
-msgid "Disable mailing interests"
-msgstr "เรื่องที่สนใจรับทางอีเมล"
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:82
-msgid "Synchronize language with Mailchimp"
-msgstr ""
-
-#: basxconnect/mailer_integration/dynamic_preferences_registry.py:90
-msgid "Automatically subscribe new persons"
-msgstr ""
-
 #: basxconnect/mailer_integration/help.py:8
-#: basxconnect/mailer_integration/views.py:84
+#: basxconnect/mailer_integration/views.py:69
 msgid "Help"
 msgstr ""
 
 #: basxconnect/mailer_integration/help.py:10
 msgid ""
 "The button below is currently the only way of getting new subcribers from "
 "the mailer into our system. Is it also the only way of getting updates for "
@@ -102,58 +88,58 @@
 
 #: basxconnect/mailer_integration/help.py:28
 msgid ""
 "If an email address is not yet in BasxConnect, a new person will be created "
 "with that email address."
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:29
+#: basxconnect/mailer_integration/layouts.py:28
 msgid "Email Subscriptions"
 msgstr "การสมัครรับข้อมูลทางอีเมล"
 
-#: basxconnect/mailer_integration/layouts.py:33
+#: basxconnect/mailer_integration/layouts.py:32
 msgid "Person has no email addresses"
 msgstr "บุคคลดังกล่าวไม่มีอีเมลที่ระบุไว้"
 
-#: basxconnect/mailer_integration/layouts.py:76
+#: basxconnect/mailer_integration/layouts.py:75
 msgid "Status before archiving"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:86
+#: basxconnect/mailer_integration/layouts.py:85
 msgid "Last synchronized"
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:121
+#: basxconnect/mailer_integration/layouts.py:120
 msgid "No subscription yet for "
 msgstr ""
 
-#: basxconnect/mailer_integration/layouts.py:123
-#: basxconnect/mailer_integration/layouts.py:180
+#: basxconnect/mailer_integration/layouts.py:122
+#: basxconnect/mailer_integration/layouts.py:171
 #, fuzzy
 #| msgid "Email Subscriptions"
 msgid "Add subscription"
 msgstr "การสมัครรับข้อมูลทางอีเมล"
 
-#: basxconnect/mailer_integration/layouts.py:140
-#: basxconnect/mailer_integration/layouts.py:143
+#: basxconnect/mailer_integration/layouts.py:139
+#: basxconnect/mailer_integration/layouts.py:142
 msgid "active"
 msgstr "เปิดใช้งาน"
 
-#: basxconnect/mailer_integration/layouts.py:146
+#: basxconnect/mailer_integration/layouts.py:145
 msgid "inactive"
 msgstr "ปิดใช้งาน"
 
-#: basxconnect/mailer_integration/layouts.py:156
+#: basxconnect/mailer_integration/layouts.py:155
 #, fuzzy
 #| msgid "Edit Email Subscriptions"
 msgid "Edit subscription"
 msgstr "แก้ไขการรับอีเมล"
 
-#: basxconnect/mailer_integration/layouts.py:163
-#: basxconnect/mailer_integration/layouts.py:192
+#: basxconnect/mailer_integration/layouts.py:162
+#: basxconnect/mailer_integration/layouts.py:177
 msgid "Save"
 msgstr "บันทึก"
 
 #: basxconnect/mailer_integration/models.py:24
 msgid "Number of persons in the mailer segment"
 msgstr ""
 
@@ -186,95 +172,75 @@
 #: basxconnect/mailer_integration/models.py:79
 #, fuzzy
 #| msgid "Email Subscriptions"
 msgid "New subscription status"
 msgstr "การสมัครรับข้อมูลทางอีเมล"
 
 #: basxconnect/mailer_integration/models.py:87
-#: basxconnect/mailer_integration/views.py:104
+#: basxconnect/mailer_integration/views.py:89
 msgid "Newly added to BasxConnect"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:88
 msgid "Not added to BasxConnect"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:89
 msgid "Synchronized previously but not this time"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:90
-#: basxconnect/mailer_integration/views.py:108
+#: basxconnect/mailer_integration/views.py:93
 msgid "Subscription status changed"
 msgstr ""
 
 #: basxconnect/mailer_integration/models.py:93
 msgid "Synchronization Status"
 msgstr ""
 
-#: basxconnect/mailer_integration/models.py:99
-#: basxconnect/mailer_integration/views.py:53
-msgid "Possible duplicate"
-msgstr ""
-
-#: basxconnect/mailer_integration/models.py:101
-msgid "Other person with same first and last name already exists"
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:36
+#: basxconnect/mailer_integration/views.py:34
 msgid "Sychronization successful"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:38
+#: basxconnect/mailer_integration/views.py:36
 #, python-format
 msgid ""
 "Synchronized with mailer segment containing %s contacts. %s new persons were "
 "added to BasxConnect."
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:55
-#, python-brace-format
-msgid ""
-"New person '{person.first_name} {person.last_name}' might be a duplicate, "
-"there is another person with the same name."
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:64
-msgid "Error"
-msgstr ""
-
-#: basxconnect/mailer_integration/views.py:75
+#: basxconnect/mailer_integration/views.py:60
 #, fuzzy
 #| msgid "Edit Email Subscriptions"
 msgid "Synchronization of Email Subcriptions"
 msgstr "แก้ไขการรับอีเมล"
 
-#: basxconnect/mailer_integration/views.py:81
+#: basxconnect/mailer_integration/views.py:66
 #, fuzzy
 #| msgid "Email Subscriptions"
 msgid "Download subscriptions"
 msgstr "การสมัครรับข้อมูลทางอีเมล"
 
-#: basxconnect/mailer_integration/views.py:112
+#: basxconnect/mailer_integration/views.py:97
 msgid "Previous Executions"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:123
+#: basxconnect/mailer_integration/views.py:108
 msgid "Delete"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:161
+#: basxconnect/mailer_integration/views.py:146
 msgid "Old"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:163
+#: basxconnect/mailer_integration/views.py:148
 msgid "New"
 msgstr ""
 
-#: basxconnect/mailer_integration/views.py:170
+#: basxconnect/mailer_integration/views.py:155
 msgid "Tools"
 msgstr ""
 
 #~ msgid "no mailing preferences yet for "
 #~ msgstr "ยังไม่มีการตั้งค่าการส่งอีเมลสำหรับ "
 
 #~ msgid "Add mailing preferences"
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/mailchimp/mailer.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/mailchimp/mailer.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/mailchimp/parsing.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/mailchimp/parsing.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0001_initial.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.4 on 2021-08-18 07:44
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     initial = True
 
     dependencies = [
         ("core", "0011_auto_20210726_2047"),
     ]
 
     operations = [
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0004_auto_20210823_1424.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0008_alter_mailingpreferences_email.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-# Generated by Django 3.2.4 on 2021-08-23 14:24
+# Generated by Django 3.2.4 on 2021-08-25 08:31
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0011_auto_20210726_2047"),
-        ("mailer_integration", "0003_alter_interest_external_id"),
+        ("mailer_integration", "0007_alter_mailingpreferences_interests"),
     ]
 
     operations = [
-        migrations.RemoveField(
-            model_name="mailingpreferences",
-            name="person",
-        ),
-        migrations.AddField(
+        migrations.AlterField(
             model_name="mailingpreferences",
             name="email",
             field=models.OneToOneField(
-                default=None,
-                on_delete=django.db.models.deletion.CASCADE,
-                to="core.person",
+                blank=True, on_delete=django.db.models.deletion.CASCADE, to="core.email"
             ),
-            preserve_default=False,
         ),
     ]
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0005_alter_mailingpreferences_email.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0005_alter_mailingpreferences_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.4 on 2021-08-23 14:30
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0011_auto_20210726_2047"),
         ("mailer_integration", "0004_auto_20210823_1424"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0006_alter_mailingpreferences_status.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0006_alter_mailingpreferences_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.4 on 2021-08-23 16:38
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0005_alter_mailingpreferences_email"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="mailingpreferences",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0008_alter_mailingpreferences_email.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0009_alter_mailingpreferences_email.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Generated by Django 3.2.4 on 2021-08-25 08:31
+# Generated by Django 3.2.4 on 2021-08-26 13:29
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("core", "0011_auto_20210726_2047"),
-        ("mailer_integration", "0007_alter_mailingpreferences_interests"),
+        ("mailer_integration", "0008_alter_mailingpreferences_email"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="mailingpreferences",
             name="email",
             field=models.OneToOneField(
-                blank=True, on_delete=django.db.models.deletion.CASCADE, to="core.email"
+                on_delete=django.db.models.deletion.CASCADE, to="core.email"
             ),
         ),
     ]
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0010_mailingpreferences_language.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0010_mailingpreferences_language.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.4 on 2021-11-02 07:33
 
 from basxbread.contrib import languages
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0009_alter_mailingpreferences_email"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="mailingpreferences",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0011_invalidperson_newperson_synchronizationresult.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0011_invalidperson_newperson_synchronizationresult.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.4 on 2021-11-03 13:09
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0010_mailingpreferences_language"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="SynchronizationResult",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0012_auto_20211119_0830.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0012_auto_20211119_0830.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import django.db.models.deletion
 import django.db.models.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0011_invalidperson_newperson_synchronizationresult"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="SynchronizationPerson",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0013_mailingpreferences_latest_sync.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0013_mailingpreferences_latest_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 3.2.4 on 2021-11-19 12:42
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0012_auto_20211119_0830"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="mailingpreferences",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0017_auto_20211122_1219.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0017_auto_20211122_1219.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.4 on 2021-11-22 11:19
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0016_remove_synchronizationperson_successfully_added"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="synchronizationperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0018_alter_synchronizationperson_sync_status.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0018_alter_synchronizationperson_sync_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.4 on 2021-11-22 13:30
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0017_auto_20211122_1219"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="synchronizationperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0022_auto_20220118_1308.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0022_auto_20220118_1308.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.4 on 2022-01-18 12:08
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0021_auto_20220106_0917"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="subscription",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/migrations/0023_auto_20220517_1700.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/migrations/0023_auto_20220517_1700.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 3.2.4 on 2022-05-17 15:00
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
+
     dependencies = [
         ("mailer_integration", "0022_auto_20220118_1308"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="synchronizationperson",
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/models.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -91,15 +91,10 @@
     ]
     sync_status = models.CharField(
         _("Synchronization Status"),
         choices=SYNC_STATUS_CHOICES,
         max_length=255,
         blank=True,
     )
-    maybe_duplicate = models.BooleanField(
-        _("Possible duplicate"),
-        default=False,
-        help_text=_("Other person with same first and last name already exists"),
-    )
 
     def __str__(self):
         return self.email
```

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/urls.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/urls.py`

 * *Files identical despite different names*

### Comparing `basxconnect-0.4.61/basxconnect/mailer_integration/views.py` & `basxconnect-0.4.7/basxconnect/mailer_integration/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,61 +23,46 @@
 
 C = basxbread.layout.grid.Col
 R = basxbread.layout.grid.Row
 
 
 @aslayout
 def mailer_synchronization_view(request):
-    notifications = []
     if request.method == "POST":
         try:
             sync_result = synchronize(settings.MAILER)
-            notifications.append(
-                basxbread.layout.components.notification.InlineNotification(
-                    _("Sychronization successful"),
-                    _(
-                        "Synchronized with mailer segment containing %s contacts. %s new persons were added to BasxConnect."
-                    )
-                    % (
-                        sync_result.total_synchronized_persons,
-                        sync_result.persons.filter(
-                            sync_status=SynchronizationPerson.NEW
-                        ).count(),
-                    ),
-                    kind="success",
+            notification = basxbread.layout.components.notification.InlineNotification(
+                _("Sychronization successful"),
+                _(
+                    "Synchronized with mailer segment containing %s contacts. %s new persons were added to BasxConnect."
                 )
+                % (
+                    sync_result.total_synchronized_persons,
+                    sync_result.persons.filter(
+                        sync_status=SynchronizationPerson.NEW
+                    ).count(),
+                ),
+                kind="success",
             )
-            for person in sync_result.persons.all():
-                if person.maybe_duplicate:
-                    notifications.append(
-                        basxbread.layout.components.notification.InlineNotification(
-                            _("Possible duplicate"),
-                            _(
-                                f"New person '{person.first_name} {person.last_name}' might be "
-                                "a duplicate, there is another person with the same name."
-                            ),
-                            kind="warning",
-                        )
-                    )
         except Exception:
-            notifications.append(
-                basxbread.layout.components.notification.InlineNotification(
-                    _("Error"),
-                    f"An error occured during synchronization. {traceback.format_exc()}",
-                    kind="error",
-                )
+            notification = basxbread.layout.components.notification.InlineNotification(
+                "Error",
+                f"An error occured during synchronization. {traceback.format_exc()}",
+                kind="error",
             )
+    else:
+        notification = None
 
     help_modal = sync_help_modal()
     return hg.BaseElement(
         Form(
             forms.Form(),
             basxbread.layout.grid.Grid(
                 hg.H3(_("Synchronization of Email Subcriptions")),
-                hg.BaseElement(*notifications),
+                notification,
                 gutter=False,
             ),
             help_modal,
             layout.forms.helpers.Submit(
                 _("Download subscriptions"), style="display: inline-block;"
             ),
             layout.button.Button(
```

### Comparing `basxconnect-0.4.61/basxconnect.egg-info/PKG-INFO` & `basxconnect-0.4.7/basxconnect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 Metadata-Version: 2.1
 Name: basxconnect
-Version: 0.4.61
+Version: 0.4.7
 Summary: CRM application for non-profit organizations
 Home-page: https://github.com/basxsoftwareassociation/basxconnect
 Author: basx Software Association
 Author-email: sam@basx.dev
 License: New BSD License
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: basx-bread
-Requires-Dist: django-formtools==2.3
-Requires-Dist: djangorestframework
-Requires-Dist: chardet
-Requires-Dist: tablib
-Requires-Dist: dateparser
 Provides-Extra: testing
-Requires-Dist: basx-bread[testing]; extra == "testing"
 Provides-Extra: mailer-integration
-Requires-Dist: mailchimp_marketing; extra == "mailer-integration"
+License-File: LICENSE
 
 [![basxconnect-ci](https://github.com/basxsoftwareassociation/basxconnect/actions/workflows/main.yml/badge.svg)](https://github.com/basxsoftwareassociation/basxconnect/actions/workflows/main.yml)
 [![Translation status](https://hosted.weblate.org/widgets/basxconnect/-/svg-badge.svg)](https://hosted.weblate.org/engage/basxconnect/)
 
 basxconnect
 ===========
 
@@ -58,31 +51,26 @@
 What we have so far
 -------------------
 
 - Integration of the core parts of carbon design in django (*"like bootstrap for django"*)
 - CRUD-framework (*"Quick generation of create/read/update/delete views"*)
 - HTML-layout framework which allows a more flexible hooking-in than the standard HTML-rendering mechanisms (*"DOM on the server side"*)
 - Core model to manage people, communication and relationships
-- Additional modules for:
-  - Generating reports
-  - Generating documents and PDFs from word templates
-  - Custom add/edit forms
-  - Data import from PDFs with form-fields
-  - Customiable Database triggers to send notification emails
-  - Invoicing module
 - Demo project which implements a bare-bone version of a *product* (this repository)
 
 What we still need to do
 ------------------------
 
+- Adding a workflow engine which allows code-based configuration of manual and automated workflows (e.g. uploading a file, waiting for approval from a certain role, sending out an email automatically, etc.)
 - Improving the existing code base to have better support for extendability
 - Write documentation where necessary and add code-examples and how-to's
 - Implement revisions completely to allow going to a certain date and maybe display diffs
 
 Other TODOs:
 - Explain more why basxConnect is necessary and the difference to alternative solutions
 
 We would like to thank the following projects for their work, they provide a valuable base for basxConnect:
 
 - Translation: https://weblate.org/
 - Design System: https://www.carbondesignsystem.com/
 
+
```

### Comparing `basxconnect-0.4.61/basxconnect.egg-info/SOURCES.txt` & `basxconnect-0.4.7/basxconnect.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 basxconnect/contributions/locale/nb_NO/LC_MESSAGES/django.po
 basxconnect/contributions/locale/pt/LC_MESSAGES/django.po
 basxconnect/contributions/locale/th/LC_MESSAGES/django.po
 basxconnect/contributions/migrations/0001_initial.py
 basxconnect/contributions/migrations/0002_alter_contribution_currency.py
 basxconnect/contributions/migrations/0003_alter_contribution__import.py
 basxconnect/contributions/migrations/0004_auto_20211030_0955.py
-basxconnect/contributions/migrations/0005_alter_contribution_currency.py
 basxconnect/contributions/migrations/__init__.py
 basxconnect/contributions/wizards/__init__.py
 basxconnect/contributions/wizards/contributionsimport.py
 basxconnect/core/__init__.py
 basxconnect/core/apps.py
 basxconnect/core/context_processors.py
 basxconnect/core/dynamic_preferences_registry.py
 basxconnect/core/search_indexes.py
 basxconnect/core/settings.py
 basxconnect/core/urls.py
+basxconnect/core/fixtures/base.de.json
+basxconnect/core/fixtures/base.en.json
 basxconnect/core/layouts/__init__.py
 basxconnect/core/layouts/settings_layout.py
 basxconnect/core/layouts/editperson/__init__.py
 basxconnect/core/layouts/editperson/common/__init__.py
 basxconnect/core/layouts/editperson/common/addresses.py
 basxconnect/core/layouts/editperson/common/base_data.py
 basxconnect/core/layouts/editperson/common/contributions_tab.py
@@ -97,24 +98,21 @@
 basxconnect/core/migrations/0025_alter_term_slug.py
 basxconnect/core/migrations/0026_auto_20211216_0946.py
 basxconnect/core/migrations/0027_auto_20211223_1948.py
 basxconnect/core/migrations/0028_auto_20220404_1058.py
 basxconnect/core/migrations/0029_auto_20220429_1138.py
 basxconnect/core/migrations/0030_auto_20220602_1434.py
 basxconnect/core/migrations/0031_alter_email_person_alter_email_type_alter_fax_person_and_more.py
-basxconnect/core/migrations/0032_alter_historicallegalperson_options_and_more.py
-basxconnect/core/migrations/0033_historicalnaturalperson_maiden_name_and_more.py
-basxconnect/core/migrations/0034_term_disabled.py
-basxconnect/core/migrations/0035_alter_email_type_alter_fax_type_and_more.py
 basxconnect/core/migrations/__init__.py
 basxconnect/core/models/__init__.py
 basxconnect/core/models/addresses.py
 basxconnect/core/models/persons.py
 basxconnect/core/models/relationships.py
 basxconnect/core/models/utils.py
+basxconnect/core/static/logo.png
 basxconnect/core/tests/__init__.py
 basxconnect/core/tests/settings.py
 basxconnect/core/tests/test_person.py
 basxconnect/core/tests/urls.py
 basxconnect/core/views/__init__.py
 basxconnect/core/views/menu_views.py
 basxconnect/core/views/relationship_views.py
@@ -125,29 +123,14 @@
 basxconnect/core/views/person/__init__.py
 basxconnect/core/views/person/person_browse_views.py
 basxconnect/core/views/person/person_details_views.py
 basxconnect/core/views/person/person_modals_views.py
 basxconnect/core/views/person/search_person_view.py
 basxconnect/core/wizards/__init__.py
 basxconnect/core/wizards/add_person.py
-basxconnect/invoicing/__init__.py
-basxconnect/invoicing/apps.py
-basxconnect/invoicing/dynamic_preferences_registry.py
-basxconnect/invoicing/models.py
-basxconnect/invoicing/urls.py
-basxconnect/invoicing/views.py
-basxconnect/invoicing/locale/de/LC_MESSAGES/django.po
-basxconnect/invoicing/locale/fr/LC_MESSAGES/django.po
-basxconnect/invoicing/locale/nb_NO/LC_MESSAGES/django.po
-basxconnect/invoicing/locale/pt/LC_MESSAGES/django.po
-basxconnect/invoicing/locale/th/LC_MESSAGES/django.po
-basxconnect/invoicing/migrations/0001_initial.py
-basxconnect/invoicing/migrations/0002_alter_invoice_note.py
-basxconnect/invoicing/migrations/0003_invoice_receipt_sent.py
-basxconnect/invoicing/migrations/__init__.py
 basxconnect/mailer_integration/__init__.py
 basxconnect/mailer_integration/apps.py
 basxconnect/mailer_integration/dynamic_preferences_registry.py
 basxconnect/mailer_integration/help.py
 basxconnect/mailer_integration/layouts.py
 basxconnect/mailer_integration/models.py
 basxconnect/mailer_integration/settings.py
@@ -184,16 +167,8 @@
 basxconnect/mailer_integration/migrations/0017_auto_20211122_1219.py
 basxconnect/mailer_integration/migrations/0018_alter_synchronizationperson_sync_status.py
 basxconnect/mailer_integration/migrations/0019_auto_20211210_1602.py
 basxconnect/mailer_integration/migrations/0020_subscription_deleted.py
 basxconnect/mailer_integration/migrations/0021_auto_20220106_0917.py
 basxconnect/mailer_integration/migrations/0022_auto_20220118_1308.py
 basxconnect/mailer_integration/migrations/0023_auto_20220517_1700.py
-basxconnect/mailer_integration/migrations/0024_synchronizationperson_maybe_duplicate.py
-basxconnect/mailer_integration/migrations/__init__.py
-basxconnect/projects/__init__.py
-basxconnect/projects/apps.py
-basxconnect/projects/models.py
-basxconnect/projects/urls.py
-basxconnect/projects/migrations/0001_initial.py
-basxconnect/projects/migrations/0002_alter_project_client.py
-basxconnect/projects/migrations/__init__.py
+basxconnect/mailer_integration/migrations/__init__.py
```

### Comparing `basxconnect-0.4.61/manage.py` & `basxconnect-0.4.7/manage.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,16 +14,14 @@
         "django.contrib.contenttypes",
         "django.contrib.sites",
         "basxbread",
         "djmoney",
         "basxconnect.core",
         "basxconnect.contributions",
         "basxconnect.mailer_integration",
-        "basxconnect.invoicing",
-        "basxconnect.projects",
     ]
     settings.configure(
         DEBUG=True,
         USE_TZ=True,
         USE_I18N=True,
         DATABASES={
             "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"}
```

### Comparing `basxconnect-0.4.61/setup.py` & `basxconnect-0.4.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/basxsoftwareassociation/basxconnect",
     author="basx Software Association",
     author_email="sam@basx.dev",
     license="New BSD License",
     install_requires=[
         "basx-bread",
-        "django-formtools == 2.3",
+        "django-formtools",
         "djangorestframework",
         "chardet",
         "tablib",
         "dateparser",
     ],
     extras_require={
         "testing": ["basx-bread[testing]"],
```

