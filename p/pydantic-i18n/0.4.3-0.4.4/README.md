# Comparing `tmp/pydantic_i18n-0.4.3.tar.gz` & `tmp/pydantic_i18n-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_i18n-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pydantic_i18n-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pydantic_i18n-0.4.3.tar` & `pydantic_i18n-0.4.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0      459 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.coveragerc
--rw-r--r--   0        0        0      291 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.editorconfig
--rw-r--r--   0        0        0      577 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       27 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      445 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      115 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/actions/comment-docs-preview-in-pr/Dockerfile
--rw-r--r--   0        0        0      386 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/actions/comment-docs-preview-in-pr/README.md
--rw-r--r--   0        0        0      396 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/actions/comment-docs-preview-in-pr/action.yml
--rw-r--r--   0        0        0     2096 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/actions/comment-docs-preview-in-pr/app/main.py
--rw-r--r--   0        0        0      429 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1542 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0      561 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      530 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/workflows/new_contributor_pr.yml
--rw-r--r--   0        0        0     1196 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/workflows/preview-docs.yml
--rw-r--r--   0        0        0      829 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1105 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1833 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/.gitignore
--rw-r--r--   0        0        0     1077 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/LICENSE
--rw-r--r--   0        0        0    17420 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/README.md
--rw-r--r--   0        0        0        0 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/data/.gitignore
--rw-r--r--   0        0        0    14738 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/contributing.md
--rw-r--r--   0        0        0      302 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/css/termynal.css
--rw-r--r--   0        0        0     2757 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/help-pydantic-i18n.md
--rw-r--r--   0        0        0      399 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/img/favicon.png
--rw-r--r--   0        0        0     2918 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/img/icon-white.png
--rw-r--r--   0        0        0    18203 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/img/logo-white.png
--rw-r--r--   0        0        0    13894 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/img/logo-white.svg
--rw-r--r--   0        0        0    11162 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/index.md
--rw-r--r--   0        0        0     4357 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/js/termynal.js
--rw-r--r--   0        0        0    14760 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/docs/release-notes.md
--rw-r--r--   0        0        0     1782 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/mkdocs.yml
--rw-r--r--   0        0        0      295 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/en/overrides/main.html
--rw-r--r--   0        0        0      220 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs/missing-translation.md
--rw-r--r--   0        0        0      498 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/babel-loader/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      714 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/babel-loader/translations/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      495 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/babel-loader/translations/en_US/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      718 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/babel-loader/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      470 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/babel-loader/tutorial001.py
--rw-r--r--   0        0        0      583 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/dict-loader/tutorial001.py
--rw-r--r--   0        0        0      418 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/fastapi-usage/main.py
--rw-r--r--   0        0        0      909 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/fastapi-usage/tr.py
--rw-r--r--   0        0        0       46 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/json-loader/translations/de_DE.json
--rw-r--r--   0        0        0       43 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/json-loader/translations/en_US.json
--rw-r--r--   0        0        0      471 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/json-loader/tutorial001.py
--rw-r--r--   0        0        0       33 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/own-loader/translations/de_DE.csv
--rw-r--r--   0        0        0       30 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/own-loader/translations/en_US.csv
--rw-r--r--   0        0        0     1118 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/own-loader/tutorial001.py
--rw-r--r--   0        0        0     1302 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/placeholder/tutorial001.py
--rw-r--r--   0        0        0      470 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/pydantic-messages/tutorial001.py
--rw-r--r--   0        0        0      570 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v1/pydantic-messages/tutorial002.py
--rw-r--r--   0        0        0      509 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/babel-loader/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      714 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/babel-loader/translations/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      506 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/babel-loader/translations/en_US/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      718 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/babel-loader/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      559 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/babel-loader/tutorial001.py
--rw-r--r--   0        0        0      669 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/dict-loader/tutorial001.py
--rw-r--r--   0        0        0      418 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/fastapi-usage/main.py
--rw-r--r--   0        0        0      909 2024-03-16 23:20:05.896307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/fastapi-usage/tr.py
--rw-r--r--   0        0        0       46 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/json-loader/translations/de_DE.json
--rw-r--r--   0        0        0       43 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/json-loader/translations/en_US.json
--rw-r--r--   0        0        0      576 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/json-loader/tutorial001.py
--rw-r--r--   0        0        0       33 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/own-loader/translations/de_DE.csv
--rw-r--r--   0        0        0       30 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/own-loader/translations/en_US.csv
--rw-r--r--   0        0        0     1223 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/own-loader/tutorial001.py
--rw-r--r--   0        0        0     1045 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/placeholder/tutorial001.py
--rw-r--r--   0        0        0      514 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/pydantic-messages/tutorial001.py
--rw-r--r--   0        0        0      534 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/docs_src/pydantic_v2/pydantic-messages/tutorial002.py
--rw-r--r--   0        0        0      402 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/mypy.ini
--rw-r--r--   0        0        0      396 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/pydantic_i18n/__init__.py
--rw-r--r--   0        0        0     2680 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/pydantic_i18n/loaders.py
--rw-r--r--   0        0        0     5024 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/pydantic_i18n/main.py
--rw-r--r--   0        0        0        0 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/pydantic_i18n/py.typed
--rw-r--r--   0        0        0     1959 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       71 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/build-docs.sh
--rw-r--r--   0        0        0       98 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/clean.sh
--rw-r--r--   0        0        0       66 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/docs-live.sh
--rw-r--r--   0        0        0    13705 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/docs.py
--rw-r--r--   0        0        0      174 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/format-imports.sh
--rw-r--r--   0        0        0      226 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/format.sh
--rw-r--r--   0        0        0      163 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/lint.sh
--rw-r--r--   0        0        0       42 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/publish.sh
--rw-r--r--   0        0        0       80 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/test-cov-html.sh
--rw-r--r--   0        0        0      152 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/test.sh
--rw-r--r--   0        0        0      108 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/scripts/zip-docs.sh
--rw-r--r--   0        0        0      362 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/setup.cfg
--rw-r--r--   0        0        0        0 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0      321 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/test_loaders/__init__.py
--rw-r--r--   0        0        0     1157 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/test_loaders/conftest.py
--rw-r--r--   0        0        0      198 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/test_loaders/test_babel_loader.py
--rw-r--r--   0        0        0     1845 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/test_loaders/test_common.py
--rw-r--r--   0        0        0      449 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/test_loaders/test_json_loader.py
--rw-r--r--   0        0        0     7740 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/test_main.py
--rw-r--r--   0        0        0     1519 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/test_pydantic_messages.py
--rw-r--r--   0        0        0      498 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/translations/babel/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      714 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/translations/babel/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      575 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/translations/babel/en_US/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      798 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/translations/babel/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      571 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/translations/babel/es_AR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      794 2024-03-16 23:20:05.900307 pydantic_i18n-0.4.3/tests/translations/babel/es_AR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    19799 1970-01-01 00:00:00.000000 pydantic_i18n-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      459 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.coveragerc
+-rw-r--r--   0        0        0      291 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.editorconfig
+-rw-r--r--   0        0        0      577 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       27 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      445 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      115 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/actions/comment-docs-preview-in-pr/Dockerfile
+-rw-r--r--   0        0        0      386 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/actions/comment-docs-preview-in-pr/README.md
+-rw-r--r--   0        0        0      396 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/actions/comment-docs-preview-in-pr/action.yml
+-rw-r--r--   0        0        0     2096 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/actions/comment-docs-preview-in-pr/app/main.py
+-rw-r--r--   0        0        0      429 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1542 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0      561 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      530 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/workflows/new_contributor_pr.yml
+-rw-r--r--   0        0        0     1196 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/workflows/preview-docs.yml
+-rw-r--r--   0        0        0      829 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1105 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1833 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1077 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/LICENSE
+-rw-r--r--   0        0        0    17420 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/data/.gitignore
+-rw-r--r--   0        0        0    14738 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/contributing.md
+-rw-r--r--   0        0        0      302 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/css/termynal.css
+-rw-r--r--   0        0        0     2757 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/help-pydantic-i18n.md
+-rw-r--r--   0        0        0      399 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/img/favicon.png
+-rw-r--r--   0        0        0     2918 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/img/icon-white.png
+-rw-r--r--   0        0        0    18203 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/img/logo-white.png
+-rw-r--r--   0        0        0    13894 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/img/logo-white.svg
+-rw-r--r--   0        0        0    11162 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/index.md
+-rw-r--r--   0        0        0     4357 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/js/termynal.js
+-rw-r--r--   0        0        0    17984 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/docs/release-notes.md
+-rw-r--r--   0        0        0     1782 2024-04-24 07:09:37.627555 pydantic_i18n-0.4.4/docs/en/mkdocs.yml
+-rw-r--r--   0        0        0      295 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs/en/overrides/main.html
+-rw-r--r--   0        0        0      220 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs/missing-translation.md
+-rw-r--r--   0        0        0      498 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/babel-loader/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      714 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/babel-loader/translations/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      495 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/babel-loader/translations/en_US/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      718 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/babel-loader/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      470 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/babel-loader/tutorial001.py
+-rw-r--r--   0        0        0      583 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/dict-loader/tutorial001.py
+-rw-r--r--   0        0        0      418 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/fastapi-usage/main.py
+-rw-r--r--   0        0        0      909 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/fastapi-usage/tr.py
+-rw-r--r--   0        0        0       46 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/json-loader/translations/de_DE.json
+-rw-r--r--   0        0        0       43 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/json-loader/translations/en_US.json
+-rw-r--r--   0        0        0      471 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/json-loader/tutorial001.py
+-rw-r--r--   0        0        0       33 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/own-loader/translations/de_DE.csv
+-rw-r--r--   0        0        0       30 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/own-loader/translations/en_US.csv
+-rw-r--r--   0        0        0     1118 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/own-loader/tutorial001.py
+-rw-r--r--   0        0        0     1302 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/placeholder/tutorial001.py
+-rw-r--r--   0        0        0      470 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/pydantic-messages/tutorial001.py
+-rw-r--r--   0        0        0      570 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v1/pydantic-messages/tutorial002.py
+-rw-r--r--   0        0        0      509 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/babel-loader/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      714 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/babel-loader/translations/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      506 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/babel-loader/translations/en_US/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      718 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/babel-loader/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      559 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/babel-loader/tutorial001.py
+-rw-r--r--   0        0        0      669 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/dict-loader/tutorial001.py
+-rw-r--r--   0        0        0      418 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/fastapi-usage/main.py
+-rw-r--r--   0        0        0      909 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/fastapi-usage/tr.py
+-rw-r--r--   0        0        0       46 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/json-loader/translations/de_DE.json
+-rw-r--r--   0        0        0       43 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/json-loader/translations/en_US.json
+-rw-r--r--   0        0        0      576 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/json-loader/tutorial001.py
+-rw-r--r--   0        0        0       33 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/own-loader/translations/de_DE.csv
+-rw-r--r--   0        0        0       30 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/own-loader/translations/en_US.csv
+-rw-r--r--   0        0        0     1223 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/own-loader/tutorial001.py
+-rw-r--r--   0        0        0     1045 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/placeholder/tutorial001.py
+-rw-r--r--   0        0        0      514 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/pydantic-messages/tutorial001.py
+-rw-r--r--   0        0        0      534 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/docs_src/pydantic_v2/pydantic-messages/tutorial002.py
+-rw-r--r--   0        0        0      402 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/mypy.ini
+-rw-r--r--   0        0        0      396 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/pydantic_i18n/__init__.py
+-rw-r--r--   0        0        0     2784 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/pydantic_i18n/loaders.py
+-rw-r--r--   0        0        0     5024 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/pydantic_i18n/main.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/pydantic_i18n/py.typed
+-rw-r--r--   0        0        0     1958 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0       71 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/build-docs.sh
+-rw-r--r--   0        0        0       98 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/clean.sh
+-rw-r--r--   0        0        0       66 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/docs-live.sh
+-rw-r--r--   0        0        0    13705 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/docs.py
+-rw-r--r--   0        0        0      174 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/format-imports.sh
+-rw-r--r--   0        0        0      226 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/format.sh
+-rw-r--r--   0        0        0      163 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/lint.sh
+-rw-r--r--   0        0        0       42 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/publish.sh
+-rw-r--r--   0        0        0       80 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/test-cov-html.sh
+-rw-r--r--   0        0        0      152 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/test.sh
+-rw-r--r--   0        0        0      108 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/scripts/zip-docs.sh
+-rw-r--r--   0        0        0      362 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/setup.cfg
+-rw-r--r--   0        0        0        0 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0      321 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/test_loaders/__init__.py
+-rw-r--r--   0        0        0     1157 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/test_loaders/conftest.py
+-rw-r--r--   0        0        0      198 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/test_loaders/test_babel_loader.py
+-rw-r--r--   0        0        0     1845 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/test_loaders/test_common.py
+-rw-r--r--   0        0        0      449 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/test_loaders/test_json_loader.py
+-rw-r--r--   0        0        0     7740 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/test_main.py
+-rw-r--r--   0        0        0     1519 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/test_pydantic_messages.py
+-rw-r--r--   0        0        0      498 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/translations/babel/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      714 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/translations/babel/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      575 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/translations/babel/en_US/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      798 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/translations/babel/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      571 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/translations/babel/es_AR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      794 2024-04-24 07:09:37.631554 pydantic_i18n-0.4.4/tests/translations/babel/es_AR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    19798 1970-01-01 00:00:00.000000 pydantic_i18n-0.4.4/PKG-INFO
```

### Comparing `pydantic_i18n-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `pydantic_i18n-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/.github/actions/comment-docs-preview-in-pr/app/main.py` & `pydantic_i18n-0.4.4/.github/actions/comment-docs-preview-in-pr/app/main.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/.github/workflows/build-docs.yml` & `pydantic_i18n-0.4.4/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/.github/workflows/latest-changes.yml` & `pydantic_i18n-0.4.4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/.github/workflows/new_contributor_pr.yml` & `pydantic_i18n-0.4.4/.github/workflows/new_contributor_pr.yml`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/.github/workflows/preview-docs.yml` & `pydantic_i18n-0.4.4/.github/workflows/preview-docs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
 
       - name: Download Artifact Docs
-        uses: dawidd6/action-download-artifact@v3.1.2
+        uses: dawidd6/action-download-artifact@v3.1.4
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           workflow: build-docs.yml
           run_id: ${{ github.event.workflow_run.id }}
           name: docs-zip
 
       - name: Unzip docs
```

### Comparing `pydantic_i18n-0.4.3/.github/workflows/publish.yml` & `pydantic_i18n-0.4.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/.github/workflows/test.yml` & `pydantic_i18n-0.4.4/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
       - name: Lint
         run: bash ./scripts/lint.sh
 
       - name: Test
         run: bash ./scripts/test.sh
 
       - name: Upload coverage
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.0
```

### Comparing `pydantic_i18n-0.4.3/.gitignore` & `pydantic_i18n-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/LICENSE` & `pydantic_i18n-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/README.md` & `pydantic_i18n-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/contributing.md` & `pydantic_i18n-0.4.4/docs/en/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/css/termynal.css` & `pydantic_i18n-0.4.4/docs/en/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/help-pydantic-i18n.md` & `pydantic_i18n-0.4.4/docs/en/docs/help-pydantic-i18n.md`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/img/icon-white.png` & `pydantic_i18n-0.4.4/docs/en/docs/img/icon-white.png`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/img/logo-white.png` & `pydantic_i18n-0.4.4/docs/en/docs/img/logo-white.png`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/img/logo-white.svg` & `pydantic_i18n-0.4.4/docs/en/docs/img/logo-white.svg`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/index.md` & `pydantic_i18n-0.4.4/docs/en/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/js/custom.js` & `pydantic_i18n-0.4.4/docs/en/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/js/termynal.js` & `pydantic_i18n-0.4.4/docs/en/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs/en/docs/release-notes.md` & `pydantic_i18n-0.4.4/docs/en/docs/release-notes.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 # Release Notes
 
 ## Latest Changes
 
+## 0.4.4
+
+### Features
+
+* 🐛 Add encoding option to JsonLoader. PR [#252](https://github.com/boardpack/pydantic-i18n/pull/252) by [@dukkee](https://github.com/dukkee).
+
+### Internal
+
+* ⬆ Bump mkdocs-material from 9.5.17 to 9.5.18. PR [#250](https://github.com/boardpack/pydantic-i18n/pull/250) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump codecov/codecov-action from 4.2.0 to 4.3.0. PR [#248](https://github.com/boardpack/pydantic-i18n/pull/248) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump black from 24.3.0 to 24.4.0. PR [#247](https://github.com/boardpack/pydantic-i18n/pull/247) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump typer from 0.12.2 to 0.12.3. PR [#246](https://github.com/boardpack/pydantic-i18n/pull/246) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump codecov/codecov-action from 4.1.1 to 4.2.0. PR [#243](https://github.com/boardpack/pydantic-i18n/pull/243) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump mkdocs-material from 9.5.16 to 9.5.17. PR [#244](https://github.com/boardpack/pydantic-i18n/pull/244) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump typer from 0.12.0 to 0.12.2. PR [#245](https://github.com/boardpack/pydantic-i18n/pull/245) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump codecov/codecov-action from 4.1.0 to 4.1.1. PR [#240](https://github.com/boardpack/pydantic-i18n/pull/240) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump mkdocs-material from 9.5.15 to 9.5.16. PR [#241](https://github.com/boardpack/pydantic-i18n/pull/241) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump typer from 0.10.0 to 0.12.0. PR [#242](https://github.com/boardpack/pydantic-i18n/pull/242) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump pytest-cov from 4.1.0 to 5.0.0. PR [#239](https://github.com/boardpack/pydantic-i18n/pull/239) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump typer from 0.9.0 to 0.10.0. PR [#237](https://github.com/boardpack/pydantic-i18n/pull/237) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump mkdocs-material from 9.5.14 to 9.5.15. PR [#238](https://github.com/boardpack/pydantic-i18n/pull/238) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump mkdocs-material from 9.5.13 to 9.5.14. PR [#233](https://github.com/boardpack/pydantic-i18n/pull/233) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump black from 24.2.0 to 24.3.0. PR [#235](https://github.com/boardpack/pydantic-i18n/pull/235) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump autoflake from 2.3.0 to 2.3.1. PR [#234](https://github.com/boardpack/pydantic-i18n/pull/234) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump markdown from 3.5.2 to 3.6. PR [#232](https://github.com/boardpack/pydantic-i18n/pull/232) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump dawidd6/action-download-artifact from 3.1.2 to 3.1.4. PR [#236](https://github.com/boardpack/pydantic-i18n/pull/236) by [@dependabot[bot]](https://github.com/apps/dependabot).
 
 ## 0.4.3
 
 ### Fixes
 
 * ⬆ Update docs examples for the usage with Pydantic 2+. PR [#231](https://github.com/boardpack/pydantic-i18n/pull/231) by [@dukkee](https://github.com/dukkee).
 * 🐛 Fix the error messages source for the Pydantic 2. PR [#229](https://github.com/boardpack/pydantic-i18n/pull/229) by [@dukkee](https://github.com/dukkee).
```

### Comparing `pydantic_i18n-0.4.3/docs/en/mkdocs.yml` & `pydantic_i18n-0.4.4/docs/en/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v1/babel-loader/translations/de_DE/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.4/docs_src/pydantic_v1/babel-loader/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v1/babel-loader/translations/en_US/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.4/docs_src/pydantic_v1/babel-loader/translations/en_US/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v1/dict-loader/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v1/dict-loader/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v1/fastapi-usage/tr.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v1/fastapi-usage/tr.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v1/own-loader/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v1/own-loader/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v1/placeholder/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v1/placeholder/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v1/pydantic-messages/tutorial002.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v1/pydantic-messages/tutorial002.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/babel-loader/translations/de_DE/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/babel-loader/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/babel-loader/translations/en_US/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/babel-loader/translations/en_US/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/babel-loader/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/babel-loader/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/dict-loader/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/dict-loader/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/fastapi-usage/tr.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/fastapi-usage/tr.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/json-loader/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/json-loader/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/own-loader/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/own-loader/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/placeholder/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/placeholder/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/pydantic-messages/tutorial001.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/pydantic-messages/tutorial001.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/docs_src/pydantic_v2/pydantic-messages/tutorial002.py` & `pydantic_i18n-0.4.4/docs_src/pydantic_v2/pydantic-messages/tutorial002.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/pydantic_i18n/loaders.py` & `pydantic_i18n-0.4.4/pydantic_i18n/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,33 +36,36 @@
         return locales
 
     def get_translations(self, locale: str) -> Mapping[str, str]:
         return self.data[locale]
 
 
 class JsonLoader(BaseLoader):
-    def __init__(self, directory: str):
+    def __init__(self, directory: str, encoding: str = "utf-8"):
         if not os.path.exists(directory):
             raise OSError(f"Directory '{directory}' doesn't exist.")
         if not os.path.isdir(directory):
             raise OSError(f"'{directory}' is not a directory.")
 
         self.directory = directory
+        self.encoding = encoding
 
     @property
     def locales(self) -> Sequence[str]:
         locales: Sequence[str] = [
             filename[:-5]
             for filename in os.listdir(self.directory)
             if filename.endswith(".json")
         ]
         return locales
 
     def get_translations(self, locale: str) -> Mapping[str, str]:
-        with open(os.path.join(self.directory, f"{locale}.json")) as fp:
+        with open(
+            os.path.join(self.directory, f"{locale}.json"), encoding=self.encoding
+        ) as fp:
             data: Dict[str, str] = json.load(fp)
 
         return data
 
 
 class BabelLoader(BaseLoader):
     def __init__(self, translations_directory: str):
```

### Comparing `pydantic_i18n-0.4.3/pydantic_i18n/main.py` & `pydantic_i18n-0.4.4/pydantic_i18n/main.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/pyproject.toml` & `pydantic_i18n-0.4.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -42,33 +42,33 @@
 Documentation = "https://pydantic-i18n.boardpack.org"
 Source = "https://github.com/boardpack/pydantic-i18n"
 
 [project.optional-dependencies]
 test = [
     "pydantic >=2",
     "pytest ==7.4.3",
-    "pytest-cov ==4.1.0",
+    "pytest-cov ==5.0.0",
     "pytest-lazy-fixture ==0.6.3",
     "mypy ==1.9.0",
     "flake8 ==7.0.0",
-    "black ==24.2.0",
+    "black ==24.4.0",
     "isort ==5.13.2",
     "babel ==2.14.0",
 ]
 dev = [
-    "autoflake ==2.3.0",
+    "autoflake ==2.3.1",
     "flake8 ==7.0.0",
     "pre-commit",
 ]
 doc = [
     "mkdocs ==1.5.3",
-    "mkdocs-material ==9.5.13",
-    "markdown ==3.5.2",
+    "mkdocs-material ==9.5.18",
+    "markdown ==3.6",
     "markdown-include ==0.8.1",
     "mkdocs-markdownextradata-plugin ==0.2.5",
-    "typer ==0.9.0",
+    "typer ==0.12.3",
     "pyyaml ==6.0.1",
 ]
 
 [tool.isort]
 profile = "black"
 known_first_party = ["pydantic_i18n", "pydantic", "babel"]
```

### Comparing `pydantic_i18n-0.4.3/scripts/docs.py` & `pydantic_i18n-0.4.4/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/test_loaders/conftest.py` & `pydantic_i18n-0.4.4/tests/test_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/test_loaders/test_common.py` & `pydantic_i18n-0.4.4/tests/test_loaders/test_common.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/test_main.py` & `pydantic_i18n-0.4.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/test_pydantic_messages.py` & `pydantic_i18n-0.4.4/tests/test_pydantic_messages.py`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/translations/babel/de_DE/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.4/tests/translations/babel/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/translations/babel/en_US/LC_MESSAGES/messages.mo` & `pydantic_i18n-0.4.4/tests/translations/babel/en_US/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/translations/babel/en_US/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.4/tests/translations/babel/en_US/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/translations/babel/es_AR/LC_MESSAGES/messages.mo` & `pydantic_i18n-0.4.4/tests/translations/babel/es_AR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/tests/translations/babel/es_AR/LC_MESSAGES/messages.po` & `pydantic_i18n-0.4.4/tests/translations/babel/es_AR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pydantic_i18n-0.4.3/PKG-INFO` & `pydantic_i18n-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-i18n
-Version: 0.4.3
+Version: 0.4.4
 Summary: pydantic-i18n is an extension to support an i18n for the pydantic error messages.
 Author-email: Roman Sadzhenytsia <urchin.dukkee@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -21,31 +21,31 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic >=1.9.0
-Requires-Dist: autoflake ==2.3.0 ; extra == "dev"
+Requires-Dist: autoflake ==2.3.1 ; extra == "dev"
 Requires-Dist: flake8 ==7.0.0 ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ==1.5.3 ; extra == "doc"
-Requires-Dist: mkdocs-material ==9.5.13 ; extra == "doc"
-Requires-Dist: markdown ==3.5.2 ; extra == "doc"
+Requires-Dist: mkdocs-material ==9.5.18 ; extra == "doc"
+Requires-Dist: markdown ==3.6 ; extra == "doc"
 Requires-Dist: markdown-include ==0.8.1 ; extra == "doc"
 Requires-Dist: mkdocs-markdownextradata-plugin ==0.2.5 ; extra == "doc"
-Requires-Dist: typer ==0.9.0 ; extra == "doc"
+Requires-Dist: typer ==0.12.3 ; extra == "doc"
 Requires-Dist: pyyaml ==6.0.1 ; extra == "doc"
 Requires-Dist: pydantic >=2 ; extra == "test"
 Requires-Dist: pytest ==7.4.3 ; extra == "test"
-Requires-Dist: pytest-cov ==4.1.0 ; extra == "test"
+Requires-Dist: pytest-cov ==5.0.0 ; extra == "test"
 Requires-Dist: pytest-lazy-fixture ==0.6.3 ; extra == "test"
 Requires-Dist: mypy ==1.9.0 ; extra == "test"
 Requires-Dist: flake8 ==7.0.0 ; extra == "test"
-Requires-Dist: black ==24.2.0 ; extra == "test"
+Requires-Dist: black ==24.4.0 ; extra == "test"
 Requires-Dist: isort ==5.13.2 ; extra == "test"
 Requires-Dist: babel ==2.14.0 ; extra == "test"
 Project-URL: Documentation, https://pydantic-i18n.boardpack.org
 Project-URL: Source, https://github.com/boardpack/pydantic-i18n
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
```

