# Comparing `tmp/pyynab-0.8.8.tar.gz` & `tmp/pyynab-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyynab-0.8.8.tar", last modified: Tue Sep 17 13:07:19 2019, max compression
+gzip compressed data, was "pyynab-0.9.0.tar", last modified: Sun Oct 16 11:25:21 2022, max compression
```

## Comparing `pyynab-0.8.8.tar` & `pyynab-0.9.0.tar`

### file list

```diff
@@ -1,203 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-09-17 13:07:19.000000 pyynab-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (115)       38 2019-09-17 13:07:19.000000 pyynab-0.8.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-09-17 13:07:19.000000 pyynab-0.8.8/test/
--rw-r--r--   0 runner    (1001) docker     (115)     1093 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_payee_location.py
--rw-r--r--   0 runner    (1001) docker     (115)     1085 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_user_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1084 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_deprecated_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1185 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_detail_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1169 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_transaction_detail_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     1093 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_payee_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1158 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_payees_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1201 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_settings_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1243 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_transaction_detail_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     1101 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_payees_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1117 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (115)     1109 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_account_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1185 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_month_category_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (115)     1043 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_account.py
--rw-r--r--   0 runner    (1001) docker     (115)     1101 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_sub_transaction.py
--rw-r--r--   0 runner    (1001) docker     (115)     1151 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_category_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1143 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_month_detail_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1093 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_summary.py
--rw-r--r--   0 runner    (1001) docker     (115)     1223 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1181 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     2267 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1085 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_month_summary.py
--rw-r--r--   0 runner    (1001) docker     (115)     1125 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_transaction_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     1125 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_hybrid_transaction.py
--rw-r--r--   0 runner    (1001) docker     (115)     1167 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_transaction_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (115)     1175 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_transactions_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (115)     1169 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_hybrid_transaction_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     1149 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1143 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_account_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1159 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1151 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_detail_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1119 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_user_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1185 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_category_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1119 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_bulk_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1175 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_sub_transaction.py
--rw-r--r--   0 runner    (1001) docker     (115)     1332 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_budgets_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1117 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_category_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1217 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_transactions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1019 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (115)     1188 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_months_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1085 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_bulk_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1183 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1129 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_detail_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     1127 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_payee_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1001 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1159 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_payee_location_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1201 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_month_summaries_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1069 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_date_format.py
--rw-r--r--   0 runner    (1001) docker     (115)     1127 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_month_category.py
--rw-r--r--   0 runner    (1001) docker     (115)     1167 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_payee_locations_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1077 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_error_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     1101 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_settings.py
--rw-r--r--   0 runner    (1001) docker     (115)     1135 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_payees_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1151 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_accounts_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1121 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_month_detail_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     1027 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_payee.py
--rw-r--r--   0 runner    (1001) docker     (115)     1233 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_hybrid_transactions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1175 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_transaction_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1167 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_month_summaries_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1077 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_month_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     1199 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_transaction_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     1109 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_transaction.py
--rw-r--r--   0 runner    (1001) docker     (115)     1193 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_payee_location_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1199 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_hybrid_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1085 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     1167 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_settings_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1207 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_transaction_summary.py
--rw-r--r--   0 runner    (1001) docker     (115)     1141 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1568 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_categories_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1346 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1153 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_bulk_response_data_bulk.py
--rw-r--r--   0 runner    (1001) docker     (115)     1133 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_transaction_summary.py
--rw-r--r--   0 runner    (1001) docker     (115)     1093 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_category_group.py
--rw-r--r--   0 runner    (1001) docker     (115)     1133 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1183 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_transactions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1441 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_payee_locations_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     1253 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_category_group_with_categories_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     1215 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1117 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1151 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_save_category_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1209 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_category_group_with_categories.py
--rw-r--r--   0 runner    (1001) docker     (115)     1167 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_categories_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1249 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_transaction_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1101 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_currency_format.py
--rw-r--r--   0 runner    (1001) docker     (115)     1193 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_budget_summary_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1177 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_month_detail_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1093 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     1051 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_category.py
--rw-r--r--   0 runner    (1001) docker     (115)     1257 2019-09-17 13:07:18.000000 pyynab-0.8.8/test/test_scheduled_transactions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     1201 2019-09-17 13:07:17.000000 pyynab-0.8.8/test/test_payee_locations_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)      561 2019-09-17 13:07:19.000000 pyynab-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1420 2019-09-17 13:07:18.000000 pyynab-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-09-17 13:07:19.000000 pyynab-0.8.8/ynab/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-09-17 13:07:19.000000 pyynab-0.8.8/ynab/models/
--rw-r--r--   0 runner    (1001) docker     (115)     3795 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/category_group_with_categories_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     9052 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/sub_transaction.py
--rw-r--r--   0 runner    (1001) docker     (115)     3331 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_detail_response.py
--rw-r--r--   0 runner    (1001) docker     (115)    18081 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/scheduled_transaction_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     3240 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/date_format.py
--rw-r--r--   0 runner    (1001) docker     (115)     3331 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     4426 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/accounts_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)    15803 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_transaction.py
--rw-r--r--   0 runner    (1001) docker     (115)     3351 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_settings_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     4920 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/scheduled_transactions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)    16209 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     6452 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/payee_location.py
--rw-r--r--   0 runner    (1001) docker     (115)    15798 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/category.py
--rw-r--r--   0 runner    (1001) docker     (115)     3291 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/category_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3351 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/month_summaries_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3264 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     6019 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/transaction_detail_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     5099 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/bulk_response_data_bulk.py
--rw-r--r--   0 runner    (1001) docker     (115)     3566 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/hybrid_transactions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     5692 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/category_group.py
--rw-r--r--   0 runner    (1001) docker     (115)     3243 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/user_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3261 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/payee_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3331 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_category_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3271 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/payees_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3351 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/payee_locations_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3465 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_transaction_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (115)     3367 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/category_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3291 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/bulk_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     7121 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/category_group_with_categories.py
--rw-r--r--   0 runner    (1001) docker     (115)     3251 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/user_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     7950 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_transactions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3311 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/categories_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     4425 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_detail_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     8083 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_summary.py
--rw-r--r--   0 runner    (1001) docker     (115)     3422 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_month_category_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (115)    14322 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/scheduled_transaction_summary.py
--rw-r--r--   0 runner    (1001) docker     (115)     4217 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_transactions_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (115)     3391 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/hybrid_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3341 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/payee_location_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3421 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/scheduled_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3778 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/scheduled_transaction_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     9464 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/month_summary.py
--rw-r--r--   0 runner    (1001) docker     (115)     3478 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/transaction_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3281 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/account_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3449 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_month_category.py
--rw-r--r--   0 runner    (1001) docker     (115)     3561 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/month_detail_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     3291 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     4326 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_settings.py
--rw-r--r--   0 runner    (1001) docker     (115)     3427 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_settings_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     9927 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/scheduled_sub_transaction.py
--rw-r--r--   0 runner    (1001) docker     (115)    10406 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/month_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     5678 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/payee.py
--rw-r--r--   0 runner    (1001) docker     (115)     3334 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/month_detail_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)    19832 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/transaction_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     3114 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/user.py
--rw-r--r--   0 runner    (1001) docker     (115)     3321 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/month_detail_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     4655 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/categories_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3543 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/payee_location_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3251 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/bulk_response.py
--rw-r--r--   0 runner    (1001) docker     (115)    21508 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/hybrid_transaction.py
--rw-r--r--   0 runner    (1001) docker     (115)    12403 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/account.py
--rw-r--r--   0 runner    (1001) docker     (115)     4517 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/error_detail.py
--rw-r--r--   0 runner    (1001) docker     (115)     4455 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_category_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     4465 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/month_summaries_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3371 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/save_transactions_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3321 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3589 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/payee_locations_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     9525 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/currency_format.py
--rw-r--r--   0 runner    (1001) docker     (115)     3336 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/account_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     6499 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/scheduled_transaction_detail_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     7715 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/hybrid_transaction_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)     3462 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (115)     4366 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_summary_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)    10924 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_detail_all_of.py
--rw-r--r--   0 runner    (1001) docker     (115)    16538 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/transaction_summary.py
--rw-r--r--   0 runner    (1001) docker     (115)     5902 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4356 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/payees_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     4584 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/transactions_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3274 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/payee_response_data.py
--rw-r--r--   0 runner    (1001) docker     (115)     3411 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/models/scheduled_transaction_response.py
--rw-r--r--   0 runner    (1001) docker     (115)     3341 2019-09-17 13:07:17.000000 pyynab-0.8.8/ynab/models/budget_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (115)    25460 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api_client.py
--rw-r--r--   0 runner    (1001) docker     (115)    10508 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/configuration.py
--rw-r--r--   0 runner    (1001) docker     (115)     4001 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-09-17 13:07:19.000000 pyynab-0.8.8/ynab/api/
--rw-r--r--   0 runner    (1001) docker     (115)    12607 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/payees_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     5244 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (115)    12709 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (115)    16638 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/budgets_api.py
--rw-r--r--   0 runner    (1001) docker     (115)    27664 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/categories_api.py
--rw-r--r--   0 runner    (1001) docker     (115)    56377 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (115)    13404 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/scheduled_transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     7353 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/deprecated_api.py
--rw-r--r--   0 runner    (1001) docker     (115)    12928 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/months_api.py
--rw-r--r--   0 runner    (1001) docker     (115)      585 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    18541 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/api/payee_locations_api.py
--rw-r--r--   0 runner    (1001) docker     (115)    12700 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/rest.py
--rw-r--r--   0 runner    (1001) docker     (115)     6766 2019-09-17 13:07:18.000000 pyynab-0.8.8/ynab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-09-17 13:07:19.000000 pyynab-0.8.8/pyynab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)       10 2019-09-17 13:07:19.000000 pyynab-0.8.8/pyynab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)     6671 2019-09-17 13:07:19.000000 pyynab-0.8.8/pyynab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-09-17 13:07:19.000000 pyynab-0.8.8/pyynab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)      561 2019-09-17 13:07:19.000000 pyynab-0.8.8/pyynab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)       48 2019-09-17 13:07:19.000000 pyynab-0.8.8/pyynab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)    11884 2019-09-17 13:07:18.000000 pyynab-0.8.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:25:21.390649 pyynab-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-16 11:25:21.390649 pyynab-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12695 2022-10-16 11:25:19.000000 pyynab-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:25:21.362647 pyynab-0.9.0/pyynab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-16 11:25:20.000000 pyynab-0.9.0/pyynab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7331 2022-10-16 11:25:21.000000 pyynab-0.9.0/pyynab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-16 11:25:20.000000 pyynab-0.9.0/pyynab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-10-16 11:25:20.000000 pyynab-0.9.0/pyynab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-16 11:25:20.000000 pyynab-0.9.0/pyynab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-16 11:25:21.390649 pyynab-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-10-16 11:25:19.000000 pyynab-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:25:21.374648 pyynab-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_account_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_account_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_accounts_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_detail_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_detail_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_detail_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_settings_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_settings_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_budget_summary_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_budgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_bulk_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_bulk_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_bulk_response_data_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_categories_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_categories_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_category.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_category_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_category_group_with_categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_category_group_with_categories_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_category_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_category_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_currency_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_date_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_deprecated_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_error_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_hybrid_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_hybrid_transaction_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_hybrid_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_hybrid_transactions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_month_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_month_detail_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_month_detail_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_month_detail_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_month_summaries_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_month_summaries_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_month_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_months_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payee.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payee_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payee_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payee_location_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_payee_locations_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payee_locations_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payee_locations_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payee_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payee_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_payees_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payees_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_payees_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_account_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_category_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_category_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_month_category.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_month_category_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_sub_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_transaction_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_transactions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_save_transactions_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_scheduled_sub_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_scheduled_transaction_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_scheduled_transaction_detail_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_scheduled_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_scheduled_transaction_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_scheduled_transaction_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_scheduled_transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_scheduled_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_scheduled_transactions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_sub_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_transaction_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_transaction_detail_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_transaction_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_transaction_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_transactions_import_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_transactions_import_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-10-16 11:25:18.000000 pyynab-0.9.0/test/test_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_transactions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_update_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_update_transaction_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_update_transactions_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-10-16 11:25:19.000000 pyynab-0.9.0/test/test_user_response_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:25:21.378648 pyynab-0.9.0/ynab/
+-rw-r--r--   0 runner    (1001) docker     (121)     7373 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:25:21.378648 pyynab-0.9.0/ynab/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18512 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16991 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/budgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27934 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/categories_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7355 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/deprecated_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12936 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/months_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18543 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/payee_locations_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12619 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/payees_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13412 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/scheduled_transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62911 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5244 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25460 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10508 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4001 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 11:25:21.390649 pyynab-0.9.0/ynab/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     6509 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14064 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/account_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/account_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/accounts_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16209 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10924 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_detail_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_detail_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4425 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_detail_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4326 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_settings_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3427 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_settings_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9002 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4273 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/budget_summary_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3251 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/bulk_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/bulk_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/bulk_response_data_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3462 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4655 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/categories_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20629 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/category.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5692 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/category_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7121 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/category_group_with_categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/category_group_with_categories_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/category_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3367 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/category_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9525 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/currency_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/date_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4517 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/error_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3264 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21223 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/hybrid_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7430 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/hybrid_transaction_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/hybrid_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3566 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/hybrid_transactions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10321 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/month_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3561 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/month_detail_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/month_detail_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3334 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/month_detail_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/month_summaries_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4465 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/month_summaries_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9379 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/month_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5682 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payee.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6452 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payee_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payee_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payee_location_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payee_locations_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payee_locations_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payee_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payee_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payees_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4356 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/payees_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_account_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_category_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_category_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_month_category.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_month_category_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7588 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_sub_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17855 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_transaction_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7954 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_transactions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/save_transactions_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9569 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/scheduled_sub_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17453 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/scheduled_transaction_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/scheduled_transaction_detail_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3411 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/scheduled_transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/scheduled_transaction_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13875 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/scheduled_transaction_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/scheduled_transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4920 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/scheduled_transactions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11500 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/sub_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19832 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/transaction_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6019 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/transaction_detail_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3321 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/transaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/transaction_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16538 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/transaction_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/transactions_import_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3727 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/transactions_import_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-10-16 11:25:18.000000 pyynab-0.9.0/ynab/models/transactions_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4584 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/models/transactions_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18595 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/models/update_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/models/update_transaction_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/models/update_transactions_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3251 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/models/user_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/models/user_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12700 2022-10-16 11:25:19.000000 pyynab-0.9.0/ynab/rest.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyynab-0.8.8/test/test_payee_location.py` & `pyynab-0.9.0/test/test_payee_location.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_user_response.py` & `pyynab-0.9.0/test/test_user_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_deprecated_api.py` & `pyynab-0.9.0/test/test_deprecated_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_detail_response_data.py` & `pyynab-0.9.0/test/test_budget_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_transaction_detail_all_of.py` & `pyynab-0.9.0/test/test_transaction_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payee_response.py` & `pyynab-0.9.0/test/test_payee_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payees_api.py` & `pyynab-0.9.0/test/test_payees_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_settings_response_data.py` & `pyynab-0.9.0/test/test_budget_settings_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_transaction_detail_all_of.py` & `pyynab-0.9.0/test/test_scheduled_transaction_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payees_response.py` & `pyynab-0.9.0/test/test_payees_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_bulk_transactions.py` & `pyynab-0.9.0/test/test_bulk_transactions.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_account_response.py` & `pyynab-0.9.0/test/test_account_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_month_category_wrapper.py` & `pyynab-0.9.0/test/test_save_month_category_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_account.py` & `pyynab-0.9.0/test/test_account.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_sub_transaction.py` & `pyynab-0.9.0/test/test_sub_transaction.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_category_response_data.py` & `pyynab-0.9.0/test/test_category_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_month_detail_response.py` & `pyynab-0.9.0/test/test_month_detail_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_summary.py` & `pyynab-0.9.0/test/test_budget_summary.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_transactions_response.py` & `pyynab-0.9.0/test/test_scheduled_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_accounts_api.py` & `pyynab-0.9.0/test/test_accounts_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 
     def setUp(self):
         self.api = ynab.api.accounts_api.AccountsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_create_account(self):
+        """Test case for create_account
+
+        Create a new account  # noqa: E501
+        """
+        pass
+
     def test_get_account_by_id(self):
         """Test case for get_account_by_id
 
         Single account  # noqa: E501
         """
         pass
```

### Comparing `pyynab-0.8.8/test/test_transactions_api.py` & `pyynab-0.9.0/test/test_transactions_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,21 @@
     def test_get_transactions_by_payee(self):
         """Test case for get_transactions_by_payee
 
         List payee transactions  # noqa: E501
         """
         pass
 
+    def test_import_transactions(self):
+        """Test case for import_transactions
+
+        Import transactions  # noqa: E501
+        """
+        pass
+
     def test_update_transaction(self):
         """Test case for update_transaction
 
         Updates an existing transaction  # noqa: E501
         """
         pass
```

### Comparing `pyynab-0.8.8/test/test_month_summary.py` & `pyynab-0.9.0/test/test_month_summary.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_transaction_detail.py` & `pyynab-0.9.0/test/test_transaction_detail.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_hybrid_transaction.py` & `pyynab-0.9.0/test/test_hybrid_transaction.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_transaction_wrapper.py` & `pyynab-0.9.0/test/test_save_transaction_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_transactions_wrapper.py` & `pyynab-0.9.0/test/test_save_transactions_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_hybrid_transaction_all_of.py` & `pyynab-0.9.0/test/test_hybrid_transaction_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_transactions_response.py` & `pyynab-0.9.0/test/test_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_account_response_data.py` & `pyynab-0.9.0/test/test_account_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_summary_response.py` & `pyynab-0.9.0/test/test_budget_summary_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_detail_response.py` & `pyynab-0.9.0/test/test_budget_detail_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_user_response_data.py` & `pyynab-0.9.0/test/test_user_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_category_response_data.py` & `pyynab-0.9.0/test/test_save_category_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_bulk_response_data.py` & `pyynab-0.9.0/test/test_bulk_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_sub_transaction.py` & `pyynab-0.9.0/test/test_scheduled_sub_transaction.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budgets_api.py` & `pyynab-0.9.0/test/test_budgets_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_category_response.py` & `pyynab-0.9.0/test/test_category_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_transactions_response_data.py` & `pyynab-0.9.0/test/test_save_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_user.py` & `pyynab-0.9.0/test/test_user.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_months_api.py` & `pyynab-0.9.0/test/test_months_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_bulk_response.py` & `pyynab-0.9.0/test/test_bulk_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_transactions_response.py` & `pyynab-0.9.0/test/test_save_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_detail_all_of.py` & `pyynab-0.9.0/test/test_budget_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payee_response_data.py` & `pyynab-0.9.0/test/test_payee_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_user_api.py` & `pyynab-0.9.0/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payee_location_response.py` & `pyynab-0.9.0/test/test_payee_location_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_month_summaries_response_data.py` & `pyynab-0.9.0/test/test_month_summaries_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_date_format.py` & `pyynab-0.9.0/test/test_date_format.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_month_category.py` & `pyynab-0.9.0/test/test_save_month_category.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payee_locations_response.py` & `pyynab-0.9.0/test/test_payee_locations_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_error_detail.py` & `pyynab-0.9.0/test/test_error_detail.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_settings.py` & `pyynab-0.9.0/test/test_budget_settings.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payees_response_data.py` & `pyynab-0.9.0/test/test_payees_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_accounts_response_data.py` & `pyynab-0.9.0/test/test_accounts_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_month_detail_all_of.py` & `pyynab-0.9.0/test/test_month_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payee.py` & `pyynab-0.9.0/test/test_payee.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_hybrid_transactions_response_data.py` & `pyynab-0.9.0/test/test_hybrid_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_transaction_response_data.py` & `pyynab-0.9.0/test/test_transaction_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_month_summaries_response.py` & `pyynab-0.9.0/test/test_month_summaries_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_month_detail.py` & `pyynab-0.9.0/test/test_month_detail.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_transaction_detail.py` & `pyynab-0.9.0/test/test_scheduled_transaction_detail.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_transaction.py` & `pyynab-0.9.0/test/test_save_transaction.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payee_location_response_data.py` & `pyynab-0.9.0/test/test_payee_location_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_hybrid_transactions_response.py` & `pyynab-0.9.0/test/test_hybrid_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_detail.py` & `pyynab-0.9.0/test/test_budget_detail.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_settings_response.py` & `pyynab-0.9.0/test/test_budget_settings_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_transaction_summary.py` & `pyynab-0.9.0/test/test_scheduled_transaction_summary.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_transaction_response.py` & `pyynab-0.9.0/test/test_transaction_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_categories_api.py` & `pyynab-0.9.0/test/test_categories_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_transactions_api.py` & `pyynab-0.9.0/test/test_scheduled_transactions_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_bulk_response_data_bulk.py` & `pyynab-0.9.0/test/test_bulk_response_data_bulk.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_transaction_summary.py` & `pyynab-0.9.0/test/test_transaction_summary.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_category_group.py` & `pyynab-0.9.0/test/test_category_group.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_categories_response.py` & `pyynab-0.9.0/test/test_categories_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_transactions_response_data.py` & `pyynab-0.9.0/test/test_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payee_locations_api.py` & `pyynab-0.9.0/test/test_payee_locations_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_category_group_with_categories_all_of.py` & `pyynab-0.9.0/test/test_category_group_with_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_transaction_response.py` & `pyynab-0.9.0/test/test_scheduled_transaction_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_accounts_response.py` & `pyynab-0.9.0/test/test_accounts_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_save_category_response.py` & `pyynab-0.9.0/test/test_save_category_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_category_group_with_categories.py` & `pyynab-0.9.0/test/test_category_group_with_categories.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_categories_response_data.py` & `pyynab-0.9.0/test/test_categories_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_transaction_response_data.py` & `pyynab-0.9.0/test/test_scheduled_transaction_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_currency_format.py` & `pyynab-0.9.0/test/test_currency_format.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_budget_summary_response_data.py` & `pyynab-0.9.0/test/test_budget_summary_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_month_detail_response_data.py` & `pyynab-0.9.0/test/test_month_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_error_response.py` & `pyynab-0.9.0/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_category.py` & `pyynab-0.9.0/test/test_category.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_scheduled_transactions_response_data.py` & `pyynab-0.9.0/test/test_scheduled_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/test/test_payee_locations_response_data.py` & `pyynab-0.9.0/test/test_payee_locations_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/setup.py` & `pyynab-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pyynab"
-VERSION = "0.8.8"
+VERSION = "0.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pyynab-0.8.8/ynab/models/category_group_with_categories_all_of.py` & `pyynab-0.9.0/ynab/models/category_group_with_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/sub_transaction.py` & `pyynab-0.9.0/ynab/models/scheduled_sub_transaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class SubTransaction(object):
+class ScheduledSubTransaction(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -34,232 +34,232 @@
     openapi_types = {
         'amount': 'int',
         'category_id': 'str',
         'deleted': 'bool',
         'id': 'str',
         'memo': 'str',
         'payee_id': 'str',
-        'transaction_id': 'str',
+        'scheduled_transaction_id': 'str',
         'transfer_account_id': 'str'
     }
 
     attribute_map = {
         'amount': 'amount',
         'category_id': 'category_id',
         'deleted': 'deleted',
         'id': 'id',
         'memo': 'memo',
         'payee_id': 'payee_id',
-        'transaction_id': 'transaction_id',
+        'scheduled_transaction_id': 'scheduled_transaction_id',
         'transfer_account_id': 'transfer_account_id'
     }
 
-    def __init__(self, amount=None, category_id=None, deleted=None, id=None, memo=None, payee_id=None, transaction_id=None, transfer_account_id=None):  # noqa: E501
-        """SubTransaction - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, amount=None, category_id=None, deleted=None, id=None, memo=None, payee_id=None, scheduled_transaction_id=None, transfer_account_id=None):  # noqa: E501
+        """ScheduledSubTransaction - a model defined in OpenAPI"""  # noqa: E501
 
         self._amount = None
         self._category_id = None
         self._deleted = None
         self._id = None
         self._memo = None
         self._payee_id = None
-        self._transaction_id = None
+        self._scheduled_transaction_id = None
         self._transfer_account_id = None
         self.discriminator = None
 
         self.amount = amount
-        self.category_id = category_id
+        if category_id is not None:
+            self.category_id = category_id
         self.deleted = deleted
         self.id = id
-        self.memo = memo
-        self.payee_id = payee_id
-        self.transaction_id = transaction_id
-        self.transfer_account_id = transfer_account_id
+        if memo is not None:
+            self.memo = memo
+        if payee_id is not None:
+            self.payee_id = payee_id
+        self.scheduled_transaction_id = scheduled_transaction_id
+        if transfer_account_id is not None:
+            self.transfer_account_id = transfer_account_id
 
     @property
     def amount(self):
-        """Gets the amount of this SubTransaction.  # noqa: E501
+        """Gets the amount of this ScheduledSubTransaction.  # noqa: E501
 
-        The subtransaction amount in milliunits format  # noqa: E501
+        The scheduled subtransaction amount in milliunits format  # noqa: E501
 
-        :return: The amount of this SubTransaction.  # noqa: E501
+        :return: The amount of this ScheduledSubTransaction.  # noqa: E501
         :rtype: int
         """
         return self._amount
 
     @amount.setter
     def amount(self, amount):
-        """Sets the amount of this SubTransaction.
+        """Sets the amount of this ScheduledSubTransaction.
 
-        The subtransaction amount in milliunits format  # noqa: E501
+        The scheduled subtransaction amount in milliunits format  # noqa: E501
 
-        :param amount: The amount of this SubTransaction.  # noqa: E501
+        :param amount: The amount of this ScheduledSubTransaction.  # noqa: E501
         :type: int
         """
         if amount is None:
             raise ValueError("Invalid value for `amount`, must not be `None`")  # noqa: E501
 
         self._amount = amount
 
     @property
     def category_id(self):
-        """Gets the category_id of this SubTransaction.  # noqa: E501
+        """Gets the category_id of this ScheduledSubTransaction.  # noqa: E501
 
 
-        :return: The category_id of this SubTransaction.  # noqa: E501
+        :return: The category_id of this ScheduledSubTransaction.  # noqa: E501
         :rtype: str
         """
         return self._category_id
 
     @category_id.setter
     def category_id(self, category_id):
-        """Sets the category_id of this SubTransaction.
+        """Sets the category_id of this ScheduledSubTransaction.
 
 
-        :param category_id: The category_id of this SubTransaction.  # noqa: E501
+        :param category_id: The category_id of this ScheduledSubTransaction.  # noqa: E501
         :type: str
         """
-        if category_id is None:
-            raise ValueError("Invalid value for `category_id`, must not be `None`")  # noqa: E501
 
         self._category_id = category_id
 
     @property
     def deleted(self):
-        """Gets the deleted of this SubTransaction.  # noqa: E501
+        """Gets the deleted of this ScheduledSubTransaction.  # noqa: E501
 
-        Whether or not the subtransaction has been deleted.  Deleted subtransactions will only be included in delta requests.  # noqa: E501
+        Whether or not the scheduled subtransaction has been deleted.  Deleted scheduled subtransactions will only be included in delta requests.  # noqa: E501
 
-        :return: The deleted of this SubTransaction.  # noqa: E501
+        :return: The deleted of this ScheduledSubTransaction.  # noqa: E501
         :rtype: bool
         """
         return self._deleted
 
     @deleted.setter
     def deleted(self, deleted):
-        """Sets the deleted of this SubTransaction.
+        """Sets the deleted of this ScheduledSubTransaction.
 
-        Whether or not the subtransaction has been deleted.  Deleted subtransactions will only be included in delta requests.  # noqa: E501
+        Whether or not the scheduled subtransaction has been deleted.  Deleted scheduled subtransactions will only be included in delta requests.  # noqa: E501
 
-        :param deleted: The deleted of this SubTransaction.  # noqa: E501
+        :param deleted: The deleted of this ScheduledSubTransaction.  # noqa: E501
         :type: bool
         """
         if deleted is None:
             raise ValueError("Invalid value for `deleted`, must not be `None`")  # noqa: E501
 
         self._deleted = deleted
 
     @property
     def id(self):
-        """Gets the id of this SubTransaction.  # noqa: E501
+        """Gets the id of this ScheduledSubTransaction.  # noqa: E501
 
 
-        :return: The id of this SubTransaction.  # noqa: E501
+        :return: The id of this ScheduledSubTransaction.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this SubTransaction.
+        """Sets the id of this ScheduledSubTransaction.
 
 
-        :param id: The id of this SubTransaction.  # noqa: E501
+        :param id: The id of this ScheduledSubTransaction.  # noqa: E501
         :type: str
         """
         if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def memo(self):
-        """Gets the memo of this SubTransaction.  # noqa: E501
+        """Gets the memo of this ScheduledSubTransaction.  # noqa: E501
 
 
-        :return: The memo of this SubTransaction.  # noqa: E501
+        :return: The memo of this ScheduledSubTransaction.  # noqa: E501
         :rtype: str
         """
         return self._memo
 
     @memo.setter
     def memo(self, memo):
-        """Sets the memo of this SubTransaction.
+        """Sets the memo of this ScheduledSubTransaction.
 
 
-        :param memo: The memo of this SubTransaction.  # noqa: E501
+        :param memo: The memo of this ScheduledSubTransaction.  # noqa: E501
         :type: str
         """
-        if memo is None:
-            raise ValueError("Invalid value for `memo`, must not be `None`")  # noqa: E501
 
         self._memo = memo
 
     @property
     def payee_id(self):
-        """Gets the payee_id of this SubTransaction.  # noqa: E501
+        """Gets the payee_id of this ScheduledSubTransaction.  # noqa: E501
 
 
-        :return: The payee_id of this SubTransaction.  # noqa: E501
+        :return: The payee_id of this ScheduledSubTransaction.  # noqa: E501
         :rtype: str
         """
         return self._payee_id
 
     @payee_id.setter
     def payee_id(self, payee_id):
-        """Sets the payee_id of this SubTransaction.
+        """Sets the payee_id of this ScheduledSubTransaction.
 
 
-        :param payee_id: The payee_id of this SubTransaction.  # noqa: E501
+        :param payee_id: The payee_id of this ScheduledSubTransaction.  # noqa: E501
         :type: str
         """
 
         self._payee_id = payee_id
 
     @property
-    def transaction_id(self):
-        """Gets the transaction_id of this SubTransaction.  # noqa: E501
+    def scheduled_transaction_id(self):
+        """Gets the scheduled_transaction_id of this ScheduledSubTransaction.  # noqa: E501
 
 
-        :return: The transaction_id of this SubTransaction.  # noqa: E501
+        :return: The scheduled_transaction_id of this ScheduledSubTransaction.  # noqa: E501
         :rtype: str
         """
-        return self._transaction_id
+        return self._scheduled_transaction_id
 
-    @transaction_id.setter
-    def transaction_id(self, transaction_id):
-        """Sets the transaction_id of this SubTransaction.
+    @scheduled_transaction_id.setter
+    def scheduled_transaction_id(self, scheduled_transaction_id):
+        """Sets the scheduled_transaction_id of this ScheduledSubTransaction.
 
 
-        :param transaction_id: The transaction_id of this SubTransaction.  # noqa: E501
+        :param scheduled_transaction_id: The scheduled_transaction_id of this ScheduledSubTransaction.  # noqa: E501
         :type: str
         """
-        if transaction_id is None:
-            raise ValueError("Invalid value for `transaction_id`, must not be `None`")  # noqa: E501
+        if scheduled_transaction_id is None:
+            raise ValueError("Invalid value for `scheduled_transaction_id`, must not be `None`")  # noqa: E501
 
-        self._transaction_id = transaction_id
+        self._scheduled_transaction_id = scheduled_transaction_id
 
     @property
     def transfer_account_id(self):
-        """Gets the transfer_account_id of this SubTransaction.  # noqa: E501
+        """Gets the transfer_account_id of this ScheduledSubTransaction.  # noqa: E501
 
-        If a transfer, the account_id which the subtransaction transfers to  # noqa: E501
+        If a transfer, the account_id which the scheduled subtransaction transfers to  # noqa: E501
 
-        :return: The transfer_account_id of this SubTransaction.  # noqa: E501
+        :return: The transfer_account_id of this ScheduledSubTransaction.  # noqa: E501
         :rtype: str
         """
         return self._transfer_account_id
 
     @transfer_account_id.setter
     def transfer_account_id(self, transfer_account_id):
-        """Sets the transfer_account_id of this SubTransaction.
+        """Sets the transfer_account_id of this ScheduledSubTransaction.
 
-        If a transfer, the account_id which the subtransaction transfers to  # noqa: E501
+        If a transfer, the account_id which the scheduled subtransaction transfers to  # noqa: E501
 
-        :param transfer_account_id: The transfer_account_id of this SubTransaction.  # noqa: E501
+        :param transfer_account_id: The transfer_account_id of this ScheduledSubTransaction.  # noqa: E501
         :type: str
         """
 
         self._transfer_account_id = transfer_account_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -291,15 +291,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SubTransaction):
+        if not isinstance(other, ScheduledSubTransaction):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `pyynab-0.8.8/ynab/models/budget_detail_response.py` & `pyynab-0.9.0/ynab/models/budget_detail_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/scheduled_transaction_detail.py` & `pyynab-0.9.0/ynab/models/scheduled_transaction_detail.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,27 +88,34 @@
         self._category_name = None
         self._payee_name = None
         self._subtransactions = None
         self.discriminator = None
 
         self.account_id = account_id
         self.amount = amount
-        self.category_id = category_id
+        if category_id is not None:
+            self.category_id = category_id
         self.date_first = date_first
         self.date_next = date_next
         self.deleted = deleted
-        self.flag_color = flag_color
+        if flag_color is not None:
+            self.flag_color = flag_color
         self.frequency = frequency
         self.id = id
-        self.memo = memo
-        self.payee_id = payee_id
-        self.transfer_account_id = transfer_account_id
+        if memo is not None:
+            self.memo = memo
+        if payee_id is not None:
+            self.payee_id = payee_id
+        if transfer_account_id is not None:
+            self.transfer_account_id = transfer_account_id
         self.account_name = account_name
-        self.category_name = category_name
-        self.payee_name = payee_name
+        if category_name is not None:
+            self.category_name = category_name
+        if payee_name is not None:
+            self.payee_name = payee_name
         self.subtransactions = subtransactions
 
     @property
     def account_id(self):
         """Gets the account_id of this ScheduledTransactionDetail.  # noqa: E501
 
 
@@ -169,16 +176,14 @@
     def category_id(self, category_id):
         """Sets the category_id of this ScheduledTransactionDetail.
 
 
         :param category_id: The category_id of this ScheduledTransactionDetail.  # noqa: E501
         :type: str
         """
-        if category_id is None:
-            raise ValueError("Invalid value for `category_id`, must not be `None`")  # noqa: E501
 
         self._category_id = category_id
 
     @property
     def date_first(self):
         """Gets the date_first of this ScheduledTransactionDetail.  # noqa: E501
 
@@ -269,16 +274,14 @@
         """Sets the flag_color of this ScheduledTransactionDetail.
 
         The scheduled transaction flag  # noqa: E501
 
         :param flag_color: The flag_color of this ScheduledTransactionDetail.  # noqa: E501
         :type: str
         """
-        if flag_color is None:
-            raise ValueError("Invalid value for `flag_color`, must not be `None`")  # noqa: E501
         allowed_values = ["red", "orange", "yellow", "green", "blue", "purple"]  # noqa: E501
         if flag_color not in allowed_values:
             raise ValueError(
                 "Invalid value for `flag_color` ({0}), must be one of {1}"  # noqa: E501
                 .format(flag_color, allowed_values)
             )
 
@@ -350,16 +353,14 @@
     def memo(self, memo):
         """Sets the memo of this ScheduledTransactionDetail.
 
 
         :param memo: The memo of this ScheduledTransactionDetail.  # noqa: E501
         :type: str
         """
-        if memo is None:
-            raise ValueError("Invalid value for `memo`, must not be `None`")  # noqa: E501
 
         self._memo = memo
 
     @property
     def payee_id(self):
         """Gets the payee_id of this ScheduledTransactionDetail.  # noqa: E501
 
@@ -373,16 +374,14 @@
     def payee_id(self, payee_id):
         """Sets the payee_id of this ScheduledTransactionDetail.
 
 
         :param payee_id: The payee_id of this ScheduledTransactionDetail.  # noqa: E501
         :type: str
         """
-        if payee_id is None:
-            raise ValueError("Invalid value for `payee_id`, must not be `None`")  # noqa: E501
 
         self._payee_id = payee_id
 
     @property
     def transfer_account_id(self):
         """Gets the transfer_account_id of this ScheduledTransactionDetail.  # noqa: E501
 
@@ -398,16 +397,14 @@
         """Sets the transfer_account_id of this ScheduledTransactionDetail.
 
         If a transfer, the account_id which the scheduled transaction transfers to  # noqa: E501
 
         :param transfer_account_id: The transfer_account_id of this ScheduledTransactionDetail.  # noqa: E501
         :type: str
         """
-        if transfer_account_id is None:
-            raise ValueError("Invalid value for `transfer_account_id`, must not be `None`")  # noqa: E501
 
         self._transfer_account_id = transfer_account_id
 
     @property
     def account_name(self):
         """Gets the account_name of this ScheduledTransactionDetail.  # noqa: E501
 
@@ -444,16 +441,14 @@
     def category_name(self, category_name):
         """Sets the category_name of this ScheduledTransactionDetail.
 
 
         :param category_name: The category_name of this ScheduledTransactionDetail.  # noqa: E501
         :type: str
         """
-        if category_name is None:
-            raise ValueError("Invalid value for `category_name`, must not be `None`")  # noqa: E501
 
         self._category_name = category_name
 
     @property
     def payee_name(self):
         """Gets the payee_name of this ScheduledTransactionDetail.  # noqa: E501
 
@@ -467,16 +462,14 @@
     def payee_name(self, payee_name):
         """Sets the payee_name of this ScheduledTransactionDetail.
 
 
         :param payee_name: The payee_name of this ScheduledTransactionDetail.  # noqa: E501
         :type: str
         """
-        if payee_name is None:
-            raise ValueError("Invalid value for `payee_name`, must not be `None`")  # noqa: E501
 
         self._payee_name = payee_name
 
     @property
     def subtransactions(self):
         """Gets the subtransactions of this ScheduledTransactionDetail.  # noqa: E501
```

### Comparing `pyynab-0.8.8/ynab/models/date_format.py` & `pyynab-0.9.0/ynab/models/date_format.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/transactions_response.py` & `pyynab-0.9.0/ynab/models/transactions_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/accounts_response_data.py` & `pyynab-0.9.0/ynab/models/accounts_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/save_transaction.py` & `pyynab-0.9.0/ynab/models/save_transaction.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,45 +38,48 @@
         'category_id': 'str',
         'cleared': 'str',
         'date': 'date',
         'flag_color': 'str',
         'import_id': 'str',
         'memo': 'str',
         'payee_id': 'str',
-        'payee_name': 'str'
+        'payee_name': 'str',
+        'subtransactions': 'list[SaveSubTransaction]'
     }
 
     attribute_map = {
         'account_id': 'account_id',
         'amount': 'amount',
         'approved': 'approved',
         'category_id': 'category_id',
         'cleared': 'cleared',
         'date': 'date',
         'flag_color': 'flag_color',
         'import_id': 'import_id',
         'memo': 'memo',
         'payee_id': 'payee_id',
-        'payee_name': 'payee_name'
+        'payee_name': 'payee_name',
+        'subtransactions': 'subtransactions'
     }
 
-    def __init__(self, account_id=None, amount=None, approved=None, category_id=None, cleared=None, date=None, flag_color=None, import_id=None, memo=None, payee_id=None, payee_name=None):  # noqa: E501
+    def __init__(self, account_id=None, amount=None, approved=None, category_id=None, cleared=None, date=None, flag_color=None, import_id=None, memo=None, payee_id=None, payee_name=None, subtransactions=None):  # noqa: E501
         """SaveTransaction - a model defined in OpenAPI"""  # noqa: E501
 
         self._account_id = None
         self._amount = None
         self._approved = None
         self._category_id = None
         self._cleared = None
         self._date = None
         self._flag_color = None
         self._import_id = None
         self._memo = None
         self._payee_id = None
         self._payee_name = None
+        self._subtransactions = None
         self.discriminator = None
 
         self.account_id = account_id
         self.amount = amount
         if approved is not None:
             self.approved = approved
         if category_id is not None:
@@ -90,14 +93,16 @@
             self.import_id = import_id
         if memo is not None:
             self.memo = memo
         if payee_id is not None:
             self.payee_id = payee_id
         if payee_name is not None:
             self.payee_name = payee_name
+        if subtransactions is not None:
+            self.subtransactions = subtransactions
 
     @property
     def account_id(self):
         """Gets the account_id of this SaveTransaction.  # noqa: E501
 
 
         :return: The account_id of this SaveTransaction.  # noqa: E501
@@ -166,26 +171,26 @@
 
         self._approved = approved
 
     @property
     def category_id(self):
         """Gets the category_id of this SaveTransaction.  # noqa: E501
 
-        The category for the transaction.  Split and Credit Card Payment categories are not permitted and will be ignored if supplied.  If an existing transaction has a Split category it cannot be changed.  # noqa: E501
+        The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.  # noqa: E501
 
         :return: The category_id of this SaveTransaction.  # noqa: E501
         :rtype: str
         """
         return self._category_id
 
     @category_id.setter
     def category_id(self, category_id):
         """Sets the category_id of this SaveTransaction.
 
-        The category for the transaction.  Split and Credit Card Payment categories are not permitted and will be ignored if supplied.  If an existing transaction has a Split category it cannot be changed.  # noqa: E501
+        The category for the transaction.  To configure a split transaction, you can specify null for `category_id` and provide a `subtransactions` array as part of the transaction object.  If an existing transaction is a split, the `category_id` cannot be changed.  Credit Card Payment categories are not permitted and will be ignored if supplied.  # noqa: E501
 
         :param category_id: The category_id of this SaveTransaction.  # noqa: E501
         :type: str
         """
 
         self._category_id = category_id
 
@@ -272,26 +277,26 @@
 
         self._flag_color = flag_color
 
     @property
     def import_id(self):
         """Gets the import_id of this SaveTransaction.  # noqa: E501
 
-        If specified, the new transaction will be assigned this import_id and considered \"imported\". *At the time of import* we will attempt to match \"imported\" transactions with non-imported (i.e. \"user-entered\") transactions.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).  # noqa: E501
+        If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).  # noqa: E501
 
         :return: The import_id of this SaveTransaction.  # noqa: E501
         :rtype: str
         """
         return self._import_id
 
     @import_id.setter
     def import_id(self, import_id):
         """Sets the import_id of this SaveTransaction.
 
-        If specified, the new transaction will be assigned this import_id and considered \"imported\". *At the time of import* we will attempt to match \"imported\" transactions with non-imported (i.e. \"user-entered\") transactions.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).  # noqa: E501
+        If specified, the new transaction will be assigned this `import_id` and considered \"imported\".  We will also attempt to match this imported transaction to an existing \"user-entered\" transation on the same account, with the same amount, and with a date +/-10 days from the imported transaction date.<br><br>Transactions imported through File Based Import or Direct Import (not through the API) are assigned an import_id in the format: 'YNAB:[milliunit_amount]:[iso_date]:[occurrence]'. For example, a transaction dated 2015-12-30 in the amount of -$294.23 USD would have an import_id of 'YNAB:-294230:2015-12-30:1'.  If a second transaction on the same account was imported and had the same date and same amount, its import_id would be 'YNAB:-294230:2015-12-30:2'.  Using a consistent format will prevent duplicates through Direct Import and File Based Import.<br><br>If import_id is omitted or specified as null, the transaction will be treated as a \"user-entered\" transaction. As such, it will be eligible to be matched against transactions later being imported (via DI, FBI, or API).  # noqa: E501
 
         :param import_id: The import_id of this SaveTransaction.  # noqa: E501
         :type: str
         """
         if import_id is not None and len(import_id) > 36:
             raise ValueError("Invalid value for `import_id`, length must be less than or equal to `36`")  # noqa: E501
 
@@ -320,58 +325,81 @@
 
         self._memo = memo
 
     @property
     def payee_id(self):
         """Gets the payee_id of this SaveTransaction.  # noqa: E501
 
-        The payee for the transaction  # noqa: E501
+        The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.  # noqa: E501
 
         :return: The payee_id of this SaveTransaction.  # noqa: E501
         :rtype: str
         """
         return self._payee_id
 
     @payee_id.setter
     def payee_id(self, payee_id):
         """Sets the payee_id of this SaveTransaction.
 
-        The payee for the transaction  # noqa: E501
+        The payee for the transaction.  To create a transfer between two accounts, use the account transfer payee pointing to the target account.  Account transfer payees are specified as `tranfer_payee_id` on the account resource.  # noqa: E501
 
         :param payee_id: The payee_id of this SaveTransaction.  # noqa: E501
         :type: str
         """
 
         self._payee_id = payee_id
 
     @property
     def payee_name(self):
         """Gets the payee_name of this SaveTransaction.  # noqa: E501
 
-        The payee name.  If a payee_name value is provided and payee_id has a null value, the payee_name value will be used to resolve the payee by either (1) a matching payee rename rule (only if import_id is also specified) or (2) a payee with the same name or (3) creation of a new payee.  # noqa: E501
+        The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.  # noqa: E501
 
         :return: The payee_name of this SaveTransaction.  # noqa: E501
         :rtype: str
         """
         return self._payee_name
 
     @payee_name.setter
     def payee_name(self, payee_name):
         """Sets the payee_name of this SaveTransaction.
 
-        The payee name.  If a payee_name value is provided and payee_id has a null value, the payee_name value will be used to resolve the payee by either (1) a matching payee rename rule (only if import_id is also specified) or (2) a payee with the same name or (3) creation of a new payee.  # noqa: E501
+        The payee name.  If a `payee_name` value is provided and `payee_id` has a null value, the `payee_name` value will be used to resolve the payee by either (1) a matching payee rename rule (only if `import_id` is also specified) or (2) a payee with the same name or (3) creation of a new payee.  # noqa: E501
 
         :param payee_name: The payee_name of this SaveTransaction.  # noqa: E501
         :type: str
         """
         if payee_name is not None and len(payee_name) > 50:
             raise ValueError("Invalid value for `payee_name`, length must be less than or equal to `50`")  # noqa: E501
 
         self._payee_name = payee_name
 
+    @property
+    def subtransactions(self):
+        """Gets the subtransactions of this SaveTransaction.  # noqa: E501
+
+        An array of subtransactions to configure a transaction as a split.  Updating `subtransactions` on an existing split transaction is not supported.  # noqa: E501
+
+        :return: The subtransactions of this SaveTransaction.  # noqa: E501
+        :rtype: list[SaveSubTransaction]
+        """
+        return self._subtransactions
+
+    @subtransactions.setter
+    def subtransactions(self, subtransactions):
+        """Sets the subtransactions of this SaveTransaction.
+
+        An array of subtransactions to configure a transaction as a split.  Updating `subtransactions` on an existing split transaction is not supported.  # noqa: E501
+
+        :param subtransactions: The subtransactions of this SaveTransaction.  # noqa: E501
+        :type: list[SaveSubTransaction]
+        """
+
+        self._subtransactions = subtransactions
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `pyynab-0.8.8/ynab/models/budget_settings_response.py` & `pyynab-0.9.0/ynab/models/budget_settings_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/scheduled_transactions_response_data.py` & `pyynab-0.9.0/ynab/models/scheduled_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/budget_detail.py` & `pyynab-0.9.0/ynab/models/budget_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,89 +28,89 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'accounts': 'list[Account]',
         'currency_format': 'CurrencyFormat',
         'date_format': 'DateFormat',
         'first_month': 'date',
         'id': 'str',
         'last_modified_on': 'datetime',
         'last_month': 'date',
         'name': 'str',
-        'accounts': 'list[Account]',
         'categories': 'list[Category]',
         'category_groups': 'list[CategoryGroup]',
         'months': 'list[MonthDetail]',
         'payee_locations': 'list[PayeeLocation]',
         'payees': 'list[Payee]',
         'scheduled_subtransactions': 'list[ScheduledSubTransaction]',
         'scheduled_transactions': 'list[ScheduledTransactionSummary]',
         'subtransactions': 'list[SubTransaction]',
         'transactions': 'list[TransactionSummary]'
     }
 
     attribute_map = {
+        'accounts': 'accounts',
         'currency_format': 'currency_format',
         'date_format': 'date_format',
         'first_month': 'first_month',
         'id': 'id',
         'last_modified_on': 'last_modified_on',
         'last_month': 'last_month',
         'name': 'name',
-        'accounts': 'accounts',
         'categories': 'categories',
         'category_groups': 'category_groups',
         'months': 'months',
         'payee_locations': 'payee_locations',
         'payees': 'payees',
         'scheduled_subtransactions': 'scheduled_subtransactions',
         'scheduled_transactions': 'scheduled_transactions',
         'subtransactions': 'subtransactions',
         'transactions': 'transactions'
     }
 
-    def __init__(self, currency_format=None, date_format=None, first_month=None, id=None, last_modified_on=None, last_month=None, name=None, accounts=None, categories=None, category_groups=None, months=None, payee_locations=None, payees=None, scheduled_subtransactions=None, scheduled_transactions=None, subtransactions=None, transactions=None):  # noqa: E501
+    def __init__(self, accounts=None, currency_format=None, date_format=None, first_month=None, id=None, last_modified_on=None, last_month=None, name=None, categories=None, category_groups=None, months=None, payee_locations=None, payees=None, scheduled_subtransactions=None, scheduled_transactions=None, subtransactions=None, transactions=None):  # noqa: E501
         """BudgetDetail - a model defined in OpenAPI"""  # noqa: E501
 
+        self._accounts = None
         self._currency_format = None
         self._date_format = None
         self._first_month = None
         self._id = None
         self._last_modified_on = None
         self._last_month = None
         self._name = None
-        self._accounts = None
         self._categories = None
         self._category_groups = None
         self._months = None
         self._payee_locations = None
         self._payees = None
         self._scheduled_subtransactions = None
         self._scheduled_transactions = None
         self._subtransactions = None
         self._transactions = None
         self.discriminator = None
 
+        if accounts is not None:
+            self.accounts = accounts
         if currency_format is not None:
             self.currency_format = currency_format
         if date_format is not None:
             self.date_format = date_format
         if first_month is not None:
             self.first_month = first_month
         self.id = id
         if last_modified_on is not None:
             self.last_modified_on = last_modified_on
         if last_month is not None:
             self.last_month = last_month
         self.name = name
-        if accounts is not None:
-            self.accounts = accounts
         if categories is not None:
             self.categories = categories
         if category_groups is not None:
             self.category_groups = category_groups
         if months is not None:
             self.months = months
         if payee_locations is not None:
@@ -123,14 +123,35 @@
             self.scheduled_transactions = scheduled_transactions
         if subtransactions is not None:
             self.subtransactions = subtransactions
         if transactions is not None:
             self.transactions = transactions
 
     @property
+    def accounts(self):
+        """Gets the accounts of this BudgetDetail.  # noqa: E501
+
+
+        :return: The accounts of this BudgetDetail.  # noqa: E501
+        :rtype: list[Account]
+        """
+        return self._accounts
+
+    @accounts.setter
+    def accounts(self, accounts):
+        """Sets the accounts of this BudgetDetail.
+
+
+        :param accounts: The accounts of this BudgetDetail.  # noqa: E501
+        :type: list[Account]
+        """
+
+        self._accounts = accounts
+
+    @property
     def currency_format(self):
         """Gets the currency_format of this BudgetDetail.  # noqa: E501
 
 
         :return: The currency_format of this BudgetDetail.  # noqa: E501
         :rtype: CurrencyFormat
         """
@@ -280,35 +301,14 @@
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
-    def accounts(self):
-        """Gets the accounts of this BudgetDetail.  # noqa: E501
-
-
-        :return: The accounts of this BudgetDetail.  # noqa: E501
-        :rtype: list[Account]
-        """
-        return self._accounts
-
-    @accounts.setter
-    def accounts(self, accounts):
-        """Sets the accounts of this BudgetDetail.
-
-
-        :param accounts: The accounts of this BudgetDetail.  # noqa: E501
-        :type: list[Account]
-        """
-
-        self._accounts = accounts
-
-    @property
     def categories(self):
         """Gets the categories of this BudgetDetail.  # noqa: E501
 
 
         :return: The categories of this BudgetDetail.  # noqa: E501
         :rtype: list[Category]
         """
```

### Comparing `pyynab-0.8.8/ynab/models/payee_location.py` & `pyynab-0.9.0/ynab/models/payee_location.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/category_response.py` & `pyynab-0.9.0/ynab/models/category_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/month_summaries_response.py` & `pyynab-0.9.0/ynab/models/month_summaries_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/error_response.py` & `pyynab-0.9.0/ynab/models/error_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/transaction_detail_all_of.py` & `pyynab-0.9.0/ynab/models/transaction_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/bulk_response_data_bulk.py` & `pyynab-0.9.0/ynab/models/bulk_response_data_bulk.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,26 @@
         self.duplicate_import_ids = duplicate_import_ids
         self.transaction_ids = transaction_ids
 
     @property
     def duplicate_import_ids(self):
         """Gets the duplicate_import_ids of this BulkResponseDataBulk.  # noqa: E501
 
-        If any Transactions were not created because they had an import_id matching a transaction already on the same account, the specified import_id(s) will be included in this list.  # noqa: E501
+        If any Transactions were not created because they had an `import_id` matching a transaction already on the same account, the specified import_id(s) will be included in this list.  # noqa: E501
 
         :return: The duplicate_import_ids of this BulkResponseDataBulk.  # noqa: E501
         :rtype: list[str]
         """
         return self._duplicate_import_ids
 
     @duplicate_import_ids.setter
     def duplicate_import_ids(self, duplicate_import_ids):
         """Sets the duplicate_import_ids of this BulkResponseDataBulk.
 
-        If any Transactions were not created because they had an import_id matching a transaction already on the same account, the specified import_id(s) will be included in this list.  # noqa: E501
+        If any Transactions were not created because they had an `import_id` matching a transaction already on the same account, the specified import_id(s) will be included in this list.  # noqa: E501
 
         :param duplicate_import_ids: The duplicate_import_ids of this BulkResponseDataBulk.  # noqa: E501
         :type: list[str]
         """
         if duplicate_import_ids is None:
             raise ValueError("Invalid value for `duplicate_import_ids`, must not be `None`")  # noqa: E501
```

### Comparing `pyynab-0.8.8/ynab/models/hybrid_transactions_response_data.py` & `pyynab-0.9.0/ynab/models/hybrid_transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/category_group.py` & `pyynab-0.9.0/ynab/models/category_group.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/user_response_data.py` & `pyynab-0.9.0/ynab/models/user_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/payee_response.py` & `pyynab-0.9.0/ynab/models/payee_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/save_category_response.py` & `pyynab-0.9.0/ynab/models/save_category_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/payees_response.py` & `pyynab-0.9.0/ynab/models/payees_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/payee_locations_response.py` & `pyynab-0.9.0/ynab/models/payee_locations_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/save_transaction_wrapper.py` & `pyynab-0.9.0/ynab/models/save_transaction_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/category_response_data.py` & `pyynab-0.9.0/ynab/models/category_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/bulk_response_data.py` & `pyynab-0.9.0/ynab/models/bulk_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/category_group_with_categories.py` & `pyynab-0.9.0/ynab/models/category_group_with_categories.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/user_response.py` & `pyynab-0.9.0/ynab/models/user_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/save_transactions_response_data.py` & `pyynab-0.9.0/ynab/models/save_transactions_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,26 +66,26 @@
         if transactions is not None:
             self.transactions = transactions
 
     @property
     def duplicate_import_ids(self):
         """Gets the duplicate_import_ids of this SaveTransactionsResponseData.  # noqa: E501
 
-        If multiple transactions were specified, a list of import_ids that were not created because of an existing import_id found on the same account  # noqa: E501
+        If multiple transactions were specified, a list of import_ids that were not created because of an existing `import_id` found on the same account  # noqa: E501
 
         :return: The duplicate_import_ids of this SaveTransactionsResponseData.  # noqa: E501
         :rtype: list[str]
         """
         return self._duplicate_import_ids
 
     @duplicate_import_ids.setter
     def duplicate_import_ids(self, duplicate_import_ids):
         """Sets the duplicate_import_ids of this SaveTransactionsResponseData.
 
-        If multiple transactions were specified, a list of import_ids that were not created because of an existing import_id found on the same account  # noqa: E501
+        If multiple transactions were specified, a list of import_ids that were not created because of an existing `import_id` found on the same account  # noqa: E501
 
         :param duplicate_import_ids: The duplicate_import_ids of this SaveTransactionsResponseData.  # noqa: E501
         :type: list[str]
         """
 
         self._duplicate_import_ids = duplicate_import_ids
```

### Comparing `pyynab-0.8.8/ynab/models/categories_response.py` & `pyynab-0.9.0/ynab/models/categories_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/budget_detail_response_data.py` & `pyynab-0.9.0/ynab/models/budget_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/budget_summary.py` & `pyynab-0.9.0/ynab/models/budget_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,59 +28,87 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'accounts': 'list[Account]',
         'currency_format': 'CurrencyFormat',
         'date_format': 'DateFormat',
         'first_month': 'date',
         'id': 'str',
         'last_modified_on': 'datetime',
         'last_month': 'date',
         'name': 'str'
     }
 
     attribute_map = {
+        'accounts': 'accounts',
         'currency_format': 'currency_format',
         'date_format': 'date_format',
         'first_month': 'first_month',
         'id': 'id',
         'last_modified_on': 'last_modified_on',
         'last_month': 'last_month',
         'name': 'name'
     }
 
-    def __init__(self, currency_format=None, date_format=None, first_month=None, id=None, last_modified_on=None, last_month=None, name=None):  # noqa: E501
+    def __init__(self, accounts=None, currency_format=None, date_format=None, first_month=None, id=None, last_modified_on=None, last_month=None, name=None):  # noqa: E501
         """BudgetSummary - a model defined in OpenAPI"""  # noqa: E501
 
+        self._accounts = None
         self._currency_format = None
         self._date_format = None
         self._first_month = None
         self._id = None
         self._last_modified_on = None
         self._last_month = None
         self._name = None
         self.discriminator = None
 
+        if accounts is not None:
+            self.accounts = accounts
         if currency_format is not None:
             self.currency_format = currency_format
         if date_format is not None:
             self.date_format = date_format
         if first_month is not None:
             self.first_month = first_month
         self.id = id
         if last_modified_on is not None:
             self.last_modified_on = last_modified_on
         if last_month is not None:
             self.last_month = last_month
         self.name = name
 
     @property
+    def accounts(self):
+        """Gets the accounts of this BudgetSummary.  # noqa: E501
+
+        The budget accounts (only included if `include_accounts=true` specified as query parameter)  # noqa: E501
+
+        :return: The accounts of this BudgetSummary.  # noqa: E501
+        :rtype: list[Account]
+        """
+        return self._accounts
+
+    @accounts.setter
+    def accounts(self, accounts):
+        """Sets the accounts of this BudgetSummary.
+
+        The budget accounts (only included if `include_accounts=true` specified as query parameter)  # noqa: E501
+
+        :param accounts: The accounts of this BudgetSummary.  # noqa: E501
+        :type: list[Account]
+        """
+
+        self._accounts = accounts
+
+    @property
     def currency_format(self):
         """Gets the currency_format of this BudgetSummary.  # noqa: E501
 
 
         :return: The currency_format of this BudgetSummary.  # noqa: E501
         :rtype: CurrencyFormat
         """
```

### Comparing `pyynab-0.8.8/ynab/models/save_month_category_wrapper.py` & `pyynab-0.9.0/ynab/models/save_month_category_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/scheduled_transaction_summary.py` & `pyynab-0.9.0/ynab/models/scheduled_transaction_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,24 +76,29 @@
         self._memo = None
         self._payee_id = None
         self._transfer_account_id = None
         self.discriminator = None
 
         self.account_id = account_id
         self.amount = amount
-        self.category_id = category_id
+        if category_id is not None:
+            self.category_id = category_id
         self.date_first = date_first
         self.date_next = date_next
         self.deleted = deleted
-        self.flag_color = flag_color
+        if flag_color is not None:
+            self.flag_color = flag_color
         self.frequency = frequency
         self.id = id
-        self.memo = memo
-        self.payee_id = payee_id
-        self.transfer_account_id = transfer_account_id
+        if memo is not None:
+            self.memo = memo
+        if payee_id is not None:
+            self.payee_id = payee_id
+        if transfer_account_id is not None:
+            self.transfer_account_id = transfer_account_id
 
     @property
     def account_id(self):
         """Gets the account_id of this ScheduledTransactionSummary.  # noqa: E501
 
 
         :return: The account_id of this ScheduledTransactionSummary.  # noqa: E501
@@ -153,16 +158,14 @@
     def category_id(self, category_id):
         """Sets the category_id of this ScheduledTransactionSummary.
 
 
         :param category_id: The category_id of this ScheduledTransactionSummary.  # noqa: E501
         :type: str
         """
-        if category_id is None:
-            raise ValueError("Invalid value for `category_id`, must not be `None`")  # noqa: E501
 
         self._category_id = category_id
 
     @property
     def date_first(self):
         """Gets the date_first of this ScheduledTransactionSummary.  # noqa: E501
 
@@ -253,16 +256,14 @@
         """Sets the flag_color of this ScheduledTransactionSummary.
 
         The scheduled transaction flag  # noqa: E501
 
         :param flag_color: The flag_color of this ScheduledTransactionSummary.  # noqa: E501
         :type: str
         """
-        if flag_color is None:
-            raise ValueError("Invalid value for `flag_color`, must not be `None`")  # noqa: E501
         allowed_values = ["red", "orange", "yellow", "green", "blue", "purple"]  # noqa: E501
         if flag_color not in allowed_values:
             raise ValueError(
                 "Invalid value for `flag_color` ({0}), must be one of {1}"  # noqa: E501
                 .format(flag_color, allowed_values)
             )
 
@@ -334,16 +335,14 @@
     def memo(self, memo):
         """Sets the memo of this ScheduledTransactionSummary.
 
 
         :param memo: The memo of this ScheduledTransactionSummary.  # noqa: E501
         :type: str
         """
-        if memo is None:
-            raise ValueError("Invalid value for `memo`, must not be `None`")  # noqa: E501
 
         self._memo = memo
 
     @property
     def payee_id(self):
         """Gets the payee_id of this ScheduledTransactionSummary.  # noqa: E501
 
@@ -357,16 +356,14 @@
     def payee_id(self, payee_id):
         """Sets the payee_id of this ScheduledTransactionSummary.
 
 
         :param payee_id: The payee_id of this ScheduledTransactionSummary.  # noqa: E501
         :type: str
         """
-        if payee_id is None:
-            raise ValueError("Invalid value for `payee_id`, must not be `None`")  # noqa: E501
 
         self._payee_id = payee_id
 
     @property
     def transfer_account_id(self):
         """Gets the transfer_account_id of this ScheduledTransactionSummary.  # noqa: E501
 
@@ -382,16 +379,14 @@
         """Sets the transfer_account_id of this ScheduledTransactionSummary.
 
         If a transfer, the account_id which the scheduled transaction transfers to  # noqa: E501
 
         :param transfer_account_id: The transfer_account_id of this ScheduledTransactionSummary.  # noqa: E501
         :type: str
         """
-        if transfer_account_id is None:
-            raise ValueError("Invalid value for `transfer_account_id`, must not be `None`")  # noqa: E501
 
         self._transfer_account_id = transfer_account_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `pyynab-0.8.8/ynab/models/save_transactions_wrapper.py` & `pyynab-0.9.0/ynab/models/save_transactions_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/hybrid_transactions_response.py` & `pyynab-0.9.0/ynab/models/hybrid_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/payee_location_response.py` & `pyynab-0.9.0/ynab/models/payee_location_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/scheduled_transactions_response.py` & `pyynab-0.9.0/ynab/models/scheduled_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/scheduled_transaction_response_data.py` & `pyynab-0.9.0/ynab/models/scheduled_transaction_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/month_summary.py` & `pyynab-0.9.0/ynab/models/month_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,38 +63,39 @@
         self._income = None
         self._month = None
         self._note = None
         self._to_be_budgeted = None
         self.discriminator = None
 
         self.activity = activity
-        self.age_of_money = age_of_money
+        if age_of_money is not None:
+            self.age_of_money = age_of_money
         self.budgeted = budgeted
         self.deleted = deleted
         self.income = income
         self.month = month
         self.note = note
         self.to_be_budgeted = to_be_budgeted
 
     @property
     def activity(self):
         """Gets the activity of this MonthSummary.  # noqa: E501
 
-        The total amount in transactions in the month, excluding those categorized to 'Inflow: To be Budgeted'  # noqa: E501
+        The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'  # noqa: E501
 
         :return: The activity of this MonthSummary.  # noqa: E501
         :rtype: int
         """
         return self._activity
 
     @activity.setter
     def activity(self, activity):
         """Sets the activity of this MonthSummary.
 
-        The total amount in transactions in the month, excluding those categorized to 'Inflow: To be Budgeted'  # noqa: E501
+        The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'  # noqa: E501
 
         :param activity: The activity of this MonthSummary.  # noqa: E501
         :type: int
         """
         if activity is None:
             raise ValueError("Invalid value for `activity`, must not be `None`")  # noqa: E501
 
@@ -116,16 +117,14 @@
         """Sets the age_of_money of this MonthSummary.
 
         The Age of Money as of the month  # noqa: E501
 
         :param age_of_money: The age_of_money of this MonthSummary.  # noqa: E501
         :type: int
         """
-        if age_of_money is None:
-            raise ValueError("Invalid value for `age_of_money`, must not be `None`")  # noqa: E501
 
         self._age_of_money = age_of_money
 
     @property
     def budgeted(self):
         """Gets the budgeted of this MonthSummary.  # noqa: E501
 
@@ -175,26 +174,26 @@
 
         self._deleted = deleted
 
     @property
     def income(self):
         """Gets the income of this MonthSummary.  # noqa: E501
 
-        The total amount in transactions categorized to 'Inflow: To be Budgeted' in the month  # noqa: E501
+        The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month  # noqa: E501
 
         :return: The income of this MonthSummary.  # noqa: E501
         :rtype: int
         """
         return self._income
 
     @income.setter
     def income(self, income):
         """Sets the income of this MonthSummary.
 
-        The total amount in transactions categorized to 'Inflow: To be Budgeted' in the month  # noqa: E501
+        The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month  # noqa: E501
 
         :param income: The income of this MonthSummary.  # noqa: E501
         :type: int
         """
         if income is None:
             raise ValueError("Invalid value for `income`, must not be `None`")  # noqa: E501
 
@@ -244,26 +243,26 @@
 
         self._note = note
 
     @property
     def to_be_budgeted(self):
         """Gets the to_be_budgeted of this MonthSummary.  # noqa: E501
 
-        The available amount for 'To be Budgeted'  # noqa: E501
+        The available amount for 'Ready to Assign'  # noqa: E501
 
         :return: The to_be_budgeted of this MonthSummary.  # noqa: E501
         :rtype: int
         """
         return self._to_be_budgeted
 
     @to_be_budgeted.setter
     def to_be_budgeted(self, to_be_budgeted):
         """Sets the to_be_budgeted of this MonthSummary.
 
-        The available amount for 'To be Budgeted'  # noqa: E501
+        The available amount for 'Ready to Assign'  # noqa: E501
 
         :param to_be_budgeted: The to_be_budgeted of this MonthSummary.  # noqa: E501
         :type: int
         """
         if to_be_budgeted is None:
             raise ValueError("Invalid value for `to_be_budgeted`, must not be `None`")  # noqa: E501
```

### Comparing `pyynab-0.8.8/ynab/models/transaction_response_data.py` & `pyynab-0.9.0/ynab/models/transaction_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/account_response.py` & `pyynab-0.9.0/ynab/models/account_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/save_month_category.py` & `pyynab-0.9.0/ynab/models/save_month_category.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/month_detail_all_of.py` & `pyynab-0.9.0/ynab/models/month_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/accounts_response.py` & `pyynab-0.9.0/ynab/models/accounts_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/budget_settings.py` & `pyynab-0.9.0/ynab/models/budget_settings.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/budget_settings_response_data.py` & `pyynab-0.9.0/ynab/models/budget_settings_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/month_detail.py` & `pyynab-0.9.0/ynab/models/month_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,39 +66,40 @@
         self._month = None
         self._note = None
         self._to_be_budgeted = None
         self._categories = None
         self.discriminator = None
 
         self.activity = activity
-        self.age_of_money = age_of_money
+        if age_of_money is not None:
+            self.age_of_money = age_of_money
         self.budgeted = budgeted
         self.deleted = deleted
         self.income = income
         self.month = month
         self.note = note
         self.to_be_budgeted = to_be_budgeted
         self.categories = categories
 
     @property
     def activity(self):
         """Gets the activity of this MonthDetail.  # noqa: E501
 
-        The total amount in transactions in the month, excluding those categorized to 'Inflow: To be Budgeted'  # noqa: E501
+        The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'  # noqa: E501
 
         :return: The activity of this MonthDetail.  # noqa: E501
         :rtype: int
         """
         return self._activity
 
     @activity.setter
     def activity(self, activity):
         """Sets the activity of this MonthDetail.
 
-        The total amount in transactions in the month, excluding those categorized to 'Inflow: To be Budgeted'  # noqa: E501
+        The total amount of transactions in the month, excluding those categorized to 'Inflow: Ready to Assign'  # noqa: E501
 
         :param activity: The activity of this MonthDetail.  # noqa: E501
         :type: int
         """
         if activity is None:
             raise ValueError("Invalid value for `activity`, must not be `None`")  # noqa: E501
 
@@ -120,16 +121,14 @@
         """Sets the age_of_money of this MonthDetail.
 
         The Age of Money as of the month  # noqa: E501
 
         :param age_of_money: The age_of_money of this MonthDetail.  # noqa: E501
         :type: int
         """
-        if age_of_money is None:
-            raise ValueError("Invalid value for `age_of_money`, must not be `None`")  # noqa: E501
 
         self._age_of_money = age_of_money
 
     @property
     def budgeted(self):
         """Gets the budgeted of this MonthDetail.  # noqa: E501
 
@@ -179,26 +178,26 @@
 
         self._deleted = deleted
 
     @property
     def income(self):
         """Gets the income of this MonthDetail.  # noqa: E501
 
-        The total amount in transactions categorized to 'Inflow: To be Budgeted' in the month  # noqa: E501
+        The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month  # noqa: E501
 
         :return: The income of this MonthDetail.  # noqa: E501
         :rtype: int
         """
         return self._income
 
     @income.setter
     def income(self, income):
         """Sets the income of this MonthDetail.
 
-        The total amount in transactions categorized to 'Inflow: To be Budgeted' in the month  # noqa: E501
+        The total amount of transactions categorized to 'Inflow: Ready to Assign' in the month  # noqa: E501
 
         :param income: The income of this MonthDetail.  # noqa: E501
         :type: int
         """
         if income is None:
             raise ValueError("Invalid value for `income`, must not be `None`")  # noqa: E501
 
@@ -248,26 +247,26 @@
 
         self._note = note
 
     @property
     def to_be_budgeted(self):
         """Gets the to_be_budgeted of this MonthDetail.  # noqa: E501
 
-        The available amount for 'To be Budgeted'  # noqa: E501
+        The available amount for 'Ready to Assign'  # noqa: E501
 
         :return: The to_be_budgeted of this MonthDetail.  # noqa: E501
         :rtype: int
         """
         return self._to_be_budgeted
 
     @to_be_budgeted.setter
     def to_be_budgeted(self, to_be_budgeted):
         """Sets the to_be_budgeted of this MonthDetail.
 
-        The available amount for 'To be Budgeted'  # noqa: E501
+        The available amount for 'Ready to Assign'  # noqa: E501
 
         :param to_be_budgeted: The to_be_budgeted of this MonthDetail.  # noqa: E501
         :type: int
         """
         if to_be_budgeted is None:
             raise ValueError("Invalid value for `to_be_budgeted`, must not be `None`")  # noqa: E501
```

### Comparing `pyynab-0.8.8/ynab/models/payee.py` & `pyynab-0.9.0/ynab/models/payee.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,26 +130,26 @@
 
         self._name = name
 
     @property
     def transfer_account_id(self):
         """Gets the transfer_account_id of this Payee.  # noqa: E501
 
-        If a transfer payee, the account_id to which this payee transfers to  # noqa: E501
+        If a transfer payee, the `account_id` to which this payee transfers to  # noqa: E501
 
         :return: The transfer_account_id of this Payee.  # noqa: E501
         :rtype: str
         """
         return self._transfer_account_id
 
     @transfer_account_id.setter
     def transfer_account_id(self, transfer_account_id):
         """Sets the transfer_account_id of this Payee.
 
-        If a transfer payee, the account_id to which this payee transfers to  # noqa: E501
+        If a transfer payee, the `account_id` to which this payee transfers to  # noqa: E501
 
         :param transfer_account_id: The transfer_account_id of this Payee.  # noqa: E501
         :type: str
         """
 
         self._transfer_account_id = transfer_account_id
```

### Comparing `pyynab-0.8.8/ynab/models/month_detail_response_data.py` & `pyynab-0.9.0/ynab/models/month_detail_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/transaction_detail.py` & `pyynab-0.9.0/ynab/models/transaction_detail.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/user.py` & `pyynab-0.9.0/ynab/models/user.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/month_detail_response.py` & `pyynab-0.9.0/ynab/models/month_detail_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/categories_response_data.py` & `pyynab-0.9.0/ynab/models/categories_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/payee_location_response_data.py` & `pyynab-0.9.0/ynab/models/payee_location_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/bulk_response.py` & `pyynab-0.9.0/ynab/models/bulk_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/hybrid_transaction.py` & `pyynab-0.9.0/ynab/models/hybrid_transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,20 @@
         self.import_id = import_id
         self.matched_transaction_id = matched_transaction_id
         self.memo = memo
         self.payee_id = payee_id
         self.transfer_account_id = transfer_account_id
         self.transfer_transaction_id = transfer_transaction_id
         self.account_name = account_name
-        self.category_name = category_name
-        self.parent_transaction_id = parent_transaction_id
-        self.payee_name = payee_name
+        if category_name is not None:
+            self.category_name = category_name
+        if parent_transaction_id is not None:
+            self.parent_transaction_id = parent_transaction_id
+        if payee_name is not None:
+            self.payee_name = payee_name
         self.type = type
 
     @property
     def account_id(self):
         """Gets the account_id of this HybridTransaction.  # noqa: E501
 
 
@@ -515,41 +518,37 @@
     def category_name(self, category_name):
         """Sets the category_name of this HybridTransaction.
 
 
         :param category_name: The category_name of this HybridTransaction.  # noqa: E501
         :type: str
         """
-        if category_name is None:
-            raise ValueError("Invalid value for `category_name`, must not be `None`")  # noqa: E501
 
         self._category_name = category_name
 
     @property
     def parent_transaction_id(self):
         """Gets the parent_transaction_id of this HybridTransaction.  # noqa: E501
 
-        For subtransaction types, this is the id of the pararent transaction.  For transaction types, this id will be always be null.  # noqa: E501
+        For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.  # noqa: E501
 
         :return: The parent_transaction_id of this HybridTransaction.  # noqa: E501
         :rtype: str
         """
         return self._parent_transaction_id
 
     @parent_transaction_id.setter
     def parent_transaction_id(self, parent_transaction_id):
         """Sets the parent_transaction_id of this HybridTransaction.
 
-        For subtransaction types, this is the id of the pararent transaction.  For transaction types, this id will be always be null.  # noqa: E501
+        For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.  # noqa: E501
 
         :param parent_transaction_id: The parent_transaction_id of this HybridTransaction.  # noqa: E501
         :type: str
         """
-        if parent_transaction_id is None:
-            raise ValueError("Invalid value for `parent_transaction_id`, must not be `None`")  # noqa: E501
 
         self._parent_transaction_id = parent_transaction_id
 
     @property
     def payee_name(self):
         """Gets the payee_name of this HybridTransaction.  # noqa: E501
 
@@ -563,16 +562,14 @@
     def payee_name(self, payee_name):
         """Sets the payee_name of this HybridTransaction.
 
 
         :param payee_name: The payee_name of this HybridTransaction.  # noqa: E501
         :type: str
         """
-        if payee_name is None:
-            raise ValueError("Invalid value for `payee_name`, must not be `None`")  # noqa: E501
 
         self._payee_name = payee_name
 
     @property
     def type(self):
         """Gets the type of this HybridTransaction.  # noqa: E501
```

### Comparing `pyynab-0.8.8/ynab/models/account.py` & `pyynab-0.9.0/ynab/models/account.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,57 +32,67 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'balance': 'int',
         'cleared_balance': 'int',
         'closed': 'bool',
         'deleted': 'bool',
+        'direct_import_in_error': 'bool',
+        'direct_import_linked': 'bool',
         'id': 'str',
         'name': 'str',
         'note': 'str',
         'on_budget': 'bool',
         'transfer_payee_id': 'str',
-        'type': 'str',
+        'type': 'AccountType',
         'uncleared_balance': 'int'
     }
 
     attribute_map = {
         'balance': 'balance',
         'cleared_balance': 'cleared_balance',
         'closed': 'closed',
         'deleted': 'deleted',
+        'direct_import_in_error': 'direct_import_in_error',
+        'direct_import_linked': 'direct_import_linked',
         'id': 'id',
         'name': 'name',
         'note': 'note',
         'on_budget': 'on_budget',
         'transfer_payee_id': 'transfer_payee_id',
         'type': 'type',
         'uncleared_balance': 'uncleared_balance'
     }
 
-    def __init__(self, balance=None, cleared_balance=None, closed=None, deleted=None, id=None, name=None, note=None, on_budget=None, transfer_payee_id=None, type=None, uncleared_balance=None):  # noqa: E501
+    def __init__(self, balance=None, cleared_balance=None, closed=None, deleted=None, direct_import_in_error=None, direct_import_linked=None, id=None, name=None, note=None, on_budget=None, transfer_payee_id=None, type=None, uncleared_balance=None):  # noqa: E501
         """Account - a model defined in OpenAPI"""  # noqa: E501
 
         self._balance = None
         self._cleared_balance = None
         self._closed = None
         self._deleted = None
+        self._direct_import_in_error = None
+        self._direct_import_linked = None
         self._id = None
         self._name = None
         self._note = None
         self._on_budget = None
         self._transfer_payee_id = None
         self._type = None
         self._uncleared_balance = None
         self.discriminator = None
 
         self.balance = balance
         self.cleared_balance = cleared_balance
         self.closed = closed
         self.deleted = deleted
+        if direct_import_in_error is not None:
+            self.direct_import_in_error = direct_import_in_error
+        if direct_import_linked is not None:
+            self.direct_import_linked = direct_import_linked
         self.id = id
         self.name = name
         self.note = note
         self.on_budget = on_budget
         self.transfer_payee_id = transfer_payee_id
         self.type = type
         self.uncleared_balance = uncleared_balance
@@ -184,14 +194,60 @@
         """
         if deleted is None:
             raise ValueError("Invalid value for `deleted`, must not be `None`")  # noqa: E501
 
         self._deleted = deleted
 
     @property
+    def direct_import_in_error(self):
+        """Gets the direct_import_in_error of this Account.  # noqa: E501
+
+        If an account linked to a financial institution (direct_import_linked=true) and the linked connection is not in a healthy state, this will be true.  # noqa: E501
+
+        :return: The direct_import_in_error of this Account.  # noqa: E501
+        :rtype: bool
+        """
+        return self._direct_import_in_error
+
+    @direct_import_in_error.setter
+    def direct_import_in_error(self, direct_import_in_error):
+        """Sets the direct_import_in_error of this Account.
+
+        If an account linked to a financial institution (direct_import_linked=true) and the linked connection is not in a healthy state, this will be true.  # noqa: E501
+
+        :param direct_import_in_error: The direct_import_in_error of this Account.  # noqa: E501
+        :type: bool
+        """
+
+        self._direct_import_in_error = direct_import_in_error
+
+    @property
+    def direct_import_linked(self):
+        """Gets the direct_import_linked of this Account.  # noqa: E501
+
+        Whether or not the account is linked to a financial institution for automatic transaction import.  # noqa: E501
+
+        :return: The direct_import_linked of this Account.  # noqa: E501
+        :rtype: bool
+        """
+        return self._direct_import_linked
+
+    @direct_import_linked.setter
+    def direct_import_linked(self, direct_import_linked):
+        """Sets the direct_import_linked of this Account.
+
+        Whether or not the account is linked to a financial institution for automatic transaction import.  # noqa: E501
+
+        :param direct_import_linked: The direct_import_linked of this Account.  # noqa: E501
+        :type: bool
+        """
+
+        self._direct_import_linked = direct_import_linked
+
+    @property
     def id(self):
         """Gets the id of this Account.  # noqa: E501
 
 
         :return: The id of this Account.  # noqa: E501
         :rtype: str
         """
@@ -304,38 +360,30 @@
 
         self._transfer_payee_id = transfer_payee_id
 
     @property
     def type(self):
         """Gets the type of this Account.  # noqa: E501
 
-        The type of account. Note: payPal, merchantAccount, investmentAccount, and mortgage types have been deprecated and will be removed in the future.  # noqa: E501
 
         :return: The type of this Account.  # noqa: E501
-        :rtype: str
+        :rtype: AccountType
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this Account.
 
-        The type of account. Note: payPal, merchantAccount, investmentAccount, and mortgage types have been deprecated and will be removed in the future.  # noqa: E501
 
         :param type: The type of this Account.  # noqa: E501
-        :type: str
+        :type: AccountType
         """
         if type is None:
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["checking", "savings", "cash", "creditCard", "lineOfCredit", "otherAsset", "otherLiability", "payPal", "merchantAccount", "investmentAccount", "mortgage"]  # noqa: E501
-        if type not in allowed_values:
-            raise ValueError(
-                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
-                .format(type, allowed_values)
-            )
 
         self._type = type
 
     @property
     def uncleared_balance(self):
         """Gets the uncleared_balance of this Account.  # noqa: E501
```

### Comparing `pyynab-0.8.8/ynab/models/error_detail.py` & `pyynab-0.9.0/ynab/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/save_category_response_data.py` & `pyynab-0.9.0/ynab/models/save_category_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/month_summaries_response_data.py` & `pyynab-0.9.0/ynab/models/month_summaries_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/save_transactions_response.py` & `pyynab-0.9.0/ynab/models/save_transactions_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/transaction_response.py` & `pyynab-0.9.0/ynab/models/transaction_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/payee_locations_response_data.py` & `pyynab-0.9.0/ynab/models/payee_locations_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/currency_format.py` & `pyynab-0.9.0/ynab/models/currency_format.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/account_response_data.py` & `pyynab-0.9.0/ynab/models/account_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/scheduled_transaction_detail_all_of.py` & `pyynab-0.9.0/ynab/models/scheduled_transaction_detail_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,16 +51,18 @@
         self._account_name = None
         self._category_name = None
         self._payee_name = None
         self._subtransactions = None
         self.discriminator = None
 
         self.account_name = account_name
-        self.category_name = category_name
-        self.payee_name = payee_name
+        if category_name is not None:
+            self.category_name = category_name
+        if payee_name is not None:
+            self.payee_name = payee_name
         self.subtransactions = subtransactions
 
     @property
     def account_name(self):
         """Gets the account_name of this ScheduledTransactionDetailAllOf.  # noqa: E501
 
 
@@ -96,16 +98,14 @@
     def category_name(self, category_name):
         """Sets the category_name of this ScheduledTransactionDetailAllOf.
 
 
         :param category_name: The category_name of this ScheduledTransactionDetailAllOf.  # noqa: E501
         :type: str
         """
-        if category_name is None:
-            raise ValueError("Invalid value for `category_name`, must not be `None`")  # noqa: E501
 
         self._category_name = category_name
 
     @property
     def payee_name(self):
         """Gets the payee_name of this ScheduledTransactionDetailAllOf.  # noqa: E501
 
@@ -119,16 +119,14 @@
     def payee_name(self, payee_name):
         """Sets the payee_name of this ScheduledTransactionDetailAllOf.
 
 
         :param payee_name: The payee_name of this ScheduledTransactionDetailAllOf.  # noqa: E501
         :type: str
         """
-        if payee_name is None:
-            raise ValueError("Invalid value for `payee_name`, must not be `None`")  # noqa: E501
 
         self._payee_name = payee_name
 
     @property
     def subtransactions(self):
         """Gets the subtransactions of this ScheduledTransactionDetailAllOf.  # noqa: E501
```

### Comparing `pyynab-0.8.8/ynab/models/hybrid_transaction_all_of.py` & `pyynab-0.9.0/ynab/models/hybrid_transaction_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,17 +54,20 @@
         self._category_name = None
         self._parent_transaction_id = None
         self._payee_name = None
         self._type = None
         self.discriminator = None
 
         self.account_name = account_name
-        self.category_name = category_name
-        self.parent_transaction_id = parent_transaction_id
-        self.payee_name = payee_name
+        if category_name is not None:
+            self.category_name = category_name
+        if parent_transaction_id is not None:
+            self.parent_transaction_id = parent_transaction_id
+        if payee_name is not None:
+            self.payee_name = payee_name
         self.type = type
 
     @property
     def account_name(self):
         """Gets the account_name of this HybridTransactionAllOf.  # noqa: E501
 
 
@@ -100,41 +103,37 @@
     def category_name(self, category_name):
         """Sets the category_name of this HybridTransactionAllOf.
 
 
         :param category_name: The category_name of this HybridTransactionAllOf.  # noqa: E501
         :type: str
         """
-        if category_name is None:
-            raise ValueError("Invalid value for `category_name`, must not be `None`")  # noqa: E501
 
         self._category_name = category_name
 
     @property
     def parent_transaction_id(self):
         """Gets the parent_transaction_id of this HybridTransactionAllOf.  # noqa: E501
 
-        For subtransaction types, this is the id of the pararent transaction.  For transaction types, this id will be always be null.  # noqa: E501
+        For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.  # noqa: E501
 
         :return: The parent_transaction_id of this HybridTransactionAllOf.  # noqa: E501
         :rtype: str
         """
         return self._parent_transaction_id
 
     @parent_transaction_id.setter
     def parent_transaction_id(self, parent_transaction_id):
         """Sets the parent_transaction_id of this HybridTransactionAllOf.
 
-        For subtransaction types, this is the id of the pararent transaction.  For transaction types, this id will be always be null.  # noqa: E501
+        For subtransaction types, this is the id of the parent transaction.  For transaction types, this id will be always be null.  # noqa: E501
 
         :param parent_transaction_id: The parent_transaction_id of this HybridTransactionAllOf.  # noqa: E501
         :type: str
         """
-        if parent_transaction_id is None:
-            raise ValueError("Invalid value for `parent_transaction_id`, must not be `None`")  # noqa: E501
 
         self._parent_transaction_id = parent_transaction_id
 
     @property
     def payee_name(self):
         """Gets the payee_name of this HybridTransactionAllOf.  # noqa: E501
 
@@ -148,16 +147,14 @@
     def payee_name(self, payee_name):
         """Sets the payee_name of this HybridTransactionAllOf.
 
 
         :param payee_name: The payee_name of this HybridTransactionAllOf.  # noqa: E501
         :type: str
         """
-        if payee_name is None:
-            raise ValueError("Invalid value for `payee_name`, must not be `None`")  # noqa: E501
 
         self._payee_name = payee_name
 
     @property
     def type(self):
         """Gets the type of this HybridTransactionAllOf.  # noqa: E501
```

### Comparing `pyynab-0.8.8/ynab/models/bulk_transactions.py` & `pyynab-0.9.0/ynab/models/bulk_transactions.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/budget_summary_response_data.py` & `pyynab-0.9.0/ynab/models/budget_summary_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         """BudgetSummaryResponseData - a model defined in OpenAPI"""  # noqa: E501
 
         self._budgets = None
         self._default_budget = None
         self.discriminator = None
 
         self.budgets = budgets
-        self.default_budget = default_budget
+        if default_budget is not None:
+            self.default_budget = default_budget
 
     @property
     def budgets(self):
         """Gets the budgets of this BudgetSummaryResponseData.  # noqa: E501
 
 
         :return: The budgets of this BudgetSummaryResponseData.  # noqa: E501
@@ -88,16 +89,14 @@
     def default_budget(self, default_budget):
         """Sets the default_budget of this BudgetSummaryResponseData.
 
 
         :param default_budget: The default_budget of this BudgetSummaryResponseData.  # noqa: E501
         :type: BudgetSummary
         """
-        if default_budget is None:
-            raise ValueError("Invalid value for `default_budget`, must not be `None`")  # noqa: E501
 
         self._default_budget = default_budget
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `pyynab-0.8.8/ynab/models/budget_detail_all_of.py` & `pyynab-0.9.0/ynab/models/budget_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/transaction_summary.py` & `pyynab-0.9.0/ynab/models/transaction_summary.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/__init__.py` & `pyynab-0.9.0/ynab/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import absolute_import
 
 # import models into model package
 from ynab.models.account import Account
 from ynab.models.account_response import AccountResponse
 from ynab.models.account_response_data import AccountResponseData
+from ynab.models.account_type import AccountType
 from ynab.models.accounts_response import AccountsResponse
 from ynab.models.accounts_response_data import AccountsResponseData
 from ynab.models.budget_detail import BudgetDetail
 from ynab.models.budget_detail_all_of import BudgetDetailAllOf
 from ynab.models.budget_detail_response import BudgetDetailResponse
 from ynab.models.budget_detail_response_data import BudgetDetailResponseData
 from ynab.models.budget_settings import BudgetSettings
@@ -63,18 +64,21 @@
 from ynab.models.payee_location_response_data import PayeeLocationResponseData
 from ynab.models.payee_locations_response import PayeeLocationsResponse
 from ynab.models.payee_locations_response_data import PayeeLocationsResponseData
 from ynab.models.payee_response import PayeeResponse
 from ynab.models.payee_response_data import PayeeResponseData
 from ynab.models.payees_response import PayeesResponse
 from ynab.models.payees_response_data import PayeesResponseData
+from ynab.models.save_account import SaveAccount
+from ynab.models.save_account_wrapper import SaveAccountWrapper
 from ynab.models.save_category_response import SaveCategoryResponse
 from ynab.models.save_category_response_data import SaveCategoryResponseData
 from ynab.models.save_month_category import SaveMonthCategory
 from ynab.models.save_month_category_wrapper import SaveMonthCategoryWrapper
+from ynab.models.save_sub_transaction import SaveSubTransaction
 from ynab.models.save_transaction import SaveTransaction
 from ynab.models.save_transaction_wrapper import SaveTransactionWrapper
 from ynab.models.save_transactions_response import SaveTransactionsResponse
 from ynab.models.save_transactions_response_data import SaveTransactionsResponseData
 from ynab.models.save_transactions_wrapper import SaveTransactionsWrapper
 from ynab.models.scheduled_sub_transaction import ScheduledSubTransaction
 from ynab.models.scheduled_transaction_detail import ScheduledTransactionDetail
@@ -86,12 +90,17 @@
 from ynab.models.scheduled_transactions_response_data import ScheduledTransactionsResponseData
 from ynab.models.sub_transaction import SubTransaction
 from ynab.models.transaction_detail import TransactionDetail
 from ynab.models.transaction_detail_all_of import TransactionDetailAllOf
 from ynab.models.transaction_response import TransactionResponse
 from ynab.models.transaction_response_data import TransactionResponseData
 from ynab.models.transaction_summary import TransactionSummary
+from ynab.models.transactions_import_response import TransactionsImportResponse
+from ynab.models.transactions_import_response_data import TransactionsImportResponseData
 from ynab.models.transactions_response import TransactionsResponse
 from ynab.models.transactions_response_data import TransactionsResponseData
+from ynab.models.update_transaction import UpdateTransaction
+from ynab.models.update_transaction_all_of import UpdateTransactionAllOf
+from ynab.models.update_transactions_wrapper import UpdateTransactionsWrapper
 from ynab.models.user import User
 from ynab.models.user_response import UserResponse
 from ynab.models.user_response_data import UserResponseData
```

### Comparing `pyynab-0.8.8/ynab/models/payees_response_data.py` & `pyynab-0.9.0/ynab/models/payees_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/transactions_response_data.py` & `pyynab-0.9.0/ynab/models/transactions_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/payee_response_data.py` & `pyynab-0.9.0/ynab/models/payee_response_data.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/scheduled_transaction_response.py` & `pyynab-0.9.0/ynab/models/scheduled_transaction_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/models/budget_summary_response.py` & `pyynab-0.9.0/ynab/models/budget_summary_response.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/api_client.py` & `pyynab-0.9.0/ynab/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.8.8/python'
+        self.user_agent = 'OpenAPI-Generator/0.9.0/python'
 
     def __del__(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
```

### Comparing `pyynab-0.8.8/ynab/configuration.py` & `pyynab-0.9.0/ynab/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.8.8".\
+               "SDK Package Version: 0.9.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pyynab-0.8.8/ynab/exceptions.py` & `pyynab-0.9.0/ynab/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/api/payees_api.py` & `pyynab-0.9.0/ynab/api/payees_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,22 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def get_payee_by_id(self, budget_id, payee_id, **kwargs):  # noqa: E501
         """Single payee  # noqa: E501
 
-        Returns single payee  # noqa: E501
+        Returns a single payee  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payee_by_id(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str payee_id: The id of the payee (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -62,22 +62,22 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.get_payee_by_id_with_http_info(budget_id, payee_id, **kwargs)  # noqa: E501
 
     def get_payee_by_id_with_http_info(self, budget_id, payee_id, **kwargs):  # noqa: E501
         """Single payee  # noqa: E501
 
-        Returns single payee  # noqa: E501
+        Returns a single payee  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payee_by_id_with_http_info(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str payee_id: The id of the payee (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -159,16 +159,16 @@
         Returns all payees  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payees(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -185,16 +185,16 @@
         Returns all payees  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payees_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `pyynab-0.8.8/ynab/api/user_api.py` & `pyynab-0.9.0/ynab/api/user_api.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/api/accounts_api.py` & `pyynab-0.9.0/ynab/api/accounts_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,25 +33,141 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
+    def create_account(self, budget_id, data, **kwargs):  # noqa: E501
+        """Create a new account  # noqa: E501
+
+        Creates a new account  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_account(budget_id, data, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param SaveAccountWrapper data: The account to create. (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: AccountResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.create_account_with_http_info(budget_id, data, **kwargs)  # noqa: E501
+
+    def create_account_with_http_info(self, budget_id, data, **kwargs):  # noqa: E501
+        """Create a new account  # noqa: E501
+
+        Creates a new account  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.create_account_with_http_info(budget_id, data, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param SaveAccountWrapper data: The account to create. (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(AccountResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['budget_id', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_account" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'budget_id' is set
+        if ('budget_id' not in local_var_params or
+                local_var_params['budget_id'] is None):
+            raise ApiValueError("Missing the required parameter `budget_id` when calling `create_account`")  # noqa: E501
+        # verify the required parameter 'data' is set
+        if ('data' not in local_var_params or
+                local_var_params['data'] is None):
+            raise ApiValueError("Missing the required parameter `data` when calling `create_account`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'budget_id' in local_var_params:
+            path_params['budget_id'] = local_var_params['budget_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in local_var_params:
+            body_params = local_var_params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['bearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/budgets/{budget_id}/accounts', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='AccountResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_account_by_id(self, budget_id, account_id, **kwargs):  # noqa: E501
         """Single account  # noqa: E501
 
         Returns a single account  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_account_by_id(budget_id, account_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str account_id: The id of the account (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -69,15 +185,15 @@
         Returns a single account  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_account_by_id_with_http_info(budget_id, account_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str account_id: The id of the account (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -159,16 +275,16 @@
         Returns all accounts  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_accounts(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -185,16 +301,16 @@
         Returns all accounts  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_accounts_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `pyynab-0.8.8/ynab/api/budgets_api.py` & `pyynab-0.9.0/ynab/api/budgets_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         Returns a single budget with all related entities.  This resource is effectively a full budget export.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budget_by_id(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -69,16 +69,16 @@
         Returns a single budget with all related entities.  This resource is effectively a full budget export.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budget_by_id_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -155,15 +155,15 @@
         Returns settings for a budget  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budget_settings_by_id(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -180,15 +180,15 @@
         Returns settings for a budget  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budget_settings_by_id_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -263,14 +263,15 @@
         Returns budgets list with summary information  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budgets(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param bool include_accounts: Whether to include the list of budget accounts
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -287,14 +288,15 @@
         Returns budgets list with summary information  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budgets_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param bool include_accounts: Whether to include the list of budget accounts
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -303,15 +305,15 @@
         :return: tuple(BudgetSummaryResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
-        all_params = []  # noqa: E501
+        all_params = ['include_accounts']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
@@ -323,14 +325,16 @@
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'include_accounts' in local_var_params:
+            query_params.append(('include_accounts', local_var_params['include_accounts']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `pyynab-0.8.8/ynab/api/categories_api.py` & `pyynab-0.9.0/ynab/api/categories_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         Returns all categories grouped by category group.  Amounts (budgeted, activity, balance, etc.) are specific to the current budget month (UTC).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_categories(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -69,16 +69,16 @@
         Returns all categories grouped by category group.  Amounts (budgeted, activity, balance, etc.) are specific to the current budget month (UTC).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_categories_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -155,15 +155,15 @@
         Returns a single category.  Amounts (budgeted, activity, balance, etc.) are specific to the current budget month (UTC).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_category_by_id(budget_id, category_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str category_id: The id of the category (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -181,15 +181,15 @@
         Returns a single category.  Amounts (budgeted, activity, balance, etc.) are specific to the current budget month (UTC).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_category_by_id_with_http_info(budget_id, category_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str category_id: The id of the category (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -271,15 +271,15 @@
         Returns a single category for a specific budget month.  Amounts (budgeted, activity, balance, etc.) are specific to the current budget month (UTC).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_month_category_by_id(budget_id, month, category_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param date month: The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC)) (required)
         :param str category_id: The id of the category (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -298,15 +298,15 @@
         Returns a single category for a specific budget month.  Amounts (budgeted, activity, balance, etc.) are specific to the current budget month (UTC).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_month_category_by_id_with_http_info(budget_id, month, category_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param date month: The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC)) (required)
         :param str category_id: The id of the category (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -388,25 +388,25 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_month_category(self, budget_id, month, category_id, data, **kwargs):  # noqa: E501
         """Update a category for a specific month  # noqa: E501
 
-        Update a category for a specific month  # noqa: E501
+        Update a category for a specific month.  Only `budgeted` amount can be updated.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_month_category(budget_id, month, category_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param date month: The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC)) (required)
         :param str category_id: The id of the category (required)
-        :param SaveMonthCategoryWrapper data: The category to update (required)
+        :param SaveMonthCategoryWrapper data: The category to update.  Only `budgeted` amount can be updated and any other fields specified will be ignored. (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -416,25 +416,25 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.update_month_category_with_http_info(budget_id, month, category_id, data, **kwargs)  # noqa: E501
 
     def update_month_category_with_http_info(self, budget_id, month, category_id, data, **kwargs):  # noqa: E501
         """Update a category for a specific month  # noqa: E501
 
-        Update a category for a specific month  # noqa: E501
+        Update a category for a specific month.  Only `budgeted` amount can be updated.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_month_category_with_http_info(budget_id, month, category_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param date month: The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC)) (required)
         :param str category_id: The id of the category (required)
-        :param SaveMonthCategoryWrapper data: The category to update (required)
+        :param SaveMonthCategoryWrapper data: The category to update.  Only `budgeted` amount can be updated and any other fields specified will be ignored. (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `pyynab-0.8.8/ynab/api/transactions_api.py` & `pyynab-0.9.0/ynab/api/transactions_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,23 +36,23 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def create_transaction(self, budget_id, data, **kwargs):  # noqa: E501
         """Create a single transaction or multiple transactions  # noqa: E501
 
-        Creates a single transaction or multiple transactions.  If you provide a body containing a 'transaction' object, a single transaction will be created and if you provide a body containing a 'transactions' array, multiple transactions will be created.  Scheduled transactions cannot be created on this endpoint.  # noqa: E501
+        Creates a single transaction or multiple transactions.  If you provide a body containing a `transaction` object, a single transaction will be created and if you provide a body containing a `transactions` array, multiple transactions will be created.  Scheduled transactions cannot be created on this endpoint.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_transaction(budget_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param SaveTransactionsWrapper data: The transaction or transactions to create.  To create a single transaction you can specify a value for the 'transaction' object and to create multiple transactions you can specify an array of 'transactions'.  It is expected that you will only provide a value for one of these objects. (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param SaveTransactionsWrapper data: The transaction or transactions to create.  To create a single transaction you can specify a value for the `transaction` object and to create multiple transactions you can specify an array of `transactions`.  It is expected that you will only provide a value for one of these objects. (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -62,23 +62,23 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.create_transaction_with_http_info(budget_id, data, **kwargs)  # noqa: E501
 
     def create_transaction_with_http_info(self, budget_id, data, **kwargs):  # noqa: E501
         """Create a single transaction or multiple transactions  # noqa: E501
 
-        Creates a single transaction or multiple transactions.  If you provide a body containing a 'transaction' object, a single transaction will be created and if you provide a body containing a 'transactions' array, multiple transactions will be created.  Scheduled transactions cannot be created on this endpoint.  # noqa: E501
+        Creates a single transaction or multiple transactions.  If you provide a body containing a `transaction` object, a single transaction will be created and if you provide a body containing a `transactions` array, multiple transactions will be created.  Scheduled transactions cannot be created on this endpoint.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_transaction_with_http_info(budget_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param SaveTransactionsWrapper data: The transaction or transactions to create.  To create a single transaction you can specify a value for the 'transaction' object and to create multiple transactions you can specify an array of 'transactions'.  It is expected that you will only provide a value for one of these objects. (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param SaveTransactionsWrapper data: The transaction or transactions to create.  To create a single transaction you can specify a value for the `transaction` object and to create multiple transactions you can specify an array of `transactions`.  It is expected that you will only provide a value for one of these objects. (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -159,15 +159,15 @@
         Returns a single transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transaction_by_id(budget_id, transaction_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str transaction_id: The id of the transaction (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -185,15 +185,15 @@
         Returns a single transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transaction_by_id_with_http_info(budget_id, transaction_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str transaction_id: The id of the transaction (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -275,18 +275,18 @@
         Returns budget transactions  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transactions(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param date since_date: If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).
-        :param str type: If specified, only transactions of the specified type will be included. 'uncategorized' and 'unapproved' are currently supported.
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str type: If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -303,18 +303,18 @@
         Returns budget transactions  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transactions_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param date since_date: If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).
-        :param str type: If specified, only transactions of the specified type will be included. 'uncategorized' and 'unapproved' are currently supported.
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str type: If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -395,19 +395,19 @@
         Returns all transactions for a specified account  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transactions_by_account(budget_id, account_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str account_id: The id of the account (required)
         :param date since_date: If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).
-        :param str type: If specified, only transactions of the specified type will be included. 'uncategorized' and 'unapproved' are currently supported.
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str type: If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -424,19 +424,19 @@
         Returns all transactions for a specified account  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transactions_by_account_with_http_info(budget_id, account_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str account_id: The id of the account (required)
         :param date since_date: If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).
-        :param str type: If specified, only transactions of the specified type will be included. 'uncategorized' and 'unapproved' are currently supported.
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str type: If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -523,19 +523,19 @@
         Returns all transactions for a specified category  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transactions_by_category(budget_id, category_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str category_id: The id of the category (required)
         :param date since_date: If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).
-        :param str type: If specified, only transactions of the specified type will be included. 'uncategorized' and 'unapproved' are currently supported.
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str type: If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -552,19 +552,19 @@
         Returns all transactions for a specified category  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transactions_by_category_with_http_info(budget_id, category_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str category_id: The id of the category (required)
         :param date since_date: If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).
-        :param str type: If specified, only transactions of the specified type will be included. 'uncategorized' and 'unapproved' are currently supported.
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str type: If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -651,19 +651,19 @@
         Returns all transactions for a specified payee  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transactions_by_payee(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str payee_id: The id of the payee (required)
         :param date since_date: If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).
-        :param str type: If specified, only transactions of the specified type will be included. 'uncategorized' and 'unapproved' are currently supported.
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str type: If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -680,19 +680,19 @@
         Returns all transactions for a specified payee  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_transactions_by_payee_with_http_info(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str payee_id: The id of the payee (required)
         :param date since_date: If specified, only transactions on or after this date will be included.  The date should be ISO formatted (e.g. 2016-12-30).
-        :param str type: If specified, only transactions of the specified type will be included. 'uncategorized' and 'unapproved' are currently supported.
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str type: If specified, only transactions of the specified type will be included. \"uncategorized\" and \"unapproved\" are currently supported.
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -769,25 +769,133 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def import_transactions(self, budget_id, **kwargs):  # noqa: E501
+        """Import transactions  # noqa: E501
+
+        Imports available transactions on all linked accounts for the given budget.  Linked accounts allow transactions to be imported directly from a specified financial institution and this endpoint initiates that import.  Sending a request to this endpoint is the equivalent of clicking \"Import\" on each account in the web application or tapping the \"New Transactions\" banner in the mobile applications.  The response for this endpoint contains the transaction ids that have been imported.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.import_transactions(budget_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: TransactionsImportResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.import_transactions_with_http_info(budget_id, **kwargs)  # noqa: E501
+
+    def import_transactions_with_http_info(self, budget_id, **kwargs):  # noqa: E501
+        """Import transactions  # noqa: E501
+
+        Imports available transactions on all linked accounts for the given budget.  Linked accounts allow transactions to be imported directly from a specified financial institution and this endpoint initiates that import.  Sending a request to this endpoint is the equivalent of clicking \"Import\" on each account in the web application or tapping the \"New Transactions\" banner in the mobile applications.  The response for this endpoint contains the transaction ids that have been imported.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.import_transactions_with_http_info(budget_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(TransactionsImportResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = ['budget_id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method import_transactions" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'budget_id' is set
+        if ('budget_id' not in local_var_params or
+                local_var_params['budget_id'] is None):
+            raise ApiValueError("Missing the required parameter `budget_id` when calling `import_transactions`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'budget_id' in local_var_params:
+            path_params['budget_id'] = local_var_params['budget_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['bearer']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/budgets/{budget_id}/transactions/import', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='TransactionsImportResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def update_transaction(self, budget_id, transaction_id, data, **kwargs):  # noqa: E501
         """Updates an existing transaction  # noqa: E501
 
-        Updates a transaction  # noqa: E501
+        Updates a single transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_transaction(budget_id, transaction_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str transaction_id: The id of the transaction (required)
         :param SaveTransactionWrapper data: The transaction to update (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -799,22 +907,22 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.update_transaction_with_http_info(budget_id, transaction_id, data, **kwargs)  # noqa: E501
 
     def update_transaction_with_http_info(self, budget_id, transaction_id, data, **kwargs):  # noqa: E501
         """Updates an existing transaction  # noqa: E501
 
-        Updates a transaction  # noqa: E501
+        Updates a single transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_transaction_with_http_info(budget_id, transaction_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str transaction_id: The id of the transaction (required)
         :param SaveTransactionWrapper data: The transaction to update (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -896,23 +1004,23 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_transactions(self, budget_id, data, **kwargs):  # noqa: E501
         """Update multiple transactions  # noqa: E501
 
-        Updates multiple transactions, by 'id' or 'import_id'.  # noqa: E501
+        Updates multiple transactions, by `id` or `import_id`.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_transactions(budget_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param SaveTransactionsWrapper data: The transactions to update.  Optionally, transaction 'id' value(s) can be specified as null and an 'import_id' value can be provided which will allow transaction(s) to updated by their import_id. (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param UpdateTransactionsWrapper data: The transactions to update. Each transaction must have either an `id` or `import_id` specified. If `id` is specified as null an `import_id` value can be provided which will allow transaction(s) to be updated by their `import_id`. If an `id` is specified, it will always be used for lookup. (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -922,23 +1030,23 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.update_transactions_with_http_info(budget_id, data, **kwargs)  # noqa: E501
 
     def update_transactions_with_http_info(self, budget_id, data, **kwargs):  # noqa: E501
         """Update multiple transactions  # noqa: E501
 
-        Updates multiple transactions, by 'id' or 'import_id'.  # noqa: E501
+        Updates multiple transactions, by `id` or `import_id`.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_transactions_with_http_info(budget_id, data, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param SaveTransactionsWrapper data: The transactions to update.  Optionally, transaction 'id' value(s) can be specified as null and an 'import_id' value can be provided which will allow transaction(s) to updated by their import_id. (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param UpdateTransactionsWrapper data: The transactions to update. Each transaction must have either an `id` or `import_id` specified. If `id` is specified as null an `import_id` value can be provided which will allow transaction(s) to be updated by their `import_id`. If an `id` is specified, it will always be used for lookup. (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `pyynab-0.8.8/ynab/api/scheduled_transactions_api.py` & `pyynab-0.9.0/ynab/api/scheduled_transactions_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         Returns a single scheduled transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_scheduled_transaction_by_id(budget_id, scheduled_transaction_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str scheduled_transaction_id: The id of the scheduled transaction (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -69,15 +69,15 @@
         Returns a single scheduled transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_scheduled_transaction_by_id_with_http_info(budget_id, scheduled_transaction_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str scheduled_transaction_id: The id of the scheduled transaction (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -159,16 +159,16 @@
         Returns all scheduled transactions  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_scheduled_transactions(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -185,16 +185,16 @@
         Returns all scheduled transactions  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_scheduled_transactions_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `pyynab-0.8.8/ynab/api/deprecated_api.py` & `pyynab-0.9.0/ynab/api/deprecated_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         Creates multiple transactions.  Although this endpoint is still supported, it is recommended to use 'POST /budgets/{budget_id}/transactions' to create multiple transactions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.bulk_create_transactions(budget_id, transactions, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param BulkTransactions transactions: The list of transactions to create (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -69,15 +69,15 @@
         Creates multiple transactions.  Although this endpoint is still supported, it is recommended to use 'POST /budgets/{budget_id}/transactions' to create multiple transactions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.bulk_create_transactions_with_http_info(budget_id, transactions, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param BulkTransactions transactions: The list of transactions to create (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
```

### Comparing `pyynab-0.8.8/ynab/api/months_api.py` & `pyynab-0.9.0/ynab/api/months_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         Returns a single budget month  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budget_month(budget_id, month, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param date month: The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC)) (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -69,15 +69,15 @@
         Returns a single budget month  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budget_month_with_http_info(budget_id, month, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param date month: The budget month in ISO format (e.g. 2016-12-01) (\"current\" can also be used to specify the current calendar month (UTC)) (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -159,16 +159,16 @@
         Returns all budget months  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budget_months(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -185,16 +185,16 @@
         Returns all budget months  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_budget_months_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
-        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since last_knowledge_of_server will be included.
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
+        :param int last_knowledge_of_server: The starting server knowledge.  If provided, only entities that have changed since `last_knowledge_of_server` will be included.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `pyynab-0.8.8/ynab/api/__init__.py` & `pyynab-0.9.0/ynab/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/api/payee_locations_api.py` & `pyynab-0.9.0/ynab/api/payee_locations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         Returns a single payee location  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payee_location_by_id(budget_id, payee_location_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str payee_location_id: id of payee location (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -69,15 +69,15 @@
         Returns a single payee location  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payee_location_by_id_with_http_info(budget_id, payee_location_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str payee_location_id: id of payee location (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -159,15 +159,15 @@
         Returns all payee locations  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payee_locations(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -184,15 +184,15 @@
         Returns all payee locations  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payee_locations_with_http_info(budget_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -260,22 +260,22 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_payee_locations_by_payee(self, budget_id, payee_id, **kwargs):  # noqa: E501
         """List locations for a payee  # noqa: E501
 
-        Returns all payee locations for the specified payee  # noqa: E501
+        Returns all payee locations for a specified payee  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payee_locations_by_payee(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str payee_id: id of payee (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -286,22 +286,22 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.get_payee_locations_by_payee_with_http_info(budget_id, payee_id, **kwargs)  # noqa: E501
 
     def get_payee_locations_by_payee_with_http_info(self, budget_id, payee_id, **kwargs):  # noqa: E501
         """List locations for a payee  # noqa: E501
 
-        Returns all payee locations for the specified payee  # noqa: E501
+        Returns all payee locations for a specified payee  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_payee_locations_by_payee_with_http_info(budget_id, payee_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str budget_id: The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget) (required)
+        :param str budget_id: The id of the budget. \"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget). (required)
         :param str payee_id: id of payee (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
```

### Comparing `pyynab-0.8.8/ynab/rest.py` & `pyynab-0.9.0/ynab/rest.py`

 * *Files identical despite different names*

### Comparing `pyynab-0.8.8/ynab/__init__.py` & `pyynab-0.9.0/ynab/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: rienafairefr@gmail.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.8.8"
+__version__ = "0.9.0"
 
 # import apis into sdk package
 from ynab.api.accounts_api import AccountsApi
 from ynab.api.budgets_api import BudgetsApi
 from ynab.api.categories_api import CategoriesApi
 from ynab.api.deprecated_api import DeprecatedApi
 from ynab.api.months_api import MonthsApi
@@ -37,14 +37,15 @@
 from ynab.exceptions import ApiValueError
 from ynab.exceptions import ApiKeyError
 from ynab.exceptions import ApiException
 # import models into sdk package
 from ynab.models.account import Account
 from ynab.models.account_response import AccountResponse
 from ynab.models.account_response_data import AccountResponseData
+from ynab.models.account_type import AccountType
 from ynab.models.accounts_response import AccountsResponse
 from ynab.models.accounts_response_data import AccountsResponseData
 from ynab.models.budget_detail import BudgetDetail
 from ynab.models.budget_detail_all_of import BudgetDetailAllOf
 from ynab.models.budget_detail_response import BudgetDetailResponse
 from ynab.models.budget_detail_response_data import BudgetDetailResponseData
 from ynab.models.budget_settings import BudgetSettings
@@ -86,18 +87,21 @@
 from ynab.models.payee_location_response_data import PayeeLocationResponseData
 from ynab.models.payee_locations_response import PayeeLocationsResponse
 from ynab.models.payee_locations_response_data import PayeeLocationsResponseData
 from ynab.models.payee_response import PayeeResponse
 from ynab.models.payee_response_data import PayeeResponseData
 from ynab.models.payees_response import PayeesResponse
 from ynab.models.payees_response_data import PayeesResponseData
+from ynab.models.save_account import SaveAccount
+from ynab.models.save_account_wrapper import SaveAccountWrapper
 from ynab.models.save_category_response import SaveCategoryResponse
 from ynab.models.save_category_response_data import SaveCategoryResponseData
 from ynab.models.save_month_category import SaveMonthCategory
 from ynab.models.save_month_category_wrapper import SaveMonthCategoryWrapper
+from ynab.models.save_sub_transaction import SaveSubTransaction
 from ynab.models.save_transaction import SaveTransaction
 from ynab.models.save_transaction_wrapper import SaveTransactionWrapper
 from ynab.models.save_transactions_response import SaveTransactionsResponse
 from ynab.models.save_transactions_response_data import SaveTransactionsResponseData
 from ynab.models.save_transactions_wrapper import SaveTransactionsWrapper
 from ynab.models.scheduled_sub_transaction import ScheduledSubTransaction
 from ynab.models.scheduled_transaction_detail import ScheduledTransactionDetail
@@ -109,13 +113,18 @@
 from ynab.models.scheduled_transactions_response_data import ScheduledTransactionsResponseData
 from ynab.models.sub_transaction import SubTransaction
 from ynab.models.transaction_detail import TransactionDetail
 from ynab.models.transaction_detail_all_of import TransactionDetailAllOf
 from ynab.models.transaction_response import TransactionResponse
 from ynab.models.transaction_response_data import TransactionResponseData
 from ynab.models.transaction_summary import TransactionSummary
+from ynab.models.transactions_import_response import TransactionsImportResponse
+from ynab.models.transactions_import_response_data import TransactionsImportResponseData
 from ynab.models.transactions_response import TransactionsResponse
 from ynab.models.transactions_response_data import TransactionsResponseData
+from ynab.models.update_transaction import UpdateTransaction
+from ynab.models.update_transaction_all_of import UpdateTransactionAllOf
+from ynab.models.update_transactions_wrapper import UpdateTransactionsWrapper
 from ynab.models.user import User
 from ynab.models.user_response import UserResponse
 from ynab.models.user_response_data import UserResponseData
```

### Comparing `pyynab-0.8.8/pyynab.egg-info/SOURCES.txt` & `pyynab-0.9.0/pyynab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 pyynab.egg-info/dependency_links.txt
 pyynab.egg-info/requires.txt
 pyynab.egg-info/top_level.txt
 test/__init__.py
 test/test_account.py
 test/test_account_response.py
 test/test_account_response_data.py
+test/test_account_type.py
 test/test_accounts_api.py
 test/test_accounts_response.py
 test/test_accounts_response_data.py
 test/test_budget_detail.py
 test/test_budget_detail_all_of.py
 test/test_budget_detail_response.py
 test/test_budget_detail_response_data.py
@@ -61,18 +62,21 @@
 test/test_payee_locations_response.py
 test/test_payee_locations_response_data.py
 test/test_payee_response.py
 test/test_payee_response_data.py
 test/test_payees_api.py
 test/test_payees_response.py
 test/test_payees_response_data.py
+test/test_save_account.py
+test/test_save_account_wrapper.py
 test/test_save_category_response.py
 test/test_save_category_response_data.py
 test/test_save_month_category.py
 test/test_save_month_category_wrapper.py
+test/test_save_sub_transaction.py
 test/test_save_transaction.py
 test/test_save_transaction_wrapper.py
 test/test_save_transactions_response.py
 test/test_save_transactions_response_data.py
 test/test_save_transactions_wrapper.py
 test/test_scheduled_sub_transaction.py
 test/test_scheduled_transaction_detail.py
@@ -86,16 +90,21 @@
 test/test_sub_transaction.py
 test/test_transaction_detail.py
 test/test_transaction_detail_all_of.py
 test/test_transaction_response.py
 test/test_transaction_response_data.py
 test/test_transaction_summary.py
 test/test_transactions_api.py
+test/test_transactions_import_response.py
+test/test_transactions_import_response_data.py
 test/test_transactions_response.py
 test/test_transactions_response_data.py
+test/test_update_transaction.py
+test/test_update_transaction_all_of.py
+test/test_update_transactions_wrapper.py
 test/test_user.py
 test/test_user_api.py
 test/test_user_response.py
 test/test_user_response_data.py
 ynab/__init__.py
 ynab/api_client.py
 ynab/configuration.py
@@ -112,14 +121,15 @@
 ynab/api/scheduled_transactions_api.py
 ynab/api/transactions_api.py
 ynab/api/user_api.py
 ynab/models/__init__.py
 ynab/models/account.py
 ynab/models/account_response.py
 ynab/models/account_response_data.py
+ynab/models/account_type.py
 ynab/models/accounts_response.py
 ynab/models/accounts_response_data.py
 ynab/models/budget_detail.py
 ynab/models/budget_detail_all_of.py
 ynab/models/budget_detail_response.py
 ynab/models/budget_detail_response_data.py
 ynab/models/budget_settings.py
@@ -161,18 +171,21 @@
 ynab/models/payee_location_response_data.py
 ynab/models/payee_locations_response.py
 ynab/models/payee_locations_response_data.py
 ynab/models/payee_response.py
 ynab/models/payee_response_data.py
 ynab/models/payees_response.py
 ynab/models/payees_response_data.py
+ynab/models/save_account.py
+ynab/models/save_account_wrapper.py
 ynab/models/save_category_response.py
 ynab/models/save_category_response_data.py
 ynab/models/save_month_category.py
 ynab/models/save_month_category_wrapper.py
+ynab/models/save_sub_transaction.py
 ynab/models/save_transaction.py
 ynab/models/save_transaction_wrapper.py
 ynab/models/save_transactions_response.py
 ynab/models/save_transactions_response_data.py
 ynab/models/save_transactions_wrapper.py
 ynab/models/scheduled_sub_transaction.py
 ynab/models/scheduled_transaction_detail.py
@@ -184,12 +197,17 @@
 ynab/models/scheduled_transactions_response_data.py
 ynab/models/sub_transaction.py
 ynab/models/transaction_detail.py
 ynab/models/transaction_detail_all_of.py
 ynab/models/transaction_response.py
 ynab/models/transaction_response_data.py
 ynab/models/transaction_summary.py
+ynab/models/transactions_import_response.py
+ynab/models/transactions_import_response_data.py
 ynab/models/transactions_response.py
 ynab/models/transactions_response_data.py
+ynab/models/update_transaction.py
+ynab/models/update_transaction_all_of.py
+ynab/models/update_transactions_wrapper.py
 ynab/models/user.py
 ynab/models/user_response.py
 ynab/models/user_response_data.py
```

### Comparing `pyynab-0.8.8/README.md` & `pyynab-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyynab
 Our API uses a REST based design, leverages the JSON data format, and relies upon HTTPS for transport. We respond with meaningful HTTP response codes and if an error occurs, we include error details in the response body.  API Documentation is at https://api.youneedabudget.com
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 0.8.8
+- Package version: 0.9.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -58,31 +58,32 @@
 # configuration.api_key_prefix['Authorization'] = 'Bearer'
 
 # Defining host is optional and default to https://api.youneedabudget.com/v1
 configuration.host = "https://api.youneedabudget.com/v1"
 # Create an instance of the API class
 api_instance = ynab.AccountsApi(ynab.ApiClient(configuration))
 budget_id = 'budget_id_example' # str | The id of the budget (\"last-used\" can be used to specify the last used budget and \"default\" can be used if default budget selection is enabled (see: https://api.youneedabudget.com/#oauth-default-budget)
-account_id = 'account_id_example' # str | The id of the account
+data = ynab.SaveAccountWrapper() # SaveAccountWrapper | The account to create.
 
 try:
-    # Single account
-    api_response = api_instance.get_account_by_id(budget_id, account_id)
+    # Create a new account
+    api_response = api_instance.create_account(budget_id, data)
     pprint(api_response)
 except ApiException as e:
-    print("Exception when calling AccountsApi->get_account_by_id: %s\n" % e)
+    print("Exception when calling AccountsApi->create_account: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.youneedabudget.com/v1*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*AccountsApi* | [**create_account**](docs/AccountsApi.md#create_account) | **POST** /budgets/{budget_id}/accounts | Create a new account
 *AccountsApi* | [**get_account_by_id**](docs/AccountsApi.md#get_account_by_id) | **GET** /budgets/{budget_id}/accounts/{account_id} | Single account
 *AccountsApi* | [**get_accounts**](docs/AccountsApi.md#get_accounts) | **GET** /budgets/{budget_id}/accounts | Account list
 *BudgetsApi* | [**get_budget_by_id**](docs/BudgetsApi.md#get_budget_by_id) | **GET** /budgets/{budget_id} | Single budget
 *BudgetsApi* | [**get_budget_settings_by_id**](docs/BudgetsApi.md#get_budget_settings_by_id) | **GET** /budgets/{budget_id}/settings | Budget Settings
 *BudgetsApi* | [**get_budgets**](docs/BudgetsApi.md#get_budgets) | **GET** /budgets | List budgets
 *CategoriesApi* | [**get_categories**](docs/CategoriesApi.md#get_categories) | **GET** /budgets/{budget_id}/categories | List categories
 *CategoriesApi* | [**get_category_by_id**](docs/CategoriesApi.md#get_category_by_id) | **GET** /budgets/{budget_id}/categories/{category_id} | Single category
@@ -100,24 +101,26 @@
 *ScheduledTransactionsApi* | [**get_scheduled_transactions**](docs/ScheduledTransactionsApi.md#get_scheduled_transactions) | **GET** /budgets/{budget_id}/scheduled_transactions | List scheduled transactions
 *TransactionsApi* | [**create_transaction**](docs/TransactionsApi.md#create_transaction) | **POST** /budgets/{budget_id}/transactions | Create a single transaction or multiple transactions
 *TransactionsApi* | [**get_transaction_by_id**](docs/TransactionsApi.md#get_transaction_by_id) | **GET** /budgets/{budget_id}/transactions/{transaction_id} | Single transaction
 *TransactionsApi* | [**get_transactions**](docs/TransactionsApi.md#get_transactions) | **GET** /budgets/{budget_id}/transactions | List transactions
 *TransactionsApi* | [**get_transactions_by_account**](docs/TransactionsApi.md#get_transactions_by_account) | **GET** /budgets/{budget_id}/accounts/{account_id}/transactions | List account transactions
 *TransactionsApi* | [**get_transactions_by_category**](docs/TransactionsApi.md#get_transactions_by_category) | **GET** /budgets/{budget_id}/categories/{category_id}/transactions | List category transactions
 *TransactionsApi* | [**get_transactions_by_payee**](docs/TransactionsApi.md#get_transactions_by_payee) | **GET** /budgets/{budget_id}/payees/{payee_id}/transactions | List payee transactions
+*TransactionsApi* | [**import_transactions**](docs/TransactionsApi.md#import_transactions) | **POST** /budgets/{budget_id}/transactions/import | Import transactions
 *TransactionsApi* | [**update_transaction**](docs/TransactionsApi.md#update_transaction) | **PUT** /budgets/{budget_id}/transactions/{transaction_id} | Updates an existing transaction
 *TransactionsApi* | [**update_transactions**](docs/TransactionsApi.md#update_transactions) | **PATCH** /budgets/{budget_id}/transactions | Update multiple transactions
 *UserApi* | [**get_user**](docs/UserApi.md#get_user) | **GET** /user | User info
 
 
 ## Documentation For Models
 
  - [Account](docs/Account.md)
  - [AccountResponse](docs/AccountResponse.md)
  - [AccountResponseData](docs/AccountResponseData.md)
+ - [AccountType](docs/AccountType.md)
  - [AccountsResponse](docs/AccountsResponse.md)
  - [AccountsResponseData](docs/AccountsResponseData.md)
  - [BudgetDetail](docs/BudgetDetail.md)
  - [BudgetDetailAllOf](docs/BudgetDetailAllOf.md)
  - [BudgetDetailResponse](docs/BudgetDetailResponse.md)
  - [BudgetDetailResponseData](docs/BudgetDetailResponseData.md)
  - [BudgetSettings](docs/BudgetSettings.md)
@@ -159,18 +162,21 @@
  - [PayeeLocationResponseData](docs/PayeeLocationResponseData.md)
  - [PayeeLocationsResponse](docs/PayeeLocationsResponse.md)
  - [PayeeLocationsResponseData](docs/PayeeLocationsResponseData.md)
  - [PayeeResponse](docs/PayeeResponse.md)
  - [PayeeResponseData](docs/PayeeResponseData.md)
  - [PayeesResponse](docs/PayeesResponse.md)
  - [PayeesResponseData](docs/PayeesResponseData.md)
+ - [SaveAccount](docs/SaveAccount.md)
+ - [SaveAccountWrapper](docs/SaveAccountWrapper.md)
  - [SaveCategoryResponse](docs/SaveCategoryResponse.md)
  - [SaveCategoryResponseData](docs/SaveCategoryResponseData.md)
  - [SaveMonthCategory](docs/SaveMonthCategory.md)
  - [SaveMonthCategoryWrapper](docs/SaveMonthCategoryWrapper.md)
+ - [SaveSubTransaction](docs/SaveSubTransaction.md)
  - [SaveTransaction](docs/SaveTransaction.md)
  - [SaveTransactionWrapper](docs/SaveTransactionWrapper.md)
  - [SaveTransactionsResponse](docs/SaveTransactionsResponse.md)
  - [SaveTransactionsResponseData](docs/SaveTransactionsResponseData.md)
  - [SaveTransactionsWrapper](docs/SaveTransactionsWrapper.md)
  - [ScheduledSubTransaction](docs/ScheduledSubTransaction.md)
  - [ScheduledTransactionDetail](docs/ScheduledTransactionDetail.md)
@@ -182,16 +188,21 @@
  - [ScheduledTransactionsResponseData](docs/ScheduledTransactionsResponseData.md)
  - [SubTransaction](docs/SubTransaction.md)
  - [TransactionDetail](docs/TransactionDetail.md)
  - [TransactionDetailAllOf](docs/TransactionDetailAllOf.md)
  - [TransactionResponse](docs/TransactionResponse.md)
  - [TransactionResponseData](docs/TransactionResponseData.md)
  - [TransactionSummary](docs/TransactionSummary.md)
+ - [TransactionsImportResponse](docs/TransactionsImportResponse.md)
+ - [TransactionsImportResponseData](docs/TransactionsImportResponseData.md)
  - [TransactionsResponse](docs/TransactionsResponse.md)
  - [TransactionsResponseData](docs/TransactionsResponseData.md)
+ - [UpdateTransaction](docs/UpdateTransaction.md)
+ - [UpdateTransactionAllOf](docs/UpdateTransactionAllOf.md)
+ - [UpdateTransactionsWrapper](docs/UpdateTransactionsWrapper.md)
  - [User](docs/User.md)
  - [UserResponse](docs/UserResponse.md)
  - [UserResponseData](docs/UserResponseData.md)
 
 
 ## Documentation For Authorization
```

