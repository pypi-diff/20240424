# Comparing `tmp/mns-scheduler-1.0.3.2.tar.gz` & `tmp/mns-scheduler-1.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.3.2.tar", last modified: Mon Apr 22 10:12:43 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.3.3.tar", last modified: Wed Apr 24 09:38:12 2024, max compression
```

## Comparing `mns-scheduler-1.0.3.2.tar` & `mns-scheduler-1.0.3.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.625495 mns-scheduler-1.0.3.2/
--rw-rw-rw-   0        0        0       62 2024-04-22 10:12:43.625495 mns-scheduler-1.0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.591585 mns-scheduler-1.0.3.2/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.593580 mns-scheduler-1.0.3.2/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.3.2/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.595575 mns-scheduler-1.0.3.2/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20332 2024-04-18 14:12:36.000000 mns-scheduler-1.0.3.2/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.596572 mns-scheduler-1.0.3.2/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.596572 mns-scheduler-1.0.3.2/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.599564 mns-scheduler-1.0.3.2/mns_scheduler/concept/em/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/em/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.599564 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.600561 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/app/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.602556 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     1662 2024-04-15 02:52:26.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.603553 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/symbol/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8757 2024-04-16 06:53:57.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.605548 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/web/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/web/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.606545 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/wen_cai/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.607543 mns-scheduler-1.0.3.2/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.3.2/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.608539 mns-scheduler-1.0.3.2/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.609537 mns-scheduler-1.0.3.2/mns_scheduler/ipo/
--rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.3.2/mns_scheduler/ipo/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.3.2/mns_scheduler/ipo/auto_ipo_buy_api.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.609537 mns-scheduler-1.0.3.2/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.611531 mns-scheduler-1.0.3.2/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.3.2/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-18 13:32:07.000000 mns-scheduler-1.0.3.2/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.612529 mns-scheduler-1.0.3.2/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.3.2/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.612529 mns-scheduler-1.0.3.2/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.613527 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.614524 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4501 2024-04-22 10:12:35.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.615521 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.616519 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-20 14:08:05.000000 mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.618513 mns-scheduler-1.0.3.2/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.3.2/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.619511 mns-scheduler-1.0.3.2/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.3.2/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.622502 mns-scheduler-1.0.3.2/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.3.2/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.3.2/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.3.2/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.2/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-16 13:51:28.000000 mns-scheduler-1.0.3.2/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.623499 mns-scheduler-1.0.3.2/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.2/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    14367 2024-04-21 03:52:33.000000 mns-scheduler-1.0.3.2/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.3.2/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:12:43.624497 mns-scheduler-1.0.3.2/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-04-22 10:12:43.000000 mns-scheduler-1.0.3.2/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3078 2024-04-22 10:12:43.000000 mns-scheduler-1.0.3.2/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 10:12:43.000000 mns-scheduler-1.0.3.2/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-22 10:12:43.000000 mns-scheduler-1.0.3.2/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 10:12:43.625495 mns-scheduler-1.0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-22 10:12:35.000000 mns-scheduler-1.0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.721346 mns-scheduler-1.0.3.3/
+-rw-rw-rw-   0        0        0       62 2024-04-24 09:38:12.720348 mns-scheduler-1.0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.689432 mns-scheduler-1.0.3.3/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.691426 mns-scheduler-1.0.3.3/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.3.3/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.693421 mns-scheduler-1.0.3.3/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20332 2024-04-18 14:12:36.000000 mns-scheduler-1.0.3.3/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.693421 mns-scheduler-1.0.3.3/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.694418 mns-scheduler-1.0.3.3/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.696412 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.697409 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.697409 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/app/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.699404 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     1662 2024-04-15 02:52:26.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.700401 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8757 2024-04-16 06:53:57.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.702396 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.703394 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/wen_cai/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.704391 mns-scheduler-1.0.3.3/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.3.3/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.705388 mns-scheduler-1.0.3.3/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.706386 mns-scheduler-1.0.3.3/mns_scheduler/ipo/
+-rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.3.3/mns_scheduler/ipo/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.3.3/mns_scheduler/ipo/auto_ipo_buy_api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.706386 mns-scheduler-1.0.3.3/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.708381 mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-18 13:32:07.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.708381 mns-scheduler-1.0.3.3/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.3.3/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.709378 mns-scheduler-1.0.3.3/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.709378 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.711372 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4765 2024-04-24 09:37:02.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.711372 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.712370 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-20 14:08:05.000000 mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.714365 mns-scheduler-1.0.3.3/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.3.3/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.715362 mns-scheduler-1.0.3.3/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.3.3/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.718354 mns-scheduler-1.0.3.3/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-16 13:51:28.000000 mns-scheduler-1.0.3.3/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.719351 mns-scheduler-1.0.3.3/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.3.3/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    14500 2024-04-24 08:54:42.000000 mns-scheduler-1.0.3.3/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.3.3/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:38:12.720348 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-24 09:38:12.000000 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3078 2024-04-24 09:38:12.000000 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:38:12.000000 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-24 09:38:12.000000 mns-scheduler-1.0.3.3/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:38:12.721346 mns-scheduler-1.0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-24 09:38:10.000000 mns-scheduler-1.0.3.3/setup.py
```

### Comparing `mns-scheduler-1.0.3.2/README.md` & `mns-scheduler-1.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.3.3/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.3.3/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.3.3/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.3.3/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.3.3/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.3.3/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.3.3/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.3.3/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,22 +47,27 @@
     kpl_best_choose_index_number = all_kpl_best_choose_index_df.shape[0]
     page_max_number = kpl_best_choose_index_number / kpl_common_api.HIS_PAGE_MAX_COUNT
     page_number = 0
     number = 1
     for end_time in KPL_MINUTE_LIST:
         while page_number <= page_max_number:
             index = page_number * kpl_common_api.HIS_PAGE_MAX_COUNT
-            kpl_plate_best_index_df = kpl_common_api.get_plate_index_his(index, kpl_common_api.BEST_CHOOSE,
+            kpl_plate_best_index_df = kpl_common_api.get_plate_index_his(index, int(kpl_common_api.BEST_CHOOSE),
                                                                          str_day, KPL_MINUTE_BEGIN,
                                                                          end_time)
 
             if data_frame_util.is_empty(kpl_plate_best_index_df):
                 continue
             kpl_plate_best_index_df['number'] = number
             kpl_plate_best_index_df['str_day'] = str_day
+            hour = end_time[0:2]
+            minute = end_time[2:4]
+            kpl_plate_best_index_df['str_day'] = str_day
+
+            kpl_plate_best_index_df['str_now_date'] = str_day + " " + hour + ":" + minute + ":00"
             kpl_plate_best_index_df = kpl_plate_best_index_df[[
                 "plate_code",
                 "plate_name",
                 "heat_score",
                 "chg",
                 "speed",
                 "amount",
@@ -74,15 +79,15 @@
                 "super_order_net",
                 "total_mv",
                 "last_reason_organ_add",
                 "ava_pe_now",
                 "ava_pe_next",
                 "number",
                 "str_day",
-
+                "str_now_date"
             ]]
             save_kpl_his_index(kpl_plate_best_index_df, str_day, end_time)
             if end_time == KPL_MINUTE_END:
                 save_kpl_his_daily(kpl_plate_best_index_df, str_day, end_time)
             page_number = page_number + 1
         # 执行下一个时间段
         page_number = 0
@@ -96,15 +101,15 @@
 
 def save_kpl_his_daily(kpl_plate_best_index_df, str_day, end_time):
     kpl_plate_best_index_df['_id'] = str_day + '-' + end_time + '-' + kpl_plate_best_index_df['plate_code']
     mongodb_util.save_mongo(kpl_plate_best_index_df, db_name_constant.KPL_BEST_CHOOSE_DAILY)
 
 
 def sync_all_days():
-    query = {"_id": {"$gte": '2022-07-22'}, 'trade_date': {"$lte": "2022-11-21"}}
+    query = {"_id": {"$gte": '2022-07-19'}, 'trade_date': {"$lte": "2024-04-23"}}
     trade_date_list = mongodb_util.find_query_data('trade_date_list', query)
     trade_date_list = trade_date_list.sort_values(by=['trade_date'], ascending=False)
     for trade_one in trade_date_list.itertuples():
         sync_best_choose_his_index(trade_one.trade_date)
 
 
 if __name__ == '__main__':
```

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.3.3/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.3.3/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.3.3/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.3.3/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.3.3/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.3.3/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.3.3/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,17 @@
 
 # 同步开盘啦当日精选指数行情数据
 
 def sync_kpl_best_his_quotes():
     now_date = datetime.now()
     str_day = now_date.strftime('%Y-%m-%d')
     if trade_date_common_service_api.is_trade_day(str_day):
-        sync_best_choose_his_index.sync_best_choose_his_index(str_day)
+        last_trade_day = trade_date_common_service_api.get_last_trade_day(str_day)
+        # 当天不能获取历史数据
+        sync_best_choose_his_index.sync_best_choose_his_index(last_trade_day)
         logger.info('同步开盘啦当日精选指数行情数据任务完成')
 
 
 # # 定义BlockingScheduler
 blockingScheduler = BlockingScheduler()
 # sync_trade_date 同步交易日期
 blockingScheduler.add_job(sync_trade_date, 'cron', hour='20', minute='43')
@@ -344,14 +346,14 @@
 # 自动打新 打新中签高时间段 10:30-11:30
 blockingScheduler.add_job(auto_ipo_buy, 'cron', hour='10', minute='40,50')
 
 # 更新开盘啦指数关系
 blockingScheduler.add_job(update_best_choose_plate_relation, 'cron', hour='09,18', minute='25')
 
 # 更新开盘啦指数关系
-blockingScheduler.add_job(sync_kpl_best_his_quotes, 'cron', hour='18,22', minute='25')
+blockingScheduler.add_job(sync_kpl_best_his_quotes, 'cron', hour='16,22', minute='48')
 
 print('定时任务启动成功')
 blockingScheduler.start()
 
 # if __name__ == '__main__':
 #     sync_daily_data_info()
```

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.3.3/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.3.2/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.3.3/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

