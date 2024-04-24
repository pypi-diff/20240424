# Comparing `tmp/notalib-2.2.0.tar.gz` & `tmp/notalib-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notalib-2.2.0.tar", max compression
+gzip compressed data, was "notalib-2.3.0.tar", max compression
```

## Comparing `notalib-2.2.0.tar` & `notalib-2.3.0.tar`

### file list

```diff
@@ -1,56 +1,76 @@
--rw-r--r--   0        0        0     1068 2022-12-12 12:38:13.108694 notalib-2.2.0/LICENSE
--rw-r--r--   0        0        0    14674 2023-08-18 15:13:12.348296 notalib-2.2.0/README.md
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/__init__.py
--rw-r--r--   0        0        0      273 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/array.py
--rw-r--r--   0        0        0     1475 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/array_test.py
--rw-r--r--   0        0        0      875 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/combinator.py
--rw-r--r--   0        0        0     3914 2023-08-18 14:40:42.730446 notalib-2.2.0/notalib/date.py
--rw-r--r--   0        0        0     2518 2023-08-18 13:35:28.281217 notalib-2.2.0/notalib/date_test.py
--rw-r--r--   0        0        0      880 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/deprecated.py
--rw-r--r--   0        0        0     2940 2023-01-18 09:17:40.644758 notalib-2.2.0/notalib/dict.py
--rw-r--r--   0        0        0     2108 2023-01-18 09:17:40.644758 notalib-2.2.0/notalib/dict_test.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/__init__.py
--rw-r--r--   0        0        0     2102 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/auth.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/clickhouse/__init__.py
--rw-r--r--   0        0        0     1685 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/clickhouse/base.py
--rw-r--r--   0        0        0     1002 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/clickhouse/mutations.py
--rw-r--r--   0        0        0     1387 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/clickhouse/profiler.py
--rw-r--r--   0        0        0      796 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/clickhouse/wait.py
--rw-r--r--   0        0        0     1392 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/colorlog.py
--rw-r--r--   0        0        0     1074 2022-12-12 12:38:13.108694 notalib-2.2.0/notalib/django/filterset.py
--rw-r--r--   0        0        0      967 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django/filterset_test.py
--rw-r--r--   0        0        0     1613 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django/formplus.py
--rw-r--r--   0        0        0     1354 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django/formplus_test.py
--rw-r--r--   0        0        0      196 2023-08-18 13:35:28.281217 notalib-2.2.0/notalib/django/http.py
--rw-r--r--   0        0        0     2298 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django/request_time_middleware.py
--rw-r--r--   0        0        0      998 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django/stream.py
--rw-r--r--   0        0        0      810 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django/stream_test.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django_xauth/__init__.py
--rw-r--r--   0        0        0      101 2023-06-27 09:19:55.956175 notalib-2.2.0/notalib/django_xauth/apps.py
--rw-r--r--   0        0        0      498 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django_xauth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django_xauth/migrations/__init__.py
--rw-r--r--   0        0        0       97 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django_xauth/models.py
--rw-r--r--   0        0        0      180 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django_xauth/serializers.py
--rw-r--r--   0        0        0      325 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django_xauth/urls.py
--rw-r--r--   0        0        0     1009 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/django_xauth/views.py
--rw-r--r--   0        0        0     8229 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/filterset.py
--rw-r--r--   0        0        0     1858 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/filterset_test.py
--rw-r--r--   0        0        0      303 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/format.py
--rw-r--r--   0        0        0     1736 2023-01-18 09:17:40.644758 notalib-2.2.0/notalib/git.py
--rw-r--r--   0        0        0     1920 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/hypertext.py
--rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/pandas/__init__.py
--rw-r--r--   0        0        0      973 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/pandas/pandasplus.py
--rw-r--r--   0        0        0     1571 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/pandas/pandasplus_test.py
--rw-r--r--   0        0        0     3304 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/polosa.py
--rw-r--r--   0        0        0     1217 2022-12-12 12:38:13.112694 notalib-2.2.0/notalib/range.py
--rw-r--r--   0        0        0        0 2023-08-18 14:49:23.091644 notalib-2.2.0/notalib/tablib/__init__.py
--rw-r--r--   0        0        0    10420 2023-08-18 14:49:23.091644 notalib-2.2.0/notalib/tablib/dataset.py
--rw-r--r--   0        0        0     4306 2023-08-18 14:49:23.091644 notalib-2.2.0/notalib/tablib/dataset_test.py
--rw-r--r--   0        0        0      492 2023-08-18 14:49:23.095644 notalib-2.2.0/notalib/tablib/shortcuts.py
--rw-r--r--   0        0        0      604 2022-12-12 12:38:13.116694 notalib-2.2.0/notalib/time.py
--rw-r--r--   0        0        0      652 2023-01-18 09:17:40.644758 notalib-2.2.0/notalib/timedelta.py
--rw-r--r--   0        0        0      925 2023-01-18 09:17:40.644758 notalib-2.2.0/notalib/timedelta_test.py
--rw-r--r--   0        0        0     2214 2022-12-12 12:38:13.116694 notalib-2.2.0/notalib/trendsetter.py
--rw-r--r--   0        0        0       22 2022-12-12 12:38:13.116694 notalib-2.2.0/notalib/utf.py
--rw-r--r--   0        0        0     1092 2023-08-18 15:13:19.288260 notalib-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    15504 1970-01-01 00:00:00.000000 notalib-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-12 12:38:13.108694 notalib-2.3.0/LICENSE
+-rw-r--r--   0        0        0    14760 2024-04-24 09:01:07.565307 notalib-2.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/__init__.py
+-rw-r--r--   0        0        0      273 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/array.py
+-rw-r--r--   0        0        0     1475 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/array_test.py
+-rw-r--r--   0        0        0      915 2024-04-24 09:01:07.565307 notalib-2.3.0/notalib/combinator.py
+-rw-r--r--   0        0        0      849 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/combinator_test.py
+-rw-r--r--   0        0        0     3914 2023-08-18 14:40:42.730446 notalib-2.3.0/notalib/date.py
+-rw-r--r--   0        0        0     4956 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/date_test.py
+-rw-r--r--   0        0        0      880 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/deprecated.py
+-rw-r--r--   0        0        0      836 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/deprecated_test.py
+-rw-r--r--   0        0        0     2940 2023-01-18 09:17:40.644758 notalib-2.3.0/notalib/dict.py
+-rw-r--r--   0        0        0     4083 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/dict_test.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/__init__.py
+-rw-r--r--   0        0        0     2102 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/auth.py
+-rw-r--r--   0        0        0     4670 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/auth_test.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1685 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/clickhouse/base.py
+-rw-r--r--   0        0        0     3448 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/clickhouse/base_test.py
+-rw-r--r--   0        0        0     1002 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/clickhouse/mutations.py
+-rw-r--r--   0        0        0      836 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/clickhouse/mutations_test.py
+-rw-r--r--   0        0        0     1387 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/clickhouse/profiler.py
+-rw-r--r--   0        0        0     2278 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/clickhouse/profiler_test.py
+-rw-r--r--   0        0        0      796 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/clickhouse/wait.py
+-rw-r--r--   0        0        0      740 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/clickhouse/wait_test.py
+-rw-r--r--   0        0        0     1392 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/colorlog.py
+-rw-r--r--   0        0        0     1234 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/colorlog_test.py
+-rw-r--r--   0        0        0     1074 2022-12-12 12:38:13.108694 notalib-2.3.0/notalib/django/filterset.py
+-rw-r--r--   0        0        0     1351 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/filterset_test.py
+-rw-r--r--   0        0        0     1732 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/formplus.py
+-rw-r--r--   0        0        0     4518 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/formplus_test.py
+-rw-r--r--   0        0        0      196 2023-08-18 13:35:28.281217 notalib-2.3.0/notalib/django/http.py
+-rw-r--r--   0        0        0      406 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/http_test.py
+-rw-r--r--   0        0        0     2298 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/django/request_time_middleware.py
+-rw-r--r--   0        0        0     2687 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django/request_time_middleware_test.py
+-rw-r--r--   0        0        0      998 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/django/stream.py
+-rw-r--r--   0        0        0      810 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/django/stream_test.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/django_xauth/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-27 09:19:55.956175 notalib-2.3.0/notalib/django_xauth/apps.py
+-rw-r--r--   0        0        0      498 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/django_xauth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/django_xauth/migrations/__init__.py
+-rw-r--r--   0        0        0       97 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/django_xauth/models.py
+-rw-r--r--   0        0        0      180 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/django_xauth/serializers.py
+-rw-r--r--   0        0        0      368 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django_xauth/urls.py
+-rw-r--r--   0        0        0     1128 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django_xauth/views.py
+-rw-r--r--   0        0        0     1466 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/django_xauth/views_test.py
+-rw-r--r--   0        0        0     8264 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/filterset.py
+-rw-r--r--   0        0        0     1858 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/filterset_test.py
+-rw-r--r--   0        0        0      394 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/format.py
+-rw-r--r--   0        0        0      643 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/format_test.py
+-rw-r--r--   0        0        0     1736 2023-01-18 09:17:40.644758 notalib-2.3.0/notalib/git.py
+-rw-r--r--   0        0        0     3561 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/git_test.py
+-rw-r--r--   0        0        0     1918 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/hypertext.py
+-rw-r--r--   0        0        0     3112 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/hypertext_test.py
+-rw-r--r--   0        0        0        0 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/pandas/__init__.py
+-rw-r--r--   0        0        0      973 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/pandas/pandasplus.py
+-rw-r--r--   0        0        0     1962 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/pandas/pandasplus_test.py
+-rw-r--r--   0        0        0     3304 2022-12-12 12:38:13.112694 notalib-2.3.0/notalib/polosa.py
+-rw-r--r--   0        0        0     2221 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/polosa_test.py
+-rw-r--r--   0        0        0     1245 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/range.py
+-rw-r--r--   0        0        0     1893 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/range_test.py
+-rw-r--r--   0        0        0        0 2023-08-18 14:49:23.091644 notalib-2.3.0/notalib/tablib/__init__.py
+-rw-r--r--   0        0        0    10420 2023-08-18 14:49:23.091644 notalib-2.3.0/notalib/tablib/dataset.py
+-rw-r--r--   0        0        0     4306 2023-08-18 14:49:23.091644 notalib-2.3.0/notalib/tablib/dataset_test.py
+-rw-r--r--   0        0        0      492 2023-08-18 14:49:23.095644 notalib-2.3.0/notalib/tablib/shortcuts.py
+-rw-r--r--   0        0        0      900 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/tablib/shortcuts_test.py
+-rw-r--r--   0        0        0     1127 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/test_fakes.py
+-rw-r--r--   0        0        0      642 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/time.py
+-rw-r--r--   0        0        0      934 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/time_test.py
+-rw-r--r--   0        0        0      652 2023-01-18 09:17:40.644758 notalib-2.3.0/notalib/timedelta.py
+-rw-r--r--   0        0        0      925 2023-01-18 09:17:40.644758 notalib-2.3.0/notalib/timedelta_test.py
+-rw-r--r--   0        0        0     2214 2022-12-12 12:38:13.116694 notalib-2.3.0/notalib/trendsetter.py
+-rw-r--r--   0        0        0     2880 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/trendsetter_test.py
+-rw-r--r--   0        0        0       62 2024-04-24 09:01:07.569307 notalib-2.3.0/notalib/utf.py
+-rw-r--r--   0        0        0     1124 2024-04-24 09:01:13.589305 notalib-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    15590 1970-01-01 00:00:00.000000 notalib-2.3.0/PKG-INFO
```

### Comparing `notalib-2.2.0/LICENSE` & `notalib-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/README.md` & `notalib-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 ```sh
 poetry add notalib
 ```
 
 
 ## Compatibility promise
 
-Version numbers follow the semver rules. Minor releases are backwards-compatible. It should be safe to update, say, from 1.2 to 1.4.
-
-Major releases are not backwards-compatible. If you upgrade, say, from 1.4 to 2.0, read the release notes to see what's changed.
+Version numbers follow the semver rules.
+* Minor releases are backwards-compatible. For example, an upgrade from 1.2 to 1.4 should be safe.
+* Major releases are not backwards-compatible. For example, an upgrade from 1.4 to 2.0 is unsafe — read the release notes to see what's changed.
 
 
 ## Maintenance & bugfixes
 
 While I try to fix bugs, add new features, and review any PRs when I have time, there're no promises and no set timeframes, even if a bug is critical. That's a project I do in my free time, free of charge.
 
 If that's not enough for you or you have an urgent request, there are paid maintenance options (bugfixing, features, expedite PR review, 24h security responses). Contact me for prices: m1kc@yandex.ru
@@ -322,16 +322,17 @@
 
 #### notalib.django.xauth
 
 Endpoints for easier authentication in APIs. Requires Django REST framework.
 
 Provides endpoints:
 
-* `/xauth/check` — returns code 200 if client is authenticated (or global permissions are set to AllowAny), 403 if not
-* `/xauth/auth-post` — authenticates a client; accepts two POST parameters `username` and `password`; returns code 200 on success and 403 on failure
+* `GET /xauth/check` — returns code 200 if client is authenticated (or global permissions are set to AllowAny), 403 if not
+* `POST /xauth/auth-post` — authenticates a client; accepts two POST parameters `username` and `password`; returns code 200 on success and 403 on failure
+* `POST /xauth/logout` — de-authenticates a client
 
 How to use:
 
 1. Make sure Django REST framework is installed.
 2. Add `'notalib.django_xauth'` to INSTALLED_APPS.
 3. Run `manage.py migrate django_xauth` (doesn't actually change your DB).
 4. Add something like this to your urls.py: `path('xauth/', include('notalib.django_xauth.urls')),`
```

### Comparing `notalib-2.2.0/notalib/array_test.py` & `notalib-2.3.0/notalib/array_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/combinator.py` & `notalib-2.3.0/notalib/combinator.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 			raise Exception("Combinator cannot combine with empty set")
 
 		if len(self.result) == 0:
 			for i in new_set:
 				self.result += [[i]]
 		else:
 			newresult = []
-			for tuple in self.result:
+			for tuple in self.result:		# FIXME: Redefinition of standard type
 				for i in new_set:
 					newresult += [tuple + [i]]
 			self.result = newresult
 		#print("New result", self.result)
 
 	def get_result(self):
 		return self.result
```

### Comparing `notalib-2.2.0/notalib/date.py` & `notalib-2.3.0/notalib/date.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/deprecated.py` & `notalib-2.3.0/notalib/deprecated.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/dict.py` & `notalib-2.3.0/notalib/dict.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/auth.py` & `notalib-2.3.0/notalib/django/auth.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/clickhouse/base.py` & `notalib-2.3.0/notalib/django/clickhouse/base.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/clickhouse/mutations.py` & `notalib-2.3.0/notalib/django/clickhouse/mutations.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/clickhouse/profiler.py` & `notalib-2.3.0/notalib/django/clickhouse/profiler.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/clickhouse/wait.py` & `notalib-2.3.0/notalib/django/clickhouse/wait.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/colorlog.py` & `notalib-2.3.0/notalib/django/colorlog.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/filterset.py` & `notalib-2.3.0/notalib/django/filterset.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/filterset_test.py` & `notalib-2.3.0/notalib/django/filterset_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,7 +35,23 @@
 		'street': 'Hi st.',
 		'building': 344,
 	}
 	r = from_request(AddressFilterSet, source)
 	assert r.is_valid
 	r.data.unfreeze(['country', 'city', 'street', 'building'])
 	assert r.data.as_dict() == expected
+
+	AddressFilterSet = create_filter_set({
+		'city': CharField(required=True),
+		'building': IntegerField(required=True, min_value=0),
+		'street': CharField(),
+	}, required=['city'], parent=CountryFilterSet)
+
+	r = from_request(AddressFilterSet, {
+		'country': 'Russia',
+		'city': 'Penza',
+		'building': 344,
+	})
+
+	assert not r.is_valid
+	assert r.data is None
+	assert len(r.errors) == 1
```

### Comparing `notalib-2.2.0/notalib/django/formplus.py` & `notalib-2.3.0/notalib/django/formplus.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 class MonthField(forms.CharField):
 	def clean(self, value):
 		if value is None: return None
 		try:
 			return parse_month(value)
 		except:
+			# FIXME: The "parse_month" function accepts another format "YYYY-M"
 			raise forms.ValidationError('Not a valid month (expected YYYY-MM)')
 
 
 class ChoiceWithDefault(forms.ChoiceField):
 	def __init__(self, *args, **kwargs):
 		default_value = kwargs['default']
 		del kwargs['default']
@@ -26,15 +27,15 @@
 
 class IntegerArrayField(forms.CharField):
 	def __init__(self, sep='|', *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.sep = sep
 
 	def clean(self, value):
-		if value is None:
+		if value is None:		# An empty string will raise an exception
 			return None
 		return list(map(int, value.split(self.sep)))
 
 
 class StringArrayField(forms.CharField):
 	def __init__(self, sep='|', strip=True, *args, **kwargs):
 		super().__init__(*args, **kwargs)
@@ -53,12 +54,12 @@
 class MonthArrayField(forms.CharField):
 	def __init__(self, sep='|', *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.sep = sep
 
 	def clean(self, value):
 		if value is None: return None
-		value = value.split('|')
+		value = value.split(self.sep)
 		try:
 			return list(map(lambda value: parse_month(value), value))
 		except:
 			raise forms.ValidationError('Not a valid month (expected YYYY-MM)')
```

### Comparing `notalib-2.2.0/notalib/django/request_time_middleware.py` & `notalib-2.3.0/notalib/django/request_time_middleware.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/stream.py` & `notalib-2.3.0/notalib/django/stream.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django/stream_test.py` & `notalib-2.3.0/notalib/django/stream_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/django_xauth/views.py` & `notalib-2.3.0/notalib/django_xauth/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .models import Nothing
 from .serializers import NothingSerializer
 
 from django.http import HttpResponse
-from django.contrib.auth import authenticate, login
+from django.contrib.auth import authenticate, login, logout
 from django.views.decorators.csrf import csrf_exempt
 from rest_framework import viewsets
 from rest_framework.decorators import renderer_classes
 from rest_framework.renderers import JSONRenderer
 
 
 # Example usage:
@@ -24,11 +24,17 @@
 	if user is not None:
 		login(request, user)
 		return HttpResponse('{"result": "ok"}', status=200)
 	else:
 		return HttpResponse('{"result": "fail"}', status=403)
 
 
+@csrf_exempt
+def logout_view(request):
+	logout(request)
+	return HttpResponse('{"result": "ok"}', status=200)
+
+
 @renderer_classes([JSONRenderer])
 class DirtyHackAuthCheckViewSet(viewsets.ReadOnlyModelViewSet):
 	queryset = Nothing.objects.none()
 	serializer_class = NothingSerializer
```

### Comparing `notalib-2.2.0/notalib/filterset.py` & `notalib-2.3.0/notalib/filterset.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 			assert (f in kwargs), f"Field `{f}` is mandatory"
 		for key in kwargs:
 			assert key in self._fields, f"Unknown field `{key}`"
 		self.values = kwargs
 
 	def __getattr__(self, name: str):
 		if name in self.__dict__:
-			return self.__dict__[name]
+			return self.__dict__[name]		# FIXME: This line is unreachable
 
 		assert (not self._frozen), "FilterSet is frozen"
 		return self.values[name]
 
 	def unfreeze(self, expected_fields):
 		assert sorted(expected_fields) == sorted(self._fields), f"Field set mismatch, expected: {self._fields}"
 		self._frozen = False
```

### Comparing `notalib-2.2.0/notalib/filterset_test.py` & `notalib-2.3.0/notalib/filterset_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/git.py` & `notalib-2.3.0/notalib/git.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/hypertext.py` & `notalib-2.3.0/notalib/hypertext.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 	"""
 	Prints an HTML table, row by row, from the given data, using attrs or
 	dictionary keys as columns.
 
 	Two ways to use it:
 
 	* Call header() / entry() / footer() manually
-	
+
 	```
 	>>> from notalib.hypertext import TablePrinter
 	>>> t = TablePrinter(['a', 'b'])
 	>>> t.header()
 	'<table><thead><tr><th>a</th><th>b</th></tr></thead><tbody>'
 	>>> t.entry({'a': 1, 'b': 2})
 	'<tr><td>1</td><td>2</td></tr>\n'
 	>>> t.entry({'a': 11, 'b': 22})
 	'<tr><td>11</td><td>22</td></tr>\n'
 	>>> t.footer()
 	'</tbody></table>'
 	```
 
 	* Pass an iterable to iterator_over()
-	
+
 	```
 	>>> from notalib.hypertext import TablePrinter
 	>>> t = TablePrinter(['a', 'b'])
 	>>> list(t.iterator_over([ {'a': 11, 'b': 22} ]))
 	['<table><thead><tr><th>a</th><th>b</th></tr></thead><tbody>', '<tr><td>11</td><td>22</td></tr>\n', '</tbody></table>']
 	```
 	"""
```

### Comparing `notalib-2.2.0/notalib/pandas/pandasplus.py` & `notalib-2.3.0/notalib/pandas/pandasplus.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/pandas/pandasplus_test.py` & `notalib-2.3.0/notalib/pandas/pandasplus_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .pandasplus import replace_null_objects
+from .pandasplus import replace_null_objects, row_to_dict
 
 from pytest import mark
 from arrow import get as arrow_get
-from pandas import DataFrame, NaT, NA
+from pandas import DataFrame, NaT, NA, Series
 
 
 SOURCE_DATAFRAME = DataFrame(
 	{
 		"dates": [arrow_get("2021-09-07").date(), arrow_get("2007-01-01").date(), NaT],
 		"strings": ["Some Data", None, NA],
 		"numbers": [1511, NA, 0],
@@ -59,7 +59,19 @@
 
 		assert proc.dates.tolist() == expected_proc['dates']
 		assert proc.strings.tolist() == expected_proc['strings']
 		assert proc.numbers.tolist() == expected_proc['numbers']
 
 	else:
 		assert proc.empty
+
+
+@mark.parametrize(
+	"row, key_as, expected_first_row",
+	[
+		((0, Series({'A': 1, 'B': 2})), None, {'A': 1, 'B': 2}),
+		((15, Series({'A': 1, 'B': 2})), 'RowID', {'A': 1, 'B': 2, 'RowID': 15}),
+		((15, Series({'A': 1, 'B': 2})), 'A', {'A': 15, 'B': 2}),
+	]
+)
+def test_row_to_dict(row, key_as, expected_first_row):
+	assert row_to_dict(row, key_as) == expected_first_row
```

### Comparing `notalib-2.2.0/notalib/polosa.py` & `notalib-2.3.0/notalib/polosa.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/range.py` & `notalib-2.3.0/notalib/range.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 	"""
 	def __init__(self, start, end):
 		self.start = start
 		self.end = end
 		# self.duration = self.end - self.start
 
 	def is_overlapped(self, other_range):
+		# TODO: Can be simplified
 		if max(self.start, other_range.start) < min(self.end, other_range.end):
 			return True
 		else:
 			return False
 
 	def get_overlapped_range(self, other_range):
 		if not self.is_overlapped(other_range): return
```

### Comparing `notalib-2.2.0/notalib/tablib/dataset.py` & `notalib-2.3.0/notalib/tablib/dataset.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/tablib/dataset_test.py` & `notalib-2.3.0/notalib/tablib/dataset_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/time.py` & `notalib-2.3.0/notalib/time.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 		with timing:
 			do_something()
 
 		timing = Timing()
 		with timing:
 			do_something()
 		print(timing.result)
+
+	TODO:
+		* Add the examples section.
 	"""
 	def __init__(self, auto_print=False):
 		super(Timing, self).__init__()
 		self.result = None
 		self._start = None
 		self.auto_print = auto_print
```

### Comparing `notalib-2.2.0/notalib/timedelta.py` & `notalib-2.3.0/notalib/timedelta.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/timedelta_test.py` & `notalib-2.3.0/notalib/timedelta_test.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/notalib/trendsetter.py` & `notalib-2.3.0/notalib/trendsetter.py`

 * *Files identical despite different names*

### Comparing `notalib-2.2.0/pyproject.toml` & `notalib-2.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notalib"
-version = "2.2.0"
+version = "2.3.0"
 description = "A collection of utility functions & classes"
 authors = ["m1kc (Max Musatov) <m1kc@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/m1kc/notalib"
 repository = "https://github.com/m1kc/notalib.git"
 documentation = "https://github.com/m1kc/notalib"
@@ -29,14 +29,15 @@
   {version = "*", python = "<3.9"}
 ]
 pandas = [
   {version = "^1.1.5", python = ">=3.9"},
   {version = "*", python = "<3.9"}
 ]
 tablib = "^3.4.0"
+djangorestframework = "^3.15.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
```

### Comparing `notalib-2.2.0/PKG-INFO` & `notalib-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notalib
-Version: 2.2.0
+Version: 2.3.0
 Summary: A collection of utility functions & classes
 Home-page: https://github.com/m1kc/notalib
 License: MIT
 Keywords: utility,django,pandas
 Author: m1kc (Max Musatov)
 Author-email: m1kc@yandex.ru
 Requires-Python: >=3.7.3,<4.0.0
@@ -38,17 +38,17 @@
 ```sh
 poetry add notalib
 ```
 
 
 ## Compatibility promise
 
-Version numbers follow the semver rules. Minor releases are backwards-compatible. It should be safe to update, say, from 1.2 to 1.4.
-
-Major releases are not backwards-compatible. If you upgrade, say, from 1.4 to 2.0, read the release notes to see what's changed.
+Version numbers follow the semver rules.
+* Minor releases are backwards-compatible. For example, an upgrade from 1.2 to 1.4 should be safe.
+* Major releases are not backwards-compatible. For example, an upgrade from 1.4 to 2.0 is unsafe — read the release notes to see what's changed.
 
 
 ## Maintenance & bugfixes
 
 While I try to fix bugs, add new features, and review any PRs when I have time, there're no promises and no set timeframes, even if a bug is critical. That's a project I do in my free time, free of charge.
 
 If that's not enough for you or you have an urgent request, there are paid maintenance options (bugfixing, features, expedite PR review, 24h security responses). Contact me for prices: m1kc@yandex.ru
@@ -344,16 +344,17 @@
 
 #### notalib.django.xauth
 
 Endpoints for easier authentication in APIs. Requires Django REST framework.
 
 Provides endpoints:
 
-* `/xauth/check` — returns code 200 if client is authenticated (or global permissions are set to AllowAny), 403 if not
-* `/xauth/auth-post` — authenticates a client; accepts two POST parameters `username` and `password`; returns code 200 on success and 403 on failure
+* `GET /xauth/check` — returns code 200 if client is authenticated (or global permissions are set to AllowAny), 403 if not
+* `POST /xauth/auth-post` — authenticates a client; accepts two POST parameters `username` and `password`; returns code 200 on success and 403 on failure
+* `POST /xauth/logout` — de-authenticates a client
 
 How to use:
 
 1. Make sure Django REST framework is installed.
 2. Add `'notalib.django_xauth'` to INSTALLED_APPS.
 3. Run `manage.py migrate django_xauth` (doesn't actually change your DB).
 4. Add something like this to your urls.py: `path('xauth/', include('notalib.django_xauth.urls')),`
```

