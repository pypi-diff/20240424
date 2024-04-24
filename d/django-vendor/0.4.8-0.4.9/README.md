# Comparing `tmp/django-vendor-0.4.8.tar.gz` & `tmp/django-vendor-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vendor-0.4.8.tar", last modified: Tue Aug 22 17:52:35 2023, max compression
+gzip compressed data, was "django-vendor-0.4.9.tar", last modified: Wed Aug 23 18:00:26 2023, max compression
```

## Comparing `django-vendor-0.4.8.tar` & `django-vendor-0.4.9.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.380343 django-vendor-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-22 17:52:35.380343 django-vendor-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-22 17:51:17.000000 django-vendor-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-22 17:51:17.000000 django-vendor-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-22 17:52:35.380343 django-vendor-0.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.356343 django-vendor-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.360343 django-vendor-0.4.8/src/django_vendor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-22 17:52:35.000000 django-vendor-0.4.8/src/django_vendor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-08-22 17:52:35.000000 django-vendor-0.4.8/src/django_vendor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-22 17:52:35.000000 django-vendor-0.4.8/src/django_vendor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-22 17:52:35.000000 django-vendor-0.4.8/src/django_vendor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-22 17:52:35.000000 django-vendor-0.4.8/src/django_vendor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.360343 django-vendor-0.4.8/src/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.360343 django-vendor-0.4.8/src/vendor/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.360343 django-vendor-0.4.8/src/vendor/api/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.360343 django-vendor-0.4.8/src/vendor/api/v1/authorizenet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/api/v1/authorizenet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/api/v1/authorizenet/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.364343 django-vendor-0.4.8/src/vendor/api/v1/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/api/v1/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/api/v1/stripe/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.364343 django-vendor-0.4.8/src/vendor/encrypt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/encrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/encrypt/cleartext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.368343 django-vendor-0.4.8/src/vendor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0002_auto_20200912_0142.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0003_auto_20200915_1839.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0004_offer_offer_description.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0005_auto_20200930_2037.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0006_auto_20201005_2257.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0007_offer_list_bundle_items.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0008_offer_allow_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0009_auto_20201111_0743.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0010_auto_20201112_0138.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0011_auto_20201120_1750.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0012_auto_20201123_1848.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0013_auto_20201202_1759.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0014_term_types_update_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0015_uuid_payments_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0016_auto_20201203_2011.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0017_auto_20201203_2107.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0018_add_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0019_fill_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0020_lock_uuid_address_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0021_auto_20210408_2303.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0022_offer_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0023_profile_null_false.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0024_offer_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0025_auto_20210914_0025.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0026_auto_20210914_1209.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0028_add_trial_date_term_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0030_auto_20220414_1055.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0031_pre_invoice_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0032_alter_invoice_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0033_payment_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0034_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0035_add_subscription_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0036_post_payment_status_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0037_auto_20220609_1644.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0038_auto_20220719_0944.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0039_customerprofile_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0040_auto_20221020_1617.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0041_offer_billing_start_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0042_offer_is_promotional.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0043_invoice_global_discount.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/0044_site_settings_stripe_processor_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.368343 django-vendor-0.4.8/src/vendor/models/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/modelmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/price.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/product.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/models/wishlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.372343 django-vendor-0.4.8/src/vendor/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63108 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/processors/authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/processors/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/processors/payment_gateway_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    71670 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/processors/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.372343 django-vendor-0.4.8/src/vendor/signals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/signals/stripe_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.360343 django-vendor-0.4.8/src/vendor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.372343 django-vendor-0.4.8/src/vendor/templates/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/address_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/checkout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.372343 django-vendor-0.4.8/src/vendor/templates/vendor/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/dummy/payment_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.376343 django-vendor-0.4.8/src/vendor/templates/vendor/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/includes/account_info_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/includes/billing_address_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/includes/cost_overview.html
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/includes/edit_link.html
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/includes/payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/integration_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/invoice_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/invoice_history_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/invoice_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.376343 django-vendor-0.4.8/src/vendor/templates/vendor/manage/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/invoice_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/invoice_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/offer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/offers.html
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/payment_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/processor_site_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/processor_site_config_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/product.html
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/products.html
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/profile_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/profile_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/receipt_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/receipt_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/subscription_add_payment.html
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/subscription_create.html
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/manage/subscription_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/orderitem_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/orderitem_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/orderitem_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/ordersummary.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/payment.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/payment_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/payment_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/payment_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/purchase_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/purchase_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/refund_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templates/vendor/refund_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.376343 django-vendor-0.4.8/src/vendor/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/templatetags/admin_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.376343 django-vendor-0.4.8/src/vendor/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/tests/test_authorizenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    42691 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.380343 django-vendor-0.4.8/src/vendor/urls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/urls/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/urls/vendor_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 17:52:35.380343 django-vendor-0.4.8/src/vendor/views/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/views/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/views/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/views/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/views/vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18137 2023-08-22 17:51:17.000000 django-vendor-0.4.8/src/vendor/views/vendor_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.272009 django-vendor-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-23 18:00:26.272009 django-vendor-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-23 17:58:46.000000 django-vendor-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-23 17:58:46.000000 django-vendor-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-23 18:00:26.272009 django-vendor-0.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.200005 django-vendor-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.208006 django-vendor-0.4.9/src/django_vendor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-23 18:00:26.000000 django-vendor-0.4.9/src/django_vendor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-08-23 18:00:26.000000 django-vendor-0.4.9/src/django_vendor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 18:00:26.000000 django-vendor-0.4.9/src/django_vendor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-23 18:00:26.000000 django-vendor-0.4.9/src/django_vendor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-23 18:00:26.000000 django-vendor-0.4.9/src/django_vendor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.212006 django-vendor-0.4.9/src/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.212006 django-vendor-0.4.9/src/vendor/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.212006 django-vendor-0.4.9/src/vendor/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.216006 django-vendor-0.4.9/src/vendor/api/v1/authorizenet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/api/v1/authorizenet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14742 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/api/v1/authorizenet/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.216006 django-vendor-0.4.9/src/vendor/api/v1/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/api/v1/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17367 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/api/v1/stripe/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.216006 django-vendor-0.4.9/src/vendor/encrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/encrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/encrypt/cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18433 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.236007 django-vendor-0.4.9/src/vendor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0002_auto_20200912_0142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0003_auto_20200915_1839.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0004_offer_offer_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0005_auto_20200930_2037.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0006_auto_20201005_2257.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0007_offer_list_bundle_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0008_offer_allow_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0009_auto_20201111_0743.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0010_auto_20201112_0138.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0011_auto_20201120_1750.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0012_auto_20201123_1848.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0013_auto_20201202_1759.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0014_term_types_update_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0015_uuid_payments_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0016_auto_20201203_2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0017_auto_20201203_2107.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0018_add_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0019_fill_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0020_lock_uuid_address_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0021_auto_20210408_2303.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0022_offer_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0023_profile_null_false.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0024_offer_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0025_auto_20210914_0025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0026_auto_20210914_1209.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0028_add_trial_date_term_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0030_auto_20220414_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0031_pre_invoice_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0032_alter_invoice_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0033_payment_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0034_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0035_add_subscription_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0036_post_payment_status_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0037_auto_20220609_1644.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0038_auto_20220719_0944.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0039_customerprofile_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0040_auto_20221020_1617.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0041_offer_billing_start_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0042_offer_is_promotional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0043_invoice_global_discount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/0044_site_settings_stripe_processor_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.240007 django-vendor-0.4.9/src/vendor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/modelmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/models/wishlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.244008 django-vendor-0.4.9/src/vendor/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63108 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/processors/authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23647 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/processors/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/processors/payment_gateway_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71692 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/processors/stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.244008 django-vendor-0.4.9/src/vendor/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/signals/stripe_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.204005 django-vendor-0.4.9/src/vendor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.252008 django-vendor-0.4.9/src/vendor/templates/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/address_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/checkout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.252008 django-vendor-0.4.9/src/vendor/templates/vendor/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/dummy/payment_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.256008 django-vendor-0.4.9/src/vendor/templates/vendor/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/includes/account_info_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/includes/billing_address_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/includes/cost_overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/includes/edit_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/includes/payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/invoice_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/invoice_history_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/invoice_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.264009 django-vendor-0.4.9/src/vendor/templates/vendor/manage/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/invoice_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/invoice_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/offer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/offers.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/payment_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/processor_site_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/processor_site_config_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/product.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/products.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/profile_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/profile_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/receipt_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/receipt_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/subscription_add_payment.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/subscription_create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/manage/subscription_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/orderitem_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/orderitem_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/orderitem_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/ordersummary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/payment.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/payment_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/payment_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/payment_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/purchase_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/purchase_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/refund_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templates/vendor/refund_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.264009 django-vendor-0.4.9/src/vendor/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/templatetags/admin_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.268009 django-vendor-0.4.9/src/vendor/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30579 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49307 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/tests/test_authorizenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42691 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.268009 django-vendor-0.4.9/src/vendor/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/urls/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/urls/vendor_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 18:00:26.272009 django-vendor-0.4.9/src/vendor/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/views/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/views/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/views/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/views/vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18137 2023-08-23 17:58:46.000000 django-vendor-0.4.9/src/vendor/views/vendor_admin.py
```

### Comparing `django-vendor-0.4.8/PKG-INFO` & `django-vendor-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor
-Version: 0.4.8
+Version: 0.4.9
 Summary: Django App Toolkit for selling digital and physical goods online.
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-0.4.8/README.md` & `django-vendor-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/pyproject.toml` & `django-vendor-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [project]
 name = "django-vendor"
-version = "0.4.8"
+version = "0.4.9"
 
 authors = [
   { name="Grant Viklund", email="renderbox@gmail.com" },
   { name="Roberto Himmelbauer" }
 ]
 description = "Django App Toolkit for selling digital and physical goods online."
 readme = "README.md"
```

### Comparing `django-vendor-0.4.8/src/django_vendor.egg-info/PKG-INFO` & `django-vendor-0.4.9/src/django_vendor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vendor
-Version: 0.4.8
+Version: 0.4.9
 Summary: Django App Toolkit for selling digital and physical goods online.
 Author: Roberto Himmelbauer
 Author-email: Grant Viklund <renderbox@gmail.com>
 Project-URL: Homepage, https://github.com/renderbox/django-vendor
 Project-URL: Bug Tracker, https://github.com/renderbox/django-vendor/issues
 Keywords: django,app
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `django-vendor-0.4.8/src/django_vendor.egg-info/SOURCES.txt` & `django-vendor-0.4.9/src/django_vendor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/admin.py` & `django-vendor-0.4.9/src/vendor/admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/api/v1/authorizenet/views.py` & `django-vendor-0.4.9/src/vendor/api/v1/authorizenet/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/api/v1/stripe/views.py` & `django-vendor-0.4.9/src/vendor/api/v1/stripe/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,31 +314,33 @@
 
     paid_date = timezone.datetime.fromtimestamp(stripe_invoice.status_transitions.paid_at, tz=timezone.utc)
     stripe_charge = processor.stripe_get_object(processor.stripe.Charge, stripe_invoice.charge)
     stripe_subscription = processor.stripe_get_object(processor.stripe.Subscription, stripe_invoice.subscription)
     subscription = processor.get_subscription(stripe_subscription)
 
     if not subscription:
-        logger.error(f"Stripe Subscription Invoice was not processed: stripe_invoice: {stripe_invoice}")
-        return HttpResponse(status=200)
+        msg = f"Stripe Subscription Invoice was not processed: stripe_invoice: {stripe_invoice}"
+        logger.error(msg)
+        return HttpResponse(status=200, content=msg)
     
     stripe_product = processor.stripe_get_object(processor.stripe.Product, stripe_subscription.plan.product)
     offer = processor.get_offer_from_stripe_product(stripe_product)
 
     customer_profile, stripe_customer = processor.get_customer_profile_and_stripe_customer(stripe_invoice.customer)
 
     if not offer or not customer_profile:
-        logger.error(f"Stripe Subscription Invoice was not processed, stripe_invoice: {stripe_invoice.id} offer: {offer}, customer_profile: {customer_profile} stripe_customer: {stripe_customer}")
-        return HttpResponse(status=200)
+        msg = f"Stripe Subscription Invoice was not processed, stripe_invoice: {stripe_invoice.id} offer: {offer}, customer_profile: {customer_profile} stripe_customer: {stripe_customer}"
+        logger.error(msg)
+        return HttpResponse(status=200, content=msg)
 
     payment_status = processor.get_payment_status(stripe_charge.status, stripe_charge.refunded)
     processor.invoice, created = processor.get_or_create_invoice_from_stripe_invoice(stripe_invoice, offer, customer_profile)
     processor.renew_subscription(subscription, stripe_invoice.charge, payment_status, payment_success=True, submitted_date=paid_date)
 
-    return HttpResponse(status=200)
+    return HttpResponse(status=200, content=f"Subscription: {stripe_subscription.id} renewed invoice: {processor.invoice.pk}")
 
 
 class StripeInvoicePaymentSuccededEvent(StripeBaseAPI):
     def post(self, request, *args, **kwargs):
         site = get_site_from_request(self.request)
 
         if not self.is_valid_post(site):
```

### Comparing `django-vendor-0.4.8/src/vendor/api/v1/urls.py` & `django-vendor-0.4.9/src/vendor/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/api/v1/views.py` & `django-vendor-0.4.9/src/vendor/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/apps.py` & `django-vendor-0.4.9/src/vendor/apps.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/config.py` & `django-vendor-0.4.9/src/vendor/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/forms.py` & `django-vendor-0.4.9/src/vendor/forms.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/integrations.py` & `django-vendor-0.4.9/src/vendor/integrations.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0001_initial.py` & `django-vendor-0.4.9/src/vendor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0003_auto_20200915_1839.py` & `django-vendor-0.4.9/src/vendor/migrations/0003_auto_20200915_1839.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0005_auto_20200930_2037.py` & `django-vendor-0.4.9/src/vendor/migrations/0005_auto_20200930_2037.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0006_auto_20201005_2257.py` & `django-vendor-0.4.9/src/vendor/migrations/0006_auto_20201005_2257.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0008_offer_allow_multiple.py` & `django-vendor-0.4.9/src/vendor/migrations/0008_offer_allow_multiple.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0009_auto_20201111_0743.py` & `django-vendor-0.4.9/src/vendor/migrations/0009_auto_20201111_0743.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0010_auto_20201112_0138.py` & `django-vendor-0.4.9/src/vendor/migrations/0010_auto_20201112_0138.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0011_auto_20201120_1750.py` & `django-vendor-0.4.9/src/vendor/migrations/0011_auto_20201120_1750.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0012_auto_20201123_1848.py` & `django-vendor-0.4.9/src/vendor/migrations/0012_auto_20201123_1848.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0013_auto_20201202_1759.py` & `django-vendor-0.4.9/src/vendor/migrations/0013_auto_20201202_1759.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0014_term_types_update_value.py` & `django-vendor-0.4.9/src/vendor/migrations/0014_term_types_update_value.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0015_uuid_payments_receipts.py` & `django-vendor-0.4.9/src/vendor/migrations/0015_uuid_payments_receipts.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0016_auto_20201203_2011.py` & `django-vendor-0.4.9/src/vendor/migrations/0016_auto_20201203_2011.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0017_auto_20201203_2107.py` & `django-vendor-0.4.9/src/vendor/migrations/0017_auto_20201203_2107.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0018_add_uuid_address_profile.py` & `django-vendor-0.4.9/src/vendor/migrations/0018_add_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0019_fill_uuid_address_profile.py` & `django-vendor-0.4.9/src/vendor/migrations/0019_fill_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0020_lock_uuid_address_profile.py` & `django-vendor-0.4.9/src/vendor/migrations/0020_lock_uuid_address_profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0021_auto_20210408_2303.py` & `django-vendor-0.4.9/src/vendor/migrations/0021_auto_20210408_2303.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0023_profile_null_false.py` & `django-vendor-0.4.9/src/vendor/migrations/0023_profile_null_false.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0025_auto_20210914_0025.py` & `django-vendor-0.4.9/src/vendor/migrations/0025_auto_20210914_0025.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0026_auto_20210914_1209.py` & `django-vendor-0.4.9/src/vendor/migrations/0026_auto_20210914_1209.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py` & `django-vendor-0.4.9/src/vendor/migrations/0027_bugfix_vendor_notes_invoice_history.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0028_add_trial_date_term_details.py` & `django-vendor-0.4.9/src/vendor/migrations/0028_add_trial_date_term_details.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py` & `django-vendor-0.4.9/src/vendor/migrations/0029_alter_customerprofile_currency_and_more.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0030_auto_20220414_1055.py` & `django-vendor-0.4.9/src/vendor/migrations/0030_auto_20220414_1055.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0031_pre_invoice_status_change.py` & `django-vendor-0.4.9/src/vendor/migrations/0031_pre_invoice_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0033_payment_status.py` & `django-vendor-0.4.9/src/vendor/migrations/0033_payment_status.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0034_subscription.py` & `django-vendor-0.4.9/src/vendor/migrations/0034_subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0035_add_subscription_relation.py` & `django-vendor-0.4.9/src/vendor/migrations/0035_add_subscription_relation.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0036_post_payment_status_change.py` & `django-vendor-0.4.9/src/vendor/migrations/0036_post_payment_status_change.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0037_auto_20220609_1644.py` & `django-vendor-0.4.9/src/vendor/migrations/0037_auto_20220609_1644.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0038_auto_20220719_0944.py` & `django-vendor-0.4.9/src/vendor/migrations/0038_auto_20220719_0944.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0040_auto_20221020_1617.py` & `django-vendor-0.4.9/src/vendor/migrations/0040_auto_20221020_1617.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0042_offer_is_promotional.py` & `django-vendor-0.4.9/src/vendor/migrations/0042_offer_is_promotional.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/migrations/0044_site_settings_stripe_processor_rename.py` & `django-vendor-0.4.9/src/vendor/migrations/0044_site_settings_stripe_processor_rename.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/__init__.py` & `django-vendor-0.4.9/src/vendor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/address.py` & `django-vendor-0.4.9/src/vendor/models/address.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/base.py` & `django-vendor-0.4.9/src/vendor/models/base.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/choice.py` & `django-vendor-0.4.9/src/vendor/models/choice.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/invoice.py` & `django-vendor-0.4.9/src/vendor/models/invoice.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/modelmanagers.py` & `django-vendor-0.4.9/src/vendor/models/modelmanagers.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/offer.py` & `django-vendor-0.4.9/src/vendor/models/offer.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/payment.py` & `django-vendor-0.4.9/src/vendor/models/payment.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/price.py` & `django-vendor-0.4.9/src/vendor/models/price.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/profile.py` & `django-vendor-0.4.9/src/vendor/models/profile.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/receipt.py` & `django-vendor-0.4.9/src/vendor/models/receipt.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/subscription.py` & `django-vendor-0.4.9/src/vendor/models/subscription.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/tax.py` & `django-vendor-0.4.9/src/vendor/models/tax.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/utils.py` & `django-vendor-0.4.9/src/vendor/models/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/validator.py` & `django-vendor-0.4.9/src/vendor/models/validator.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/models/wishlist.py` & `django-vendor-0.4.9/src/vendor/models/wishlist.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/processors/__init__.py` & `django-vendor-0.4.9/src/vendor/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/processors/authorizenet.py` & `django-vendor-0.4.9/src/vendor/processors/authorizenet.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/processors/base.py` & `django-vendor-0.4.9/src/vendor/processors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """
 Base Payment processor used by all derived processors.
 """
-import django.dispatch
-
+import logging
 from datetime import timedelta
-from decimal import Decimal, ROUND_DOWN
-from django.conf import settings
+from decimal import Decimal
+
+import django.dispatch
 from django.utils import timezone
 
 from vendor import config
-from vendor.forms import CreditCardForm, BillingAddressForm
-from vendor.models import Payment, Invoice, Receipt, Subscription
-from vendor.models.choice import PurchaseStatus, SubscriptionStatus, TermType, InvoiceStatus, PaymentTypes
+from vendor.forms import BillingAddressForm, CreditCardForm
+from vendor.models import Payment, Receipt, Subscription
+from vendor.models.choice import (InvoiceStatus, PaymentTypes, PurchaseStatus,
+                                  SubscriptionStatus, TermType)
+
+logger = logging.getLogger(__name__)
+
 
 ##########
 # SIGNALS
 vendor_pre_authorization = django.dispatch.Signal()
 vendor_process_payment = django.dispatch.Signal()
 vendor_post_authorization = django.dispatch.Signal()
 vendor_subscription_cancel = django.dispatch.Signal()
@@ -524,29 +528,44 @@
         """
         return True
 
     def renew_subscription(self, subscription, payment_transaction_id="", payment_status=PurchaseStatus.QUEUED, payment_success=True, submitted_date=timezone.now()):
         """
         Function to renew already paid subscriptions form the payment gateway provider.
         """
+        if Payment.objects.filter(
+                profile=subscription.profile,
+                invoice=self.invoice,
+                transaction=payment_transaction_id,
+                subscription=subscription).exists():
+            return None
+        
+        if Receipt.objects.filter(
+            transaction=payment_transaction_id,
+            profile=subscription.profile,
+            subscription=subscription
+        ).exists():
+            return None
+
         self.subscription = subscription
 
         self.payment = Payment.objects.create(
             profile=subscription.profile,
             invoice=self.invoice,
             transaction=payment_transaction_id,
-            submitted_date=submitted_date,
             subscription=subscription,
+            submitted_date=submitted_date,
             amount=self.invoice.total,
             success=payment_success,
             status=payment_status,
             payee_full_name=" ".join([self.invoice.profile.user.first_name, self.invoice.profile.user.last_name])
         )
-
-        self.create_receipts(self.invoice.order_items.all())
+            
+        if payment_status in [PurchaseStatus.QUEUED, PurchaseStatus.CAPTURED, PurchaseStatus.AUTHORIZED, PurchaseStatus.SETTLED]:
+            self.create_receipts(self.invoice.order_items.all())
 
     def subscription_update_price(self, subscription, new_price, user):
         """
         Call to handle when a new subscription price needs to be approved.
         """
         now = timezone.now().strftime("%Y-%m-%d_%H:%M:%S")
```

### Comparing `django-vendor-0.4.8/src/vendor/processors/payment_gateway_data_transfer.py` & `django-vendor-0.4.9/src/vendor/processors/payment_gateway_data_transfer.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/processors/stripe.py` & `django-vendor-0.4.9/src/vendor/processors/stripe.py`

 * *Files 0% similar despite different names*

```diff
@@ -691,15 +691,15 @@
             Returns:
                 CustomerProfile Instance or None
                 Stripe Customer Object or None
         """
         stripe_customer = None
         customer_profile = None
         
-        stripe_customer = self.stripe_get_object(stripe_customer_id)
+        stripe_customer = self.stripe_get_object(self.stripe.Customer, stripe_customer_id)
         if not stripe_customer:
             logger.info(f"Stripe Customer was not found: {stripe_customer_id}")
             return customer_profile, stripe_customer
 
         customer_profile = self.get_customer_profile(stripe_customer)
         if not customer_profile:
             logger.info(f"Customer Profile not found for stripe_customer {stripe_customer.id} site: {self.site}")
```

### Comparing `django-vendor-0.4.8/src/vendor/signals/stripe_signals.py` & `django-vendor-0.4.9/src/vendor/signals/stripe_signals.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/checkout.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/checkout.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/includes/account_info_form.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/includes/account_info_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/includes/billing_address_form.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/includes/billing_address_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/includes/cost_overview.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/includes/cost_overview.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/includes/payment_form.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/includes/payment_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/integration_form.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/integration_form.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/invoice_detail.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/invoice_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/invoice_history_detail.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/invoice_history_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/invoice_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/invoice_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/config_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/dashboard.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/invoice_detail.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/invoice_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/invoice_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/invoice_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/offer.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/offer.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/offers.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/offers.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/payment_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/payment_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/processor_site_config_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/processor_site_config_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/product.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/product.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/products.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/products.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/profile_detail.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/profile_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/profile_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/profile_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/receipt_detail.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/receipt_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/receipt_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/receipt_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/subscription_add_payment.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/subscription_add_payment.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/subscription_create.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/subscription_create.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/manage/subscription_detail.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/manage/subscription_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/orderitem_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/orderitem_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/ordersummary.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/ordersummary.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/payment_summary.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/payment_summary.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/purchase_detail.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/purchase_detail.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/purchase_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/purchase_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templates/vendor/refund_list.html` & `django-vendor-0.4.9/src/vendor/templates/vendor/refund_list.html`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/templatetags/admin_tags.py` & `django-vendor-0.4.9/src/vendor/templatetags/admin_tags.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/tests/__init__.py` & `django-vendor-0.4.9/src/vendor/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/tests/test_authorizenet.py` & `django-vendor-0.4.9/src/vendor/tests/test_authorizenet.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/tests/test_processor.py` & `django-vendor-0.4.9/src/vendor/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/tests/test_stripe.py` & `django-vendor-0.4.9/src/vendor/tests/test_stripe.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/urls/vendor.py` & `django-vendor-0.4.9/src/vendor/urls/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/urls/vendor_admin.py` & `django-vendor-0.4.9/src/vendor/urls/vendor_admin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/utils.py` & `django-vendor-0.4.9/src/vendor/utils.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/views/__init__.py` & `django-vendor-0.4.9/src/vendor/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/views/config.py` & `django-vendor-0.4.9/src/vendor/views/config.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/views/integration.py` & `django-vendor-0.4.9/src/vendor/views/integration.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/views/mixin.py` & `django-vendor-0.4.9/src/vendor/views/mixin.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/views/report.py` & `django-vendor-0.4.9/src/vendor/views/report.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/views/vendor.py` & `django-vendor-0.4.9/src/vendor/views/vendor.py`

 * *Files identical despite different names*

### Comparing `django-vendor-0.4.8/src/vendor/views/vendor_admin.py` & `django-vendor-0.4.9/src/vendor/views/vendor_admin.py`

 * *Files identical despite different names*

