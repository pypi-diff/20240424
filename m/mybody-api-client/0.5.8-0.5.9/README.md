# Comparing `tmp/mybody_api_client-0.5.8.tar.gz` & `tmp/mybody_api_client-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybody_api_client-0.5.8.tar", last modified: Wed Mar  6 17:11:46 2024, max compression
+gzip compressed data, was "mybody_api_client-0.5.9.tar", last modified: Thu Mar  7 13:31:30 2024, max compression
```

## Comparing `mybody_api_client-0.5.8.tar` & `mybody_api_client-0.5.9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.765173 mybody_api_client-0.5.8/
--rw-rw-rw-   0        0        0    11556 2023-12-15 11:35:24.000000 mybody_api_client-0.5.8/LICENSE
--rw-rw-rw-   0        0        0     1155 2024-03-06 17:11:46.765173 mybody_api_client-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      669 2024-01-31 13:13:35.000000 mybody_api_client-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.676124 mybody_api_client-0.5.8/mybody_api_client/
--rw-rw-rw-   0        0        0      703 2024-02-02 20:15:19.000000 mybody_api_client-0.5.8/mybody_api_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.683126 mybody_api_client-0.5.8/mybody_api_client/routes/
--rw-rw-rw-   0        0        0      861 2024-02-02 20:15:19.000000 mybody_api_client-0.5.8/mybody_api_client/routes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.684123 mybody_api_client-0.5.8/mybody_api_client/routes/admin/
--rw-rw-rw-   0        0        0     1979 2024-03-05 10:34:02.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.686123 mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/
--rw-rw-rw-   0        0        0     1871 2024-02-15 20:23:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.687124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/roles/
--rw-rw-rw-   0        0        0     1923 2024-02-15 20:23:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/roles/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.687124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/services/
--rw-rw-rw-   0        0        0     2669 2024-02-06 17:20:23.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.688123 mybody_api_client-0.5.8/mybody_api_client/routes/admin/articles/
--rw-rw-rw-   0        0        0     2167 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/articles/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.689124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/articles/translations/
--rw-rw-rw-   0        0        0     1552 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/articles/translations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.690125 mybody_api_client-0.5.8/mybody_api_client/routes/admin/countries/
--rw-rw-rw-   0        0        0     2228 2024-03-05 10:34:02.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/countries/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.691124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/currencies/
--rw-rw-rw-   0        0        0     1358 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/currencies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.692125 mybody_api_client-0.5.8/mybody_api_client/routes/admin/exercises/
--rw-rw-rw-   0        0        0     1584 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/exercises/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.694124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/images/
--rw-rw-rw-   0        0        0     1478 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/images/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.695127 mybody_api_client-0.5.8/mybody_api_client/routes/admin/languages/
--rw-rw-rw-   0        0        0     1331 2024-03-05 15:23:22.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/languages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.696125 mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/
--rw-rw-rw-   0        0        0     3441 2024-02-15 20:23:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.697125 mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/products/
--rw-rw-rw-   0        0        0     2354 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/products/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.698125 mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/reports/
--rw-rw-rw-   0        0        0     1897 2024-02-15 20:23:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.699126 mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/reports/products/
--rw-rw-rw-   0        0        0     1786 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/reports/products/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.700125 mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/
--rw-rw-rw-   0        0        0     2838 2024-03-06 11:18:16.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.701124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/methods/
--rw-rw-rw-   0        0        0     1561 2024-03-05 10:34:02.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.702125 mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/methods/currencies/
--rw-rw-rw-   0        0        0     1450 2024-03-05 10:34:02.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/methods/currencies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.703125 mybody_api_client-0.5.8/mybody_api_client/routes/admin/permissions/
--rw-rw-rw-   0        0        0     1792 2024-02-15 20:23:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/permissions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.704124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/products/
--rw-rw-rw-   0        0        0     2502 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/products/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.706124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/roles/
--rw-rw-rw-   0        0        0     1793 2024-03-05 10:34:02.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/roles/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.707124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/roles/permissions/
--rw-rw-rw-   0        0        0     1898 2024-03-05 10:34:02.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/roles/permissions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.708123 mybody_api_client-0.5.8/mybody_api_client/routes/admin/services/
--rw-rw-rw-   0        0        0     1978 2024-03-06 11:18:16.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.709122 mybody_api_client-0.5.8/mybody_api_client/routes/admin/services/costs/
--rw-rw-rw-   0        0        0     1790 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/services/costs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.711133 mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/
--rw-rw-rw-   0        0        0     2745 2024-03-02 09:49:11.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.713124 mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/packs/
--rw-rw-rw-   0        0        0     1432 2024-03-05 15:34:34.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/packs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.714123 mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/translations/
--rw-rw-rw-   0        0        0     2266 2024-03-02 09:49:11.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/translations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.716123 mybody_api_client-0.5.8/mybody_api_client/routes/admin/timezones/
--rw-rw-rw-   0        0        0     1427 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/timezones/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.717132 mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/
--rw-rw-rw-   0        0        0     3196 2024-02-29 09:15:49.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.719123 mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/exercises/
--rw-rw-rw-   0        0        0     2703 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/exercises/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.720123 mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/reports/
--rw-rw-rw-   0        0        0     1806 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.721124 mybody_api_client-0.5.8/mybody_api_client/routes/client/
--rw-rw-rw-   0        0        0     1908 2024-03-06 17:11:37.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.722123 mybody_api_client-0.5.8/mybody_api_client/routes/client/accounts/
--rw-rw-rw-   0        0        0     2908 2024-02-15 20:23:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/accounts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.723124 mybody_api_client-0.5.8/mybody_api_client/routes/client/accounts/services/
--rw-rw-rw-   0        0        0     1571 2024-02-05 12:27:20.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/accounts/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.724122 mybody_api_client-0.5.8/mybody_api_client/routes/client/articles/
--rw-rw-rw-   0        0        0     1562 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/articles/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.725125 mybody_api_client-0.5.8/mybody_api_client/routes/client/countries/
--rw-rw-rw-   0        0        0     1305 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/countries/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.726124 mybody_api_client-0.5.8/mybody_api_client/routes/client/currencies/
--rw-rw-rw-   0        0        0     1311 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/currencies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.727124 mybody_api_client-0.5.8/mybody_api_client/routes/client/exercises/
--rw-rw-rw-   0        0        0     1299 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/exercises/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.728125 mybody_api_client-0.5.8/mybody_api_client/routes/client/images/
--rw-rw-rw-   0        0        0     1508 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/images/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.729126 mybody_api_client-0.5.8/mybody_api_client/routes/client/languages/
--rw-rw-rw-   0        0        0     1343 2024-02-06 17:49:58.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/languages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.730125 mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/
--rw-rw-rw-   0        0        0     1683 2024-02-06 17:20:23.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.731124 mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/products/
--rw-rw-rw-   0        0        0     1330 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/products/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.732168 mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/reports/
--rw-rw-rw-   0        0        0     1719 2024-02-15 20:23:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.733125 mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/
--rw-rw-rw-   0        0        0     2193 2024-03-06 11:18:16.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.734124 mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/methods/
--rw-rw-rw-   0        0        0     1524 2024-03-06 11:18:16.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.735125 mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/methods/currencies/
--rw-rw-rw-   0        0        0     1019 2024-03-05 10:34:02.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/methods/currencies/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.735125 mybody_api_client-0.5.8/mybody_api_client/routes/client/products/
--rw-rw-rw-   0        0        0     1386 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/products/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.737122 mybody_api_client-0.5.8/mybody_api_client/routes/client/services/
--rw-rw-rw-   0        0        0     1426 2024-03-06 11:18:16.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.737122 mybody_api_client-0.5.8/mybody_api_client/routes/client/services/costs/
--rw-rw-rw-   0        0        0     1099 2024-03-06 17:11:37.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/services/costs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.738123 mybody_api_client-0.5.8/mybody_api_client/routes/client/sessions/
--rw-rw-rw-   0        0        0     1147 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/sessions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.739124 mybody_api_client-0.5.8/mybody_api_client/routes/client/texts/
--rw-rw-rw-   0        0        0      872 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/texts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.740124 mybody_api_client-0.5.8/mybody_api_client/routes/client/texts/packs/
--rw-rw-rw-   0        0        0     1086 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/texts/packs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.741124 mybody_api_client-0.5.8/mybody_api_client/routes/client/timezones/
--rw-rw-rw-   0        0        0     1307 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/timezones/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.742124 mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/
--rw-rw-rw-   0        0        0     2036 2024-02-29 09:15:49.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.744124 mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/exercises/
--rw-rw-rw-   0        0        0     1428 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/exercises/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.745124 mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/reports/
--rw-rw-rw-   0        0        0     1807 2024-02-05 10:44:54.000000 mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.753172 mybody_api_client-0.5.8/mybody_api_client/utils/
--rw-rw-rw-   0        0        0      769 2024-02-02 21:03:59.000000 mybody_api_client-0.5.8/mybody_api_client/utils/__init__.py
--rw-rw-rw-   0        0        0      908 2024-02-02 19:53:17.000000 mybody_api_client-0.5.8/mybody_api_client/utils/base_api_client.py
--rw-rw-rw-   0        0        0     3951 2024-03-06 11:18:16.000000 mybody_api_client-0.5.8/mybody_api_client/utils/base_route.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.764172 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/
--rw-rw-rw-   0        0        0     1269 2024-03-04 11:45:22.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1873 2024-03-05 10:36:59.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/account.py
--rw-rw-rw-   0        0        0      799 2024-01-18 15:55:31.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/article.py
--rw-rw-rw-   0        0        0      946 2024-01-17 20:51:08.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/base.py
--rw-rw-rw-   0        0        0      801 2024-01-18 15:55:31.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/exercise.py
--rw-rw-rw-   0        0        0      926 2024-01-18 15:55:31.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/image.py
--rw-rw-rw-   0        0        0     1313 2024-02-27 08:34:53.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/main.py
--rw-rw-rw-   0        0        0      793 2024-01-18 15:55:31.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/meal.py
--rw-rw-rw-   0        0        0      929 2024-03-04 11:45:22.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/payment.py
--rw-rw-rw-   0        0        0     1002 2024-01-18 15:55:31.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/product.py
--rw-rw-rw-   0        0        0      790 2024-02-27 08:34:53.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/service.py
--rw-rw-rw-   0        0        0     1155 2024-02-02 21:24:07.000000 mybody_api_client-0.5.8/mybody_api_client/utils/exceptions_manager.py
-drwxrwxrwx   0        0        0        0 2024-03-06 17:11:46.682169 mybody_api_client-0.5.8/mybody_api_client.egg-info/
--rw-rw-rw-   0        0        0     1155 2024-03-06 17:11:46.000000 mybody_api_client-0.5.8/mybody_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4128 2024-03-06 17:11:46.000000 mybody_api_client-0.5.8/mybody_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 17:11:46.000000 mybody_api_client-0.5.8/mybody_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-15 11:35:57.000000 mybody_api_client-0.5.8/mybody_api_client.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2024-03-06 17:11:46.000000 mybody_api_client-0.5.8/mybody_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-03-06 17:11:46.000000 mybody_api_client-0.5.8/mybody_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-06 17:11:46.766173 mybody_api_client-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1675 2024-03-06 17:11:37.000000 mybody_api_client-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.641981 mybody_api_client-0.5.9/
+-rw-rw-rw-   0        0        0    11556 2023-12-15 11:35:24.000000 mybody_api_client-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0     1155 2024-03-07 13:31:30.642980 mybody_api_client-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2024-01-31 13:13:35.000000 mybody_api_client-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.556214 mybody_api_client-0.5.9/mybody_api_client/
+-rw-rw-rw-   0        0        0      703 2024-02-02 20:15:19.000000 mybody_api_client-0.5.9/mybody_api_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.564150 mybody_api_client-0.5.9/mybody_api_client/routes/
+-rw-rw-rw-   0        0        0      861 2024-02-02 20:15:19.000000 mybody_api_client-0.5.9/mybody_api_client/routes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.566151 mybody_api_client-0.5.9/mybody_api_client/routes/admin/
+-rw-rw-rw-   0        0        0     1979 2024-03-05 10:34:02.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.567151 mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/
+-rw-rw-rw-   0        0        0     1871 2024-02-15 20:23:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.569151 mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/roles/
+-rw-rw-rw-   0        0        0     1923 2024-02-15 20:23:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/roles/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.570151 mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/services/
+-rw-rw-rw-   0        0        0     2669 2024-02-06 17:20:23.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.571150 mybody_api_client-0.5.9/mybody_api_client/routes/admin/articles/
+-rw-rw-rw-   0        0        0     2167 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/articles/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.572149 mybody_api_client-0.5.9/mybody_api_client/routes/admin/articles/translations/
+-rw-rw-rw-   0        0        0     1552 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/articles/translations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.573150 mybody_api_client-0.5.9/mybody_api_client/routes/admin/countries/
+-rw-rw-rw-   0        0        0     2228 2024-03-05 10:34:02.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/countries/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.574151 mybody_api_client-0.5.9/mybody_api_client/routes/admin/currencies/
+-rw-rw-rw-   0        0        0     1358 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/currencies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.574983 mybody_api_client-0.5.9/mybody_api_client/routes/admin/exercises/
+-rw-rw-rw-   0        0        0     1584 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/exercises/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.576042 mybody_api_client-0.5.9/mybody_api_client/routes/admin/images/
+-rw-rw-rw-   0        0        0     1478 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/images/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.576983 mybody_api_client-0.5.9/mybody_api_client/routes/admin/languages/
+-rw-rw-rw-   0        0        0     1331 2024-03-05 15:23:22.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/languages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.577981 mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/
+-rw-rw-rw-   0        0        0     3441 2024-02-15 20:23:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.578980 mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/products/
+-rw-rw-rw-   0        0        0     2354 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/products/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.580980 mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/reports/
+-rw-rw-rw-   0        0        0     1897 2024-02-15 20:23:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.581982 mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/reports/products/
+-rw-rw-rw-   0        0        0     1786 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/reports/products/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.582981 mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/
+-rw-rw-rw-   0        0        0     2838 2024-03-06 11:18:16.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.582981 mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/methods/
+-rw-rw-rw-   0        0        0     1561 2024-03-05 10:34:02.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.583981 mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/methods/currencies/
+-rw-rw-rw-   0        0        0     1450 2024-03-05 10:34:02.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/methods/currencies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.585987 mybody_api_client-0.5.9/mybody_api_client/routes/admin/permissions/
+-rw-rw-rw-   0        0        0     1792 2024-02-15 20:23:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/permissions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.587983 mybody_api_client-0.5.9/mybody_api_client/routes/admin/products/
+-rw-rw-rw-   0        0        0     2502 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/products/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.588982 mybody_api_client-0.5.9/mybody_api_client/routes/admin/roles/
+-rw-rw-rw-   0        0        0     1793 2024-03-05 10:34:02.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/roles/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.589980 mybody_api_client-0.5.9/mybody_api_client/routes/admin/roles/permissions/
+-rw-rw-rw-   0        0        0     1898 2024-03-05 10:34:02.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/roles/permissions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.590980 mybody_api_client-0.5.9/mybody_api_client/routes/admin/services/
+-rw-rw-rw-   0        0        0     1978 2024-03-06 11:18:16.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.591980 mybody_api_client-0.5.9/mybody_api_client/routes/admin/services/costs/
+-rw-rw-rw-   0        0        0     1790 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/services/costs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.592980 mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/
+-rw-rw-rw-   0        0        0     2745 2024-03-02 09:49:11.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.593981 mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/packs/
+-rw-rw-rw-   0        0        0     1432 2024-03-05 15:34:34.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/packs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.594981 mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/translations/
+-rw-rw-rw-   0        0        0     2266 2024-03-02 09:49:11.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/translations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.596028 mybody_api_client-0.5.9/mybody_api_client/routes/admin/timezones/
+-rw-rw-rw-   0        0        0     1427 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/timezones/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.596981 mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/
+-rw-rw-rw-   0        0        0     3196 2024-02-29 09:15:49.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.597979 mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/exercises/
+-rw-rw-rw-   0        0        0     2703 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/exercises/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.598980 mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/reports/
+-rw-rw-rw-   0        0        0     1806 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.599980 mybody_api_client-0.5.9/mybody_api_client/routes/client/
+-rw-rw-rw-   0        0        0     1908 2024-03-06 17:11:37.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.600982 mybody_api_client-0.5.9/mybody_api_client/routes/client/accounts/
+-rw-rw-rw-   0        0        0     2908 2024-02-15 20:23:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/accounts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.601980 mybody_api_client-0.5.9/mybody_api_client/routes/client/accounts/services/
+-rw-rw-rw-   0        0        0     1571 2024-02-05 12:27:20.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/accounts/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.602980 mybody_api_client-0.5.9/mybody_api_client/routes/client/articles/
+-rw-rw-rw-   0        0        0     1562 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/articles/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.603981 mybody_api_client-0.5.9/mybody_api_client/routes/client/countries/
+-rw-rw-rw-   0        0        0     1305 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/countries/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.604983 mybody_api_client-0.5.9/mybody_api_client/routes/client/currencies/
+-rw-rw-rw-   0        0        0     1311 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/currencies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.607982 mybody_api_client-0.5.9/mybody_api_client/routes/client/exercises/
+-rw-rw-rw-   0        0        0     1299 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/exercises/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.608983 mybody_api_client-0.5.9/mybody_api_client/routes/client/images/
+-rw-rw-rw-   0        0        0     1508 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/images/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.609981 mybody_api_client-0.5.9/mybody_api_client/routes/client/languages/
+-rw-rw-rw-   0        0        0     1343 2024-02-06 17:49:58.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/languages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.610981 mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/
+-rw-rw-rw-   0        0        0     1683 2024-02-06 17:20:23.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.611981 mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/products/
+-rw-rw-rw-   0        0        0     1330 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/products/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.612981 mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/reports/
+-rw-rw-rw-   0        0        0     1719 2024-02-15 20:23:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.613982 mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/
+-rw-rw-rw-   0        0        0     2193 2024-03-06 11:18:16.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.614981 mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/methods/
+-rw-rw-rw-   0        0        0     1524 2024-03-06 11:18:16.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.616042 mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/methods/currencies/
+-rw-rw-rw-   0        0        0     1019 2024-03-05 10:34:02.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/methods/currencies/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.616981 mybody_api_client-0.5.9/mybody_api_client/routes/client/products/
+-rw-rw-rw-   0        0        0     1386 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/products/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.617980 mybody_api_client-0.5.9/mybody_api_client/routes/client/services/
+-rw-rw-rw-   0        0        0     1426 2024-03-06 11:18:16.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.618980 mybody_api_client-0.5.9/mybody_api_client/routes/client/services/costs/
+-rw-rw-rw-   0        0        0     1099 2024-03-06 17:11:37.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/services/costs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.619982 mybody_api_client-0.5.9/mybody_api_client/routes/client/sessions/
+-rw-rw-rw-   0        0        0     1147 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/sessions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.620983 mybody_api_client-0.5.9/mybody_api_client/routes/client/texts/
+-rw-rw-rw-   0        0        0      872 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/texts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.621981 mybody_api_client-0.5.9/mybody_api_client/routes/client/texts/packs/
+-rw-rw-rw-   0        0        0     1086 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/texts/packs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.622981 mybody_api_client-0.5.9/mybody_api_client/routes/client/timezones/
+-rw-rw-rw-   0        0        0     1307 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/timezones/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.623981 mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/
+-rw-rw-rw-   0        0        0     2036 2024-02-29 09:15:49.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.624981 mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/exercises/
+-rw-rw-rw-   0        0        0     1428 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/exercises/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.626985 mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/reports/
+-rw-rw-rw-   0        0        0     1807 2024-02-05 10:44:54.000000 mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.631981 mybody_api_client-0.5.9/mybody_api_client/utils/
+-rw-rw-rw-   0        0        0      769 2024-02-02 21:03:59.000000 mybody_api_client-0.5.9/mybody_api_client/utils/__init__.py
+-rw-rw-rw-   0        0        0      908 2024-02-02 19:53:17.000000 mybody_api_client-0.5.9/mybody_api_client/utils/base_api_client.py
+-rw-rw-rw-   0        0        0     4034 2024-03-06 18:53:41.000000 mybody_api_client-0.5.9/mybody_api_client/utils/base_route.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.641981 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/
+-rw-rw-rw-   0        0        0     1269 2024-03-04 11:45:22.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-03-05 10:36:59.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/account.py
+-rw-rw-rw-   0        0        0      799 2024-01-18 15:55:31.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/article.py
+-rw-rw-rw-   0        0        0      946 2024-01-17 20:51:08.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/base.py
+-rw-rw-rw-   0        0        0      801 2024-01-18 15:55:31.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/exercise.py
+-rw-rw-rw-   0        0        0      926 2024-01-18 15:55:31.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/image.py
+-rw-rw-rw-   0        0        0     1313 2024-02-27 08:34:53.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/main.py
+-rw-rw-rw-   0        0        0      793 2024-01-18 15:55:31.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/meal.py
+-rw-rw-rw-   0        0        0      929 2024-03-04 11:45:22.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/payment.py
+-rw-rw-rw-   0        0        0     1002 2024-01-18 15:55:31.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/product.py
+-rw-rw-rw-   0        0        0      790 2024-02-27 08:34:53.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/service.py
+-rw-rw-rw-   0        0        0     1155 2024-02-02 21:24:07.000000 mybody_api_client-0.5.9/mybody_api_client/utils/exceptions_manager.py
+drwxrwxrwx   0        0        0        0 2024-03-07 13:31:30.563151 mybody_api_client-0.5.9/mybody_api_client.egg-info/
+-rw-rw-rw-   0        0        0     1155 2024-03-07 13:31:30.000000 mybody_api_client-0.5.9/mybody_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4128 2024-03-07 13:31:30.000000 mybody_api_client-0.5.9/mybody_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-07 13:31:30.000000 mybody_api_client-0.5.9/mybody_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-12-15 11:35:57.000000 mybody_api_client-0.5.9/mybody_api_client.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2024-03-07 13:31:30.000000 mybody_api_client-0.5.9/mybody_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-03-07 13:31:30.000000 mybody_api_client-0.5.9/mybody_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-07 13:31:30.642980 mybody_api_client-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1675 2024-03-07 13:29:56.000000 mybody_api_client-0.5.9/setup.py
```

### Comparing `mybody_api_client-0.5.8/LICENSE` & `mybody_api_client-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/PKG-INFO` & `mybody_api_client-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybody_api_client
-Version: 0.5.8
+Version: 0.5.9
 Home-page: https://yegoryakubovich.com
 Author: Yegor Yakubovich
 Author-email: personal@yegoryakubovich.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `mybody_api_client-0.5.8/README.md` & `mybody_api_client-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/roles/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/accounts/services/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/accounts/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/articles/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/articles/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/articles/translations/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/articles/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/countries/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/countries/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/currencies/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/exercises/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/exercises/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/images/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/images/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/languages/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/products/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/products/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/reports/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/meals/reports/products/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/meals/reports/products/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/methods/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/payments/methods/currencies/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/payments/methods/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/permissions/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/products/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/products/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/roles/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/roles/permissions/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/roles/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/services/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/services/costs/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/services/costs/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/packs/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/packs/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/texts/translations/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/texts/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/timezones/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/timezones/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/exercises/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/exercises/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/admin/trainings/reports/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/admin/trainings/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/accounts/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/accounts/services/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/accounts/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/articles/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/articles/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/countries/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/countries/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/currencies/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/exercises/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/exercises/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/images/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/images/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/languages/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/products/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/products/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/meals/reports/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/meals/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/methods/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/payments/methods/currencies/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/payments/methods/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/products/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/products/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/services/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/services/costs/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/services/costs/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/sessions/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/texts/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/texts/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/texts/packs/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/texts/packs/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/timezones/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/timezones/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/exercises/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/exercises/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/routes/client/trainings/reports/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/routes/client/trainings/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/base_api_client.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/base_api_client.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/base_route.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/base_route.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 #
 
 
 from io import BufferedReader
 
 from addict import Dict
-from aiohttp import ClientSession, ContentTypeError
+from aiohttp import ClientSession, ContentTypeError, FormData
 from furl import furl
 
 from mybody_api_client.utils.exceptions import ApiException
 from mybody_api_client.utils.exceptions_manager import exceptions
 
 
 class RequestTypes:
@@ -52,23 +52,23 @@
         return f.url
 
     async def create_data(self, parameters, token_required, type_):
         parameters = parameters or {}
 
         json = {}
         url_parameters = {}
-        data = {}
+        data = FormData()
         if token_required and self.token:
             url_parameters['token'] = self.token
 
         have_data = False
         for pk, pv in parameters.items():
             if isinstance(pv, BufferedReader) or isinstance(pv, bytes):
                 have_data = True
-                data[pk] = pv
+                data.add_field(name=pk, value=pv, filename='1.jpg', content_type='image/jpeg')
                 continue
 
             url_parameters[pk] = pv
 
         if type_ == RequestTypes.POST and not have_data:
             json = url_parameters
             url_parameters = {}
```

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/__init__.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/account.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/account.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/article.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/article.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/base.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/exercise.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/exercise.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/image.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/image.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/main.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/meal.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/meal.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/payment.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/payment.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/product.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/product.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions/service.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client/utils/exceptions_manager.py` & `mybody_api_client-0.5.9/mybody_api_client/utils/exceptions_manager.py`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/mybody_api_client.egg-info/PKG-INFO` & `mybody_api_client-0.5.9/mybody_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mybody-api-client
-Version: 0.5.8
+Version: 0.5.9
 Home-page: https://yegoryakubovich.com
 Author: Yegor Yakubovich
 Author-email: personal@yegoryakubovich.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `mybody_api_client-0.5.8/mybody_api_client.egg-info/SOURCES.txt` & `mybody_api_client-0.5.9/mybody_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mybody_api_client-0.5.8/setup.py` & `mybody_api_client-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from os import path
 
 from setuptools import setup, PEP420PackageFinder
 
 
 NAME = 'mybody_api_client'
-VERSION = '0.5.8'
+VERSION = '0.5.9'
 DESCRIPTION = ''
 URL = 'https://yegoryakubovich.com'
 PACKAGE_ROOT = path.abspath(path.dirname(__file__))
 README = open('README.md', 'r').read()
 
 packages = [
     package
```

