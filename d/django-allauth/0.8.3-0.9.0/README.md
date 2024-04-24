# Comparing `tmp/django-allauth-0.8.3.tar.gz` & `tmp/django-allauth-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-allauth-0.8.3.tar", last modified: Thu Dec  6 23:13:38 2012, max compression, from Unix
+gzip compressed data, was "django-allauth-0.9.0.tar", last modified: Wed Jan 30 22:26:48 2013, max compression, from Unix
```

## Comparing `django-allauth-0.8.3.tar` & `django-allauth-0.9.0.tar`

### file list

```diff
@@ -1,212 +1,221 @@
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:38.000000 django-allauth-0.8.3/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:36.000000 django-allauth-0.8.3/allauth/
--rw-r--r--   0 pennersr   (501) staff       (20)      367 2012-12-06 23:03:16.000000 django-allauth-0.8.3/AUTHORS
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:38.000000 django-allauth-0.8.3/django_allauth.egg-info/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:38.000000 django-allauth-0.8.3/example/
--rw-r--r--   0 pennersr   (501) staff       (20)     1075 2012-06-27 15:47:42.000000 django-allauth-0.8.3/LICENSE
--rw-r--r--   0 pennersr   (501) staff       (20)       96 2012-07-18 02:25:13.000000 django-allauth-0.8.3/MANIFEST.in
--rw-r--r--   0 pennersr   (501) staff       (20)    26627 2012-12-06 23:13:38.000000 django-allauth-0.8.3/PKG-INFO
--rw-r--r--   0 pennersr   (501) staff       (20)    20654 2012-12-06 22:49:03.000000 django-allauth-0.8.3/README.rst
--rw-r--r--   0 pennersr   (501) staff       (20)       59 2012-12-06 23:13:38.000000 django-allauth-0.8.3/setup.cfg
--rw-r--r--   0 pennersr   (501) staff       (20)     4743 2012-12-06 22:56:20.000000 django-allauth-0.8.3/setup.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:47:38.000000 django-allauth-0.8.3/example/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)      503 2012-06-27 15:47:41.000000 django-allauth-0.8.3/example/manage.py
--rw-r--r--   0 pennersr   (501) staff       (20)     5800 2012-09-04 20:00:46.000000 django-allauth-0.8.3/example/settings.py
--rw-r--r--   0 pennersr   (501) staff       (20)      524 2012-06-27 15:47:41.000000 django-allauth-0.8.3/example/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)        1 2012-12-06 23:13:36.000000 django-allauth-0.8.3/django_allauth.egg-info/dependency_links.txt
--rw-r--r--   0 pennersr   (501) staff       (20)    26627 2012-12-06 23:13:36.000000 django-allauth-0.8.3/django_allauth.egg-info/PKG-INFO
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-12-06 23:13:36.000000 django-allauth-0.8.3/django_allauth.egg-info/requires.txt
--rw-r--r--   0 pennersr   (501) staff       (20)     8015 2012-12-06 23:13:36.000000 django-allauth-0.8.3/django_allauth.egg-info/SOURCES.txt
--rw-r--r--   0 pennersr   (501) staff       (20)        8 2012-12-06 23:13:36.000000 django-allauth-0.8.3/django_allauth.egg-info/top_level.txt
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:49:56.000000 django-allauth-0.8.3/allauth/__init__.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:36.000000 django-allauth-0.8.3/allauth/account/
--rw-r--r--   0 pennersr   (501) staff       (20)      726 2012-10-29 21:00:22.000000 django-allauth-0.8.3/allauth/app_settings.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:15.000000 django-allauth-0.8.3/allauth/models.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:36.000000 django-allauth-0.8.3/allauth/socialaccount/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/templates/
--rw-r--r--   0 pennersr   (501) staff       (20)      931 2012-09-08 21:42:17.000000 django-allauth-0.8.3/allauth/tests.py
--rw-r--r--   0 pennersr   (501) staff       (20)      694 2012-06-27 15:50:15.000000 django-allauth-0.8.3/allauth/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     3498 2012-10-29 21:00:13.000000 django-allauth-0.8.3/allauth/utils.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/templates/account/
--rw-r--r--   0 pennersr   (501) staff       (20)      585 2012-09-28 20:35:34.000000 django-allauth-0.8.3/allauth/templates/base.html
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/templates/openid/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:38.000000 django-allauth-0.8.3/allauth/templates/socialaccount/
--rw-r--r--   0 pennersr   (501) staff       (20)      249 2012-06-27 15:50:00.000000 django-allauth-0.8.3/allauth/templates/socialaccount/account_inactive.html
--rw-r--r--   0 pennersr   (501) staff       (20)      324 2012-09-08 22:08:05.000000 django-allauth-0.8.3/allauth/templates/socialaccount/authentication_error.html
--rw-r--r--   0 pennersr   (501) staff       (20)       35 2012-06-27 15:50:00.000000 django-allauth-0.8.3/allauth/templates/socialaccount/base.html
--rw-r--r--   0 pennersr   (501) staff       (20)     1418 2012-09-01 07:19:28.000000 django-allauth-0.8.3/allauth/templates/socialaccount/connections.html
--rw-r--r--   0 pennersr   (501) staff       (20)      482 2012-09-08 22:08:05.000000 django-allauth-0.8.3/allauth/templates/socialaccount/login_cancelled.html
--rw-r--r--   0 pennersr   (501) staff       (20)      755 2012-06-27 15:50:00.000000 django-allauth-0.8.3/allauth/templates/socialaccount/signup.html
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:38.000000 django-allauth-0.8.3/allauth/templates/socialaccount/snippets/
--rw-r--r--   0 pennersr   (501) staff       (20)       52 2012-08-24 19:15:21.000000 django-allauth-0.8.3/allauth/templates/socialaccount/snippets/login_extra.html
--rw-r--r--   0 pennersr   (501) staff       (20)      548 2012-08-24 19:15:21.000000 django-allauth-0.8.3/allauth/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0 pennersr   (501) staff       (20)       40 2012-06-27 15:50:01.000000 django-allauth-0.8.3/allauth/templates/openid/base.html
--rw-r--r--   0 pennersr   (501) staff       (20)      384 2012-07-03 17:05:45.000000 django-allauth-0.8.3/allauth/templates/openid/login.html
--rw-r--r--   0 pennersr   (501) staff       (20)       28 2012-06-27 15:50:00.000000 django-allauth-0.8.3/allauth/templates/account/base.html
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/templates/account/email/
--rw-r--r--   0 pennersr   (501) staff       (20)     2333 2012-09-08 22:08:05.000000 django-allauth-0.8.3/allauth/templates/account/email.html
--rw-r--r--   0 pennersr   (501) staff       (20)      959 2012-11-13 18:04:21.000000 django-allauth-0.8.3/allauth/templates/account/email_confirm.html
--rw-r--r--   0 pennersr   (501) staff       (20)      486 2012-08-29 18:57:51.000000 django-allauth-0.8.3/allauth/templates/account/email_confirmed.html
--rw-r--r--   0 pennersr   (501) staff       (20)     1405 2012-08-24 19:15:21.000000 django-allauth-0.8.3/allauth/templates/account/login.html
--rw-r--r--   0 pennersr   (501) staff       (20)      226 2012-06-27 15:49:59.000000 django-allauth-0.8.3/allauth/templates/account/logout.html
--rw-r--r--   0 pennersr   (501) staff       (20)      420 2012-06-27 15:49:59.000000 django-allauth-0.8.3/allauth/templates/account/password_change.html
--rw-r--r--   0 pennersr   (501) staff       (20)      463 2012-06-27 15:49:59.000000 django-allauth-0.8.3/allauth/templates/account/password_delete.html
--rw-r--r--   0 pennersr   (501) staff       (20)      277 2012-06-27 15:50:00.000000 django-allauth-0.8.3/allauth/templates/account/password_delete_done.html
--rw-r--r--   0 pennersr   (501) staff       (20)      896 2012-09-04 18:34:42.000000 django-allauth-0.8.3/allauth/templates/account/password_reset.html
--rw-r--r--   0 pennersr   (501) staff       (20)      474 2012-09-04 18:35:09.000000 django-allauth-0.8.3/allauth/templates/account/password_reset_done.html
--rw-r--r--   0 pennersr   (501) staff       (20)      973 2012-07-03 17:04:35.000000 django-allauth-0.8.3/allauth/templates/account/password_reset_from_key.html
--rw-r--r--   0 pennersr   (501) staff       (20)      406 2012-06-27 15:49:59.000000 django-allauth-0.8.3/allauth/templates/account/password_set.html
--rw-r--r--   0 pennersr   (501) staff       (20)      889 2012-07-03 17:04:57.000000 django-allauth-0.8.3/allauth/templates/account/signup.html
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/templates/account/snippets/
--rw-r--r--   0 pennersr   (501) staff       (20)      480 2012-09-04 18:40:22.000000 django-allauth-0.8.3/allauth/templates/account/verification_sent.html
--rw-r--r--   0 pennersr   (501) staff       (20)      822 2012-09-04 18:36:10.000000 django-allauth-0.8.3/allauth/templates/account/verified_email_required.html
--rw-r--r--   0 pennersr   (501) staff       (20)      204 2012-08-24 19:15:21.000000 django-allauth-0.8.3/allauth/templates/account/snippets/already_logged_in.html
--rw-r--r--   0 pennersr   (501) staff       (20)      316 2012-10-28 19:38:33.000000 django-allauth-0.8.3/allauth/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0 pennersr   (501) staff       (20)      115 2012-11-24 19:45:15.000000 django-allauth-0.8.3/allauth/templates/account/email/email_confirmation_subject.txt
--rw-r--r--   0 pennersr   (501) staff       (20)      452 2012-06-27 15:49:59.000000 django-allauth-0.8.3/allauth/templates/account/email/password_reset_key_message.txt
--rw-r--r--   0 pennersr   (501) staff       (20)      113 2012-11-24 19:44:52.000000 django-allauth-0.8.3/allauth/templates/account/email/password_reset_key_subject.txt
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:02.000000 django-allauth-0.8.3/allauth/socialaccount/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)      617 2012-11-26 21:06:13.000000 django-allauth-0.8.3/allauth/socialaccount/admin.py
--rw-r--r--   0 pennersr   (501) staff       (20)      908 2012-06-27 15:50:13.000000 django-allauth-0.8.3/allauth/socialaccount/app_settings.py
--rw-r--r--   0 pennersr   (501) staff       (20)      138 2012-06-27 15:50:02.000000 django-allauth-0.8.3/allauth/socialaccount/context_processors.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1961 2012-06-27 15:50:13.000000 django-allauth-0.8.3/allauth/socialaccount/fields.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2242 2012-11-24 18:40:52.000000 django-allauth-0.8.3/allauth/socialaccount/forms.py
--rw-r--r--   0 pennersr   (501) staff       (20)     7199 2012-10-29 20:55:53.000000 django-allauth-0.8.3/allauth/socialaccount/helpers.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/migrations/
--rw-r--r--   0 pennersr   (501) staff       (20)     6753 2012-11-26 21:14:39.000000 django-allauth-0.8.3/allauth/socialaccount/models.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/
--rw-r--r--   0 pennersr   (501) staff       (20)     1540 2012-06-28 18:59:22.000000 django-allauth-0.8.3/allauth/socialaccount/requests.py
--rw-r--r--   0 pennersr   (501) staff       (20)      337 2012-08-21 19:19:55.000000 django-allauth-0.8.3/allauth/socialaccount/signals.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/templatetags/
--rw-r--r--   0 pennersr   (501) staff       (20)     2602 2012-07-01 22:00:44.000000 django-allauth-0.8.3/allauth/socialaccount/tests.py
--rw-r--r--   0 pennersr   (501) staff       (20)      420 2012-06-27 15:50:13.000000 django-allauth-0.8.3/allauth/socialaccount/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2272 2012-11-24 18:40:48.000000 django-allauth-0.8.3/allauth/socialaccount/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:02.000000 django-allauth-0.8.3/allauth/socialaccount/templatetags/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1629 2012-09-04 18:52:45.000000 django-allauth-0.8.3/allauth/socialaccount/templatetags/socialaccount.py
--rw-r--r--   0 pennersr   (501) staff       (20)      174 2012-08-24 19:13:54.000000 django-allauth-0.8.3/allauth/socialaccount/templatetags/socialaccount_tags.py
--rw-r--r--   0 pennersr   (501) staff       (20)      935 2012-07-01 21:36:34.000000 django-allauth-0.8.3/allauth/socialaccount/providers/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1547 2012-06-27 15:50:04.000000 django-allauth-0.8.3/allauth/socialaccount/providers/base.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/github/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/google/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/linkedin/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/persona/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/soundcloud/
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:08.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/__init__.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1237 2012-10-10 20:09:00.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)      164 2012-07-01 21:41:11.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1820 2012-10-29 20:55:51.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)     7424 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/0001_initial.py
--rw-r--r--   0 pennersr   (501) staff       (20)     6058 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/0002_snowflake.py
--rw-r--r--   0 pennersr   (501) staff       (20)     8228 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/0003_tosocialaccount.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1925 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/0004_auto__del_twitteraccount__del_twitterapp.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:08.000000 django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-08-17 18:39:41.000000 django-allauth-0.8.3/allauth/socialaccount/providers/soundcloud/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/soundcloud/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)      905 2012-08-17 19:30:00.000000 django-allauth-0.8.3/allauth/socialaccount/providers/soundcloud/provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)      172 2012-08-17 18:41:33.000000 django-allauth-0.8.3/allauth/socialaccount/providers/soundcloud/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1779 2012-10-29 20:55:52.000000 django-allauth-0.8.3/allauth/socialaccount/providers/soundcloud/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-09-28 20:44:31.000000 django-allauth-0.8.3/allauth/socialaccount/providers/persona/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1028 2012-09-28 22:12:22.000000 django-allauth-0.8.3/allauth/socialaccount/providers/persona/provider.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:36.000000 django-allauth-0.8.3/allauth/socialaccount/providers/persona/templates/
--rw-r--r--   0 pennersr   (501) staff       (20)      173 2012-09-28 21:04:38.000000 django-allauth-0.8.3/allauth/socialaccount/providers/persona/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1537 2012-10-29 20:55:52.000000 django-allauth-0.8.3/allauth/socialaccount/providers/persona/views.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/persona/templates/persona/
--rw-r--r--   0 pennersr   (501) staff       (20)      913 2012-09-28 22:13:34.000000 django-allauth-0.8.3/allauth/socialaccount/providers/persona/templates/persona/auth.html
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:05.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)      286 2012-06-27 15:50:05.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/admin.py
--rw-r--r--   0 pennersr   (501) staff       (20)      205 2012-06-27 15:50:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/forms.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/migrations/
--rw-r--r--   0 pennersr   (501) staff       (20)      643 2012-07-01 21:26:02.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2030 2012-07-01 21:25:35.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)      497 2012-09-04 18:52:45.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/tests.py
--rw-r--r--   0 pennersr   (501) staff       (20)      266 2012-07-01 21:41:11.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2138 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/utils.py
--rw-r--r--   0 pennersr   (501) staff       (20)     4128 2012-10-29 20:55:52.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)     7529 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/migrations/0001_initial.py
--rw-r--r--   0 pennersr   (501) staff       (20)     7741 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/migrations/0002_tosocialaccount.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1958 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/migrations/0003_auto__del_openidaccount.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/openid/migrations/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:09.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1957 2012-08-17 18:56:52.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/client.py
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)      602 2012-07-01 20:45:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)      487 2012-06-27 20:19:38.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     3009 2012-08-17 18:57:22.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:03.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)     6958 2012-10-10 20:26:38.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth/client.py
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)      599 2012-10-10 18:52:03.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth/provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)      485 2012-06-27 20:19:38.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     3579 2012-10-10 19:51:07.000000 django-allauth-0.8.3/allauth/socialaccount/providers/oauth/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:07.000000 django-allauth-0.8.3/allauth/socialaccount/providers/linkedin/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/linkedin/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)      657 2012-10-10 19:56:40.000000 django-allauth-0.8.3/allauth/socialaccount/providers/linkedin/provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)      166 2012-07-01 21:40:21.000000 django-allauth-0.8.3/allauth/socialaccount/providers/linkedin/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2759 2012-10-29 20:55:52.000000 django-allauth-0.8.3/allauth/socialaccount/providers/linkedin/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:04.000000 django-allauth-0.8.3/allauth/socialaccount/providers/google/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/google/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1128 2012-07-01 21:41:40.000000 django-allauth-0.8.3/allauth/socialaccount/providers/google/provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)      163 2012-07-01 21:40:13.000000 django-allauth-0.8.3/allauth/socialaccount/providers/google/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2166 2012-10-29 20:55:52.000000 django-allauth-0.8.3/allauth/socialaccount/providers/google/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:02.000000 django-allauth-0.8.3/allauth/socialaccount/providers/github/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/github/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)      751 2012-07-01 21:41:59.000000 django-allauth-0.8.3/allauth/socialaccount/providers/github/provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)      164 2012-07-01 21:40:04.000000 django-allauth-0.8.3/allauth/socialaccount/providers/github/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1477 2012-10-29 20:55:52.000000 django-allauth-0.8.3/allauth/socialaccount/providers/github/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:10.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/__init__.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/data/
--rw-r--r--   0 pennersr   (501) staff       (20)      116 2012-06-27 15:50:11.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/forms.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2333 2012-07-06 12:17:54.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/locale.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/
--rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)     3269 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/provider.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:36.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/templates/
--rw-r--r--   0 pennersr   (501) staff       (20)      436 2012-07-01 21:39:54.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     3183 2012-10-29 20:44:09.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/views.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:37.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/templates/facebook/
--rw-r--r--   0 pennersr   (501) staff       (20)       81 2012-07-06 12:06:23.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/templates/facebook/channel.html
--rw-r--r--   0 pennersr   (501) staff       (20)     1759 2012-07-06 12:06:23.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/templates/facebook/fbconnect.html
--rw-r--r--   0 pennersr   (501) staff       (20)     7041 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/0001_initial.py
--rw-r--r--   0 pennersr   (501) staff       (20)     7101 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/0002_auto__add_facebookaccesstoken__add_unique_facebookaccesstoken_app_acco.py
--rw-r--r--   0 pennersr   (501) staff       (20)     8978 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/0003_tosocialaccount.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2774 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/0004_auto__del_facebookapp__del_facebookaccesstoken__del_unique_facebookacc.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:11.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)    12870 2012-07-06 12:06:23.000000 django-allauth-0.8.3/allauth/socialaccount/providers/facebook/data/FacebookLocales.xml
--rw-r--r--   0 pennersr   (501) staff       (20)     4545 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/migrations/0001_initial.py
--rw-r--r--   0 pennersr   (501) staff       (20)     9426 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/migrations/0002_genericmodels.py
--rw-r--r--   0 pennersr   (501) staff       (20)     6551 2012-09-03 20:24:06.000000 django-allauth-0.8.3/allauth/socialaccount/migrations/0003_auto__add_unique_socialaccount_uid_provider.py
--rw-r--r--   0 pennersr   (501) staff       (20)     6641 2012-11-26 20:48:56.000000 django-allauth-0.8.3/allauth/socialaccount/migrations/0004_add_sites.py
--rw-r--r--   0 pennersr   (501) staff       (20)     6338 2012-11-26 21:03:49.000000 django-allauth-0.8.3/allauth/socialaccount/migrations/0005_set_sites.py
--rw-r--r--   0 pennersr   (501) staff       (20)     6229 2012-11-26 21:05:15.000000 django-allauth-0.8.3/allauth/socialaccount/migrations/0006_auto__del_field_socialapp_site.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:13.000000 django-allauth-0.8.3/allauth/socialaccount/migrations/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:49:57.000000 django-allauth-0.8.3/allauth/account/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1859 2012-11-24 19:50:34.000000 django-allauth-0.8.3/allauth/account/adapter.py
--rw-r--r--   0 pennersr   (501) staff       (20)      710 2012-08-29 23:08:48.000000 django-allauth-0.8.3/allauth/account/admin.py
--rw-r--r--   0 pennersr   (501) staff       (20)     3944 2012-11-24 17:58:53.000000 django-allauth-0.8.3/allauth/account/app_settings.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1743 2012-10-29 20:55:53.000000 django-allauth-0.8.3/allauth/account/auth_backends.py
--rw-r--r--   0 pennersr   (501) staff       (20)      241 2012-09-04 18:32:43.000000 django-allauth-0.8.3/allauth/account/context_processors.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1625 2012-09-04 19:16:52.000000 django-allauth-0.8.3/allauth/account/decorators.py
--rw-r--r--   0 pennersr   (501) staff       (20)    17634 2012-11-24 19:47:22.000000 django-allauth-0.8.3/allauth/account/forms.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:36.000000 django-allauth-0.8.3/allauth/account/management/
--rw-r--r--   0 pennersr   (501) staff       (20)     1547 2012-11-24 13:56:12.000000 django-allauth-0.8.3/allauth/account/managers.py
--rw-r--r--   0 pennersr   (501) staff       (20)     4166 2012-11-24 19:51:38.000000 django-allauth-0.8.3/allauth/account/models.py
--rw-r--r--   0 pennersr   (501) staff       (20)      748 2012-09-28 20:39:39.000000 django-allauth-0.8.3/allauth/account/signals.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:36.000000 django-allauth-0.8.3/allauth/account/templatetags/
--rw-r--r--   0 pennersr   (501) staff       (20)     5410 2012-11-24 19:34:54.000000 django-allauth-0.8.3/allauth/account/tests.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1222 2012-08-29 17:50:12.000000 django-allauth-0.8.3/allauth/account/urls.py
--rw-r--r--   0 pennersr   (501) staff       (20)     7918 2012-11-24 19:40:31.000000 django-allauth-0.8.3/allauth/account/utils.py
--rw-r--r--   0 pennersr   (501) staff       (20)    15793 2012-11-24 18:40:52.000000 django-allauth-0.8.3/allauth/account/views.py
--rw-r--r--   0 pennersr   (501) staff       (20)        1 2012-06-27 15:49:56.000000 django-allauth-0.8.3/allauth/account/templatetags/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)     1185 2012-06-27 15:49:56.000000 django-allauth-0.8.3/allauth/account/templatetags/account.py
--rw-r--r--   0 pennersr   (501) staff       (20)      153 2012-08-24 19:11:48.000000 django-allauth-0.8.3/allauth/account/templatetags/account_tags.py
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-08-29 19:53:24.000000 django-allauth-0.8.3/allauth/account/management/__init__.py
-drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2012-12-06 23:13:36.000000 django-allauth-0.8.3/allauth/account/management/commands/
--rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-08-29 19:53:27.000000 django-allauth-0.8.3/allauth/account/management/commands/__init__.py
--rw-r--r--   0 pennersr   (501) staff       (20)     2571 2012-08-30 18:46:59.000000 django-allauth-0.8.3/allauth/account/management/commands/account_emailconfirmationmigration.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:48.000000 django-allauth-0.9.0/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/
+-rw-r--r--   0 pennersr   (501) staff       (20)      400 2013-01-30 22:09:07.000000 django-allauth-0.9.0/AUTHORS
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:48.000000 django-allauth-0.9.0/django_allauth.egg-info/
+-rw-r--r--   0 pennersr   (501) staff       (20)     1075 2012-06-27 15:47:42.000000 django-allauth-0.9.0/LICENSE
+-rw-r--r--   0 pennersr   (501) staff       (20)       96 2012-07-18 02:25:13.000000 django-allauth-0.9.0/MANIFEST.in
+-rw-r--r--   0 pennersr   (501) staff       (20)    27615 2013-01-30 22:26:48.000000 django-allauth-0.9.0/PKG-INFO
+-rw-r--r--   0 pennersr   (501) staff       (20)    21442 2013-01-30 22:16:25.000000 django-allauth-0.9.0/README.rst
+-rw-r--r--   0 pennersr   (501) staff       (20)       59 2013-01-30 22:26:48.000000 django-allauth-0.9.0/setup.cfg
+-rw-r--r--   0 pennersr   (501) staff       (20)     4882 2013-01-30 22:11:27.000000 django-allauth-0.9.0/setup.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        1 2013-01-30 22:26:46.000000 django-allauth-0.9.0/django_allauth.egg-info/dependency_links.txt
+-rw-r--r--   0 pennersr   (501) staff       (20)    27615 2013-01-30 22:26:46.000000 django-allauth-0.9.0/django_allauth.egg-info/PKG-INFO
+-rw-r--r--   0 pennersr   (501) staff       (20)       36 2013-01-30 22:26:46.000000 django-allauth-0.9.0/django_allauth.egg-info/requires.txt
+-rw-r--r--   0 pennersr   (501) staff       (20)     8624 2013-01-30 22:26:46.000000 django-allauth-0.9.0/django_allauth.egg-info/SOURCES.txt
+-rw-r--r--   0 pennersr   (501) staff       (20)        8 2013-01-30 22:26:46.000000 django-allauth-0.9.0/django_allauth.egg-info/top_level.txt
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:49:56.000000 django-allauth-0.9.0/allauth/__init__.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/account/
+-rw-r--r--   0 pennersr   (501) staff       (20)      726 2012-10-29 21:00:22.000000 django-allauth-0.9.0/allauth/app_settings.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      235 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/exceptions.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:15.000000 django-allauth-0.9.0/allauth/models.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/socialaccount/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/templates/
+-rw-r--r--   0 pennersr   (501) staff       (20)     1880 2012-12-22 16:09:16.000000 django-allauth-0.9.0/allauth/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      685 2013-01-25 20:53:01.000000 django-allauth-0.9.0/allauth/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     3743 2012-12-15 22:46:57.000000 django-allauth-0.9.0/allauth/utils.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:48.000000 django-allauth-0.9.0/allauth/templates/account/
+-rw-r--r--   0 pennersr   (501) staff       (20)      585 2012-09-28 20:35:34.000000 django-allauth-0.9.0/allauth/templates/base.html
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:48.000000 django-allauth-0.9.0/allauth/templates/openid/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:48.000000 django-allauth-0.9.0/allauth/templates/socialaccount/
+-rw-r--r--   0 pennersr   (501) staff       (20)      249 2012-06-27 15:50:00.000000 django-allauth-0.9.0/allauth/templates/socialaccount/account_inactive.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      324 2012-09-08 22:08:05.000000 django-allauth-0.9.0/allauth/templates/socialaccount/authentication_error.html
+-rw-r--r--   0 pennersr   (501) staff       (20)       35 2012-06-27 15:50:00.000000 django-allauth-0.9.0/allauth/templates/socialaccount/base.html
+-rw-r--r--   0 pennersr   (501) staff       (20)     1418 2012-09-01 07:19:28.000000 django-allauth-0.9.0/allauth/templates/socialaccount/connections.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      482 2012-09-08 22:08:05.000000 django-allauth-0.9.0/allauth/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      755 2012-06-27 15:50:00.000000 django-allauth-0.9.0/allauth/templates/socialaccount/signup.html
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:48.000000 django-allauth-0.9.0/allauth/templates/socialaccount/snippets/
+-rw-r--r--   0 pennersr   (501) staff       (20)       52 2012-08-24 19:15:21.000000 django-allauth-0.9.0/allauth/templates/socialaccount/snippets/login_extra.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      548 2012-08-24 19:15:21.000000 django-allauth-0.9.0/allauth/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0 pennersr   (501) staff       (20)       40 2012-06-27 15:50:01.000000 django-allauth-0.9.0/allauth/templates/openid/base.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      384 2012-07-03 17:05:45.000000 django-allauth-0.9.0/allauth/templates/openid/login.html
+-rw-r--r--   0 pennersr   (501) staff       (20)       28 2012-06-27 15:50:00.000000 django-allauth-0.9.0/allauth/templates/account/base.html
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:48.000000 django-allauth-0.9.0/allauth/templates/account/email/
+-rw-r--r--   0 pennersr   (501) staff       (20)     2333 2012-09-08 22:08:05.000000 django-allauth-0.9.0/allauth/templates/account/email.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      959 2012-11-13 18:04:21.000000 django-allauth-0.9.0/allauth/templates/account/email_confirm.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      486 2012-08-29 18:57:51.000000 django-allauth-0.9.0/allauth/templates/account/email_confirmed.html
+-rw-r--r--   0 pennersr   (501) staff       (20)     1405 2012-08-24 19:15:21.000000 django-allauth-0.9.0/allauth/templates/account/login.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      226 2012-06-27 15:49:59.000000 django-allauth-0.9.0/allauth/templates/account/logout.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      420 2012-06-27 15:49:59.000000 django-allauth-0.9.0/allauth/templates/account/password_change.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      463 2012-06-27 15:49:59.000000 django-allauth-0.9.0/allauth/templates/account/password_delete.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      277 2012-06-27 15:50:00.000000 django-allauth-0.9.0/allauth/templates/account/password_delete_done.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      896 2012-09-04 18:34:42.000000 django-allauth-0.9.0/allauth/templates/account/password_reset.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      474 2012-09-04 18:35:09.000000 django-allauth-0.9.0/allauth/templates/account/password_reset_done.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      973 2012-07-03 17:04:35.000000 django-allauth-0.9.0/allauth/templates/account/password_reset_from_key.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      406 2012-06-27 15:49:59.000000 django-allauth-0.9.0/allauth/templates/account/password_set.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      889 2012-07-03 17:04:57.000000 django-allauth-0.9.0/allauth/templates/account/signup.html
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:48.000000 django-allauth-0.9.0/allauth/templates/account/snippets/
+-rw-r--r--   0 pennersr   (501) staff       (20)      480 2012-09-04 18:40:22.000000 django-allauth-0.9.0/allauth/templates/account/verification_sent.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      822 2012-09-04 18:36:10.000000 django-allauth-0.9.0/allauth/templates/account/verified_email_required.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      204 2012-08-24 19:15:21.000000 django-allauth-0.9.0/allauth/templates/account/snippets/already_logged_in.html
+-rw-r--r--   0 pennersr   (501) staff       (20)      316 2012-10-28 19:38:33.000000 django-allauth-0.9.0/allauth/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0 pennersr   (501) staff       (20)      115 2012-11-24 19:45:15.000000 django-allauth-0.9.0/allauth/templates/account/email/email_confirmation_subject.txt
+-rw-r--r--   0 pennersr   (501) staff       (20)      452 2012-06-27 15:49:59.000000 django-allauth-0.9.0/allauth/templates/account/email/password_reset_key_message.txt
+-rw-r--r--   0 pennersr   (501) staff       (20)      113 2012-11-24 19:44:52.000000 django-allauth-0.9.0/allauth/templates/account/email/password_reset_key_subject.txt
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:02.000000 django-allauth-0.9.0/allauth/socialaccount/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1548 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/adapter.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      617 2012-11-26 21:06:13.000000 django-allauth-0.9.0/allauth/socialaccount/admin.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1774 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/app_settings.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      138 2012-06-27 15:50:02.000000 django-allauth-0.9.0/allauth/socialaccount/context_processors.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1919 2013-01-29 19:23:05.000000 django-allauth-0.9.0/allauth/socialaccount/fields.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2242 2012-11-24 18:40:52.000000 django-allauth-0.9.0/allauth/socialaccount/forms.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     7571 2013-01-29 19:43:34.000000 django-allauth-0.9.0/allauth/socialaccount/helpers.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/
+-rw-r--r--   0 pennersr   (501) staff       (20)     7931 2013-01-29 19:23:05.000000 django-allauth-0.9.0/allauth/socialaccount/models.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/socialaccount/providers/
+-rw-r--r--   0 pennersr   (501) staff       (20)      337 2012-08-21 19:19:55.000000 django-allauth-0.9.0/allauth/socialaccount/signals.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/templatetags/
+-rw-r--r--   0 pennersr   (501) staff       (20)     2226 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      411 2013-01-25 20:53:01.000000 django-allauth-0.9.0/allauth/socialaccount/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2272 2012-11-24 18:40:48.000000 django-allauth-0.9.0/allauth/socialaccount/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:02.000000 django-allauth-0.9.0/allauth/socialaccount/templatetags/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2153 2012-12-15 22:46:57.000000 django-allauth-0.9.0/allauth/socialaccount/templatetags/socialaccount.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      174 2012-08-24 19:13:54.000000 django-allauth-0.9.0/allauth/socialaccount/templatetags/socialaccount_tags.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      935 2012-07-01 21:36:34.000000 django-allauth-0.9.0/allauth/socialaccount/providers/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1547 2012-06-27 15:50:04.000000 django-allauth-0.9.0/allauth/socialaccount/providers/base.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/github/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/google/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/linkedin/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/persona/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/stackexchange/
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:08.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/__init__.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1237 2012-10-10 20:09:00.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      164 2012-07-01 21:41:11.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1890 2013-01-29 19:23:04.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     7424 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/0001_initial.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     6058 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/0002_snowflake.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     8228 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/0003_tosocialaccount.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1925 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/0004_auto__del_twitteraccount__del_twitterapp.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:08.000000 django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:02.000000 django-allauth-0.9.0/allauth/socialaccount/providers/stackexchange/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/stackexchange/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      925 2012-12-22 19:52:22.000000 django-allauth-0.9.0/allauth/socialaccount/providers/stackexchange/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1517 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/stackexchange/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      178 2012-12-22 18:10:40.000000 django-allauth-0.9.0/allauth/socialaccount/providers/stackexchange/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1816 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/stackexchange/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-08-17 18:39:41.000000 django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      905 2012-08-17 19:30:00.000000 django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1342 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      172 2012-08-17 18:41:33.000000 django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1506 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-09-28 20:44:31.000000 django-allauth-0.9.0/allauth/socialaccount/providers/persona/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      999 2013-01-29 19:23:04.000000 django-allauth-0.9.0/allauth/socialaccount/providers/persona/provider.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/socialaccount/providers/persona/templates/
+-rw-r--r--   0 pennersr   (501) staff       (20)      164 2013-01-25 20:53:01.000000 django-allauth-0.9.0/allauth/socialaccount/providers/persona/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1543 2013-01-25 18:53:46.000000 django-allauth-0.9.0/allauth/socialaccount/providers/persona/views.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/persona/templates/persona/
+-rw-r--r--   0 pennersr   (501) staff       (20)      913 2012-09-28 22:13:34.000000 django-allauth-0.9.0/allauth/socialaccount/providers/persona/templates/persona/auth.html
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:05.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      286 2012-06-27 15:50:05.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/admin.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      205 2012-06-27 15:50:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/forms.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/migrations/
+-rw-r--r--   0 pennersr   (501) staff       (20)      643 2012-07-01 21:26:02.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2030 2012-07-01 21:25:35.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      497 2012-09-04 18:52:45.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      257 2013-01-25 20:53:01.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2138 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/utils.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     4183 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     7529 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/migrations/0001_initial.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     7741 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/migrations/0002_tosocialaccount.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1958 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/migrations/0003_auto__del_openidaccount.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/openid/migrations/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:09.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1932 2012-12-22 16:07:57.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/client.py
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      602 2012-07-01 20:45:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      478 2013-01-25 20:53:01.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     3015 2012-12-22 18:56:19.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:03.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     6958 2012-10-10 20:26:38.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth/client.py
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      599 2012-10-10 18:52:03.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      476 2013-01-25 20:53:01.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     3585 2012-12-22 18:56:20.000000 django-allauth-0.9.0/allauth/socialaccount/providers/oauth/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:07.000000 django-allauth-0.9.0/allauth/socialaccount/providers/linkedin/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/linkedin/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      657 2012-10-10 19:56:40.000000 django-allauth-0.9.0/allauth/socialaccount/providers/linkedin/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      166 2012-07-01 21:40:21.000000 django-allauth-0.9.0/allauth/socialaccount/providers/linkedin/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2740 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/linkedin/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:04.000000 django-allauth-0.9.0/allauth/socialaccount/providers/google/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/google/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1128 2012-07-01 21:41:40.000000 django-allauth-0.9.0/allauth/socialaccount/providers/google/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     3242 2013-01-29 19:49:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/google/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      163 2012-07-01 21:40:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/google/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2626 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/google/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:02.000000 django-allauth-0.9.0/allauth/socialaccount/providers/github/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/github/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      751 2012-07-01 21:41:59.000000 django-allauth-0.9.0/allauth/socialaccount/providers/github/provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1977 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/github/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      164 2012-07-01 21:40:04.000000 django-allauth-0.9.0/allauth/socialaccount/providers/github/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1487 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/github/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:10.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/__init__.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/data/
+-rw-r--r--   0 pennersr   (501) staff       (20)      116 2012-06-27 15:50:11.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/forms.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2333 2012-07-06 12:17:54.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/locale.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/
+-rw-r--r--   0 pennersr   (501) staff       (20)       27 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     3269 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/provider.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/templates/
+-rw-r--r--   0 pennersr   (501) staff       (20)      991 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      427 2013-01-25 20:53:02.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     3142 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/views.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:47.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/templates/facebook/
+-rw-r--r--   0 pennersr   (501) staff       (20)       81 2012-07-06 12:06:23.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/templates/facebook/channel.html
+-rw-r--r--   0 pennersr   (501) staff       (20)     1765 2012-12-22 21:00:05.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/templates/facebook/fbconnect.html
+-rw-r--r--   0 pennersr   (501) staff       (20)     7041 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/0001_initial.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     7101 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/0002_auto__add_facebookaccesstoken__add_unique_facebookaccesstoken_app_acco.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     8978 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/0003_tosocialaccount.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2774 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/0004_auto__del_facebookapp__del_facebookaccesstoken__del_unique_facebookacc.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:11.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)    12870 2012-07-06 12:06:23.000000 django-allauth-0.9.0/allauth/socialaccount/providers/facebook/data/FacebookLocales.xml
+-rw-r--r--   0 pennersr   (501) staff       (20)     4545 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/0001_initial.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     9426 2012-09-03 20:24:06.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/0002_genericmodels.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     6551 2012-12-27 17:40:22.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/0003_auto__add_unique_socialaccount_uid_provider.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     6641 2012-11-26 20:48:56.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/0004_add_sites.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     6338 2012-11-26 21:03:49.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/0005_set_sites.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     6229 2012-11-26 21:05:15.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/0006_auto__del_field_socialapp_site.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     6438 2012-12-22 18:51:03.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/0007_auto__add_field_socialapp_client_id.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     6323 2012-12-22 18:52:14.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/0008_client_id.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:50:13.000000 django-allauth-0.9.0/allauth/socialaccount/migrations/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-06-27 15:49:57.000000 django-allauth-0.9.0/allauth/account/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2724 2012-12-15 22:46:56.000000 django-allauth-0.9.0/allauth/account/adapter.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      710 2012-08-29 23:08:48.000000 django-allauth-0.9.0/allauth/account/admin.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     5445 2012-12-21 18:35:13.000000 django-allauth-0.9.0/allauth/account/app_settings.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1743 2012-10-29 20:55:53.000000 django-allauth-0.9.0/allauth/account/auth_backends.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      241 2012-09-04 18:32:43.000000 django-allauth-0.9.0/allauth/account/context_processors.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1625 2012-09-04 19:16:52.000000 django-allauth-0.9.0/allauth/account/decorators.py
+-rw-r--r--   0 pennersr   (501) staff       (20)    17634 2012-11-24 19:47:22.000000 django-allauth-0.9.0/allauth/account/forms.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/account/management/
+-rw-r--r--   0 pennersr   (501) staff       (20)     1547 2012-11-24 13:56:12.000000 django-allauth-0.9.0/allauth/account/managers.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     4166 2012-11-24 19:51:38.000000 django-allauth-0.9.0/allauth/account/models.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      824 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/account/signals.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/account/templatetags/
+-rw-r--r--   0 pennersr   (501) staff       (20)     4755 2012-12-21 18:42:11.000000 django-allauth-0.9.0/allauth/account/tests.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1213 2013-01-25 20:51:40.000000 django-allauth-0.9.0/allauth/account/urls.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     8003 2013-01-29 19:35:38.000000 django-allauth-0.9.0/allauth/account/utils.py
+-rw-r--r--   0 pennersr   (501) staff       (20)    15992 2013-01-25 18:47:13.000000 django-allauth-0.9.0/allauth/account/views.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        1 2012-06-27 15:49:56.000000 django-allauth-0.9.0/allauth/account/templatetags/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     1185 2012-06-27 15:49:56.000000 django-allauth-0.9.0/allauth/account/templatetags/account.py
+-rw-r--r--   0 pennersr   (501) staff       (20)      153 2012-08-24 19:11:48.000000 django-allauth-0.9.0/allauth/account/templatetags/account_tags.py
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-08-29 19:53:24.000000 django-allauth-0.9.0/allauth/account/management/__init__.py
+drwxr-xr-x   0 pennersr   (501) staff       (20)        0 2013-01-30 22:26:46.000000 django-allauth-0.9.0/allauth/account/management/commands/
+-rw-r--r--   0 pennersr   (501) staff       (20)        0 2012-08-29 19:53:27.000000 django-allauth-0.9.0/allauth/account/management/commands/__init__.py
+-rw-r--r--   0 pennersr   (501) staff       (20)     2571 2012-08-30 18:46:59.000000 django-allauth-0.9.0/allauth/account/management/commands/account_emailconfirmationmigration.py
```

### Comparing `django-allauth-0.8.3/LICENSE` & `django-allauth-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/PKG-INFO` & `django-allauth-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: django-allauth
-Version: 0.8.3
+Version: 0.9.0
 Summary: Integrated set of Django applications addressing authentication, registration, account management as well as 3rd party (social) account authentication.
 Home-page: http://github.com/pennersr/django-allauth
 Author: Raymond Penners
 Author-email: raymond.penners@intenct.nl
 License: UNKNOWN
 Description: ==========================
         Welcome to django-allauth!
@@ -13,17 +13,14 @@
         Integrated set of Django applications addressing authentication,
         registration, account management as well as 3rd party (social) account
         authentication.
         
         Rationale
         =========
         
-        Why?
-        ----
-        
         Most existing Django apps that address the problem of social
         authentication focus on just that. You typically need to integrate
         another app in order to support authentication via a local
         account. 
         
         This approach separates the worlds of local and social
         authentication. However, there are common scenarios to be dealt with
@@ -37,34 +34,14 @@
         local account registration app to your `INSTALLED_APPS` list.
         
         This is the reason this project got started -- to offer a fully
         integrated authentication app that allows for both local and social
         authentication, with flows that just work.
         
         
-        Why Not?
-        --------
-        
-        From the start the focus has been to deliver an integrated experience
-        and flows that just work, and to a lesser extent a completely
-        pluggable social authentication framework.
-        
-        Earlier versions of the project suffered from this, e.g. each provider
-        had its own implementation with its own social account model
-        definition. 
-        
-        Work is well underway to rectify this situation. These days, social
-        account models have been unified, and adding support for additional
-        OAuth/OAuth2 providers is child's play. All hardcodedness with respect
-        to providers has been removed.
-        
-        Ofcourse, there is always more that can be done. Do know that the
-        biggest hurdles to overcome the initial shortcomings have been
-        taken...
-        
         Overview
         ========
         
         Supported Flows
         ---------------
         
         - Signup of both local and social accounts
@@ -95,14 +72,16 @@
         
         - OpenId
         
         - Persona
         
         - SoundCloud (OAuth2)
         
+        - Stack Exchange (OAuth2)
+        
         - Twitter
         
         Note: OAuth/OAuth2 support is built using a common code base, making it easy to add support for additional OAuth/OAuth2 providers. More will follow soon...
         
          
         Features
         --------
@@ -166,14 +145,15 @@
                 'allauth.socialaccount.providers.facebook',
                 'allauth.socialaccount.providers.google',
                 'allauth.socialaccount.providers.github',
                 'allauth.socialaccount.providers.linkedin',
                 'allauth.socialaccount.providers.openid',
                 'allauth.socialaccount.providers.persona',
                 'allauth.socialaccount.providers.soundcloud',
+                'allauth.socialaccount.providers.stackexchange',
                 'allauth.socialaccount.providers.twitter',
                 ...
             )
         
         urls.py::
         
             urlpatterns = patterns('',
@@ -196,17 +176,18 @@
           Specifies the login method to use -- whether the user logs in by
           entering his username, e-mail address, or either one of both.
         
         ACCOUNT_EMAIL_CONFIRMATION_ANONYMOUS_REDIRECT_URL (=settings.LOGIN_URL)
           The URL to redirect to after a successful e-mail confirmation, in case no
           user is logged in.
         
-        ACCOUNT_EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL (=settings.LOGIN_REDIRECT_URL)
-          The URL to redirect to after a successful e-mail confirmation, in case of
-          an authenticated user.
+        ACCOUNT_EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL (=None)
+          The URL to redirect to after a successful e-mail confirmation, in
+          case of an authenticated user. Set to `None` to use
+          `settings.LOGIN_REDIRECT_URL`.
         
         ACCOUNT_EMAIL_CONFIRMATION_EXPIRE_DAYS (=3)
           Determines the expiration date of email confirmation mails (# of days).
         
         ACCOUNT_EMAIL_REQUIRED (=False)
           The user is required to hand over an e-mail address when signing up.
         
@@ -251,14 +232,18 @@
         
         ACCOUNT_PASSWORD_INPUT_RENDER_VALUE (=False)
           `render_value` parameter as passed to `PasswordInput` fields.
         
         ACCOUNT_PASSWORD_MIN_LENGTH (=6)
           An integer specifying the minimum password length.
         
+        SOCIALACCOUNT_ADAPTER (="allauth.socialaccount.adapter.DefaultSocialAccountAdapter")
+          Specifies the adapter class to use, allowing you to alter certain
+          default behaviour.
+        
         SOCIALACCOUNT_QUERY_EMAIL (=ACCOUNT_EMAIL_REQUIRED)
           Request e-mail address from 3rd party account provider? E.g. using
           OpenID AX, or the Facebook "email" permission.
         
         SOCIALACCOUNT_AUTO_SIGNUP (=True) 
           Attempt to bypass the signup form by using fields (e.g. username,
           email) retrieved from the social account provider. If a conflict
@@ -272,14 +257,24 @@
         SOCIALACCOUNT_PROVIDERS (= dict)
             Dictionary containing provider specific settings.
         
         
         Upgrading
         ---------
         
+        From 0.8.3
+        **********
+        
+        - `requests` is now a dependency (dropped `httplib2`).
+        
+        - Added a new column `SocialApp.client_id`. The value of `key` needs
+          to be moved to the new `client_id` column. The `key` column is
+          required for Stack Exchange. Migrations are in place to handle all
+          of this automatically.
+        
         From 0.8.2
         **********
         
         - The `ACCOUNT_EMAIL_VERIFICATION` setting is no longer a boolean
           based setting. Use a string value of "none", "optional" or
           "mandatory" instead.
         
@@ -436,15 +431,15 @@
         `LOCALE_FUNC` setting, which takes either a callable or a path to a callable.
         This callable must take exactly one argument, the request, and return `a
         valid Facebook locale <http://developers.facebook.com/docs/
         internationalization/>`_ as a string::
         
             SOCIALACCOUNT_PROVIDERS = \
                 { 'facebook':
-                    { 'LOCALE_FUNC': lambda request: return 'zh_CN'} }
+                    { 'LOCALE_FUNC': lambda request: 'zh_CN'} }
         
         Google
         ------
         
         The Google provider is OAuth2 based. Register your Google API client
         over at `https://code.google.com/apis/console/`. Make sure you list a
         redirect uri of the form
@@ -530,14 +525,33 @@
         SoundCloud
         ----------
         
         SoundCloud allows you to choose between OAuth1 and OAuth2.  Choose the
         latter. 
         
         
+        Stack Exchange
+        --------------
+        
+        Register your OAuth2 over at
+        `http://stackapps.com/apps/oauth/register`.  Do not enable "Client
+        Side Flow". For local development you can simply use "localhost" for
+        the OAuth domain.
+        
+        As for all providers, provider specific data is stored in
+        `SocialAccount.extra_data`. For Stack Exchange we need to choose what
+        data to store there by choosing the Stack Exchange site (e.g. Stack
+        Overflow, or Server Fault). This can be controlled by means of the
+        `SITE` setting::
+        
+            SOCIALACCOUNT_PROVIDERS = \
+                { 'stackexchange': 
+                    { 'SITE': 'stackoverflow' } }
+        
+        
         Signals
         =======
         
         The following signals are emitted:
         
         - `allauth.account.signals.user_logged_in`
         
@@ -601,14 +615,24 @@
         
             {% load socialaccount %}
         
             <a href="{% provider_login_url "openid" openid="https://www.google.com/accounts/o8/id" next="/success/url/" %}">Google</a>
             <a href="{% provider_login_url "twitter" %}">Twitter</a>
         
         
+        For easy access to the social accounts for a user::
+        
+            {% get_social_accounts user as accounts %}
+        
+        Then::
+        
+            {{accounts.twitter}} -- a list of connected Twitter accounts
+            {{accounts.twitter.0}} -- the first Twitter account
+            {% if accounts %} -- if there is at least one social account
+        
         Decorators
         ==========
         
         Verified E-mail Required
         ------------------------
         
         Even when email verification is not mandatory during signup, there
@@ -633,14 +657,15 @@
           address.
         
         
         
         Showcase
         ========
         
+        - http://www.highlightcam.com/
         - http://officecheese.com
         - http://www.mycareerstack.com
         - http://jug.gl
         - http://www.charityblossom.org/
         - http://www.superreceptionist.in
         - http://www.edithuddle.com
         - http://kwatsi.com
```

### Comparing `django-allauth-0.8.3/README.rst` & `django-allauth-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 Integrated set of Django applications addressing authentication,
 registration, account management as well as 3rd party (social) account
 authentication.
 
 Rationale
 =========
 
-Why?
-----
-
 Most existing Django apps that address the problem of social
 authentication focus on just that. You typically need to integrate
 another app in order to support authentication via a local
 account. 
 
 This approach separates the worlds of local and social
 authentication. However, there are common scenarios to be dealt with
@@ -29,34 +26,14 @@
 local account registration app to your `INSTALLED_APPS` list.
 
 This is the reason this project got started -- to offer a fully
 integrated authentication app that allows for both local and social
 authentication, with flows that just work.
 
 
-Why Not?
---------
-
-From the start the focus has been to deliver an integrated experience
-and flows that just work, and to a lesser extent a completely
-pluggable social authentication framework.
-
-Earlier versions of the project suffered from this, e.g. each provider
-had its own implementation with its own social account model
-definition. 
-
-Work is well underway to rectify this situation. These days, social
-account models have been unified, and adding support for additional
-OAuth/OAuth2 providers is child's play. All hardcodedness with respect
-to providers has been removed.
-
-Ofcourse, there is always more that can be done. Do know that the
-biggest hurdles to overcome the initial shortcomings have been
-taken...
-
 Overview
 ========
 
 Supported Flows
 ---------------
 
 - Signup of both local and social accounts
@@ -87,14 +64,16 @@
 
 - OpenId
 
 - Persona
 
 - SoundCloud (OAuth2)
 
+- Stack Exchange (OAuth2)
+
 - Twitter
 
 Note: OAuth/OAuth2 support is built using a common code base, making it easy to add support for additional OAuth/OAuth2 providers. More will follow soon...
 
  
 Features
 --------
@@ -158,14 +137,15 @@
         'allauth.socialaccount.providers.facebook',
         'allauth.socialaccount.providers.google',
         'allauth.socialaccount.providers.github',
         'allauth.socialaccount.providers.linkedin',
         'allauth.socialaccount.providers.openid',
         'allauth.socialaccount.providers.persona',
         'allauth.socialaccount.providers.soundcloud',
+        'allauth.socialaccount.providers.stackexchange',
         'allauth.socialaccount.providers.twitter',
         ...
     )
 
 urls.py::
 
     urlpatterns = patterns('',
@@ -188,17 +168,18 @@
   Specifies the login method to use -- whether the user logs in by
   entering his username, e-mail address, or either one of both.
 
 ACCOUNT_EMAIL_CONFIRMATION_ANONYMOUS_REDIRECT_URL (=settings.LOGIN_URL)
   The URL to redirect to after a successful e-mail confirmation, in case no
   user is logged in.
 
-ACCOUNT_EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL (=settings.LOGIN_REDIRECT_URL)
-  The URL to redirect to after a successful e-mail confirmation, in case of
-  an authenticated user.
+ACCOUNT_EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL (=None)
+  The URL to redirect to after a successful e-mail confirmation, in
+  case of an authenticated user. Set to `None` to use
+  `settings.LOGIN_REDIRECT_URL`.
 
 ACCOUNT_EMAIL_CONFIRMATION_EXPIRE_DAYS (=3)
   Determines the expiration date of email confirmation mails (# of days).
 
 ACCOUNT_EMAIL_REQUIRED (=False)
   The user is required to hand over an e-mail address when signing up.
 
@@ -243,14 +224,18 @@
 
 ACCOUNT_PASSWORD_INPUT_RENDER_VALUE (=False)
   `render_value` parameter as passed to `PasswordInput` fields.
 
 ACCOUNT_PASSWORD_MIN_LENGTH (=6)
   An integer specifying the minimum password length.
 
+SOCIALACCOUNT_ADAPTER (="allauth.socialaccount.adapter.DefaultSocialAccountAdapter")
+  Specifies the adapter class to use, allowing you to alter certain
+  default behaviour.
+
 SOCIALACCOUNT_QUERY_EMAIL (=ACCOUNT_EMAIL_REQUIRED)
   Request e-mail address from 3rd party account provider? E.g. using
   OpenID AX, or the Facebook "email" permission.
 
 SOCIALACCOUNT_AUTO_SIGNUP (=True) 
   Attempt to bypass the signup form by using fields (e.g. username,
   email) retrieved from the social account provider. If a conflict
@@ -264,14 +249,24 @@
 SOCIALACCOUNT_PROVIDERS (= dict)
     Dictionary containing provider specific settings.
 
 
 Upgrading
 ---------
 
+From 0.8.3
+**********
+
+- `requests` is now a dependency (dropped `httplib2`).
+
+- Added a new column `SocialApp.client_id`. The value of `key` needs
+  to be moved to the new `client_id` column. The `key` column is
+  required for Stack Exchange. Migrations are in place to handle all
+  of this automatically.
+
 From 0.8.2
 **********
 
 - The `ACCOUNT_EMAIL_VERIFICATION` setting is no longer a boolean
   based setting. Use a string value of "none", "optional" or
   "mandatory" instead.
 
@@ -428,15 +423,15 @@
 `LOCALE_FUNC` setting, which takes either a callable or a path to a callable.
 This callable must take exactly one argument, the request, and return `a
 valid Facebook locale <http://developers.facebook.com/docs/
 internationalization/>`_ as a string::
 
     SOCIALACCOUNT_PROVIDERS = \
         { 'facebook':
-            { 'LOCALE_FUNC': lambda request: return 'zh_CN'} }
+            { 'LOCALE_FUNC': lambda request: 'zh_CN'} }
 
 Google
 ------
 
 The Google provider is OAuth2 based. Register your Google API client
 over at `https://code.google.com/apis/console/`. Make sure you list a
 redirect uri of the form
@@ -522,14 +517,33 @@
 SoundCloud
 ----------
 
 SoundCloud allows you to choose between OAuth1 and OAuth2.  Choose the
 latter. 
 
 
+Stack Exchange
+--------------
+
+Register your OAuth2 over at
+`http://stackapps.com/apps/oauth/register`.  Do not enable "Client
+Side Flow". For local development you can simply use "localhost" for
+the OAuth domain.
+
+As for all providers, provider specific data is stored in
+`SocialAccount.extra_data`. For Stack Exchange we need to choose what
+data to store there by choosing the Stack Exchange site (e.g. Stack
+Overflow, or Server Fault). This can be controlled by means of the
+`SITE` setting::
+
+    SOCIALACCOUNT_PROVIDERS = \
+        { 'stackexchange': 
+            { 'SITE': 'stackoverflow' } }
+
+
 Signals
 =======
 
 The following signals are emitted:
 
 - `allauth.account.signals.user_logged_in`
 
@@ -593,14 +607,24 @@
 
     {% load socialaccount %}
 
     <a href="{% provider_login_url "openid" openid="https://www.google.com/accounts/o8/id" next="/success/url/" %}">Google</a>
     <a href="{% provider_login_url "twitter" %}">Twitter</a>
 
 
+For easy access to the social accounts for a user::
+
+    {% get_social_accounts user as accounts %}
+
+Then::
+
+    {{accounts.twitter}} -- a list of connected Twitter accounts
+    {{accounts.twitter.0}} -- the first Twitter account
+    {% if accounts %} -- if there is at least one social account
+
 Decorators
 ==========
 
 Verified E-mail Required
 ------------------------
 
 Even when email verification is not mandatory during signup, there
@@ -625,14 +649,15 @@
   address.
 
 
 
 Showcase
 ========
 
+- http://www.highlightcam.com/
 - http://officecheese.com
 - http://www.mycareerstack.com
 - http://jug.gl
 - http://www.charityblossom.org/
 - http://www.superreceptionist.in
 - http://www.edithuddle.com
 - http://kwatsi.com
```

### Comparing `django-allauth-0.8.3/setup.py` & `django-allauth-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,34 +94,37 @@
 
 excluded_directories = standard_exclude_directories
 
 package_data = find_package_data(exclude_directories=excluded_directories)
 
 METADATA = dict(
     name='django-allauth',
-    version='0.8.3',
+    version='0.9.0',
     author='Raymond Penners',
     author_email='raymond.penners@intenct.nl',
     description='Integrated set of Django applications addressing authentication, registration, account management as well as 3rd party (social) account authentication.',
     long_description=open('README.rst').read(),
     url='http://github.com/pennersr/django-allauth',
     keywords='django auth account social openid twitter facebook oauth registration',
     install_requires=['django',
                       'oauth2',
-                      'python-openid'],
+                      'python-openid',
+                      'requests'],
     include_package_data=True,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Environment :: Web Environment',
         'Topic :: Internet',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Framework :: Django',
     ],
     packages=find_packages(exclude=['example']),
-    package_data=package_data
+    package_data=package_data,
+    tests_require=['django-setuptest', 'argparse'],
+    test_suite='setuptest.setuptest.SetupTestSuite'
 )
 
 if __name__ == '__main__':
     setup(**METADATA)
```

### Comparing `django-allauth-0.8.3/django_allauth.egg-info/PKG-INFO` & `django-allauth-0.9.0/django_allauth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: django-allauth
-Version: 0.8.3
+Version: 0.9.0
 Summary: Integrated set of Django applications addressing authentication, registration, account management as well as 3rd party (social) account authentication.
 Home-page: http://github.com/pennersr/django-allauth
 Author: Raymond Penners
 Author-email: raymond.penners@intenct.nl
 License: UNKNOWN
 Description: ==========================
         Welcome to django-allauth!
@@ -13,17 +13,14 @@
         Integrated set of Django applications addressing authentication,
         registration, account management as well as 3rd party (social) account
         authentication.
         
         Rationale
         =========
         
-        Why?
-        ----
-        
         Most existing Django apps that address the problem of social
         authentication focus on just that. You typically need to integrate
         another app in order to support authentication via a local
         account. 
         
         This approach separates the worlds of local and social
         authentication. However, there are common scenarios to be dealt with
@@ -37,34 +34,14 @@
         local account registration app to your `INSTALLED_APPS` list.
         
         This is the reason this project got started -- to offer a fully
         integrated authentication app that allows for both local and social
         authentication, with flows that just work.
         
         
-        Why Not?
-        --------
-        
-        From the start the focus has been to deliver an integrated experience
-        and flows that just work, and to a lesser extent a completely
-        pluggable social authentication framework.
-        
-        Earlier versions of the project suffered from this, e.g. each provider
-        had its own implementation with its own social account model
-        definition. 
-        
-        Work is well underway to rectify this situation. These days, social
-        account models have been unified, and adding support for additional
-        OAuth/OAuth2 providers is child's play. All hardcodedness with respect
-        to providers has been removed.
-        
-        Ofcourse, there is always more that can be done. Do know that the
-        biggest hurdles to overcome the initial shortcomings have been
-        taken...
-        
         Overview
         ========
         
         Supported Flows
         ---------------
         
         - Signup of both local and social accounts
@@ -95,14 +72,16 @@
         
         - OpenId
         
         - Persona
         
         - SoundCloud (OAuth2)
         
+        - Stack Exchange (OAuth2)
+        
         - Twitter
         
         Note: OAuth/OAuth2 support is built using a common code base, making it easy to add support for additional OAuth/OAuth2 providers. More will follow soon...
         
          
         Features
         --------
@@ -166,14 +145,15 @@
                 'allauth.socialaccount.providers.facebook',
                 'allauth.socialaccount.providers.google',
                 'allauth.socialaccount.providers.github',
                 'allauth.socialaccount.providers.linkedin',
                 'allauth.socialaccount.providers.openid',
                 'allauth.socialaccount.providers.persona',
                 'allauth.socialaccount.providers.soundcloud',
+                'allauth.socialaccount.providers.stackexchange',
                 'allauth.socialaccount.providers.twitter',
                 ...
             )
         
         urls.py::
         
             urlpatterns = patterns('',
@@ -196,17 +176,18 @@
           Specifies the login method to use -- whether the user logs in by
           entering his username, e-mail address, or either one of both.
         
         ACCOUNT_EMAIL_CONFIRMATION_ANONYMOUS_REDIRECT_URL (=settings.LOGIN_URL)
           The URL to redirect to after a successful e-mail confirmation, in case no
           user is logged in.
         
-        ACCOUNT_EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL (=settings.LOGIN_REDIRECT_URL)
-          The URL to redirect to after a successful e-mail confirmation, in case of
-          an authenticated user.
+        ACCOUNT_EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL (=None)
+          The URL to redirect to after a successful e-mail confirmation, in
+          case of an authenticated user. Set to `None` to use
+          `settings.LOGIN_REDIRECT_URL`.
         
         ACCOUNT_EMAIL_CONFIRMATION_EXPIRE_DAYS (=3)
           Determines the expiration date of email confirmation mails (# of days).
         
         ACCOUNT_EMAIL_REQUIRED (=False)
           The user is required to hand over an e-mail address when signing up.
         
@@ -251,14 +232,18 @@
         
         ACCOUNT_PASSWORD_INPUT_RENDER_VALUE (=False)
           `render_value` parameter as passed to `PasswordInput` fields.
         
         ACCOUNT_PASSWORD_MIN_LENGTH (=6)
           An integer specifying the minimum password length.
         
+        SOCIALACCOUNT_ADAPTER (="allauth.socialaccount.adapter.DefaultSocialAccountAdapter")
+          Specifies the adapter class to use, allowing you to alter certain
+          default behaviour.
+        
         SOCIALACCOUNT_QUERY_EMAIL (=ACCOUNT_EMAIL_REQUIRED)
           Request e-mail address from 3rd party account provider? E.g. using
           OpenID AX, or the Facebook "email" permission.
         
         SOCIALACCOUNT_AUTO_SIGNUP (=True) 
           Attempt to bypass the signup form by using fields (e.g. username,
           email) retrieved from the social account provider. If a conflict
@@ -272,14 +257,24 @@
         SOCIALACCOUNT_PROVIDERS (= dict)
             Dictionary containing provider specific settings.
         
         
         Upgrading
         ---------
         
+        From 0.8.3
+        **********
+        
+        - `requests` is now a dependency (dropped `httplib2`).
+        
+        - Added a new column `SocialApp.client_id`. The value of `key` needs
+          to be moved to the new `client_id` column. The `key` column is
+          required for Stack Exchange. Migrations are in place to handle all
+          of this automatically.
+        
         From 0.8.2
         **********
         
         - The `ACCOUNT_EMAIL_VERIFICATION` setting is no longer a boolean
           based setting. Use a string value of "none", "optional" or
           "mandatory" instead.
         
@@ -436,15 +431,15 @@
         `LOCALE_FUNC` setting, which takes either a callable or a path to a callable.
         This callable must take exactly one argument, the request, and return `a
         valid Facebook locale <http://developers.facebook.com/docs/
         internationalization/>`_ as a string::
         
             SOCIALACCOUNT_PROVIDERS = \
                 { 'facebook':
-                    { 'LOCALE_FUNC': lambda request: return 'zh_CN'} }
+                    { 'LOCALE_FUNC': lambda request: 'zh_CN'} }
         
         Google
         ------
         
         The Google provider is OAuth2 based. Register your Google API client
         over at `https://code.google.com/apis/console/`. Make sure you list a
         redirect uri of the form
@@ -530,14 +525,33 @@
         SoundCloud
         ----------
         
         SoundCloud allows you to choose between OAuth1 and OAuth2.  Choose the
         latter. 
         
         
+        Stack Exchange
+        --------------
+        
+        Register your OAuth2 over at
+        `http://stackapps.com/apps/oauth/register`.  Do not enable "Client
+        Side Flow". For local development you can simply use "localhost" for
+        the OAuth domain.
+        
+        As for all providers, provider specific data is stored in
+        `SocialAccount.extra_data`. For Stack Exchange we need to choose what
+        data to store there by choosing the Stack Exchange site (e.g. Stack
+        Overflow, or Server Fault). This can be controlled by means of the
+        `SITE` setting::
+        
+            SOCIALACCOUNT_PROVIDERS = \
+                { 'stackexchange': 
+                    { 'SITE': 'stackoverflow' } }
+        
+        
         Signals
         =======
         
         The following signals are emitted:
         
         - `allauth.account.signals.user_logged_in`
         
@@ -601,14 +615,24 @@
         
             {% load socialaccount %}
         
             <a href="{% provider_login_url "openid" openid="https://www.google.com/accounts/o8/id" next="/success/url/" %}">Google</a>
             <a href="{% provider_login_url "twitter" %}">Twitter</a>
         
         
+        For easy access to the social accounts for a user::
+        
+            {% get_social_accounts user as accounts %}
+        
+        Then::
+        
+            {{accounts.twitter}} -- a list of connected Twitter accounts
+            {{accounts.twitter.0}} -- the first Twitter account
+            {% if accounts %} -- if there is at least one social account
+        
         Decorators
         ==========
         
         Verified E-mail Required
         ------------------------
         
         Even when email verification is not mandatory during signup, there
@@ -633,14 +657,15 @@
           address.
         
         
         
         Showcase
         ========
         
+        - http://www.highlightcam.com/
         - http://officecheese.com
         - http://www.mycareerstack.com
         - http://jug.gl
         - http://www.charityblossom.org/
         - http://www.superreceptionist.in
         - http://www.edithuddle.com
         - http://kwatsi.com
```

### Comparing `django-allauth-0.8.3/django_allauth.egg-info/SOURCES.txt` & `django-allauth-0.9.0/django_allauth.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 allauth/__init__.py
 allauth/app_settings.py
+allauth/exceptions.py
 allauth/models.py
 allauth/tests.py
 allauth/urls.py
 allauth/utils.py
 allauth/account/__init__.py
 allauth/account/adapter.py
 allauth/account/admin.py
@@ -27,58 +28,63 @@
 allauth/account/management/__init__.py
 allauth/account/management/commands/__init__.py
 allauth/account/management/commands/account_emailconfirmationmigration.py
 allauth/account/templatetags/__init__.py
 allauth/account/templatetags/account.py
 allauth/account/templatetags/account_tags.py
 allauth/socialaccount/__init__.py
+allauth/socialaccount/adapter.py
 allauth/socialaccount/admin.py
 allauth/socialaccount/app_settings.py
 allauth/socialaccount/context_processors.py
 allauth/socialaccount/fields.py
 allauth/socialaccount/forms.py
 allauth/socialaccount/helpers.py
 allauth/socialaccount/models.py
-allauth/socialaccount/requests.py
 allauth/socialaccount/signals.py
 allauth/socialaccount/tests.py
 allauth/socialaccount/urls.py
 allauth/socialaccount/views.py
 allauth/socialaccount/migrations/0001_initial.py
 allauth/socialaccount/migrations/0002_genericmodels.py
 allauth/socialaccount/migrations/0003_auto__add_unique_socialaccount_uid_provider.py
 allauth/socialaccount/migrations/0004_add_sites.py
 allauth/socialaccount/migrations/0005_set_sites.py
 allauth/socialaccount/migrations/0006_auto__del_field_socialapp_site.py
+allauth/socialaccount/migrations/0007_auto__add_field_socialapp_client_id.py
+allauth/socialaccount/migrations/0008_client_id.py
 allauth/socialaccount/migrations/__init__.py
 allauth/socialaccount/providers/__init__.py
 allauth/socialaccount/providers/base.py
 allauth/socialaccount/providers/facebook/__init__.py
 allauth/socialaccount/providers/facebook/forms.py
 allauth/socialaccount/providers/facebook/locale.py
 allauth/socialaccount/providers/facebook/models.py
 allauth/socialaccount/providers/facebook/provider.py
+allauth/socialaccount/providers/facebook/tests.py
 allauth/socialaccount/providers/facebook/urls.py
 allauth/socialaccount/providers/facebook/views.py
 allauth/socialaccount/providers/facebook/data/FacebookLocales.xml
 allauth/socialaccount/providers/facebook/migrations/0001_initial.py
 allauth/socialaccount/providers/facebook/migrations/0002_auto__add_facebookaccesstoken__add_unique_facebookaccesstoken_app_acco.py
 allauth/socialaccount/providers/facebook/migrations/0003_tosocialaccount.py
 allauth/socialaccount/providers/facebook/migrations/0004_auto__del_facebookapp__del_facebookaccesstoken__del_unique_facebookacc.py
 allauth/socialaccount/providers/facebook/migrations/__init__.py
 allauth/socialaccount/providers/facebook/templates/facebook/channel.html
 allauth/socialaccount/providers/facebook/templates/facebook/fbconnect.html
 allauth/socialaccount/providers/github/__init__.py
 allauth/socialaccount/providers/github/models.py
 allauth/socialaccount/providers/github/provider.py
+allauth/socialaccount/providers/github/tests.py
 allauth/socialaccount/providers/github/urls.py
 allauth/socialaccount/providers/github/views.py
 allauth/socialaccount/providers/google/__init__.py
 allauth/socialaccount/providers/google/models.py
 allauth/socialaccount/providers/google/provider.py
+allauth/socialaccount/providers/google/tests.py
 allauth/socialaccount/providers/google/urls.py
 allauth/socialaccount/providers/google/views.py
 allauth/socialaccount/providers/linkedin/__init__.py
 allauth/socialaccount/providers/linkedin/models.py
 allauth/socialaccount/providers/linkedin/provider.py
 allauth/socialaccount/providers/linkedin/urls.py
 allauth/socialaccount/providers/linkedin/views.py
@@ -111,16 +117,23 @@
 allauth/socialaccount/providers/persona/provider.py
 allauth/socialaccount/providers/persona/urls.py
 allauth/socialaccount/providers/persona/views.py
 allauth/socialaccount/providers/persona/templates/persona/auth.html
 allauth/socialaccount/providers/soundcloud/__init__.py
 allauth/socialaccount/providers/soundcloud/models.py
 allauth/socialaccount/providers/soundcloud/provider.py
+allauth/socialaccount/providers/soundcloud/tests.py
 allauth/socialaccount/providers/soundcloud/urls.py
 allauth/socialaccount/providers/soundcloud/views.py
+allauth/socialaccount/providers/stackexchange/__init__.py
+allauth/socialaccount/providers/stackexchange/models.py
+allauth/socialaccount/providers/stackexchange/provider.py
+allauth/socialaccount/providers/stackexchange/tests.py
+allauth/socialaccount/providers/stackexchange/urls.py
+allauth/socialaccount/providers/stackexchange/views.py
 allauth/socialaccount/providers/twitter/__init__.py
 allauth/socialaccount/providers/twitter/models.py
 allauth/socialaccount/providers/twitter/provider.py
 allauth/socialaccount/providers/twitter/urls.py
 allauth/socialaccount/providers/twitter/views.py
 allauth/socialaccount/providers/twitter/migrations/0001_initial.py
 allauth/socialaccount/providers/twitter/migrations/0002_snowflake.py
@@ -162,12 +175,8 @@
 allauth/templates/socialaccount/signup.html
 allauth/templates/socialaccount/snippets/login_extra.html
 allauth/templates/socialaccount/snippets/provider_list.html
 django_allauth.egg-info/PKG-INFO
 django_allauth.egg-info/SOURCES.txt
 django_allauth.egg-info/dependency_links.txt
 django_allauth.egg-info/requires.txt
-django_allauth.egg-info/top_level.txt
-example/__init__.py
-example/manage.py
-example/settings.py
-example/urls.py
+django_allauth.egg-info/top_level.txt
```

### Comparing `django-allauth-0.8.3/allauth/app_settings.py` & `django-allauth-0.9.0/allauth/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/urls.py` & `django-allauth-0.9.0/allauth/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.conf.urls.defaults import url, patterns, include
+from django.conf.urls import url, patterns, include
 from django.utils import importlib
 
 from allauth.socialaccount import providers
 
 import app_settings
 
 urlpatterns = patterns('', url('^', include('allauth.account.urls')))
```

### Comparing `django-allauth-0.8.3/allauth/utils.py` & `django-allauth-0.9.0/allauth/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,25 @@
 from django.utils.http import urlencode
 from django.contrib.auth import REDIRECT_FIELD_NAME
 from django.utils import importlib
 
 import app_settings
 
 def get_login_redirect_url(request, 
-                           fallback=app_settings.LOGIN_REDIRECT_URL):
+                           fallback=True):
     """
     Returns a url to redirect to after the login
+    
+    TODO: 
+    - Cleanup, check overlap with account.utils.get_default_redirect
+    - Move to allauth.account
     """
+    if fallback and type(fallback) == bool:
+        from account.adapter import get_adapter
+        fallback = get_adapter().get_login_redirect_url(request)
     url = request.REQUEST.get(REDIRECT_FIELD_NAME) or fallback
     return url
 
 
 def passthrough_login_redirect_url(request, url):
     assert url.find("?") < 0  # TODO: Handle this case properly
     next = get_login_redirect_url(request, fallback=None)
```

### Comparing `django-allauth-0.8.3/allauth/templates/base.html` & `django-allauth-0.9.0/allauth/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/socialaccount/connections.html` & `django-allauth-0.9.0/allauth/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/socialaccount/signup.html` & `django-allauth-0.9.0/allauth/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/socialaccount/snippets/provider_list.html` & `django-allauth-0.9.0/allauth/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/account/email.html` & `django-allauth-0.9.0/allauth/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/account/email_confirm.html` & `django-allauth-0.9.0/allauth/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/account/login.html` & `django-allauth-0.9.0/allauth/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/account/password_reset.html` & `django-allauth-0.9.0/allauth/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/account/password_reset_from_key.html` & `django-allauth-0.9.0/allauth/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/account/signup.html` & `django-allauth-0.9.0/allauth/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/templates/account/verified_email_required.html` & `django-allauth-0.9.0/allauth/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/admin.py` & `django-allauth-0.9.0/allauth/socialaccount/admin.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/fields.py` & `django-allauth-0.9.0/allauth/socialaccount/fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Courtesy of django-social-auth
+import json
 
 from django.core.exceptions import ValidationError
 from django.db import models
-from django.utils import simplejson
 from django.utils.encoding import smart_unicode
 
 
 class JSONField(models.TextField):
     """Simple JSON field that stores python structures as JSON strings
     on database.
     """
@@ -17,34 +17,34 @@
         Convert the input JSON value into python structures, raises
         django.core.exceptions.ValidationError if the data can't be converted.
         """
         if self.blank and not value:
             return None
         if isinstance(value, basestring):
             try:
-                return simplejson.loads(value)
+                return json.loads(value)
             except Exception, e:
                 raise ValidationError(str(e))
         else:
             return value
 
     def validate(self, value, model_instance):
         """Check value is a valid JSON string, raise ValidationError on
         error."""
         if isinstance(value, basestring):
             super(JSONField, self).validate(value, model_instance)
             try:
-                simplejson.loads(value)
+                json.loads(value)
             except Exception, e:
                 raise ValidationError(str(e))
 
     def get_prep_value(self, value):
         """Convert value to JSON string before save"""
         try:
-            return simplejson.dumps(value)
+            return json.dumps(value)
         except Exception, e:
             raise ValidationError(str(e))
 
     def value_to_string(self, obj):
         """Return value from object converted to string properly"""
         return smart_unicode(self.get_prep_value(self._get_val_from_obj(obj)))
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/forms.py` & `django-allauth-0.9.0/allauth/socialaccount/forms.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/helpers.py` & `django-allauth-0.9.0/allauth/socialaccount/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 from django.template.defaultfilters import slugify
 
 from allauth.utils import (generate_unique_username, email_address_exists,
                            get_user_model)
 from allauth.account.utils import send_email_confirmation, \
     perform_login, complete_signup
 from allauth.account import app_settings as account_settings
+from allauth.exceptions import ImmediateHttpResponse
 
 from models import SocialLogin
 import app_settings
 import signals
+from adapter import get_adapter
 
 User = get_user_model()
 
 def _process_signup(request, sociallogin):
     # If email is specified, check for duplicate and if so, no auto signup.
     auto_signup = app_settings.AUTO_SIGNUP
     email = sociallogin.account.user.email
@@ -70,30 +72,34 @@
     if not user.is_active:
         ret = render_to_response(
             'socialaccount/account_inactive.html',
             {},
             context_instance=RequestContext(request))
     else:
         ret = perform_login(request, user, 
-                            redirect_url=sociallogin.get_redirect_url())
+                            redirect_url=sociallogin.get_redirect_url(request))
     return ret
 
 
 def render_authentication_error(request, extra_context={}):
     return render_to_response(
         "socialaccount/authentication_error.html",
         extra_context, context_instance=RequestContext(request))
 
 
 def complete_social_login(request, sociallogin):
     assert not sociallogin.is_existing
     sociallogin.lookup()
-    signals.pre_social_login.send(sender=SocialLogin,
-                                  request=request, 
-                                  sociallogin=sociallogin)
+    try:
+        get_adapter().pre_social_login(request, sociallogin)
+        signals.pre_social_login.send(sender=SocialLogin,
+                                      request=request, 
+                                      sociallogin=sociallogin)
+    except ImmediateHttpResponse, e:
+        return e.response
     if request.user.is_authenticated():
         if sociallogin.is_existing:
             # Existing social account, existing user
             if sociallogin.account.user != request.user:
                 # Social account of other user. Simply logging in may
                 # not be correct in the case that the user was
                 # attempting to hook up another social account to his
@@ -104,15 +110,16 @@
                 pass
             ret = _login_social_account(request, sociallogin)
         else:
             # New social account
             sociallogin.account.user = request.user
             sociallogin.save()
             default_next = reverse('socialaccount_connections')
-            next = sociallogin.get_redirect_url(fallback=default_next)
+            next = sociallogin.get_redirect_url(request,
+                                                fallback=default_next)
             messages.add_message(request, messages.INFO, 
                                  _('The social account has been connected'))
             return HttpResponseRedirect(next)
     else:
         if sociallogin.is_existing:
             # Login existing user
             ret = _login_social_account(request, sociallogin)
@@ -169,15 +176,16 @@
 
 
 def complete_social_signup(request, sociallogin):
     if app_settings.AVATAR_SUPPORT:
         _copy_avatar(request, sociallogin.account.user, sociallogin.account)
     return complete_signup(request, 
                            sociallogin.account.user, 
-                           sociallogin.get_redirect_url())
+                           sociallogin.get_redirect_url(request),
+                           signal_kwargs={'sociallogin': sociallogin})
 
 
 # TODO: Factor out callable importing functionality
 # See: account.utils.user_display
 def import_path(path):
     modname, _, attr = path.rpartition('.')
     m = __import__(modname, fromlist=[attr])
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/models.py` & `django-allauth-0.9.0/allauth/socialaccount/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+import json
+
 from django.db import models
 from django.contrib.auth import authenticate
 from django.contrib.sites.models import Site
-from django.utils import simplejson
 
 import allauth.app_settings
-from allauth.utils import get_login_redirect_url
+from allauth.account import app_settings as account_settings
+from allauth.utils import (get_login_redirect_url,
+                           valid_email_or_none)
+from allauth.account.adapter import get_adapter
+from allauth.account.models import EmailAddress
 
 import providers
 from fields import JSONField
 
 
 class SocialAppManager(models.Manager):
     def get_current(self, provider):
@@ -19,22 +24,27 @@
 
 class SocialApp(models.Model):
     objects = SocialAppManager()
 
     provider = models.CharField(max_length=30, 
                                 choices=providers.registry.as_choices())
     name = models.CharField(max_length=40)
+    client_id = models.CharField(max_length=100,
+                                 help_text='App ID, or consumer key')
     key = models.CharField(max_length=100,
-                           help_text='App ID, or consumer key')
+                           blank=True,
+                           help_text='Key (Stack Exchange only)')
     secret = models.CharField(max_length=100,
-                              help_text='API secret, or consumer secret')
+                              help_text='API secret, client secret, or'
+                              ' consumer secret')
     # Most apps can be used across multiple domains, therefore we use
     # a ManyToManyField. Note that Facebook requires an app per domain
     # (unless the domains share a common base name).
-    sites = models.ManyToManyField(Site)
+    # blank=True allows for disabling apps without removing them
+    sites = models.ManyToManyField(Site, blank=True)
 
     def __unicode__(self):
         return self.name
 
 class SocialAccount(models.Model):
     user = models.ForeignKey(allauth.app_settings.USER_MODEL)
     provider = models.CharField(max_length=30,
@@ -112,32 +122,47 @@
     handshake.
 
     `state` (`dict`): The state to be preserved during the
     authentication handshake. Note that this state may end up in the
     url (e.g. OAuth2 `state` parameter) -- do not put any secrets in
     there. It currently only contains the url to redirect to after
     login.
+
+    `email_addresses` (list of `EmailAddress`): Optional list of
+    e-mail addresses retrieved from the provider.
     """
 
-    def __init__(self, account, token=None):
+    def __init__(self, account, token=None, email_addresses=[]):
         if token:
             assert token.account is None or token.account == account
             token.account = account
         self.token = token
         self.account = account
+        self.email_addresses = email_addresses
         self.state = {}
 
     def save(self):
         user = self.account.user
         user.save()
         self.account.user = user
         self.account.save()
         if self.token:
             self.token.account = self.account
             self.token.save()
+        for email_address in self.email_addresses:
+            # Pick up only valid ones...
+            email = valid_email_or_none(email_address.email)
+            if not email:
+                continue
+            # ... and non-conflicting ones...
+            if (account_settings.UNIQUE_EMAIL 
+                and EmailAddress.objects.filter(email__iexact=email).exists()):
+                continue
+            email_address.user = user
+            email_address.save()
 
     @property
     def is_existing(self):
         """
         Account is temporary, not yet backed by a database record.
         """
         return self.account.pk
@@ -166,34 +191,35 @@
                     self.token = t
                 except SocialToken.DoesNotExist:
                     self.token.account = a
                     self.token.save()
         except SocialAccount.DoesNotExist:
             pass
     
-    def get_redirect_url(self, 
-                         fallback=allauth.app_settings.LOGIN_REDIRECT_URL):
+    def get_redirect_url(self, request, fallback=True):
+        if fallback and type(fallback) == bool:
+            fallback = get_adapter().get_login_redirect_url(request)
         url = self.state.get('next') or fallback
         return url
             
     @classmethod
     def state_from_request(cls, request):
         state = {}
         next = get_login_redirect_url(request, fallback=None)
         if next:
             state['next'] = next
         return state
 
     @classmethod
     def marshall_state(cls, request):
         state = cls.state_from_request(request)
-        return simplejson.dumps(state)
+        return json.dumps(state)
     
     @classmethod
     def unmarshall_state(cls, state_string):
         if state_string:
-            state = simplejson.loads(state_string)
+            state = json.loads(state_string)
         else:
             state = {}
         return state
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/tests.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/google/tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-import urlparse
-import warnings
+from django.test.utils import override_settings
 
-from django.test import TestCase
-from django.core.urlresolvers import reverse
-from django.contrib.sites.models import Site
+from allauth.socialaccount.tests import create_oauth2_tests
+from allauth.account import app_settings as account_settings
+from allauth.account.models import EmailConfirmation, EmailAddress
+from allauth.socialaccount.providers import registry
+from allauth.tests import MockedResponse
+from allauth.account.signals import user_signed_up
 
-import providers
-from allauth.socialaccount import requests
+from provider import GoogleProvider
 
-from providers.oauth2.provider import OAuth2Provider
+class GoogleTests(create_oauth2_tests(registry.by_id(GoogleProvider.id))):
 
-from models import SocialApp
-
-
-mocked_oauth_responses = {
-    'google': requests.Response(200, """
+    def get_mocked_response(self, verified_email=True):
+        return MockedResponse(200, """
 {"family_name": "Penners", "name": "Raymond Penners", 
                "picture": "https://lh5.googleusercontent.com/-GOFYGBVOdBQ/AAAAAAAAAAI/AAAAAAAAAGM/WzRfPkv4xbo/photo.jpg", 
                "locale": "nl", "gender": "male", 
                "email": "raymond.penners@gmail.com", 
                "link": "https://plus.google.com/108204268033311374519", 
                "given_name": "Raymond", "id": "108204268033311374519", 
-                "verified_email": true}
-""")
-}
-
-def create_oauth2_tests(provider):
-    def setUp(self):
-        self.app = SocialApp.objects.create(site=Site.objects.get_current(),
-                                            provider=self.provider.id,
-                                            name='oauth2 test',
-                                            key='123',
-                                            secret='abc')
-
-    def test_login(self):
-        resp = self.client.get(reverse(self.provider.id + '_login'))
-        p = urlparse.urlparse(resp['location'])
-        q = urlparse.parse_qs(p.query)
-        complete_url = reverse(self.provider.id+'_callback')
-        self.assertGreater(q['redirect_uri'][0]
-                           .find(complete_url), 0)
-        resp_mock = mocked_oauth_responses.get(self.provider.id)
-        if not resp_mock:
-            warnings.warn("Cannot test provider %s, no oauth mock" 
-                          % self.provider.id)
-            return
-        requests.mock_next_request \
-            (requests.Response(200,
-                               '{"access_token":"testac"}',
-                               {'content-type': 
-                                'application/json'}))
-        requests.mock_next_request(resp_mock)
-        resp = self.client.get(complete_url,
-                               { 'code': 'test' })
-        self.assertRedirects(resp, reverse('socialaccount_signup'))
-
-    
-    impl = { 'setUp': setUp,
-             'test_login': test_login }
-    class_name = 'OAuth2Tests_'+provider.id
-    Class = type(class_name, (TestCase,), impl)
-    globals()[class_name] = Class
-    Class.provider = provider
-
-for provider in providers.registry.get_list():
-    if isinstance(provider,OAuth2Provider):
-        create_oauth2_tests(provider)
+                "verified_email": %s }
+""" % (repr(verified_email).lower()))
+
+    @override_settings(SOCIALACCOUNT_AUTO_SIGNUP=True,
+                       ACCOUNT_SIGNUP_FORM_CLASS=None,
+                       ACCOUNT_EMAIL_VERIFICATION
+                       =account_settings.EmailVerificationMethod.MANDATORY)
+    def test_email_verified(self):
+        test_email = 'raymond.penners@gmail.com'
+        self.login(self.get_mocked_response(verified_email=True))
+        EmailAddress.objects \
+            .get(email=test_email,
+                 verified=True)
+        self.assertFalse(EmailConfirmation.objects \
+                             .filter(email_address__email=test_email) \
+                             .exists())
+
+    @override_settings(SOCIALACCOUNT_AUTO_SIGNUP=True,
+                       ACCOUNT_SIGNUP_FORM_CLASS=None,
+                       ACCOUNT_EMAIL_VERIFICATION
+                       =account_settings.EmailVerificationMethod.MANDATORY)
+    def test_user_signed_up_signal(self):
+        sent_signals = []
+
+        def on_signed_up(sender, request, user, **kwargs):
+            sociallogin = kwargs['sociallogin']
+            self.assertEquals(sociallogin.account.provider,
+                              GoogleProvider.id)
+            self.assertEquals(sociallogin.account.user,
+                              user)
+            sent_signals.append(sender)
+
+        user_signed_up.connect(on_signed_up)
+        self.login(self.get_mocked_response(verified_email=True))
+        self.assertTrue(len(sent_signals) > 0)
+
+    @override_settings(SOCIALACCOUNT_AUTO_SIGNUP=True,
+                       ACCOUNT_SIGNUP_FORM_CLASS=None,
+                       ACCOUNT_EMAIL_VERIFICATION
+                       =account_settings.EmailVerificationMethod.MANDATORY)
+    def test_email_unverified(self):
+        test_email = 'raymond.penners@gmail.com'
+        self.login(self.get_mocked_response(verified_email=False))
+        email_address = EmailAddress.objects \
+            .get(email=test_email)
+        self.assertFalse(email_address.verified)
+        self.assertTrue(EmailConfirmation.objects \
+                            .filter(email_address__email=test_email) \
+                            .exists())
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/views.py` & `django-allauth-0.9.0/allauth/socialaccount/views.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/__init__.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/base.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/base.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/twitter/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/twitter/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/twitter/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/twitter/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from django.utils import simplejson
+import json
 
 from allauth.socialaccount.providers.oauth.client import OAuth
 from allauth.socialaccount.providers.oauth.views import (OAuthAdapter,
                                                          OAuthLoginView,
                                                          OAuthCallbackView)
 from allauth.socialaccount.models import SocialLogin, SocialAccount
-from allauth.utils import get_user_model
+from allauth.socialaccount.adapter import get_adapter
 
 from provider import TwitterProvider
 
-User = get_user_model()
-
 class TwitterAPI(OAuth):
     """
     Verifying twitter credentials
     """
     url = 'https://api.twitter.com/1.1/account/verify_credentials.json'
 
     def get_user_info(self):
-        user = simplejson.loads(self.query(self.url))
+        user = json.loads(self.query(self.url))
         return user
 
 
 class TwitterOAuthAdapter(OAuthAdapter):
     provider_id = TwitterProvider.id
     request_token_url = 'https://api.twitter.com/oauth/request_token'
     access_token_url = 'https://api.twitter.com/oauth/access_token'
     # Issue #42 -- this one authenticates over and over again...
     # authorize_url = 'https://api.twitter.com/oauth/authorize'
     authorize_url = 'https://api.twitter.com/oauth/authenticate'
 
     def complete_login(self, request, app, token):
-        client = TwitterAPI(request, app.key, app.secret,
+        client = TwitterAPI(request, app.client_id, app.secret,
                             self.request_token_url)
         extra_data = client.get_user_info()
         uid = extra_data['id']
-        user = User(username=extra_data['screen_name'])
+        user = get_adapter() \
+            .populate_new_user(username=extra_data.get('screen_name'),
+                               name=extra_data.get('name'))
         account = SocialAccount(user=user,
                                 uid=uid,
                                 provider=TwitterProvider.id,
                                 extra_data=extra_data)
         return SocialLogin(account)
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/0001_initial.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/0002_snowflake.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/0002_snowflake.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/0003_tosocialaccount.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/0003_tosocialaccount.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/twitter/migrations/0004_auto__del_twitteraccount__del_twitterapp.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/twitter/migrations/0004_auto__del_twitteraccount__del_twitterapp.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/soundcloud/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/soundcloud/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/soundcloud/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,32 @@
+import requests
+
 from allauth.socialaccount.providers.oauth2.views import (OAuth2Adapter,
                                                           OAuth2LoginView,
                                                           OAuth2CallbackView)
-from allauth.socialaccount import requests
 from allauth.socialaccount.models import SocialAccount, SocialLogin
-from allauth.utils import get_user_model
+from allauth.socialaccount.adapter import get_adapter
 
 from provider import SoundCloudProvider
 
-User = get_user_model()
-
 class SoundCloudOAuth2Adapter(OAuth2Adapter):
     provider_id = SoundCloudProvider.id
     access_token_url = 'https://api.soundcloud.com/oauth2/token'
     authorize_url = 'https://soundcloud.com/connect'
     profile_url = 'https://api.soundcloud.com/me.json'
 
     def complete_login(self, request, app, token):
         resp = requests.get(self.profile_url,
                             params={ 'oauth_token': token.token })
-        extra_data = resp.json
+        extra_data = resp.json()
         uid = str(extra_data['id'])
-        name_parts = extra_data.get('full_name', '').split(' ', 1)
-        if len(name_parts) == 2:
-            first_name, last_name = name_parts
-        else:
-            first_name, last_name = name_parts[0], ''
-        user_kwargs = {'first_name': first_name, 
-                       'last_name': last_name}
-        user = User(username=extra_data.get('username', ''),
-                    email=extra_data.get('email', ''),
-                    **user_kwargs)
+        user = get_adapter() \
+            .populate_new_user(name=extra_data.get('full_name'),
+                               username=extra_data.get('username'),
+                               email=extra_data.get('email'))
         account = SocialAccount(user=user,
                                 uid=uid,
                                 extra_data=extra_data,
                                 provider=self.provider_id)
         return SocialLogin(account)
 
 oauth2_login = OAuth2LoginView.adapter_view(SoundCloudOAuth2Adapter)
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/persona/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/persona/provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import json
+
 from django.template.loader import render_to_string
 from django.template import RequestContext
-from django.utils import simplejson
 
 from allauth.socialaccount import providers
 from allauth.socialaccount.providers.base import ProviderAccount, Provider
 
 
 class PersonaAccount(ProviderAccount):
     def __unicode__(self):
@@ -15,15 +16,15 @@
     name = 'Persona'
     package = 'allauth.socialaccount.providers.persona'
     account_class = PersonaAccount
 
     def media_js(self, request):
         settings = self.get_settings()
         request_parameters = settings.get('REQUEST_PARAMETERS', {})
-        ctx = { 'request_parameters': simplejson.dumps(request_parameters) }
+        ctx = { 'request_parameters': json.dumps(request_parameters) }
         return render_to_string('persona/auth.html',
                                 ctx,
                                 RequestContext(request))
 
     def get_login_url(self, request, **kwargs):
         return 'javascript:allauth.persona.login()'
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/persona/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/persona/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+import requests
+
 from allauth.socialaccount.helpers import complete_social_login
 from allauth.socialaccount.helpers import render_authentication_error
-from allauth.socialaccount import requests
 from allauth.socialaccount.models import SocialAccount, SocialLogin
-from allauth.utils import get_user_model
+from allauth.socialaccount.adapter import get_adapter
 
 from provider import PersonaProvider
 
-User = get_user_model()
-
 def persona_login(request):
     assertion = request.POST.get('assertion', '')
     audience = request.build_absolute_uri('/') 
     resp = requests.post('https://verifier.login.persona.org/verify',
                          { 'assertion': assertion,
                            'audience': audience })
-    if resp.json['status'] != 'okay':
+    if resp.json()['status'] != 'okay':
         return render_authentication_error(request)
-    email = resp.json['email']
-    user = User(email=email)
-    extra_data = resp.json
+    email = resp.json()['email']
+    user = get_adapter() \
+        .populate_new_user(email=email)
+    extra_data = resp.json()
     account = SocialAccount(uid=email,
                             provider=PersonaProvider.id,
                             extra_data=extra_data,
                             user=user)
     # TBD: Persona e-mail addresses are verified, so we could check if
     # a matching local user account already exists with an identical
     # verified e-mail address and short-circuit the social login. Then
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/persona/templates/persona/auth.html` & `django-allauth-0.9.0/allauth/socialaccount/providers/persona/templates/persona/auth.html`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/openid/models.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/openid/models.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/openid/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/openid/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/openid/utils.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/openid/utils.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/openid/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/openid/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 from openid.extensions.sreg import SRegRequest, SRegResponse
 from openid.extensions.ax import FetchRequest, FetchResponse, AttrInfo
 
 from allauth.socialaccount.app_settings import QUERY_EMAIL
 from allauth.socialaccount.models import SocialAccount, SocialLogin
 from allauth.socialaccount.helpers import render_authentication_error
 from allauth.socialaccount.helpers import complete_social_login
-from allauth.utils import valid_email_or_none, get_user_model
+from allauth.socialaccount.adapter import get_adapter
+from allauth.utils import valid_email_or_none
 
 from utils import DBOpenIDStore
 from forms import LoginForm
 from provider import OpenIDProvider
 
-User = get_user_model()
-
 class AXAttribute:
     CONTACT_EMAIL = 'http://axschema.org/contact/email'
 
 
 class SRegField:
     EMAIL = 'email'
 
@@ -90,15 +89,16 @@
 @csrf_exempt
 def callback(request):
     client = _openid_consumer(request)
     response = client.complete(
         dict(request.REQUEST.items()),
         request.build_absolute_uri(request.path))
     if response.status == consumer.SUCCESS:
-        user = User(email=_get_email_from_response(response))
+        user = get_adapter() \
+            .populate_new_user(email=_get_email_from_response(response))
         account = SocialAccount(uid=response.identity_url,
                                 provider=OpenIDProvider.id,
                                 user=user,
                                 extra_data={})
         login = SocialLogin(account)
         login.state = SocialLogin.unmarshall_state(request.REQUEST.get('state'))
         ret = complete_social_login(request, login)
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/openid/migrations/0001_initial.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/openid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/openid/migrations/0002_tosocialaccount.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/openid/migrations/0002_tosocialaccount.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/openid/migrations/0003_auto__del_openidaccount.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/openid/migrations/0003_auto__del_openidaccount.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/client.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import urllib
 import urlparse
+import requests
 
-from allauth.socialaccount import requests
 
 class OAuth2Error(Exception):
     pass
 
 
 class OAuth2Client(object):
 
@@ -43,15 +43,15 @@
                   'code': code}
         url = self.access_token_url
         # TODO: Proper exception handling
         resp = requests.post(url, params)
         access_token = None
         if resp.status_code == 200:
             if resp.headers['content-type'].split(';')[0] == 'application/json':
-                data = resp.json
+                data = resp.json()
             else:
                 data = dict(urlparse.parse_qsl(resp.content))
             access_token = data.get('access_token')
         if not access_token:
             raise OAuth2Error('Error retrieving access token: %s' 
                               % resp.content)
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/oauth2/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/oauth2/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             self.adapter = adapter()
             return self.dispatch(request, *args, **kwargs)
         return view
 
     def get_client(self, request, app):
         callback_url = reverse(self.adapter.provider_id + "_callback")
         callback_url = request.build_absolute_uri(callback_url)
-        client = OAuth2Client(self.request, app.key, app.secret,
+        client = OAuth2Client(self.request, app.client_id, app.secret,
                               self.adapter.authorize_url,
                               self.adapter.access_token_url,
                               callback_url,
                               self.adapter.get_provider().get_scope())
         return client
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/oauth/client.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/oauth/client.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/oauth/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/oauth/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/oauth/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/oauth/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def _get_client(self, request, callback_url):
         provider = self.adapter.get_provider()
         app = provider.get_app(request)
         scope = ' '.join(provider.get_scope())
         parameters = {}
         if scope:
             parameters['scope'] = scope
-        client = OAuthClient(request, app.key, app.secret,
+        client = OAuthClient(request, app.client_id, app.secret,
                              self.adapter.request_token_url,
                              self.adapter.access_token_url,
                              self.adapter.authorize_url,
                              callback_url,
                              parameters=parameters)
         return client
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/linkedin/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/linkedin/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/linkedin/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/linkedin/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 from xml.parsers.expat import ExpatError
 
 from allauth.socialaccount.providers.oauth.client import OAuth
 from allauth.socialaccount.providers.oauth.views import (OAuthAdapter,
                                                          OAuthLoginView,
                                                          OAuthCallbackView)
 from allauth.socialaccount.models import SocialAccount, SocialLogin
-from allauth.utils import valid_email_or_none, get_user_model
+from allauth.socialaccount.adapter import get_adapter
 
 from provider import LinkedInProvider
 
-User = get_user_model()
-
 class LinkedInAPI(OAuth):
     url = 'https://api.linkedin.com/v1/people/~'
     fields = ['id', 'first-name', 'last-name', 'email-address']
 
     def get_user_info(self):
         url = self.url + ':(%s)' % ','.join(self.fields)
         raw_xml = self.query(url)
@@ -47,24 +45,23 @@
 class LinkedInOAuthAdapter(OAuthAdapter):
     provider_id = LinkedInProvider.id
     request_token_url = 'https://api.linkedin.com/uas/oauth/requestToken'
     access_token_url = 'https://api.linkedin.com/uas/oauth/accessToken'
     authorize_url = 'https://www.linkedin.com/uas/oauth/authenticate'
 
     def complete_login(self, request, app, token):
-        client = LinkedInAPI(request, app.key, app.secret,
+        client = LinkedInAPI(request, app.client_id, app.secret,
                              self.request_token_url)
         extra_data = client.get_user_info()
         uid = extra_data['id']
-        email = valid_email_or_none(extra_data.get('email-address', ''))
-        user = User(first_name=extra_data.get('first-name', ''),
-                    last_name=extra_data.get('last-name', ''),
-                    email=email)
+        user = get_adapter() \
+            .populate_new_user(email=extra_data.get('email-address'),
+                               first_name=extra_data.get('first-name'),
+                               last_name=extra_data.get('last-name'))
         account = SocialAccount(user=user,
                                 provider=self.provider_id,
                                 extra_data=extra_data,
                                 uid=uid)
         return SocialLogin(account)
 
 oauth_login = OAuthLoginView.adapter_view(LinkedInOAuthAdapter)
 oauth_callback = OAuthCallbackView.adapter_view(LinkedInOAuthAdapter)
-
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/google/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/google/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/google/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/google/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,55 @@
+import requests
+
+from allauth.account.models import EmailAddress
 from allauth.socialaccount.providers.oauth2.views import (OAuth2Adapter,
                                                           OAuth2LoginView,
                                                           OAuth2CallbackView)
 
-from allauth.socialaccount import requests
 from allauth.socialaccount.models import SocialLogin, SocialAccount
+from allauth.socialaccount.adapter import get_adapter
 from allauth.utils import get_user_model
 
 from provider import GoogleProvider
 
-User = get_user_model()
-
 class GoogleOAuth2Adapter(OAuth2Adapter):
     provider_id = GoogleProvider.id
     access_token_url = 'https://accounts.google.com/o/oauth2/token'
     authorize_url = 'https://accounts.google.com/o/oauth2/auth'
     profile_url = 'https://www.googleapis.com/oauth2/v1/userinfo'
 
     def complete_login(self, request, app, token):
         resp = requests.get(self.profile_url,
-                            { 'access_token': token.token,
-                              'alt': 'json' })
-        extra_data = resp.json
+                            params={ 'access_token': token.token,
+                                     'alt': 'json' })
+        extra_data = resp.json()
         # extra_data is something of the form:
         # 
         # {u'family_name': u'Penners', u'name': u'Raymond Penners', 
         #  u'picture': u'https://lh5.googleusercontent.com/-GOFYGBVOdBQ/AAAAAAAAAAI/AAAAAAAAAGM/WzRfPkv4xbo/photo.jpg', 
         #  u'locale': u'nl', u'gender': u'male', 
         #  u'email': u'raymond.penners@gmail.com', 
         #  u'link': u'https://plus.google.com/108204268033311374519', 
         #  u'given_name': u'Raymond', u'id': u'108204268033311374519', 
         #  u'verified_email': True}
         #
         # TODO: We could use verified_email to bypass allauth email verification
         uid = str(extra_data['id'])
-        user = User(email=extra_data.get('email', ''),
-                    last_name=extra_data.get('family_name', ''),
-                    first_name=extra_data.get('given_name', ''))
+        user = get_adapter() \
+            .populate_new_user(email=extra_data.get('email'),
+                               last_name=extra_data.get('family_name'),
+                               first_name=extra_data.get('given_name'))
+        email_addresses = []
+        if user.email and extra_data.get('verified_email'):
+            email_addresses.append(EmailAddress(email=user.email,
+                                                verified=True,
+                                                primary=True))
         account = SocialAccount(extra_data=extra_data,
                                 uid=uid,
                                 provider=self.provider_id,
                                 user=user)
-        return SocialLogin(account)
+        return SocialLogin(account,
+                           email_addresses=email_addresses)
 
 oauth2_login = OAuth2LoginView.adapter_view(GoogleOAuth2Adapter)
 oauth2_callback = OAuth2CallbackView.adapter_view(GoogleOAuth2Adapter)
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/github/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/github/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/github/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/stackexchange/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+import requests
+
 from allauth.socialaccount.providers.oauth2.views import (OAuth2Adapter,
                                                           OAuth2LoginView,
                                                           OAuth2CallbackView)
-from allauth.socialaccount import requests
 from allauth.socialaccount.models import SocialAccount, SocialLogin
-from allauth.utils import get_user_model
-
-from provider import GitHubProvider
+from allauth.socialaccount.providers import registry
+from allauth.socialaccount.adapter import get_adapter
 
-User = get_user_model()
+from provider import StackExchangeProvider
 
-class GitHubOAuth2Adapter(OAuth2Adapter):
-    provider_id = GitHubProvider.id
-    access_token_url = 'https://github.com/login/oauth/access_token'
-    authorize_url = 'https://github.com/login/oauth/authorize'
-    profile_url = 'https://api.github.com/user'
+class StackExchangeOAuth2Adapter(OAuth2Adapter):
+    provider_id = StackExchangeProvider.id
+    access_token_url = 'https://stackexchange.com/oauth/access_token'
+    authorize_url = 'https://stackexchange.com/oauth'
+    profile_url = 'https://api.stackexchange.com/2.1/me'
 
     def complete_login(self, request, app, token):
+        provider = registry.by_id(app.provider)
+        site = provider.get_site()
         resp = requests.get(self.profile_url,
-                            params={ 'access_token': token.token })
-        extra_data = resp.json
-        uid = str(extra_data['id'])
-        user = User(username=extra_data.get('login', ''),
-                    email=extra_data.get('email', ''),
-                    first_name=extra_data.get('name', ''))
+                            params={ 'access_token': token.token,
+                                     'key': app.key,
+                                     'site': site })
+        extra_data = resp.json()['items'][0]
+        # `user_id` varies if you use the same account for
+        # e.g. StackOverflow and ServerFault. Therefore, we pick
+        # `account_id`.
+        uid = str(extra_data['account_id'])
+        user = get_adapter() \
+            .populate_new_user(username=extra_data.get('display_name'))
         account = SocialAccount(user=user,
                                 uid=uid,
                                 extra_data=extra_data,
                                 provider=self.provider_id)
         return SocialLogin(account)
 
 
-oauth2_login = OAuth2LoginView.adapter_view(GitHubOAuth2Adapter)
-oauth2_callback = OAuth2CallbackView.adapter_view(GitHubOAuth2Adapter)
+oauth2_login = OAuth2LoginView.adapter_view(StackExchangeOAuth2Adapter)
+oauth2_callback = OAuth2CallbackView.adapter_view(StackExchangeOAuth2Adapter)
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/locale.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/locale.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/provider.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/provider.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/views.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 from django.utils.cache import patch_response_headers
 from django.shortcuts import render
 
+import requests
+
 from allauth.socialaccount.models import SocialAccount, SocialLogin, SocialToken
 from allauth.socialaccount.helpers import complete_social_login
 from allauth.socialaccount.helpers import render_authentication_error
+from allauth.socialaccount.adapter import get_adapter
 from allauth.socialaccount import providers
 from allauth.socialaccount.providers.oauth2.views import (OAuth2Adapter,
                                                           OAuth2LoginView,
                                                           OAuth2CallbackView)
-from allauth.socialaccount import requests
 
 from forms import FacebookConnectForm
 from provider import FacebookProvider
 
-from allauth.utils import valid_email_or_none, get_user_model
-
-User = get_user_model()
-
 def fb_complete_login(app, token):
     resp = requests.get('https://graph.facebook.com/me',
                         params={ 'access_token': token.token })
-    extra_data = resp.json
-    email = valid_email_or_none(extra_data.get('email'))
+    extra_data = resp.json()
     uid = extra_data['id']
-    user = User(email=email)
-    # some facebook accounts don't have this data
-    for k in ['username', 'first_name', 'last_name']:
-        v = extra_data.get(k)
-        if v:
-            setattr(user, k, v)
+    user = get_adapter() \
+        .populate_new_user(email=extra_data.get('email'),
+                           username=extra_data.get('username'),
+                           first_name=extra_data.get('first_name'),
+                           last_name=extra_data.get('last_name'))
     account = SocialAccount(uid=uid,
                             provider=FacebookProvider.id,
                             extra_data=extra_data,
                             user=user)
     return SocialLogin(account)
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/templates/facebook/fbconnect.html` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/templates/facebook/fbconnect.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load url from future %}
 <div id="fb-root"></div>
 <script>
   window.FB_login = function() {};
   window.fbAsyncInit = function() {
     FB.init({
-      appId      : '{{facebook_app.key}}',
+      appId      : '{{facebook_app.client_id}}',
       channelUrl : '{{facebook_channel_url}}',
       status     : true,
       cookie     : true,
       oauth      : true,
       xfbml      : true
     });
     window.FB_login = function(nextUrl) {
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/0001_initial.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/0002_auto__add_facebookaccesstoken__add_unique_facebookaccesstoken_app_acco.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/0002_auto__add_facebookaccesstoken__add_unique_facebookaccesstoken_app_acco.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/0003_tosocialaccount.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/0003_tosocialaccount.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/migrations/0004_auto__del_facebookapp__del_facebookaccesstoken__del_unique_facebookacc.py` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/migrations/0004_auto__del_facebookapp__del_facebookaccesstoken__del_unique_facebookacc.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/providers/facebook/data/FacebookLocales.xml` & `django-allauth-0.9.0/allauth/socialaccount/providers/facebook/data/FacebookLocales.xml`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/migrations/0001_initial.py` & `django-allauth-0.9.0/allauth/socialaccount/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/migrations/0002_genericmodels.py` & `django-allauth-0.9.0/allauth/socialaccount/migrations/0002_genericmodels.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/migrations/0003_auto__add_unique_socialaccount_uid_provider.py` & `django-allauth-0.9.0/allauth/socialaccount/migrations/0003_auto__add_unique_socialaccount_uid_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # encoding: utf-8
 from south.db import db
 from south.v2 import SchemaMigration
 from django.conf import settings
 
 class Migration(SchemaMigration):
-    depends_on = ()
+    depends_on = []
     if 'facebook' in settings.INSTALLED_APPS:
         depends_on.append(('facebook', '0003_tosocialaccount'),)
     if 'twitter' in settings.INSTALLED_APPS:
         depends_on.append(('twitter', '0003_tosocialaccount'),)
     if 'openid' in settings.INSTALLED_APPS:
         depends_on.append(('openid', '0002_tosocialaccount'),)
```

### Comparing `django-allauth-0.8.3/allauth/socialaccount/migrations/0004_add_sites.py` & `django-allauth-0.9.0/allauth/socialaccount/migrations/0004_add_sites.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/migrations/0005_set_sites.py` & `django-allauth-0.9.0/allauth/socialaccount/migrations/0005_set_sites.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/socialaccount/migrations/0006_auto__del_field_socialapp_site.py` & `django-allauth-0.9.0/allauth/socialaccount/migrations/0006_auto__del_field_socialapp_site.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/account/adapter.py` & `django-allauth-0.9.0/allauth/account/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,10 +41,31 @@
         body = render_to_string('{0}_message.txt'.format(template_prefix),
                                 context).strip()
         # remove superfluous line breaks
         subject = " ".join(subject.splitlines()).strip()
         subject = self.format_email_subject(subject)
         send_mail(subject, body, settings.DEFAULT_FROM_EMAIL, [email])
 
+    def get_login_redirect_url(self, request):
+        """
+        Returns the default URL to redirect to after logging in.  Note
+        that URLs passed explicitly (e.g. by passing along a `next`
+        GET parameter) take precedence over the value returned here.
+        """
+        return settings.LOGIN_REDIRECT_URL
+
+    def get_email_confirmation_redirect_url(self, request):
+        """
+        The URL to return to after successful e-mail confirmation.
+        """
+        if request.user.is_authenticated():
+            if app_settings.EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL:
+                return  \
+                    app_settings.EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL
+            else:
+                return self.get_login_redirect_url(request)
+        else:
+            return app_settings.EMAIL_CONFIRMATION_ANONYMOUS_REDIRECT_URL
+
 def get_adapter():
     return import_attribute(app_settings.ADAPTER)()
```

### Comparing `django-allauth-0.8.3/allauth/account/admin.py` & `django-allauth-0.9.0/allauth/account/admin.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/account/auth_backends.py` & `django-allauth-0.9.0/allauth/account/auth_backends.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/account/decorators.py` & `django-allauth-0.9.0/allauth/account/decorators.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/account/forms.py` & `django-allauth-0.9.0/allauth/account/forms.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/account/managers.py` & `django-allauth-0.9.0/allauth/account/managers.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/account/models.py` & `django-allauth-0.9.0/allauth/account/models.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/account/signals.py` & `django-allauth-0.9.0/allauth/account/signals.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 
 email_confirmed = Signal(providing_args=["email_address"])
 email_confirmation_sent = Signal(providing_args=["confirmation"])
 
 email_changed = Signal(providing_args=["request", "user",
                             "from_email_address", "to_email_address"])
 email_added = Signal(providing_args=["request", "user", "email_address"])
+email_removed = Signal(providing_args=["request", "user", "email_address"])
```

### Comparing `django-allauth-0.8.3/allauth/account/tests.py` & `django-allauth-0.9.0/allauth/account/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from datetime import timedelta
-try:
-    from django.utils.timezone import now
-except ImportError:
-    from datetime import datetime
-    now = datetime.now
 
+from django.utils.timezone import now
+from django.test.utils import override_settings
 from django.test import TestCase
 from django.conf import settings
 from django.core.urlresolvers import reverse
 from django.test.client import Client
 from django.core import mail
 from django.contrib.sites.models import Site
 from django.test.client import RequestFactory
 
 from allauth.account.models import EmailAddress, EmailConfirmation
 from allauth.utils import get_user_model
 
-from app_settings import AuthenticationMethod, EmailVerificationMethod
 import app_settings
 
+from adapter import get_adapter
+
 User = get_user_model()
 
+@override_settings \
+    (ACCOUNT_EMAIL_VERIFICATION=app_settings.EmailVerificationMethod.MANDATORY,
+     ACCOUNT_AUTHENTICATION_METHOD=app_settings.AuthenticationMethod.USERNAME,
+     ACCOUNT_SIGNUP_FORM_CLASS=None,
+     ACCOUNT_EMAIL_SUBJECT_PREFIX=None,
+     ACCOUNT_ADAPTER='allauth.account.adapter.DefaultAccountAdapter',
+     ACCOUNT_USERNAME_REQUIRED=True)
 class AccountTests(TestCase):
     def setUp(self):
-        self.OLD_EMAIL_VERIFICATION = app_settings.EMAIL_VERIFICATION
-        self.OLD_AUTHENTICATION_METHOD = app_settings.AUTHENTICATION_METHOD
-        self.OLD_SIGNUP_FORM_CLASS = app_settings.SIGNUP_FORM_CLASS
-        self.OLD_USERNAME_REQUIRED = app_settings.USERNAME_REQUIRED
-        app_settings.EMAIL_VERIFICATION = EmailVerificationMethod.MANDATORY
-        app_settings.AUTHENTICATION_METHOD = AuthenticationMethod.USERNAME
-        app_settings.SIGNUP_FORM_CLASS = None
-        app_settings.USERNAME_REQUIRED = True
-
         if 'allauth.socialaccount' in settings.INSTALLED_APPS:
             # Otherwise ImproperlyConfigured exceptions may occur
             from ..socialaccount.models import SocialApp
-            SocialApp.objects.create(name='testfb',
-                                     provider='facebook',
-                                     site=Site.objects.get_current())
+            sa = SocialApp.objects.create(name='testfb',
+                                          provider='facebook')
+            sa.sites.add(Site.objects.get_current())
 
 
     def test_signup_email_verified_externally(self):
         request = RequestFactory().post(reverse('account_signup'),
                       { 'username': 'johndoe',
                         'email': 'john@doe.com',
                         'password1': 'johndoe',
@@ -51,15 +47,16 @@
         from django.contrib.sessions.middleware import SessionMiddleware
         SessionMiddleware().process_request(request)
         MessageMiddleware().process_request(request)
         request.session['account_email_verified'] ='john@doe.com'
         from views import signup
         resp = signup(request)
         self.assertEquals(resp.status_code, 302)
-        self.assertEquals(resp['location'], settings.LOGIN_REDIRECT_URL)
+        self.assertEquals(resp['location'], 
+                          get_adapter().get_login_redirect_url(request))
         self.assertEquals(len(mail.outbox), 0)
 
 
     def test_email_verification_mandatory(self):
         c = Client()
         # Signup
         resp = c.post(reverse('account_signup'),
@@ -100,27 +97,15 @@
                           'http://testserver'+settings.LOGIN_REDIRECT_URL)
 
 
 
 
 
     def test_email_escaping(self):
-        """
-        Test is only valid if emailconfirmation is listed after
-        allauth in INSTALLED_APPS
-        """
         site = Site.objects.get_current()
         site.name = '<enc&"test>'
         site.save()
         u = User.objects.create(username='test',
                                 email='foo@bar.com')
         request = RequestFactory().get('/')
         EmailAddress.objects.add_email(request, u, u.email, confirm=True)
         self.assertTrue(mail.outbox[0].subject[1:].startswith(site.name))
-                        
-
-    def tearDown(self):
-        app_settings.EMAIL_VERIFICATION = self.OLD_EMAIL_VERIFICATION
-        app_settings.AUTHENTICATION_METHOD = self.OLD_AUTHENTICATION_METHOD
-        app_settings.SIGNUP_FORM_CLASS = self.OLD_SIGNUP_FORM_CLASS
-        app_settings.USERNAME_REQUIRED = self.OLD_USERNAME_REQUIRED
-
```

### Comparing `django-allauth-0.8.3/allauth/account/urls.py` & `django-allauth-0.9.0/allauth/account/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.conf.urls.defaults import patterns, url
+from django.conf.urls import patterns, url
 
 import views
 
 urlpatterns = patterns("",
     url(r"^email/$", views.email, name="account_email"),
     url(r"^signup/$", views.signup, name="account_signup"),
     url(r"^login/$", views.login, name="account_login"),
```

### Comparing `django-allauth-0.8.3/allauth/account/utils.py` & `django-allauth-0.9.0/allauth/account/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     - a REQUEST value, GET or POST, named "next" by default.
     - LOGIN_REDIRECT_URL - the URL in the setting
     - LOGIN_REDIRECT_URLNAME - the name of a URLconf entry in the settings
     """
     if login_redirect_urlname:
         default_redirect_to = reverse(login_redirect_urlname)
     else:
-        default_redirect_to = settings.LOGIN_REDIRECT_URL
+        default_redirect_to = get_adapter().get_login_redirect_url(request)
     redirect_to = request.REQUEST.get(redirect_field_name)
     if not redirect_to:
         # try the session if available
         if hasattr(request, "session"):
             redirect_to = request.session.get(session_key_value)
     # light security check -- make sure redirect_to isn't garabage.
     if not redirect_to or "://" in redirect_to or " " in redirect_to:
@@ -104,18 +104,19 @@
                          ugettext("Successfully signed in as %(user)s.") % { "user": user_display(user) } )
 
     if not redirect_url:
         redirect_url = get_default_redirect(request)
     return HttpResponseRedirect(redirect_url)
 
 
-def complete_signup(request, user, success_url):
+def complete_signup(request, user, success_url, signal_kwargs={}):
     signals.user_signed_up.send(sender=user.__class__, 
                                 request=request, 
-                                user=user)
+                                user=user,
+                                **signal_kwargs)
     return perform_login(request, user, redirect_url=success_url)
 
 
 def setup_user_email(request, user):
     """
     Creates proper EmailAddress for the user that was just signed
     up. Only sets up, doesn't do any other handling such as sending
```

### Comparing `django-allauth-0.8.3/allauth/account/views.py` & `django-allauth-0.9.0/allauth/account/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from utils import get_default_redirect, complete_signup
 from forms import AddEmailForm, ChangePasswordForm
 from forms import LoginForm, ResetPasswordKeyForm
 from forms import ResetPasswordForm, SetPasswordForm, SignupForm
 from utils import sync_user_email_addresses
 from models import EmailAddress, EmailConfirmation
 
-import app_settings
 import signals
+from adapter import get_adapter
 
 User = get_user_model()
 
 def login(request, **kwargs):
     form_class = kwargs.pop("form_class", LoginForm)
     template_name = kwargs.pop("template_name", "account/login.html")
     success_url = kwargs.pop("success_url", None)
@@ -90,18 +90,18 @@
         "email_confirmed": {
             "level": messages.SUCCESS,
             "text": _("You have confirmed %(email)s.")
         }
     }
     
     def get_template_names(self):
-        return {
-            "GET": ["account/email_confirm.html"],
-            "POST": ["account/email_confirmed.html"],
-        }[self.request.method]
+        if self.request.method == 'POST':
+            return ["account/email_confirmed.html"]
+        else:
+            return [ "account/email_confirm.html" ]
     
     def get(self, *args, **kwargs):
         try:
             self.object = self.get_object()
         except Http404:
             self.object = None
         ctx = self.get_context_data()
@@ -145,19 +145,15 @@
     
     def get_context_data(self, **kwargs):
         ctx = kwargs
         ctx["confirmation"] = self.object
         return ctx
     
     def get_redirect_url(self):
-        if self.request.user.is_authenticated():
-            return app_settings.EMAIL_CONFIRMATION_AUTHENTICATED_REDIRECT_URL
-        else:
-            return app_settings.EMAIL_CONFIRMATION_ANONYMOUS_REDIRECT_URL
-
+        return get_adapter().get_email_confirmation_redirect_url(self.request)
 
 confirm_email = ConfirmEmailView.as_view()
 
 @login_required
 def email(request, **kwargs):
     form_class = kwargs.pop("form_class", AddEmailForm)
     template_name = kwargs.pop("template_name", "account/email.html")
@@ -206,14 +202,18 @@
                             messages.add_message \
                                 (request, messages.ERROR,
                                  ugettext("You cannot remove your primary"
                                           " e-mail address (%(email)s)")
                                  % { "email": email })
                         else:
                             email_address.delete()
+                            signals.email_removed.send(sender=request.user.__class__,
+                                                       request=request, 
+                                                       user=request.user,
+                                                       email_address=email_address)
                             messages.add_message(request, messages.SUCCESS,
                                 ugettext("Removed e-mail address %(email)s") % {
                                     "email": email,
                                 }
                             )
                             return HttpResponseRedirect(reverse('account_email'))
                     except EmailAddress.DoesNotExist:
```

### Comparing `django-allauth-0.8.3/allauth/account/templatetags/account.py` & `django-allauth-0.9.0/allauth/account/templatetags/account.py`

 * *Files identical despite different names*

### Comparing `django-allauth-0.8.3/allauth/account/management/commands/account_emailconfirmationmigration.py` & `django-allauth-0.9.0/allauth/account/management/commands/account_emailconfirmationmigration.py`

 * *Files identical despite different names*

