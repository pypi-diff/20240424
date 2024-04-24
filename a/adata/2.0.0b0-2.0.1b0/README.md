# Comparing `tmp/adata-2.0.0b0.tar.gz` & `tmp/adata-2.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-2.0.0b0.tar", last modified: Wed Apr 17 10:30:56 2024, max compression
+gzip compressed data, was "adata-2.0.1b0.tar", last modified: Wed Apr 17 10:56:33 2024, max compression
```

## Comparing `adata-2.0.0b0.tar` & `adata-2.0.1b0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.418604 adata-2.0.0b0/
--rw-rw-rw-   0        0        0    11558 2023-04-07 05:48:39.000000 adata-2.0.0b0/LICENSE
--rw-rw-rw-   0        0        0      126 2023-10-23 06:31:33.000000 adata-2.0.0b0/MANIFEST.in
--rw-rw-rw-   0        0        0    21039 2024-04-17 10:30:56.418604 adata-2.0.0b0/PKG-INFO
--rw-rw-rw-   0        0        0    20328 2024-04-17 10:27:23.000000 adata-2.0.0b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.306074 adata-2.0.0b0/adata/
--rw-rw-rw-   0        0        0     1189 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/__init__.py
--rw-rw-rw-   0        0        0      737 2024-04-17 10:30:41.000000 adata-2.0.0b0/adata/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.312075 adata-2.0.0b0/adata/bond/
--rw-rw-rw-   0        0        0      261 2023-06-05 11:07:12.000000 adata-2.0.0b0/adata/bond/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.313076 adata-2.0.0b0/adata/bond/cache/
--rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.0.0b0/adata/bond/cache/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.315076 adata-2.0.0b0/adata/bond/info/
--rw-rw-rw-   0        0        0      261 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/bond/info/__init__.py
--rw-rw-rw-   0        0        0     2200 2023-05-31 08:21:01.000000 adata-2.0.0b0/adata/bond/info/bond_code.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.317076 adata-2.0.0b0/adata/bond/market/
--rw-rw-rw-   0        0        0      104 2023-05-31 08:12:06.000000 adata-2.0.0b0/adata/bond/market/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/bond/market/bond_market.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.318076 adata-2.0.0b0/adata/common/
--rw-rw-rw-   0        0        0      150 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.321077 adata-2.0.0b0/adata/common/base/
--rw-rw-rw-   0        0        0      133 2023-06-05 03:44:57.000000 adata-2.0.0b0/adata/common/base/__init__.py
--rw-rw-rw-   0        0        0      195 2023-08-14 05:47:34.000000 adata-2.0.0b0/adata/common/base/base_req.py
--rw-rw-rw-   0        0        0     3015 2023-08-18 09:30:57.000000 adata-2.0.0b0/adata/common/base/base_ths.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.325078 adata-2.0.0b0/adata/common/exception/
--rw-rw-rw-   0        0        0       97 2023-07-10 08:15:13.000000 adata-2.0.0b0/adata/common/exception/__init__.py
--rw-rw-rw-   0        0        0      379 2023-08-01 09:58:42.000000 adata-2.0.0b0/adata/common/exception/exception_msg.py
--rw-rw-rw-   0        0        0      350 2023-08-14 06:04:13.000000 adata-2.0.0b0/adata/common/exception/handler.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.330081 adata-2.0.0b0/adata/common/headers/
--rw-rw-rw-   0        0        0     6407 2023-07-10 08:15:13.000000 adata-2.0.0b0/adata/common/headers/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/common/headers/baidu_headers.py
--rw-rw-rw-   0        0        0      571 2023-08-14 05:47:34.000000 adata-2.0.0b0/adata/common/headers/east_headers.py
--rw-rw-rw-   0        0        0      602 2023-04-18 11:18:06.000000 adata-2.0.0b0/adata/common/headers/sina_headers.py
--rw-rw-rw-   0        0        0     3085 2023-08-08 04:51:00.000000 adata-2.0.0b0/adata/common/headers/ths_headers.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.333081 adata-2.0.0b0/adata/common/js/
--rw-rw-rw-   0        0        0       99 2023-05-05 10:05:38.000000 adata-2.0.0b0/adata/common/js/__init__.py
--rw-rw-rw-   0        0        0    15792 2023-08-01 09:31:40.000000 adata-2.0.0b0/adata/common/js/hexin.js
--rw-rw-rw-   0        0        0    39849 2023-06-28 03:35:45.000000 adata-2.0.0b0/adata/common/js/ths.js
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.339080 adata-2.0.0b0/adata/common/utils/
--rw-rw-rw-   0        0        0      190 2023-07-10 08:15:13.000000 adata-2.0.0b0/adata/common/utils/__init__.py
--rw-rw-rw-   0        0        0      501 2023-12-04 11:20:28.000000 adata-2.0.0b0/adata/common/utils/code_utils.py
--rw-rw-rw-   0        0        0      877 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/common/utils/cookie.py
--rw-rw-rw-   0        0        0     3046 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/common/utils/snowflake.py
--rw-rw-rw-   0        0        0     2891 2023-08-07 03:04:02.000000 adata-2.0.0b0/adata/common/utils/sunrequests.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.340595 adata-2.0.0b0/adata/fund/
--rw-rw-rw-   0        0        0      327 2024-04-17 10:25:02.000000 adata-2.0.0b0/adata/fund/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.341586 adata-2.0.0b0/adata/fund/cache/
--rw-rw-rw-   0        0        0      103 2023-06-02 06:05:35.000000 adata-2.0.0b0/adata/fund/cache/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.343586 adata-2.0.0b0/adata/fund/info/
--rw-rw-rw-   0        0        0      260 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/fund/info/__init__.py
--rw-rw-rw-   0        0        0     5247 2023-08-01 10:31:22.000000 adata-2.0.0b0/adata/fund/info/fund_info.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.348587 adata-2.0.0b0/adata/fund/market/
--rw-rw-rw-   0        0        0      379 2024-04-17 10:25:02.000000 adata-2.0.0b0/adata/fund/market/__init__.py
--rw-rw-rw-   0        0        0     2170 2024-04-17 10:25:02.000000 adata-2.0.0b0/adata/fund/market/etf_market.py
--rw-rw-rw-   0        0        0      657 2024-04-17 10:07:40.000000 adata-2.0.0b0/adata/fund/market/etf_market_template.py
--rw-rw-rw-   0        0        0     7993 2024-04-17 10:07:40.000000 adata-2.0.0b0/adata/fund/market/etf_market_ths.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.349587 adata-2.0.0b0/adata/message/
--rw-rw-rw-   0        0        0      103 2023-04-07 05:48:39.000000 adata-2.0.0b0/adata/message/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.355589 adata-2.0.0b0/adata/sentiment/
--rw-rw-rw-   0        0        0      466 2023-08-01 04:36:50.000000 adata-2.0.0b0/adata/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.356589 adata-2.0.0b0/adata/sentiment/cache/
--rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.0.0b0/adata/sentiment/cache/__init__.py
--rw-rw-rw-   0        0        0     9633 2023-08-01 04:08:30.000000 adata-2.0.0b0/adata/sentiment/north_flow.py
--rw-rw-rw-   0        0        0     3741 2023-08-18 09:30:57.000000 adata-2.0.0b0/adata/sentiment/securities_margin.py
--rw-rw-rw-   0        0        0     4271 2023-08-08 04:51:00.000000 adata-2.0.0b0/adata/sentiment/stock_lifting.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.357589 adata-2.0.0b0/adata/stock/
--rw-rw-rw-   0        0        0      420 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/stock/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.361590 adata-2.0.0b0/adata/stock/cache/
--rw-rw-rw-   0        0        0      267 2023-10-18 11:49:59.000000 adata-2.0.0b0/adata/stock/cache/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.386597 adata-2.0.0b0/adata/stock/cache/calendar/
--rw-rw-rw-   0        0        0       34 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2004.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2005.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2006.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2007.csv
--rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2008.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2009.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2010.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2011.csv
--rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2012.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2013.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2014.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2015.csv
--rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2016.csv
--rw-rw-rw-   0        0        0     5858 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2017.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2018.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2019.csv
--rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2020.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2021.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2022.csv
--rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/cache/calendar/2023.csv
--rw-rw-rw-   0        0        0     5888 2023-12-29 03:33:12.000000 adata-2.0.0b0/adata/stock/cache/calendar/2024.csv
--rw-rw-rw-   0        0        0      428 2023-12-11 07:21:42.000000 adata-2.0.0b0/adata/stock/cache/calendar/__init__.py
--rw-rw-rw-   0        0        0   174847 2023-10-18 12:45:02.000000 adata-2.0.0b0/adata/stock/cache/code.csv
--rw-rw-rw-   0        0        0     8752 2023-06-02 06:45:42.000000 adata-2.0.0b0/adata/stock/cache/index_code_rel_ths.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.389598 adata-2.0.0b0/adata/stock/index/
--rw-rw-rw-   0        0        0      267 2023-06-02 03:44:46.000000 adata-2.0.0b0/adata/stock/index/__init__.py
--rw-rw-rw-   0        0        0      207 2023-06-02 03:44:46.000000 adata-2.0.0b0/adata/stock/index/cal_index.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.392597 adata-2.0.0b0/adata/stock/info/
--rw-rw-rw-   0        0        0      501 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/stock/info/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.398599 adata-2.0.0b0/adata/stock/info/concept/
--rw-rw-rw-   0        0        0       86 2023-08-07 03:04:02.000000 adata-2.0.0b0/adata/stock/info/concept/__init__.py
--rw-rw-rw-   0        0        0      485 2023-08-07 03:04:02.000000 adata-2.0.0b0/adata/stock/info/concept/stock_concept.py
--rw-rw-rw-   0        0        0     5595 2024-02-26 03:31:53.000000 adata-2.0.0b0/adata/stock/info/concept/stock_concept_east.py
--rw-rw-rw-   0        0        0      463 2023-12-04 11:54:33.000000 adata-2.0.0b0/adata/stock/info/concept/stock_concept_template.py
--rw-rw-rw-   0        0        0    15126 2023-12-29 03:33:12.000000 adata-2.0.0b0/adata/stock/info/concept/stock_concept_ths.py
--rw-rw-rw-   0        0        0     5770 2023-10-18 12:46:30.000000 adata-2.0.0b0/adata/stock/info/stock_code.py
--rw-rw-rw-   0        0        0    10715 2023-10-18 04:49:44.000000 adata-2.0.0b0/adata/stock/info/stock_index.py
--rw-rw-rw-   0        0        0     2321 2023-08-08 04:46:57.000000 adata-2.0.0b0/adata/stock/info/trade_calendar.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.400600 adata-2.0.0b0/adata/stock/market/
--rw-rw-rw-   0        0        0      550 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/stock/market/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.403600 adata-2.0.0b0/adata/stock/market/concepth_market/
--rw-rw-rw-   0        0        0      385 2023-08-07 03:32:53.000000 adata-2.0.0b0/adata/stock/market/concepth_market/__init__.py
--rw-rw-rw-   0        0        0     7028 2023-08-08 11:22:09.000000 adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_east.py
--rw-rw-rw-   0        0        0      695 2023-08-08 11:05:55.000000 adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_template.py
--rw-rw-rw-   0        0        0     9587 2023-08-08 10:57:42.000000 adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_ths.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.409601 adata-2.0.0b0/adata/stock/market/index_market/
--rw-rw-rw-   0        0        0       97 2023-08-07 03:04:02.000000 adata-2.0.0b0/adata/stock/market/index_market/__init__.py
--rw-rw-rw-   0        0        0     2218 2023-12-29 03:56:23.000000 adata-2.0.0b0/adata/stock/market/index_market/market_index.py
--rw-rw-rw-   0        0        0     6865 2023-12-29 03:55:54.000000 adata-2.0.0b0/adata/stock/market/index_market/market_index_east.py
--rw-rw-rw-   0        0        0     1746 2023-08-08 11:47:56.000000 adata-2.0.0b0/adata/stock/market/index_market/market_index_template.py
--rw-rw-rw-   0        0        0     8246 2023-08-08 11:48:17.000000 adata-2.0.0b0/adata/stock/market/index_market/market_index_ths.py
--rw-rw-rw-   0        0        0     3199 2023-10-18 04:50:22.000000 adata-2.0.0b0/adata/stock/market/stock_dividend.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.416602 adata-2.0.0b0/adata/stock/market/stock_market/
--rw-rw-rw-   0        0        0      176 2023-10-10 02:59:10.000000 adata-2.0.0b0/adata/stock/market/stock_market/__init__.py
--rw-rw-rw-   0        0        0     3519 2024-04-17 10:25:01.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market.py
--rw-rw-rw-   0        0        0    11398 2023-12-04 12:31:36.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market_baidu.py
--rw-rw-rw-   0        0        0     5415 2023-09-18 06:30:43.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market_qq.py
--rw-rw-rw-   0        0        0     2666 2023-07-07 08:19:03.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market_sina.py
--rw-rw-rw-   0        0        0     2658 2023-09-13 12:58:10.000000 adata-2.0.0b0/adata/stock/market/stock_market/stock_market_template.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:30:56.311075 adata-2.0.0b0/adata.egg-info/
--rw-rw-rw-   0        0        0    21039 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3649 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 10:30:56.000000 adata-2.0.0b0/adata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 10:30:56.418604 adata-2.0.0b0/setup.cfg
--rw-rw-rw-   0        0        0     1838 2023-12-04 12:31:36.000000 adata-2.0.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.239185 adata-2.0.1b0/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 05:48:39.000000 adata-2.0.1b0/LICENSE
+-rw-rw-rw-   0        0        0      126 2023-10-23 06:31:33.000000 adata-2.0.1b0/MANIFEST.in
+-rw-rw-rw-   0        0        0    21039 2024-04-17 10:56:33.239185 adata-2.0.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0    20328 2024-04-17 10:27:23.000000 adata-2.0.1b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.129518 adata-2.0.1b0/adata/
+-rw-rw-rw-   0        0        0     1189 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/__init__.py
+-rw-rw-rw-   0        0        0      737 2024-04-17 10:56:21.000000 adata-2.0.1b0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.135520 adata-2.0.1b0/adata/bond/
+-rw-rw-rw-   0        0        0      261 2023-06-05 11:07:12.000000 adata-2.0.1b0/adata/bond/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.137521 adata-2.0.1b0/adata/bond/cache/
+-rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.0.1b0/adata/bond/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.139521 adata-2.0.1b0/adata/bond/info/
+-rw-rw-rw-   0        0        0      261 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/bond/info/__init__.py
+-rw-rw-rw-   0        0        0     2200 2023-05-31 08:21:01.000000 adata-2.0.1b0/adata/bond/info/bond_code.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.141522 adata-2.0.1b0/adata/bond/market/
+-rw-rw-rw-   0        0        0      104 2023-05-31 08:12:06.000000 adata-2.0.1b0/adata/bond/market/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/bond/market/bond_market.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.142522 adata-2.0.1b0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.145523 adata-2.0.1b0/adata/common/base/
+-rw-rw-rw-   0        0        0      133 2023-06-05 03:44:57.000000 adata-2.0.1b0/adata/common/base/__init__.py
+-rw-rw-rw-   0        0        0      195 2023-08-14 05:47:34.000000 adata-2.0.1b0/adata/common/base/base_req.py
+-rw-rw-rw-   0        0        0     3015 2023-08-18 09:30:57.000000 adata-2.0.1b0/adata/common/base/base_ths.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.148523 adata-2.0.1b0/adata/common/exception/
+-rw-rw-rw-   0        0        0       97 2023-07-10 08:15:13.000000 adata-2.0.1b0/adata/common/exception/__init__.py
+-rw-rw-rw-   0        0        0      379 2023-08-01 09:58:42.000000 adata-2.0.1b0/adata/common/exception/exception_msg.py
+-rw-rw-rw-   0        0        0      350 2023-08-14 06:04:13.000000 adata-2.0.1b0/adata/common/exception/handler.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.154524 adata-2.0.1b0/adata/common/headers/
+-rw-rw-rw-   0        0        0     6407 2023-07-10 08:15:13.000000 adata-2.0.1b0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      571 2023-08-14 05:47:34.000000 adata-2.0.1b0/adata/common/headers/east_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 11:18:06.000000 adata-2.0.1b0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     3085 2023-08-08 04:51:00.000000 adata-2.0.1b0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.158525 adata-2.0.1b0/adata/common/js/
+-rw-rw-rw-   0        0        0       99 2023-05-05 10:05:38.000000 adata-2.0.1b0/adata/common/js/__init__.py
+-rw-rw-rw-   0        0        0    15792 2023-08-01 09:31:40.000000 adata-2.0.1b0/adata/common/js/hexin.js
+-rw-rw-rw-   0        0        0    39849 2023-06-28 03:35:45.000000 adata-2.0.1b0/adata/common/js/ths.js
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.163526 adata-2.0.1b0/adata/common/utils/
+-rw-rw-rw-   0        0        0      190 2023-07-10 08:15:13.000000 adata-2.0.1b0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-12-04 11:20:28.000000 adata-2.0.1b0/adata/common/utils/code_utils.py
+-rw-rw-rw-   0        0        0      877 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/common/utils/cookie.py
+-rw-rw-rw-   0        0        0     3046 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0     2891 2023-08-07 03:04:02.000000 adata-2.0.1b0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.164527 adata-2.0.1b0/adata/fund/
+-rw-rw-rw-   0        0        0      327 2024-04-17 10:25:02.000000 adata-2.0.1b0/adata/fund/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.165527 adata-2.0.1b0/adata/fund/cache/
+-rw-rw-rw-   0        0        0      103 2023-06-02 06:05:35.000000 adata-2.0.1b0/adata/fund/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.167527 adata-2.0.1b0/adata/fund/info/
+-rw-rw-rw-   0        0        0      260 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/fund/info/__init__.py
+-rw-rw-rw-   0        0        0     5247 2023-08-01 10:31:22.000000 adata-2.0.1b0/adata/fund/info/fund_info.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.171529 adata-2.0.1b0/adata/fund/market/
+-rw-rw-rw-   0        0        0      379 2024-04-17 10:25:02.000000 adata-2.0.1b0/adata/fund/market/__init__.py
+-rw-rw-rw-   0        0        0     2416 2024-04-17 10:44:44.000000 adata-2.0.1b0/adata/fund/market/etf_market.py
+-rw-rw-rw-   0        0        0      654 2024-04-17 10:45:50.000000 adata-2.0.1b0/adata/fund/market/etf_market_template.py
+-rw-rw-rw-   0        0        0     7990 2024-04-17 10:45:50.000000 adata-2.0.1b0/adata/fund/market/etf_market_ths.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.172528 adata-2.0.1b0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-07 05:48:39.000000 adata-2.0.1b0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.176529 adata-2.0.1b0/adata/sentiment/
+-rw-rw-rw-   0        0        0      466 2023-08-01 04:36:50.000000 adata-2.0.1b0/adata/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.177530 adata-2.0.1b0/adata/sentiment/cache/
+-rw-rw-rw-   0        0        0      103 2023-08-18 09:30:57.000000 adata-2.0.1b0/adata/sentiment/cache/__init__.py
+-rw-rw-rw-   0        0        0     9633 2023-08-01 04:08:30.000000 adata-2.0.1b0/adata/sentiment/north_flow.py
+-rw-rw-rw-   0        0        0     3741 2023-08-18 09:30:57.000000 adata-2.0.1b0/adata/sentiment/securities_margin.py
+-rw-rw-rw-   0        0        0     4271 2023-08-08 04:51:00.000000 adata-2.0.1b0/adata/sentiment/stock_lifting.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.178530 adata-2.0.1b0/adata/stock/
+-rw-rw-rw-   0        0        0      420 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.181530 adata-2.0.1b0/adata/stock/cache/
+-rw-rw-rw-   0        0        0      267 2023-10-18 11:49:59.000000 adata-2.0.1b0/adata/stock/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.207178 adata-2.0.1b0/adata/stock/cache/calendar/
+-rw-rw-rw-   0        0        0       34 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2004.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2005.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2006.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2007.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2008.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2009.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2010.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2011.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2012.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2013.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2014.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2015.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2016.csv
+-rw-rw-rw-   0        0        0     5858 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2017.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2018.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2019.csv
+-rw-rw-rw-   0        0        0     5890 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2020.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2021.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2022.csv
+-rw-rw-rw-   0        0        0     5874 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/cache/calendar/2023.csv
+-rw-rw-rw-   0        0        0     5888 2023-12-29 03:33:12.000000 adata-2.0.1b0/adata/stock/cache/calendar/2024.csv
+-rw-rw-rw-   0        0        0      428 2023-12-11 07:21:42.000000 adata-2.0.1b0/adata/stock/cache/calendar/__init__.py
+-rw-rw-rw-   0        0        0   174847 2023-10-18 12:45:02.000000 adata-2.0.1b0/adata/stock/cache/code.csv
+-rw-rw-rw-   0        0        0     8752 2023-06-02 06:45:42.000000 adata-2.0.1b0/adata/stock/cache/index_code_rel_ths.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.210179 adata-2.0.1b0/adata/stock/index/
+-rw-rw-rw-   0        0        0      267 2023-06-02 03:44:46.000000 adata-2.0.1b0/adata/stock/index/__init__.py
+-rw-rw-rw-   0        0        0      207 2023-06-02 03:44:46.000000 adata-2.0.1b0/adata/stock/index/cal_index.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.214180 adata-2.0.1b0/adata/stock/info/
+-rw-rw-rw-   0        0        0      501 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/stock/info/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.220181 adata-2.0.1b0/adata/stock/info/concept/
+-rw-rw-rw-   0        0        0       86 2023-08-07 03:04:02.000000 adata-2.0.1b0/adata/stock/info/concept/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-08-07 03:04:02.000000 adata-2.0.1b0/adata/stock/info/concept/stock_concept.py
+-rw-rw-rw-   0        0        0     5595 2024-02-26 03:31:53.000000 adata-2.0.1b0/adata/stock/info/concept/stock_concept_east.py
+-rw-rw-rw-   0        0        0      463 2023-12-04 11:54:33.000000 adata-2.0.1b0/adata/stock/info/concept/stock_concept_template.py
+-rw-rw-rw-   0        0        0    15126 2023-12-29 03:33:12.000000 adata-2.0.1b0/adata/stock/info/concept/stock_concept_ths.py
+-rw-rw-rw-   0        0        0     5770 2023-10-18 12:46:30.000000 adata-2.0.1b0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0    10715 2023-10-18 04:49:44.000000 adata-2.0.1b0/adata/stock/info/stock_index.py
+-rw-rw-rw-   0        0        0     2321 2023-08-08 04:46:57.000000 adata-2.0.1b0/adata/stock/info/trade_calendar.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.222181 adata-2.0.1b0/adata/stock/market/
+-rw-rw-rw-   0        0        0      550 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/stock/market/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.226183 adata-2.0.1b0/adata/stock/market/concepth_market/
+-rw-rw-rw-   0        0        0      385 2023-08-07 03:32:53.000000 adata-2.0.1b0/adata/stock/market/concepth_market/__init__.py
+-rw-rw-rw-   0        0        0     7028 2023-08-08 11:22:09.000000 adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_east.py
+-rw-rw-rw-   0        0        0      695 2023-08-08 11:05:55.000000 adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_template.py
+-rw-rw-rw-   0        0        0     9587 2023-08-08 10:57:42.000000 adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_ths.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.230183 adata-2.0.1b0/adata/stock/market/index_market/
+-rw-rw-rw-   0        0        0       97 2023-08-07 03:04:02.000000 adata-2.0.1b0/adata/stock/market/index_market/__init__.py
+-rw-rw-rw-   0        0        0     2218 2023-12-29 03:56:23.000000 adata-2.0.1b0/adata/stock/market/index_market/market_index.py
+-rw-rw-rw-   0        0        0     6865 2023-12-29 03:55:54.000000 adata-2.0.1b0/adata/stock/market/index_market/market_index_east.py
+-rw-rw-rw-   0        0        0     1746 2023-08-08 11:47:56.000000 adata-2.0.1b0/adata/stock/market/index_market/market_index_template.py
+-rw-rw-rw-   0        0        0     8246 2023-08-08 11:48:17.000000 adata-2.0.1b0/adata/stock/market/index_market/market_index_ths.py
+-rw-rw-rw-   0        0        0     3199 2023-10-18 04:50:22.000000 adata-2.0.1b0/adata/stock/market/stock_dividend.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.237185 adata-2.0.1b0/adata/stock/market/stock_market/
+-rw-rw-rw-   0        0        0      176 2023-10-10 02:59:10.000000 adata-2.0.1b0/adata/stock/market/stock_market/__init__.py
+-rw-rw-rw-   0        0        0     3519 2024-04-17 10:25:01.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market.py
+-rw-rw-rw-   0        0        0    11398 2023-12-04 12:31:36.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market_baidu.py
+-rw-rw-rw-   0        0        0     5415 2023-09-18 06:30:43.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market_qq.py
+-rw-rw-rw-   0        0        0     2666 2023-07-07 08:19:03.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market_sina.py
+-rw-rw-rw-   0        0        0     2658 2023-09-13 12:58:10.000000 adata-2.0.1b0/adata/stock/market/stock_market/stock_market_template.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:56:33.134520 adata-2.0.1b0/adata.egg-info/
+-rw-rw-rw-   0        0        0    21039 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3649 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 10:56:33.000000 adata-2.0.1b0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:56:33.240186 adata-2.0.1b0/setup.cfg
+-rw-rw-rw-   0        0        0     1838 2023-12-04 12:31:36.000000 adata-2.0.1b0/setup.py
```

### Comparing `adata-2.0.0b0/LICENSE` & `adata-2.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/PKG-INFO` & `adata-2.0.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 2.0.0b0
+Version: 2.0.1b0
 Summary: A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line
 Home-page: https://github.com/1nchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adata Version: 2.0.0b0 Summary: A Data,A
+Metadata-Version: 2.1 Name: adata Version: 2.0.1b0 Summary: A Data,A
 Stock,ETF,Bond,Quant,Stock Market,K Line Home-page: https://github.com/1nchaos/
 adata Author: 1nchaos Author-email: 9527@1nchaos.com License: Apache License
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `adata-2.0.0b0/README.md` & `adata-2.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/__init__.py` & `adata-2.0.1b0/adata/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/__version__.py` & `adata-2.0.1b0/adata/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-VERSION = (2, 0, 0)
+VERSION = (2, 0, 1)
 PRERELEASE = 'beta'  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
     if prerelease is not None:
```

### Comparing `adata-2.0.0b0/adata/bond/info/bond_code.py` & `adata-2.0.1b0/adata/bond/info/bond_code.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/base/base_ths.py` & `adata-2.0.1b0/adata/common/base/base_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/headers/__init__.py` & `adata-2.0.1b0/adata/common/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/headers/baidu_headers.py` & `adata-2.0.1b0/adata/common/headers/baidu_headers.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/headers/east_headers.py` & `adata-2.0.1b0/adata/common/headers/east_headers.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/headers/sina_headers.py` & `adata-2.0.1b0/adata/common/headers/sina_headers.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/headers/ths_headers.py` & `adata-2.0.1b0/adata/common/headers/ths_headers.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/js/hexin.js` & `adata-2.0.1b0/adata/common/js/hexin.js`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/js/ths.js` & `adata-2.0.1b0/adata/common/js/ths.js`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/utils/cookie.py` & `adata-2.0.1b0/adata/common/utils/cookie.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/utils/snowflake.py` & `adata-2.0.1b0/adata/common/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/common/utils/sunrequests.py` & `adata-2.0.1b0/adata/common/utils/sunrequests.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/fund/info/fund_info.py` & `adata-2.0.1b0/adata/fund/info/fund_info.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/fund/market/etf_market.py` & `adata-2.0.1b0/adata/fund/market/etf_market.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,7 +47,13 @@
         :return: k线行情数据 [ETF代码,交易时间，交易日期，开，高，低，当前价格,成交量，成交额]
         ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000,存储芯片
         k:   1,      7,      8,       9,      11,      13,         19,        name
         成交量：股 820953530  821万手
         成交额：元 16959251000.000 169.6亿
         """
         return self.ths.get_market_etf_current_ths(fund_code, k_type)
+
+
+if __name__ == '__main__':
+    print(ETFMarket().get_market_etf(fund_code='512880', start_date='2024-01-01'))
+    print(ETFMarket().get_market_etf_min(fund_code='512880'))
+    print(ETFMarket().get_market_etf_current(fund_code='512880'))
```

### Comparing `adata-2.0.0b0/adata/fund/market/etf_market_template.py` & `adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_template.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-@summary: etf 行情
+@summary: 股票概念 行情
 """
 
 
-class ETFMarketTemplate(object):
+class ConceptMarketTemplate(object):
     """
-    etf 行情
+    股票概念 行情
     """
-    _MARKET_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount',
-                       'change', 'change_pct']
-    _MARKET_ETF_MIN_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'price', 'avg_price', 'volume', 'amount',
-                               'change', 'change_pct']
-    _MARKET_ETF_CURRENT_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume',
-                                   'amount', 'change', 'change_pct']
+    _MARKET_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'close', 'volume',
+                       'amount', 'change', 'change_pct']
+    _MARKET_CONCEPT_MIN_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'price', 'avg_price', 'volume', 'amount',
+                                   'change', 'change_pct']
+    _MARKET_CONCEPT_CURRENT_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'price',
+                                       'volume', 'amount', 'change', 'change_pct']
```

### Comparing `adata-2.0.0b0/adata/fund/market/etf_market_ths.py` & `adata-2.0.1b0/adata/fund/market/etf_market_ths.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             return Exception(THS_IP_LIMIT_MSG)
         result_text = text[text.index('{'):-1]
         data_list = json.loads(result_text)['data'].split(';')
         data = []
         for d in data_list:
             data.append(str(d).split(',')[0:7])
         result_df = pd.DataFrame(data=data, columns=['trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount'])
-        result_df['index_code'] = fund_code
+        result_df['fund_code'] = fund_code
         result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
         result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
         result_df['close'] = result_df['close'].astype(float)
         result_df['change'] = result_df['close'] - result_df['close'].shift(1)
         result_df['change_pct'] = result_df['change'] / result_df['close'].shift(1) * 100
 
         # 3. 清洗数据
@@ -88,15 +88,15 @@
         trade_date = result_json['date']
         data_list = result_json['data'].split(';')
         data = []
         for d in data_list:
             data.append(str(d).split(','))
         # 3. 封装数据
         result_df = pd.DataFrame(data=data, columns=['trade_time', 'price', 'amount', 'avg_price', 'volume'])
-        result_df['index_code'] = fund_code
+        result_df['fund_code'] = fund_code
         result_df['trade_time'] = trade_date + result_df['trade_time']
         result_df['trade_date'] = pd.to_datetime(trade_date, format='%Y%m%d').strftime('%Y-%m-%d')
         result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
             '%Y-%m-%d %H:%M:%S')
         result_df['price'] = result_df['price']
         result_df['change'] = result_df['price'].astype(float) - float(pre_price)
         result_df['change_pct'] = result_df['change'] / float(pre_price) * 100
@@ -135,15 +135,15 @@
                   '19': 'amount', 'open': 'status'}
         result_df = pd.DataFrame(data=data_list).rename(columns=rename)
         result_df['trade_time'] = result_df['trade_date'] + result_df['dt']
         result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
             '%Y-%m-%d %H:%M:%S')
         columns = ['trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume', 'amount']
         result_df = result_df[columns]
-        result_df['index_code'] = fund_code
+        result_df['fund_code'] = fund_code
         result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
         result_df['change'] = None
         result_df['change_pct'] = None
         return result_df[self._MARKET_ETF_CURRENT_COLUMNS]
 
 
 if __name__ == '__main__':
```

### Comparing `adata-2.0.0b0/adata/sentiment/north_flow.py` & `adata-2.0.1b0/adata/sentiment/north_flow.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/sentiment/securities_margin.py` & `adata-2.0.1b0/adata/sentiment/securities_margin.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/sentiment/stock_lifting.py` & `adata-2.0.1b0/adata/sentiment/stock_lifting.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2005.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2005.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2006.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2006.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2007.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2007.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2008.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2008.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2009.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2009.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2010.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2010.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2011.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2011.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2012.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2012.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2013.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2013.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2014.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2014.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2015.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2015.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2016.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2016.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2017.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2017.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2018.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2018.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2019.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2019.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2020.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2020.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2021.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2021.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2022.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2022.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2023.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2023.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/calendar/2024.csv` & `adata-2.0.1b0/adata/stock/cache/calendar/2024.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/code.csv` & `adata-2.0.1b0/adata/stock/cache/code.csv`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/cache/index_code_rel_ths.py` & `adata-2.0.1b0/adata/stock/cache/index_code_rel_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/info/concept/stock_concept_east.py` & `adata-2.0.1b0/adata/stock/info/concept/stock_concept_east.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/info/concept/stock_concept_ths.py` & `adata-2.0.1b0/adata/stock/info/concept/stock_concept_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/info/stock_code.py` & `adata-2.0.1b0/adata/stock/info/stock_code.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/info/stock_index.py` & `adata-2.0.1b0/adata/stock/info/stock_index.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/info/trade_calendar.py` & `adata-2.0.1b0/adata/stock/info/trade_calendar.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/__init__.py` & `adata-2.0.1b0/adata/stock/market/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_east.py` & `adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_east.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_template.py` & `adata-2.0.1b0/adata/fund/market/etf_market_template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-@summary: 股票概念 行情
+@summary: etf 行情
 """
 
 
-class ConceptMarketTemplate(object):
+class ETFMarketTemplate(object):
     """
-    股票概念 行情
+    etf 行情
     """
-    _MARKET_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'close', 'volume',
-                       'amount', 'change', 'change_pct']
-    _MARKET_CONCEPT_MIN_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'price', 'avg_price', 'volume', 'amount',
-                                   'change', 'change_pct']
-    _MARKET_CONCEPT_CURRENT_COLUMNS = ['index_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'price',
-                                       'volume', 'amount', 'change', 'change_pct']
+    _MARKET_COLUMNS = ['fund_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount',
+                       'change', 'change_pct']
+    _MARKET_ETF_MIN_COLUMNS = ['fund_code', 'trade_time', 'trade_date', 'price', 'avg_price', 'volume', 'amount',
+                               'change', 'change_pct']
+    _MARKET_ETF_CURRENT_COLUMNS = ['fund_code', 'trade_time', 'trade_date', 'open', 'high', 'low', 'price', 'volume',
+                                   'amount', 'change', 'change_pct']
```

### Comparing `adata-2.0.0b0/adata/stock/market/concepth_market/concept_market_ths.py` & `adata-2.0.1b0/adata/stock/market/concepth_market/concept_market_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/index_market/market_index.py` & `adata-2.0.1b0/adata/stock/market/index_market/market_index.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/index_market/market_index_east.py` & `adata-2.0.1b0/adata/stock/market/index_market/market_index_east.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/index_market/market_index_template.py` & `adata-2.0.1b0/adata/stock/market/index_market/market_index_template.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/index_market/market_index_ths.py` & `adata-2.0.1b0/adata/stock/market/index_market/market_index_ths.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/stock_dividend.py` & `adata-2.0.1b0/adata/stock/market/stock_dividend.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/stock_market/stock_market.py` & `adata-2.0.1b0/adata/stock/market/stock_market/stock_market.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/stock_market/stock_market_baidu.py` & `adata-2.0.1b0/adata/stock/market/stock_market/stock_market_baidu.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/stock_market/stock_market_qq.py` & `adata-2.0.1b0/adata/stock/market/stock_market/stock_market_qq.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/stock_market/stock_market_sina.py` & `adata-2.0.1b0/adata/stock/market/stock_market/stock_market_sina.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata/stock/market/stock_market/stock_market_template.py` & `adata-2.0.1b0/adata/stock/market/stock_market/stock_market_template.py`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/adata.egg-info/PKG-INFO` & `adata-2.0.1b0/adata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 2.0.0b0
+Version: 2.0.1b0
 Summary: A Data,A Stock,ETF,Bond,Quant,Stock Market,K Line
 Home-page: https://github.com/1nchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adata Version: 2.0.0b0 Summary: A Data,A
+Metadata-Version: 2.1 Name: adata Version: 2.0.1b0 Summary: A Data,A
 Stock,ETF,Bond,Quant,Stock Market,K Line Home-page: https://github.com/1nchaos/
 adata Author: 1nchaos Author-email: 9527@1nchaos.com License: Apache License
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `adata-2.0.0b0/adata.egg-info/SOURCES.txt` & `adata-2.0.1b0/adata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adata-2.0.0b0/setup.py` & `adata-2.0.1b0/setup.py`

 * *Files identical despite different names*

