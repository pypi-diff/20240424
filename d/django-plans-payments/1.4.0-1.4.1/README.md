# Comparing `tmp/django-plans-payments-1.4.0.tar.gz` & `tmp/django-plans-payments-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plans-payments-1.4.0.tar", last modified: Mon Apr 15 13:57:15 2024, max compression
+gzip compressed data, was "django-plans-payments-1.4.1.tar", last modified: Wed Apr 24 07:16:55 2024, max compression
```

## Comparing `django-plans-payments-1.4.0.tar` & `django-plans-payments-1.4.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/
--rw-rw-r--   0 petr      (1000) petr      (1000)      207 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.235564 django-plans-payments-1.4.0/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      350 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.235564 django-plans-payments-1.4.0/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3278 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      452 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3330 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1640 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      182 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1557 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)     5313 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2790 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.235564 django-plans-payments-1.4.0/django_plans_payments.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     5313 2024-04-15 13:57:15.000000 django-plans-payments-1.4.0/django_plans_payments.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     1855 2024-04-15 13:57:15.000000 django-plans-payments-1.4.0/django_plans_payments.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-15 13:57:15.000000 django-plans-payments-1.4.0/django_plans_payments.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-15 13:57:15.000000 django-plans-payments-1.4.0/django_plans_payments.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       36 2024-04-15 13:57:15.000000 django-plans-payments-1.4.0/django_plans_payments.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       15 2024-04-15 13:57:15.000000 django-plans-payments-1.4.0/django_plans_payments.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.235564 django-plans-payments-1.4.0/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8443 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      452 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      678 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      191 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/mypy.ini
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.235564 django-plans-payments-1.4.0/plans_payments/
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1695 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      122 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/plans_payments/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4514 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      424 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/migrations/0002_payment_transaction_fee.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      716 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/migrations/0003_auto_20201006_0855.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      513 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/migrations/0004_payment_billing_phone.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      633 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/migrations/0005_payment_plans_payme_status_9ad17d_idx_and_more.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     9598 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.231565 django-plans-payments-1.4.0/plans_payments/static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/plans_payments/static/img/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3674 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/static/img/visa-logo.svg
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.231565 django-plans-payments-1.4.0/plans_payments/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/plans_payments/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)       49 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templates/mail/renew_cvv_3ds_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       36 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templates/mail/renew_cvv_3ds_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/plans_payments/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      197 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templates/plans/order_detail.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/plans_payments/templates/plans_payments/
--rw-rw-r--   0 petr      (1000) petr      (1000)       77 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templates/plans_payments/failure.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      217 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templates/plans_payments/payment.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      777 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templates/plans_payments/payment_buttons.html
--rw-rw-r--   0 petr      (1000) petr      (1000)       85 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templates/plans_payments/success.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/plans_payments/templatetags/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templatetags/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      353 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/templatetags/payment_buttons.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      385 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2714 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/plans_payments/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       93 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      187 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      325 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2402 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/setup.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1984 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/tests/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/tests/templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)       49 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/tests/templates/base.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:15.239564 django-plans-payments-1.4.0/tests/templates/registration/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/tests/templates/registration/login.html
--rw-rw-r--   0 petr      (1000) petr      (1000)    22760 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/tests/test_models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3522 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      345 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      758 2024-04-15 13:57:14.000000 django-plans-payments-1.4.0/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      207 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.353016 django-plans-payments-1.4.1/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      350 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.353016 django-plans-payments-1.4.1/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3278 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      452 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3330 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1760 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      182 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1557 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/Makefile
+-rw-r--r--   0 petr      (1000) petr      (1000)     5499 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2790 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/django_plans_payments.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     5499 2024-04-24 07:16:55.000000 django-plans-payments-1.4.1/django_plans_payments.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1855 2024-04-24 07:16:55.000000 django-plans-payments-1.4.1/django_plans_payments.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-24 07:16:55.000000 django-plans-payments-1.4.1/django_plans_payments.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-24 07:16:55.000000 django-plans-payments-1.4.1/django_plans_payments.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       36 2024-04-24 07:16:55.000000 django-plans-payments-1.4.1/django_plans_payments.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       15 2024-04-24 07:16:55.000000 django-plans-payments-1.4.1/django_plans_payments.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.353016 django-plans-payments-1.4.1/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8443 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      452 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      678 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      191 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/mypy.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.353016 django-plans-payments-1.4.1/plans_payments/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1695 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      122 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/plans_payments/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4514 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      424 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/migrations/0002_payment_transaction_fee.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      716 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/migrations/0003_auto_20201006_0855.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      513 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/migrations/0004_payment_billing_phone.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      633 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/migrations/0005_payment_plans_payme_status_9ad17d_idx_and_more.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8902 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.349015 django-plans-payments-1.4.1/plans_payments/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/plans_payments/static/img/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3674 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/static/img/visa-logo.svg
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.349015 django-plans-payments-1.4.1/plans_payments/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/plans_payments/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       49 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templates/mail/renew_cvv_3ds_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       36 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templates/mail/renew_cvv_3ds_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/plans_payments/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      197 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templates/plans/order_detail.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/plans_payments/templates/plans_payments/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       77 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templates/plans_payments/failure.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      217 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templates/plans_payments/payment.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      777 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templates/plans_payments/payment_buttons.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)       85 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templates/plans_payments/success.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/plans_payments/templatetags/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templatetags/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      353 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/templatetags/payment_buttons.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      385 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2714 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/plans_payments/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       93 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      187 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      325 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2402 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/setup.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1984 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/tests/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/tests/templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       49 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/tests/templates/base.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:55.357016 django-plans-payments-1.4.1/tests/templates/registration/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/tests/templates/registration/login.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)    21927 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3522 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      345 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      758 2024-04-24 07:16:54.000000 django-plans-payments-1.4.1/tox.ini
```

### Comparing `django-plans-payments-1.4.0/.github/workflows/main.yml` & `django-plans-payments-1.4.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/CONTRIBUTING.rst` & `django-plans-payments-1.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/HISTORY.rst` & `django-plans-payments-1.4.1/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+1.4.1 (2024-04-24)
+++++++++++++++++++
+
+* do not check whether a confirmed payment of a completed order is left anymore
+
 1.4.0 (2024-04-15)
 ++++++++++++++++++
 
 * migrate to `RecurringUserPlan.renewal_triggered_by`
 * add `renewal_triggered_by` parameter to `Payment.set_renew_token`
 * deprecate `automatic_renewal` parameter of `Payment.set_renew_token`; use `renewal_triggered_by` parameter instead
 * deprecate `None` value of `renewal_triggered_by` parameter of `Payment.set_renew_token`; set an `AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY` instead
```

### Comparing `django-plans-payments-1.4.0/LICENSE` & `django-plans-payments-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/Makefile` & `django-plans-payments-1.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/PKG-INFO` & `django-plans-payments-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans-payments
-Version: 1.4.0
+Version: 1.4.1
 Summary: Integration between django-plans and django-payments.
 Home-page: https://github.com/PetrDlouhy/django-plans-payments
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-plans-payments
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django-plans>=1.1.0
+Requires-Dist: django-payments
 
 =============================
 Django plans payments
 =============================
 
 .. image:: https://badge.fury.io/py/django-plans-payments.svg
     :target: https://badge.fury.io/py/django-plans-payments
@@ -113,14 +115,19 @@
 
 
 
 
 History
 -------
 
+1.4.1 (2024-04-24)
+++++++++++++++++++
+
+* do not check whether a confirmed payment of a completed order is left anymore
+
 1.4.0 (2024-04-15)
 ++++++++++++++++++
 
 * migrate to `RecurringUserPlan.renewal_triggered_by`
 * add `renewal_triggered_by` parameter to `Payment.set_renew_token`
 * deprecate `automatic_renewal` parameter of `Payment.set_renew_token`; use `renewal_triggered_by` parameter instead
 * deprecate `None` value of `renewal_triggered_by` parameter of `Payment.set_renew_token`; set an `AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY` instead
```

### Comparing `django-plans-payments-1.4.0/README.rst` & `django-plans-payments-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/django_plans_payments.egg-info/PKG-INFO` & `django-plans-payments-1.4.1/django_plans_payments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans-payments
-Version: 1.4.0
+Version: 1.4.1
 Summary: Integration between django-plans and django-payments.
 Home-page: https://github.com/PetrDlouhy/django-plans-payments
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-plans-payments
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django-plans>=1.1.0
+Requires-Dist: django-payments
 
 =============================
 Django plans payments
 =============================
 
 .. image:: https://badge.fury.io/py/django-plans-payments.svg
     :target: https://badge.fury.io/py/django-plans-payments
@@ -113,14 +115,19 @@
 
 
 
 
 History
 -------
 
+1.4.1 (2024-04-24)
+++++++++++++++++++
+
+* do not check whether a confirmed payment of a completed order is left anymore
+
 1.4.0 (2024-04-15)
 ++++++++++++++++++
 
 * migrate to `RecurringUserPlan.renewal_triggered_by`
 * add `renewal_triggered_by` parameter to `Payment.set_renew_token`
 * deprecate `automatic_renewal` parameter of `Payment.set_renew_token`; use `renewal_triggered_by` parameter instead
 * deprecate `None` value of `renewal_triggered_by` parameter of `Payment.set_renew_token`; set an `AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY` instead
```

### Comparing `django-plans-payments-1.4.0/django_plans_payments.egg-info/SOURCES.txt` & `django-plans-payments-1.4.1/django_plans_payments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/docs/Makefile` & `django-plans-payments-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/docs/conf.py` & `django-plans-payments-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/docs/make.bat` & `django-plans-payments-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/docs/usage.rst` & `django-plans-payments-1.4.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/plans_payments/admin.py` & `django-plans-payments-1.4.1/plans_payments/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/plans_payments/migrations/0001_initial.py` & `django-plans-payments-1.4.1/plans_payments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/plans_payments/migrations/0003_auto_20201006_0855.py` & `django-plans-payments-1.4.1/plans_payments/migrations/0003_auto_20201006_0855.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/plans_payments/migrations/0004_payment_billing_phone.py` & `django-plans-payments-1.4.1/plans_payments/migrations/0004_payment_billing_phone.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/plans_payments/migrations/0005_payment_plans_payme_status_9ad17d_idx_and_more.py` & `django-plans-payments-1.4.1/plans_payments/migrations/0005_payment_plans_payme_status_9ad17d_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/plans_payments/models.py` & `django-plans-payments-1.4.1/plans_payments/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import warnings
 from decimal import Decimal
 from urllib.parse import urljoin
 
 from django.conf import settings
-from django.core.exceptions import ObjectDoesNotExist, ValidationError
+from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.dispatch.dispatcher import receiver
 from django.urls import reverse
 from payments import PaymentStatus, PurchasedItem
 from payments.core import get_base_url
 from payments.models import BasePayment
 from payments.signals import status_changed
@@ -41,28 +41,14 @@
 
     class Meta:
         indexes = [
             models.Index(fields=["status"]),
             models.Index(fields=["status", "transaction_id"]),
         ]
 
-    def clean(self):
-        if self.order.status == Order.STATUS.COMPLETED:
-            confirmed_payment_count = self.order.payment_set.exclude(pk=self.pk)
-            confirmed_payment_count = confirmed_payment_count.filter(
-                status=PaymentStatus.CONFIRMED
-            ).count()
-            if self.status != PaymentStatus.CONFIRMED and confirmed_payment_count == 0:
-                raise ValidationError(
-                    {
-                        "status": "Can't leave confirmed order without any confirmed payment. "
-                        "Please change Order first if you still want to perform this change.",
-                    },
-                )
-
     def save(self, **kwargs):
         if "payu" in self.variant:
             # TODO: base this on actual payment methods and currency fees on PayU
             # or even better on real PayU info
             self.transaction_fee = self.total * Decimal("0.029") + Decimal("0.05")
         elif hasattr(self, "extra_data") and self.extra_data:
             extra_data = json.loads(self.extra_data)
```

### Comparing `django-plans-payments-1.4.0/plans_payments/static/img/visa-logo.svg` & `django-plans-payments-1.4.1/plans_payments/static/img/visa-logo.svg`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/plans_payments/templates/plans_payments/payment_buttons.html` & `django-plans-payments-1.4.1/plans_payments/templates/plans_payments/payment_buttons.html`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/plans_payments/views.py` & `django-plans-payments-1.4.1/plans_payments/views.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/runtests.py` & `django-plans-payments-1.4.1/runtests.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/setup.py` & `django-plans-payments-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/tests/settings.py` & `django-plans-payments-1.4.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/tests/test_models.py` & `django-plans-payments-1.4.1/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,38 +22,14 @@
 from plans_payments import models
 
 
 class TestPlansPayments(TestCase):
     def setUp(self):
         pass
 
-    def test_clean(self):
-        p = models.Payment(order=baker.make("Order", status=Order.STATUS.NEW))
-        p.clean()
-        self.assertEqual(p.status, "waiting")
-
-    def test_clean_completed(self):
-        p = models.Payment(
-            order=baker.make("Order", status=Order.STATUS.COMPLETED),
-            status=PaymentStatus.CONFIRMED,
-        )
-        p.clean()
-        self.assertEqual(p.status, "confirmed")
-
-    def test_clean_completed_no_confirmed_payment(self):
-        p = models.Payment(
-            order=baker.make("Order", status=Order.STATUS.COMPLETED),
-            status=PaymentStatus.WAITING,
-        )
-        with self.assertRaisesRegex(
-            Exception, "Can't leave confirmed order without any confirmed payment."
-        ):
-            p.clean()
-        self.assertEqual(p.status, "waiting")
-
     def test_save(self):
         p = models.Payment(transaction_fee=1)
         p.save()
         rp = models.Payment.objects.get()
         self.assertEqual(rp.transaction_fee, 1)
 
     def test_save_extra_data(self):
```

### Comparing `django-plans-payments-1.4.0/tests/test_views.py` & `django-plans-payments-1.4.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.4.0/tox.ini` & `django-plans-payments-1.4.1/tox.ini`

 * *Files identical despite different names*

